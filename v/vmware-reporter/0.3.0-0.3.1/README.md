# Comparing `tmp/vmware_reporter-0.3.0-py3-none-any.whl.zip` & `tmp/vmware_reporter-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,24 @@
-Zip file size: 36666 bytes, number of entries: 18
--rw-rw-rw-  2.0 fat    31153 b- defN 24-May-23 17:26 vmware_reporter/__init__.py
--rw-rw-rw-  2.0 fat     3466 b- defN 24-May-23 10:33 vmware_reporter/__main__.py
--rw-rw-rw-  2.0 fat      427 b- defN 24-May-23 17:27 vmware_reporter/_version.py
--rw-rw-rw-  2.0 fat     1447 b- defN 24-May-23 15:52 vmware_reporter/autoreport.py
--rw-rw-rw-  2.0 fat      844 b- defN 24-May-23 12:13 vmware_reporter/customfield.py
--rw-rw-rw-  2.0 fat    18826 b- defN 24-May-23 17:23 vmware_reporter/datastore.py
--rw-rw-rw-  2.0 fat     2547 b- defN 24-May-23 17:25 vmware_reporter/dump.py
--rw-rw-rw-  2.0 fat     4034 b- defN 24-May-23 16:52 vmware_reporter/host.py
--rw-rw-rw-  2.0 fat     7968 b- defN 24-May-23 17:24 vmware_reporter/inventory.py
--rw-rw-rw-  2.0 fat     5971 b- defN 24-May-23 12:16 vmware_reporter/net.py
--rw-rw-rw-  2.0 fat      235 b- defN 24-May-23 11:12 vmware_reporter/settings.py
--rw-rw-rw-  2.0 fat    54717 b- defN 24-May-23 12:24 vmware_reporter/vm.py
--rw-rw-rw-  2.0 fat     1098 b- defN 24-May-23 17:27 vmware_reporter-0.3.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     3435 b- defN 24-May-23 17:27 vmware_reporter-0.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 17:27 vmware_reporter-0.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       66 b- defN 24-May-23 17:27 vmware_reporter-0.3.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       16 b- defN 24-May-23 17:27 vmware_reporter-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1529 b- defN 24-May-23 17:27 vmware_reporter-0.3.0.dist-info/RECORD
-18 files, 137871 bytes uncompressed, 34150 bytes compressed:  75.2%
+Zip file size: 46825 bytes, number of entries: 22
+-rw-r--r--  2.0 unx    36933 b- defN 24-May-28 15:03 vmware_reporter/__init__.py
+-rw-r--r--  2.0 unx     3757 b- defN 24-May-28 15:00 vmware_reporter/__main__.py
+-rw-r--r--  2.0 unx      411 b- defN 24-May-28 15:36 vmware_reporter/_version.py
+-rw-r--r--  2.0 unx     1992 b- defN 24-May-28 15:29 vmware_reporter/autoreport.py
+-rw-r--r--  2.0 unx     3307 b- defN 24-May-28 12:26 vmware_reporter/cluster.py
+-rw-r--r--  2.0 unx      866 b- defN 24-May-28 12:26 vmware_reporter/customvalue.py
+-rw-r--r--  2.0 unx    18360 b- defN 24-May-28 12:26 vmware_reporter/datastore.py
+-rw-r--r--  2.0 unx     2520 b- defN 24-May-28 12:26 vmware_reporter/dump.py
+-rw-r--r--  2.0 unx     3991 b- defN 24-May-28 12:26 vmware_reporter/host.py
+-rw-r--r--  2.0 unx     8160 b- defN 24-May-28 12:26 vmware_reporter/inventory.py
+-rw-r--r--  2.0 unx     5792 b- defN 24-May-28 12:26 vmware_reporter/net.py
+-rw-r--r--  2.0 unx    14413 b- defN 24-May-28 12:26 vmware_reporter/perf.py
+-rw-r--r--  2.0 unx     3255 b- defN 24-May-28 12:26 vmware_reporter/resourcepool.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-28 12:13 vmware_reporter/settings.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-28 12:26 vmware_reporter/tag.py
+-rw-r--r--  2.0 unx    60990 b- defN 24-May-28 15:11 vmware_reporter/vm.py
+-rw-r--r--  2.0 unx     1079 b- defN 24-May-28 15:36 vmware_reporter-0.3.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     4147 b- defN 24-May-28 15:36 vmware_reporter-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-28 15:36 vmware_reporter-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 24-May-28 15:36 vmware_reporter-0.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 24-May-28 15:36 vmware_reporter-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1860 b- defN 24-May-28 15:36 vmware_reporter-0.3.1.dist-info/RECORD
+22 files, 174646 bytes uncompressed, 43801 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -6,15 +6,18 @@
 
 Filename: vmware_reporter/_version.py
 Comment: 
 
 Filename: vmware_reporter/autoreport.py
 Comment: 
 
-Filename: vmware_reporter/customfield.py
+Filename: vmware_reporter/cluster.py
+Comment: 
+
+Filename: vmware_reporter/customvalue.py
 Comment: 
 
 Filename: vmware_reporter/datastore.py
 Comment: 
 
 Filename: vmware_reporter/dump.py
 Comment: 
@@ -24,32 +27,41 @@
 
 Filename: vmware_reporter/inventory.py
 Comment: 
 
 Filename: vmware_reporter/net.py
 Comment: 
 
+Filename: vmware_reporter/perf.py
+Comment: 
+
+Filename: vmware_reporter/resourcepool.py
+Comment: 
+
 Filename: vmware_reporter/settings.py
 Comment: 
 
+Filename: vmware_reporter/tag.py
+Comment: 
+
 Filename: vmware_reporter/vm.py
 Comment: 
 
-Filename: vmware_reporter-0.3.0.dist-info/LICENSE.txt
+Filename: vmware_reporter-0.3.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vmware_reporter-0.3.0.dist-info/METADATA
+Filename: vmware_reporter-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: vmware_reporter-0.3.0.dist-info/WHEEL
+Filename: vmware_reporter-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: vmware_reporter-0.3.0.dist-info/entry_points.txt
+Filename: vmware_reporter-0.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: vmware_reporter-0.3.0.dist-info/top_level.txt
+Filename: vmware_reporter-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: vmware_reporter-0.3.0.dist-info/RECORD
+Filename: vmware_reporter-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vmware_reporter/__init__.py

