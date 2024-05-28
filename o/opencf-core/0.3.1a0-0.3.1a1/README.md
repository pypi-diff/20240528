# Comparing `tmp/opencf_core-0.3.1a0.tar.gz` & `tmp/opencf_core-0.3.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencf_core-0.3.1a0.tar", max compression
+gzip compressed data, was "opencf_core-0.3.1a1.tar", max compression
```

## Comparing `opencf_core-0.3.1a0.tar` & `opencf_core-0.3.1a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     7078 2024-05-08 14:58:19.894394 opencf_core-0.3.1a0/README.md
--rw-r--r--   0        0        0        0 2024-05-08 14:58:19.894394 opencf_core-0.3.1a0/opencf_core/__init__.py
--rw-r--r--   0        0        0    19862 2024-05-23 17:47:40.073650 opencf_core-0.3.1a0/opencf_core/base_converter.py
--rw-r--r--   0        0        0     6430 2024-05-23 17:47:40.073650 opencf_core-0.3.1a0/opencf_core/converter_app.py
--rw-r--r--   0        0        0     1109 2024-05-23 17:46:59.309102 opencf_core-0.3.1a0/opencf_core/exceptions.py
--rw-r--r--   0        0        0    16054 2024-05-23 17:47:40.077650 opencf_core-0.3.1a0/opencf_core/filetypes.py
--rw-r--r--   0        0        0     5891 2024-05-08 14:58:19.894394 opencf_core-0.3.1a0/opencf_core/io_handler.py
--rw-r--r--   0        0        0     3566 2024-05-23 09:27:20.464956 opencf_core-0.3.1a0/opencf_core/logging_config.py
--rw-r--r--   0        0        0     2030 2024-05-23 10:30:58.320136 opencf_core-0.3.1a0/opencf_core/mimes.py
--rw-r--r--   0        0        0      543 2024-05-23 17:46:59.309102 opencf_core-0.3.1a0/opencf_core/utils.py
--rw-r--r--   0        0        0     1110 2024-05-23 17:52:49.677591 opencf_core-0.3.1a0/pyproject.toml
--rw-r--r--   0        0        0     8275 1970-01-01 00:00:00.000000 opencf_core-0.3.1a0/PKG-INFO
+-rw-r--r--   0        0        0     7078 2024-05-08 14:58:19.894394 opencf_core-0.3.1a1/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 14:58:19.894394 opencf_core-0.3.1a1/opencf_core/__init__.py
+-rw-r--r--   0        0        0    19810 2024-05-28 01:21:54.874612 opencf_core-0.3.1a1/opencf_core/base_converter.py
+-rw-r--r--   0        0        0     6372 2024-05-28 01:21:54.842612 opencf_core-0.3.1a1/opencf_core/converter_app.py
+-rw-r--r--   0        0        0     1109 2024-05-23 17:46:59.309102 opencf_core-0.3.1a1/opencf_core/exceptions.py
+-rw-r--r--   0        0        0    21502 2024-05-28 01:21:54.874612 opencf_core-0.3.1a1/opencf_core/filetypes.py
+-rw-r--r--   0        0        0     5891 2024-05-08 14:58:19.894394 opencf_core-0.3.1a1/opencf_core/io_handler.py
+-rw-r--r--   0        0        0     3566 2024-05-23 09:27:20.464956 opencf_core-0.3.1a1/opencf_core/logging_config.py
+-rw-r--r--   0        0        0     2030 2024-05-23 10:30:58.320136 opencf_core-0.3.1a1/opencf_core/mimes.py
+-rw-r--r--   0        0        0      543 2024-05-23 17:46:59.309102 opencf_core-0.3.1a1/opencf_core/utils.py
+-rw-r--r--   0        0        0     1128 2024-05-28 01:22:20.078967 opencf_core-0.3.1a1/pyproject.toml
+-rw-r--r--   0        0        0     8314 1970-01-01 00:00:00.000000 opencf_core-0.3.1a1/PKG-INFO
```

### Comparing `opencf_core-0.3.1a0/README.md` & `opencf_core-0.3.1a1/README.md`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.1a0/opencf_core/base_converter.py` & `opencf_core-0.3.1a1/opencf_core/base_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 
 from abc import ABC, abstractmethod
 from enum import Enum
 from pathlib import Path
 from typing import Any, Iterable, List, Optional, Tuple, Type, Union
 
-from .filetypes import BaseFileType, EmptySuffixError, FileType
+from .filetypes import EmptySuffixError, FileType
 from .io_handler import FileReader, FileWriter, SamePathReader
 from .logging_config import logger
 
 
 class ResolvedInputFile:
     """
     Handles resolving the file type of a given file or folder, managing path adjustments and optional content reading.
@@ -34,15 +34,15 @@
         self,
         path: Union[str, Path],
         is_dir: Optional[bool] = None,
         should_exist: bool = True,
         file_type: Optional[str] = None,
         add_suffix: bool = False,
         read_content: bool = False,
-        filetype_class: Optional[Type[BaseFileType]] = FileType,
+        filetype_class: Optional[Type[FileType]] = FileType,
     ):
         """
         Initializes an instance of ResolvedInputFile with options for type resolution and path modification.
 
         Args:
             path (str): The path to the file or folder.
             is_dir (bool, optional): Specifies if the path is a directory. If None, inferred using pathlib. Defaults to None.
@@ -129,69 +129,73 @@
         """
         if self.path.is_file():
             raise ValueError(
                 f"The specified path '{self.path}' is a file, not a directory."
             )
         # Create directory if it doesn't exist
         self.path.mkdir(exist_ok=True)
-        resolved_file_type = self.filetype_class.from_suffix(file_type, raise_err=True)
+        resolved_file_type, _ = self.filetype_class.from_suffix(
+            file_type, raise_err=True
+        )
         assert resolved_file_type.is_true_filetype()
-        suffix = resolved_file_type.get_suffix()
+        suffix = resolved_file_type.get_one_suffix()
         return resolved_file_type, suffix
 
     def _resolve_file_type(
         self, file_type: Optional[str], read_content: bool, add_suffix: bool
     ):
         """
         Resolves the file type based on given parameters.
 
         Args:
-            file_type (BaseFileType or str, optional): An explicit file type or extension.
+            file_type (FileType or str, optional): An explicit file type or extension.
             read_content (bool): Indicates if file content should be used to help resolve the file type.
             add_suffix (bool): Whether to append the resolved file type's suffix to the file path.
         """
         resolved_file_type = self.__resolve_filetype__(
             file_type, self.path, read_content
         )
         assert resolved_file_type.is_true_filetype()
 
         # Get the suffix corresponding to the resolved file type
-        suffix = resolved_file_type.get_suffix()
+        suffix = resolved_file_type.get_one_suffix()
 
         # Optionally add suffix to the file path
         if add_suffix:
             self.path = self.path.with_suffix(suffix)
 
         return resolved_file_type, suffix
 
     def __resolve_filetype__(
         self, file_type: Optional[str], file_path: Path, read_content: bool
-    ) -> BaseFileType:
+    ) -> FileType:
         """
         Determines the file type, utilizing the provided type, file path, or content as needed.
 
         Args:
-            file_type (BaseFileType or str, optional): An explicit file type or extension.
+            file_type (FileType or str, optional): An explicit file type or extension.
             file_path (str): The path to the file, used if file_type is not provided.
             read_content (bool): Indicates if file content should be used to help resolve the file type.
 
         Returns:
-            BaseFileType: The resolved file type.
+            FileType: The resolved file type.
         """
         if not file_type:
             try:
                 return self.filetype_class.from_path(
                     file_path, read_content=read_content, raise_err=True
-                )
+                )[0]
             except EmptySuffixError:
                 raise ValueError("filepath suffix is emtpy but file_type not set")
 
-        resolved_file_type = self.filetype_class.from_suffix(file_type, raise_err=True)
+        resolved_file_type, _ = self.filetype_class.from_suffix(
+            file_type, raise_err=True
+        )
 
-        file_type_from_path = self.filetype_class.from_path(
+        file_type_from_path, _ = self.filetype_class.from_path(
             file_path, read_content=read_content, raise_err=False
         )
 
         if file_type_from_path.is_true_filetype():
             assert file_type_from_path == resolved_file_type
 
         return resolved_file_type
@@ -328,15 +332,15 @@
             ), f"output_path {output_path} is not a dir while a folder is required for this conversion"
             kwargs["output_folder"] = output_path
         else:
             assert (
                 not output_path.is_dir()
             ), f"output_path {output_path} exists as a dir while a file is required for this conversion"
             # if output_path.is_dir():
-            #     suffix = self.get_supported_output_types().get_suffix()
+            #     suffix = self.get_supported_output_types().get_one_suffix()
             #     output_path = (output_path / "opencf-output").with_suffix(suffix)
             kwargs["output_file"] = output_path
         return kwargs, output_path
 
     def _check_file_types(self):
         """
         Validates that the provided files have acceptable and supported file types for conversion.
@@ -387,78 +391,76 @@
         return cls.get_supported_input_types()
 
     @classmethod
     def get_output_types(cls):
         return cls.get_supported_output_types()
 
     @classmethod
-    def get_supported_input_types(cls) -> Tuple[BaseFileType, ...]:
+    def get_supported_input_types(cls) -> Tuple[FileType, ...]:
         """
         Defines the supported input file types for this converter.
 
         Returns:
-            Tuple[BaseFileType]: The file types supported for input.
+            Tuple[FileType]: The file types supported for input.
         """
         input_types = cls._get_supported_input_types()
 
-        # Check if input_types is a single BaseFileType instance
-        if isinstance(input_types, BaseFileType):
+        # Check if input_types is a single FileType instance
+        if isinstance(input_types, FileType):
             return (input_types,)  # Convert single instance to tuple
 
-        # Check if input_types is an iterable of BaseFileType instances
+        # Check if input_types is an iterable of FileType instances
         input_types = tuple(input_types)
-        if not all(isinstance(input_type, BaseFileType) for input_type in input_types):
+        if not all(isinstance(input_type, FileType) for input_type in input_types):
             raise ValueError("Invalid supported input file type")
 
         return input_types
 
     @classmethod
-    def get_supported_output_types(cls) -> Tuple[BaseFileType, ...]:
+    def get_supported_output_types(cls) -> Tuple[FileType, ...]:
         """
         Defines the supported output file types for this converter.
 
         Returns:
-            Tuple[BaseFileType]: The file types supported for output.
+            Tuple[FileType]: The file types supported for output.
         """
         output_types = cls._get_supported_output_types()
 
-        # Check if output_types is a single BaseFileType instance
-        if isinstance(output_types, BaseFileType):
+        # Check if output_types is a single FileType instance
+        if isinstance(output_types, FileType):
             return (output_types,)  # Convert single instance to tuple
 
-        # Check if output_types is an iterable of BaseFileType instances
+        # Check if output_types is an iterable of FileType instances
         output_types = tuple(output_types)
-        if not all(
-            isinstance(output_type, BaseFileType) for output_type in output_types
-        ):
+        if not all(isinstance(output_type, FileType) for output_type in output_types):
             raise ValueError("Invalid supported output file type")
 
         return output_types
 
     @classmethod
     @abstractmethod
-    def _get_supported_input_types(cls) -> Iterable[BaseFileType]:
+    def _get_supported_input_types(cls) -> Iterable[FileType]:
         """
         Abstract method to define the supported input file types by the converter.
 
         Returns:
-            Iterable[BaseFileType]: The supported input file type.
+            Iterable[FileType]: The supported input file type.
         """
         raise NotImplementedError(
             f"{cls.__name__}._get_supported_input_typess() must be implemented by subclasses."
         )
 
     @classmethod
     @abstractmethod
-    def _get_supported_output_types(cls) -> Iterable[BaseFileType]:
+    def _get_supported_output_types(cls) -> Iterable[FileType]:
         """
         Abstract method to define the supported output file types by the converter.
 
         Returns:
-            Iterable[BaseFileType]: The supported output file type.
+            Iterable[FileType]: The supported output file type.
         """
         raise NotImplementedError(
             f"{cls.__name__}._get_supported_output_typess() must be implemented by subclasses."
         )
 
     @abstractmethod
     def _convert(
```

