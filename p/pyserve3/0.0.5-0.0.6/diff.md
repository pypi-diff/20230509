# Comparing `tmp/pyserve3-0.0.5.tar.gz` & `tmp/pyserve3-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyserve3-0.0.5.tar", last modified: Wed Apr 26 23:09:05 2023, max compression
+gzip compressed data, was "pyserve3-0.0.6.tar", last modified: Tue May  9 00:55:03 2023, max compression
```

## Comparing `pyserve3-0.0.5.tar` & `pyserve3-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 23:09:05.162360 pyserve3-0.0.5/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-03-26 23:32:22.000000 pyserve3-0.0.5/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1415 2023-04-26 23:09:05.162360 pyserve3-0.0.5/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)      944 2023-03-19 20:01:09.000000 pyserve3-0.0.5/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 23:09:05.162360 pyserve3-0.0.5/pyserve/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5912 2023-04-26 22:52:30.000000 pyserve3-0.0.5/pyserve/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1608 2023-04-26 22:44:45.000000 pyserve3-0.0.5/pyserve/abc.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     6906 2023-04-26 23:07:38.000000 pyserve3-0.0.5/pyserve/threading.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3029 2023-04-26 22:37:10.000000 pyserve3-0.0.5/pyserve/transport.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-26 23:09:05.162360 pyserve3-0.0.5/pyserve3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1415 2023-04-26 23:09:05.000000 pyserve3-0.0.5/pyserve3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      231 2023-04-26 23:09:05.000000 pyserve3-0.0.5/pyserve3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-26 23:09:05.000000 pyserve3-0.0.5/pyserve3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        8 2023-04-26 23:09:05.000000 pyserve3-0.0.5/pyserve3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-26 23:09:05.162360 pyserve3-0.0.5/setup.cfg
--rw-r--r--   0 andrew    (1000) andrew    (1000)      674 2023-04-26 23:08:11.000000 pyserve3-0.0.5/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-09 00:55:03.437190 pyserve3-0.0.6/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-03-26 23:32:22.000000 pyserve3-0.0.6/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1415 2023-05-09 00:55:03.433190 pyserve3-0.0.6/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      944 2023-03-19 20:01:09.000000 pyserve3-0.0.6/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-09 00:55:03.433190 pyserve3-0.0.6/pyserve/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5942 2023-05-09 00:45:08.000000 pyserve3-0.0.6/pyserve/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2139 2023-05-09 00:45:25.000000 pyserve3-0.0.6/pyserve/abc.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     6849 2023-05-09 00:45:41.000000 pyserve3-0.0.6/pyserve/threading.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2997 2023-05-06 22:37:04.000000 pyserve3-0.0.6/pyserve/transport.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-05-09 00:55:03.433190 pyserve3-0.0.6/pyserve3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1415 2023-05-09 00:55:03.000000 pyserve3-0.0.6/pyserve3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      231 2023-05-09 00:55:03.000000 pyserve3-0.0.6/pyserve3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-05-09 00:55:03.000000 pyserve3-0.0.6/pyserve3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        8 2023-05-09 00:55:03.000000 pyserve3-0.0.6/pyserve3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-05-09 00:55:03.437190 pyserve3-0.0.6/setup.cfg
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      674 2023-05-09 00:54:46.000000 pyserve3-0.0.6/setup.py
```

### Comparing `pyserve3-0.0.5/LICENSE` & `pyserve3-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyserve3-0.0.5/PKG-INFO` & `pyserve3-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyserve3
-Version: 0.0.5
+Version: 0.0.6
 Summary: Unify SocketServer Implementations based on a Session Model
 Home-page: https://github.com/imgurbot12/pyserve
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyserve3-0.0.5/README.md` & `pyserve3-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyserve3-0.0.5/pyserve/__init__.py` & `pyserve3-0.0.6/pyserve/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """
 Unify SocketServer Implementations based on Session Model
 """
 import asyncio
 from ssl import SSLContext
 from typing import Type, Optional
 