```diff
@@ -1,858 +1,1030 @@
-"""
-Top-level API of vmware-reporter library.
-"""
-from __future__ import annotations
-
-import json
-import logging
-import os
-import re
-from collections.abc import Callable, Iterator
-from configparser import ConfigParser
-from contextlib import nullcontext
-from datetime import date
-from inspect import signature
-from io import IOBase
-from pathlib import Path
-from types import (BuiltinFunctionType, BuiltinMethodType, FunctionType,
-                   MethodType)
-from typing import Any, Literal, TypeVar, overload
-from uuid import UUID
-
-from pyVim.connect import Disconnect, SmartConnect
-from pyVmomi import vim, vmodl
-from pyVmomi.VmomiSupport import _managedDefMap
-from zut import (ExtendedJSONEncoder, Filters, MessageError,
-                 iter_dicts_from_csv, resolve_host)
-from zut.excel import ExcelWorkbook, is_excel_path, split_excel_path
-
-from .settings import CONFIG, CONFIG_SECTION
-
-__prog__ = 'vmware-reporter'
-
-try:
-    # Version generated by setuptools_scm during build
-    from ._version import __version__, __version_tuple__
-except ImportError:
-    __version__ = None
-    __version_tuple__ = None
-
-_logger = logging.getLogger(__name__)
-
-T_Obj = TypeVar('T_Obj', bound=vim.ManagedEntity)
-
-
-class VCenterClient:
-    """
-    Main entry point of the library to retrieve VMWare managed objects and interact with them. 
-    """
-    def __init__(self, env: str = None, *, host: str = None, user: str = None, password: str = None, no_ssl_verify: bool = None, config: ConfigParser = None, section: str = None):
-        """
-        Create a new vCenter client.
-
-        If `host`, `user`, `password` or `no_ssl_verify` options are not provided, they are read from configuration file
-        in section `[vmware-reporter]` (or `[vmware-reporter:{name}]` if `name` is given).
-
-        :param env: An optional name to distinguish between several vCenters.
-        :param host: Host name of the vCenter.
-        :param user: Name of the vCenter user having access to the API.
-        :param password: Password of the vCenter user having access to the API.
-        """        
-        if not config:
-            config = CONFIG
-        if not section:
-            section = CONFIG_SECTION
-        
-        if not env:
-            envs = VCenterClient.get_configured_envs(config=config, section=section)
-            if len(envs) > 1:
-                raise MessageError(f"Name of the environment / VCenter to use must be provided. Available: {', '.join(envs) if envs else 'none'}.")
-            elif len(envs) == 1:
-                env = envs[0]
-            else:
-                raise MessageError(f"No VCenter client configured.")
-        self.env = env or 'default'
-
-        full_section = section + ('' if env == 'default' else f':{env}')
-        self.host = host if host is not None else config.get(full_section, 'host')
-        self.user = user if user is not None else config.get(full_section, 'user')
-        self.password = password if password is not None else config.get(full_section, 'password')
-        self.no_ssl_verify = no_ssl_verify if no_ssl_verify is not None else config.getboolean(full_section, 'no_ssl_verify', fallback=False)
-        
-        self.logger = logging.getLogger(f'{self.__class__.__module__}.{self.__class__.__qualname__}' + ('' if env == 'default' else f'.{self.env}'))
-
-
-    #region Enter/connect and exit/close
-
-    def __enter__(self):
-        self.connect()
-        return self
-
-
-    def __exit__(self, exc_type = None, exc_value = None, exc_traceback = None):
-        self.close()
-
-
-    def connect(self):
-        addrs = resolve_host(self.host, timeout=2.0)
-        if not addrs:
-            raise ValueError(f"Cannot resolve host name \"{self.host}\"")
-        
-        addr = addrs[0]
-        self.logger.debug(f"Connect to {addr} ({self.host}) with user {self.user}")
-
-        options = {}
-        if 'httpConnectionTimeout' in signature(SmartConnect).parameters:
-            # Introduced in pyVmomi 8.0.0.1 (see https://github.com/vmware/pyvmomi/issues/627)
-            options['httpConnectionTimeout'] = 5.0
-
-        self._service_instance = SmartConnect(host=self.host, user=self.user, pwd=self.password, disableSslCertValidation=self.no_ssl_verify, **options)
-
-
-    def close(self):
-        try:
-            Disconnect(self._service_instance)
-        except AttributeError:
-            pass
-    
-
-    @property
-    def service_instance(self) -> vim.ServiceInstance:
-        try:
-            return self._service_instance
-        except AttributeError:
-            pass
-
-        self.connect()
-        return self._service_instance
-
-
-    @property
-    def service_content(self) -> vim.ServiceInstanceContent:
-        try:
-            return self._service_content
-        except AttributeError:
-            pass
-
-        self._service_content = self.service_instance.RetrieveContent()
-        return self._service_content
-
-    #endregion
-
-
-    #region Retrieve managed objects
-
-    @property
-    def datacenter(self):
-        try:
-            return self._datacenter
-        except AttributeError:
-            pass
-
-        datacenters = self.get_objs(vim.Datacenter)
-        if not datacenters:
-            raise ValueError(f"Datacenter not found")
-        if len(datacenters) > 1:
-            raise ValueError(f"Several datacenter found")
-        self._datacenter = datacenters[0]
-        return self._datacenter
-
-
-    def get_obj(self, type: type[T_Obj], search: list[str|re.Pattern]|str|re.Pattern|UUID, *, normalize: bool = False, key: Literal['name', 'ref', 'uuid', 'bios_uuid'] = 'name') -> T_Obj:
-        """
-        Find a single VMWare managed object.
-
-        Raise KeyError if not found or several found.
-        """
-        if key in ['uuid', 'bios_uuid']:
-            if not isinstance(search, (UUID,str)):
-                raise TypeError(f"specs must be UUID or str for key {key}, got {type(search).__name__}")
-            
-            if isinstance(search, UUID):
-                uuid = search
-            else:
-                uuid = UUID(search)
-
-            obj = None
-            
-            if key == 'bios_uuid':
-                # NOTE: uuid is "BIOS UUID". Seems to match the end of `sudo cat /sys/class/dmi/id/product_uuid`.
-                if type == vim.VirtualMachine:
-                    obj = self._find_by_uuid(uuid, for_vm=True, instance_uuid=False)
-                else:
-                    raise ValueError(f"key '{key}' can be used only for virtual machines")
-                
-            else:
-                if type == vim.VirtualMachine:
-                    obj = self._find_by_uuid(uuid, for_vm=True, instance_uuid=True)
-                elif type == vim.HostSystem:
-                    obj = self._find_by_uuid(uuid, for_vm=False, instance_uuid=False)
-                else:
-                    raise ValueError(f"key '{key}' can be used only for virtual machines or host systems")
-
-            if obj:
-                return obj
-            else:
-                raise KeyError(f"Not found: {search} (type: {type.__name__})")
-
-        else:
-            iterator = self.iter_objs(types=type, search=search, normalize=normalize, key=key)
-            try:
-                found = next(iterator)
-            except StopIteration:
-                raise KeyError(f"Not found: {search} (type: {type.__name__})")
-            
-            try:
-                next(iterator)
-                raise KeyError(f"Several found: {search} (type: {type.__name__})")
-            except StopIteration:
-                pass
-            return found
-            
-
-    def _find_by_uuid(self, uuid: UUID|str, for_vm: bool, instance_uuid: bool):
-        if isinstance(uuid, UUID):
-            uuid = str(uuid)
-        
-        for datacenter in self.iter_objs(vim.Datacenter):
-            obj = self.service_content.searchIndex.FindByUuid(datacenter, uuid, vmSearch=for_vm, instanceUuid=instance_uuid)
-            if obj:
-                return obj
-
-
-    @overload
-    def get_objs(self, types: type[T_Obj], search: list[str|Path|re.Pattern]|str|Path|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name', sort_key: str|list[str]|Callable = None) -> list[T_Obj]:
-        ...
-
-    def get_objs(self, types: list[type|str]|type|str = None, search: list[str|Path|re.Pattern]|str|Path|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name', sort_key: str|list[str]|Callable = None):        
-        """
-        List VMWare managed objects matching the given search.
-        """
-        objs = [obj for obj in self.iter_objs(types, search, normalize=normalize, key=key)]
-
-        if sort_key:
-            if isinstance(sort_key, str):
-                sort_key = [sort_key]
-
-            if isinstance(sort_key, list):
-                sort_func = lambda obj: [getattr(obj, attr) for attr in sort_key]
-            else:
-                sort_func = sort_key
-
-            objs.sort(key=sort_func)
-
-        return objs
-
-
-    @overload
-    def iter_objs(self, types: type[T_Obj], search: list[str|Path|re.Pattern]|str|Path|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name') -> Iterator[T_Obj]:
-        ...
-
-    def iter_objs(self, types: list[type|str]|type|str = None, search: list[str|Path|re.Pattern]|str|Path|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name'):
-        """
-        Iterate over VMWare managed objects matching the given search.
-        """
-        # Expand search from CSV or Excel files if search ends with '.csv' or '.xlsx'
-        search = _expand_search_from_files(search, key=key)
-
-        # Prepare value filter
-        filters = Filters(search, normalize=normalize)
-
-        # Prepare types
-        if not types:
-            types = []
-        elif isinstance(types, (str,type)):
-            types = [types]
-        
-        types = [self.parse_obj_type(_type) for _type in types]
-
-        # Search using a container view
-        view = None
-        try:
-            view = self.service_content.viewManager.CreateContainerView(self.service_content.rootFolder, types, recursive=True)
-
-            for obj in view.view:
-                if self._obj_matches(obj, key, filters):
-                    yield obj
-        finally:
-            if view:
-                view.Destroy()
-
-
-    def _obj_matches(self, obj: vim.ManagedEntity, key: Literal['name', 'ref'], filters: Filters):
-        if not filters:
-            return True
-        
-        if key == 'name':
-            try:
-                value = obj.name
-            except vim.fault.NoPermission:
-                return False
-            
-        elif key == 'ref':
-            value = get_obj_ref(obj)
-            
-        else:
-            raise ValueError(f"key not supported: {key}")
-        
-        return filters.matches(value)
-
-    #endregion
-
-
-    #region Instance helpers
-
-    @property
-    def cookie(self) -> dict:
-        try:
-            return self._cookie
-        except AttributeError:
-            pass
-    
-        # Get the cookie built from the current session
-        client_cookie = self.service_instance._stub.cookie
-
-        # Break apart the cookie into it's component parts
-        cookie_name = client_cookie.split("=", 1)[0]
-        cookie_value = client_cookie.split("=", 1)[1].split(";", 1)[0]
-        cookie_path = client_cookie.split("=", 1)[1].split(";", 1)[1].split(
-            ";", 1)[0].lstrip()
-        cookie_text = " " + cookie_value + "; $" + cookie_path
-
-        # Make a cookie
-        self._cookie = dict()
-        self._cookie[cookie_name] = cookie_text
-        return self._cookie
-
-
-    def wait_for_task(self, tasks: vim.Task|list[vim.Task]|dict[vim.Task,Any]):
-        """
-        Given a service instance and tasks, return after all the tasks are complete.
-        - `tasks`: a task, a list of tasks, or a dict associating task to log prefixes.
-        """
-        task_list: list[vim.Task] = []
-        log_prefixes: dict[vim.Task,Any] = {}
-        if isinstance(tasks, dict):
-            log_prefixes = tasks
-            for task in tasks.keys():
-                if not isinstance(task, vim.Task):
-                    raise TypeError(f"Invalid dict key: {task} (type {type(task).__name__}, expected vim.Task)")
-                task_list.append(task)
-        elif isinstance(tasks, list):
-            for task in tasks:
-                if not isinstance(task, vim.Task):
-                    raise TypeError(f"Invalid list element: {task} (type {type(task).__name__}, expected vim.Task)")
-                task_list.append(task)
-        elif isinstance(tasks, vim.Task):
-            task_list.append(tasks)
-        else:
-            raise TypeError(f"Invalid argument: {task} (type {type(task).__name__}, expected vim.Task)")
-        
-        # Create filter
-        obj_specs = [vmodl.query.PropertyCollector.ObjectSpec(obj=task) for task in task_list]   
-        property_spec = vmodl.query.PropertyCollector.PropertySpec(type=vim.Task, pathSet=[], all=True)
-        filter_spec = vmodl.query.PropertyCollector.FilterSpec(objectSet=obj_specs, propSet=[property_spec])
-        pc = self.service_instance.content.propertyCollector
-        pc_filter = pc.CreateFilter(filter_spec, True)
-
-        task_failures = 0
-        try:
-            remaining_task_strs = [str(task) for task in task_list]
-            version = None
-            state = None
-            # Loop looking for updates till the state moves to a completed state.
-            # (tasks are removed from task_list one by one when they reach a completed)
-            while remaining_task_strs:
-                update = pc.WaitForUpdates(version)
-                for filter_set in update.filterSet:
-                    for obj_set in filter_set.objectSet:
-                        task: vim.Task = obj_set.obj
-                        for change in obj_set.changeSet:
-                            if change.name == 'info':
-                                state = change.val.state
-                            elif change.name == 'info.state':
-                                state = change.val
-                            else:
-                                continue
-
-                            if not str(task) in remaining_task_strs:
-                                continue
-
-                            if state == vim.TaskInfo.State.success:
-                                remaining_task_strs.remove(str(task))
-                                if log_prefix := log_prefixes.get(task):
-                                    self.logger.info(f"{log_prefix}: success")
-                            elif state == vim.TaskInfo.State.error:
-                                if len(task_list) > 1:
-                                    remaining_task_strs.remove(str(task))
-                                    log_prefix = log_prefixes.get(task)
-                                    self.logger.error(f"{f'{log_prefix}: ' if log_prefix else ''}{task.info.error}", exc_info=task.info.error)
-                                    task_failures += 1
-                                else:
-                                    raise task.info.error
-                # Move to next version
-                version = update.version
-        finally:
-            if pc_filter:
-                pc_filter.Destroy()
-
-        if task_failures > 0:
-            raise MessageError(f"{task_failures} task{'s' if task_failures > 1 else ''} failed (see previous logs)")
-
- 
-    def get_out_dir(self):
-        return Path('data' if self.env == 'default' else f'data/{self.env}')
-
-    #endregion
-
-
-    #region Class helpers
-    
-    @classmethod
-    def get_configured_envs(cls, *, config: ConfigParser = None, section: str = None):
-        if not config:
-            config = CONFIG
-        if not section:
-            section = CONFIG_SECTION
-        
-        envs: list[str] = []
-        for _section in config.sections():
-            if m := re.match(r'^' + re.escape(section) + r'(?:\:(.+))?', _section):
-                env = m[1]
-                if env == 'default':
-                    raise ValueError(f"Invalid configuration section \"{_section}\": name \"default\" is reserved")
-                if not env:
-                    env = 'default'
-                envs.append(env)
-        return envs
-        
-    @classmethod
-    def parse_obj_type(cls, value: str|type|vim.ManagedEntity) -> type[vim.ManagedEntity]:
-        if not value:
-            raise ValueError(f"name cannot be blank")
-        
-        elif isinstance(value, type):
-            if not issubclass(value, vim.ManagedEntity):
-                raise TypeError(f"type {value} is not a subclass of vim.ManagedEntity")
-            
-            return value
-        
-        elif isinstance(value, vim.ManagedEntity):
-            return type(value)
-        
-        elif not isinstance(value, str):
-            raise TypeError(f"invalid type for name: {value}")
-        
-        else:
-            lower = value.lower()
-
-            # Search in types
-            if lower in cls.OBJ_TYPES:
-                return cls.OBJ_TYPES[lower]
-
-            # Handle aliases            
-            if lower == 'vm':
-                return vim.VirtualMachine
-            if lower == 'host':
-                return vim.HostSystem
-            if lower == 'net':
-                return vim.Network
-            if lower == 'dvs':
-                return vim.DistributedVirtualSwitch
-            if lower == 'dvp':
-                return vim.dvs.DistributedVirtualPortgroup
-            if lower == 'ds':
-                return vim.Datastore
-            if lower == 'dc':
-                return vim.Datacenter
-            if lower == 'cluster':
-                return vim.ClusterComputeResource
-
-            raise KeyError(f"vim managed object type not found for name {value}")
-
-    def _build_obj_types() -> dict[str,type[vim.ManagedEntity]]:
-        types = {}
-
-        for key in _managedDefMap.keys():
-            if not key.startswith('vim.'):
-                continue
-
-            attr = key[len('vim.'):]
-            _type = getattr(vim, attr)
-            if not issubclass(_type, vim.ManagedEntity):
-                continue
-
-            lower = attr.lower()
-            if lower in types:
-                continue
-
-            types[lower] = _type
-
-        return types
-            
-    OBJ_TYPES = _build_obj_types()
-    
-    #endregion
-
-
-    #region Retrieve network objects by key
-    
-    def get_portgroup_by_key(self, key: str) -> vim.dvs.DistributedVirtualPortgroup:
-        if key is None:
-            return None
-        
-        try:
-            by_key = self._portgroups_by_key
-        except AttributeError:
-            by_key = {}
-            for obj in self.iter_objs(vim.dvs.DistributedVirtualPortgroup):
-                by_key[obj.key] = obj
-            self._portgroups_by_key = by_key
-
-        return by_key.get(key)
-    
-    def get_switch_by_uuid(self, uuid: str) -> vim.DistributedVirtualSwitch:
-        if uuid is None:
-            return None
-        
-        try:
-            by_uuid = self._switchs_by_uuid
-        except AttributeError:
-            by_uuid = {}
-            for obj in self.iter_objs(vim.DistributedVirtualSwitch):
-                by_uuid[obj.uuid] = obj
-            self._switchs_by_uuid = by_uuid
-
-        return by_uuid.get(uuid)
-
-    #endregion
-    
-
-def _expand_search_from_files(search: list[str|Path|re.Pattern]|str|Path|re.Pattern|None, *, key: Literal['name', 'ref'] = 'name') -> list[str|re.Pattern]|None:
-    """
-    Expand search from CSV or Excel files if search ends with '.csv' or '.xlsx'.
-    """
-    if search is None:
-        return None
-    elif isinstance(search, (str,Path,re.Pattern)):
-        search = [search]
-    
-    def expand_from_xlsx_file(path: Path, table_name: str = None):
-        workbook = ExcelWorkbook(path)
-        table = workbook.get_table(table_name)
-        if not key in table.column_names:
-            raise ValueError(f"Column \"{key}\" not found in {path}")
-        for row in table:
-            if row[key]:
-                yield row[key]
-
-    def expand_from_csv_file(path: Path):
-        for row in iter_dicts_from_csv(path):
-            if not key in row:
-                raise ValueError(f"Column \"{key}\" not found in {path}")
-            if row[key]:
-                yield row[key]
-    
-    result = []
-    for elem in search:
-        if isinstance(elem, Path):
-            if elem.suffix.lower() == '.xlsx':
-                for file_elem in expand_from_xlsx_file(elem):
-                    result.append(file_elem)
-            elif elem.suffix.lower() == '.csv':
-                for file_elem in expand_from_csv_file(elem):
-                    result.append(file_elem)
-            else:
-                raise ValueError(f"Invalid search path extension: {elem}")
-        elif isinstance(elem, str):
-            if is_excel_path(elem, accept_table_suffix=True):
-                path, table_name = split_excel_path(elem)
-                for file_elem in expand_from_xlsx_file(path, table_name):
-                    result.append(file_elem)
-            elif elem.lower().endswith('.csv'):
-                for file_elem in expand_from_csv_file(Path(elem)):
-                    result.append(file_elem)
-            else:
-                result.append(elem)
-        else:
-            result.append(elem)
-
-    return result
-
-
-def get_obj_ref(obj: vim.ManagedObject) -> str:
-    """
-    Get the value of the Managed Object Reference (MOR) of the given object.
-
-    See: https://vdc-repo.vmware.com/vmwb-repository/dcr-public/1ef6c336-7bef-477d-b9bb-caa1767d7e30/82521f49-9d9a-42b7-b19b-9e6cd9b30db1/mo-types-landing.html
-    """
-    text = str(obj)
-    m = re.match(r"^'(.*)\:(.*)'$", text)
-    if not m:
-        raise ValueError(f'Invalid object identifier: {text}')
-    
-    expected_type = type(obj).__name__
-    if m.group(1) != expected_type:
-        raise ValueError(f'Invalid type for object identifier: {text}, expected: {expected_type}')
-    return m.group(2)
-
-
-def get_obj_path(obj: vim.ManagedEntity, full: bool = False) -> str:
-    """ Return the path of the given vim managed entity. """
-    if not obj:
-        return None
-    if isinstance(obj, vim.Datacenter):
-        return obj.name
-    if not full:
-        if obj.parent:
-            if isinstance(obj.parent, vim.Datacenter):
-                return None            
-            super_parent = obj.parent.parent
-            if isinstance(super_parent, vim.Datacenter):
-                return obj.name
-                
-    if not obj.parent:
-        return obj.name
-    elif not full and isinstance(obj, vim.ResourcePool) and obj.name == 'Resources':
-        return get_obj_path(obj.parent, full=full)
-    else:        
-        return get_obj_path(obj.parent, full=full) + "/" + obj.name
-
-
-def identify_obj(obj: vim.ManagedObject) -> dict:
-    if obj is None:
-        return None
-
-    if not isinstance(obj, vim.ManagedObject):
-        raise ValueError(f'invalid type: {type(obj)}')
-
-    data = {
-        "_type": type(obj).__name__, # managed object type
-        "ref": get_obj_ref(obj),
-    }
-
-    try:
-        if name := getattr(obj, 'name', None):
-            data["name"] = name            
-    except vim.fault.NoPermission:
-        data["name"] = '!error:no_permission'
-
-    if 'name' in data and data["name"] == "Resources" and isinstance(obj, vim.ResourcePool) and hasattr(obj, 'parent') and isinstance(obj.parent, vim.ClusterComputeResource):
-        # root resource pool of a cluster (named 'Resources'): let's prepend cluster name
-        data["name"] = obj.parent.name + "/" + data["name"]
-
-    return data
-    
-
-def dictify_value(data: list|str):
-    """
-    Return a dict if data is a list of OptionValue, StringValue or SystemIdentificationInfo objects, or if it is a string like guestOS.detailed.data.
-    Otherwise leave as is.
-    """
-    def allinstance(enumerable_instance, element_type):
-        any = False
-        for element in enumerable_instance:
-            any = True
-            if not isinstance(element, element_type):
-                return False
-        return any
-        
-    if isinstance(data, list):
-        if allinstance(data, vim.option.OptionValue) or allinstance(data, vim.CustomFieldsManager.StringValue): #example for vm: config.extraConfig, summary.config.customValue
-            result = {}
-            for ov in data:
-                key = ov.key
-                value = ov.value
-                if key == "guestOS.detailed.data":
-                    value = dictify_value(value)
-                result[key] = value
-            return result
-
-        elif allinstance(data, vim.host.SystemIdentificationInfo): #example for host: summary.hardware.otherIdentifyingInfo
-            result = {}
-            for ov in data:
-                key = ov.identifierType.key
-                value = ov.identifierValue
-                result[key] = value
-            return result
-
-        else:
-            return data
-    
-    if isinstance(data, str):
-        if matches := re.findall(r"([a-zA-Z0-9]+)='([^']+)'", data): # example: guestOS.detailed.data
-            result = {}
-            for m in matches:
-                key = m[0]
-                value = m[1]
-                if key == 'bitness' and re.match(r'^\d+$', value):
-                    value = int(value)
-                result[key] = value
-            return result
-
-        else:
-            return data       
-        
-    else:
-        return data
-
-
-def dictify_obj(obj: vim.ManagedEntity, *, object_types=False, exclude_keys=[], max_depth=None) -> dict:
-    """
-    Export all available information about the given VMWare managed object to a dictionnary.
-    """    
-    for key in ['dynamicProperty', 'recentTask']:
-        if not key in exclude_keys:
-            exclude_keys.append(key)
-    exclude_keys_containing = ['capability', 'alarm']
-    keypath = []
-
-    def keypath_str():
-        s = ''
-        for key in keypath:
-            s += ('.' if s and not isinstance(key, int) else '') + (f"[{key}]" if isinstance(key, int) else key)
-        return s
-
-    def forward(key: str):
-        keypath.append(key)
-
-    def backward():
-        del keypath[-1]
-
-    def handle_object(obj: object):
-        if method := getattr(obj.__class__, 'to_dict', None):
-            value = method(obj)
-            if value and object_types:
-                    return { '_type': type(obj).__name__, **value }
-            return value
-
-        result = { '_type': type(obj).__name__ } if object_types else {}
-        any = False
-        for key in dir(obj):
-            ignore = False
-            if key.startswith('_') or key in exclude_keys:
-                ignore = True
-            else:
-                for containing in exclude_keys_containing:
-                    if containing in key.lower():
-                        ignore = True
-                        break
-
-            if ignore:
-                continue
-
-            forward(key)
-            
-            try:
-                value = getattr(obj, key)
-            except: # problem getting the data (e.g. invalid/not-supported accessor)
-                _key = keypath_str()
-                if _key not in ['configManagerEnabled', 'environmentBrowser']:
-                    _logger.error('Cannot read attribute: %s', _key)
-                value = "!error:cannot_read"
-            
-            value = handle_any(value)
-
-            if value is not None:
-                result[key] = value
-                any = True
-
-            backward()
-
-        if any:
-            return result
-
-    def handle_dict(data: dict):
-        result = {}
-        any = False
-        for key in data:
-            forward(key)
-            value = handle_any(data[key])
-            if value is not None:
-                result[key] = value
-                any = True
-            backward()
-
-        if any:
-            return result
-
-    def handle_list(data: list):
-        result = dictify_value(data)
-        if isinstance(result, dict):
-            return result
-
-        # general case
-        result = []
-        any = False
-        for i, value in enumerate(data):
-            forward(i)
-            extracted = handle_any(value)
-            if extracted is not None:
-                result.append(extracted)
-                any = True
-            backward()
-
-        if any:
-            return result
-
-    def handle_any(data):
-        if data is None or isinstance(data, (type, FunctionType, MethodType, BuiltinMethodType, BuiltinFunctionType)):
-            return None
-        
-        elif isinstance(data, (str, int, float, complex)):
-            return data
-
-        elif isinstance(data, date):
-            if data.year == 1970 and data.month == 1 and data.day == 1:
-                return None
-            return data
-
-        elif isinstance(data, vim.ManagedObject):
-            if not keypath: # depth == 0
-                result = identify_obj(data)
-                for key, value in handle_object(data).items():
-                    result[key] = value
-                return result
-            else:
-                return identify_obj(data)
-
-        elif max_depth and len(keypath) >= max_depth:
-            _logger.error('Reached max depth: %s', type(data).__name__)
-            return f"!error:max_depth({type(data).__name__})"
-
-        elif isinstance(data, dict):
-            return handle_dict(data)
-
-        elif isinstance(data, list):
-            return handle_list(data)
-            
-        else:
-            return handle_object(data)
-
-    return handle_any(obj)
-
-
-def dump_obj(obj: vim.ManagedObject, obj_out: os.PathLike|IOBase, *, title: str = None):
-    if not title:
-        title = getattr(obj, 'name', None)
-        if not title:
-            title = type(obj).__name__
-
-    if isinstance(obj_out, IOBase):
-        out_name = getattr(obj_out, 'name', '<io>')
-    else:
-        out_name = str(obj_out)
-
-    data = dictify_obj(obj)
-
-    _logger.info(f"Export {title} to {out_name}")
-    with nullcontext(obj_out) if isinstance(obj_out, IOBase) else open(obj_out, 'w', encoding='utf-8') as fp:
-        json.dump(data, fp=fp, indent=4, cls=ExtendedJSONEncoder, ensure_ascii=False)
-
-
-# For docs
-__all__ = (
-    '__prog__', '__version__', '__version_tuple__',
-    'VCenterClient',
-    'get_obj_ref', 'get_obj_path', 'identify_obj', 'dictify_value', 'dictify_obj', 'dump_obj',
-)
+"""
+Top-level API of vmware-reporter library.
+"""
+from __future__ import annotations
+
+import json
+import logging
+import os
+import re
+import urllib3
+import requests
+from collections.abc import Callable, Iterator
+from configparser import ConfigParser
+from contextlib import nullcontext
+from datetime import date
+from inspect import signature
+from io import IOBase
+from pathlib import Path
+from types import (BuiltinFunctionType, BuiltinMethodType, FunctionType,
+                   MethodType)
+from typing import Any, Iterable, Literal, TypeVar, overload
+from uuid import UUID
+
+from pyVim.connect import Disconnect, SmartConnect
+from pyVmomi import vim, vmodl
+from pyVmomi.VmomiSupport import _managedDefMap
+from zut import (ExtendedJSONEncoder, Filters, MessageError,
+                 iter_dicts_from_csv, resolve_host, configure_smb_credentials)
+from zut.excel import ExcelWorkbook, is_excel_path, split_excel_path
+
+from .settings import CONFIG, CONFIG_SECTION
+
+__prog__ = 'vmware-reporter'
+
+try:
+    # Version generated by setuptools_scm during build
+    from ._version import __version__, __version_tuple__
+except ImportError:
+    __version__ = None
+    __version_tuple__ = None
+
+_logger = logging.getLogger(__name__)
+
+T_Obj = TypeVar('T_Obj', bound=vim.ManagedEntity)
+
+
+class VCenterClient:
+    """
+    Main entry point of the library to retrieve VMWare managed objects and interact with them. 
+    """
+    _first_instanciation = True
+
+    def __init__(self, env: str = None, *, host: str = None, user: str = None, password: str = None, no_ssl_verify: bool = None, out_dir: str|Path = None, config: ConfigParser = None, section: str = None):
+        """
+        Create a new vCenter client.
+
+        If `host`, `user`, `password` or `no_ssl_verify` options are not provided, they are read from configuration file
+        in section `[vmware-reporter]` (or `[vmware-reporter:{name}]` if `name` is given).
+
+        :param env: An optional name to distinguish between several vCenters.
+        :param host: Host name of the vCenter.
+        :param user: Name of the vCenter user having access to the API.
+        :param password: Password of the vCenter user having access to the API.
+        """        
+        if not config:
+            config = CONFIG
+        if not section:
+            section = CONFIG_SECTION
+
+        if type(self)._first_instanciation:
+            smb_user = config.get(section, 'smb_user', fallback=None)
+            smb_password = config.get(section, 'smb_password', fallback=None)
+            if smb_user and smb_password:
+                configure_smb_credentials(smb_user, smb_password)
+            type(self)._first_instanciation = False
+        
+        if not env:
+            envs = VCenterClient.get_configured_envs(config=config, section=section)
+            if len(envs) > 1:
+                raise MessageError(f"Name of the environment / VCenter to use must be provided. Available: {', '.join(envs) if envs else 'none'}.")
+            elif len(envs) == 1:
+                env = envs[0]
+            else:
+                raise MessageError(f"No VCenter client configured.")
+        self.env = env or 'default'
+
+        full_section = section + ('' if env == 'default' else f':{env}')
+        self.host = host if host is not None else config.get(full_section, 'host')
+        self.user = user if user is not None else config.get(full_section, 'user')
+        self.password = password if password is not None else config.get(full_section, 'password')
+        self.no_ssl_verify = no_ssl_verify if no_ssl_verify is not None else config.getboolean(full_section, 'no_ssl_verify', fallback=False)
+
+        if out_dir is None:
+            out_dir = config.get(full_section, 'out_dir', fallback=None)
+            if out_dir is None:
+                out_dir = config.get(section, 'out_dir', fallback=None)
+                if out_dir is None:
+                    out_dir = 'data' if env == 'default' else 'data/{env}'
+        self.out_dir = Path(str(out_dir).format(env=env))
+        
+        self.logger = logging.getLogger(f'{self.__class__.__module__}.{self.__class__.__qualname__}' + ('' if env == 'default' else f'.{self.env}'))
+
+        self._rest_session = requests.Session()
+        self._categories: dict[UUID,Category] = None
+        self._tags: dict[UUID,Tag] = None
+
+
+    #region Enter/connect and exit/close
+
+    def __enter__(self):
+        self.connect()
+        return self
+
+
+    def __exit__(self, exc_type = None, exc_value = None, exc_traceback = None):
+        self.close()
+
+
+    def connect(self):
+        addrs = resolve_host(self.host, timeout=2.0)
+        if not addrs:
+            raise ValueError(f"Cannot resolve host name \"{self.host}\"")
+        
+        addr = addrs[0]
+        self.logger.debug(f"Connect to {addr} ({self.host}) with user {self.user}")
+
+        self._service_instance = SmartConnect(host=self.host, user=self.user, pwd=self.password, disableSslCertValidation=self.no_ssl_verify)
+
+
+    def close(self):
+        try:
+            Disconnect(self._service_instance)
+        except AttributeError:
+            pass
+
+        self._rest_disconnect()
+    
+
+    @property
+    def service_instance(self) -> vim.ServiceInstance:
+        try:
+            return self._service_instance
+        except AttributeError:
+            pass
+
+        self.connect()
+        return self._service_instance
+
+
+    @property
+    def service_content(self) -> vim.ServiceInstanceContent:
+        try:
+            return self._service_content
+        except AttributeError:
+            pass
+
+        self._service_content = self.service_instance.RetrieveContent()
+        return self._service_content
+    
+    #endregion
+
+
+    #region Retrieve managed objects
+
+    @property
+    def datacenter(self):
+        try:
+            return self._datacenter
+        except AttributeError:
+            pass
+
+        datacenters = self.get_objs(vim.Datacenter)
+        if not datacenters:
+            raise ValueError(f"Datacenter not found")
+        if len(datacenters) > 1:
+            raise ValueError(f"Several datacenter found")
+        self._datacenter = datacenters[0]
+        return self._datacenter
+
+
+    def get_obj(self, type: type[T_Obj], search: list[str|re.Pattern]|str|re.Pattern|UUID, *, normalize: bool = False, key: Literal['name', 'ref', 'uuid', 'bios_uuid'] = 'name') -> T_Obj:
+        """
+        Find a single VMWare managed object.
+
+        Raise KeyError if not found or several found.
+        """
+        if key in ['uuid', 'bios_uuid']:
+            if not isinstance(search, (UUID,str)):
+                raise TypeError(f"specs must be UUID or str for key {key}, got {type(search).__name__}")
+            
+            if isinstance(search, UUID):
+                uuid = search
+            else:
+                uuid = UUID(search)
+
+            obj = None
+            
+            if key == 'bios_uuid':
+                # NOTE: uuid is "BIOS UUID". Seems to match the end of `sudo cat /sys/class/dmi/id/product_uuid`.
+                if type == vim.VirtualMachine:
+                    obj = self._find_by_uuid(uuid, for_vm=True, instance_uuid=False)
+                else:
+                    raise ValueError(f"key '{key}' can be used only for virtual machines")
+                
+            else:
+                if type == vim.VirtualMachine:
+                    obj = self._find_by_uuid(uuid, for_vm=True, instance_uuid=True)
+                elif type == vim.HostSystem:
+                    obj = self._find_by_uuid(uuid, for_vm=False, instance_uuid=False)
+                else:
+                    raise ValueError(f"key '{key}' can be used only for virtual machines or host systems")
+
+            if obj:
+                return obj
+            else:
+                raise KeyError(f"Not found: {search} (type: {type.__name__})")
+
+        else:
+            iterator = self.iter_objs(types=type, search=search, normalize=normalize, key=key)
+            try:
+                found = next(iterator)
+            except StopIteration:
+                raise KeyError(f"Not found: {search} (type: {type.__name__})")
+            
+            try:
+                next(iterator)
+                raise KeyError(f"Several found: {search} (type: {type.__name__})")
+            except StopIteration:
+                pass
+            return found
+            
+
+    def _find_by_uuid(self, uuid: UUID|str, for_vm: bool, instance_uuid: bool):
+        if isinstance(uuid, UUID):
+            uuid = str(uuid)
+        
+        for datacenter in self.iter_objs(vim.Datacenter):
+            obj = self.service_content.searchIndex.FindByUuid(datacenter, uuid, vmSearch=for_vm, instanceUuid=instance_uuid)
+            if obj:
+                return obj
+
+
+    @overload
+    def get_objs(self, types: type[T_Obj], search: list[str|Path|re.Pattern]|str|Path|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name', sort_key: str|list[str]|Callable = None) -> list[T_Obj]:
+        ...
+
+    def get_objs(self, types: list[type|str]|type|str = None, search: list[str|Path|re.Pattern]|str|Path|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name', sort_key: str|list[str]|Callable = None):        
+        """
+        List VMWare managed objects matching the given search.
+        """
+        objs = [obj for obj in self.iter_objs(types, search, normalize=normalize, key=key)]
+
+        if sort_key:
+            if isinstance(sort_key, str):
+                sort_key = [sort_key]
+
+            if isinstance(sort_key, list):
+                sort_func = lambda obj: [getattr(obj, attr) for attr in sort_key]
+            else:
+                sort_func = sort_key
+
+            objs.sort(key=sort_func)
+
+        return objs
+
+
+    @overload
+    def iter_objs(self, types: type[T_Obj], search: list[str|Path|re.Pattern]|str|Path|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name') -> Iterator[T_Obj]:
+        ...
+
+    def iter_objs(self, types: list[type|str]|type|str = None, search: list[str|Path|re.Pattern]|str|Path|re.Pattern = None, *, normalize: bool = None, key: Literal['name', 'ref'] = 'name'):
+        """
+        Iterate over VMWare managed objects matching the given search.
+        """
+        # Expand search from CSV or Excel files if search ends with '.csv' or '.xlsx'
+        search = _expand_search_from_files(search, key=key)
+
+        # Prepare value filter
+        filters = Filters(search, normalize=normalize)
+
+        # Prepare types
+        if not types:
+            types = []
+        elif isinstance(types, (str,type)):
+            types = [types]
+        
+        types = [self.parse_obj_type(_type) for _type in types]
+
+        # Search using a container view
+        view = None
+        try:
+            view = self.service_content.viewManager.CreateContainerView(self.service_content.rootFolder, types, recursive=True)
+
+            for obj in view.view:
+                if self._obj_matches(obj, key, filters):
+                    yield obj
+        finally:
+            if view:
+                view.Destroy()
+
+
+    def _obj_matches(self, obj: vim.ManagedEntity, key: Literal['name', 'ref'], filters: Filters):
+        if not filters:
+            return True
+        
+        if key == 'name':
+            try:
+                value = obj.name
+            except vim.fault.NoPermission:
+                return False
+            
+        elif key == 'ref':
+            value = get_obj_ref(obj)
+            
+        else:
+            raise ValueError(f"key not supported: {key}")
+        
+        return filters.matches(value)
+
+    #endregion
+
+
+    #region Instance helpers
+
+    @property
+    def cookie(self) -> dict:
+        try:
+            return self._cookie
+        except AttributeError:
+            pass
+    
+        # Get the cookie built from the current session
+        client_cookie = self.service_instance._stub.cookie
+
+        # Break apart the cookie into it's component parts
+        cookie_name = client_cookie.split("=", 1)[0]
+        cookie_value = client_cookie.split("=", 1)[1].split(";", 1)[0]
+        cookie_path = client_cookie.split("=", 1)[1].split(";", 1)[1].split(
+            ";", 1)[0].lstrip()
+        cookie_text = " " + cookie_value + "; $" + cookie_path
+
+        # Make a cookie
+        self._cookie = dict()
+        self._cookie[cookie_name] = cookie_text
+        return self._cookie
+
+
+    def wait_for_task(self, tasks: vim.Task|list[vim.Task]|dict[vim.Task,str], *, success_callback=None, error_callback=None):
+        """
+        Given a service instance and tasks, return after all the tasks are complete.
+        - `tasks`: a task, a list of tasks, or a dict associating task to log prefixes.
+        """
+        task_list: list[vim.Task] = []
+        log_prefixes: dict[vim.Task,str] = {}
+        if isinstance(tasks, dict):
+            log_prefixes = tasks
+            for task in tasks.keys():
+                if not isinstance(task, vim.Task):
+                    raise TypeError(f"Invalid dict key: {task} (type {type(task).__name__}, expected vim.Task)")
+                task_list.append(task)
+        elif isinstance(tasks, list):
+            for task in tasks:
+                if not isinstance(task, vim.Task):
+                    raise TypeError(f"Invalid list element: {task} (type {type(task).__name__}, expected vim.Task)")
+                task_list.append(task)
+        elif isinstance(tasks, vim.Task):
+            task_list.append(tasks)
+        else:
+            raise TypeError(f"Invalid argument: {task} (type {type(task).__name__}, expected vim.Task)")
+        
+        # Create filter
+        obj_specs = [vmodl.query.PropertyCollector.ObjectSpec(obj=task) for task in task_list]   
+        property_spec = vmodl.query.PropertyCollector.PropertySpec(type=vim.Task, pathSet=[], all=True)
+        filter_spec = vmodl.query.PropertyCollector.FilterSpec(objectSet=obj_specs, propSet=[property_spec])
+        pc = self.service_instance.content.propertyCollector
+        pc_filter = pc.CreateFilter(filter_spec, True)
+
+        task_failures = 0
+        try:
+            remaining_task_strs = [str(task) for task in task_list]
+            version = None
+            state = None
+            # Loop looking for updates till the state moves to a completed state.
+            # (tasks are removed from task_list one by one when they reach a completed)
+            while remaining_task_strs:
+                update = pc.WaitForUpdates(version)
+                for filter_set in update.filterSet:
+                    for obj_set in filter_set.objectSet:
+                        task: vim.Task = obj_set.obj
+                        for change in obj_set.changeSet:
+                            if change.name == 'info':
+                                state = change.val.state
+                            elif change.name == 'info.state':
+                                state = change.val
+                            else:
+                                continue
+
+                            if not str(task) in remaining_task_strs:
+                                continue
+
+                            if state == vim.TaskInfo.State.success:
+                                remaining_task_strs.remove(str(task))
+                                if log_prefix := log_prefixes.get(task):
+                                    self.logger.info(f"{log_prefix}: SUCCESS")
+                                if success_callback:
+                                    success_callback(task)
+                            elif state == vim.TaskInfo.State.error:
+                                if len(task_list) > 1:
+                                    remaining_task_strs.remove(str(task))
+                                    log_prefix = log_prefixes.get(task)
+                                    self.logger.error(f"{f'{log_prefix}: ' if log_prefix else ''}{task.info.error}", exc_info=task.info.error)                                        
+                                    if error_callback:
+                                        error_callback(task, task.info.error)
+                                    task_failures += 1
+                                else:
+                                    raise task.info.error
+                # Move to next version
+                version = update.version
+        finally:
+            if pc_filter:
+                pc_filter.Destroy()
+
+        if task_failures > 0:
+            raise MessageError(f"{task_failures} task{'s' if task_failures > 1 else ''} failed (see previous logs)")
+
+    #endregion
+
+
+    #region Class helpers
+    
+    @classmethod
+    def get_configured_envs(cls, *, config: ConfigParser = None, section: str = None):
+        if not config:
+            config = CONFIG
+        if not section:
+            section = CONFIG_SECTION
+
+        envs: list[str] = []
+        for _section in config.sections():
+            if m := re.match(r'^' + re.escape(section) + r'(?:\:(.+))?', _section):
+                env = m[1]
+                if env == 'default':
+                    raise ValueError(f"Invalid configuration section \"{_section}\": name \"default\" is reserved")
+                if not env:
+                    env = 'default'
+                if config.get(_section, 'host', fallback=None) is not None:
+                    envs.append(env)
+
+        return envs
+        
+    @classmethod
+    def parse_obj_type(cls, value: str|type|vim.ManagedEntity) -> type[vim.ManagedEntity]:
+        if not value:
+            raise ValueError(f"name cannot be blank")
+        
+        elif isinstance(value, type):
+            if not issubclass(value, vim.ManagedEntity):
+                raise TypeError(f"type {value} is not a subclass of vim.ManagedEntity")
+            
+            return value
+        
+        elif isinstance(value, vim.ManagedEntity):
+            return type(value)
+        
+        elif not isinstance(value, str):
+            raise TypeError(f"invalid type for name: {value}")
+        
+        else:
+            lower = value.lower()
+
+            # Search in types
+            if lower in cls.OBJ_TYPES:
+                return cls.OBJ_TYPES[lower]
+
+            # Handle aliases            
+            if lower == 'vm':
+                return vim.VirtualMachine
+            if lower == 'host':
+                return vim.HostSystem
+            if lower == 'net':
+                return vim.Network
+            if lower == 'dvs':
+                return vim.DistributedVirtualSwitch
+            if lower == 'dvp':
+                return vim.dvs.DistributedVirtualPortgroup
+            if lower == 'ds':
+                return vim.Datastore
+            if lower == 'dc':
+                return vim.Datacenter
+
+            raise KeyError(f"vim managed object type not found for name {value}")
+
+    def _build_obj_types() -> dict[str,type[vim.ManagedEntity]]:
+        types = {}
+
+        for key in _managedDefMap.keys():
+            if not key.startswith('vim.'):
+                continue
+
+            attr = key[len('vim.'):]
+            _type = getattr(vim, attr)
+            if not issubclass(_type, vim.ManagedEntity):
+                continue
+
+            lower = attr.lower()
+            if lower in types:
+                continue
+
+            types[lower] = _type
+
+        return types
+            
+    OBJ_TYPES = _build_obj_types()
+    
+    #endregion
+
+
+    #region Retrieve network objects by key
+    
+    def get_portgroup_by_key(self, key: str) -> vim.dvs.DistributedVirtualPortgroup:
+        if key is None:
+            return None
+        
+        try:
+            by_key = self._portgroups_by_key
+        except AttributeError:
+            by_key = {}
+            for obj in self.iter_objs(vim.dvs.DistributedVirtualPortgroup):
+                by_key[obj.key] = obj
+            self._portgroups_by_key = by_key
+
+        return by_key.get(key)
+    
+    def get_switch_by_uuid(self, uuid: str) -> vim.DistributedVirtualSwitch:
+        if uuid is None:
+            return None
+        
+        try:
+            by_uuid = self._switchs_by_uuid
+        except AttributeError:
+            by_uuid = {}
+            for obj in self.iter_objs(vim.DistributedVirtualSwitch):
+                by_uuid[obj.uuid] = obj
+            self._switchs_by_uuid = by_uuid
+
+        return by_uuid.get(uuid)
+
+    #endregion
+
+
+    #region REST API client
+    # See: https://gist.github.com/em2er/74cdabdd0fd337f382939df3e5f6a68e
+    # See: https://vdc-download.vmware.com/vmwb-repository/dcr-public/1cd28284-3b72-4885-9e31-d1c6d9e26686/71ef7304-a6c9-43b3-a3cd-868b2c236c81/doc/index.html
+
+    def _rest_disconnect(self):
+        if 'vmware-api-session-id' in self._rest_session.headers:
+            self.rest_request('/rest/com/vmware/cis/session', method='DELETE')
+
+    def rest_request(self, path: str, *, method = 'GET', **options):
+        if not 'vmware-api-session-id' in self._rest_session.headers and not 'auth' in options:
+            session_id = self.rest_request('/rest/com/vmware/cis/session', method='POST', auth=(self.user, self.password))
+            self._rest_session.headers.update({'vmware-api-session-id': session_id})
+
+        self.logger.debug("%s %s", method, path)
+        url = f"https://{self.host}{path}"
+
+        with urllib3.warnings.catch_warnings() if self.no_ssl_verify else nullcontext():
+            if self.no_ssl_verify:
+                urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+            response = self._rest_session.request(method, url, verify=not self.no_ssl_verify, **options)
+
+        response.raise_for_status()
+        if response.headers.get('content-type') == 'application/json':
+            dict_response = response.json()
+            self.logger.debug("JSON response: %s", dict_response)
+            return dict_response['value']
+        else:
+            if self.logger.isEnabledFor(logging.DEBUG):
+                text_response = response.text
+                self.logger.debug("TEXT response: %s", text_response)
+            return None
+    
+    @property
+    def categories(self):
+        if self._categories is None:
+            self._categories = {}
+            for category_id in self.rest_request('/rest/com/vmware/cis/tagging/category'):
+                structure = self.rest_request(f'/rest/com/vmware/cis/tagging/category/id:{category_id}')
+                category = Category(structure)
+                self._categories[category.uuid] = category
+        return self._categories
+
+    def get_categories(self) -> Iterable[Category]:
+        return self.categories.values()
+
+    def get_category_by_key(self, key: str|UUID):
+        if isinstance(key, str):
+            key = Category.parse_id(key)
+        return self.categories[key]
+
+    @property
+    def tags(self):
+        if self._tags is None:
+            self._tags = {}
+            for tag_id in self.rest_request('/rest/com/vmware/cis/tagging/tag'):
+                data = self.rest_request(f'/rest/com/vmware/cis/tagging/tag/id:{tag_id}')
+                tag = Tag(data, self.categories)
+                self._tags[tag.uuid] = tag
+        return self._tags
+
+    def get_tags(self) -> Iterable[Tag]:
+        return self.tags.values()
+
+    def get_tag_by_key(self, key: str|UUID):
+        if isinstance(key, str):
+            key = Tag.parse_id(key)
+        return self.tags[key]
+    
+    def get_obj_tags(self, obj: vim.ManagedObject):
+        tag_ids = self.rest_request(f'/rest/com/vmware/cis/tagging/tag-association?~action=list-attached-tags', method='POST', json={
+            "object_id": {
+                "id": get_obj_ref(obj),
+                "type": get_obj_typename(obj),
+            }
+        })
+        return [self.get_tag_by_key(tag_id) for tag_id in tag_ids]
+
+    #endregion
+
+
+class Category:
+    def __init__(self, structure):
+        self.uuid = self.parse_id(structure['id'])
+        self.name: str = structure['name']
+        self.description: str = structure['description']
+        self.cardinality: str = structure['cardinality']
+        self.associable_types: list[str] = structure['associable_types']
+
+    @classmethod
+    def parse_id(cls, id: str):                    
+        if m := re.match(r'^urn:vmomi:InventoryServiceCategory:([0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}):GLOBAL$', id):
+            return UUID(m[1])
+        else:
+            raise ValueError(f"Invalid category id: {id}")
+        
+    @property
+    def id(self):
+        return f"urn:vmomi:InventoryServiceCategory:{self.uuid}:GLOBAL"
+    
+    def __repr__(self):
+        return self.name
+
+
+class Tag:
+    def __init__(self, structure, categories: dict[UUID,Category]):
+        self.uuid = self.parse_id(structure['id'])
+        self.name: str = structure['name']
+        self.description: str = structure['description']
+        self.category = categories[Category.parse_id(structure['category_id'])]
+
+    @classmethod
+    def parse_id(cls, id: str):                    
+        if m := re.match(r'^urn:vmomi:InventoryServiceTag:([0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}):GLOBAL$', id):
+            return UUID(m[1])
+        else:
+            raise ValueError(f"Invalid tag id: {id}")
+        
+    @property
+    def id(self):
+        return f"urn:vmomi:InventoryServiceTag:{self.uuid}:GLOBAL"
+    
+    def __repr__(self):
+        return self.name
+
+
+def _expand_search_from_files(search: list[str|Path|re.Pattern]|str|Path|re.Pattern|None, *, key: Literal['name', 'ref'] = 'name') -> list[str|re.Pattern]|None:
+    """
+    Expand search from CSV or Excel files if search ends with '.csv' or '.xlsx'.
+    """
+    if search is None:
+        return None
+    elif isinstance(search, (str,Path,re.Pattern)):
+        search = [search]
+    
+    def expand_from_xlsx_file(path: Path, table_name: str = None):
+        workbook = ExcelWorkbook(path)
+        table = workbook.get_table(table_name)
+        if not key in table.column_names:
+            raise ValueError(f"Column \"{key}\" not found in {path}")
+        for row in table:
+            if row[key]:
+                if row.get('status') == 'IGNORE':
+                    _logger.info(f"Ignore {key}")
+                else:
+                    yield row[key]
+
+    def expand_from_csv_file(path: Path):
+        for row in iter_dicts_from_csv(path):
+            if not key in row:
+                raise ValueError(f"Column \"{key}\" not found in {path}")
+            if row[key]:
+                yield row[key]
+    
+    result = []
+    for elem in search:
+        if isinstance(elem, Path):
+            if elem.suffix.lower() == '.xlsx':
+                for file_elem in expand_from_xlsx_file(elem):
+                    result.append(file_elem)
+            elif elem.suffix.lower() == '.csv':
+                for file_elem in expand_from_csv_file(elem):
+                    result.append(file_elem)
+            else:
+                raise ValueError(f"Invalid search path extension: {elem}")
+        elif isinstance(elem, str):
+            if is_excel_path(elem, accept_table_suffix=True):
+                path, table_name = split_excel_path(elem)
+                for file_elem in expand_from_xlsx_file(path, table_name):
+                    result.append(file_elem)
+            elif elem.lower().endswith('.csv'):
+                for file_elem in expand_from_csv_file(Path(elem)):
+                    result.append(file_elem)
+            else:
+                result.append(elem)
+        else:
+            result.append(elem)
+
+    return result
+
+
+def get_obj_name(obj: vim.ManagedObject) -> str:
+    if obj is None:
+        return None
+    
+    if isinstance(obj, vim.ResourcePool) and obj.name == 'Resources' and obj.parent:
+        return f"{obj.parent.name}/{obj.name}"
+    else:
+        return obj.name
+
+
+def get_obj_ref(obj: vim.ManagedObject) -> str:
+    """
+    Get the value of the Managed Object Reference (MOR) of the given object.
+
+    See: https://vdc-repo.vmware.com/vmwb-repository/dcr-public/1ef6c336-7bef-477d-b9bb-caa1767d7e30/82521f49-9d9a-42b7-b19b-9e6cd9b30db1/mo-types-landing.html
+    """
+    if obj is None:
+        return None
+    
+    text = str(obj)
+    m = re.match(r"^'(.*)\:(.*)'$", text)
+    if not m:
+        raise ValueError(f'Invalid object identifier: {text}')
+    
+    expected_type = type(obj).__name__
+    if m.group(1) != expected_type:
+        raise ValueError(f'Invalid type for object identifier: {text}, expected: {expected_type}')
+    return m.group(2)
+
+
+def get_obj_path(obj: vim.ManagedEntity, full: bool = False) -> str:
+    """ Return the path of the given vim managed entity. """
+    if obj is None:
+        return None
+    
+    if isinstance(obj, vim.Datacenter):
+        return obj.name
+    if not full:
+        if obj.parent:
+            if isinstance(obj.parent, vim.Datacenter):
+                return None            
+            super_parent = obj.parent.parent
+            if isinstance(super_parent, vim.Datacenter):
+                return obj.name
+                
+    if not obj.parent:
+        return obj.name
+    else:        
+        return get_obj_path(obj.parent, full=full) + "/" + obj.name
+
+
+def get_obj_typename(obj: vim.ManagedObject) -> str:
+    if obj is None:
+        return None
+    
+    return type(obj).__name__.split('.')[-1]
+
+
+def identify_obj(obj: vim.ManagedObject) -> dict:
+    if obj is None:
+        return None
+
+    if not isinstance(obj, vim.ManagedObject):
+        raise ValueError(f'invalid type: {type(obj)}')
+
+    data = {
+        "_type": type(obj).__name__, # managed object type
+        "ref": get_obj_ref(obj),
+    }
+
+    try:
+        if name := getattr(obj, 'name', None):
+            data["name"] = name            
+    except vim.fault.NoPermission:
+        data["name"] = '!error:no_permission'
+
+    if 'name' in data and data["name"] == "Resources" and isinstance(obj, vim.ResourcePool) and hasattr(obj, 'parent') and isinstance(obj.parent, vim.ClusterComputeResource):
+        # root resource pool of a cluster (named 'Resources'): let's prepend cluster name
+        data["name"] = obj.parent.name + "/" + data["name"]
+
+    return data
+    
+
+def dictify_value(data: list|str):
+    """
+    Return a dict if data is a list of OptionValue, StringValue or SystemIdentificationInfo objects, or if it is a string like guestOS.detailed.data.
+    Otherwise leave as is.
+    """
+    def allinstance(enumerable_instance, element_type):
+        any = False
+        for element in enumerable_instance:
+            any = True
+            if not isinstance(element, element_type):
+                return False
+        return any
+        
+    if isinstance(data, list):
+        if allinstance(data, vim.option.OptionValue) or allinstance(data, vim.CustomFieldsManager.StringValue): #example for vm: config.extraConfig, summary.config.customValue
+            result = {}
+            for ov in data:
+                key = ov.key
+                value = ov.value
+                if key == "guestOS.detailed.data":
+                    value = dictify_value(value)
+                result[key] = value
+            return result
+
+        elif allinstance(data, vim.host.SystemIdentificationInfo): #example for host: summary.hardware.otherIdentifyingInfo
+            result = {}
+            for ov in data:
+                key = ov.identifierType.key
+                value = ov.identifierValue
+                result[key] = value
+            return result
+
+        else:
+            return data
+    
+    if isinstance(data, str):
+        if matches := re.findall(r"([a-zA-Z0-9]+)='([^']+)'", data): # example: guestOS.detailed.data
+            result = {}
+            for m in matches:
+                key = m[0]
+                value = m[1]
+                if key == 'bitness' and re.match(r'^\d+$', value):
+                    value = int(value)
+                result[key] = value
+            return result
+
+        else:
+            return data       
+        
+    else:
+        return data
+
+
+def dictify_obj(obj: vim.ManagedEntity, *, object_types=False, exclude_keys=[], max_depth=None) -> dict:
+    """
+    Export all available information about the given VMWare managed object to a dictionnary.
+    """    
+    for key in ['dynamicProperty', 'recentTask']:
+        if not key in exclude_keys:
+            exclude_keys.append(key)
+    exclude_keys_containing = ['capability', 'alarm']
+    keypath = []
+
+    def keypath_str():
+        s = ''
+        for key in keypath:
+            s += ('.' if s and not isinstance(key, int) else '') + (f"[{key}]" if isinstance(key, int) else key)
+        return s
+
+    def forward(key: str):
+        keypath.append(key)
+
+    def backward():
+        del keypath[-1]
+
+    def handle_object(obj: object):
+        if method := getattr(obj.__class__, 'to_dict', None):
+            value = method(obj)
+            if value and object_types:
+                    return { '_type': type(obj).__name__, **value }
+            return value
+
+        result = { '_type': type(obj).__name__ } if object_types else {}
+        any = False
+        for key in dir(obj):
+            ignore = False
+            if key.startswith('_') or key in exclude_keys:
+                ignore = True
+            else:
+                for containing in exclude_keys_containing:
+                    if containing in key.lower():
+                        ignore = True
+                        break
+
+            if ignore:
+                continue
+
+            forward(key)
+            
+            try:
+                value = getattr(obj, key)
+            except: # problem getting the data (e.g. invalid/not-supported accessor)
+                _key = keypath_str()
+                if _key not in ['configManagerEnabled', 'environmentBrowser']:
+                    _logger.error('Cannot read attribute: %s', _key)
+                value = "!error:cannot_read"
+            
+            value = handle_any(value)
+
+            if value is not None:
+                result[key] = value
+                any = True
+
+            backward()
+
+        if any:
+            return result
+
+    def handle_dict(data: dict):
+        result = {}
+        any = False
+        for key in data:
+            forward(key)
+            value = handle_any(data[key])
+            if value is not None:
+                result[key] = value
+                any = True
+            backward()
+
+        if any:
+            return result
+
+    def handle_list(data: list):
+        result = dictify_value(data)
+        if isinstance(result, dict):
+            return result
+
+        # general case
+        result = []
+        any = False
+        for i, value in enumerate(data):
+            forward(i)
+            extracted = handle_any(value)
+            if extracted is not None:
+                result.append(extracted)
+                any = True
+            backward()
+
+        if any:
+            return result
+
+    def handle_any(data):
+        if data is None or isinstance(data, (type, FunctionType, MethodType, BuiltinMethodType, BuiltinFunctionType)):
+            return None
+        
+        elif isinstance(data, (str, int, float, complex)):
+            return data
+
+        elif isinstance(data, date):
+            if data.year == 1970 and data.month == 1 and data.day == 1:
+                return None
+            return data
+
+        elif isinstance(data, vim.ManagedObject):
+            if not keypath: # depth == 0
+                result = identify_obj(data)
+                for key, value in handle_object(data).items():
+                    result[key] = value
+                return result
+            else:
+                return identify_obj(data)
+
+        elif max_depth and len(keypath) >= max_depth:
+            _logger.error('Reached max depth: %s', type(data).__name__)
+            return f"!error:max_depth({type(data).__name__})"
+
+        elif isinstance(data, dict):
+            return handle_dict(data)
+
+        elif isinstance(data, list):
+            return handle_list(data)
+            
+        else:
+            return handle_object(data)
+
+    return handle_any(obj)
+
+
+def dump_obj(obj: vim.ManagedObject, obj_out: os.PathLike|IOBase, *, title: str = None):
+    if not title:
+        title = getattr(obj, 'name', None)
+        if not title:
+            title = type(obj).__name__
+
+    if isinstance(obj_out, IOBase):
+        out_name = getattr(obj_out, 'name', '<io>')
+    else:
+        out_name = str(obj_out)
+
+    data = dictify_obj(obj)
+
+    _logger.info(f"Export {title} to {out_name}")
+    
+    if not isinstance(obj_out, IOBase):
+        if dir := os.path.dirname(obj_out):
+            os.makedirs(dir, exist_ok=True)
+
+    with nullcontext(obj_out) if isinstance(obj_out, IOBase) else open(obj_out, 'w', encoding='utf-8') as fp:
+        json.dump(data, fp=fp, indent=4, cls=ExtendedJSONEncoder, ensure_ascii=False)
+
+
+# For docs
+__all__ = (
+    '__prog__', '__version__', '__version_tuple__',
+    'VCenterClient', 'Category', 'Tag',
+    'get_obj_name', 'get_obj_ref', 'get_obj_path', 'get_obj_typename', 'identify_obj', 'dictify_value', 'dictify_obj', 'dump_obj',
+)
```

