# Comparing `tmp/fabricplus-0.1.0.tar.gz` & `tmp/fabricplus-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabricplus-0.1.0.tar", max compression
+gzip compressed data, was "fabricplus-1.0.0.tar", max compression
```

## Comparing `fabricplus-0.1.0.tar` & `fabricplus-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2024-05-17 15:43:25.164496 fabricplus-0.1.0/LICENSE
--rw-r--r--   0        0        0     9625 2024-05-22 18:44:23.510894 fabricplus-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-17 15:43:25.164738 fabricplus-0.1.0/fabricplus/__init__.py
--rw-r--r--   0        0        0    17195 2024-05-22 18:23:02.176353 fabricplus-0.1.0/fabricplus/connection.py
--rw-r--r--   0        0        0        0 2024-05-17 16:42:43.780850 fabricplus-0.1.0/fabricplus/paramiko_modifications/__init__.py
--rw-r--r--   0        0        0    13644 2024-05-22 18:39:43.400152 fabricplus-0.1.0/fabricplus/paramiko_modifications/client.py
--rw-r--r--   0        0        0        0 2024-05-20 15:20:04.799917 fabricplus-0.1.0/fabricplus/py.typed
--rw-r--r--   0        0        0     2463 2024-05-22 18:23:27.098201 fabricplus-0.1.0/fabricplus/transfer.py
--rw-r--r--   0        0        0     1426 2024-05-22 19:23:06.426897 fabricplus-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10945 1970-01-01 00:00:00.000000 fabricplus-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-28 19:30:11.913711 fabricplus-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3669 2024-05-28 19:30:11.913711 fabricplus-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 19:30:11.921711 fabricplus-1.0.0/fabricplus/__init__.py
+-rw-r--r--   0        0        0    17737 2024-05-28 19:30:11.921711 fabricplus-1.0.0/fabricplus/connection.py
+-rw-r--r--   0        0        0        0 2024-05-28 19:30:11.921711 fabricplus-1.0.0/fabricplus/paramiko_modifications/__init__.py
+-rw-r--r--   0        0        0    13458 2024-05-28 19:30:11.921711 fabricplus-1.0.0/fabricplus/paramiko_modifications/client.py
+-rw-r--r--   0        0        0        0 2024-05-28 19:30:11.921711 fabricplus-1.0.0/fabricplus/py.typed
+-rw-r--r--   0        0        0     2430 2024-05-28 19:30:11.921711 fabricplus-1.0.0/fabricplus/transfer.py
+-rw-r--r--   0        0        0     1591 2024-05-28 19:30:11.921711 fabricplus-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4991 1970-01-01 00:00:00.000000 fabricplus-1.0.0/PKG-INFO
```

### Comparing `fabricplus-0.1.0/LICENSE` & `fabricplus-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fabricplus-0.1.0/fabricplus/connection.py` & `fabricplus-1.0.0/fabricplus/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 # External Imports
 from fabric.connection import Connection, opens
 import fabric.transfer
 import re
 from invoke.watchers import FailingResponder, Responder
 from paramiko import WarningPolicy, SSHClient, Transport
+from invoke.runners import Result
 
 from scp import SCPClient
 from invoke.exceptions import Failure, ResponseNotAccepted, AuthFailure
 
 # Internal Imports
 from fabricplus.transfer import TransferPlus
 from fabricplus.paramiko_modifications.client import SSHJumpClient, simple_auth_handler
 
 # Typing Imports
 from typing import Optional, Union, Callable, List, Any, AnyStr, TYPE_CHECKING, TypeVar
 from paramiko.channel import ChannelFile, ChannelStderrFile
+
 if TYPE_CHECKING:
-    from invoke.runners import Runner, Result
+    from invoke.runners import Runner  # pragma: no cover
 
 # Type Variable For Connection-Like objects
 Conn = TypeVar("Conn", bound=Connection, covariant=True)
 # Type Variable For SSHClient-Like objects
 Client = Union[SSHJumpClient, SSHClient]
 
+
 class ConnectionPlus(Connection):
     """ConnectionPlus is a subclass of the Connection object from the Fabric library.
-    
+
     This subclass provides additional functionality to the Connection object, such as SCP transfers,
-    running commands as another user, and running commands on a jumphost, as well as connecting to 
+    running commands as another user, and running commands on a jumphost, as well as connecting to
     a host through a jumphost.
     """