-from .abc import RawAddr, Address, Writer, Session, modify_socket
+from .abc import * 
 from .transport import UdpProtocol, TcpProtocol
 from .threading import UdpThreadServer, TcpThreadServer
 
 #** Variables **#
 __all__ = [
     'listen_udp_async',
     'listen_tcp_async',
     'listen_udp_threaded',
     'listen_tcp_threaded',
 
     'Address',
     'Writer',
+    'UdpWriter',
     'Session',
 ]
 
 #** Functions **#
 
 async def listen_udp_async(
     address:         RawAddr, 
     factory:         Type[Session],
     *args,
-    interface:       Optional[bytes] = None,
-    reuse_port:      bool            = False,
-    allow_broadcast: bool            = False,
+    interface:       Optional[str] = None,
+    reuse_port:      bool          = False,
+    allow_broadcast: bool          = False,
     **kwargs,
 ):
     """
     :param address:         host/port of server
     :param factory:         type factory for server request handler
     :param args:            positional args to pass to the session factory
     :param interface:       interface to bind server socket to
@@ -60,15 +61,15 @@
         tport.close()
 
 async def listen_tcp_async(
     address:    RawAddr, 
     factory:    Type[Session],
     *args,
     timeout:    Optional[int]        = None,
-    interface:  Optional[bytes]      = None,
+    interface:  Optional[str]        = None,
     reuse_port: bool                 = False,
     backlog:    int                  = 100,
     ssl:        Optional[SSLContext] = None,
     **kwargs,
 ):
     """
     :param address:         host/port of server
@@ -97,17 +98,18 @@
     async with server:
         await server.serve_forever()
 
 def listen_udp_threaded(
     address:         RawAddr, 
     factory:         Type[Session],
     *args,
-    interface:       Optional[bytes] = None,
-    reuse_port:      bool            = False,
-    allow_broadcast: bool            = False,
+    interface:       Optional[str] = None,
+    reuse_port:      bool          = False,
+    allow_broadcast: bool          = False,
+    blocksize:  int                = 8192,
     **kwargs,
 ):
     """
     :param address:         host/port of server
     :param factory:         type factory for server request handler
     :param args:            positional args to pass to the session factory
     :param timeout:         max socket lifetime duration timeout if configured
@@ -118,27 +120,28 @@
     """
     factory(*args, **kwargs)
     server = UdpThreadServer(
         address=address, 
         factory=factory, 
         args=args, 
         kwargs=kwargs, 
-        interface=interface, 
+        interface=interface,
+        blocksize=blocksize,
         reuse_port=reuse_port, 
         allow_broadcast=allow_broadcast,
     )
     with server:
         server.serve_forever()
 
 def listen_tcp_threaded(
     address:    RawAddr,
     factory:    Type[Session],
     *args,
     timeout:    Optional[int]        = None,
-    interface:  Optional[bytes]      = None,
+    interface:  Optional[str]        = None,
     reuse_port: bool                 = False,
     ssl:        Optional[SSLContext] = None,
     blocksize:  int                  = 8192,
     **kwargs,
 ):
     """
     :param address:         host/port of server
```

### Comparing `pyserve3-0.0.5/pyserve/abc.py` & `pyserve3-0.0.6/pyserve/abc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,51 @@
 """
 
 """
 import socket
 from abc import abstractmethod
 from collections import namedtuple
-from typing import Tuple, Protocol, Optional
+from typing import Tuple, Protocol, Optional, Union
 
 #** Variables **#
 __all__ = [
     'modify_socket',
 
     'RawAddr',
-    'Address', 
-    'Writer', 
+    'Address',
+    'AnyAddr',
+    'Writer',
+    'UdpWriter',
     'Session',
 ]
 
 #: raw address tuple
 RawAddr = Tuple[str, int]
 
 #: named address tuple
 Address = namedtuple('Address', ('host', 'port'))
 
+#: any address tuple
+AnyAddr = Union[RawAddr, Address]
+
 #** Functions **#
 
 def modify_socket(
     sock:      socket.socket, 
     timeout:   Optional[int], 
-    interface: Optional[bytes]
+    interface: Optional[str]
 ) -> socket.socket:
     """
     modify the socket object w/ the following options
     """
     if timeout is not None:
         sock.settimeout(timeout)
     if interface is not None:
-        sock.setsockopt(socket.SOL_SOCKET, socket.SO_BINDTODEVICE, interface)
+        iface = interface.encode()
+        sock.setsockopt(socket.SOL_SOCKET, socket.SO_BINDTODEVICE, iface)
     return sock 
 
 #** Classes **#
 
 class Writer(Protocol):
     """
     abstract data-writing implementation for single server connection
@@ -50,14 +56,31 @@
         raise NotImplementedError
     
     @abstractmethod
     def close(self):
         raise NotImplementedError
 
     @abstractmethod
+    def is_closing(self) -> bool:
+        raise NotImplementedError
+
+class UdpWriter(Writer, Protocol):
+    """
+    abstract data-writing implementation for udp server connection
+    """
+
+    @abstractmethod
+    def write(self, data: bytes, addr: Optional[AnyAddr] = None):
+        raise NotImplementedError
+    
+    @abstractmethod
+    def close(self):
+        raise NotImplementedError
+
+    @abstractmethod
     def is_closing(self) -> bool:
         raise NotImplementedError
 
 class Session(Protocol):
     """
     abstract session-manager implemention for single server connection
     """