## vmware_reporter/__main__.py

```diff
@@ -1,87 +1,96 @@
-"""
-Interact easily with your VMWare clusters.
-"""
-from __future__ import annotations
-
-import logging
-import os
-from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
-from configparser import ConfigParser
-from contextlib import nullcontext
-from inspect import signature
-from types import FunctionType
-
-from zut import (OutTable, add_func_command, add_module_command,
-                 configure_logging, exec_command, get_help_text,
-                 register_locale)
-
-from . import VCenterClient, __prog__, __version__, customfield, autoreport
-from .datastore import add_datastore_commands
-from .dump import dump
-from .host import add_host_commands
-from .inventory import export_inventory
-from .net import add_net_commands
-from .vm import add_vm_commands
-
-logger = logging.getLogger(__name__)
-
-def main():
-    configure_logging()
-    register_locale(use_excel_csv=(os.environ.get('USE_EXCEL_CSV') or '1').lower() in ['1', 'yes', 'true', 'on'])
-    OutTable.DEFAULT_EXCEL_ATEXIT = (os.environ.get('DEFAULT_EXCEL_ATEXIT') or '1').lower() in ['1', 'yes', 'true', 'on']
-
-    parser = init_parser(__prog__, __version__, __doc__)
-
-    subparsers = parser.add_subparsers(title='Commands')
-    add_commands(subparsers)
-    
-    parse_and_exec_command(parser)
-    
-
-def init_parser(prog: str = None, version: str = None, doc: str = None, *, config: ConfigParser = None, section: str = None):
-    parser = ArgumentParser(prog=prog, description=get_help_text(doc), formatter_class=RawTextHelpFormatter, add_help=False, epilog='\n'.join(doc.splitlines()[2:]) if doc else None)
-    
-    envs = VCenterClient.get_configured_envs(config=config, section=section)
-
-    group = parser.add_argument_group(title='General options')
-    group.add_argument('-e', '--env', default=os.environ.get('VMWARE_DEFAULT_ENV'), help=f"Name of the vCenter to use. Available: {', '.join(envs) if envs else 'none'}.")
-    group.add_argument('-h', '--help', action='help', help=f"Show this program help message and exit.")
-    group.add_argument('--version', action='version', version=f"{prog} {version or '?'}", help="Show version information and exit.")
-
-    return parser
-
-
-def add_commands(subparsers: _SubParsersAction[ArgumentParser]):
-    add_func_command(subparsers, export_inventory, name='inventory')
-    add_func_command(subparsers, dump, name='dump')
-
-    add_datastore_commands(subparsers, name='datastore')
-    add_net_commands(subparsers, name='net')
-    add_host_commands(subparsers, name='host')
-    add_vm_commands(subparsers, name='vm')
-    add_func_command(subparsers, customfield.list_customfields, name='customfield')
-
-    add_module_command(subparsers, autoreport)
-        
-
-def get_vcenter(handle: FunctionType, args: dict, *, config: ConfigParser = None, section: str = None):
-    if 'vcenter' in signature(handle).parameters:
-        env = args.pop('env', None)
-        vcenter = VCenterClient(env, config=config, section=section)
-        args['vcenter'] = vcenter    
-    else:
-        vcenter = nullcontext()
-
-    return vcenter
-        
-
-def parse_and_exec_command(parser: ArgumentParser, *, config: ConfigParser = None, section: str = None):    
-    args = vars(parser.parse_args())
-    handle = args.pop('handle', None)
-
-    with get_vcenter(handle, args, config=config, section=section):
-        exec_command(handle, args)
-
-
-if __name__ == '__main__':
-    main()
+"""
+Interact easily with your VMWare clusters.
+"""
+from __future__ import annotations
+
+import logging
+import os
+from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
+from configparser import ConfigParser
+from contextlib import nullcontext
+from inspect import signature
+from types import FunctionType
+
+from zut import (OutTable, add_func_command, add_module_command,
+                 configure_logging, exec_command, get_help_text,
+                 register_locale)
+
+from . import VCenterClient, __prog__, __version__, autoreport, customvalue
+from .cluster import add_cluster_commands
+from .resourcepool import add_resourcepool_commands
+from .datastore import add_datastore_commands
+from .dump import dump
+from .host import add_host_commands
+from .inventory import export_inventory
+from .net import add_net_commands
+from .tag import add_tag_commands
+from .vm import add_vm_commands
+from .perf import add_perf_commands
+
+logger = logging.getLogger(__name__)
+
+def main():
+    configure_logging()
+    register_locale(use_excel_csv=(os.environ.get('USE_EXCEL_CSV') or '1').lower() in ['1', 'yes', 'true', 'on'])
+    OutTable.DEFAULT_EXCEL_ATEXIT = (os.environ.get('DEFAULT_EXCEL_ATEXIT') or '1').lower() in ['1', 'yes', 'true', 'on']
+
+    parser = init_parser(__prog__, __version__, __doc__)
+
+    subparsers = parser.add_subparsers(title='Commands')
+    add_commands(subparsers)
+    
+    parse_and_exec_command(parser)
+    
+
+def init_parser(prog: str = None, version: str = None, doc: str = None, *, config: ConfigParser = None, section: str = None):
+    parser = ArgumentParser(prog=prog, description=get_help_text(doc), formatter_class=RawTextHelpFormatter, add_help=False, epilog='\n'.join(doc.splitlines()[2:]) if doc else None)
+    
+    envs = VCenterClient.get_configured_envs(config=config, section=section)
+
+    group = parser.add_argument_group(title='General options')
+    group.add_argument('-e', '--env', default=os.environ.get('VMWARE_DEFAULT_ENV'), help=f"Name of the vCenter to use. Available: {', '.join(envs) if envs else 'none'}.")
+    group.add_argument('-h', '--help', action='help', help=f"Show this program help message and exit.")
+    group.add_argument('--version', action='version', version=f"{prog} {version or '?'}", help="Show version information and exit.")
+
+    return parser
+
+
+def add_commands(subparsers: _SubParsersAction[ArgumentParser]):
+    add_func_command(subparsers, export_inventory, name='inventory')
+    add_func_command(subparsers, dump, name='dump')
+
+    add_cluster_commands(subparsers, name='cluster')
+    add_resourcepool_commands(subparsers, name='resourcepool')
+    add_datastore_commands(subparsers, name='datastore')
+    add_net_commands(subparsers, name='net')
+    add_host_commands(subparsers, name='host')
+    add_vm_commands(subparsers, name='vm')
+    add_func_command(subparsers, customvalue.list_custom_values, name='customvalue')
+    add_tag_commands(subparsers, name='tag')
+    
+    add_perf_commands(subparsers, name='perf')
+
+    add_module_command(subparsers, autoreport)
+        
+
+def get_vcenter(handle: FunctionType, args: dict, *, config: ConfigParser = None, section: str = None):
+    if 'vcenter' in signature(handle).parameters:
+        env = args.pop('env', None)
+        vcenter = VCenterClient(env, config=config, section=section)
+        args['vcenter'] = vcenter    
+    else:
+        vcenter = nullcontext()
+
+    return vcenter
+        
+
+def parse_and_exec_command(parser: ArgumentParser, *, config: ConfigParser = None, section: str = None):    
+    args = vars(parser.parse_args())
+    handle = args.pop('handle', None)
+
+    with get_vcenter(handle, args, config=config, section=section):
+        exec_command(handle, args)
+
+
+if __name__ == '__main__':
+    main()
```

## vmware_reporter/_version.py

```diff
@@ -1,16 +1,16 @@
-# file generated by setuptools_scm
-# don't change, don't track in version control
-TYPE_CHECKING = False
-if TYPE_CHECKING:
-    from typing import Tuple, Union
-    VERSION_TUPLE = Tuple[Union[int, str], ...]
-else:
-    VERSION_TUPLE = object
-
-version: str
-__version__: str
-__version_tuple__: VERSION_TUPLE
-version_tuple: VERSION_TUPLE
-
-__version__ = version = '0.3.0'
-__version_tuple__ = version_tuple = (0, 3, 0)
+# file generated by setuptools_scm
+# don't change, don't track in version control
+TYPE_CHECKING = False
+if TYPE_CHECKING:
+    from typing import Tuple, Union
+    VERSION_TUPLE = Tuple[Union[int, str], ...]
+else:
+    VERSION_TUPLE = object
+
+version: str
+__version__: str
+__version_tuple__: VERSION_TUPLE
+version_tuple: VERSION_TUPLE
+
+__version__ = version = '0.3.1'
+__version_tuple__ = version_tuple = (0, 3, 1)
```

## vmware_reporter/autoreport.py

```diff
@@ -1,39 +1,51 @@
-import os
-from argparse import ArgumentParser
-from io import IOBase
-
-from zut import files
-from zut.excel import is_excel_path, split_excel_path
-
-from . import VCenterClient
-from .customfield import list_customfields
-from .datastore import list_datastores, list_datastore_stats
-from .host import list_hosts
-from .net import list_nets
-from .vm import list_vms, list_vm_disks, list_vm_nics
-from .settings import CONFIG, CONFIG_SECTION
-
-_DEFAULT_OUT = CONFIG.get(CONFIG_SECTION, 'autoreport_out', fallback='autoreport.xlsx#{title}')
-
-def handle(vcenter: VCenterClient, out: os.PathLike|IOBase = _DEFAULT_OUT):
-    """
-    Export automatic report.
-    """
-    if is_excel_path(out, accept_table_suffix=True):
-        path, _ = split_excel_path(out, dir=vcenter.get_out_dir(), env=vcenter.env, title='__title__')
-        target = path.parent.joinpath('archives')
-        files.archivate(path, target, missing_ok=True, keep=True)
-
-    list_vms(vcenter, out=out)
-    list_vm_disks(vcenter, out=out)
-    list_vm_nics(vcenter, out=out)
-    list_hosts(vcenter, out=out)
-    list_nets(vcenter, out=out)
-    list_datastores(vcenter, out=out)
-    list_datastore_stats(vcenter, out=out)
-    list_customfields(vcenter, out=out)
-    
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output tables (default: %(default)s).")
-
-handle.add_arguments = _add_arguments
+import os
+from argparse import ArgumentParser
+from io import IOBase
+
+from zut import files
+from zut.excel import is_excel_path, split_excel_path
+
+from . import VCenterClient
+from .cluster import list_clusters
+from .customvalue import list_custom_values
+from .datastore import list_datastores, list_datastore_stats
+from .host import list_hosts
+from .net import list_nets
+from .resourcepool import list_resourcepool
+from .vm import list_vms, list_vm_disks, list_vm_nics
+from .tag import list_categories, list_tags
+from .perf import list_perf_counters, list_perf_intervals, list_perf_metrics
+from .settings import CONFIG, CONFIG_SECTION
+
+_DEFAULT_OUT = CONFIG.get(CONFIG_SECTION, 'autoreport_out', fallback='autoreport.xlsx#{title}')
+
+def handle(vcenter: VCenterClient, out: os.PathLike|IOBase = _DEFAULT_OUT):
+    """
+    Export automatic report.
+    """
+    if is_excel_path(out, accept_table_suffix=True):
+        path, _ = split_excel_path(out, dir=vcenter.out_dir, env=vcenter.env, title='__title__')
+        archives_dir = CONFIG.get(CONFIG_SECTION, 'autoreport_archives', fallback='archives')
+        target = files.join(files.dirname(path), archives_dir)
+        files.archivate(path, target, missing_ok=True, keep=True)
+
+    list_vms(vcenter, out=out)
+    list_vm_disks(vcenter, out=out)
+    list_vm_nics(vcenter, out=out)
+    list_hosts(vcenter, out=out)
+    list_nets(vcenter, out=out)
+    list_datastores(vcenter, out=out)
+    list_datastore_stats(vcenter, out=out)
+    list_clusters(vcenter, out=out)
+    list_resourcepool(vcenter, out=out)
+    list_perf_intervals(vcenter, out=out)
+    list_perf_counters(vcenter, out=out)
+    list_perf_metrics(vcenter, first=True, out=out)
+    list_categories(vcenter, out=out)
+    list_tags(vcenter, out=out)
+    list_custom_values(vcenter, out=out)
+    
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output tables (default: %(default)s).")
+
+handle.add_arguments = _add_arguments
```

## vmware_reporter/datastore.py

```diff
@@ -1,448 +1,448 @@
-"""
-Analyze datastores or perform operations on datastores.
-"""
-from __future__ import annotations
-
-import logging
-import os
-import re
-from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
-from contextlib import nullcontext
-from datetime import datetime
-from http import HTTPStatus
-from io import IOBase
-from pathlib import Path
-from typing import BinaryIO
-from urllib.parse import urlencode
-
-import requests
-from pyVmomi import vim
-from zut import (Header, add_func_command, get_description_text, get_help_text,
-                 out_table)
-
-from . import VCenterClient, get_obj_path, get_obj_ref
-
-_logger = logging.getLogger(__name__)
-
-
-def add_datastore_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
-    parser = commands_subparsers.add_parser(name, help=get_help_text(__doc__), description=get_description_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False)
-
-    group = parser.add_argument_group(title='Command options')
-    group.add_argument('-h', '--help', action='help', help=f"Show this command help message and exit.")
-
-    subparsers = parser.add_subparsers(title='Sub commands')
-    add_func_command(subparsers, list_datastores, name='list')
-    add_func_command(subparsers, list_datastore_elements, name='elements')
-    add_func_command(subparsers, list_datastore_stats, name='stats')
-    add_func_command(subparsers, download_from_datastore, name='download')
-    add_func_command(subparsers, upload_to_datastore, name='upload')
-    add_func_command(subparsers, delete_from_datastore, name='delete')
-
-
-_DEFAULT_OUT = '{title}.csv'
-
-
-def list_datastores(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: os.PathLike|IOBase = _DEFAULT_OUT):
-    headers = [
-        'name',
-        'ref',
-        'overall_status',
-        'config_status',
-        Header('capacity', fmt='gib'),
-        Header('freespace', fmt='gib'),
-        'accessible',
-        'maintenance_mode',
-        'vmfs_version',
-        'url',
-        'extent',
-        'multiple_host_access',
-        'host_access',
-    ]
-
-    with out_table(out, title='datastores', dir=vcenter.get_out_dir(), env=vcenter.env, headers=headers) as t:
-        for obj in vcenter.iter_objs(vim.Datastore, search, normalize=normalize, key=key):            
-            try:
-                _logger.info(f"Analyze datastore {obj.name}")
-
-                t.append([
-                    obj.name,
-                    get_obj_ref(obj),
-                    obj.overallStatus,
-                    obj.configStatus,
-                    obj.info.vmfs.capacity,
-                    obj.info.freeSpace,
-                    obj.summary.accessible,
-                    obj.summary.maintenanceMode,
-                    obj.info.vmfs.version,
-                    obj.info.url,
-                    parse_datacore_extent(obj.info.vmfs.extent),
-                    obj.summary.multipleHostAccess,
-                    get_datastore_host_summaries(obj),
-                ])
-            
-            except Exception as err:
-                _logger.exception(f"Error while analyzing {str(obj)}")
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('search', nargs='*', help="Search term(s).")
-    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
-    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
-    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output table (default: %(default)s).")
-
-list_datastores.add_arguments = _add_arguments
-
-
-def get_datastore_host_summaries(datastore: vim.Datastore):
-    summaries = []
-    for host_access in sorted(datastore.host, key=lambda ha: ha.key.name):
-        issue = ''
-
-        if not host_access.mountInfo.mounted:
-            issue = (', ' if issue else '') + f'notMounted'
-        elif not host_access.mountInfo.accessible:
-            issue = (', ' if issue else '') + f'notAccessible'
-
-        if host_access.mountInfo.accessMode != 'readWrite':
-            issue = (', ' if issue else '') + f'{host_access.mountInfo.accessMode}'
-
-        summaries.append(host_access.key.name + (f' [{issue}]' if issue else ''))
-
-    return summaries
-
-
-def parse_datacore_extent(extent: list[vim.host.ScsiDisk.Partition]):
-    if extent is None:
-        return None
-    return [part.diskName + ('' if part.partition == 1 else f' (partition {part.partition})') for part in extent]
-
-
-def iterate_datastore_elements(vcenter: VCenterClient, obj: vim.Datastore, path: str = None, *, pattern: str = None, max_depth: int = None, with_size: bool = True, with_mtime: bool = True, with_owner: bool = True, case_sensitive: bool = False):
-    """
-    Iterate over datastore elements (files and directories).
-    """
-    if path:
-        path = path.strip("/\\")
-        dspath = f"[{obj.name}] {path}"
-    else:
-        dspath = f"[{obj.name}]"
-
-    search_specs = {}
-    search_specs["searchCaseInsensitive"] = not case_sensitive
-
-    if with_size or with_mtime or with_owner:
-        details = vim.host.DatastoreBrowser.FileInfo.Details()
-        if with_size:
-            details.fileSize = True
-        if with_owner:
-            details.fileOwner = True
-        if with_mtime:
-            details.modification = True
-        search_specs["details"] = details
-
-    if pattern == "#folders":
-        search_specs["query"] = [vim.host.DatastoreBrowser.FolderQuery()]
-    elif pattern:
-        search_specs["matchPattern"] = [pattern]
-    
-    spec = vim.host.DatastoreBrowser.SearchSpec(**search_specs)
-
-    if max_depth is None:
-        task = obj.browser.SearchDatastoreSubFolders_Task(dspath, spec)
-        vcenter.wait_for_task(task)
-        for result in task.info.result:
-            for element in result.file:
-                yield DatastoreElement(obj, element, result.folderPath)
-    else:
-        task = obj.browser.SearchDatastore_Task(dspath, spec)
-        vcenter.wait_for_task(task)
-        for element in task.info.result.file:
-            info = DatastoreElement(obj, element, task.info.result.folderPath)
-            yield info
-            if info.is_folder and max_depth > 1:
-                yield from iterate_datastore_elements(vcenter, obj, info.path, pattern=pattern, max_depth=max_depth-1, with_size=with_size, with_mtime=with_mtime, with_owner=with_owner, case_sensitive=case_sensitive)
-
-
-def get_datastore_stats(vcenter: VCenterClient, obj: vim.Datastore, path: str = None, *, pattern: str = None, max_depth: int = 1, case_sensitive: bool = False) -> list[DatastoreStat]:
-    """
-    Return stats about datastore elements (files and directories).
-    """
-    stats: dict[str,DatastoreStat] = {}
-
-    for info in iterate_datastore_elements(vcenter, obj, path=path, case_sensitive=case_sensitive, pattern=pattern, with_mtime=True, with_owner=True, with_size=True):
-        path_split = info.path.split("/")
-        stat_path = "/".join(path_split[0:max_depth])
-        depth = len(path_split)
-
-        if stat_path in stats:
-            stat = stats[stat_path]
-        else:
-            stat = DatastoreStat(obj, stat_path)
-            stats[stat_path] = stat
-
-        stat.size += info.size or 0
-
-        if stat.mtime is None or info.mtime > stat.mtime:
-            stat.mtime = info.mtime
-
-        if stat.owner is None:
-            stat.owner = info.owner
-        elif stat.owner != info.owner:
-            stat.owner = "<multi>"
-
-        if depth > stat.depth:
-            stat.depth = depth
-
-        if info.path == stat_path:
-            stat.nature = info.nature
-        
-        if info.nature == "Folder":
-            stat.dir_count += 1
-        elif info.nature == "File":
-            stat.file_count += 1
-        else:
-            stat.other_count += 1
-
-    return sorted(stats.values(), key=lambda stat: stat.path)
-
-
-def list_datastore_elements(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', path: str = None, max_depth: int = None, out: os.PathLike|IOBase = _DEFAULT_OUT, bytes: bool = False):
-    """
-    List datastore elements (files and directories).
-    """
-    with out_table(out, headers=DatastoreElement.get_headers(bytes=bytes), title="datastore_elements", dir=vcenter.get_out_dir(), env=vcenter.env) as t:
-        for obj in vcenter.get_objs(vim.Datastore, search, normalize=normalize, key=key, sort_key='name'):
-            _logger.info(f'List datastore elements: {obj.name}')
-        
-            try:
-                for info in sorted(iterate_datastore_elements(vcenter, obj, path=path, max_depth=max_depth), key=lambda info: info.path):
-                    t.append(info.as_row())
-            except:
-                _logger.exception(f'Cannot analyze datastore {obj.name}')
-
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('search', nargs='*', help="Search term(s).")
-    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
-    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
-    parser.add_argument("--path", help="Detail elements only for the given path.")
-    parser.add_argument("--max-depth", type=int, help="Detail elements until the given depth (default: %(default)s).")
-    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output file (default: %(default)s).")
-    parser.add_argument('--bytes', action="store_true", help="Display size as bytes.")
-
-list_datastore_elements.add_arguments = _add_arguments
-
-
-def list_datastore_stats(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', path: str = None, max_depth: int = 1, out: os.PathLike|IOBase = _DEFAULT_OUT, bytes: bool = False):
-    """
-    Analyze stats about datastore elements (files and directories).
-    """
-    with out_table(out, headers=DatastoreStat.get_headers(bytes=bytes), title="datastore_stats", dir=vcenter.get_out_dir(), env=vcenter.env) as t:
-        for obj in vcenter.get_objs(vim.Datastore, search, normalize=normalize, key=key, sort_key='name'):
-            _logger.info(f'Analyze datastore stats: {obj.name}')
-
-            try:
-                for info in get_datastore_stats(vcenter, obj, path=path, max_depth=max_depth):
-                    t.append(info.as_row())
-            except:
-                _logger.exception(f'Cannot analyze datastore {obj.name}')
-
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('search', nargs='*', help="Search term(s).")
-    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
-    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
-    parser.add_argument("--path", help="Detail elements only for the given path.")
-    parser.add_argument("--max-depth", type=int, default=1, help="Detail elements until the given depth (default: %(default)s).")
-    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output file (default: %(default)s).")
-    parser.add_argument('--bytes', action="store_true", help="Display size as bytes.")
-
-list_datastore_stats.add_arguments = _add_arguments
-
-
-def request_datastore_resource(method: str, vcenter: VCenterClient, datastore: vim.Datastore|str, path: os.PathLike, data: BinaryIO = None):
-    datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
-
-    if not isinstance(path, Path):
-        path = Path(path)
-
-    path = "/folder/%s" % path.as_posix()
-    params = {"dsName": datastore_name, "dcPath": get_obj_path(vcenter.datacenter, full=True)}
-    url = f"https://{vcenter.host}" + path + '?' + urlencode(params)
-    
-    headers = {}
-    if data:
-        headers['Content-Type'] = 'application/octet-stream'
-
-    response = requests.request(method, url, data=data, headers=headers, cookies=vcenter.cookie, verify=not vcenter.no_ssl_verify)
-    response.raise_for_status()
-    return response
-
-
-def download_from_datastore(vcenter: VCenterClient, datastore: vim.Datastore|str, path: os.PathLike, target: os.PathLike = ''):
-    """
-    Download a file from a datastore.
-    """
-    if isinstance(target, str) and (target == '' or target.endswith(('/', '\\'))):
-        target += os.path.basename(path)
-
-    response = request_datastore_resource('GET', vcenter, datastore, path)
-    with open(target, 'wb') as fp:
-        for chunck in response.iter_content():
-            fp.write(chunck)
-    
-    datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
-    _logger.info("%s %s from datastore %s to %s", 'downloaded' if response.status_code == HTTPStatus.OK else f'{response.status_code} {response.reason}', path, datastore_name, target)
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('datastore', help="Name of the datastore.")
-    parser.add_argument('path', help="Path of the object to download on the datastore.")
-    parser.add_argument('target', nargs='?', default='', help="Target path on the local file system.")
-
-download_from_datastore.add_arguments = _add_arguments
-
-
-def upload_to_datastore(vcenter: VCenterClient, source: os.PathLike|BinaryIO, datastore: vim.Datastore|str, target: os.PathLike = ''):
-    """
-    Upload a file to a datastore.
-    """
-    if isinstance(target, str) and (target == '' or target.endswith(('/', '\\'))):
-        if isinstance(source, IOBase):
-            raise ValueError(f"Cannot upload to a directory ({target}): source is not a path")
-        target += os.path.basename(source)
-
-    if isinstance(source, IOBase) and hasattr(source, 'encoding'):
-        raise ValueError("Cannot send files opened in text mode")
-
-    with nullcontext(source) if isinstance(source, IOBase) else open(source, 'rb') as fp:
-        response = request_datastore_resource('PUT', vcenter, datastore, target, data=fp)
-    
-    datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
-    _logger.info("uploaded %s to datastore %s: %s %s", source, datastore_name, 'created' if response.status_code == HTTPStatus.CREATED else ('updated' if response.status_code == HTTPStatus.OK else f'{response.status_code} {response.reason}'), target)
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('source', help="Path of the source data.")
-    parser.add_argument('datastore', help="Name of the datastore.")
-    parser.add_argument('target', nargs='?', default='', help="Target path on the datastore.")
-
-upload_to_datastore.add_arguments = _add_arguments
-
-
-def delete_from_datastore(vcenter: VCenterClient, datastore: vim.Datastore|str, path: os.PathLike):
-    """
-    Delete a file from a datastore.
-    """
-    response = request_datastore_resource('DELETE', vcenter, datastore, path)
-    
-    datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
-    _logger.info("%s %s from datastore %s", 'deleted' if response.status_code == HTTPStatus.NO_CONTENT else f'{response.status_code} {response.reason}', path, datastore_name)
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('datastore', help="Name of the datastore.")
-    parser.add_argument('path', help="Path of the object to delete on the datastore.")
-
-delete_from_datastore.add_arguments = _add_arguments
-
-
-def remove_datastore_prefix(obj: vim.Datastore, dspath: str):
-    if dspath.startswith(f'[{obj.name}]'):
-        dspath = dspath[len(f'[{obj.name}]'):]
-        if dspath.startswith(' '):
-            dspath = dspath[1:]
-    return dspath
-
-
-class DatastoreElement:
-    def __init__(self, obj: vim.Datastore, info: vim.host.DatastoreBrowser.FileInfo, parent_dspath: str):
-        self.obj = obj
-        parent_dspath = remove_datastore_prefix(obj, parent_dspath)
-        self.path: str = parent_dspath + info.path
-
-        if isinstance(info, vim.host.DatastoreBrowser.FolderInfo):
-            self.nature = "Folder"
-        elif isinstance(info, vim.host.DatastoreBrowser.FileInfo):
-            self.nature = "File"
-        else:
-            # FloppyImageFileInfo, FolderFileInfo, IsoImageFileInfo, VmConfigFileInfo, VmDiskFileInfo, VmLogFileInfo, VmNvramFileInfo, VmSnapshotFileInfo
-            self.nature: str = type(info).__name__ 
-            if self.nature.endswith('FileInfo'):
-                self.nature = self.nature[:-len('FileInfo')]
-            
-        self.size: int|None = int(info.fileSize) if info.fileSize is not None else None
-        self.mtime: datetime|None = info.modification
-        self.owner: str|None = info.owner
-
-    @property
-    def is_folder(self):
-        return self.nature == 'Folder'
-
-
-    @classmethod
-    def get_headers(cls, *, bytes = False):
-        return [
-            'datastore',
-            'path',
-            'nature',
-            'size' if bytes else Header('size', fmt='gib'),
-            'mtime',
-            'owner',
-        ]
-
-    def as_row(self):
-        return [
-            self.obj.name,
-            self.path,
-            self.nature,
-            self.size,
-            self.mtime,
-            self.owner,
-        ]
-
-
-class DatastoreStat:
-    def __init__(self, obj: vim.Datastore, path: str):
-        self.obj = obj
-        self.path = path
-
-        self.nature: str|None = None
-        self.size: int = 0
-        self.mtime: datetime|None = None
-        self.owner: str|None = None
-
-        self.depth: int = 0
-        self.dir_count: int = 0
-        self.file_count: int = 0
-        self.other_count: int = 0
-
-    @property
-    def is_folder(self):
-        return self.nature == 'Folder'
-
-    @classmethod
-    def get_headers(cls, *, bytes = False):
-        return [
-            'datastore',
-            'path',
-            'nature',
-            'size' if bytes else Header('size', fmt='gib'),
-            'mtime',
-            'owner',
-            'depth',
-            'dir_count',
-            'file_count',
-            'other_count',
-        ]
-
-    def as_row(self):
-        return [
-            self.obj.name,
-            self.path,
-            self.nature,
-            self.size,
-            self.mtime,
-            self.owner,
-            self.depth,
-            self.dir_count,
-            self.file_count,
-            self.other_count,
-        ]
+"""
+Analyze datastores or perform operations on datastores.
+"""
+from __future__ import annotations
+
+import logging
+import os
+import re
+from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
+from contextlib import nullcontext
+from datetime import datetime
+from http import HTTPStatus
+from io import IOBase
+from pathlib import Path
+from typing import BinaryIO
+from urllib.parse import urlencode
+
+import requests
+from pyVmomi import vim
+from zut import (Header, add_func_command, get_description_text, get_help_text,
+                 out_table)
+
+from . import VCenterClient, get_obj_path, get_obj_ref
+
+_logger = logging.getLogger(__name__)
+
+
+def add_datastore_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
+    parser = commands_subparsers.add_parser(name, help=get_help_text(__doc__), description=get_description_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False)
+
+    group = parser.add_argument_group(title='Command options')
+    group.add_argument('-h', '--help', action='help', help=f"Show this command help message and exit.")
+
+    subparsers = parser.add_subparsers(title='Sub commands')
+    add_func_command(subparsers, list_datastores, name='list')
+    add_func_command(subparsers, list_datastore_elements, name='elements')
+    add_func_command(subparsers, list_datastore_stats, name='stats')
+    add_func_command(subparsers, download_from_datastore, name='download')
+    add_func_command(subparsers, upload_to_datastore, name='upload')
+    add_func_command(subparsers, delete_from_datastore, name='delete')
+
+
+_DEFAULT_OUT = '{title}.csv'
+
+
+def list_datastores(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: os.PathLike|IOBase = _DEFAULT_OUT):
+    headers = [
+        'name',
+        'ref',
+        'overall_status',
+        'config_status',
+        Header('capacity', fmt='gib'),
+        Header('freespace', fmt='gib'),
+        'accessible',
+        'maintenance_mode',
+        'vmfs_version',
+        'url',
+        'extent',
+        'multiple_host_access',
+        'host_access',
+    ]
+
+    with out_table(out, title='datastores', dir=vcenter.out_dir, env=vcenter.env, headers=headers) as t:
+        for obj in vcenter.iter_objs(vim.Datastore, search, normalize=normalize, key=key):            
+            try:
+                _logger.info(f"Analyze datastore {obj.name}")
+
+                t.append([
+                    obj.name,
+                    get_obj_ref(obj),
+                    obj.overallStatus,
+                    obj.configStatus,
+                    obj.info.vmfs.capacity,
+                    obj.info.freeSpace,
+                    obj.summary.accessible,
+                    obj.summary.maintenanceMode,
+                    obj.info.vmfs.version,
+                    obj.info.url,
+                    parse_datacore_extent(obj.info.vmfs.extent),
+                    obj.summary.multipleHostAccess,
+                    get_datastore_host_summaries(obj),
+                ])
+            
+            except Exception as err:
+                _logger.exception(f"Error while analyzing {str(obj)}")
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output table (default: %(default)s).")
+
+list_datastores.add_arguments = _add_arguments
+
+
+def get_datastore_host_summaries(datastore: vim.Datastore):
+    summaries = []
+    for host_access in sorted(datastore.host, key=lambda ha: ha.key.name):
+        issue = ''
+
+        if not host_access.mountInfo.mounted:
+            issue = (', ' if issue else '') + f'notMounted'
+        elif not host_access.mountInfo.accessible:
+            issue = (', ' if issue else '') + f'notAccessible'
+
+        if host_access.mountInfo.accessMode != 'readWrite':
+            issue = (', ' if issue else '') + f'{host_access.mountInfo.accessMode}'
+
+        summaries.append(host_access.key.name + (f' [{issue}]' if issue else ''))
+
+    return summaries
+
+
+def parse_datacore_extent(extent: list[vim.host.ScsiDisk.Partition]):
+    if extent is None:
+        return None
+    return [part.diskName + ('' if part.partition == 1 else f' (partition {part.partition})') for part in extent]
+
+
+def iterate_datastore_elements(vcenter: VCenterClient, obj: vim.Datastore, path: str = None, *, pattern: str = None, max_depth: int = None, with_size: bool = True, with_mtime: bool = True, with_owner: bool = True, case_sensitive: bool = False):
+    """
+    Iterate over datastore elements (files and directories).
+    """
+    if path:
+        path = path.strip("/\\")
+        dspath = f"[{obj.name}] {path}"
+    else:
+        dspath = f"[{obj.name}]"
+
+    search_specs = {}
+    search_specs["searchCaseInsensitive"] = not case_sensitive
+
+    if with_size or with_mtime or with_owner:
+        details = vim.host.DatastoreBrowser.FileInfo.Details()
+        if with_size:
+            details.fileSize = True
+        if with_owner:
+            details.fileOwner = True
+        if with_mtime:
+            details.modification = True
+        search_specs["details"] = details
+
+    if pattern == "#folders":
+        search_specs["query"] = [vim.host.DatastoreBrowser.FolderQuery()]
+    elif pattern:
+        search_specs["matchPattern"] = [pattern]
+    
+    spec = vim.host.DatastoreBrowser.SearchSpec(**search_specs)
+
+    if max_depth is None:
+        task = obj.browser.SearchDatastoreSubFolders_Task(dspath, spec)
+        vcenter.wait_for_task(task)
+        for result in task.info.result:
+            for element in result.file:
+                yield DatastoreElement(obj, element, result.folderPath)
+    else:
+        task = obj.browser.SearchDatastore_Task(dspath, spec)
+        vcenter.wait_for_task(task)
+        for element in task.info.result.file:
+            info = DatastoreElement(obj, element, task.info.result.folderPath)
+            yield info
+            if info.is_folder and max_depth > 1:
+                yield from iterate_datastore_elements(vcenter, obj, info.path, pattern=pattern, max_depth=max_depth-1, with_size=with_size, with_mtime=with_mtime, with_owner=with_owner, case_sensitive=case_sensitive)
+
+
+def get_datastore_stats(vcenter: VCenterClient, obj: vim.Datastore, path: str = None, *, pattern: str = None, max_depth: int = 1, case_sensitive: bool = False) -> list[DatastoreStat]:
+    """
+    Return stats about datastore elements (files and directories).
+    """
+    stats: dict[str,DatastoreStat] = {}
+
+    for info in iterate_datastore_elements(vcenter, obj, path=path, case_sensitive=case_sensitive, pattern=pattern, with_mtime=True, with_owner=True, with_size=True):
+        path_split = info.path.split("/")
+        stat_path = "/".join(path_split[0:max_depth])
+        depth = len(path_split)
+
+        if stat_path in stats:
+            stat = stats[stat_path]
+        else:
+            stat = DatastoreStat(obj, stat_path)
+            stats[stat_path] = stat
+
+        stat.size += info.size or 0
+
+        if stat.mtime is None or info.mtime > stat.mtime:
+            stat.mtime = info.mtime
+
+        if stat.owner is None:
+            stat.owner = info.owner
+        elif stat.owner != info.owner:
+            stat.owner = "<multi>"
+
+        if depth > stat.depth:
+            stat.depth = depth
+
+        if info.path == stat_path:
+            stat.nature = info.nature
+        
+        if info.nature == "Folder":
+            stat.dir_count += 1
+        elif info.nature == "File":
+            stat.file_count += 1
+        else:
+            stat.other_count += 1
+
+    return sorted(stats.values(), key=lambda stat: stat.path)
+
+
+def list_datastore_elements(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', path: str = None, max_depth: int = None, out: os.PathLike|IOBase = _DEFAULT_OUT, bytes: bool = False):
+    """
+    List datastore elements (files and directories).
+    """
+    with out_table(out, headers=DatastoreElement.get_headers(bytes=bytes), title="datastore_elements", dir=vcenter.out_dir, env=vcenter.env) as t:
+        for obj in vcenter.get_objs(vim.Datastore, search, normalize=normalize, key=key, sort_key='name'):
+            _logger.info(f'List datastore elements: {obj.name}')
+        
+            try:
+                for info in sorted(iterate_datastore_elements(vcenter, obj, path=path, max_depth=max_depth), key=lambda info: info.path):
+                    t.append(info.as_row())
+            except:
+                _logger.exception(f'Cannot analyze datastore {obj.name}')
+
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument("--path", help="Detail elements only for the given path.")
+    parser.add_argument("--max-depth", type=int, help="Detail elements until the given depth (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output file (default: %(default)s).")
+    parser.add_argument('--bytes', action="store_true", help="Display size as bytes.")
+
+list_datastore_elements.add_arguments = _add_arguments
+
+
+def list_datastore_stats(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', path: str = None, max_depth: int = 1, out: os.PathLike|IOBase = _DEFAULT_OUT, bytes: bool = False):
+    """
+    Analyze stats about datastore elements (files and directories).
+    """
+    with out_table(out, headers=DatastoreStat.get_headers(bytes=bytes), title="datastore_stats", dir=vcenter.out_dir, env=vcenter.env) as t:
+        for obj in vcenter.get_objs(vim.Datastore, search, normalize=normalize, key=key, sort_key='name'):
+            _logger.info(f'Analyze datastore stats: {obj.name}')
+
+            try:
+                for info in get_datastore_stats(vcenter, obj, path=path, max_depth=max_depth):
+                    t.append(info.as_row())
+            except:
+                _logger.exception(f'Cannot analyze datastore {obj.name}')
+
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument("--path", help="Detail elements only for the given path.")
+    parser.add_argument("--max-depth", type=int, default=1, help="Detail elements until the given depth (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output file (default: %(default)s).")
+    parser.add_argument('--bytes', action="store_true", help="Display size as bytes.")
+
+list_datastore_stats.add_arguments = _add_arguments
+
+
+def request_datastore_resource(method: str, vcenter: VCenterClient, datastore: vim.Datastore|str, path: os.PathLike, data: BinaryIO = None):
+    datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
+
+    if not isinstance(path, Path):
+        path = Path(path)
+
+    path = "/folder/%s" % path.as_posix()
+    params = {"dsName": datastore_name, "dcPath": get_obj_path(vcenter.datacenter, full=True)}
+    url = f"https://{vcenter.host}" + path + '?' + urlencode(params)
+    
+    headers = {}
+    if data:
+        headers['Content-Type'] = 'application/octet-stream'
+
+    response = requests.request(method, url, data=data, headers=headers, cookies=vcenter.cookie, verify=not vcenter.no_ssl_verify)
+    response.raise_for_status()
+    return response
+
+
+def download_from_datastore(vcenter: VCenterClient, datastore: vim.Datastore|str, path: os.PathLike, target: os.PathLike = ''):
+    """
+    Download a file from a datastore.
+    """
+    if isinstance(target, str) and (target == '' or target.endswith(('/', '\\'))):
+        target += os.path.basename(path)
+
+    response = request_datastore_resource('GET', vcenter, datastore, path)
+    with open(target, 'wb') as fp:
+        for chunck in response.iter_content():
+            fp.write(chunck)
+    
+    datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
+    _logger.info("%s %s from datastore %s to %s", 'downloaded' if response.status_code == HTTPStatus.OK else f'{response.status_code} {response.reason}', path, datastore_name, target)
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('datastore', help="Name of the datastore.")
+    parser.add_argument('path', help="Path of the object to download on the datastore.")
+    parser.add_argument('target', nargs='?', default='', help="Target path on the local file system.")
+
+download_from_datastore.add_arguments = _add_arguments
+
+
+def upload_to_datastore(vcenter: VCenterClient, source: os.PathLike|BinaryIO, datastore: vim.Datastore|str, target: os.PathLike = ''):
+    """
+    Upload a file to a datastore.
+    """
+    if isinstance(target, str) and (target == '' or target.endswith(('/', '\\'))):
+        if isinstance(source, IOBase):
+            raise ValueError(f"Cannot upload to a directory ({target}): source is not a path")
+        target += os.path.basename(source)
+
+    if isinstance(source, IOBase) and hasattr(source, 'encoding'):
+        raise ValueError("Cannot send files opened in text mode")
+
+    with nullcontext(source) if isinstance(source, IOBase) else open(source, 'rb') as fp:
+        response = request_datastore_resource('PUT', vcenter, datastore, target, data=fp)
+    
+    datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
+    _logger.info("uploaded %s to datastore %s: %s %s", source, datastore_name, 'created' if response.status_code == HTTPStatus.CREATED else ('updated' if response.status_code == HTTPStatus.OK else f'{response.status_code} {response.reason}'), target)
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('source', help="Path of the source data.")
+    parser.add_argument('datastore', help="Name of the datastore.")
+    parser.add_argument('target', nargs='?', default='', help="Target path on the datastore.")
+
+upload_to_datastore.add_arguments = _add_arguments
+
+
+def delete_from_datastore(vcenter: VCenterClient, datastore: vim.Datastore|str, path: os.PathLike):
+    """
+    Delete a file from a datastore.
+    """
+    response = request_datastore_resource('DELETE', vcenter, datastore, path)
+    
+    datastore_name = datastore.name if isinstance(datastore, vim.Datastore) else datastore
+    _logger.info("%s %s from datastore %s", 'deleted' if response.status_code == HTTPStatus.NO_CONTENT else f'{response.status_code} {response.reason}', path, datastore_name)
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('datastore', help="Name of the datastore.")
+    parser.add_argument('path', help="Path of the object to delete on the datastore.")
+
+delete_from_datastore.add_arguments = _add_arguments
+
+
+def remove_datastore_prefix(obj: vim.Datastore, dspath: str):
+    if dspath.startswith(f'[{obj.name}]'):
+        dspath = dspath[len(f'[{obj.name}]'):]
+        if dspath.startswith(' '):
+            dspath = dspath[1:]
+    return dspath
+
+
+class DatastoreElement:
+    def __init__(self, obj: vim.Datastore, info: vim.host.DatastoreBrowser.FileInfo, parent_dspath: str):
+        self.obj = obj
+        parent_dspath = remove_datastore_prefix(obj, parent_dspath)
+        self.path: str = parent_dspath + info.path
+
+        if isinstance(info, vim.host.DatastoreBrowser.FolderInfo):
+            self.nature = "Folder"
+        elif isinstance(info, vim.host.DatastoreBrowser.FileInfo):
+            self.nature = "File"
+        else:
+            # FloppyImageFileInfo, FolderFileInfo, IsoImageFileInfo, VmConfigFileInfo, VmDiskFileInfo, VmLogFileInfo, VmNvramFileInfo, VmSnapshotFileInfo
+            self.nature: str = type(info).__name__ 
+            if self.nature.endswith('FileInfo'):
+                self.nature = self.nature[:-len('FileInfo')]
+            
+        self.size: int|None = int(info.fileSize) if info.fileSize is not None else None
+        self.mtime: datetime|None = info.modification
+        self.owner: str|None = info.owner
+
+    @property
+    def is_folder(self):
+        return self.nature == 'Folder'
+
+
+    @classmethod
+    def get_headers(cls, *, bytes = False):
+        return [
+            'datastore',
+            'path',
+            'nature',
+            'size' if bytes else Header('size', fmt='gib'),
+            'mtime',
+            'owner',
+        ]
+
+    def as_row(self):
+        return [
+            self.obj.name,
+            self.path,
+            self.nature,
+            self.size,
+            self.mtime,
+            self.owner,
+        ]
+
+
+class DatastoreStat:
+    def __init__(self, obj: vim.Datastore, path: str):
+        self.obj = obj
+        self.path = path
+
+        self.nature: str|None = None
+        self.size: int = 0
+        self.mtime: datetime|None = None
+        self.owner: str|None = None
+
+        self.depth: int = 0
+        self.dir_count: int = 0
+        self.file_count: int = 0
+        self.other_count: int = 0
+
+    @property
+    def is_folder(self):
+        return self.nature == 'Folder'
+
+    @classmethod
+    def get_headers(cls, *, bytes = False):
+        return [
+            'datastore',
+            'path',
+            'nature',
+            'size' if bytes else Header('size', fmt='gib'),
+            'mtime',
+            'owner',
+            'depth',
+            'dir_count',
+            'file_count',
+            'other_count',
+        ]
+
+    def as_row(self):
+        return [
+            self.obj.name,
+            self.path,
+            self.nature,
+            self.size,
+            self.mtime,
+            self.owner,
+            self.depth,
+            self.dir_count,
+            self.file_count,
+            self.other_count,
+        ]
```