### Comparing `opencf_core-0.3.1a0/opencf_core/converter_app.py` & `opencf_core-0.3.1a1/opencf_core/converter_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,45 +6,45 @@
 
 from collections import defaultdict
 from itertools import product
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Type
 
 from .base_converter import BaseConverter, ResolvedInputFile
-from .filetypes import BaseFileType, FileType
+from .filetypes import FileType
 from .logging_config import logger
 
 
 class BaseConverterApp:
     """
     Main application class responsible for managing file conversions.
     """
 
     converters: List[Type[BaseConverter]] = []
-    filetype_class: Type[BaseFileType] = FileType
+    filetype_class: Type[FileType] = FileType
 
     def __init__(
         self,
         input_file_paths: List[str],
         input_file_type: Optional[str] = None,
         output_file_path: Optional[str] = None,
         output_file_type: Optional[str] = None,
     ):
         """
         Initializes the BaseConverterApp instance.
 
         Args:
             input_file_paths (List[str]): List of paths to the input files.
-            input_file_type (BaseFileType, optional): The type of the input file. Defaults to None.
+            input_file_type (FileType, optional): The type of the input file. Defaults to None.
             output_file_path (str, optional): The path to the output file. Defaults to None.
-            output_file_type (BaseFileType, optional): The type of the output file. Defaults to None.
+            output_file_type (FileType, optional): The type of the output file. Defaults to None.
         """
 
         self._converter_map: Dict[
-            Tuple[BaseFileType, BaseFileType], List[Type[BaseConverter]]
+            Tuple[FileType, FileType], List[Type[BaseConverter]]
         ] = defaultdict(list)
 
         if not isinstance(input_file_paths, list):
             raise TypeError("input_file_paths sould be a list")
         if len(input_file_paths) == 0:
             raise ValueError("input_file_paths should not be a empty list")
 