-    def __init__(self,
-                 *args,
-                 jumphost_target: Optional[Union[Client, str, Conn]] = None,
-                 scp: bool = False,
-                 jump_uname: Optional[str] = None,
-                 jump_port: Optional[int] = None,
-                 **kwargs):
+
+    def __init__(
+        self,
+        *args,
+        jumphost_target: Optional[Union[Client, str, Conn]] = None,
+        scp: Optional[bool] = None,
+        jump_uname: Optional[str] = None,
+        jump_port: Optional[int] = None,
+        **kwargs,
+    ):
         """Initialize the ConnectionPlus object.
-        
+
         Initializes using the Connection initialization, but also sets up the client object
         for the ConnectionPlus object via a jumphost target.
-        
+
         See the Connection object documentation for additional arguments.
-        
+
         :param args: Additional arguments to pass to the Connection object.
-        :param jumphost_target: 
+        :param jumphost_target:
             Jumphost to connect to the host through.
             Can be an instance of SSHJumpClient, SSHClient, URL/IP string,
             or Connection/ConnectionPlus.
             Defaults to None.
         :param scp:
             Boolean value to define if the ConnectionPlus object should
             use SCP for file transfers.
@@ -61,74 +67,92 @@
             Port for the jumphost if different than the default SSH_PORT.
             Defaults to None.
         :param kwargs:
             Additional keyword arguments to pass to the Connection object.
         """
         super().__init__(*args, **kwargs)
         self._scp: Optional[SCPClient] = None
-        self.__scp: bool = scp
-        self.client: Optional[Client] = self.__client_setup(jumphost_target=jumphost_target,
-                                          jump_uname=jump_uname,
-                                          jump_port=jump_port)
+        self.__scp: Optional[bool] = scp
+        self.client: Optional[Client] = self.__client_setup(
+            jumphost_target=jumphost_target, jump_uname=jump_uname, jump_port=jump_port
+        )
         if self.client is None:
-            raise AttributeError("The ConnectionPlus object could not initialize it's client.")
+            raise AttributeError(
+                "The ConnectionPlus object could not initialize it's client."
+            )
         self.client.set_missing_host_key_policy(WarningPolicy())
         self.client.load_system_host_keys()
-    
-    def su(self,
-           command: str,
-           user: str,
-           password:Optional[str] = None,
-           timeout: int = 10,
-           **kwargs: Any) -> Optional["Result"]:
+
+    def su(
+        self,
+        command: str,
+        user: str,
+        password: Optional[str] = None,
+        timeout: int = 10,
+        **kwargs: Any,
+    ) -> Optional["Result"]:
         """Run a command as another user, via su.
-        
+
         Requires the target user's password be given, either directly, or via the ConnectionPlus object.
-        
+
         Note: This method doesn't work on Windows, as Windows doesn't have su, nor does it work in parallel on
         some systems due to the way su is implemented (e.g. it may require a tty).
 
         :param command: Command to run in su.
         :param user: User to run the command as.
         :param password: Password for the target user. Needed, but defaults to None.
         :param timeout: Timeout for the command. Defaults to 10.
         :param kwargs: Additional keyword arguments to pass to the command execution.
         :raises ValueError: If the password is not given.
         :return: Result object from the command execution.
         :rtype: Optional[Result]
         """
         _password: str = password or self.connect_kwargs.get("password", None)
         if _password is None:
-            raise ValueError("The password must be given to run a command as another user.")
-        return self._su(runner=self._remote_runner(), command=command, user=user, password=_password, timeout=timeout, pty=True, **kwargs)
-    
-    def _su(self,
-            runner: "Runner",
-            command: str,
-            user: str,
-            password: Optional[str] = None,
-            timeout: int = 10,
-            **kwargs: Any) -> Optional["Result"]:
+            raise ValueError(
+                "The password must be given to run a command as another user."
+            )
+        return self._su(
+            runner=self._remote_runner(),
+            command=command,
+            user=user,
+            password=_password,
+            timeout=timeout,
+            pty=True,
+            **kwargs,
+        )
+
+    def _su(
+        self,
+        runner: "Runner",
+        command: str,
+        user: str,
+        password: Optional[str] = None,
+        timeout: int = 10,
+        **kwargs: Any,
+    ) -> Optional["Result"]:
         """Internal representation to run a command as another user, via su.
-        
+
         :param runner: The runner object to run the command.
         :param command: Command to run in su.
         :param user: User to run the command as.
         :param password: Password for the target user. Needed, but defaults to None.
         :param timeout: Timeout for the command. Defaults to 10.
         :param kwargs: Additional keyword arguments to pass to the command execution.
         :raises AuthFailure: If the authentication fails.
         :raises failure: If the command execution fails.
         :return: Result object from the command execution.
         :rtype: Optional[Result]
         """
         _prompt: str = "Password: "
         _command: str = self._prefix_commands(command)
         # Escape all double quotes in the command.