## vmware_reporter/dump.py

```diff
@@ -1,65 +1,65 @@
-"""
-Dump all available data about VMWare managed objects.
-"""
-from __future__ import annotations
-
-import logging
-import os
-import re
-import sys
-from argparse import ArgumentParser
-from io import IOBase
-
-from . import VCenterClient, get_obj_ref, dump_obj
-
-_logger = logging.getLogger(__name__)
-
-_DEFAULT_OUT = os.path.join("dumps", "{type}", "{name} ({ref}).json")
-
-
-def dump(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', first: bool = False, types: list[type|str]|type|str = None, out: os.PathLike|IOBase = _DEFAULT_OUT):
-    """
-    Export all available data about VMWare managed objects to JSON files.
-    """
-    if not out or out == 'stdout':
-        out = sys.stdout
-    elif out == 'stderr':
-        out = sys.stderr
-    elif not isinstance(out, IOBase):
-        if not isinstance(out, str):
-            out = str(out)
-        if not '{name}' in out and not '{ref}' in out:
-            raise ValueError("out must contain {name} or {ref} placeholder")
-
-    first_types = []
-
-    for obj in vcenter.iter_objs(types, search, normalize=normalize, key=key):
-        if first:
-            if type(obj) in first_types:
-                continue
-
-        name = obj.name
-        ref = get_obj_ref(obj)
-        
-        if isinstance(out, IOBase):
-            obj_out = out
-        else:
-            obj_out = os.path.join(vcenter.get_out_dir(), str(out).format(type=type(obj).__name__, name=name, ref=ref, env=vcenter.env))
-            obj_out_dir = os.path.dirname(obj_out)
-            if obj_out_dir:
-                os.makedirs(obj_out_dir, exist_ok=True)
-        
-        dump_obj(obj, obj_out, title=f'{name} ({ref})')
-
-        if first:
-            first_types.append(type(obj))
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('search', nargs='*', help="Search term(s).")
-    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
-    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
-    parser.add_argument('-t', '--type', dest='types', metavar='type', help="Managed object type name (example: datastore).")
-    parser.add_argument('--first', action='store_true', help="Only handle the first object found for each type.")
-    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output JSON file (default: %(default)s).")
-
-dump.add_arguments = _add_arguments
+"""
+Dump all available data about VMWare managed objects.
+"""
+from __future__ import annotations
+
+import logging
+import os
+import re
+import sys
+from argparse import ArgumentParser
+from io import IOBase
+
+from . import VCenterClient, get_obj_name, get_obj_ref, get_obj_typename, dump_obj
+
+_logger = logging.getLogger(__name__)
+
+_DEFAULT_OUT = os.path.join("dumps", "{type}", "{name} ({ref}).json")
+
+
+def dump(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', first: bool = False, types: list[type|str]|type|str = None, out: os.PathLike|IOBase = _DEFAULT_OUT):
+    """
+    Export all available data about VMWare managed objects to JSON files.
+    """
+    if not out or out == 'stdout':
+        out = sys.stdout
+    elif out == 'stderr':
+        out = sys.stderr
+    elif not isinstance(out, IOBase):
+        if not isinstance(out, str):
+            out = str(out)
+        if not '{name}' in out and not '{ref}' in out:
+            raise ValueError("out must contain {name} or {ref} placeholder")
+
+    first_types = []
+
+    for obj in vcenter.iter_objs(types, search, normalize=normalize, key=key):
+        if first:
+            if type(obj) in first_types:
+                continue
+
+        name = get_obj_name(obj)
+        ref = get_obj_ref(obj)
+        
+        if isinstance(out, IOBase):
+            obj_out = out
+        else:
+            obj_out = os.path.join(vcenter.out_dir, str(out).format(type=get_obj_typename(obj), name=name, ref=ref, env=vcenter.env))
+            obj_out_dir = os.path.dirname(obj_out)
+            if obj_out_dir:
+                os.makedirs(obj_out_dir, exist_ok=True)
+        
+        dump_obj(obj, obj_out, title=f'{name} ({ref})')
+
+        if first:
+            first_types.append(type(obj))
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument('--first', action='store_true', help="Only handle the first object found for each type.")
+    parser.add_argument('-t', '--type', dest='types', metavar='type', help="Managed object type name (example: datastore).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output JSON file (default: %(default)s).")
+
+dump.add_arguments = _add_arguments
```

## vmware_reporter/host.py

```diff
@@ -1,105 +1,107 @@
-"""
-Manage ESXi hosts.
-"""
-from __future__ import annotations
-
-import logging
-import os
-import re
-from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
-from io import IOBase
-
-from pyVmomi import vim
-from zut import (Header, add_func_command, get_description_text, get_help_text,
-                 out_table)
-
-from . import VCenterClient, dictify_value, get_obj_ref
-
-_logger = logging.getLogger(__name__)
-
-def add_host_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
-    parser = commands_subparsers.add_parser(name, help=get_help_text(__doc__), description=get_description_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False)
-
-    group = parser.add_argument_group(title='Command options')
-    group.add_argument('-h', '--help', action='help', help=f"Show this command help message and exit.")
-
-    subparsers = parser.add_subparsers(title='Sub commands')
-    add_func_command(subparsers, list_hosts, name='list')
-
-
-_DEFAULT_OUT = 'hosts.csv'
-
-
-#region List
-
-def list_hosts(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: os.PathLike|IOBase = _DEFAULT_OUT):
-    headers = [
-        'name',
-        'ref',
-        'overall_status',
-        'config_status',
-        'cpu_packages',
-        'cpu_cores',
-        Header('memory', fmt='gib'),
-        'cluster',
-        'state',        
-        'power_state',
-        'standby_mode',
-        'connection_state',
-        'maintenance_mode',
-        'quarantine_mode',
-        'reboot_required',
-        'boot_time',
-        'vmware_product',
-        'vendor',
-        'model',
-        'serial',
-        'enclosure',
-        'cpu_model',
-    ]
-
-    with out_table(out, title='hosts', dir=vcenter.get_out_dir(), env=vcenter.env, headers=headers, after1970=True) as t:
-        for obj in vcenter.iter_objs(vim.HostSystem, search, normalize=normalize, key=key):  
-            try:
-                _logger.info(f"Analyze host {obj.name}")
-
-                oii = dictify_value(obj.hardware.systemInfo.otherIdentifyingInfo)
-
-                t.append([
-                    obj.name,
-                    get_obj_ref(obj),
-                    obj.overallStatus,
-                    obj.configStatus,
-                    obj.hardware.cpuInfo.numCpuPackages,
-                    obj.hardware.cpuInfo.numCpuCores,
-                    obj.hardware.memorySize,
-                    obj.parent.name if obj.parent and obj.parent != obj else None,
-                    obj.runtime.dasHostState.state if obj.runtime.dasHostState else None,                                        
-                    obj.runtime.powerState,
-                    obj.runtime.standbyMode,
-                    obj.runtime.connectionState,
-                    obj.runtime.inMaintenanceMode,
-                    obj.runtime.inQuarantineMode,
-                    obj.summary.rebootRequired,
-                    obj.runtime.bootTime,
-                    obj.config.product.fullName,
-                    obj.hardware.systemInfo.vendor,
-                    obj.hardware.systemInfo.model,
-                    oii.get('SerialNumberTag'),
-                    oii.get('EnclosureSerialNumberTag'),
-                    obj.summary.hardware.cpuModel,
-                ])
-            
-            except Exception as err:
-                _logger.exception(f"Error while analyzing {str(obj)}")
-
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('search', nargs='*', help="Search term(s).")
-    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
-    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
-    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output table (default: %(default)s).")
-
-list_hosts.add_arguments = _add_arguments
-
-#endregion
+"""
+Manage ESXi hosts.
+"""
+from __future__ import annotations
+
+import logging
+import os
+import re
+from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
+from io import IOBase
+
+from pyVmomi import vim
+from zut import (Header, add_func_command, get_description_text, get_help_text,
+                 out_table)
+
+from . import VCenterClient, dictify_value, get_obj_ref
+
+_logger = logging.getLogger(__name__)
+
+def add_host_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
+    parser = commands_subparsers.add_parser(name, help=get_help_text(__doc__), description=get_description_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False)
+
+    group = parser.add_argument_group(title='Command options')
+    group.add_argument('-h', '--help', action='help', help=f"Show this command help message and exit.")
+
+    subparsers = parser.add_subparsers(title='Sub commands')
+    add_func_command(subparsers, list_hosts, name='list')
+
+
+_DEFAULT_OUT = 'hosts.csv'
+
+
+#region List
+
+def list_hosts(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: os.PathLike|IOBase = _DEFAULT_OUT):
+    headers = [
+        'name',
+        'ref',
+        'overall_status',
+        'config_status',
+        'cpu_cores',
+        'cpu_mhz',
+        Header('memory', fmt='gib'),
+        'cluster',
+        'state',        
+        'power_state',
+        'standby_mode',
+        'connection_state',
+        'maintenance_mode',
+        'quarantine_mode',
+        'reboot_required',
+        'boot_time',
+        'vmware_product',
+        'vendor',
+        'model',
+        'serial',
+        'enclosure',
+        'cpu_packages',
+        'cpu_model',
+    ]
+
+    with out_table(out, title='hosts', dir=vcenter.out_dir, env=vcenter.env, headers=headers, after1970=True) as t:
+        for obj in vcenter.iter_objs(vim.HostSystem, search, normalize=normalize, key=key):  
+            try:
+                _logger.info(f"Analyze host {obj.name}")
+
+                oii = dictify_value(obj.hardware.systemInfo.otherIdentifyingInfo)
+
+                t.append([
+                    obj.name,
+                    get_obj_ref(obj),
+                    obj.overallStatus,
+                    obj.configStatus,
+                    obj.hardware.cpuInfo.numCpuCores,
+                    obj.summary.hardware.cpuMhz,
+                    obj.hardware.memorySize,
+                    obj.parent.name if obj.parent and obj.parent != obj else None,
+                    obj.runtime.dasHostState.state if obj.runtime.dasHostState else None,                                        
+                    obj.runtime.powerState,
+                    obj.runtime.standbyMode,
+                    obj.runtime.connectionState,
+                    obj.runtime.inMaintenanceMode,
+                    obj.runtime.inQuarantineMode,
+                    obj.summary.rebootRequired,
+                    obj.runtime.bootTime,
+                    obj.config.product.fullName,
+                    obj.hardware.systemInfo.vendor,
+                    obj.hardware.systemInfo.model,
+                    oii.get('SerialNumberTag'),
+                    oii.get('EnclosureSerialNumberTag'),
+                    obj.hardware.cpuInfo.numCpuPackages,
+                    obj.summary.hardware.cpuModel,
+                ])
+            
+            except Exception as err:
+                _logger.exception(f"Error while analyzing {str(obj)}")
+
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output table (default: %(default)s).")
+
+list_hosts.add_arguments = _add_arguments
+
+#endregion
```

## vmware_reporter/inventory.py