@@ -108,15 +108,15 @@
         output_types = converter_class.get_output_types()
 
         # Add the converter pair to the converter map
         for input_type, output_type in product(input_types, output_types):
             self._converter_map[(input_type, output_type)].append(converter_class)
 
     def get_converters_for_conversion(
-        self, input_type: BaseFileType, output_type: BaseFileType
+        self, input_type: FileType, output_type: FileType
     ) -> List[Type[BaseConverter]]:
         """
         Returns a list of converter classes for a given input-output type pair.
 
         Args:
             input_type (str): The input type.
             output_type (str): The output type.
@@ -124,20 +124,20 @@
         Returns:
             List[Type[BaseConverter]]: List of converter classes if found, else an empty list.
         """
         return self._converter_map[(input_type, output_type)]
 
     def get_supported_conversions(
         self,
-    ) -> Tuple[Tuple[BaseFileType, BaseFileType], ...]:
+    ) -> Tuple[Tuple[FileType, FileType], ...]:
         """
         Retrieves the supported conversions.
 
         Returns:
-            Tuple[Tuple[BaseFileType, BaseFileType]]: A tuple of tuples representing supported conversions.
+            Tuple[Tuple[FileType, FileType]]: A tuple of tuples representing supported conversions.
         """
         return tuple(self._converter_map.keys())
 
     def run(self):
         """
         Runs the conversion process.
         """
```

### Comparing `opencf_core-0.3.1a0/opencf_core/exceptions.py` & `opencf_core-0.3.1a1/opencf_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.1a0/opencf_core/filetypes.py` & `opencf_core-0.3.1a1/opencf_core/filetypes.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,382 +8,516 @@
 
 Classes:
 - UnsupportedFileTypeError: Custom exception for handling unsupported file types.
 - EmptySuffixError: Specialized exception for cases where a file's suffix does not provide enough information
                     to determine its type.
 - FileNotFoundError: Raised when a specified file does not exist.
 - MismatchedException: Exception for handling cases where there's a mismatch between expected and actual file attributes.