-        _cmd_str: str  = f'su - {user} -Conn "{command}"'.format(user=user, command=_command.replace('"', '\\"'))
+        _cmd_str: str = f'su - {user} -Conn "{command}"'.format(
+            user=user, command=_command.replace('"', '\\"')
+        )
         _watcher: FailingResponder = FailingResponder(
             pattern=re.escape(_prompt),
             response="{password}\n".format(password=password),
             sentinel="Sorry, try again.\n",
         )
         watchers: List[Union[FailingResponder, Responder]] = kwargs.pop("watchers", [])
         watchers.append(_watcher)
@@ -136,28 +160,27 @@
             return runner.run(_cmd_str, timeout=timeout, watchers=watchers, **kwargs)
         except Failure as failure:
             if isinstance(failure.reason, ResponseNotAccepted):
                 raise AuthFailure(result=failure.result, prompt=_prompt)
             else:
                 raise failure
 
-    def __client_connect(self,
-                         client: Client,
-                         username: Optional[str] = None,
-                         port: Optional[int] = None) -> None:
+    def __client_connect(
+        self, client: Client, username: Optional[str] = None, port: Optional[int] = None
+    ) -> None:
         """Connect the client object for the ConnectionPlus object.
-        
+
         Helps pass in the connect arguments from the Connection object.
-        
+
         These include some loaded from SSH Config.
-        
+
         :param client: The client object to connect.
         :param username: Username to connect with. Defaults to None.
         :param port: Port to connect with. Defaults to None.
-        """        
+        """
         # Ensure dict-ness
         if self.connect_kwargs is None:
             self.connect_kwargs: dict[str, Any] = {}
         # Short-circuit
         if self.is_connected:
             return
         err = "Refusing to be ambiguous: connect() kwarg '{}' was given both via regular arg and via connect_kwargs!"  # noqa
@@ -166,27 +189,25 @@
             hostname
             port
             username
         """.split():
             if key in self.connect_kwargs:
                 raise ValueError(err.format(key))
         # These may be given one way or the other, but not both
-        if (
-            "timeout" in self.connect_kwargs
-            and self.connect_timeout is not None
-        ):
+        if "timeout" in self.connect_kwargs and self.connect_timeout is not None:
             raise ValueError(err.format("timeout"))
         # No conflicts -> merge 'em together
         kwarg_updates: dict[str, Any] = {
             "hostname": self.host,
-            "port":port or self.port,
+            "port": port or self.port,
             "username": username or self.user,
         }
-        kwargs: dict[str, Any] = (self.connect_kwargs.copy() if self.connect_kwargs
-                                 else kwarg_updates)
+        kwargs: dict[str, Any] = (
+            self.connect_kwargs.copy() if self.connect_kwargs else kwarg_updates
+        )
         kwargs.update(kwarg_updates)
         if self.gateway:
             kwargs["sock"] = self.open_gateway()
         if self.connect_timeout:
             kwargs["timeout"] = self.connect_timeout
         # Strip out empty defaults for less noisy debugging
         if "key_filename" in kwargs and not kwargs["key_filename"]:
@@ -209,152 +230,187 @@
             kwargs["auth_strategy"] = auth_strategy_class(
                 ssh_config=self.ssh_config,
                 fabric_config=self.config,
                 username=username or self.user,
             )
         client.connect(**kwargs)
         return None