```diff
@@ -1,217 +1,230 @@
-"""
-Inventory of VMWare managed objects.
-"""
-from __future__ import annotations
-
-import logging
-import os
-import sys
-from argparse import ArgumentParser
-from contextlib import nullcontext
-from io import IOBase
-
-from pyVmomi import vim
-
-from . import VCenterClient, get_obj_ref
-
-_logger = logging.getLogger(__name__)
-
-_DEFAULT_OUT = "inventory.yml"
-
-
-def export_inventory(vcenter: VCenterClient, assets: list[str] = None, out: os.PathLike|IOBase = _DEFAULT_OUT):
-    """
-    Export an inventory of VMWare managed objects to a YAML file.
-    """
-    inventory = build_inventory(vcenter, assets=assets)
-    
-    if not out or out == 'stdout':
-        out = sys.stdout
-    elif out == 'stderr':
-        out = sys.stderr
-
-    if isinstance(out, IOBase):
-        out_name = getattr(out, 'name', '<io>')
-    else:
-        out = os.path.join(vcenter.get_out_dir(), str(out).format(env=vcenter.env))
-        out_name = str(out)
-        
-    _logger.info(f"export inventory to {out_name}")
-    inventory.to_yaml(out)
-
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output YAML file (default: %(default)s).")
-    parser.add_argument('--asset', nargs='*', dest='assets')
-
-export_inventory.add_arguments = _add_arguments
-
-
-def build_inventory(vcenter: VCenterClient, assets: list[str] = None) -> InventoryNode:
-    node = InventoryNode(vcenter.env, nature=VCenterClient)
-
-    if not assets:
-        assets = ['folder', 'license', 'authorization']
-
-    for asset in assets:
-        if asset == 'folder':
-            _logger.info(f"build folder inventory")
-            build_folder_inventory(vcenter, parent=node)
-            
-        elif asset == 'authorization':
-            _logger.info(f"build authorization inventory")
-            build_authorization_inventory(vcenter, parent=node)
-        
-        elif asset == 'license':
-            _logger.info(f"build license inventory")
-            build_license_inventory(vcenter, parent=node)
-
-        else:
-            _logger.error(f"Unknown asset: {asset}")
-
-    return node
-
-
-def build_folder_inventory(vcenter: VCenterClient, parent = None) -> InventoryNode:
-    found_by_ref: dict[str,vim.ManagedEntity] = {}
-
-    def recurse_tree(obj: vim.ManagedEntity, parent: InventoryNode):
-        ref = get_obj_ref(obj)
-        name = obj.name
-        found_by_ref[ref] = obj
-        node = InventoryNode(name, nature=type(obj), ref=ref, parent=parent)
-
-        if isinstance(obj, vim.Datacenter):
-            datastore_node = InventoryNode("(datastores)", parent=node)
-            for sub in obj.datastore:
-                recurse_tree(sub,datastore_node)
-            
-            network_node = InventoryNode("(networks)", parent=node)
-            for sub in obj.network:
-                recurse_tree(sub, network_node)
-        
-            recurse_tree(obj.datastoreFolder, node)
-            recurse_tree(obj.networkFolder, node)
-            recurse_tree(obj.hostFolder, node)
-            recurse_tree(obj.vmFolder, node)
-
-        elif isinstance(obj, vim.ComputeResource):
-            host_node = InventoryNode("(hosts)", parent=node)
-            for sub in obj.host:
-                recurse_tree(sub, host_node)
-
-            recurse_tree(obj.resourcePool, node)
-
-        if hasattr(obj, 'childEntity'):
-            for sub in obj.childEntity:
-                recurse_tree(sub, node)
-
-        return node
-
-    # Walk through the tree starting from root folder
-    node = recurse_tree(vcenter.service_content.rootFolder, parent)
-
-    # Search through the container view
-    view = None
-    try:
-        view = vcenter.service_content.viewManager.CreateContainerView(vcenter.service_content.rootFolder, recursive=True)
-        additional_node = None
-        for obj in view.view:
-            ref = get_obj_ref(obj)
-            if not found_by_ref.pop(ref, None):
-                if not additional_node:
-                    additional_node = InventoryNode('(found in container view but not in folder tree)', parent=node)
-            
-                name = obj.name
-                InventoryNode(name, nature=type(obj), ref=ref, child_of=f'{obj.parent.name} ({get_obj_ref(obj.parent)})', parent=additional_node)
-    finally:
-        if view:
-            view.Destroy()
-
-    # Show elements missing in the container view
-    additional_node = None
-    for ref, obj in found_by_ref.items():
-        if obj == vcenter.service_content.rootFolder:
-            continue
-
-        if not additional_node:
-            additional_node = InventoryNode('(found in folder tree but not in container view)', parent=node)
-    
-        name = obj.name
-        InventoryNode(name, nature=type(obj), ref=ref, child_of=f'{obj.parent.name} ({get_obj_ref(obj.parent)})', parent=additional_node)
-
-    return node
-
-
-def build_authorization_inventory(vcenter: VCenterClient, parent = None) -> InventoryNode:
-    node = InventoryNode("(roles)", parent=parent)
-
-    role_nodes = {}
-    for role in vcenter.service_content.authorizationManager.roleList:
-        role_node = InventoryNode(role.name, nature=type(role), id=role.roleId, parent=node)
-        role_node._user_node = None
-        role_node._group_node = None
-        role_nodes[role.roleId] = role_node
-
-    principal_nodes: dict[str,InventoryNode] = {}
-    for permission in vcenter.service_content.authorizationManager.RetrieveAllPermissions():
-        role_node = role_nodes[permission.roleId]
-
-        if permission.group:
-            if not role_node._group_node:
-                role_node._group_node = InventoryNode("(groups)", parent=role_node)
-            parent = role_node._group_node
-            nature = 'group'
-        else:
-            if not role_node._user_node:
-                role_node._user_node = InventoryNode("(users)", parent=role_node)
-            parent = role_node._user_node
-            nature = 'user'
-
-        if permission.principal in principal_nodes:
-            principal_node = principal_nodes[permission.principal]
-        else:
-            principal_node = InventoryNode(permission.principal, nature=nature, parent=parent)
-
-        ref = get_obj_ref(permission.entity)
-        name = permission.entity.name
-        InventoryNode(name, nature=f"{type(permission.entity).__name__} permission", ref=ref, propagate=permission.propagate, parent=principal_node)
-
-
-def build_license_inventory(vcenter: VCenterClient, parent = None) -> InventoryNode:
-    node = InventoryNode("(licenses)", parent=parent)
-
-    for license in vcenter.service_content.licenseManager.licenses:
-        InventoryNode(license.name, nature=type(license), key=license.licenseKey, parent=node)
-
-
-class InventoryNode:
-    indent_size = 2
-
-    def __init__(self, name: str, *, nature: type|str = None, parent: InventoryNode = None, **attrs):
-        self.name = name        
-        self.nature = nature.__name__ if isinstance(nature, type) else (str(nature) if nature else None)
-        self.parent = parent
-        self.attrs = attrs
-        self.children: list[InventoryNode] = []
-        if parent:
-            parent.children.append(self)
-
-    def __str__(self):
-        result = self.name
-        need_comma = True
-        if self.nature:
-            result += f' [{self.nature}]'
-            need_comma = False
-
-        for name, value in self.attrs.items():
-            result += (', ' if need_comma else ' ') + f'{name}={value}'
-            need_comma = True
-
-        return result
-
-    def to_yaml(self, file, depth = 0):
-        with nullcontext(file) if isinstance(file, IOBase) else open(file, 'w', encoding='utf-8') as fp:
-            print(f"{' ' * self.indent_size * depth + '- ' if depth > 0 else ''}{self}:", file=fp)
-            for child in self.children:
-                child.to_yaml(fp, depth+1)
+"""
+Inventory of VMWare managed objects.
+"""
+from __future__ import annotations
+
+import logging
+import os
+import sys
+from argparse import ArgumentParser
+from contextlib import nullcontext
+from io import IOBase
+
+from pyVmomi import vim
+
+from . import VCenterClient, get_obj_name, get_obj_ref
+
+_logger = logging.getLogger(__name__)
+
+_DEFAULT_OUT = "inventory.yml"
+
+
+def export_inventory(vcenter: VCenterClient, assets: list[str] = None, out: os.PathLike|IOBase = _DEFAULT_OUT):
+    """
+    Export an inventory of VMWare managed objects to a YAML file.
+    """
+    inventory = build_inventory(vcenter, assets=assets)
+    
+    if not out or out == 'stdout':
+        out = sys.stdout
+    elif out == 'stderr':
+        out = sys.stderr
+
+    if isinstance(out, IOBase):
+        out_name = getattr(out, 'name', '<io>')
+    else:
+        out = os.path.join(vcenter.out_dir, str(out).format(env=vcenter.env))
+        out_name = str(out)
+        
+    _logger.info(f"export inventory to {out_name}")
+    inventory.to_yaml(out)
+
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output YAML file (default: %(default)s).")
+    parser.add_argument('--asset', nargs='*', dest='assets')
+
+export_inventory.add_arguments = _add_arguments
+
+
+def build_inventory(vcenter: VCenterClient, assets: list[str] = None) -> InventoryNode:
+    node = InventoryNode(vcenter.env, nature=VCenterClient)
+
+    if not assets:
+        assets = ['folder', 'license', 'authorization']
+
+    for asset in assets:
+        if asset == 'folder':
+            _logger.info(f"build folder inventory")
+            build_folder_inventory(vcenter, parent=node)
+            
+        elif asset == 'authorization':
+            _logger.info(f"build authorization inventory")
+            build_authorization_inventory(vcenter, parent=node)
+        
+        elif asset == 'license':
+            _logger.info(f"build license inventory")
+            build_license_inventory(vcenter, parent=node)
+
+        else:
+            _logger.error(f"Unknown asset: {asset}")
+
+    return node
+
+
+def build_folder_inventory(vcenter: VCenterClient, parent = None) -> InventoryNode:
+    found_by_ref: dict[str,vim.ManagedEntity] = {}
+
+    def recurse_tree(obj: vim.ManagedEntity, parent: InventoryNode):
+        ref = get_obj_ref(obj)
+        name = get_obj_name(obj)
+        found_by_ref[ref] = obj
+        node = InventoryNode(name, nature=type(obj), ref=ref, parent=parent)
+
+        if isinstance(obj, vim.Datacenter):
+            datastore_node = InventoryNode("(datastores)", parent=node)
+            for sub in obj.datastore:
+                recurse_tree(sub,datastore_node)
+            
+            network_node = InventoryNode("(networks)", parent=node)
+            for sub in obj.network:
+                recurse_tree(sub, network_node)
+        
+            recurse_tree(obj.datastoreFolder, node)
+            recurse_tree(obj.networkFolder, node)
+            recurse_tree(obj.hostFolder, node)
+            recurse_tree(obj.vmFolder, node)
+
+        elif isinstance(obj, vim.ComputeResource):
+            host_node = InventoryNode("(hosts)", parent=node)
+            for sub in obj.host:
+                recurse_tree(sub, host_node)
+
+            recurse_tree(obj.resourcePool, node)
+
+        if hasattr(obj, 'childEntity'):
+            for sub in obj.childEntity:
+                recurse_tree(sub, node)
+
+        return node
+
+    # Walk through the tree starting from root folder
+    node = recurse_tree(vcenter.service_content.rootFolder, parent)
+
+    # Search through the container view
+    view = None
+    try:
+        view = vcenter.service_content.viewManager.CreateContainerView(vcenter.service_content.rootFolder, recursive=True)
+        additional_node = None
+        for obj in view.view:
+            ref = get_obj_ref(obj)
+            if not found_by_ref.pop(ref, None):
+                if not additional_node:
+                    additional_node = InventoryNode('(found in container view but not in folder tree)', parent=node)
+            
+                name = get_obj_name(obj)
+                InventoryNode(name, nature=type(obj), ref=ref, child_of=f'{get_obj_name(obj.parent)} ({get_obj_ref(obj.parent)})', parent=additional_node)
+    finally:
+        if view:
+            view.Destroy()
+
+    # Show elements missing in the container view
+    additional_node = None
+    for ref, obj in found_by_ref.items():
+        if obj == vcenter.service_content.rootFolder:
+            continue
+
+        if not additional_node:
+            additional_node = InventoryNode('(found in folder tree but not in container view)', parent=node)
+    
+        name = get_obj_name(obj)
+        InventoryNode(name, nature=type(obj), ref=ref, child_of=f'{get_obj_name(obj.parent)} ({get_obj_ref(obj.parent)})', parent=additional_node)
+
+    return node
+
+
+def build_authorization_inventory(vcenter: VCenterClient, parent = None) -> InventoryNode:
+    node = InventoryNode("(roles)", parent=parent)
+
+    role_nodes = {}
+    for role in vcenter.service_content.authorizationManager.roleList:
+        role_node = InventoryNode(role.name, nature=type(role), id=role.roleId, parent=node)
+        role_node._user_node = None
+        role_node._group_node = None
+        role_nodes[role.roleId] = role_node
+
+    principal_nodes: dict[str,InventoryNode] = {}
+    for permission in vcenter.service_content.authorizationManager.RetrieveAllPermissions():
+        role_node = role_nodes[permission.roleId]
+
+        if permission.group:
+            if not role_node._group_node:
+                role_node._group_node = InventoryNode("(groups)", parent=role_node)
+            parent = role_node._group_node
+            nature = 'group'
+        else:
+            if not role_node._user_node:
+                role_node._user_node = InventoryNode("(users)", parent=role_node)
+            parent = role_node._user_node
+            nature = 'user'
+
+        if permission.principal in principal_nodes:
+            principal_node = principal_nodes[permission.principal]
+        else:
+            principal_node = InventoryNode(permission.principal, nature=nature, parent=parent)
+
+        ref = get_obj_ref(permission.entity)
+        name = permission.entity.name
+        InventoryNode(name, nature=f"{type(permission.entity).__name__} permission", ref=ref, propagate=permission.propagate, parent=principal_node)
+
+    return node
+
+
+def build_license_inventory(vcenter: VCenterClient, parent = None) -> InventoryNode:
+    node = None
+
+    try:
+        for license in vcenter.service_content.licenseManager.licenses:
+            if not node:
+                node = InventoryNode("(licenses)", parent=parent)
+            InventoryNode(license.name, nature=type(license), key=license.licenseKey, parent=node)
+    except vim.fault.NoPermission:
+        _logger.warning("Skip license inventory (no permission)")
+
+    return node
+
+
+class InventoryNode:
+    indent_size = 2
+
+    def __init__(self, name: str, *, nature: type|str = None, parent: InventoryNode = None, **attrs):
+        self.name = name        
+        self.nature = nature.__name__ if isinstance(nature, type) else (str(nature) if nature else None)
+        self.parent = parent
+        self.attrs = attrs
+        self.children: list[InventoryNode] = []
+        if parent:
+            parent.children.append(self)
+
+    def __str__(self):
+        result = self.name
+        need_comma = True
+        if self.nature:
+            result += f' [{self.nature}]'
+            need_comma = False
+
+        for name, value in self.attrs.items():
+            result += (', ' if need_comma else ' ') + f'{name}={value}'
+            need_comma = True
+
+        return result
+
+    def to_yaml(self, file, depth = 0):
+        if not isinstance(file, IOBase):
+            if dir := os.path.dirname(file):
+                os.makedirs(dir, exist_ok=True)
+                
+        with nullcontext(file) if isinstance(file, IOBase) else open(file, 'w', encoding='utf-8') as fp:
+            print(f"{' ' * self.indent_size * depth + '- ' if depth > 0 else ''}{self}:", file=fp)
+            for child in self.children:
+                child.to_yaml(fp, depth+1)
```

## vmware_reporter/net.py

```diff
@@ -1,188 +1,188 @@
-"""
-Analyze networking.
-"""
-from __future__ import annotations
-
-import re
-from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
-
-from pyVmomi import vim
-from zut import add_func_command, out_table, get_help_text, get_description_text
-
-from . import VCenterClient, get_obj_ref
-
-
-def add_net_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
-    parser = commands_subparsers.add_parser(name, help=get_help_text(__doc__), description=get_description_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False)
-
-    group = parser.add_argument_group(title='Command options')
-    group.add_argument('-h', '--help', action='help', help=f"Show this command help message and exit.")
-
-    subparsers = parser.add_subparsers(title='Sub commands')
-    add_func_command(subparsers, list_nets, name='list')
-
-
-_DEFAULT_OUT = '{title}.csv'
-
-def list_nets(vcenter: VCenterClient, *, out: str = _DEFAULT_OUT):
-    """
-    List switchs (`vim.dvs.DistributedVirtualSwitch` objects) and networks (`vim.Network` and `vim.dvs.DistributedVirtualPortgroup` objects).
-    """
-    switchs_headers = [
-        'name',
-        'ref',
-        'overall_status',
-        'config_status',
-        'uuid',
-        'uplinks',
-        'default_vlan',
-    ]
-
-    with out_table(out, title='switchs', dir=vcenter.get_out_dir(), env=vcenter.env, headers=switchs_headers) as t:
-        for obj in vcenter.iter_objs(vim.DistributedVirtualSwitch):
-            uplinks = []
-            for portgroup in obj.config.uplinkPortgroup:
-                uplink = portgroup.name
-                uplinks.append(uplink)
-
-            t.append([
-                obj.name,
-                get_obj_ref(obj),
-                obj.overallStatus,
-                obj.configStatus,
-                obj.uuid,
-                uplinks,
-                _vlan_repr(obj.config.defaultPortConfig.vlan),
-            ])
-
-    networks_headers = [
-        'name',
-        'ref',
-        'overall_status',
-        'config_status',
-        'type',
-        'switch',
-        'ports',
-        'default_vlan',
-    ]
-
-    with out_table(out, title='networks', dir=vcenter.get_out_dir(), env=vcenter.env, headers=networks_headers) as t:
-        for obj in sorted(vcenter.iter_objs(vim.Network), key=_network_sortkey):
-            if isinstance(obj, vim.dvs.DistributedVirtualPortgroup):
-                typename = 'DVP'
-                switch = obj.config.distributedVirtualSwitch.name
-                vlan = obj.config.defaultPortConfig.vlan
-                ports = f'{obj.config.numPorts}: ' + ','.join(_get_portkey_ranges(obj.portKeys))
-            elif isinstance(obj, vim.Network):
-                typename = 'Network'
-                switch = None
-                vlan = None
-                ports = None
-            elif isinstance(obj, vim.Network):
-                typename = type(obj).__name__
-                switch = None
-                vlan = None
-                ports = None
-
-            t.append([
-                obj.name,
-                get_obj_ref(obj),
-                obj.overallStatus,
-                obj.configStatus,
-                typename,
-                switch,
-                ports,
-                _vlan_repr(vlan),
-            ])
-
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
-
-list_nets.add_arguments = _add_arguments
-
-
-def _network_sortkey(obj: vim.Network):
-    if isinstance(obj, vim.dvs.DistributedVirtualPortgroup):
-        minkey = None
-        for key in obj.portKeys:
-            if key is not None and re.match(r'^\d+$', key):
-                key = int(key)
-                if minkey is None or key < minkey:
-                    minkey = key
-
-        if minkey is None:
-            minkey = 0
-        return (1, obj.config.distributedVirtualSwitch.name, minkey ,obj.name)
-
-    else:
-        return (2, obj.name)
-
-
-def _vlan_repr(vlan: vim.dvs.VmwareDistributedVirtualSwitch.VlanIdSpec|vim.dvs.VmwareDistributedVirtualSwitch.TrunkVlanSpec) -> int|str:
-    if vlan is None:
-        return None
-    
-    if isinstance(vlan, vim.dvs.VmwareDistributedVirtualSwitch.VlanIdSpec):
-        result = 'id: '
-    elif isinstance(vlan, vim.dvs.VmwareDistributedVirtualSwitch.TrunkVlanSpec):
-        result = 'trunk: '
-    else:
-        result = f'{type(vlan).__name__}: '
-    
-    if isinstance(vlan.vlanId, list):
-        parts = []
-        for spec in vlan.vlanId:
-            if isinstance(spec, vim.NumericRange):
-                parts.append(f'{spec.start}-{spec.end}')
-            else:
-                parts.append(f'{spec}')
-        result += ','.join(parts)
-    elif isinstance(vlan.vlanId, vim.NumericRange):
-        result += f'{vlan.vlanId.start}-{vlan.vlanId.end}'
-    else:
-        result += f'{vlan.vlanId}'
-
-    if vlan.inherited:
-        result += ', inherited'
-
-    return result
-
-
-def _get_portkey_ranges(portkeys: list[int|str]) -> list[str]:
-    intkeys = []
-    strkeys = []
-
-    for key in portkeys:
-        if re.match(r'^\d+$', key):
-            intkeys.append(int(key))
-        else:
-            strkeys.append(str(key))
-    
-    intkeys.sort()
-
-    results = []
-
-    last_start = None
-    last_end = None
-
-    def append_last():
-        if last_end is not None:
-            if last_end == last_start:
-                results.append(str(last_start))
-            else:
-                results.append(f'{last_start}-{last_end}')
-
-    for key in intkeys:
-        if last_end is not None and key == last_end + 1: 
-            last_end = key
-        else:
-            append_last()
-            last_start = key
-            last_end = key
-
-    append_last()
-
-    for key in strkeys:
-        results.append(key)
-    return results
+"""
+Analyze networking.
+"""
+from __future__ import annotations
+
+import re
+from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
+
+from pyVmomi import vim
+from zut import add_func_command, out_table, get_help_text, get_description_text
+
+from . import VCenterClient, get_obj_ref, get_obj_typename
+
+
+def add_net_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
+    parser = commands_subparsers.add_parser(name, help=get_help_text(__doc__), description=get_description_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False)
+
+    group = parser.add_argument_group(title='Command options')
+    group.add_argument('-h', '--help', action='help', help=f"Show this command help message and exit.")
+
+    subparsers = parser.add_subparsers(title='Sub commands')
+    add_func_command(subparsers, list_nets, name='list')
+
+
+_DEFAULT_OUT = '{title}.csv'
+
+def list_nets(vcenter: VCenterClient, *, out: str = _DEFAULT_OUT):
+    """
+    List switchs (`vim.dvs.DistributedVirtualSwitch` objects) and networks (`vim.Network` and `vim.dvs.DistributedVirtualPortgroup` objects).
+    """
+    switchs_headers = [
+        'name',
+        'ref',
+        'overall_status',
+        'config_status',
+        'uuid',
+        'uplinks',
+        'default_vlan',
+    ]
+
+    with out_table(out, title='switchs', dir=vcenter.out_dir, env=vcenter.env, headers=switchs_headers) as t:
+        for obj in vcenter.iter_objs(vim.DistributedVirtualSwitch):
+            uplinks = []
+            for portgroup in obj.config.uplinkPortgroup:
+                uplink = portgroup.name
+                uplinks.append(uplink)
+
+            t.append([
+                obj.name,
+                get_obj_ref(obj),
+                obj.overallStatus,
+                obj.configStatus,
+                obj.uuid,
+                uplinks,
+                _vlan_repr(obj.config.defaultPortConfig.vlan),
+            ])
+
+    networks_headers = [
+        'name',
+        'ref',
+        'overall_status',
+        'config_status',
+        'type',
+        'switch',
+        'ports',
+        'default_vlan',
+    ]
+
+    with out_table(out, title='networks', dir=vcenter.out_dir, env=vcenter.env, headers=networks_headers) as t:
+        for obj in sorted(vcenter.iter_objs(vim.Network), key=_network_sortkey):
+            if isinstance(obj, vim.dvs.DistributedVirtualPortgroup):
+                typename = 'DVP'
+                switch = obj.config.distributedVirtualSwitch.name
+                vlan = obj.config.defaultPortConfig.vlan
+                ports = f'{obj.config.numPorts}: ' + ','.join(_get_portkey_ranges(obj.portKeys))
+            elif isinstance(obj, vim.Network):
+                typename = 'Network'
+                switch = None
+                vlan = None
+                ports = None
+            elif isinstance(obj, vim.Network):
+                typename = get_obj_typename(obj)
+                switch = None
+                vlan = None
+                ports = None
+
+            t.append([
+                obj.name,
+                get_obj_ref(obj),
+                obj.overallStatus,
+                obj.configStatus,
+                typename,
+                switch,
+                ports,
+                _vlan_repr(vlan),
+            ])
+
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
+
+list_nets.add_arguments = _add_arguments
+
+
+def _network_sortkey(obj: vim.Network):
+    if isinstance(obj, vim.dvs.DistributedVirtualPortgroup):
+        minkey = None
+        for key in obj.portKeys:
+            if key is not None and re.match(r'^\d+$', key):
+                key = int(key)
+                if minkey is None or key < minkey:
+                    minkey = key
+
+        if minkey is None:
+            minkey = 0
+        return (1, obj.config.distributedVirtualSwitch.name, minkey ,obj.name)
+
+    else:
+        return (2, obj.name)
+
+
+def _vlan_repr(vlan: vim.dvs.VmwareDistributedVirtualSwitch.VlanIdSpec|vim.dvs.VmwareDistributedVirtualSwitch.TrunkVlanSpec) -> int|str:
+    if vlan is None:
+        return None
+    
+    if isinstance(vlan, vim.dvs.VmwareDistributedVirtualSwitch.VlanIdSpec):
+        result = 'id: '
+    elif isinstance(vlan, vim.dvs.VmwareDistributedVirtualSwitch.TrunkVlanSpec):
+        result = 'trunk: '
+    else:
+        result = f'{type(vlan).__name__}: '
+    
+    if isinstance(vlan.vlanId, list):
+        parts = []
+        for spec in vlan.vlanId:
+            if isinstance(spec, vim.NumericRange):
+                parts.append(f'{spec.start}-{spec.end}')
+            else:
+                parts.append(f'{spec}')
+        result += ','.join(parts)
+    elif isinstance(vlan.vlanId, vim.NumericRange):
+        result += f'{vlan.vlanId.start}-{vlan.vlanId.end}'
+    else:
+        result += f'{vlan.vlanId}'
+
+    if vlan.inherited:
+        result += ', inherited'
+
+    return result
+
+
+def _get_portkey_ranges(portkeys: list[int|str]) -> list[str]:
+    intkeys = []
+    strkeys = []
+
+    for key in portkeys:
+        if re.match(r'^\d+$', key):
+            intkeys.append(int(key))
+        else:
+            strkeys.append(str(key))
+    
+    intkeys.sort()
+
+    results = []
+
+    last_start = None
+    last_end = None
+
+    def append_last():
+        if last_end is not None:
+            if last_end == last_start:
+                results.append(str(last_start))
+            else:
+                results.append(f'{last_start}-{last_end}')
+
+    for key in intkeys:
+        if last_end is not None and key == last_end + 1: 
+            last_end = key
+        else:
+            append_last()
+            last_start = key
+            last_end = key
+
+    append_last()
+
+    for key in strkeys:
+        results.append(key)
+    return results
```