```

### Comparing `pyserve3-0.0.5/pyserve/threading.py` & `pyserve3-0.0.6/pyserve/threading.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Threading Implementations of session-based servers
 """
 import socket
 import socketserver
-from ssl import SSLContext, wrap_socket
+from ssl import SSLContext
 from dataclasses import dataclass, field
 from typing import Type, Optional, Dict, Any, ClassVar
 
-from .abc import RawAddr, Address, Writer, Session, modify_socket
+from .abc import *
 
 #** Variables **#
 __all__ = ['UdpThreadServer', 'TcpThreadServer']
 
 #** Functions **#
 
 def new_handler(
@@ -34,20 +34,20 @@
         kwargs=kwargs,
         blocksize=blocksize,
     ))
 
 #** Classes **#
 
 @dataclass
-class UdpWriter(Writer):
+class UdpWriter(UdpWriter):
     addr: Address
     sock: socket.socket
     closing: bool = False
-    
-    def write(self, data: bytes, addr: Optional[Address] = None):
+
+    def write(self, data: bytes, addr: Optional[AnyAddr] = None):
         self.sock.sendto(data, addr or self.addr)
 
     def close(self):
         self.sock.close()
         self.closing = True
 
     def is_closing(self) -> bool:
@@ -130,19 +130,19 @@
 
 @dataclass
 class BaseThreadServer(socketserver.ThreadingMixIn):
     handler: ClassVar[Type[BaseRequestHandler]]
 
     address:    RawAddr
     factory:    Type[Session]
-    args:       tuple           = field(default_factory=tuple)
-    kwargs:     Dict[str, Any]  = field(default_factory=dict)
-    interface:  Optional[bytes] = None
-    reuse_port: bool            = False
-    blocksize: int              = 8192
+    args:       tuple          = field(default_factory=tuple)
+    kwargs:     Dict[str, Any] = field(default_factory=dict)
+    interface:  Optional[str]  = None
+    reuse_port: bool           = False
+    blocksize: int             = 8192
  
     def __post_init__(self):
         self.max_packet_size  = self.blocksize
         self.allow_reuse_port = self.reuse_port
 
     def new_handler(self) -> Type[BaseRequestHandler]:
         return new_handler(
@@ -208,15 +208,15 @@
         self.shutdown()
  
     def server_bind(self):
         """additional socket modification controls on server-bind"""
         super().server_bind()
         modify_socket(self.socket, None, self.interface)
         if self.ssl:
-            self.socket = wrap_socket(self.socket, server_side=True)
+            self.socket = self.ssl.wrap_socket(self.socket, server_side=True)
 
     def get_request(self):
         """respawn socket after socket error to prevent infinite hanging loop"""
         try:
             sock, addr = super().get_request()
             modify_socket(sock, self.timeout, None)
             return (sock, addr)
```

### Comparing `pyserve3-0.0.5/pyserve/transport.py` & `pyserve3-0.0.6/pyserve/transport.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 AsyncIO Implementations of session-based servers
 """
 import asyncio
 from dataclasses import dataclass, field
 from typing import Type, Optional, Dict, Any
 
-from .abc import RawAddr, Address, Writer, Session
+from .abc import * 
 
 #** Variables **#
 __all__ = ['UdpProtocol', 'TcpProtocol']
 
 #** Classes **#
 
 @dataclass
-class UdpWriter(Writer):
+class UdpWriter(UdpWriter):
     addr:      Address
     transport: asyncio.DatagramTransport
-    
-    def write(self, data: bytes, addr: Optional[Address] = None):
+
+    def write(self, data: bytes, addr: Optional[AnyAddr] = None):
         self.transport.sendto(data, addr or self.addr)
 
     def close(self):
         self.transport.close()
 
     def is_closing(self) -> bool:
         return self.transport.is_closing()
```

### Comparing `pyserve3-0.0.5/pyserve3.egg-info/PKG-INFO` & `pyserve3-0.0.6/pyserve3.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyserve3
-Version: 0.0.5
+Version: 0.0.6
 Summary: Unify SocketServer Implementations based on a Session Model
 Home-page: https://github.com/imgurbot12/pyserve
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyserve3-0.0.5/setup.py` & `pyserve3-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='pyserve3',
-    version='0.0.5',
+    version='0.0.6',
     license='MIT',
     packages=find_packages(),
     url='https://github.com/imgurbot12/pyserve',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     description='Unify SocketServer Implementations based on a Session Model',
     python_requires='>=3.7',
```