-- filetype: Enum class that encapsulates various file types supported by the system, providing methods for
-            type determination from file attributes.
+- FileType: Enum class that encapsulates various file types supported by the system, providing methods for
+                type determination from file attributes.
 
 Functions:
 - test_file_type_parsing(): Demonstrates and validates the parsing functionality for various file types.
-- test_file_type_matching(): Tests the matching and validation capabilities of the filetype class.
+- test_file_type_matching(): Tests the matching and validation capabilities of the FileType class.
 
 Dependencies:
 - collections.namedtuple: For defining simple classes for storing MIME type information.
-- enum.Enum: For creating the filetype enumeration.
+- enum.Enum: For creating the FileType enumeration.
 - pathlib.Path: For file path manipulations and checks.
 - opencf_core.mimes.guess_mime_type_from_file: Utility function to guess MIME type from a file path.
+
+Usage Examples:
+```python
+from pathlib import Path
+from mymodule import FileType, EmptySuffixError, UnsupportedFileTypeError
+
+# Example: Determine file type from suffix
+try:
+    file_type, _ = FileType.from_suffix('.txt')
+    print(f'File type: {file_type.name}')
+except (EmptySuffixError, UnsupportedFileTypeError) as e:
+    print(f'Error: {e}')
+
+# Example: Determine file type from MIME type
+try:
+    file_path = Path('/path/to/file.txt')
+    file_type, _ = FileType.from_mimetype(file_path)
+    print(f'File type: {file_type.name}')
+except FileNotFoundError as e:
+    print(f'Error: {e}')
+except UnsupportedFileTypeError as e:
+    print(f'Error: {e}')
+
+# Example: Validate file type by path and content
+file_path = Path('/path/to/file.txt')
+is_valid = FileType.TEXT.is_valid_path(file_path, read_content=True)
+print(f'Is valid: {is_valid}')
+```
 """
+from __future__ import annotations
 
-from abc import ABCMeta, abstractmethod
 from dataclasses import dataclass
-from enum import Enum, EnumMeta
 from pathlib import Path
-from typing import Callable, Dict, Iterable, Tuple, Type, Union
+from typing import TYPE_CHECKING, Dict, Iterable, Tuple, Type, Union
+
+from aenum import extend_enum  # type: ignore
 
 from opencf_core.exceptions import (
     EmptySuffixError,
     MismatchedException,
     UnsupportedFileTypeError,
 )
 
 from .mimes import guess_mime_type_from_file
 
+if TYPE_CHECKING:
+    # this is only processed by MyPy (i.e. not at runtime)
+    from enum import Enum
+else:
+    # this is real runtime code
+    from aenum import Enum
+
 
-# File Type and MIME Type Definitions
 @dataclass(eq=False, frozen=True)
 class MimeType:
+    """Class representing MIME type information.
+
+    Attributes:
+        extensions (Tuple[str, ...]): Tuple of file extensions associated with the MIME type.
+        mime_types (Tuple[str, ...]): Tuple of MIME types.
+        upper_mime_types (Tuple[str, ...]): Tuple of additional MIME types that can be considered equivalent.
+    """
+
     extensions: Tuple[str, ...] = ()
     mime_types: Tuple[str, ...] = ()
     upper_mime_types: Tuple[str, ...] = ()
 
 
-class BaseFileType(ABCMeta, EnumMeta):  # type:ignore
+class FileType(Enum):
+    """Base enumeration for file types, providing methods for type determination and validation.
+
+    Attributes:
+        NOTYPE (MimeType): Represents an undefined file type.
+        TEXT (MimeType): Represents a text file type.
+        UNHANDLED (MimeType): Represents an unhandled file type.
+    """
+
     NOTYPE: MimeType = MimeType()
     TEXT = MimeType(("txt",), ("text/plain",))
     UNHANDLED: MimeType = MimeType()
 
-    __filetype_members__ = {"NOTYPE": NOTYPE, "TEXT": TEXT, "UNHANDLED": UNHANDLED}
-
-    @abstractmethod
     def get_value(self) -> MimeType:
-        pass
-
-    @classmethod
-    def from_mimetype(cls, file_path: Union[str, Path], raise_err: bool = False):
-        pass
-
-    @classmethod
-    def from_path(cls, path: Path, read_content=False, raise_err=False):
-        pass
+        """Returns the `MimeType` associated with the enumeration member.
 
-    @classmethod
-    def from_suffix(cls, suffix: str, raise_err: bool = False):
-        pass
-
-    @abstractmethod
-    def is_true_filetype(self) -> bool:
-        pass
-
-    @abstractmethod
-    def get_suffix(self) -> str:
-        pass
-
-
-class FileTypeMethods(BaseFileType):
-    def get_value(self) -> MimeType:
-        # self.value is defined for Enum subclass instances
+        Returns:
+            MimeType: The MIME type information.
+        """
         return self.value  # type:ignore
 
     @classmethod
     def get_filetypes(cls):
+        """Yields all valid file types in the enumeration."""
         for member in cls:
             if not isinstance(member.get_value(), MimeType):
                 continue
             yield member
 
     @classmethod
-    def from_suffix(cls, suffix: str, raise_err: bool = False):
-        """
-        Determines a filetype from a file's suffix.
+    def clean_suffix(cls, suffix: str) -> str:
+        return suffix.lower().lstrip(".")
+
+    @classmethod
+    def from_suffix(
+        cls, suffix: str, raise_err: bool = False, return_matches: bool = False
+    ) -> Tuple[FileType, Tuple[FileType, ...]]:
+        """Determines a filetype from a file's suffix.
 
         Args:
             suffix (str): The file suffix (extension).
             raise_err (bool, optional): Whether to raise an exception if the type is unhandled. Defaults to False.
+            return_matches (bool, optional): Whether to return a tuple with the first matching filetype and a list of all options. Defaults to False.
 
         Returns:
-            filetype: The determined filetype enumeration member.
+            FileType: The determined filetype enumeration member, or a tuple with the first matching filetype and a list of all options.
 
         Raises:
             EmptySuffixError: If the suffix is empty and raise_err is True.
             UnsupportedFileTypeError: If the file type is unhandled and raise_err is True.
         """
