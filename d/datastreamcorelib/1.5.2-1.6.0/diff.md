# Comparing `tmp/datastreamcorelib-1.5.2.tar.gz` & `tmp/datastreamcorelib-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastreamcorelib-1.5.2.tar", max compression
+gzip compressed data, was "datastreamcorelib-1.6.0.tar", max compression
```

## Comparing `datastreamcorelib-1.5.2.tar` & `datastreamcorelib-1.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-03-20 11:05:42.637064 datastreamcorelib-1.5.2/LICENSE
--rw-r--r--   0        0        0     3488 2023-03-20 11:05:42.637064 datastreamcorelib-1.5.2/README.rst
--rw-r--r--   0        0        0     2238 2023-03-20 11:05:42.645064 datastreamcorelib-1.5.2/pyproject.toml
--rw-r--r--   0        0        0      168 2023-03-20 11:05:42.645064 datastreamcorelib-1.5.2/src/datastreamcorelib/__init__.py
--rw-r--r--   0        0        0     4869 2023-03-20 11:05:42.645064 datastreamcorelib-1.5.2/src/datastreamcorelib/abstract.py
--rw-r--r--   0        0        0     1257 2023-03-20 11:05:42.645064 datastreamcorelib-1.5.2/src/datastreamcorelib/binpackers.py
--rw-r--r--   0        0        0     2649 2023-03-20 11:05:42.645064 datastreamcorelib-1.5.2/src/datastreamcorelib/datamessage.py
--rw-r--r--   0        0        0     5842 2023-03-20 11:05:42.645064 datastreamcorelib-1.5.2/src/datastreamcorelib/imagemessage.py
--rw-r--r--   0        0        0      228 2023-03-20 11:05:42.645064 datastreamcorelib-1.5.2/src/datastreamcorelib/logging.py
--rw-r--r--   0        0        0    10635 2023-03-20 11:05:42.645064 datastreamcorelib-1.5.2/src/datastreamcorelib/pubsub.py
--rw-r--r--   0        0        0        0 2023-03-20 11:05:42.645064 datastreamcorelib-1.5.2/src/datastreamcorelib/py.typed
--rw-r--r--   0        0        0     7953 2023-03-20 11:05:42.645064 datastreamcorelib-1.5.2/src/datastreamcorelib/reqrep.py
--rw-r--r--   0        0        0      144 2023-03-20 11:05:42.645064 datastreamcorelib-1.5.2/src/datastreamcorelib/testhelpers.py
--rw-r--r--   0        0        0      926 2023-03-20 11:05:42.645064 datastreamcorelib-1.5.2/src/datastreamcorelib/utils.py
--rw-r--r--   0        0        0     4597 2023-03-20 11:05:43.760282 datastreamcorelib-1.5.2/setup.py
--rw-r--r--   0        0        0     4432 2023-03-20 11:05:43.760857 datastreamcorelib-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-09 09:54:19.126783 datastreamcorelib-1.6.0/LICENSE
+-rw-r--r--   0        0        0     3488 2023-05-09 09:54:19.126783 datastreamcorelib-1.6.0/README.rst
+-rw-r--r--   0        0        0     2452 2023-05-09 09:54:19.130783 datastreamcorelib-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-09 09:54:19.130783 datastreamcorelib-1.6.0/src/datastreamcorelib/__init__.py
+-rw-r--r--   0        0        0     4825 2023-05-09 09:54:19.130783 datastreamcorelib-1.6.0/src/datastreamcorelib/abstract.py
+-rw-r--r--   0        0        0     1257 2023-05-09 09:54:19.130783 datastreamcorelib-1.6.0/src/datastreamcorelib/binpackers.py
+-rw-r--r--   0        0        0     2563 2023-05-09 09:54:19.130783 datastreamcorelib-1.6.0/src/datastreamcorelib/datamessage.py
+-rw-r--r--   0        0        0     5756 2023-05-09 09:54:19.130783 datastreamcorelib-1.6.0/src/datastreamcorelib/imagemessage.py
+-rw-r--r--   0        0        0      228 2023-05-09 09:54:19.130783 datastreamcorelib-1.6.0/src/datastreamcorelib/logging.py
+-rw-r--r--   0        0        0    10591 2023-05-09 09:54:19.130783 datastreamcorelib-1.6.0/src/datastreamcorelib/pubsub.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:54:19.130783 datastreamcorelib-1.6.0/src/datastreamcorelib/py.typed
+-rw-r--r--   0        0        0     7953 2023-05-09 09:54:19.130783 datastreamcorelib-1.6.0/src/datastreamcorelib/reqrep.py
+-rw-r--r--   0        0        0      144 2023-05-09 09:54:19.130783 datastreamcorelib-1.6.0/src/datastreamcorelib/testhelpers.py
+-rw-r--r--   0        0        0      926 2023-05-09 09:54:19.130783 datastreamcorelib-1.6.0/src/datastreamcorelib/utils.py
+-rw-r--r--   0        0        0     4597 2023-05-09 09:54:20.062703 datastreamcorelib-1.6.0/setup.py
+-rw-r--r--   0        0        0     4432 2023-05-09 09:54:20.063293 datastreamcorelib-1.6.0/PKG-INFO
```

### Comparing `datastreamcorelib-1.5.2/LICENSE` & `datastreamcorelib-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datastreamcorelib-1.5.2/README.rst` & `datastreamcorelib-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `datastreamcorelib-1.5.2/pyproject.toml` & `datastreamcorelib-1.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datastreamcorelib"
-version = "1.5.2"
+version = "1.6.0"
 description = "Helpers and utilities for https://gitlab.com/advian-oss/python-datastreamservicelib that are not eventloop specific."
 authors = ["Eero af Heurlin <eero.afheurlin@iki.fi>"]
 homepage = "https://gitlab.com/advian-oss/python-datastreamcorelib/"
 repository = "https://gitlab.com/advian-oss/python-datastreamcorelib/"
 license = "MIT"
 readme = "README.rst"
 
@@ -28,14 +28,15 @@
   |  __pycache__
 )
 '''
 
 [tool.pytest.ini_options]
 junit_family="xunit2"
 addopts="--cov=datastreamcorelib --cov-fail-under=65 --cov-branch"
+asyncio_mode="strict"
 
 [tool.pylint.format]
 max-line-length = 120
 
 [tool.pylint.messages_control]
 disable=["fixme", "logging-format-interpolation", "C0209"]
 
@@ -56,28 +57,34 @@
 # [tool.poetry.group.dev.dependencies] # This won't work for py36 since the available poetry-core is too old
 [tool.poetry.dev-dependencies]
 pytest = [
     { version = "^7.1", python="^3.7" },
     { version = "^6.2", python="~3.6" }
 ]
 coverage = [
-    { version = "^6.3", extras = ["toml"], python="^3.7" },
-    { version = "^5.4", extras = ["toml"], python="~3.6" }
+    { version = "^7.0", extras = ["toml"], python="^3.7" },
+    { version = "^5.4", extras = ["toml"], python=">3.6" }
+]
+pytest-cov = "^4.0"
+pylint = [
+    { version = "^2.17", python=">=3.8,<=4.0" },
+    { version = "^2.13", python=">=3.0,<=3.8" }
 ]
-pytest-cov = "^3.0"
-pylint = "^2.13"
 black = "^22.3"
 bandit = [
     { version = "^1.7", extras = ["toml"], python="^3.7" },
     { version = "=1.7.1", extras = ["toml"], python="~3.6" }
 ]
-mypy = "^0.942"
+mypy = [
+    { version = "^1.2", python=">=3.8,<=4.0" },
+    { version = "^0.942", python=">=3.0,<=3.8" }
+]
 pre-commit = "^2.17"
 pytest-asyncio = [
-    { version="^0.18", python="^3.7" },
+    { version=">=0.18,<=1.0", python="^3.7" },
     { version="^0.14", python="~3.6" }
 ]
 bump2version = "^1.0"
 detect-secrets = "^1.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `datastreamcorelib-1.5.2/src/datastreamcorelib/abstract.py` & `datastreamcorelib-1.6.0/src/datastreamcorelib/abstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Abstract baseclasses so that different eventloop implementations have common API for the user."""
 import enum
-from abc import ABC, abstractmethod
+from abc import ABC, abstractmethod  # pylint: disable=E0611  # false positive
 from dataclasses import dataclass, field
 from typing import Dict, List, Sequence, Union, Type, Set
 
 from .binpackers import normalize_uri_topic_list
 
 
 SOCKETHANDLER_SINGLETONS: Dict[Type["BaseSocketHandler"], "BaseSocketHandler"] = {}
@@ -107,16 +107,15 @@
 
     @abstractmethod
     def __hash__(self) -> int:
         """Sockets are used as parts of dict keys, they must be "hashable" """
         raise NotImplementedError()
 
 
-# See https://github.com/python/mypy/issues/5374 why the typing ignore
-@dataclass  # type: ignore
+@dataclass
 class BaseSocketHandler(ABC):
     """Baseclass for IOLoop specific socket handling stuff."""
 
     _sockets_by_desc: Dict[ZMQSocketDescription, ZMQSocket] = field(default_factory=dict, init=False, repr=False)
 
     def _get_cached_socket(self, desc: ZMQSocketDescription) -> Union[ZMQSocket, None]:
         """Get socket from cache if it exists"""
```

### Comparing `datastreamcorelib-1.5.2/src/datastreamcorelib/binpackers.py` & `datastreamcorelib-1.6.0/src/datastreamcorelib/binpackers.py`

 * *Files identical despite different names*

### Comparing `datastreamcorelib-1.5.2/src/datastreamcorelib/datamessage.py` & `datastreamcorelib-1.6.0/src/datastreamcorelib/datamessage.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 from typing import Any, Dict, List
 
 from .abstract import BaseMessage, TooFewPartsError
 from .binpackers import msgpack_pack, msgpack_unpack
 from .pubsub import PubSubMessage
 
 
-# See https://github.com/python/mypy/issues/5374 why the typing ignore
-@dataclass  # type: ignore # pylint: disable=W0223
-class BaseDataMessage(BaseMessage):
+@dataclass
+class BaseDataMessage(BaseMessage):  # pylint: disable=W0223
     """Baseclass for all ZMQ DataMessage types."""
 
     messageid: uuid.UUID = field(default_factory=uuid.uuid4)
     data: Dict[Any, Any] = field(compare=False, default_factory=dict)
 
     def __post_init__(self) -> None:
         """Auto-add systemtime if data is empty"""
```

### Comparing `datastreamcorelib-1.5.2/src/datastreamcorelib/imagemessage.py` & `datastreamcorelib-1.6.0/src/datastreamcorelib/imagemessage.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,17 +16,16 @@
     """Image format errors"""
 
 
 class MissingImgAttributeError(ImgFormatError):
     """Somthing is missing"""
 
 
-# See https://github.com/python/mypy/issues/5374 why the typing ignore
-@dataclass  # type: ignore # pylint: disable=W0223
-class BaseImageMessage(BaseDataMessage):
+@dataclass
+class BaseImageMessage(BaseDataMessage):  # pylint: disable=W0223
     """
     Baseclass for image messages (extension to DataMessages)
 
     These are DataMessages with extra part for the image and well-known
     key in the data part for the image format data.
 
         data["imginfo"] = {
```

### Comparing `datastreamcorelib-1.5.2/src/datastreamcorelib/pubsub.py` & `datastreamcorelib-1.6.0/src/datastreamcorelib/pubsub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """PUB/SUB related helpers."""
 from typing import Any, Coroutine, Callable, Dict, List, Sequence, Tuple, Type, Union, Optional, cast
-from abc import ABC, abstractmethod
+from abc import ABC, abstractmethod  # pylint: disable=E0611  # false positive
 from dataclasses import dataclass, field
 import logging
 import uuid
 
 
 from .abstract import (
     BaseMessage,
@@ -143,16 +143,15 @@
             raise exc
 
 
 # Alias for readability
 SubscriptionMKType = Tuple[ZMQSocket, bytes]
 
 
-# See https://github.com/python/mypy/issues/5374 why the typing ignore
-@dataclass  # type: ignore
+@dataclass
 class BasePubSubManager(ABC):
     """
     Manage subscriptions, the actual sockethandler implementation will take care of opening sockets
     as needed.
     """
 
     handlerklass: Type[BaseSocketHandler] = field(repr=False)
```

### Comparing `datastreamcorelib-1.5.2/src/datastreamcorelib/reqrep.py` & `datastreamcorelib-1.6.0/src/datastreamcorelib/reqrep.py`

 * *Files identical despite different names*

### Comparing `datastreamcorelib-1.5.2/src/datastreamcorelib/utils.py` & `datastreamcorelib-1.6.0/src/datastreamcorelib/utils.py`

 * *Files identical despite different names*

### Comparing `datastreamcorelib-1.5.2/setup.py` & `datastreamcorelib-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['libadvian>=0.3,<=2.0', 'msgpack>=1.0,<2.0']
 
 extras_require = \
 {':python_version >= "3.6" and python_version < "3.7"': ['dataclasses>=0.8,<0.9']}
 
 setup_kwargs = {
     'name': 'datastreamcorelib',
-    'version': '1.5.2',
+    'version': '1.6.0',
     'description': 'Helpers and utilities for https://gitlab.com/advian-oss/python-datastreamservicelib that are not eventloop specific.',
     'long_description': '=================\ndatastreamcorelib\n=================\n\nCore helpers and Abstract Base Classes for making use of ZMQ nice, easy and DRY.\n\nYou should probably look at https://gitlab.com/advian-oss/python-datastreamservicelib and\nhttps://gitlab.com/advian-oss/python-datastreamserviceapp_template unless you\'re working\non an adapter for yet unsupported eventloop.\n\nDocker\n------\n\nFor more controlled deployments and to get rid of "works on my computer" -syndrome, we always\nmake sure our software works under docker.\n\nIt\'s also a quick way to get started with a standard development environment.\n\nSSH agent forwarding\n^^^^^^^^^^^^^^^^^^^^\n\nWe need buildkit_::\n\n    export DOCKER_BUILDKIT=1\n\n.. _buildkit: https://docs.docker.com/develop/develop-images/build_enhancements/\n\nAnd also the exact way for forwarding agent to running instance is different on OSX::\n\n    export DOCKER_SSHAGENT="-v /run/host-services/ssh-auth.sock:/run/host-services/ssh-auth.sock -e SSH_AUTH_SOCK=/run/host-services/ssh-auth.sock"\n\nand Linux::\n\n    export DOCKER_SSHAGENT="-v $SSH_AUTH_SOCK:$SSH_AUTH_SOCK -e SSH_AUTH_SOCK"\n\nCreating a development container\n^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^\n\nBuild image, create container and start it::\n\n    docker build --ssh default --target devel_shell -t datastreamcorelib:devel_shell .\n    docker create --name datastreamcorelib_devel -v `pwd`":/app" -it -v /tmp:/tmp `echo $DOCKER_SSHAGENT` datastreamcorelib:devel_shell\n    docker start -i datastreamcorelib_devel\n\npre-commit considerations\n^^^^^^^^^^^^^^^^^^^^^^^^^\n\nIf working in Docker instead of native env you need to run the pre-commit checks in docker too::\n\n    docker exec -i datastreamcorelib_devel /bin/bash -c "pre-commit install"\n    docker exec -i datastreamcorelib_devel /bin/bash -c "pre-commit run --all-files"\n\nYou need to have the container running, see above. Or alternatively use the docker run syntax but using\nthe running container is faster::\n\n    docker run -it --rm -v `pwd`":/app" datastreamcorelib:devel_shell -c "pre-commit run --all-files"\n\nTest suite\n^^^^^^^^^^\n\nYou can use the devel shell to run py.test when doing development, for CI use\nthe "tox" target in the Dockerfile::\n\n    docker build --ssh default --target tox -t datastreamcorelib:tox .\n    docker run -it --rm -v `pwd`":/app" `echo $DOCKER_SSHAGENT` datastreamcorelib:tox\n\nProduction docker\n^^^^^^^^^^^^^^^^^\n\nThere\'s a "production" target since it\'s our standard pattern, however this library does not yet\nexpose any CLI tools so the production target is kinda useless.\n\nLocal Development\n-----------------\n\nTLDR:\n\n- Create and activate a Python 3.6 virtualenv (assuming virtualenvwrapper)::\n\n    mkvirtualenv -p `which python3.6` my_virtualenv\n\n- change to a branch::\n\n    git checkout -b my_branch\n\n- install Poetry: https://python-poetry.org/docs/#installation\n- Install project deps and pre-commit hooks::\n\n    poetry install\n    pre-commit install\n    pre-commit run --all-files\n\n- Ready to go.\n\nUse Python 3.6 for development since it\'s the lowest supported version so you don\'t accidentally\nuse features only available in higher versions and then have to re-do everything when CI tests fail\non 3.6.\n\nRemember to activate your virtualenv whenever working on the repo, this is needed\nbecause pylint and mypy pre-commit hooks use the "system" python for now (because reasons).\n\nRunning "pre-commit run --all-files" and "py.test -v" regularly during development and\nespecially before committing will save you some headache.\n',
     'author': 'Eero af Heurlin',
     'author_email': 'eero.afheurlin@iki.fi',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/advian-oss/python-datastreamcorelib/',
```

### Comparing `datastreamcorelib-1.5.2/PKG-INFO` & `datastreamcorelib-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datastreamcorelib
-Version: 1.5.2
+Version: 1.6.0
 Summary: Helpers and utilities for https://gitlab.com/advian-oss/python-datastreamservicelib that are not eventloop specific.
 Home-page: https://gitlab.com/advian-oss/python-datastreamcorelib/
 License: MIT
 Author: Eero af Heurlin
 Author-email: eero.afheurlin@iki.fi
 Requires-Python: >=3.6.2,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