## vmware_reporter/settings.py

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-import os
-import vmware_reporter
-from zut import get_config
-
-CONFIG = get_config(os.environ.get('VMWARE_REPORTER_CONFIG') or vmware_reporter)
-CONFIG_SECTION = os.environ.get('VMWARE_REPORTER_CONFIG_SECTION') or 'vmware-reporter'
+import os
+import vmware_reporter
+from zut import get_config
+
+CONFIG = get_config(os.environ.get('VMWARE_REPORTER_CONFIG') or vmware_reporter)
+CONFIG_SECTION = os.environ.get('VMWARE_REPORTER_CONFIG_SECTION') or 'vmware-reporter'
```

## vmware_reporter/vm.py

```diff
@@ -1,1364 +1,1484 @@
-"""
-Manage virtual machines.
-"""
-from __future__ import annotations
-
-import json
-import logging
-import os
-import re
-from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
-from datetime import datetime
-from io import IOBase
-from ipaddress import IPv4Address, IPv6Address, ip_address
-from pathlib import Path
-from typing import Any, Callable, Literal
-
-from pyVmomi import vim
-from zut import (Header, add_func_command, get_description_text, get_help_text,
-                 gigi_bytes, out_table, slugify)
-from zut.excel import ExcelRow, ExcelWorkbook, split_excel_path
-
-from . import (VCenterClient, dictify_obj, dictify_value, get_obj_path,
-               get_obj_ref)
-
-logger = logging.getLogger(__name__)
-
-_DEFAULT_OUT = '{title}.csv'
-
-def add_vm_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
-    parser = commands_subparsers.add_parser(name, help=get_help_text(__doc__), description=get_description_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False)
-
-    group = parser.add_argument_group(title='Command options')
-    group.add_argument('-h', '--help', action='help', help=f"Show this command help message and exit.")
-
-    subparsers = parser.add_subparsers(title='Sub commands')
-    add_func_command(subparsers, list_vms, name='list')
-    add_func_command(subparsers, list_vm_disks, name='disks')
-    add_func_command(subparsers, list_vm_nics, name='nics')
-    
-    # Operations
-    add_func_command(subparsers, start_vms, name='start')
-    add_func_command(subparsers, stop_vms, name='stop')
-    add_func_command(subparsers, suspend_vms, name='suspend')    
-    add_func_command(subparsers, reconfigure_vms, name='reconfigure')
-
-
-#region List
-
-def list_vms(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: os.PathLike|IOBase = _DEFAULT_OUT):
-    headers = [
-        'name',
-        'ref',
-        'overall_status',
-        'config_status',
-        'template',
-        # Config
-        'vcpu',
-        'cores_per_socket',
-        Header('memory', fmt='gib'),
-        Header('disk_capacity', fmt='gib'),
-        Header('disk_freespace', fmt='gib'),
-        'disk_count',
-        'nic_count',
-        # Dossier / rangement
-        'folder',
-        'Appartenance',
-        'other_custom_values',
-        'annotation',
-        'create_date',
-        'change_date',
-        # Config details
-        'hostname',
-        'network',
-        'disk',
-        # ResourcePool / runtime
-        'resource_pool',
-        'host',
-        'power_state',
-        'paused',
-        'connection_state',
-        'boot_time',
-        'hw_version',
-        # Guest info
-        'os_family',
-        'os_version',
-        'os_distro_version',
-        'os_kernel_version',
-        'tools_status',
-        'tools_running_status',
-        'tools_version_number',
-        'tools_version',
-        'guestinfo_publish_time',
-    ]
-
-    with out_table(out, title='vms', dir=vcenter.get_out_dir(), env=vcenter.env, headers=headers, after1970=True) as t:
-        for obj in vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key):  
-            try:
-                logger.info(f"Analyze vm {obj.name}")
-
-                disks = extract_disks(obj)
-                nics = extract_nics(obj, vcenter=vcenter)
-
-                custom_values = get_custom_values(obj)
-                Appartenance = custom_values.pop('Appartenance', None)
-                other_custom_values = ' | '.join(f"{key}: {value}" for key, value in custom_values.items())
-
-                extra_config = dictify_value(obj.config.extraConfig)
-
-                t.append([
-                    obj.name,
-                    get_obj_ref(obj),
-                    obj.overallStatus,
-                    obj.configStatus,
-                    obj.config.template,
-                    # Config
-                    obj.config.hardware.numCPU,
-                    obj.config.hardware.numCoresPerSocket,
-                    obj.config.hardware.memoryMB * 1024 * 1024,
-                    disks.capacity,
-                    disks.freespace,
-                    obj.summary.config.numVirtualDisks,
-                    obj.summary.config.numEthernetCards,
-                    # Dossier / rangement
-                    get_obj_path(obj.parent),
-                    Appartenance,
-                    other_custom_values,
-                    obj.config.annotation,
-                    obj.config.createDate,
-                    datetime.fromisoformat(obj.config.changeVersion),
-                    # Config details
-                    obj.guest.hostName,
-                    nics.to_summary(ip_version=4),
-                    disks.to_summary(),
-                    # ResourcePool / runtime
-                    get_obj_path(obj.resourcePool),
-                    obj.runtime.host.name,
-                    obj.runtime.powerState,
-                    obj.runtime.paused,
-                    obj.runtime.connectionState,
-                    obj.runtime.bootTime,
-                    obj.config.version,
-                    # Guest info
-                    get_os_family(extra_config, obj.config.guestFullName),
-                    get_os_version(extra_config),
-                    get_os_distro_version(extra_config),
-                    get_os_kernel_version(extra_config),
-                    obj.guest.toolsStatus,  # nominal: toolsOk
-                    obj.guest.toolsRunningStatus,  # nominal: guestToolsRunning
-                    get_tools_version_number(obj.guest.toolsVersion),  # version number
-                    get_tools_version(extra_config, obj.guest.toolsVersion),      
-                    get_guestinfo_publish_time(extra_config),
-                ])
-            
-            except Exception as err:
-                logger.exception(f"Error while analyzing {str(obj)}")
-
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('search', nargs='*', help="Search term(s).")
-    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
-    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
-    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output table (default: %(default)s).")
-
-list_vms.add_arguments = _add_arguments
-
-#endregion
-
-
-#region Start, stop, suspend
-
-def start_vms(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', **options):
-    _invoke_and_track('PowerOn', vcenter, search, normalize=normalize, key=key)
-
-def stop_vms(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', force: bool = False):
-    if force:
-        _invoke_and_track('PowerOff', vcenter, search, normalize=normalize, key=key)
-    else:
-        _invoke_and_track('ShutdownGuest', vcenter, search, normalize=normalize, key=key)
-
-def suspend_vms(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', force: bool = False):
-    if force:
-        _invoke_and_track('Suspend', vcenter, search, normalize=normalize, key=key)
-    else:
-        _invoke_and_track('StandbyGuest', vcenter, search, normalize=normalize, key=key)
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('search', nargs='*', help="Search term(s).")
-    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
-    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
-    parser.add_argument('-f', '--force', action='store_true', help="Force operation.")
-
-start_vms.add_arguments = _add_arguments
-stop_vms.add_arguments = _add_arguments
-suspend_vms.add_arguments = _add_arguments
-
-
-def _invoke_and_track(op: str, vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name'):
-    # Idea: https://github.com/reubenur-rahman/vmware-pyvmomi-examples/blob/master/vm_power_ops.py
-    tasks = {}
-    for vm in vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key):
-        log_prefix = f"{vm.name} ({get_obj_ref(vm)})"
-        logger.info(f"{op} {log_prefix}...")
-        func = getattr(vm, op)
-        try:
-            task = func()
-            if task is not None:
-                tasks[task] = log_prefix
-        except Exception as err:
-            logger.error(f"{log_prefix}: {str(err)}")
-
-    if tasks:
-        vcenter.wait_for_task(tasks)
-
-
-#endregion
-
-
-#region Reconfigure
-
-DEFAULT_RECONFIGURE_FILE = 'vms_reconfigure.xlsx'
-DEFAULT_RECONFIGURE_TABLE = 'vms'
-
-def reconfigure_vms(vcenter: VCenterClient, path: str|Path = DEFAULT_RECONFIGURE_FILE, top: int = None, ignore_invalid_current: bool = False):
-    """
-    Reconfigure VMs (vcpu, memory, annotation, custom fields) as a mass operation, using an Excel file.
-    """
-    class Helper:
-        def __init__(self, row: ExcelRow, found: bool = False):
-            self.row = row
-            self.found = found
-
-        def report_ok(self, details: str):
-            logger.info(f"OK: {details}")
-            self.row['status'] = 'OK'
-            self.row['details'] = details
-
-        def report_error(self, details: str):
-            logger.error(details)
-            self.row['status'] = 'ERROR'
-            self.row['details'] = details
-            
-    class FieldDef:
-        def __init__(self, name: str, type: type, getter: Callable[[vim.VirtualMachine],Any]|Literal['__customvalue__'], target_key:str|int, target_formatter: Callable[[vim.VirtualMachine],Any] = None):
-            """
-            - `key`: if str, this is the reconfigure ConfigSpec argument to use. If int, this is the customfield key to use.
-            """
-            self.name = name
-            self.type = type
-            self.getter = getter
-            self.target_key = target_key
-            self.target_formatter = target_formatter
-
-        def get_from_vm(self, vm: vim.VirtualMachine):
-            if self.getter == '__customvalue__':
-                for kv in vm.customValue:
-                    if kv.key == self.target_key:
-                        return kv.value
-            else:
-                return self.getter(vm)
-
-        def get_from_row(self, row: ExcelRow, suffix: str = None):
-            value = row.get(f"{self.name}_{suffix}" if suffix else self.name)
-            if value is None or value == '':
-                return None
-            if self.type == str and value == '-':
-                return ''
-            return self.type(value)
-        
-        def format_for_target(self, value):
-            if not self.target_formatter:
-                return value
-            return self.target_formatter(value)
-
-    fielddefs: list[FieldDef] = [
-        FieldDef('vcpu', int, lambda vm: vm.config.hardware.numCPU, 'numCPUs'),
-        FieldDef('memory', float, lambda vm: vm.config.hardware.memoryMB / 1024.0, 'memoryMB', lambda val: int(val * 1024.0)),
-        FieldDef('annotation', str, lambda vm: vm.config.annotation, 'annotation'),
-    ]
-
-    for customfield in vcenter.service_content.customFieldsManager.field:
-        if customfield.managedObjectType == vim.VirtualMachine:
-            fielddefs.append(FieldDef(customfield.name, str, '__customvalue__', customfield.key))
-    
-    path, tablename = split_excel_path(path, default_table_name=DEFAULT_RECONFIGURE_TABLE, dir=vcenter.get_out_dir(), env=vcenter.env)
-
-    workbook = ExcelWorkbook(path)
-    table = workbook.get_or_create_table(tablename)
-    
-    helpers: dict[str,Helper] = {}
-    search_by_ref = 'ref' in table.column_names
-    for row in table:
-        if search_by_ref:
-            if row['ref']:
-                helpers[row['ref']] = Helper(row)
-        else:
-            if row['name']:
-                helpers[slugify(row['name'])] = Helper(row)
-        row['status'] = None
-        row['details'] = None
-    
-    n = 0
-    for vm in vcenter.iter_objs(vim.VirtualMachine):
-        if top is not None and n == top:
-            logger.warning(f"Stop after {n} VMs")
-            break
-
-        key = get_obj_ref(vm) if search_by_ref else slugify(vm.name)
-        helper = helpers.get(key)
-        if not helper:
-            continue
-        
-        if helper.found:
-            logger.error(f"VM {vm.name}: ignore (several VMs with key \"{key}\")")
-            continue
-        helper.found = True
-
-        n += 1        
-        logger.info(f"Handle {vm.name} ({get_obj_ref(vm)})")
-        row = helper.row
-
-        try:
-            if search_by_ref and slugify(vm.name) != slugify(row['name']):
-                helper.report_error(f"Invalid VM name: expected {vm.name}")
-                continue
-
-            if vm.config.template:
-                helper.report_error(f"This is a template")
-                continue
-
-            if vm.runtime.powerState != 'poweredOff':
-                helper.report_error(f"Not powered off")
-                continue
-
-            config_previous: dict[str|int,Any] = {}
-            config_targets: dict[str|int,Any] = {}
-            invalid_current = ''
-
-            # Prepare reconfiguration
-            change_version = vm.config.changeVersion  # used to guard against updates that have happened between when configInfo is read and when it is applied
-
-            for fielddef in fielddefs:
-                target = fielddef.get_from_row(row, 'target')
-                if target is None:
-                    continue
-
-                current = fielddef.get_from_vm(vm)
-                current_expected = fielddef.get_from_row(row)
-                if current_expected is not None:
-                    if current_expected != current and not ignore_invalid_current:
-                        invalid_current += (', ' if invalid_current else '') + f"current {fielddef.name}: {'(empty)' if current == '' else current}"   
-                        continue
-
-                if target != current:
-                    config_previous[fielddef.target_key] = fielddef.format_for_target(current)
-                    config_targets[fielddef.target_key] = fielddef.format_for_target(target)
-
-            if invalid_current:
-                helper.report_error(f"Invalid {invalid_current}")
-                continue
-
-            if not config_targets:
-                helper.report_ok("Nothing to do")
-                continue
-
-            config_targets_reconfigure = {}
-            config_targets_customfields = {}
-            for key, value in config_targets.items():
-                if isinstance(key, str):
-                    config_targets_reconfigure[key] = value
-                else:
-                    config_targets_customfields[key] = value
-
-            # Perform the reconfiguration
-            if config_targets_reconfigure:
-                logger.debug("Reconfigure VM: %s", config_targets_reconfigure)
-                configspec = vim.vm.ConfigSpec(**config_targets_reconfigure, changeVersion=change_version)
-                task = vm.ReconfigVM_Task(configspec)
-                vcenter.wait_for_task(task)
-
-            for key, value in config_targets_customfields.items():
-                logger.debug("Set custom field %s: %s", key, value)
-                vcenter.service_content.customFieldsManager.SetField(vm, key, value)
-
-            # Verification
-            status_ok = True
-            details = ''
-
-            for fielddef in fielddefs:
-                if not fielddef.target_key in config_targets:
-                    continue # field not modified
-
-                previous_value = config_previous[fielddef.target_key]
-                target_value = config_targets[fielddef.target_key]
-                new_value = fielddef.format_for_target(fielddef.get_from_vm(vm))
-                details += (', ' if details else '') + f"{fielddef.target_key}: {previous_value} -> {'(empty)' if new_value == '' else new_value}"
-
-                if new_value != target_value:
-                    status_ok = False
-                    details += ' [ERROR]'
-
-            if status_ok:
-                helper.report_ok(details)
-            else:
-                helper.report_error(details)
-        
-        except Exception as err:
-            logger.exception(str(err))
-            row['status'] = type(err).__name__
-            row['details'] = str(err)
-
-    # Report not found
-    for key, helper in helpers.items():
-        if not helper.found:
-            helper.report_error(f"VM {key} not found")
-
-    workbook.close()
-
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('path', nargs='?', default=DEFAULT_RECONFIGURE_FILE, help="Path to Excel file describing VMs to reconfigure.")
-    parser.add_argument('--top', type=int)
-    parser.add_argument('--ignore-invalid-current', action='store_true')
-
-reconfigure_vms.add_arguments = _add_arguments
-
-
-#endregion
-
-
-#region Disks
-
-def list_vm_disks(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: str = _DEFAULT_OUT, top: int = None):
-    """
-    Analyze VM disks.
-    """
-    disks_per_vm_headers = [
-        'vm',
-        'power_state',
-        'os_family',
-        'os_version',
-        'device_disks',
-        'guest_disks',
-        'with_mappings',
-        'without_mappings',
-        'mapped_guest',
-        'unmapped_guest',
-        Header('capacity', fmt='gib'),
-        Header('freespace', fmt='gib'),
-        Header('mapped_disks_capacity', fmt='gib'),
-        Header('mapped_guests_capacity', fmt='gib'),
-        Header('mapped_guests_freespace', fmt='gib'),
-        Header('unmapped_disks_capacity', fmt='gib'),
-        Header('unmapped_guests_capacity', fmt='gib'),
-        Header('unmapped_guests_freespace', fmt='gib'),
-        'issues',
-    ]
-
-    disks_headers = [
-        'vm',
-        'power_state',
-        'os_family',
-        'os_version',
-        'key',
-        'backing',
-        'datastore',
-        'filename',
-        'diskmode',
-        'sharing',
-        'remaining_backing_info',
-        Header('capacity', fmt='gib'),
-        Header('freespace', fmt='gib'),
-        'mapping',
-        'guests',
-        Header('guests_capacity', fmt='gib'),
-        Header('guests_freespace', fmt='gib'),
-        'capacity_loss_pct',
-    ]
-    
-    with (out_table(out, title='vm_disks', headers=disks_headers, dir=vcenter.get_out_dir(), env=vcenter.env) as t_disks,
-          out_table(out, title='vm_disks_per_vm', headers=disks_per_vm_headers, dir=vcenter.get_out_dir(), env=vcenter.env) as t_disks_per_vm):
-        
-        for i, vm in enumerate(vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key)):
-            if top is not None and i == top:
-                break
-            
-            try:
-                logger.info(f"Analyze vm {vm.name} disks")
-
-                info = extract_disks(vm)
-
-                extra_config = dictify_value(vm.config.extraConfig)
-                os_family = get_os_family(extra_config, vm.config.guestFullName)
-                os_version = get_os_version(extra_config)
-
-                mapped_guests: list[vim.vm.GuestInfo.DiskInfo] = []
-                for disk in info.disks:
-                    for guest in disk.guests:
-                        mapped_guests.append(guest)
-
-                t_disks_per_vm.append([
-                    vm.name, # vm
-                    vm.runtime.powerState, # power_state
-                    os_family,
-                    os_version,
-                    len(info.disks), # 'device_disks',
-                    len(mapped_guests) + len(info.unmapped_guests), # 'guest_disks',
-                    len(mapped_guests), # 'with_mappings',
-                    len(info.unmapped_guests), # 'without_mappings',
-                    sorted(f'{guest.diskPath} ({guest.filesystemType})' if guest.filesystemType else guest.diskPath for guest in mapped_guests), # 'mapped_guest',
-                    sorted(f'{guest.diskPath} ({guest.filesystemType})' if guest.filesystemType else guest.diskPath for guest in info.unmapped_guests),# 'unmapped_guests',
-                    info.capacity,
-                    info.freespace,
-                    info.mapped_disks_capacity if mapped_guests else None,
-                    info.mapped_guests_capacity if mapped_guests else None,
-                    info.mapped_guests_freespace if mapped_guests else None,
-                    info.unmapped_disks_capacity if info.unmapped_disks_capacity > 0 else None,
-                    info.unmapped_guests_capacity if info.unmapped_guests else None,
-                    info.unmapped_guests_freespace if info.unmapped_guests else None,
-                    info.issues,
-                ])
-
-                for disk in info.disks:
-                    device_backing = dictify_obj(disk.device.backing)
-                    backing_typename = type(disk.device.backing).__name__
-                    if backing_typename.startswith('vim.vm.device.VirtualDisk.'):
-                        backing_typename = backing_typename[len('vim.vm.device.VirtualDisk.'):]
-                    datastore = device_backing.pop('datastore', None)
-                    fileName = device_backing.pop('fileName', None)
-                    diskMode = device_backing.pop('diskMode', None)
-                    sharing = device_backing.pop('sharing', None)
-
-                    capacity_loss = disk.capacity - disk.guests_capacity if disk.guests else None
-                    capacity_loss_pct = 100 * capacity_loss / disk.capacity if disk.guests else None
-                    
-                    t_disks.append([
-                        vm.name, # vm
-                        vm.runtime.powerState, # power_state
-                        os_family,
-                        os_version,
-                        disk.device.key, # key
-                        backing_typename, # backing
-                        datastore['name'] if datastore else None, # datastore
-                        fileName,
-                        diskMode,
-                        sharing,
-                        device_backing, # remaining_backing_info
-                        disk.capacity,
-                        disk.freespace,
-                        disk.guests_mapping,
-                        sorted(f'{guest.diskPath} ({guest.filesystemType})' if guest.filesystemType else guest.diskPath for guest in disk.guests), # guests
-                        disk.guests_capacity if disk.guests else None,
-                        disk.guests_freespace if disk.guests else None,
-                        capacity_loss_pct,
-                    ])
-
-                for guest in [*info.unmapped_guests, *info.ignored_guests]:
-                    t_disks.append([
-                        vm.name, # vm
-                        vm.runtime.powerState, # power_state
-                        os_family,
-                        os_version,
-                        None, # key
-                        guest.mappings, # backing
-                        None, # datastore
-                        None, # filename
-                        None, # diskMode
-                        None, # sharing
-                        None, # remaining_backing_info
-                        None, # capacity
-                        None, # freespace
-                        'ignored' if guest in info.ignored_guests else 'unmapped', # mapping
-                        f'{guest.diskPath} ({guest.filesystemType})' if guest.filesystemType else guest.diskPath, # guests
-                        guest.capacity, # guests_capacity
-                        guest.freeSpace, # guests_freespace
-                        None, # capacity_loss_pct
-                    ])
-
-            except Exception as err:
-                logger.exception(f"Error while analyzing {str(vm)} disks: {err}")
-
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('search', nargs='*', help="Search term(s).")
-    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
-    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
-    parser.add_argument('--top', type=int)
-    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
-
-list_vm_disks.add_arguments = _add_arguments
-
-
-def extract_disks(vm: vim.VirtualMachine):
-    info = VmDisks(vm)
-
-    # Retrieve disk devices
-    disks_per_key: dict[int,VmDisk] = {}
-    keys_to_ignore = set()
-    for obj in vm.config.hardware.device:
-        if not isinstance(obj, vim.vm.device.VirtualDisk):
-            continue
-
-        disk = VmDisk(obj)
-        info.disks.append(disk)
-        info.capacity += disk.capacity
-
-        if obj.key is None:
-            info._append_issue(f"Device disk has no key: {obj}")
-        elif not isinstance(obj.key, int):
-            info._append_issue(f"Device disk has a non-int key: {obj}")
-        elif obj.key in disks_per_key:
-            info._append_issue(f"Several disk have key {obj.key}")
-            keys_to_ignore.add(obj.key)
-        else:
-            disks_per_key[obj.key] = disk
-
-    for key in keys_to_ignore:
-        del disks_per_key[key]
-
-    # Retrieve guest disks
-    # Associate them to device disks if a consistent mapping is provided
-    for obj in vm.guest.disk:
-        mappings = obj.mappings
-        if mappings:
-            mapping_keys = set()
-            for mapping in mappings:
-                mapping_keys.add(mapping.key)
-
-            if len(mapping_keys) > 1:
-                info._append_issue(f"Guest disk {obj.diskPath} mapped to several device disk keys: {mapping_keys}")
-                info.unmapped_guests.append(obj)
-
-            else:
-                disk = disks_per_key.get(mapping.key)
-                if not disk:
-                    info._append_issue(f"Guest disk {obj.diskPath} mapped to unknown device disk key: {mapping.key}")
-                    info.unmapped_guests.append(obj)
-
-                else:
-                    disk.guests.append(obj)
-                    disk.guests_mapping = 'key'
-        else:
-            info.unmapped_guests.append(obj)
-
-    # Verify consistency of mapped guests capacity
-    for disk in info.disks:
-        if disk.guests:
-            for guest in disk.guests:
-                disk.guests_capacity += guest.capacity
-                disk.guests_freespace += guest.freeSpace
-            if disk.guests_capacity > disk.capacity:
-                info._append_issue(f"Inconsistent capacity ({disk.guests_capacity:,}) for guests {', '.join(guest.diskPath for guest in disk.guests)} (device {disk.device.key} capacity: {disk.capacity:,})")
-
-    # Identify guests to ignore
-    info._identify_ignored_guests()
-    
-    # Try to map remaining guests by capacity
-    unmapped_guests = sorted([guest for guest in info.unmapped_guests], key=lambda obj: obj.capacity, reverse=True)
-    unmapped_disks = sorted([disk for disk in info.disks if not disk.guests], key=lambda disk: disk.capacity, reverse=True)
-
-    confirm_mapping = True
-    if len(unmapped_disks) == len(unmapped_guests):
-        for i in range(0, len(unmapped_disks)):
-            disk = unmapped_disks[i]
-            guest = unmapped_guests[i]
-            if guest.capacity > disk.capacity:
-                confirm_mapping = False
-                break
-
-            if i < len(unmapped_disks) - 1:
-                next_disk = unmapped_disks[i+1]
-                if guest.capacity <= next_disk.capacity: # another disk could match
-                    confirm_mapping = False
-                    break
-
-        if confirm_mapping:
-            for i in range(0, len(unmapped_disks)):
-                disk = unmapped_disks[i]
-                guest = unmapped_guests[i]
-                info.unmapped_guests.remove(guest)
-                disk.guests.append(guest)
-                disk.guests_capacity += guest.capacity
-                disk.guests_freespace += guest.freeSpace
-                disk.guests_mapping = 'capacity'
-
-    # Finalize capacity and freespace sums
-    for disk in info.disks:
-        if disk.guests:
-            disk.freespace = disk.guests_freespace + (disk.capacity - disk.guests_capacity)
-            info.mapped_guests_capacity += disk.guests_capacity
-            info.mapped_guests_freespace += disk.guests_freespace
-            info.mapped_disks_capacity += disk.capacity
-            info.mapped_disks_freespace += disk.freespace
-        else:
-            info.unmapped_disks_capacity += disk.capacity
-
-    for guest in info.unmapped_guests:
-        info.unmapped_guests_capacity += guest.capacity
-        info.unmapped_guests_freespace += guest.freeSpace
-
-    # (estimation of unmapped disk freespace)
-    if info.unmapped_disks_capacity > 0:
-        if info.unmapped_guests_capacity > info.unmapped_disks_capacity:
-            info.unmapped_disks_freespace = info.unmapped_guests_freespace * (info.unmapped_disks_capacity / info.unmapped_guests_capacity)
-        else:
-            info.unmapped_disks_freespace = info.unmapped_guests_freespace + (info.unmapped_disks_capacity - info.unmapped_guests_capacity)
-
-    info.freespace = info.mapped_disks_freespace + info.unmapped_disks_freespace
-
-    return info
-
-
-class VmDisks:
-    def __init__(self, vm: vim.VirtualMachine):
-        self.vm = vm
-        self.disks: list[VmDisk] = []
-        self.unmapped_guests: list[vim.vm.GuestInfo.DiskInfo] = []
-        self.ignored_guests: list[vim.vm.GuestInfo.DiskInfo] = []
-        self.issues: list[str] = []
-
-        self.capacity: int = 0
-        """ Sum of device capacities. """
-
-        self.freespace: int = 0
-        """ Sum of device freespaces. This is sum of mapped device freespaces + an estimation of unmapped freespace. """
-
-        self.mapped_disks_capacity: int = 0
-        self.mapped_disks_freespace: int = 0
-        self.mapped_guests_capacity: int = 0
-        self.mapped_guests_freespace: int = 0
-        
-        self.unmapped_disks_capacity: int = 0
-        self.unmapped_disks_freespace: int = 0
-        self.unmapped_guests_capacity: int = 0
-        self.unmapped_guests_freespace: int = 0
-
-    def _append_issue(self, message: str):
-        logger.warning(f"{self.vm.name}: {message}")
-        self.issues.append(message)
-
-    def _identify_ignored_guests(self):
-        for guest in list(self.unmapped_guests):
-            if self._must_ignore(guest):
-                self.unmapped_guests.remove(guest)
-                self.ignored_guests.append(guest)
-
-    def _must_ignore(self, guest: vim.vm.GuestInfo.DiskInfo):      
-        if guest.diskPath.startswith('C:\\Users\\'):
-            return True
-
-        elif '/' in guest.diskPath and guest.diskPath != '/': # Search Linux mount points with the exact same capacity as a parent. Example: /var/lib/rancher/volumes, /var/lib/kubelet.
-            parts = [part for part in guest.diskPath.split('/')]
-            for n in range(1, len(parts)):
-                search_parent = '/' + '/'.join(parts[1:n])
-                for parent in self.guests:
-                    if parent.diskPath == search_parent and parent.capacity == guest.capacity:
-                        return True
-                    
-        return False
-
-    @property
-    def guests(self):
-        for disk in self.disks:
-            for guest in disk.guests:
-                yield guest
-
-        for guest in self.unmapped_guests:
-            yield guest
-
-        for guest in self.ignored_guests:
-            yield guest
-
-    def to_dict(self):
-        data = []
-
-        for disk in self.disks:
-            data.append(disk.to_dict())
-
-        if self.unmapped_guests:
-            guests_data = []
-            data.append({'guests_mapping': 'unmapped', 'guests':  guests_data})
-            for guest in self.unmapped_guests:
-                guests_data.append(self._get_guest_dict(guest))
-
-        if self.ignored_guests:
-            guests_data = []
-            data.append({'guests_mapping': 'ignored', 'guests':  guests_data})
-            for guest in self.ignored_guests:
-                guests_data.append(self._get_guest_dict(guest))
-
-        return data
-    
-    def to_summary(self):
-        result = ''
-
-        for disk in self.disks:
-            result += (' | ' if result else '') + disk.to_summary()
-
-        if self.unmapped_guests:
-            result += (' | ' if result else '') + f"Unmapped guests ("
-            for i, guest in enumerate(self.unmapped_guests):
-                if i > 0:
-                    result += ', '
-                result += self._get_guest_summary(guest)
-            result += ')'
-
-        return result
-    
-    @classmethod
-    def _get_guest_dict(cls, guest: vim.vm.GuestInfo.DiskInfo):
-        data = {}
-        data['path'] = guest.diskPath
-        data['capacity'] = gigi_bytes(guest.capacity)
-        data['freespace'] = gigi_bytes(guest.freeSpace)
-        if value := guest.filesystemType:
-            data['filesystem'] = value
-        return data
-    
-    @classmethod
-    def _get_guest_summary(cls, guest: vim.vm.GuestInfo.DiskInfo):
-        path = guest.diskPath.rstrip(':\\')
-        return f'{path}: {gigi_bytes(guest.freeSpace):.1f}/{gigi_bytes(guest.capacity):.1f} GiB'
-
-
-class VmDisk:
-    def __init__(self, device: vim.vm.device.VirtualDisk):
-        self.device = device
-        self.guests: list[vim.vm.GuestInfo.DiskInfo] = []
-        self.guests_mapping: Literal['key','capacity'] = None
-
-        self.capacity: int = device.capacityInBytes
-        """ Device capacities. """
-
-        self.freespace: int = 0
-        """ Device freespace. This is `guests_freespace + (capacity - guests_capacity)`. """
-
-        self.guests_capacity: int = 0
-        """ Sum of guest capacities. """
-
-        self.guests_freespace: int = 0
-        """ Sum of guest freespaces. """
-
-    def to_dict(self):
-        data = {}
-        data['key'] = self.device.key
-        data['capacity'] = gigi_bytes(self.capacity)
-
-        if self.guests:
-            data['freespace'] = gigi_bytes(self.freespace)
-
-        backing_typename = type(self.device.backing).__name__
-        if backing_typename.startswith('vim.vm.device.VirtualDisk.'):
-            backing_typename = backing_typename[len('vim.vm.device.VirtualDisk.'):]
-        data['backing'] = backing_typename
-
-        datastore: vim.Datastore = getattr(self.device.backing, 'datastore', None)
-        if datastore:
-            data['datastore'] = {'name': datastore.name, 'ref': get_obj_ref(datastore)}
-
-        filename: str = getattr(self.device.backing, 'fileName', None)
-        if filename:
-            data['filename'] = filename
-
-        if self.guests_mapping:
-            data['guests_mapping'] = self.guests_mapping
-        if self.guests:
-            data['guests'] = []
-
-            for guest in self.guests:
-                data['guests'].append(VmDisks._get_guest_dict(guest))
-        
-        return data
-    
-    def to_summary(self):
-
-        filename: str = getattr(self.device.backing, 'fileName', None)
-        if filename:
-            identifier = filename
-        else:
-            identifier = f'#{self.device.key}'
-
-        result = f'{identifier}: {gigi_bytes(self.freespace):.1f}/{gigi_bytes(self.capacity):.1f} GiB'
-
-        if self.guests:
-            result += f' ('
-            for i, guest in enumerate(self.guests):
-                if i > 0:
-                    result += ', '
-                result += VmDisks._get_guest_summary(guest)
-            result += ')'
-        return result
-
-#endregion
-
-
-#region NICs
-
-def list_vm_nics(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: str = _DEFAULT_OUT, top: int = None):
-    """
-    Analyze VM network interfaces.
-    """
-    nics_per_vm_headers = [
-        'vm',
-        'power_state',
-        'os_family',
-        'os_version',
-        'device_networks',
-        'guest_networks',
-        'with_mappings',
-        'without_mappings',
-        'mapped_guest',
-        'unmapped_guest',
-        'issues',
-    ]
-
-    nics_headers = [
-        'vm',
-        'power_state',
-        'os_family',
-        'os_version',
-        'backing',
-        'network',
-        'address_type',
-        'key',
-        'mac',
-        'guests_ips',
-        'guests_network_name',
-    ]
-    
-    with (out_table(out, title='vm_nics', headers=nics_headers, dir=vcenter.get_out_dir(), env=vcenter.env) as t_nics,
-          out_table(out, title='vm_nics_per_vm', headers=nics_per_vm_headers, dir=vcenter.get_out_dir(), env=vcenter.env) as t_nics_per_vm):
-        
-        for i, vm in enumerate(vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key)):
-            if top is not None and i == top:
-                break
-            
-            try:
-                logger.info(f"Analyze vm {vm.name} nics")
-
-                info = extract_nics(vm, vcenter=vcenter)
-
-                extra_config = dictify_value(vm.config.extraConfig)
-                os_family = get_os_family(extra_config, vm.config.guestFullName)
-                os_version = get_os_version(extra_config)
-
-                mapped_guests: list[vim.vm.GuestInfo.NicInfo] = []
-                for nic in info.nics:
-                    for guest in nic.guests:
-                        mapped_guests.append(guest)
-
-                t_nics_per_vm.append([
-                    vm.name, # vm
-                    vm.runtime.powerState, # power_state
-                    os_family,
-                    os_version,
-                    len(info.nics), # 'device_networks',
-                    len(mapped_guests) + len(info.unmapped_guests), # 'guest_networks',
-                    len(mapped_guests), # 'with_mappings',
-                    len(info.unmapped_guests), # 'without_mappings',
-                    [guest.macAddress for guest in mapped_guests], # 'mapped_guest',
-                    [guest.macAddress for guest in info.unmapped_guests], # 'unmapped_guests',
-                    info.issues,
-                ])
-
-                for nic in info.nics:
-                    backing_typename = type(nic.device.backing).__name__
-                    if backing_typename.startswith('vim.vm.device.VirtualEthernetCard.'):
-                        backing_typename = backing_typename[len('vim.vm.device.VirtualEthernetCard.'):]
-
-                    if isinstance(nic.device.backing, vim.vm.device.VirtualEthernetCard.DistributedVirtualPortBackingInfo):
-                        connection_obj = nic.device.backing.port
-                        network_obj = vcenter.get_portgroup_by_key(connection_obj.portgroupKey)
-                        if network_obj:
-                            network = network_obj.name
-                        else:
-                            switch_obj = vcenter.get_switch_by_uuid(connection_obj.switchUuid)
-                            if switch_obj:
-                                network = f"Switch {switch_obj.name} (port {connection_obj.portKey})"
-                            else:
-                                network = f"Switch {connection_obj.switchUuid} (port {connection_obj.portKey})"
-                    elif isinstance(nic.device.backing, vim.vm.device.VirtualEthernetCard.NetworkBackingInfo):
-                        network_obj = nic.device.backing.network
-                        network = network_obj.name
-                    else:
-                        network = None
-
-                    ip_addresses = []
-                    networks = []
-                    for guest in nic.guests:
-                        for ip in guest.ipAddress:
-                            ip_addresses.append(ip)
-                        networks.append(guest.network)
-                    
-                    t_nics.append([
-                        vm.name, # vm
-                        vm.runtime.powerState, # power_state
-                        os_family,
-                        os_version,
-                        backing_typename, # backing
-                        network,
-                        nic.device.addressType, # address_type
-                        nic.device.key, # key
-                        nic.device.macAddress.lower(), # mac
-                        ip_addresses,
-                        networks,
-                    ])
-
-                for guest in info.unmapped_guests:
-                    t_nics.append([
-                        vm.name, # vm
-                        vm.runtime.powerState, # power_state
-                        os_family,
-                        os_version,
-                        None, # backing
-                        None, # network
-                        None, # address_type
-                        guest.deviceConfigId, # key
-                        guest.macAddress.lower(), # mac
-                        guest.ipAddress,
-                        guest.network,
-                    ])
-
-            except Exception as err:
-                logger.exception(f"Error while analyzing {str(vm)} nics: {err}")
-
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('search', nargs='*', help="Search term(s).")
-    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
-    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
-    parser.add_argument('--top', type=int)
-    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
-
-list_vm_nics.add_arguments = _add_arguments
-
-
-def extract_nics(vm: vim.VirtualMachine, *, vcenter: VCenterClient):
-    info = VmNics(vm)
-
-    # Retrieve nic devices
-    nics_per_key: dict[int,VmNic] = {}
-    keys_to_ignore = set()
-    for obj in vm.config.hardware.device:
-        if not isinstance(obj, vim.vm.device.VirtualEthernetCard):
-            continue
-
-        nic = VmNic(obj, vcenter=vcenter)
-        info.nics.append(nic)
-
-        if obj.key is None:
-            info._append_issue(f"Device NIC has no key: {obj}")
-        elif not isinstance(obj.key, int):
-            info._append_issue(f"Device NIC has a non-int key: {obj}")
-        elif obj.key in nics_per_key:
-            info._append_issue(f"Several NIC have key {obj.key}")
-            keys_to_ignore.add(obj.key)
-        else:
-            nics_per_key[obj.key] = nic
-
-    for key in keys_to_ignore:
-        del nics_per_key[key]
-
-    # Retrieve guest NICs
-    # Associate them to device NICs if a consistent mapping is provided
-    for obj in vm.guest.net:
-        if obj.deviceConfigId and obj.deviceConfigId != -1:
-            nic = nics_per_key.get(obj.deviceConfigId)
-            if not nic:
-                info._append_issue(f"Guest NIC {obj.macAddress} mapped to unknown device NIC key: {obj.deviceConfigId}")
-                info.unmapped_guests.append(obj)
-            else:
-                nic.guests.append(obj)
-        else:
-            info.unmapped_guests.append(obj)
-
-    # Verify consistency of mapped guests address MACs
-    for nic in info.nics:
-        for guest in nic.guests:
-            if guest.macAddress.lower() != nic.device.macAddress.lower():
-                info._append_issue(f"Inconsistent MAC address ({guest.macAddress.lower()}) for guest {guest.ipAddress} (device {nic.device.key} MAC address: {nic.device.macAddress.lower()})")
-
-    return info
-
-
-class VmNics:
-    def __init__(self, vm: vim.VirtualMachine):
-        self.vm = vm
-        self.nics: list[VmNic] = []
-        self.unmapped_guests: list[vim.vm.GuestInfo.NicInfo] = []
-        self.issues: list[str] = []
-
-    def _append_issue(self, message: str):
-        logger.warning(f"{self.vm.name}: {message}")
-        self.issues.append(message)
-
-    @property
-    def guests(self):
-        for nic in self.nics:
-            for guest in nic.guests:
-                yield guest
-
-        for guest in self.unmapped_guests:
-            yield guest
-
-    @property
-    def network_names(self):
-        names = set()
-
-        for nic in self.nics:
-            name = nic.network_name
-            if name:
-                names.add(name)
-
-        return sorted(names)      
-    
-    def to_dict(self):
-        data = []
-
-        for nic in self.nics:
-            data.append(nic.to_dict())
-
-        if self.unmapped_guests:
-            for guest in self.unmapped_guests:
-                data.append({'key': guest.deviceConfigId, 'mac': guest.macAddress.lower(), 'guest':  self._get_guest_dict(guest)})
-
-        return data
-    
-    def to_summary(self, ip_version: int = None):
-        result = ''
-        
-        for nic in self.nics:
-            result += (' | ' if result else '') + nic.to_summary(ip_version=ip_version)
-
-        if self.unmapped_guests:
-            for guest in self.unmapped_guests:
-                result += (' | ' if result else '') + f"unmapped {guest.macAddress.lower()}: {guest.network} (" + VmNics._get_guest_summary(guest, ip_version=ip_version) + ")"
-
-        return result
-    
-    @classmethod
-    def _get_guest_dict(cls, guest: vim.vm.GuestInfo.NicInfo):
-        data = {}
-        data['ips'] = guest.ipAddress
-        data['connected'] = guest.connected
-        data['network_name'] = guest.network
-        return data
-    
-    @classmethod
-    def _get_guest_summary(cls, guest: vim.vm.GuestInfo.NicInfo, ip_version: int = None):        
-        ip_addresses: list[IPv4Address|IPv6Address] = []
-        for ip_str in guest.ipAddress:
-            ip = ip_address(ip_str)
-            if ip_version is None or ip.version == ip_version:
-                ip_addresses.append(ip)
-
-        ip_addresses.sort()
-                
-        result = ''
-        for ip in ip_addresses:
-            result += (', ' if result else '') + ip.compressed
-        result += (', ' if result else '') + ('connected' if guest.connected else 'notConnected')
-        return result
-
-
-class VmNic:
-    def __init__(self, device: vim.vm.device.VirtualEthernetCard, *, vcenter: VCenterClient):
-        self.vcenter = vcenter
-        self.device = device
-        self.guests: list[vim.vm.GuestInfo.NicInfo] = []
-
-    @property
-    def network(self):
-        if isinstance(self.device.backing, vim.vm.device.VirtualEthernetCard.DistributedVirtualPortBackingInfo):
-            connection_obj = self.device.backing.port
-            network_obj = self.vcenter.get_portgroup_by_key(connection_obj.portgroupKey)
-            if network_obj:
-                return network_obj
-            else:
-                switch_obj = self.vcenter.get_switch_by_uuid(connection_obj.switchUuid)
-                port_key = int(connection_obj.portKey) if connection_obj.portKey is not None and re.match(r'^\d+$', connection_obj.portKey) else connection_obj.portKey
-                if switch_obj:
-                    return {'switch': switch_obj, 'port': port_key}
-                else:
-                    return {'switch_uuid': connection_obj.switchUuid, 'port': port_key}
-        elif isinstance(self.device.backing, vim.vm.device.VirtualEthernetCard.NetworkBackingInfo):
-            return self.device.backing.network
-        else:
-            return None
-        
-    @property
-    def network_name(self):
-        network = self.network
-        if not network:
-            return None
-        elif isinstance(network, (vim.dvs.DistributedVirtualPortgroup, vim.Network)):
-            return network.name
-        elif isinstance(network, dict):
-            result = ''
-            for key, value in network.items():
-                if isinstance(value, vim.ManagedEntity):
-                    value = value.name
-                result += (', ' if result else '') + f"{key}: {value}"
-            return str(network)
-        else:
-            return str(network)
-
-    def to_dict(self):
-        data = {}
-        data['key'] = self.device.key
-        data['mac'] = self.device.macAddress.lower()
-
-        # vim.vm.device.VirtualEthernetCard.NetworkBackingInfo, vim.vm.device.VirtualEthernetCard.DistributedVirtualPortBackingInfo, etc
-        backing_typename = type(self.device.backing).__name__
-        if backing_typename.startswith('vim.vm.device.VirtualEthernetCard.'):
-            backing_typename = backing_typename[len('vim.vm.device.VirtualEthernetCard.'):]
-        data['backing'] = backing_typename
-
-        if network := self.network:
-            if isinstance(network, dict) and 'switch' in dict:
-                network['switch'] = {'name': network['switch'].name, 'ref': get_obj_ref(network['switch'])}
-            else:
-                network = {'name': network.name, 'ref': get_obj_ref(network)}
-            data['network'] = network
-
-        data['address_type'] = self.device.addressType
-
-        if self.guests:
-            data['guests'] = [VmNics._get_guest_dict(guest) for guest in self.guests]
-        
-        return data
-    
-    def to_summary(self, ip_version: int = None):
-        result = f"{self.device.macAddress.lower()}: {self.network_name}"
-        if self.guests:
-            result += " ("
-            for i, guest in enumerate(self.guests):
-                if i > 0:
-                    result += ', '
-                result += VmNics._get_guest_summary(guest, ip_version=ip_version)
-            result += ")"
-        return result
-
-#endregion
-
-
-def get_tools_version_number(toolsversion: str):
-    if re.match(r'^\d+$', toolsversion):
-        toolsversion = int(toolsversion)
-        if toolsversion == 0 or toolsversion == 2147483647:
-            return None
-        return toolsversion    
-    elif toolsversion:
-        return str(toolsversion)
-    else:
-        return None
-
-
-def get_os_family(extra_config: dict, configured_fullname: str):
-    def get_family_from_configured(fullname: str):
-        if m := re.match(r'^(.+) \(\d\d\-bit\)$', fullname):
-            fullname = m[1]
-            
-        lower_fullname = fullname.lower()
-        if 'windows' in lower_fullname:
-            return "Windows"
-        elif 'linux' in lower_fullname or 'centos' in lower_fullname:
-            return "Linux"
-        elif lower_fullname == 'other':
-            return None
-        else:
-            return fullname
-      
-    if 'guestInfo.detailed.data' in extra_config:
-        line = extra_config['guestInfo.detailed.data']
-        if m := re.match(r".*familyName='([^']+)'.*", line):
-            return m[1]
-    elif 'guestOS.detailed.data' in extra_config:
-        data = extra_config.get("guestOS.detailed.data")
-        if isinstance(data, dict) and 'familyName' in data:
-            return data['familyName']
-
-    if configured_fullname:
-        return get_family_from_configured(configured_fullname)
-
-
-
-def get_os_version(extra_config: dict):
-    if 'guestInfo.detailed.data' in extra_config:
-        line = extra_config['guestInfo.detailed.data']
-        if m := re.match(r".*prettyName='([^']+)'.*", line):
-            return m[1]
-        else:
-            return line
-    elif 'guestOS.detailed.data' in extra_config:
-        data = extra_config.get("guestOS.detailed.data")
-        if isinstance(data, dict) and 'prettyName' in data:
-            return data['prettyName']
-        else:
-            return str(data)
-    else:
-        return None
-
-
-def get_os_distro_version(extra_config: dict):
-    if 'guestInfo.detailed.data' in extra_config:
-        line = extra_config['guestInfo.detailed.data']
-        if m := re.match(r".*distroVersion='([^']+)'.*", line):
-            return m[1]
-    if 'guestOS.detailed.data' in extra_config:
-        data = extra_config.get("guestOS.detailed.data")
-        if isinstance(data, dict) and 'distroVersion' in data:
-            return data['distroVersion']
-
-
-def get_os_kernel_version(extra_config: dict):
-    if 'guestInfo.detailed.data' in extra_config:
-        line = extra_config['guestInfo.detailed.data']
-        if m := re.match(r".*kernelVersion='([^']+)'.*", line):
-            return m[1]
-    if 'guestOS.detailed.data' in extra_config:
-        data = extra_config.get("guestOS.detailed.data")
-        if isinstance(data, dict) and 'kernelVersion' in data:
-            return data['kernelVersion']
-        
-
-def get_guestinfo_publish_time(extra_config: dict):
-    if not 'guestinfo.appInfo' in extra_config:
-        return
-    
-    appinfo_str = extra_config['guestinfo.appInfo']
-    if not isinstance(appinfo_str, str):
-        return str(appinfo_str)
-    
-    if appinfo_str == "":
-        return
-    
-    try:
-        appinfo = json.loads(appinfo_str)
-    except json.decoder.JSONDecodeError as err:
-        return f"Cannot parse \"{appinfo_str}\": {err}"
-
-    if 'publishTime' in appinfo:
-        return datetime.fromisoformat(appinfo['publishTime'])
-
-
-def get_tools_version(extra_config: dict, version_number: str):
-    if 'guestinfo.vmtools.versionNumber' in extra_config and 'guestinfo.vmtools.description' in extra_config:
-        if extra_config['guestinfo.vmtools.versionNumber'] == version_number:
-            return extra_config['guestinfo.vmtools.description']
-
-
-def get_custom_values(vm: vim.VirtualMachine):
-    available_fields = {}
-    custom_values = {}
-
-    for field in vm.availableField:
-        available_fields[field.key] = field.name
-
-    for value in vm.value:
-        custom_values[available_fields[value.key]] = value.value
-        
-    for value in vm.customValue:
-        custom_values[available_fields[value.key]] = value.value
-
-    return custom_values
+"""
+Manage virtual machines.
+"""
+from __future__ import annotations
+
+import json
+import logging
+import os
+import re
+from argparse import ArgumentParser, RawTextHelpFormatter, _SubParsersAction
+from datetime import datetime
+from io import IOBase
+from ipaddress import IPv4Address, IPv6Address, ip_address
+from pathlib import Path
+from typing import Any, Callable, Literal
+from time import sleep
+
+from pyVmomi import vim
+from zut import (Header, add_func_command, get_description_text, get_help_text,
+                 gigi_bytes, out_table, slugify)
+from zut.excel import ExcelRow, ExcelWorkbook, split_excel_path
+
+from . import (Tag, VCenterClient, dictify_obj, dictify_value, get_obj_name, get_obj_path,
+               get_obj_ref, CONFIG, CONFIG_SECTION)
+
+logger = logging.getLogger(__name__)
+
+_DEFAULT_OUT = '{title}.csv'
+
+def add_vm_commands(commands_subparsers: _SubParsersAction[ArgumentParser], *, name: str):
+    parser = commands_subparsers.add_parser(name, help=get_help_text(__doc__), description=get_description_text(__doc__), formatter_class=RawTextHelpFormatter, add_help=False)
+
+    group = parser.add_argument_group(title='Command options')
+    group.add_argument('-h', '--help', action='help', help=f"Show this command help message and exit.")
+
+    subparsers = parser.add_subparsers(title='Sub commands')
+    add_func_command(subparsers, list_vms, name='list')
+    add_func_command(subparsers, list_vm_disks, name='disks')
+    add_func_command(subparsers, list_vm_nics, name='nics')
+    
+    # Operations
+    add_func_command(subparsers, start_vms, name='start')
+    add_func_command(subparsers, stop_vms, name='stop')
+    add_func_command(subparsers, suspend_vms, name='suspend')    
+    add_func_command(subparsers, reconfigure_vms, name='reconfigure')
+
+
+#region List
+
+def list_vms(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: os.PathLike|IOBase = _DEFAULT_OUT):
+    extract_categories = CONFIG.getlist(CONFIG_SECTION, 'extract_categories', delimiter=',')
+    extract_custom_values = CONFIG.getlist(CONFIG_SECTION, 'extract_custom_values', delimiter=',')
+
+    headers = [
+        'name',
+        'ref',
+        'overall_status',
+        'config_status',
+        'template',
+        # Config
+        'vcpu',
+        'cores_per_socket',
+        Header('memory', fmt='gib'),
+        Header('disk_capacity', fmt='gib'),
+        Header('disk_freespace', fmt='gib'),
+        'disk_count',
+        'nic_count',
+        # Dossier / rangement
+        'folder',
+    ]
+
+    for cat in extract_categories:
+        headers.append(cat)
+
+    headers += [
+        'other_tags' if extract_categories else 'tags',
+    ]
+
+    for cv in extract_custom_values:
+        headers.append(cv)
+    
+    headers += [
+        'other_custom_values' if extract_custom_values else 'custom_values',
+        'annotation',
+        'create_date',
+        'change_date',
+        # Config details
+        'hostname',
+        'network',
+        'disk',
+        # ResourcePool / runtime
+        'cluster',
+        'resourcepool',
+        'host',
+        'power_state',
+        'paused',
+        'connection_state',
+        'boot_time',
+        'hw_version',
+        # Guest info
+        'os_family',
+        'os_version',
+        'os_distro_version',
+        'os_kernel_version',
+        'tools_status',
+        'tools_running_status',
+        'tools_version_number',
+        'tools_version',
+        'guestinfo_publish_time',
+    ]
+
+    with out_table(out, title='vms', dir=vcenter.out_dir, env=vcenter.env, headers=headers, after1970=True) as t:
+        for obj in vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key):  
+            try:
+                logger.info(f"Analyze vm {obj.name}")
+
+                disks = extract_disks(obj)
+                nics = extract_nics(obj, vcenter=vcenter)
+                extra_config = dictify_value(obj.config.extraConfig) if obj.config is not None else {}
+
+                row = [
+                    obj.name,
+                    get_obj_ref(obj),
+                    obj.overallStatus,
+                    obj.configStatus,
+                    obj.config.template if obj.config is not None else None,
+                    # Config
+                    obj.config.hardware.numCPU if obj.config is not None else None,
+                    obj.config.hardware.numCoresPerSocket if obj.config is not None else None,
+                    obj.config.hardware.memoryMB * 1024 * 1024 if obj.config is not None else None,
+                    disks.capacity if disks is not None else None,
+                    disks.freespace if disks is not None else None,
+                    obj.summary.config.numVirtualDisks,
+                    obj.summary.config.numEthernetCards,
+                    # Dossier / rangement
+                    get_obj_path(obj.parent),
+                ]
+
+                tags = vcenter.get_obj_tags(obj)
+                for category_name in extract_categories:
+                    category_tags: list[Tag] = []
+                    for tag in tags:
+                        if tag.category.name == category_name:
+                            category_tags.append(tag)
+                    for tag in category_tags:
+                        tags.remove(tag)
+                    row.append([tag.name for tag in category_tags])
+
+                # other tags
+                row.append([f"{tag.name} ({tag.category.name})" for tag in tags])
+                
+                custom_values = get_custom_values(obj)
+                for cv in extract_custom_values:
+                    row.append(custom_values.pop(cv, None))
+                other_custom_values = ' | '.join(f"{key}: {value}" for key, value in custom_values.items())
+
+                row += [
+                    other_custom_values,
+                    obj.config.annotation if obj.config is not None else None,
+                    obj.config.createDate if obj.config is not None else None,
+                    datetime.fromisoformat(obj.config.changeVersion) if obj.config is not None else None,
+                    # Config details
+                    obj.guest.hostName,
+                    nics.to_summary(ip_version=4) if nics is not None else None,
+                    disks.to_summary() if disks is not None else None,
+                    # ResourcePool / runtime
+                    obj.resourcePool.owner.name if obj.resourcePool else None,
+                    get_obj_name(obj.resourcePool),
+                    obj.runtime.host.name if obj.runtime.host is not None else None,
+                    obj.runtime.powerState,
+                    obj.runtime.paused,
+                    obj.runtime.connectionState,
+                    obj.runtime.bootTime,
+                    obj.config.version if obj.config is not None else None,
+                    # Guest info
+                    get_os_family(extra_config, obj.config.guestFullName) if obj.config is not None else None,
+                    get_os_version(extra_config),
+                    get_os_distro_version(extra_config),
+                    get_os_kernel_version(extra_config),
+                    obj.guest.toolsStatus,  # nominal: toolsOk
+                    obj.guest.toolsRunningStatus,  # nominal: guestToolsRunning
+                    get_tools_version_number(obj.guest.toolsVersion),  # version number
+                    get_tools_version(extra_config, obj.guest.toolsVersion),      
+                    get_guestinfo_publish_time(extra_config),
+                ]
+                
+                t.append(row)
+            
+            except Exception as err:
+                logger.exception(f"Error while analyzing {obj}: {err}")
+
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output table (default: %(default)s).")
+
+list_vms.add_arguments = _add_arguments
+
+#endregion
+
+
+#region Start, stop, suspend, reconfigure
+
+_DEFAULT_START_BATCH = 10
+_DEFAULT_BATCH_PAUSE = 60.0
+
+def start_vms(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', batch: int = _DEFAULT_START_BATCH, batch_pause: float = _DEFAULT_BATCH_PAUSE):
+    _invoke_and_track('PowerOn', 'poweredOn', vcenter, search, normalize=normalize, key=key, batch=batch, batch_pause=batch_pause)
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument('-b', '--batch', type=int, default=_DEFAULT_START_BATCH, help="Batch size: maximum number of VMs to start at the same time (default: %(default)s).")
+    parser.add_argument('--batch-pause', type=float, default=_DEFAULT_BATCH_PAUSE, help="Batch pause: duration of pauses between batchs, in seconds (default: %(default)s).")
+
+start_vms.add_arguments = _add_arguments
+
+
+def stop_vms(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', force: bool = False):
+    if force:
+        _invoke_and_track('PowerOff', 'poweredOff', vcenter, search, normalize=normalize, key=key)
+    else:
+        _invoke_and_track('ShutdownGuest', 'poweredOff', vcenter, search, normalize=normalize, key=key)
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument('-f', '--force', action='store_true', help="Force operation.")
+
+stop_vms.add_arguments = _add_arguments
+
+
+def suspend_vms(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', force: bool = False):
+    if force:
+        _invoke_and_track('Suspend', 'suspended', vcenter, search, normalize=normalize, key=key)
+    else:
+        _invoke_and_track('StandbyGuest', 'suspended', vcenter, search, normalize=normalize, key=key)
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument('-f', '--force', action='store_true', help="Force operation.")
+
+suspend_vms.add_arguments = _add_arguments
+
+
+def _invoke_and_track(op: str, target_status: str, vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', batch: int = None, batch_pause: float = _DEFAULT_BATCH_PAUSE):
+    # Idea: https://github.com/reubenur-rahman/vmware-pyvmomi-examples/blob/master/vm_power_ops.py
+    task_helpers: dict[vim.Task,ReportHelper] = {}
+    
+    def task_success_callback(task):
+        helper = task_helpers[task]
+        if helper.row:
+            helper.row['status'] = 'SUCCESS'
+            helper.row['details'] = None
+
+    def task_error_callback(task, details):
+        helper = task_helpers[task]
+        if helper.row:
+            helper.row['status'] = 'ERROR'
+            helper.row['details'] = details
+
+    tasks: dict[vim.VirtualMachine,str] = {}
+    loop_objs: dict[vim.VirtualMachine,ReportHelper] = {}
+    for i, vm in enumerate(vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key)):
+        if batch is not None and i > 0 and i % batch == 0:
+            logger.info(f"Handled {i} VMs, wait for {batch_pause} seconds")
+            sleep(batch_pause)
+
+        log_prefix = f"{vm.name} ({get_obj_ref(vm)})"
+        logger.info(f"{op} {log_prefix}...")
+        func = getattr(vm, op)
+        helper = ReportHelper(log_prefix=log_prefix)
+        try:
+            task = func()
+            if task is not None:
+                tasks[task] = helper.log_prefix
+                task_helpers[task] = helper
+            else:
+                loop_objs[vm] = helper
+        except vim.fault.InvalidPowerState as err:
+            helper.error(f"Invalid current state \"{err.existingState}\" (expected \"{err.requestedState}\")")
+        except vim.fault.ToolsUnavailable as err:
+            helper.error(f"VMWare Tools is not running")
+        except Exception as err:
+            helper.error(f"{err}")
+
+    if tasks:
+        vcenter.wait_for_task(tasks, success_callback=task_success_callback, error_callback=task_error_callback)
+
+    total_seconds = 60
+    remaining_seconds = total_seconds
+    while len(loop_objs) > 0 and remaining_seconds > 0:
+        if remaining_seconds % 10 == 0:
+            logger.info("Wait %s entities to reach status %s (%s seconds max)", len(loop_objs), target_status, remaining_seconds)
+        sleep(1)
+
+        vms_to_remove = []
+        for vm, helper in loop_objs.items():
+            if vm.runtime.powerState == target_status:
+                helper.success()
+                vms_to_remove.append(vm)
+
+        for vm in vms_to_remove:
+            del loop_objs[vm]
+
+        remaining_seconds -= 1
+
+    for vm, helper in loop_objs.items():
+        helper.error(f"VM still not {target_status} after {total_seconds} seconds")
+
+
+DEFAULT_RECONFIGURE_FILE = 'vms_reconfigure.xlsx'
+DEFAULT_RECONFIGURE_TABLE = 'vms'
+
+def reconfigure_vms(vcenter: VCenterClient, path: str|Path = DEFAULT_RECONFIGURE_FILE, top: int = None, ignore_invalid_current: bool = False):
+    """
+    Reconfigure VMs (vcpu, memory, annotation, custom fields) as a mass operation, using an Excel file.
+    """
+      
+    class FieldDef:
+        def __init__(self, name: str, type: type, getter: Callable[[vim.VirtualMachine],Any]|Literal['__customvalue__'], target_key:str|int, target_formatter: Callable[[vim.VirtualMachine],Any] = None):
+            """
+            - `key`: if str, this is the reconfigure ConfigSpec argument to use. If int, this is the custom_value key to use.
+            """
+            self.name = name
+            self.type = type
+            self.getter = getter
+            self.target_key = target_key
+            self.target_formatter = target_formatter
+
+        def get_from_vm(self, vm: vim.VirtualMachine):
+            if self.getter == '__customvalue__':
+                for kv in vm.customValue:
+                    if kv.key == self.target_key:
+                        return kv.value
+            else:
+                return self.getter(vm)
+
+        def get_from_row(self, row: ExcelRow, suffix: str = None):
+            value = row.get(f"{self.name}_{suffix}" if suffix else self.name)
+            if value is None or value == '':
+                return None
+            if self.type == str and value == '-':
+                return ''
+            return self.type(value)
+        
+        def format_for_target(self, value):
+            if not self.target_formatter:
+                return value
+            return self.target_formatter(value)
+
+    fielddefs: list[FieldDef] = [
+        FieldDef('vcpu', int, lambda vm: vm.config.hardware.numCPU, 'numCPUs'),
+        FieldDef('memory', float, lambda vm: vm.config.hardware.memoryMB / 1024.0, 'memoryMB', lambda val: int(val * 1024.0)),
+        FieldDef('annotation', str, lambda vm: vm.config.annotation, 'annotation'),
+    ]
+
+    for cf in vcenter.service_content.customFieldsManager.field:
+        if cf.managedObjectType == vim.VirtualMachine:
+            fielddefs.append(FieldDef(cf.name, str, '__customvalue__', cf.key))
+    
+    path, tablename = split_excel_path(path, default_table_name=DEFAULT_RECONFIGURE_TABLE, dir=vcenter.out_dir, env=vcenter.env)
+
+    workbook = ExcelWorkbook(path)
+    table = workbook.get_or_create_table(tablename)
+    
+    helpers: dict[str,ReportHelper] = {}
+    search_by_ref = 'ref' in table.column_names
+    for row in table:
+        if search_by_ref:
+            if row['ref']:
+                if row.get('status') == 'IGNORE':
+                    logger.info(f"Ignore {row['ref']}")
+                    continue
+                helpers[row['ref']] = ReportHelper(row=row)
+        else:
+            if row['name']:
+                if row.get('status') == 'IGNORE':
+                    logger.info(f"Ignore {row['name']}")
+                    continue
+                helpers[slugify(row['name'])] = ReportHelper(row=row)
+        row['status'] = None
+        row['details'] = None
+    
+    n = 0
+    for vm in vcenter.iter_objs(vim.VirtualMachine):
+        if top is not None and n == top:
+            logger.warning(f"Stop after {n} VMs")
+            break
+
+        key = get_obj_ref(vm) if search_by_ref else slugify(vm.name)
+        helper = helpers.get(key)
+        if not helper:
+            continue
+        
+        if helper.found:
+            logger.error(f"VM {vm.name}: ignore (several VMs with key \"{key}\")")
+            continue
+        helper.found = True
+
+        n += 1        
+        logger.info(f"Handle {vm.name} ({get_obj_ref(vm)})")
+        row = helper.row
+
+        try:
+            if search_by_ref and slugify(vm.name) != slugify(row['name']):
+                helper.error(f"Invalid VM name: expected {vm.name}")
+                continue
+
+            if vm.config.template:
+                helper.error(f"This is a template")
+                continue
+
+            if vm.runtime.powerState != 'poweredOff':
+                helper.error(f"Not powered off")
+                continue
+
+            config_previous: dict[str|int,Any] = {}
+            config_targets: dict[str|int,Any] = {}
+            invalid_current = ''
+
+            # Prepare reconfiguration
+            change_version = vm.config.changeVersion  # used to guard against updates that have happened between when configInfo is read and when it is applied
+
+            for fielddef in fielddefs:
+                target = fielddef.get_from_row(row, 'target')
+                if target is None:
+                    continue
+
+                current = fielddef.get_from_vm(vm)
+                current_expected = fielddef.get_from_row(row)
+                if current_expected is not None:
+                    if current_expected != current and not ignore_invalid_current:
+                        invalid_current += (', ' if invalid_current else '') + f"current {fielddef.name}: {'(empty)' if current == '' else current}"   
+                        continue
+
+                if target != current:
+                    config_previous[fielddef.target_key] = fielddef.format_for_target(current)
+                    config_targets[fielddef.target_key] = fielddef.format_for_target(target)
+
+            if invalid_current:
+                helper.error(f"Invalid {invalid_current}")
+                continue
+
+            if not config_targets:
+                helper.success("Nothing to do")
+                continue
+
+            config_targets_reconfigure = {}
+            config_targets_customfields = {}
+            for key, value in config_targets.items():
+                if isinstance(key, str):
+                    config_targets_reconfigure[key] = value
+                else:
+                    config_targets_customfields[key] = value
+
+            # Perform the reconfiguration
+            if config_targets_reconfigure:
+                logger.debug("Reconfigure VM: %s", config_targets_reconfigure)
+                configspec = vim.vm.ConfigSpec(**config_targets_reconfigure, changeVersion=change_version)
+                task = vm.ReconfigVM_Task(configspec)
+                vcenter.wait_for_task(task)
+
+            for key, value in config_targets_customfields.items():
+                logger.debug("Set custom field %s: %s", key, value)
+                vcenter.service_content.customFieldsManager.SetField(vm, key, value)
+
+            # Verification
+            success = True
+            details = ''
+
+            for fielddef in fielddefs:
+                if not fielddef.target_key in config_targets:
+                    continue # field not modified
+
+                previous_value = config_previous[fielddef.target_key]
+                target_value = config_targets[fielddef.target_key]
+                new_value = fielddef.format_for_target(fielddef.get_from_vm(vm))
+                details += (', ' if details else '') + f"{fielddef.target_key}: {'(empty)' if previous_value == '' else previous_value} -> {'(empty)' if new_value == '' else new_value}"
+
+                if new_value != target_value:
+                    success = False
+                    details += ' [ERROR]'
+
+            if success:
+                helper.success(details)
+            else:
+                helper.error(details)
+        
+        except Exception as err:
+            logger.exception(str(err))
+            row['status'] = type(err).__name__
+            row['details'] = str(err)
+
+    # Report not found
+    for key, helper in helpers.items():
+        if not helper.found:
+            helper.error(f"VM {key} not found")
+
+    workbook.close()
+
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('path', nargs='?', default=DEFAULT_RECONFIGURE_FILE, help="Path to Excel file describing VMs to reconfigure.")
+    parser.add_argument('--top', type=int)
+    parser.add_argument('--ignore-invalid-current', action='store_true')
+
+reconfigure_vms.add_arguments = _add_arguments
+
+
+class ReportHelper:
+    def __init__(self, *, log_prefix: str, row: ExcelRow = None, found: bool = False):
+        self.log_prefix = log_prefix
+        self.row = row
+        self.found = found
+
+    def success(self, details: str = None):
+        logger.info((f"{self.log_prefix }: " if self.log_prefix else '') + f"SUCCESS{f': {details}' if details else ''}")
+        if self.row:
+            self.row['status'] = 'SUCCESS'
+            self.row['details'] = details
+
+    def error(self, details: str):
+        logger.error((f"{self.log_prefix }: " if self.log_prefix else '') + f"{details}")
+        if self.row:
+            self.row['status'] = 'ERROR'
+            self.row['details'] = details
+
+#endregion
+
+
+#region Disks
+
+def list_vm_disks(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: str = _DEFAULT_OUT, top: int = None):
+    """
+    Analyze VM disks.
+    """
+    disks_per_vm_headers = [
+        'vm',
+        'device_disks',
+        'guest_disks',
+        'with_mappings',
+        'without_mappings',
+        'mapped_guest',
+        'unmapped_guest',
+        Header('capacity', fmt='gib'),
+        Header('freespace', fmt='gib'),
+        Header('mapped_disks_capacity', fmt='gib'),
+        Header('mapped_guests_capacity', fmt='gib'),
+        Header('mapped_guests_freespace', fmt='gib'),
+        Header('unmapped_disks_capacity', fmt='gib'),
+        Header('unmapped_guests_capacity', fmt='gib'),
+        Header('unmapped_guests_freespace', fmt='gib'),
+        'issues',
+    ]
+
+    disks_headers = [
+        'vm',
+        'key',
+        'backing',
+        'datastore',
+        'filename',
+        'diskmode',
+        'sharing',
+        'thin_provisioned',
+        'compatibility_mode',
+        'identification',
+        'remaining_backing_info',
+        Header('capacity', fmt='gib'),
+        Header('freespace', fmt='gib'),
+        'mapping',
+        'guests',
+        Header('guests_capacity', fmt='gib'),
+        Header('guests_freespace', fmt='gib'),
+    ]
+    
+    with (out_table(out, title='vm_disks', headers=disks_headers, dir=vcenter.out_dir, env=vcenter.env) as t_disks,
+          out_table(out, title='vm_disks_per_vm', headers=disks_per_vm_headers, dir=vcenter.out_dir, env=vcenter.env) as t_disks_per_vm):
+        
+        for i, vm in enumerate(vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key)):
+            if top is not None and i == top:
+                break
+            
+            try:
+                logger.info(f"Analyze vm {vm.name} disks")
+
+                info = extract_disks(vm)
+
+                mapped_guests: list[vim.vm.GuestInfo.DiskInfo] = []
+                if info is not None:
+                    for disk in info.disks:
+                        for guest in disk.guests:
+                            mapped_guests.append(guest)
+
+                t_disks_per_vm.append([
+                    vm.name, # vm
+                    len(info.disks) if info is not None else None, # 'device_disks',
+                    len(mapped_guests) + len(info.unmapped_guests) if info is not None else None, # 'guest_disks',
+                    len(mapped_guests) if info is not None else None, # 'with_mappings',
+                    len(info.unmapped_guests) if info is not None else None, # 'without_mappings',
+                    sorted((guest.diskPath.rstrip(':\\') + f" ({guest.filesystemType})") if guest.filesystemType else guest.diskPath.rstrip(':\\') for guest in mapped_guests) if info is not None else None, # 'mapped_guest',
+                    sorted((guest.diskPath.rstrip(':\\') + f" ({guest.filesystemType})") if guest.filesystemType else guest.diskPath.rstrip(':\\') for guest in info.unmapped_guests) if info is not None else None, # 'unmapped_guests',
+                    info.capacity if info is not None else None,
+                    info.freespace if info is not None else None,
+                    info.mapped_disks_capacity if info is not None and mapped_guests else None,
+                    info.mapped_guests_capacity if info is not None and mapped_guests else None,
+                    info.mapped_guests_freespace if info is not None and mapped_guests else None,
+                    info.unmapped_disks_capacity if info is not None and info.unmapped_disks_capacity > 0 else None,
+                    info.unmapped_guests_capacity if info is not None and info.unmapped_guests else None,
+                    info.unmapped_guests_freespace if info is not None and info.unmapped_guests else None,
+                    info.issues if info is not None else None,
+                ])
+
+                if info is not None:
+                    for disk in info.disks:
+                        device_backing = dictify_obj(disk.device.backing)
+                        backing_typename = type(disk.device.backing).__name__
+                        if backing_typename.startswith('vim.vm.device.VirtualDisk.'):
+                            backing_typename = backing_typename[len('vim.vm.device.VirtualDisk.'):]
+                        datastore = device_backing.pop('datastore', None)
+                        fileName = device_backing.pop('fileName', None)
+                        diskMode = device_backing.pop('diskMode', None)
+                        sharing = device_backing.pop('sharing', None)
+                        thinProvisioned = device_backing.pop('thinProvisioned', None)
+                        compatibilityMode = device_backing.pop('compatibilityMode', None)
+                        
+                        identification = {}
+                        if value := device_backing.pop('uuid', None):
+                            identification['uuid'] = value
+                        if value := device_backing.pop('contentId', None):
+                            identification['contentId'] = value
+                        if value := device_backing.pop('changeId', None):
+                            identification['changeId'] = value
+                        if value := device_backing.pop('parent', None):
+                            identification['parent'] = value
+                        if value := device_backing.pop('deviceName', None): # Raw
+                            identification['deviceName'] = value
+                        if value := device_backing.pop('lunUuid', None): # Raw
+                            identification['lunUuid'] = value
+                        
+                        t_disks.append([
+                            vm.name, # vm
+                            disk.device.key, # key
+                            backing_typename, # backing
+                            datastore['name'] if datastore else None, # datastore
+                            fileName,
+                            diskMode,
+                            sharing,
+                            thinProvisioned,
+                            compatibilityMode,
+                            identification,
+                            device_backing, # remaining_backing_info
+                            disk.capacity,
+                            disk.freespace,
+                            disk.guests_mapping,
+                            sorted((guest.diskPath.rstrip(':\\') + f" ({guest.filesystemType})") if guest.filesystemType else guest.diskPath.rstrip(':\\') for guest in disk.guests), # guests
+                            disk.guests_capacity if disk.guests else None,
+                            disk.guests_freespace if disk.guests else None,
+                        ])
+
+                    for guest in [*info.unmapped_guests, *info.ignored_guests]:
+                        t_disks.append([
+                            vm.name, # vm
+                            None, # key
+                            guest.mappings, # backing
+                            None, # datastore
+                            None, # filename
+                            None, # diskMode
+                            None, # sharing
+                            None, # thin_provisioned
+                            None, # compatibility_mode
+                            None, # identification'
+                            None, # remaining_backing_info
+                            None, # capacity
+                            None, # freespace
+                            'ignored' if guest in info.ignored_guests else 'unmapped', # mapping
+                            (guest.diskPath.rstrip(':\\') + f" ({guest.filesystemType})") if guest.filesystemType else guest.diskPath.rstrip(':\\'), # guests
+                            guest.capacity, # guests_capacity
+                            guest.freeSpace, # guests_freespace
+                        ])
+
+            except Exception as err:
+                logger.exception(f"Error while analyzing {str(vm)} disks: {err}")
+
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument('--top', type=int)
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
+
+list_vm_disks.add_arguments = _add_arguments
+
+
+def extract_disks(vm: vim.VirtualMachine):
+    if vm.config is None:
+        # VM is not yet configured
+        return None
+    
+    info = VmDisks(vm)
+
+    # Retrieve disk devices
+    disks_per_key: dict[int,VmDisk] = {}
+    keys_to_ignore = set()
+    for obj in vm.config.hardware.device:
+        if not isinstance(obj, vim.vm.device.VirtualDisk):
+            continue
+
+        disk = VmDisk(obj)
+        info.disks.append(disk)
+        info.capacity += disk.capacity
+
+        if obj.key is None:
+            info._append_issue(f"Device disk has no key: {obj}")
+        elif not isinstance(obj.key, int):
+            info._append_issue(f"Device disk has a non-int key: {obj}")
+        elif obj.key in disks_per_key:
+            info._append_issue(f"Several disk have key {obj.key}")
+            keys_to_ignore.add(obj.key)
+        else:
+            disks_per_key[obj.key] = disk
+
+    for key in keys_to_ignore:
+        del disks_per_key[key]
+
+    # Retrieve guest disks
+    # Associate them to device disks if a consistent mapping is provided
+    for obj in vm.guest.disk:
+        mappings = obj.mappings
+        if mappings:
+            mapping_keys = set()
+            for mapping in mappings:
+                mapping_keys.add(mapping.key)
+
+            if len(mapping_keys) > 1:
+                info._append_issue(f"Guest disk {obj.diskPath} mapped to several device disk keys: {mapping_keys}")
+                info.unmapped_guests.append(obj)
+
+            else:
+                disk = disks_per_key.get(mapping.key)
+                if not disk:
+                    info._append_issue(f"Guest disk {obj.diskPath} mapped to unknown device disk key: {mapping.key}")
+                    info.unmapped_guests.append(obj)
+
+                else:
+                    disk.guests.append(obj)
+                    disk.guests_mapping = 'key'
+        else:
+            info.unmapped_guests.append(obj)
+
+    # Verify consistency of mapped guests capacity
+    for disk in info.disks:
+        if disk.guests:
+            for guest in disk.guests:
+                disk.guests_capacity += guest.capacity
+                disk.guests_freespace += guest.freeSpace
+            if disk.guests_capacity > disk.capacity:
+                guest_list = ', '.join(guest.diskPath.rstrip(':\\') for guest in disk.guests)
+                info._append_issue(f"Inconsistent capacity ({disk.guests_capacity:,}) for guests {guest_list} (device {disk.device.key} capacity: {disk.capacity:,})")
+
+    # Identify guests to ignore
+    info._identify_ignored_guests()
+    
+    # Try to map remaining guests automatically
+    unmapped_guests = sorted([guest for guest in info.unmapped_guests], key=lambda obj: obj.capacity, reverse=True)
+    unmapped_disks = sorted([disk for disk in info.disks if not disk.guests], key=lambda disk: disk.capacity, reverse=True)
+
+    confirm_mapping = True
+    if len(unmapped_disks) == len(unmapped_guests):
+        for i in range(0, len(unmapped_disks)):
+            disk = unmapped_disks[i]
+            guest = unmapped_guests[i]
+            if guest.capacity > disk.capacity:
+                confirm_mapping = False
+                break
+
+            if i < len(unmapped_disks) - 1:
+                next_disk = unmapped_disks[i+1]
+                if guest.capacity <= next_disk.capacity: # another disk could match
+                    confirm_mapping = False
+                    break
+
+        if confirm_mapping:
+            for i in range(0, len(unmapped_disks)):
+                disk = unmapped_disks[i]
+                guest = unmapped_guests[i]
+                info.unmapped_guests.remove(guest)
+                disk.guests.append(guest)
+                disk.guests_capacity += guest.capacity
+                disk.guests_freespace += guest.freeSpace
+                disk.guests_mapping = 'auto'
+
+    # Finalize capacity and freespace sums
+    for disk in info.disks:
+        if disk.guests:
+            disk.freespace = disk.guests_freespace + (disk.capacity - disk.guests_capacity)
+            info.mapped_guests_capacity += disk.guests_capacity
+            info.mapped_guests_freespace += disk.guests_freespace
+            info.mapped_disks_capacity += disk.capacity
+            info.mapped_disks_freespace += disk.freespace
+        else:
+            info.unmapped_disks_capacity += disk.capacity
+
+    for guest in info.unmapped_guests:
+        info.unmapped_guests_capacity += guest.capacity
+        info.unmapped_guests_freespace += guest.freeSpace
+
+    # (estimation of unmapped disk freespace)
+    if info.unmapped_disks_capacity > 0:
+        if info.unmapped_guests_capacity > info.unmapped_disks_capacity:
+            info.unmapped_disks_freespace = int(info.unmapped_guests_freespace * (info.unmapped_disks_capacity / info.unmapped_guests_capacity))
+        else:
+            info.unmapped_disks_freespace = info.unmapped_guests_freespace + (info.unmapped_disks_capacity - info.unmapped_guests_capacity)
+
+    info.freespace = info.mapped_disks_freespace + info.unmapped_disks_freespace
+
+    return info
+
+
+class VmDisks:
+    def __init__(self, vm: vim.VirtualMachine):
+        self.vm = vm
+        self.disks: list[VmDisk] = []
+        self.unmapped_guests: list[vim.vm.GuestInfo.DiskInfo] = []
+        self.ignored_guests: list[vim.vm.GuestInfo.DiskInfo] = []
+        self.issues: list[str] = []
+
+        self.capacity: int = 0
+        """ Sum of device capacities. """
+
+        self.freespace: int = 0
+        """ Sum of device freespaces. This is sum of mapped device freespaces + an estimation of unmapped freespace. """
+
+        self.mapped_disks_capacity: int = 0
+        self.mapped_disks_freespace: int = 0
+        self.mapped_guests_capacity: int = 0
+        self.mapped_guests_freespace: int = 0
+        
+        self.unmapped_disks_capacity: int = 0
+        self.unmapped_disks_freespace: int = 0
+        self.unmapped_guests_capacity: int = 0
+        self.unmapped_guests_freespace: int = 0
+
+    def _append_issue(self, message: str):
+        logger.warning(f"{self.vm.name}: {message}")
+        self.issues.append(message)
+
+    def _identify_ignored_guests(self):
+        for guest in list(self.unmapped_guests):
+            if self._must_ignore(guest):
+                self.unmapped_guests.remove(guest)
+                self.ignored_guests.append(guest)
+
+    def _must_ignore(self, guest: vim.vm.GuestInfo.DiskInfo):      
+        if guest.diskPath.startswith('C:\\Users\\'):
+            return True
+
+        elif '/' in guest.diskPath and guest.diskPath != '/': # Search Linux mount points with the exact same capacity as a parent. Example: /var/lib/rancher/volumes, /var/lib/kubelet.
+            parts = [part for part in guest.diskPath.split('/')]
+            for n in range(1, len(parts)):
+                search_parent = '/' + '/'.join(parts[1:n])
+                for parent in self.guests:
+                    if parent.diskPath == search_parent and parent.capacity == guest.capacity:
+                        return True
+                    
+        return False
+
+    @property
+    def guests(self):
+        for disk in self.disks:
+            for guest in disk.guests:
+                yield guest
+
+        for guest in self.unmapped_guests:
+            yield guest
+
+        for guest in self.ignored_guests:
+            yield guest
+
+    def to_dict(self, bytes=False):
+        data = []
+
+        for disk in self.disks:
+            data.append(disk.to_dict(bytes=bytes))
+
+        if self.unmapped_guests:
+            guests_data = []
+            data.append({'guests_mapping': 'unmapped', 'guests':  guests_data})
+            for guest in self.unmapped_guests:
+                guests_data.append(self._get_guest_dict(guest, bytes=bytes))
+
+        if self.ignored_guests:
+            guests_data = []
+            data.append({'guests_mapping': 'ignored', 'guests':  guests_data})
+            for guest in self.ignored_guests:
+                guests_data.append(self._get_guest_dict(guest, bytes=bytes))
+
+        return data
+    
+    def to_summary(self):
+        result = ''
+
+        for disk in self.disks:
+            result += (' | ' if result else '') + disk.to_summary()
+
+        if self.unmapped_guests:
+            result += (' | ' if result else '') + f"Unmapped guests ("
+            for i, guest in enumerate(self.unmapped_guests):
+                if i > 0:
+                    result += ', '
+                result += self._get_guest_summary(guest)
+            result += ')'
+
+        return result
+    
+    @classmethod
+    def _get_guest_dict(cls, guest: vim.vm.GuestInfo.DiskInfo, bytes=False):
+        data = {}
+        data['path'] = guest.diskPath
+        data['capacity'] = guest.capacity if bytes else gigi_bytes(guest.capacity)
+        data['freespace'] = guest.freeSpace if bytes else gigi_bytes(guest.freeSpace)
+        if value := guest.filesystemType:
+            data['filesystem'] = value
+        return data
+    
+    @classmethod
+    def _get_guest_summary(cls, guest: vim.vm.GuestInfo.DiskInfo):
+        path = guest.diskPath.rstrip(':\\')
+        return f'{path}: {gigi_bytes(guest.freeSpace):.1f}/{gigi_bytes(guest.capacity):.1f} GiB'
+
+
+class VmDisk:
+    def __init__(self, device: vim.vm.device.VirtualDisk):
+        self.device = device
+        self.guests: list[vim.vm.GuestInfo.DiskInfo] = []
+        self.guests_mapping: Literal['key','auto'] = None
+
+        self.capacity: int = device.capacityInBytes
+        """ Device capacities. """
+
+        self.freespace: int = 0
+        """ Device freespace. This is `guests_freespace + (capacity - guests_capacity)`. """
+
+        self.guests_capacity: int = 0
+        """ Sum of guest capacities. """
+
+        self.guests_freespace: int = 0
+        """ Sum of guest freespaces. """
+
+    def to_dict(self, bytes=False):
+        data = {}
+        data['key'] = self.device.key
+        data['capacity'] = self.capacity if bytes else gigi_bytes(self.capacity)
+
+        if self.guests:
+            data['freespace'] = self.freespace if bytes else gigi_bytes(self.freespace)
+
+        backing_typename = type(self.device.backing).__name__
+        if backing_typename.startswith('vim.vm.device.VirtualDisk.'):
+            backing_typename = backing_typename[len('vim.vm.device.VirtualDisk.'):]
+        data['backing'] = backing_typename
+
+        datastore: vim.Datastore = getattr(self.device.backing, 'datastore', None)
+        if datastore:
+            data['datastore'] = {'name': datastore.name, 'ref': get_obj_ref(datastore)}
+
+        filename: str = getattr(self.device.backing, 'fileName', None)
+        if filename:
+            data['filename'] = filename
+
+        if self.guests_mapping:
+            data['guests_mapping'] = self.guests_mapping
+        if self.guests:
+            data['guests'] = []
+
+            for guest in self.guests:
+                data['guests'].append(VmDisks._get_guest_dict(guest, bytes=bytes))
+        
+        return data
+    
+    def to_summary(self):
+        filename: str = getattr(self.device.backing, 'fileName', None)
+        if filename:
+            identifier = filename
+        else:
+            identifier = f'#{self.device.key}'
+
+        result = f'{identifier}: {gigi_bytes(self.freespace):.1f}/{gigi_bytes(self.capacity):.1f} GiB'
+
+        if self.guests:
+            result += f' ('
+            for i, guest in enumerate(self.guests):
+                if i > 0:
+                    result += ', '
+                result += VmDisks._get_guest_summary(guest)
+            result += ')'
+        return result
+
+#endregion
+
+
+#region NICs
+
+def list_vm_nics(vcenter: VCenterClient, search: list[str|re.Pattern]|str|re.Pattern = None, *, normalize: bool = False, key: str = 'name', out: str = _DEFAULT_OUT, top: int = None):
+    """
+    Analyze VM network interfaces.
+    """
+    nics_per_vm_headers = [
+        'vm',
+        'device_networks',
+        'guest_networks',
+        'with_mappings',
+        'without_mappings',
+        'mapped_guest',
+        'unmapped_guest',
+        'issues',
+    ]
+
+    nics_headers = [
+        'vm',
+        'backing',
+        'network',
+        'address_type',
+        'key',
+        'mac',
+        'guests_ipv4',
+        'guests_ipv6',
+        'guests_network_name',
+    ]
+    
+    with (out_table(out, title='vm_nics', headers=nics_headers, dir=vcenter.out_dir, env=vcenter.env) as t_nics,
+          out_table(out, title='vm_nics_per_vm', headers=nics_per_vm_headers, dir=vcenter.out_dir, env=vcenter.env) as t_nics_per_vm):
+        
+        for i, vm in enumerate(vcenter.iter_objs(vim.VirtualMachine, search, normalize=normalize, key=key)):
+            if top is not None and i == top:
+                break
+            
+            try:
+                logger.info(f"Analyze vm {vm.name} nics")
+
+                info = extract_nics(vm, vcenter=vcenter)
+
+                mapped_guests: list[vim.vm.GuestInfo.NicInfo] = []
+                if info is not None:
+                    for nic in info.nics:
+                        for guest in nic.guests:
+                            mapped_guests.append(guest)
+
+                t_nics_per_vm.append([
+                    vm.name, # vm
+                    len(info.nics) if info is not None else None, # 'device_networks',
+                    len(mapped_guests) + len(info.unmapped_guests) if info is not None else None, # 'guest_networks',
+                    len(mapped_guests) if info is not None else None, # 'with_mappings',
+                    len(info.unmapped_guests) if info is not None else None, # 'without_mappings',
+                    [guest.macAddress for guest in mapped_guests] if info is not None else None, # 'mapped_guest',
+                    [guest.macAddress for guest in info.unmapped_guests] if info is not None else None, # 'unmapped_guests',
+                    info.issues if info is not None else None,
+                ])
+
+                if info is not None:
+                    for nic in info.nics:
+                        backing_typename = type(nic.device.backing).__name__
+                        if backing_typename.startswith('vim.vm.device.VirtualEthernetCard.'):
+                            backing_typename = backing_typename[len('vim.vm.device.VirtualEthernetCard.'):]
+
+                        if isinstance(nic.device.backing, vim.vm.device.VirtualEthernetCard.DistributedVirtualPortBackingInfo):
+                            connection_obj = nic.device.backing.port
+                            network_obj = vcenter.get_portgroup_by_key(connection_obj.portgroupKey)
+                            if network_obj:
+                                network = network_obj.name
+                            else:
+                                switch_obj = vcenter.get_switch_by_uuid(connection_obj.switchUuid)
+                                if switch_obj:
+                                    network = f"Switch {switch_obj.name} (port {connection_obj.portKey})"
+                                else:
+                                    network = f"Switch {connection_obj.switchUuid} (port {connection_obj.portKey})"
+                        elif isinstance(nic.device.backing, vim.vm.device.VirtualEthernetCard.NetworkBackingInfo):
+                            network_obj = nic.device.backing.network
+                            network = network_obj.name
+                        else:
+                            network = None
+
+                        ipv4 = []
+                        ipv6 = []
+                        networks = []
+                        for guest in nic.guests:
+                            for ip in guest.ipAddress:
+                                ip = ip_address(ip)
+                                if ip.version == 4:
+                                    ipv4.append(ip)
+                                else:
+                                    ipv6.append(ip)
+                            networks.append(guest.network)
+                        
+                        t_nics.append([
+                            vm.name, # vm
+                            backing_typename, # backing
+                            network,
+                            nic.device.addressType, # address_type
+                            nic.device.key, # key
+                            nic.device.macAddress.lower(), # mac
+                            ipv4,
+                            ipv6,
+                            networks,
+                        ])
+
+                    for guest in info.unmapped_guests:
+                        ipv4 = []
+                        ipv6 = []
+                        for ip in guest.ipAddress:
+                            ip = ip_address(ip)
+                            if ip.version == 4:
+                                ipv4.append(ip)
+                            else:
+                                ipv6.append(ip)
+
+                        t_nics.append([
+                            vm.name, # vm
+                            None, # backing
+                            None, # network
+                            None, # address_type
+                            guest.deviceConfigId, # key
+                            guest.macAddress.lower(), # mac
+                            ipv4,
+                            ipv6,
+                            guest.network,
+                        ])
+
+            except Exception as err:
+                logger.exception(f"Error while analyzing {str(vm)} nics: {err}")
+
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('search', nargs='*', help="Search term(s).")
+    parser.add_argument('-n', '--normalize', action='store_true', help="Normalise search term(s).")
+    parser.add_argument('-k', '--key', choices=['name', 'ref'], default='name', help="Search key (default: %(default)s).")
+    parser.add_argument('--top', type=int)
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output Excel or CSV file (default: %(default)s).")
+
+list_vm_nics.add_arguments = _add_arguments
+
+
+def extract_nics(vm: vim.VirtualMachine, *, vcenter: VCenterClient):
+    if vm.config is None:
+        # VM is not yet configured
+        return None
+    
+    info = VmNics(vm)
+
+    # Retrieve nic devices
+    nics_per_key: dict[int,VmNic] = {}
+    keys_to_ignore = set()
+    for obj in vm.config.hardware.device:
+        if not isinstance(obj, vim.vm.device.VirtualEthernetCard):
+            continue
+
+        nic = VmNic(obj, vcenter=vcenter)
+        info.nics.append(nic)
+
+        if obj.key is None:
+            info._append_issue(f"Device NIC has no key: {obj}")
+        elif not isinstance(obj.key, int):
+            info._append_issue(f"Device NIC has a non-int key: {obj}")
+        elif obj.key in nics_per_key:
+            info._append_issue(f"Several NIC have key {obj.key}")
+            keys_to_ignore.add(obj.key)
+        else:
+            nics_per_key[obj.key] = nic
+
+    for key in keys_to_ignore:
+        del nics_per_key[key]
+
+    # Retrieve guest NICs
+    # Associate them to device NICs if a consistent mapping is provided
+    for obj in vm.guest.net:
+        if obj.deviceConfigId and obj.deviceConfigId != -1:
+            nic = nics_per_key.get(obj.deviceConfigId)
+            if not nic:
+                info._append_issue(f"Guest NIC {obj.macAddress} mapped to unknown device NIC key: {obj.deviceConfigId}")
+                info.unmapped_guests.append(obj)
+            else:
+                nic.guests.append(obj)
+        else:
+            info.unmapped_guests.append(obj)
+
+    # Verify consistency of mapped guests address MACs
+    for nic in info.nics:
+        for guest in nic.guests:
+            if guest.macAddress.lower() != nic.device.macAddress.lower():
+                info._append_issue(f"Inconsistent MAC address ({guest.macAddress.lower()}) for guest {guest.ipAddress} (device {nic.device.key} MAC address: {nic.device.macAddress.lower()})")
+
+    return info
+
+
+class VmNics:
+    def __init__(self, vm: vim.VirtualMachine):
+        self.vm = vm
+        self.nics: list[VmNic] = []
+        self.unmapped_guests: list[vim.vm.GuestInfo.NicInfo] = []
+        self.issues: list[str] = []
+
+    def _append_issue(self, message: str):
+        logger.warning(f"{self.vm.name}: {message}")
+        self.issues.append(message)
+
+    @property
+    def guests(self):
+        for nic in self.nics:
+            for guest in nic.guests:
+                yield guest
+
+        for guest in self.unmapped_guests:
+            yield guest
+
+    @property
+    def network_names(self):
+        names = set()
+
+        for nic in self.nics:
+            name = nic.network_name
+            if name:
+                names.add(name)
+
+        return sorted(names)      
+    
+    def to_dict(self):
+        data = []
+
+        for nic in self.nics:
+            data.append(nic.to_dict())
+
+        if self.unmapped_guests:
+            for guest in self.unmapped_guests:
+                data.append({'key': guest.deviceConfigId, 'mac': guest.macAddress.lower(), 'guest':  self._get_guest_dict(guest)})
+
+        return data
+    
+    def to_summary(self, ip_version: int = None):
+        result = ''
+        
+        for nic in self.nics:
+            result += (' | ' if result else '') + nic.to_summary(ip_version=ip_version)
+
+        if self.unmapped_guests:
+            for guest in self.unmapped_guests:
+                result += (' | ' if result else '') + f"unmapped {guest.macAddress.lower()}: {guest.network} (" + VmNics._get_guest_summary(guest, ip_version=ip_version) + ")"
+
+        return result
+    
+    @classmethod
+    def _get_guest_dict(cls, guest: vim.vm.GuestInfo.NicInfo):
+        data = {}
+        data['ips'] = guest.ipAddress
+        data['connected'] = guest.connected
+        data['network_name'] = guest.network
+        return data
+    
+    @classmethod
+    def _get_guest_summary(cls, guest: vim.vm.GuestInfo.NicInfo, ip_version: int = None):        
+        ip_addresses: list[IPv4Address|IPv6Address] = []
+        for ip_str in guest.ipAddress:
+            ip = ip_address(ip_str)
+            if ip_version is None or ip.version == ip_version:
+                ip_addresses.append(ip)
+
+        ip_addresses.sort()
+                
+        result = ''
+        for ip in ip_addresses:
+            result += (', ' if result else '') + ip.compressed
+        result += (', ' if result else '') + ('connected' if guest.connected else 'notConnected')
+        return result
+
+
+class VmNic:
+    def __init__(self, device: vim.vm.device.VirtualEthernetCard, *, vcenter: VCenterClient):
+        self.vcenter = vcenter
+        self.device = device
+        self.guests: list[vim.vm.GuestInfo.NicInfo] = []
+
+    @property
+    def network(self):
+        if isinstance(self.device.backing, vim.vm.device.VirtualEthernetCard.DistributedVirtualPortBackingInfo):
+            connection_obj = self.device.backing.port
+            network_obj = self.vcenter.get_portgroup_by_key(connection_obj.portgroupKey)
+            if network_obj:
+                return network_obj
+            else:
+                switch_obj = self.vcenter.get_switch_by_uuid(connection_obj.switchUuid)
+                port_key = int(connection_obj.portKey) if connection_obj.portKey is not None and re.match(r'^\d+$', connection_obj.portKey) else connection_obj.portKey
+                if switch_obj:
+                    return {'switch': switch_obj, 'port': port_key}
+                else:
+                    return {'switch_uuid': connection_obj.switchUuid, 'port': port_key}
+        elif isinstance(self.device.backing, vim.vm.device.VirtualEthernetCard.NetworkBackingInfo):
+            return self.device.backing.network
+        else:
+            return None
+        
+    @property
+    def network_name(self):
+        network = self.network
+        if not network:
+            return None
+        elif isinstance(network, (vim.dvs.DistributedVirtualPortgroup, vim.Network)):
+            return network.name
+        elif isinstance(network, dict):
+            result = ''
+            for key, value in network.items():
+                if isinstance(value, vim.ManagedEntity):
+                    value = value.name
+                result += (', ' if result else '') + f"{key}: {value}"
+            return str(network)
+        else:
+            return str(network)
+
+    def to_dict(self):
+        data = {}
+        data['key'] = self.device.key
+        data['mac'] = self.device.macAddress.lower()
+
+        # vim.vm.device.VirtualEthernetCard.NetworkBackingInfo, vim.vm.device.VirtualEthernetCard.DistributedVirtualPortBackingInfo, etc
+        backing_typename = type(self.device.backing).__name__
+        if backing_typename.startswith('vim.vm.device.VirtualEthernetCard.'):
+            backing_typename = backing_typename[len('vim.vm.device.VirtualEthernetCard.'):]
+        data['backing'] = backing_typename
+
+        if network := self.network:
+            if isinstance(network, dict) and 'switch' in dict:
+                network['switch'] = {'name': network['switch'].name, 'ref': get_obj_ref(network['switch'])}
+            else:
+                network = {'name': network.name, 'ref': get_obj_ref(network)}
+            data['network'] = network
+
+        data['address_type'] = self.device.addressType
+
+        if self.guests:
+            data['guests'] = [VmNics._get_guest_dict(guest) for guest in self.guests]
+        
+        return data
+    
+    def to_summary(self, ip_version: int = None):
+        result = f"{self.device.macAddress.lower()}: {self.network_name}"
+        if self.guests:
+            result += " ("
+            for i, guest in enumerate(self.guests):
+                if i > 0:
+                    result += ', '
+                result += VmNics._get_guest_summary(guest, ip_version=ip_version)
+            result += ")"
+        return result
+
+#endregion
+
+
+def get_tools_version_number(toolsversion: str):
+    if toolsversion is None:
+        return None
+    elif re.match(r'^\d+$', toolsversion):
+        toolsversion = int(toolsversion)
+        if toolsversion == 0 or toolsversion == 2147483647:
+            return None
+        return toolsversion    
+    elif toolsversion:
+        return str(toolsversion)
+    else:
+        return None
+
+
+def get_os_family(extra_config: dict, configured_fullname: str):
+    def get_family_from_configured(fullname: str):
+        if m := re.match(r'^(.+) \(\d\d\-bit\)$', fullname):
+            fullname = m[1]
+            
+        lower_fullname = fullname.lower()
+        if 'windows' in lower_fullname:
+            return "Windows"
+        elif 'linux' in lower_fullname or 'centos' in lower_fullname:
+            return "Linux"
+        elif lower_fullname == 'other':
+            return None
+        else:
+            return fullname
+      
+    if 'guestInfo.detailed.data' in extra_config:
+        line = extra_config['guestInfo.detailed.data']
+        if m := re.match(r".*familyName='([^']+)'.*", line):
+            return m[1]
+    elif 'guestOS.detailed.data' in extra_config:
+        data = extra_config.get("guestOS.detailed.data")
+        if isinstance(data, dict) and 'familyName' in data:
+            return data['familyName']
+
+    if configured_fullname:
+        return get_family_from_configured(configured_fullname)
+
+
+
+def get_os_version(extra_config: dict):
+    if 'guestInfo.detailed.data' in extra_config:
+        line = extra_config['guestInfo.detailed.data']
+        if m := re.match(r".*prettyName='([^']+)'.*", line):
+            return m[1]
+        else:
+            return line
+    elif 'guestOS.detailed.data' in extra_config:
+        data = extra_config.get("guestOS.detailed.data")
+        if isinstance(data, dict) and 'prettyName' in data:
+            return data['prettyName']
+        else:
+            return str(data)
+    else:
+        return None
+
+
+def get_os_distro_version(extra_config: dict):
+    if 'guestInfo.detailed.data' in extra_config:
+        line = extra_config['guestInfo.detailed.data']
+        if m := re.match(r".*distroVersion='([^']+)'.*", line):
+            return m[1]
+    if 'guestOS.detailed.data' in extra_config:
+        data = extra_config.get("guestOS.detailed.data")
+        if isinstance(data, dict) and 'distroVersion' in data:
+            return data['distroVersion']
+
+
+def get_os_kernel_version(extra_config: dict):
+    if 'guestInfo.detailed.data' in extra_config:
+        line = extra_config['guestInfo.detailed.data']
+        if m := re.match(r".*kernelVersion='([^']+)'.*", line):
+            return m[1]
+    if 'guestOS.detailed.data' in extra_config:
+        data = extra_config.get("guestOS.detailed.data")
+        if isinstance(data, dict) and 'kernelVersion' in data:
+            return data['kernelVersion']
+        
+
+def get_guestinfo_publish_time(extra_config: dict):
+    if not 'guestinfo.appInfo' in extra_config:
+        return
+    
+    appinfo_str = extra_config['guestinfo.appInfo']
+    if not isinstance(appinfo_str, str):
+        return str(appinfo_str)
+    
+    if appinfo_str == "":
+        return
+    
+    try:
+        appinfo = json.loads(appinfo_str)
+    except json.decoder.JSONDecodeError as err:
+        return f"Cannot parse \"{appinfo_str}\": {err}"
+
+    if 'publishTime' in appinfo:
+        return datetime.fromisoformat(appinfo['publishTime'])
+
+
+def get_tools_version(extra_config: dict, version_number: str):
+    if 'guestinfo.vmtools.versionNumber' in extra_config and 'guestinfo.vmtools.description' in extra_config:
+        if extra_config['guestinfo.vmtools.versionNumber'] == version_number:
+            return extra_config['guestinfo.vmtools.description']
+
+
+def get_custom_values(vm: vim.VirtualMachine):
+    available_fields = {}
+    custom_values = {}
+
+    for field in vm.availableField:
+        available_fields[field.key] = field.name
+
+    for value in vm.value:
+        custom_values[available_fields[value.key]] = value.value
+        
+    for value in vm.customValue:
+        custom_values[available_fields[value.key]] = value.value
+
+    return custom_values
```

## Comparing `vmware_reporter/customfield.py` & `vmware_reporter/customvalue.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-import os
-from argparse import ArgumentParser
-from io import IOBase
-
-from zut import out_table
-
-from . import VCenterClient
-
-_DEFAULT_OUT = 'stdout'
-
-def list_customfields(vcenter: VCenterClient, out: os.PathLike|IOBase = _DEFAULT_OUT):
-    """
-    Export custom fields.
-    """
-    headers=['name', 'key', 'obj_type', 'data_type']
-
-    with out_table(out, title="customfields", dir=vcenter.get_out_dir(), env=vcenter.env, headers=headers) as t:
-        for field in vcenter.service_content.customFieldsManager.field:
-            t.append([field.name, field.key, field.managedObjectType.__name__, field.type.__name__])
-
-def _add_arguments(parser: ArgumentParser):
-    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output table (default: %(default)s).")
-
-list_customfields.add_arguments = _add_arguments
+"""
+List custom values defined on the system.
+"""
+import os
+from argparse import ArgumentParser
+from io import IOBase
+
+from zut import out_table
+
+from . import VCenterClient
+
+_DEFAULT_OUT = 'stdout'
+
+def list_custom_values(vcenter: VCenterClient, out: os.PathLike|IOBase = _DEFAULT_OUT):
+    """
+    Export custom fields.
+    """
+    headers=['name', 'key', 'obj_type', 'data_type']
+
+    with out_table(out, title="customvalues", dir=vcenter.out_dir, env=vcenter.env, headers=headers) as t:
+        for field in vcenter.service_content.customFieldsManager.field:
+            t.append([field.name, field.key, field.managedObjectType.__name__, field.type.__name__])
+
+def _add_arguments(parser: ArgumentParser):
+    parser.add_argument('-o', '--out', default=_DEFAULT_OUT, help="Output table (default: %(default)s).")
+
+list_custom_values.add_arguments = _add_arguments
```

## Comparing `vmware_reporter-0.3.0.dist-info/LICENSE.txt` & `vmware_reporter-0.3.1.dist-info/LICENSE.txt`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (C) 2024, Sébastien Hocquet <dev@ipamo.net>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (C) 2024, Sébastien Hocquet <dev@ipamo.net>
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

## Comparing `vmware_reporter-0.3.0.dist-info/RECORD` & `vmware_reporter-0.3.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-vmware_reporter/__init__.py,sha256=qRQcQQxnfr6UjXYaTAvd_JIIxrMA7Q8Re4u9BzpyKXI,31153
-vmware_reporter/__main__.py,sha256=KjoRljGbAPbNyWcMA2BdVcOo8b9Ne5lHr7iNK1La874,3466
-vmware_reporter/_version.py,sha256=MQTeK44Cj4PxMB5VTeNSrMxwkURTN6SjVTQLlqfFFH8,427
-vmware_reporter/autoreport.py,sha256=3zkwSC6gPgoj0oAQ7b0pTFV-zELIqVzsQ2NF4NTBhMU,1447
-vmware_reporter/customfield.py,sha256=JLvG3El-IGihWHbS7Rtj-FAG7BLj962RZ11W8pIbCls,844
-vmware_reporter/datastore.py,sha256=xR_Xn0uE35ZaEolkCg5epLJGmG003NjWjsv7Ffx6sUc,18826
-vmware_reporter/dump.py,sha256=eS_aYOO-ac0uuePdbjWp2tOaCrXvDB073lVmK040VsM,2547
-vmware_reporter/host.py,sha256=sz5Bq7A5vIMk-7cC0QpHzMm-hUZf29z8-VHG7Rnb_50,4034
-vmware_reporter/inventory.py,sha256=hYV5xryl1bbfb84qLCw_OmwYePkEl4Gjsm8VceZCXK4,7968
-vmware_reporter/net.py,sha256=w0iTS3u6mpGTZseK1eOokz1gx47kKI4XthHnvFyxZVY,5971
-vmware_reporter/settings.py,sha256=TDs4bXPO7nGg46nZHvNFJHsavQgQyuG7NBRgeJAWVtQ,235
-vmware_reporter/vm.py,sha256=1XdOhGHOr105v-2wWOLJAiDFlF2MQ8OIweKE8a3VCF0,54717
-vmware_reporter-0.3.0.dist-info/LICENSE.txt,sha256=GIOy7i81R9zaxGmerWRrvgsSukOj10VspxRwsEWtlCY,1098
-vmware_reporter-0.3.0.dist-info/METADATA,sha256=j8qBGUO0Z2Xkg0wafvMtU9KHZOAdyIcaH30zOOPxJIo,3435
-vmware_reporter-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-vmware_reporter-0.3.0.dist-info/entry_points.txt,sha256=Sd7R6PmUzLkJr4eez7nM8-z6yISX2pb3Dc8mnXDuguM,66
-vmware_reporter-0.3.0.dist-info/top_level.txt,sha256=uBrhSJjB5QxsyeQKqRdCv8l6JOmXKhnfPKnetEEAqso,16
-vmware_reporter-0.3.0.dist-info/RECORD,,
+vmware_reporter/__init__.py,sha256=Poe7Zv7LJ-ydS_-Y4M1HaKyVklY-L4hqUBRX6JmfCL0,36933
+vmware_reporter/__main__.py,sha256=_-NKG72nzdo-KJI8cglxBZ2OyZ6j_huzIT2mjEk_OiU,3757
+vmware_reporter/_version.py,sha256=HzPz9rq3s1AiZXregKlqKaJJ2wGMtvH_a3V9la9CnpM,411
+vmware_reporter/autoreport.py,sha256=7RA46S1AVh90a3-ICuzIF9NtOo8-kMYxHGXdkWKJyeM,1992
+vmware_reporter/cluster.py,sha256=WJbxIh8c0TOWi75brbF1Dy_WmT5lQtNnEYN26Es7_OY,3307
+vmware_reporter/customvalue.py,sha256=qR-aGfMdBwvELSRDTulrozobKVVW3C7GwAINfsfHNEY,866
+vmware_reporter/datastore.py,sha256=HeXJvT-FAydywyiye3J9HN_J-Zaw-Z2U9MDQBo7WZD4,18360
+vmware_reporter/dump.py,sha256=eBG_EaeLrDp2nq52N8N6jvDmqKGr-0aX0Tl5SOUlWU8,2520
+vmware_reporter/host.py,sha256=Z3RRmQS4t8RpO4Urjv53SAqvjzE2BlY9ZJ4a7o5ktbo,3991
+vmware_reporter/inventory.py,sha256=XMoFWB7yjuULTJV2m0xvBlVgYFuAKm3-dyv-fAW9JuI,8160
+vmware_reporter/net.py,sha256=1Y5DAmHqHmWUA3pd9xTrPfheumrSA1nszWMdH_ajPis,5792
+vmware_reporter/perf.py,sha256=Faf03FTM59GymtXpPndKx-ppayXP2t50WRQolEhtpAU,14413
+vmware_reporter/resourcepool.py,sha256=ddBO4G4vFnl-5X0DEgii7uyfvVaDpj4aBa6udCT27Jk,3255
+vmware_reporter/settings.py,sha256=hJpZqYcmLviCCqu_lu9UPPS365rMkmVwO3fG9QWMCqk,229
+vmware_reporter/tag.py,sha256=IU1pqd9RorpnXpdNIrdb37UqxHR6O8RFDMh5xp8he44,2410
+vmware_reporter/vm.py,sha256=SDr1V35UjMx_kO3W0UyfSE0-N-5_1QaGU0eSFDj961Y,60990
+vmware_reporter-0.3.1.dist-info/LICENSE.txt,sha256=IpfXMCFhyEtTBZwZrQWjWyoXj1WE9ht2Yn9GxdxdNr4,1079
+vmware_reporter-0.3.1.dist-info/METADATA,sha256=O_5jBP-cYcMsqAJlLCHLao4U4A4nkvUKhxWDfckd5zk,4147
+vmware_reporter-0.3.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+vmware_reporter-0.3.1.dist-info/entry_points.txt,sha256=Sd7R6PmUzLkJr4eez7nM8-z6yISX2pb3Dc8mnXDuguM,66
+vmware_reporter-0.3.1.dist-info/top_level.txt,sha256=uBrhSJjB5QxsyeQKqRdCv8l6JOmXKhnfPKnetEEAqso,16
+vmware_reporter-0.3.1.dist-info/RECORD,,
```