-        
-    
-    def __client_setup(self,
-                         *args,
-                         jumphost_target: Optional[Union[Client, str, Conn]] = None,
-                         interactive_prompt: bool = False,
-                         jump_uname: Optional[str] = None,
-                         jump_port: Optional[int] = None,
-                         **kwargs) -> Optional[Client]:
+
+    def __client_setup(
+        self,
+        *args,
+        jumphost_target: Optional[Union[Client, str, Conn]] = None,
+        interactive_prompt: bool = False,
+        jump_uname: Optional[str] = None,
+        jump_port: Optional[int] = None,
+        **kwargs,
+    ) -> Optional[Client]:
         """Setup the client object for the ConnectionPlus object.
-        
+
         This method can be used to setup the client object for the ConnectionPlus object.
         But it also can be used to setup the jumphost for the ConnectionPlus object.
-        
+
         :param jumphost_target: Jumphost to run all actions through for this client. Defaults to None.
         :param interactive_prompt: Whether to use an interactive method for the jumphost connectivity. Defaults to False.
         :param jump_uname: Username for jumphost if different than connection. Defaults to None.
         :param jump_port: Port for the jumphost if different than default SSH_PORT. Defaults to None.
         :raises TypeError: If the jumphost_target is not an instance of SSHJumpClient, SSHClient, URL/IP string, or Connection/ConnectionPlus.
         :return: The SSHClient object for the ConnectionPlus object.
         :rtype: Union[SSHClient/SSHJumpClient]
         """
         _client: Optional[Client] = None
-        _auth_handler: Optional[Callable[..., List[Any]]] = simple_auth_handler if interactive_prompt else None
+        _auth_handler: Optional[Callable[..., List[Any]]] = (
+            simple_auth_handler if interactive_prompt else None
+        )
         if jumphost_target is not None:
             if isinstance(jumphost_target, SSHJumpClient):
                 _client = jumphost_target
             elif isinstance(jumphost_target, SSHClient):
                 _client = jumphost_target
             elif isinstance(jumphost_target, str):
                 _client = SSHJumpClient(auth_handler=_auth_handler)
                 _client.set_missing_host_key_policy(WarningPolicy())
                 _client.load_system_host_keys()
-                self.__client_connect(_client, username=jump_uname or self.user, port=jump_port)
-            elif isinstance(jumphost_target, Connection) or isinstance(jumphost_target, ConnectionPlus):
+                self.__client_connect(
+                    _client, username=jump_uname or self.user, port=jump_port
+                )
+            elif isinstance(jumphost_target, Connection) or isinstance(
+                jumphost_target, ConnectionPlus
+            ):
                 if jumphost_target.client is None:
                     jumphost_target.open()
                 _client = jumphost_target.client
             else:
-                raise TypeError("The jumphost_target must be an instance of SSHJumpClient, SSHClient, URL/IP string, or Connection/ConnectionPlus.")
-        return SSHJumpClient(*args, jump_session=_client, auth_handler=_auth_handler, **kwargs)
-    
+                raise TypeError(
+                    "The jumphost_target must be an instance of SSHJumpClient, SSHClient, URL/IP string, or Connection/ConnectionPlus."
+                )
+        return SSHJumpClient(
+            *args, jump_session=_client, auth_handler=_auth_handler, **kwargs
+        )
+
     @property
     def jump_client(self) -> Optional[Client]:
         """
         Get the jump client object for the ConnectionPlus object.
-        
+
         :return: The jump client object for the ConnectionPlus object.
         :rtype: Optional[SSHJumpClient]
         """
         if self.client is None:
-            raise AttributeError("The ConnectionPlus object does not have a client initialized.")
-        return self.client._jump_session if isinstance(self.client, SSHJumpClient) else None
-        
+            raise AttributeError(
+                "The ConnectionPlus object does not have a client initialized."
+            )
+        return (
+            self.client._jump_session
+            if isinstance(self.client, SSHJumpClient)
+            else None
+        )
+
     def jump_run(self, command: str, timeout: int = 10, **kwargs) -> Optional["Result"]:
         """Run a command on the jumphost.
-        
+
         :param command: Command to run on the jumphost.
         :param timeout: Timeout for the command. Defaults to 10.
         :param kwargs: Additional keyword arguments to pass to the command execution.
         :raises AttributeError: If the ConnectionPlus object does not have a jump client initialized.
         :return: Result object from the command execution.
         :rtype: Optional[Result]
         """
         if self.jump_client is None:
-            raise AttributeError("The ConnectionPlus object does not have a jump client initialized.")
+            raise AttributeError(
+                "The ConnectionPlus object does not have a jump client initialized."
+            )
         try:
             _timeout: int = kwargs.pop("timeout", timeout)
             # typehints for exec_command aren't porting over, so do them here
             # See: PEP-0526 for more information
             _stderr: ChannelStderrFile
             _stdout: ChannelFile