-
-        # get suffix
         suffix = suffix.lower().lstrip(".")
         if not suffix:
             if raise_err:
                 raise EmptySuffixError()
-            return cls.NOTYPE
+            return (cls.NOTYPE, tuple())
 
-        # get a valid member
+        matches = []
         for member in cls.get_filetypes():
             member_value = member.get_value()
             if member_value.extensions and suffix in member_value.extensions:
-                return member
+                if not return_matches:
+                    return (member, tuple())
+                matches.append(member)
 
-        if raise_err:
-            raise UnsupportedFileTypeError(f"Unhandled filetype from suffix={suffix}")
-
-        return cls.UNHANDLED
+        if len(matches) == 0:
+            if raise_err:
+                raise UnsupportedFileTypeError(
+                    f"Unhandled filetype from suffix={suffix}"
+                )
+            return (cls.UNHANDLED, tuple())
+
+        return (
+            (matches[0], tuple())
+            if not return_matches
+            else (matches[0], tuple(matches))
+        )
 
     @classmethod
-    def from_mimetype(cls, file_path: Union[str, Path], raise_err: bool = False):
-        """
-        Determines a filetype from a file's MIME type.
+    def from_mimetype(
+        cls,
+        file_path: Union[str, Path],
+        raise_err: bool = False,
+        return_matches: bool = False,
+    ) -> Tuple[FileType, Tuple[FileType, ...]]:
+        """Determines a filetype from a file's MIME type.
 
         Args:
             file_path (str): The path to the file.
             raise_err (bool, optional): Whether to raise an exception if the type is unhandled. Defaults to False.
+            return_matches (bool, optional): Whether to return a tuple with the first matching filetype and a list of all options. Defaults to False.
 
         Returns:
-            filetype: The determined filetype enumeration member.
+            FileType: The determined filetype enumeration member, or a tuple with the first matching filetype and a list of all options.
 
         Raises:
             FileNotFoundError: If the file does not exist.
             UnsupportedFileTypeError: If the file type is unhandled and raise_err is True.
         """
-
         file = Path(file_path)
 
         if not file.exists():
             raise FileNotFoundError(file_path)
 
         file_mimetype = guess_mime_type_from_file(str(file))
 
+        matches = []
         for member in cls.get_filetypes():
             if (
                 member.get_value().mime_types
                 and file_mimetype in member.get_value().mime_types
             ):
-                return member
+                if not return_matches:
+                    return (member, tuple())
+                matches.append(member)
 
-        if raise_err:
-            raise UnsupportedFileTypeError(
-                f"Unhandled filetype from mimetype={file_mimetype}"
-            )
-        else:
-            return cls.UNHANDLED
+        if len(matches) == 0:
+            if raise_err:
+                raise UnsupportedFileTypeError(
+                    f"Unhandled filetype from mimetype={file_mimetype}"
+                )
+            return (cls.UNHANDLED, tuple())
+
+        return (
+            (matches[0], tuple())
+            if not return_matches
+            else (matches[0], tuple(matches))
+        )
 
     # @classmethod
     # def from_content(cls, path: Path, raise_err=False):
     #     file_path = Path(path)
     #     file_type = get_file_type(file_path)['f_type']
     #     # logger.info(file_type)
     #     return file_type #text/plain, application/json, text/xml, image/png, application/csv, image/gif, ...
     #     member = cls.UNHANDLED
     #     return member
 
     @classmethod
-    def from_path(cls, path: Path, read_content=False, raise_err=False):
-        """
-        Determines the filetype of a file based on its path. Optionally reads the file's content to verify its type.
+    def from_path(
+        cls,
+        path: Union[str, Path],
+        read_content=False,
+        raise_err=False,
+        return_matches=False,
+    ) -> Tuple[FileType, Tuple[FileType, ...]]:
+        """Determines the filetype of a file based on its path. Optionally reads the file's content to verify its type.
 
         Args:
             path (Path): The path to the file.
             read_content (bool, optional): If True, the method also checks the file's content to determine its type.
                                            Defaults to False.
             raise_err (bool, optional): If True, raises exceptions for unsupported types or when file does not exist.
                                         Defaults to False.
+            return_matches (bool, optional): Whether to return a tuple with the first matching filetype and a list of all options. Defaults to False.
 
         Returns:
-            filetype: The determined filetype enumeration member based on the file's suffix and/or content.
+            FileType: The determined filetype enumeration member based on the file's suffix and/or content, or a tuple with the first matching filetype and a list of all options.
 
         Raises:
             FileNotFoundError: If the file does not exist when attempting to read its content.
             UnsupportedFileTypeError: If the file type is unsupported and raise_err is True.
             AssertionError: If there is a mismatch between the file type determined from the file's suffix and its content.
         """
         file_path = Path(path)
 