-            _, _stdout, _stderr = self.jump_client.exec_command(command, timeout=_timeout, **kwargs) or (None, None, None)
+            _, _stdout, _stderr = self.jump_client.exec_command(
+                command, timeout=_timeout, **kwargs
+            ) or (None, None, None)
             _stderr_str: str = _stderr.read().decode("utf-8").strip("\n")
             _stdout_str: str = _stdout.read().decode("utf-8").strip("\n")
-            return Result(stdout=_stdout_str, stderr=_stderr_str, exited=0, encoding="utf-8", command=command)
+            return Result(
+                stdout=_stdout_str,
+                stderr=_stderr_str,
+                exited=0,
+                encoding="utf-8",
+                command=command,
+            )
         except Exception as e:
-            return Result(stdout="", stderr=str(e), exited=1, encoding="utf-8", command=command)
-        
-        
-    
+            return Result(
+                stdout="", stderr=str(e), exited=1, encoding="utf-8", command=command
+            )
+
     @opens
     def scp(self) -> SCPClient:
         """Get the SCP client object for the ConnectionPlus object.
-        
+
         Will open an SCP client object if one is not already open.
 
         :raises AttributeError: If the base fabric Connection object does not have an SSH client initialized.
         :raises AttributeError: If the base fabric Connection object does not have an SCP client initialized.
         :raises AttributeError: If the ConnectionPlus object could not initialize it's client.
         :return: The SCP client object for the ConnectionPlus object.
         :rtype: SCPClient
         """
         if self._scp is None:
             try:
                 self.open()
                 if self.client is None:
-                        raise AttributeError("The ConnectionPlus object could"
-                                             " not initialize it's client.")
+                    raise AttributeError(
+                        "The ConnectionPlus object could" " not initialize it's client."
+                    )
                 transport: Optional[Transport] = self.client.get_transport()
                 if transport is None:
-                    raise AttributeError("The ConnectionPlus object could"
-                                         " not initialize it's transport.")
+                    raise AttributeError(
+                        "The ConnectionPlus object could"
+                        " not initialize it's transport."
+                    )
                 self._scp = SCPClient(transport)
             except AttributeError:
-                raise AttributeError("The base fabric Connection object does "
-                                     "not have a client initialized.")
+                raise AttributeError(
+                    "The base fabric Connection object does "
+                    "not have a client initialized."
+                )
         return self._scp
 
     def get(self, *args, **kwargs) -> Optional[fabric.transfer.Result]:
         """Get a file from the remote host.
-        
+
         :param remote_path: The path to the file on the remote host.
         :param local_path: The path to save the file locally. Defaults to current working dir.
         :param scp: If the transfer should be done via SCP. Defaults to False or the Connection value.
         :param recursive: If the transfer should be recursive. Defaults to False.
         :param preserve_times: If the file times should be preserved. Defaults to False.
         :return: Result object from the transfer, or None.
         :rtype: Optional[fabric.transfer.Result]
         """
-        _scp: bool = kwargs.pop("scp", None) or self.__scp
-        if _scp is True:
+        _scp: Optional[bool] = kwargs.pop("scp", None) or self.__scp
+        if _scp is not None and _scp is True:
             TransferPlus(self).get(*args, **kwargs)
             return None
         else:
-            return super().get(*args, **kwargs)
-        
-        
+            # not covering this, as its just a call to the base version and is covered by
+            # fabric's base tests.
+            return super().get(*args, **kwargs)  # pragma: no cover
+
     def put(self, *args, **kwargs) -> Optional[fabric.transfer.Result]:
         """Put a file on the remote host.
-        
+
         :param local_path: The path to the file on the local host.
         :param remote_path: The path to save the file remotely. Defaults to current working dir for the session.
         :param scp: If the transfer should be done via SCP. Defaults to False or the Connection value.
         :param recursive: If the transfer should be recursive. Defaults to False.
         :param preserve_times: If the file times should be preserved. Defaults to False.
         :return: Result object from the transfer.
         :rtype: Optional[fabric.transfer.Result]
         """
-        _scp: bool = kwargs.pop("scp", None) or self.__scp
-        if _scp is True:
+        _scp: Optional[bool] = kwargs.pop("scp", None) or self.__scp
+        if _scp is not None and _scp is True:
             TransferPlus(self).put(*args, **kwargs)
             return None
         else:
-            return super().put(*args, **kwargs)
+            # not covering this, as its just a call to the base version and is covered by
+            # fabric's base tests.
+            return super().put(*args, **kwargs)  # pragma: no cover
```

### Comparing `fabricplus-0.1.0/fabricplus/paramiko_modifications/client.py` & `fabricplus-1.0.0/fabricplus/paramiko_modifications/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,78 +43,80 @@
 class SSHJumpClient(SSHClient):
     """
     Manage an SSH session which is optionally being proxied
     through a Jump Host.
     """
 
     def __init__(
-            self,
-            *,
-            jump_session: Optional[SSHClient] = None,
-            auth_handler: Optional[Callable] = None,
+        self,
+        *,
+        jump_session: Optional[SSHClient] = None,
+        auth_handler: Optional[Callable] = None,
     ) -> None:
         """
         SSHJumpClient constructor, which is a subclass of
         paramiko.client.SSHClient.
-        
+
         :param jump_session:
             If provided, proxy SSH connections through the another
             instance of SSHClient.
         :param auth_handler:
             If provided, keyboard-interactive authentication will be
             implemented, using this handler as the callback. If this
             is set to None, use Paramiko's default authentication
             algorithm instead of forcing keyboard-interactive
             authentication.
         """
         super().__init__()
         self._jump_session: Optional[SSHClient] = jump_session
         j: Optional[SSHClient] = self._jump_session
-        if j is not None and not hasattr(j, '_transport'):
-            raise TypeError(f'bad jump_session: {j}')
+        if j is not None and not hasattr(j, "_transport"):
+            raise TypeError(f"bad jump_session: {j}")
         self._auth_handler: Optional[Callable[..., Any]] = auth_handler
 
     def __repr__(self) -> str:
         """Return repr(self).
 
         :return: The class name and the jump session and auth handler.
         :rtype: str
         """
-        return (f'{self.__class__.__name__}('
-                f'jump_session={self._jump_session!r}, '
-                f'auth_handler={self._auth_handler!r})')
+        return (
+            f"{self.__class__.__name__}("
+            f"jump_session={self._jump_session!r}, "
+            f"auth_handler={self._auth_handler!r})"
+        )
 
     def __str__(self) -> str:
         """String representation of the object.
 
         :return: The class name.
         :rtype: str
         """
         return self.__class__.__name__
 
     def _auth(
-            self,
-            username: AnyStr,
-            password: Optional[AnyStr] = None,
-            pkey: Optional[PKey] = None,
-            key_filenames: Optional[AnyStr] = None,
-            allow_agent: bool = True,
-            look_for_keys: bool = True,
-            gss_auth: bool = False,
-            gss_kex: bool = False,
-            gss_deleg_creds: bool = True,
-            gss_host: Optional[AnyStr] = None,
-            passphrase: Optional[AnyStr] = None,
+        self,
+        username: AnyStr,
+        password: Optional[AnyStr] = None,
+        pkey: Optional[PKey] = None,
+        key_filenames: Optional[AnyStr] = None,
+        allow_agent: bool = True,
+        look_for_keys: bool = True,
+        gss_auth: bool = False,
+        gss_kex: bool = False,
+        gss_deleg_creds: bool = True,
+        gss_host: Optional[AnyStr] = None,
+        passphrase: Optional[AnyStr] = None,
     ) -> None:  # pylint: disable=R0913
         """
         Authenticate to the server.
-        
-        :param username: 
+
+        :param username:
             Username to authenticate with.
-        :param password: 
+        :param password:
             Password to authenticate with, defaults to None
         :param pkey:
             Private key file to use for authentication, defaults to None
         :param key_filenames:
             Private key filenames to use for authentication, defaults to None
         :param allow_agent:
             Allow local SSH Agent to provide private key files, defaults to True
@@ -132,60 +134,60 @@
             Passphrase to use for private key, defaults to None
         :return: None
         :rtype: None
         """
         if callable(self._auth_handler):
             # Ignore type issues here, as the super class does
             # not share _transport information (which is private)