-        raise_err1 = raise_err and (not read_content)
-        raise_err2 = raise_err
+        raise_err_suffix: bool = raise_err and (not read_content)
+        raise_err_mimetype: bool = raise_err
 
         # get member from suffix
-        member1 = cls.from_suffix(file_path.suffix, raise_err=raise_err1)
+        filetype_from_suffix, suffix_matches = cls.from_suffix(
+            file_path.suffix, raise_err=raise_err_suffix, return_matches=True
+        )
 
         # if we're not checking the file content, return
         if not read_content:
-            return member1
+            return filetype_from_suffix, suffix_matches
 
-        # the file should exists for content reading
+        # the file should exist for content reading
         if not file_path.exists():
             raise FileNotFoundError(f"File '{file_path}' does not exist.")
 
         # get member from content
-        member2 = cls.from_mimetype(file_path, raise_err=raise_err2)
+        filetype_from_mimetype, mimetype_matches = cls.from_mimetype(
+            file_path, raise_err=raise_err_mimetype, return_matches=True
+        )
 
-        # if suffix didnt give a filetype, use the one from content
-        if not member1.is_true_filetype():
-            return member2
+        # combine results from both methods
 
-        assert (
-            member1 == member2
-        ), f"file type from suffix ({member1}) mismatch with filepath from path({member2})"
+        # if suffix didn't give a filetype, use the one from content
+        if filetype_from_suffix.is_true_filetype():
+            return (
+                (filetype_from_suffix, tuple())
+                if not return_matches
+                else (filetype_from_mimetype, mimetype_matches)
+            )
 
-        return member1
+        # if content mimetype didn't give a filetype, use the one from suffix
+        if filetype_from_mimetype.is_true_filetype():
+            return (
+                (filetype_from_suffix, tuple())
+                if not return_matches
+                else (filetype_from_suffix, suffix_matches)
+            )
+
+        # find common matches
+        common_members = tuple(m for m in suffix_matches if m in mimetype_matches)
+
+        if len(common_members) == 0:
+            if raise_err:
+                raise AssertionError(
+                    f"file type from suffix ({suffix_matches}) mismatch with file type from content ({mimetype_matches})"
+                )
+            return (cls.NOTYPE, tuple())
+
+        return (
+            (common_members[0], tuple())
+            if not return_matches
+            else (common_members[0], common_members)
+        )
 
     def is_true_filetype(self) -> bool:
-        """
-        Determines if the filetype instance represents a supported file type based on the presence of defined extensions.
+        """Determines if the filetype instance represents a supported file type based on the presence of defined extensions.
 
         Returns:
             bool: True if the filetype has at least one associated file extension, False otherwise.
         """
         return len(self.get_value().extensions) != 0
 
-    def get_suffix(self) -> str:
+    def get_one_suffix(self) -> str:
         """
         Retrieves the primary file extension associated with the filetype.
 
         Returns:
             str: The primary file extension for the filetype, prefixed with a period.
                  Returns an empty string if the filetype does not have an associated extension.
         """
         if not self.is_true_filetype():
             return ""
         ext = self.get_value().extensions[0]
         return f".{ext}"
 
-    def is_valid_suffix(self, suffix: str, raise_err=False):
+    def get_one_mimetype(self) -> str:
         """
-        Validates whether a given file extension matches the filetype's expected extensions.
+        Retrieves the primary mimetype associated with the filetype.
+
+        Returns:
+            Mimetype: The primary mimetype for the filetype.
+                 Returns an empty string if the filetype does not have an associated extension.
+        """
+        if not self.is_true_filetype():
+            return ""
+        return self.get_value().mime_types[0]
+
+    def is_valid_suffix(self, suffix: str, raise_err=False):
+        """Validates whether a given file extension matches the filetype's expected extensions.
 
         Args:
             suffix (str): The file extension to validate, including the leading period (e.g., ".txt").
             raise_err (bool, optional): If True, raises a MismatchedException for invalid extensions.
                                         Defaults to False.
 
         Returns:
             bool: True if the suffix matches one of the filetype's extensions, False otherwise.
 
         Raises:
-            MismatchedException: If the suffix does not match and raise_err is True.
+            MismatchedException: If the suffix does not match the filetype's extensions and raise_err is True.
         """
-        _val = self.from_suffix(suffix=suffix)
-        is_valid = _val == self
-        if raise_err and not is_valid:
+        if not self.is_true_filetype():
+            return False
+        suffix = self.__class__.clean_suffix(suffix)
+        if suffix in self.get_value().extensions:
+            return True
+        if raise_err:
             raise MismatchedException(
-                f"suffix ({suffix})", _val, self.get_value().extensions
+                f"filetype ({self.name}) mismatch with suffix ({suffix})",
+                suffix,
+                self.get_one_suffix(),
             )
-        return is_valid
+        return False
 
-    def is_valid_path(self, path: Path, raise_err=False, read_content=False):
-        """
-        Validates whether the file at a given path matches the filetype, optionally checking the file's content.
+    def is_valid_path(
+        self, file_path: Union[str, Path], read_content=False, raise_err=False
+    ):
+        """Validates the filetype of a given file path. Optionally reads the file's content to verify its type.
 
         Args:
-            path (Path): The path to the file to validate.
-            raise_err (bool, optional): If True, raises a MismatchedException for a mismatching file type.
-                                        Defaults to False.
-            read_content (bool, optional): If True, also validates the file's content type against the filetype.
+            file_path (Union[str, Path]): The file path to validate.
+            read_content (bool, optional): If True, the method also checks the file's content to validate its type.
                                            Defaults to False.
+            raise_err (bool, optional): If True, raises exceptions for mismatched or unsupported types.
+                                        Defaults to False.
 
         Returns:
-            bool: True if the file's type matches the filetype, based on its path and optionally its content.
-                  False otherwise.
+            bool: True if the file path's type matches the filetype, False otherwise.
 
         Raises:
-            MismatchedException: If the file's type does not match and raise_err is True.
+            AssertionError: If there is a mismatch between the file type determined from the file's suffix and its content.
+            MismatchedException: If the file type determined from the file's suffix or content does not match the filetype.
         """
-        _val = self.from_path(path, read_content=read_content)
-        is_valid = _val == self
+        _val, matches = self.from_path(
+            file_path, read_content=read_content, return_matches=True
+        )
+        is_valid = (self == _val) if not self.is_true_filetype() else (self in matches)
         if raise_err and not is_valid:
             raise MismatchedException(
-                f"suffix/mime-type ({path})", _val, self.get_value()
+                f"suffix/mime-type ({file_path})", _val, self.get_value()
             )
         return is_valid
 
-    def is_valid_mime_type(self, path: Path, raise_err=False):
+    def is_valid_mimetype(self, file_mimetype: str, raise_err=False):
+        """Validates whether a given MIME type matches the filetype's expected MIME types.
+
+        Args:
+            file_mimetype (str): The MIME type to validate.
+            raise_err (bool, optional): If True, raises a MismatchedException for invalid MIME types.
+                                        Defaults to False.
+
+        Returns:
+            bool: True if the MIME type matches one of the filetype's MIME types, False otherwise.
+
+        Raises:
+            MismatchedException: If the MIME type does not match the filetype's MIME types and raise_err is True.
+        """
+        if not self.is_true_filetype():
+            return False
+        if file_mimetype in self.get_value().mime_types:
+            return True
+        if raise_err:
+            raise MismatchedException(
+                f"filetype ({self.name}) mismatch with mimetype ({file_mimetype})",
+                self.get_one_mimetype(),
+                file_mimetype,
+            )
+        return False
+
+    def is_valid_mime_type(self, file_path: Path, raise_err=False):
         """
         Validates whether the MIME type of the file at the specified path aligns with the filetype's expected MIME types.
 
         This method first determines the filetype based on the file's actual MIME type (determined by reading the file's content)
         and then checks if this determined filetype matches the instance calling this method. Special consideration is given to
         filetype.TEXT, where a broader compatibility check is performed due to the generic nature of text MIME types.
 
         Args:
-            path (Path): The path to the file whose MIME type is to be validated.
+            file_path (Path): The path to the file whose MIME type is to be validated.
             raise_err (bool, optional): If True, a MismatchedException is raised if the file's MIME type does not match
                                         the expected MIME types of the filetype instance. Defaults to False.
 
         Returns:
             bool: True if the file's MIME type matches the expected MIME types for this filetype instance or if special
                 compatibility conditions are met (e.g., for filetype.TEXT with "text/plain"). Otherwise, False.
 
         Raises:
             MismatchedException: If raise_err is True and the file's MIME type does not match the expected MIME types
                                 for this filetype instance, including detailed information about the mismatch.
         """
-        _val = self.from_mimetype(path)
-        is_valid = _val == self
+        _val, matches = self.from_mimetype(file_path, return_matches=True)
+        is_valid = (self == _val) if not self.is_true_filetype() else (self in matches)
 
         # many things can be text/plain
-        if _val == self.TEXT and "text/plain" in self.get_value().upper_mime_types:
+        if (self.TEXT in matches) and "text/plain" in self.get_value().upper_mime_types:
             is_valid = True
 
         if raise_err and not is_valid:
             raise MismatchedException(
-                f"content-type({path})", _val, self.get_value().mime_types
+                f"content-type({file_path})", _val, self.get_value().mime_types
             )
         return is_valid
 
 
-def dd(cls: Type):
-    joined: Dict[str, MimeType] = {}
+def extract_enum_members(enum_cls: Type) -> Dict[str, MimeType]:
+    """Extracts MimeType instances from an enum class.
+
+    Args:
+        enum_cls (Type): The enum class.
+
+    Returns:
+        Dict[str, MimeType]: Dictionary of MimeType instances keyed by enum member names.
+    """
+    extracted_members: Dict[str, MimeType] = {}
     items: Iterable
 
-    # Copy values from the inherited enum
-    if issubclass(cls, Enum):
-        items = ((item.name, item.value) for item in cls)
+    if issubclass(enum_cls, FileType):
+        enum_cls = enum_cls
+
+    if issubclass(enum_cls, Enum):
+        items = ((item.name, item.value) for item in enum_cls)
     else:
-        assert hasattr(cls, "__filetype_members__")
-        filetype_members: Dict[str, MimeType] = cls.__filetype_members__
+        assert hasattr(enum_cls, "__filetype_members__")
+        filetype_members: Dict[str, MimeType] = enum_cls.__filetype_members__
         assert isinstance(filetype_members, dict)
         items = filetype_members.items()
 
     # Copy values from the added enum
     for item_name, item_value in items:
         # Make sure the value is of the inherited enum type
         assert isinstance(item_value, MimeType)