-            return self._transport.auth_interactive( # type: ignore
+            return self._transport.auth_interactive(  # type: ignore
                 username=username,
                 handler=self._auth_handler,
             )
 
-        return super()._auth( # type: ignore
+        return super()._auth(  # type: ignore
             username=username,
             password=password,
             pkey=pkey,
             key_filenames=key_filenames,
             allow_agent=allow_agent,
             look_for_keys=look_for_keys,
             gss_auth=gss_auth,
             gss_kex=gss_kex,
             gss_deleg_creds=gss_deleg_creds,
             gss_host=gss_host,
             passphrase=passphrase,
         )
 
     def connect(
-            self,
-            hostname: str,
-            port: int = SSH_PORT,
-            username: Optional[str] = None,
-            password: Optional[str] = None,
-            pkey: Optional[PKey] = None,
-            key_filename: Optional[str] = None,
-            timeout: Optional[int] = None,
-            allow_agent: bool = True,
-            look_for_keys: bool = True,
-            compress: bool = False,
-            sock: Optional[socket] = None,
-            gss_auth: bool = False,
-            gss_kex: bool = False,
-            gss_deleg_creds: bool = True,
-            gss_host: Optional[str] = None,
-            banner_timeout: Optional[int] = None,
-            auth_timeout: Optional[int] = None,
-            gss_trust_dns: bool = True,
-            passphrase: Optional[str] = None,
-            disabled_algorithms: Optional[Dict[str, List[str]]] = None,
+        self,
+        hostname: str,
+        port: int = SSH_PORT,
+        username: Optional[str] = None,
+        password: Optional[str] = None,
+        pkey: Optional[PKey] = None,
+        key_filename: Optional[str] = None,
+        timeout: Optional[int] = None,
+        allow_agent: bool = True,
+        look_for_keys: bool = True,
+        compress: bool = False,
+        sock: Optional[socket] = None,
+        gss_auth: bool = False,
+        gss_kex: bool = False,
+        gss_deleg_creds: bool = True,
+        gss_host: Optional[str] = None,
+        banner_timeout: Optional[int] = None,
+        auth_timeout: Optional[int] = None,
+        gss_trust_dns: bool = True,
+        passphrase: Optional[str] = None,
+        disabled_algorithms: Optional[Dict[str, List[str]]] = None,
     ) -> None:  # pylint: disable=R0913,R0914
         """
         Connect to an SSH server and authenticate to it.
 
-        :param hostname: 
+        :param hostname:
             Hostname or IP address of the remote host.
         :param port:
             Port number of the remote host, defaults to SSH_PORT (22)
         :param username:
             Username to authenticate as, defaults to None
         :param password:
             Password to authenticate with, defaults to None
@@ -225,19 +227,20 @@
             If jump_session and sock are both provided as arguments;
             they are mutually exclusive
         :return: None
         :rtype: None
         """
         if self._jump_session is not None:
             if sock is not None:
-                raise ValueError('jump_session= and sock= are mutually '
-                                 'exclusive')
-            transport = self._jump_session._transport  # pylint: disable=W0212 # type: ignore
+                raise ValueError("jump_session= and sock= are mutually " "exclusive")
+            transport = (
+                self._jump_session._transport
+            )  # pylint: disable=W0212 # type: ignore
             sock = transport.open_channel(
-                kind='direct-tcpip',
+                kind="direct-tcpip",
                 dest_addr=(hostname, port),
                 src_addr=transport.getpeername(),
                 timeout=timeout,
             )
 
         return super().connect(
             hostname=hostname,
@@ -292,20 +295,20 @@
 
     def __next__(self):
         return next(self._iterator)
 
 
 @contextmanager
 def jump_host(
-        hostname: AnyStr,
-        username: AnyStr,
-        password: AnyStr,
-        auth_handler: Optional[Callable[..., Any]] = None,
-        look_for_keys: bool = True,
-        auto_add_missing_key_policy: bool = False,
+    hostname: AnyStr,
+    username: AnyStr,
+    password: AnyStr,
+    auth_handler: Optional[Callable[..., Any]] = None,
+    look_for_keys: bool = True,
+    auto_add_missing_key_policy: bool = False,
 ) -> Iterator:  # pylint: disable=R0913
     """
 
     Example
     -------
     >>> from paramiko_jump import SSHJumpClient, simple_auth_handler
     >>> with jump_host(
@@ -354,17 +357,17 @@
         )
         yield jumper
     finally:
         jumper.close()
 
 
 def simple_auth_handler(
-        title: AnyStr,
-        instructions: AnyStr,
-        prompt_list: Sequence[_Prompt],
+    title: AnyStr,
+    instructions: AnyStr,
+    prompt_list: Sequence[_Prompt],
 ) -> List[AnyStr]:
     """
     Authentication callback, for keyboard-interactive
     authentication.
 
     :param title:
         Displayed to the end user before anything else.
@@ -385,19 +388,19 @@
     if title:
         print(title)
     if instructions:
         print(instructions)
 
     for prompt, show_input in prompt_list:
         input_ = input if show_input else getpass
-        answers.append(input_(prompt)) # type: ignore
+        answers.append(input_(prompt))  # type: ignore
     return answers
 
 
 # LICENSE INFORMATION
 # -------------------
 # Copyright 2020, Andrew Blair Schenck
 # Licensed under the Apache License, Version 2.0.
 # A copy of the License is available at:
 #     http://www.apache.org/licenses/LICENSE-2.0
 # -------------------
-# END OF FILE
+# END OF FILE
```

### Comparing `fabricplus-0.1.0/fabricplus/transfer.py` & `fabricplus-1.0.0/fabricplus/transfer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import fabric
 from fabric.transfer import Transfer
 import scp
 
-from typing import Union, TypeVar
+from typing import TypeVar
 
 # Type hint for a fabric Connection object.
 Conn = TypeVar("Conn", bound=fabric.connection.Connection)
 
+
 class TransferPlus(Transfer):
     """TransferPlus is a subclass of the base fabric Transfer object, overloading
     the parent object to provide additional functionality for SCP transfers.
     """
 
-    def __init__(self,
-                 connection: Conn) -> None:
+    def __init__(self, connection: Conn) -> None:
         """Initializes the TransferPlus object.
 
         :param connection: A fabric Connection-like object.
         """
         self.connection: Conn = connection
 
     @property
@@ -27,35 +27,37 @@
         :raises AttributeError: If the base fabric Connection object does not have an SCP client.
         :return: An SCP client object.
         :rtype: scp.SCPClient
         """
         try:
             return self.connection.scp()
         except AttributeError:
-            raise AttributeError("The base fabric Connection object does not have an SCP client"
-                                 ", use ConnectionPlus instead.")
-    
+            raise AttributeError(
+                "The base fabric Connection object does not have an SCP client"
+                ", use ConnectionPlus instead."
+            )
+
     def get(self, *args, **kwargs) -> None:
         """Get a file from the remote host.
-        
+
         :param remote_path: The path to the file on the remote host.
         :param local_path: The path to save the file locally. Defaults to current working dir.
         :param scp: If the transfer should be done via SCP. Defaults to False or the Connection value.
         :param recursive: If the transfer should be recursive. Defaults to False.
         :param preserve_times: If the file times should be preserved. Defaults to False.
         :return: None
         :rtype: None
         """
         return self.scp.get(*args, **kwargs)
-    
+
     def put(self, *args, **kwargs) -> None:
         """Put a file on the remote host.
-        
+
         :param local_path: The path to the file on the local host.
         :param remote_path: The path to save the file remotely. Defaults to current working dir for the session.
         :param scp: If the transfer should be done via SCP. Defaults to False or the Connection value.
         :param recursive: If the transfer should be recursive. Defaults to False.
         :param preserve_times: If the file times should be preserved. Defaults to False.
         :return: None
         :rtype: None
         """
-        return self.scp.put(*args, **kwargs)
+        return self.scp.put(*args, **kwargs)
```

### Comparing `fabricplus-0.1.0/pyproject.toml` & `fabricplus-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fabricplus"
-version = "0.1.0"
+version = "1.0.0"
 description = "A Python 3.8.10+ wrapper to add in SCP functionality for file transfer in Fabric."
 authors = ["Courtney Caldwell <courtneyccaldwell@gmail.com>"]
 maintainers = ["Courtney Caldwell <courtneyccaldwell@gmail.com>"]
 repository = "https://github.com/prokopto-dev/fabric-plus"
 homepage = "https://fabricplus.prokopto.dev/"
 keywords = ["fabric", "scp", "file transfer", "python", "wrapper", "paramiko", "connection", "transfer"]
 classifiers = [
@@ -21,23 +21,28 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.8.1,<4.0"
 scp = "^0.14.5"
 fabric = "^3.2.2"
 paramiko = "^3.4.0"
 invoke = "^2.2.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 poetry = "^1.8.3"
 pytest-cov = "^5.0.0"
 pytest-mock = "^3.14.0"
 mypy = "^1.10.0"
+flake8 = "^7.0.0"
+black = "^24.4.2"
+
+[tool.pytest.ini_options]
+addopts = "-v --cov=fabricplus --cov-report=term-missing --cov-report=xml --cov-config=.coveragerc"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