-        joined[item_name] = item_value
-
-    return joined
+        extracted_members[item_name] = item_value
 
+    return extracted_members
 
-def extend_filetype_enum(
-    inherited_enum: Union[Type[Enum], Type[BaseFileType]],
-) -> Callable[[Union[Type[Enum], Type[BaseFileType]]], Type[Enum]]:
-    def wrapper(added_enum: Union[Type[Enum], Type[BaseFileType]]) -> Type[Enum]:
-        # Create a dictionary to hold the merged enum values
-        joined = {}
-
-        joined.update(dd(inherited_enum))
-        joined.update(dd(added_enum))
-
-        # Create a new Enum class with the merged values$
-        new_enum = Enum(added_enum.__name__, joined)  # type: ignore
-
-        # users can override/add enum members, methods, class methods in the added enum
-        methods = tuple(inherited_enum.__dict__.items()) + tuple(
-            added_enum.__dict__.items()
-        )
-
-        # Copy methods and class methods from the inherited enum
-        for method_name, method in methods:
-            if callable(method):
-                setattr(new_enum, method_name, method)
-            if isinstance(method, classmethod):
-                setattr(new_enum, method_name, method)
 
-        return new_enum
+def extend_filetype_enum(added_enum: Type[Enum]) -> None:
+    """Extends the BaseFileType enumeration with members from another enumeration.
 
-    return wrapper
+    Args:
+        added_enum (Type[Enum]): The enum class to extend BaseFileType with.
+    """
+    inherited_enum = FileType
+
+    # Add new members from added_enum to inherited_enum
+    for name, member in added_enum.__members__.items():
+        extend_enum(inherited_enum, name, member.value)
+
+    # Copy methods from inherited_enum and added_enum to the new class
+    for method_name, method in {
+        **added_enum.__dict__,
+        **inherited_enum.__dict__,
+    }.items():
+        if callable(method) or isinstance(method, classmethod):
+            setattr(inherited_enum, method_name, method)
 
 
 class FileTypeExamples(Enum):
     """Enumeration of supported file types with methods for type determination and validation."""
 
     CSV = MimeType(("csv",), ("text/csv",), ("text/plain",))
     MARKDOWN = MimeType(("md",), ("text/markdown",), ("text/plain",))
@@ -406,17 +540,8 @@
     PDF = MimeType(("pdf",), ("application/pdf",))
     IMAGE = MimeType(("jpg", "jpeg", "png"), ("image/jpeg", "image/png"))
     GIF = MimeType(("gif",), ("image/gif",))
     VIDEO = MimeType(("mp4", "avi"), ("video/mp4", "video/x-msvideo"))
     XML = MimeType(("xml",), ("application/xml", "text/xml"))
 
 
-# add an enum that contains members
-# it does need to be an enum but it is easier to define members in a Enum subclass
-# than using __filetype_members__ to list predifined mimetypes
-@extend_filetype_enum(FileTypeExamples)
-# add an subclass of BaseFileType that implements methods i use in other modules,
-# on instances of mixin(FileTypeExamples, FileTypeMethods) (like FileType)
-@extend_filetype_enum(FileTypeMethods)
-class FileType(FileTypeMethods):
-    # __filetype_members__: Dict[str, MimeType] = {}
-    pass
+extend_filetype_enum(FileTypeExamples)
```

### Comparing `opencf_core-0.3.1a0/opencf_core/io_handler.py` & `opencf_core-0.3.1a1/opencf_core/io_handler.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.1a0/opencf_core/logging_config.py` & `opencf_core-0.3.1a1/opencf_core/logging_config.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.1a0/opencf_core/mimes.py` & `opencf_core-0.3.1a1/opencf_core/mimes.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.1a0/opencf_core/utils.py` & `opencf_core-0.3.1a1/opencf_core/utils.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.1a0/pyproject.toml` & `opencf_core-0.3.1a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "opencf-core"
 packages = [
     {include = "opencf_core"}
 ]
-version = "0.3.1a0"
+version = "0.3.1a1"
 description = "A robust framework for handling file conversion tasks in Python"
 authors = ["Hermann Agossou <agossouhermann7@gmail.com>"]
 readme = "README.md"
 maintainers = [
     "Hermann Agossou <agossouhermann7@gmail.com>"
 ]
 license = "MIT"
@@ -21,14 +21,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 python-magic = "^0.4.27"
+aenum = "^3.1.15"
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.10.2"
 black = "^23.0.0"
 flake8 = "^5.0.0"
 mypy = "^1.4.0"
```

### Comparing `opencf_core-0.3.1a0/PKG-INFO` & `opencf_core-0.3.1a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencf-core
-Version: 0.3.1a0
+Version: 0.3.1a1
 Summary: A robust framework for handling file conversion tasks in Python
 Home-page: https://github.com/Hermann-web/opencf-core
 License: MIT
 Keywords: file conversion,data processing,file formats
 Author: Hermann Agossou
 Author-email: agossouhermann7@gmail.com
 Maintainer: Hermann Agossou
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: aenum (>=3.1.15,<4.0.0)
 Requires-Dist: python-magic (>=0.4.27,<0.5.0)
 Project-URL: Documentation, https://opencf-core.readthedocs.io
 Project-URL: Repository, https://github.com/Hermann-web/opencf-core
 Description-Content-Type: text/markdown
 
 # OpenCF Core: The File Convertion Framework
```

