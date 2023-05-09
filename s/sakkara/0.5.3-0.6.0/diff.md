# Comparing `tmp/sakkara-0.5.3.tar.gz` & `tmp/sakkara-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sakkara-0.5.3.tar", max compression
+gzip compressed data, was "sakkara-0.6.0.tar", max compression
```

## Comparing `sakkara-0.5.3.tar` & `sakkara-0.6.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     1082 2023-03-07 10:34:12.072457 sakkara-0.5.3/LICENSE
--rw-r--r--   0        0        0      590 2023-03-17 13:43:09.343582 sakkara-0.5.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-07 10:34:12.334926 sakkara-0.5.3/sakkara/__init__.py
--rw-r--r--   0        0        0      580 2023-03-17 09:47:10.624449 sakkara-0.5.3/sakkara/model/__init__.py
--rw-r--r--   0        0        0     2988 2023-03-14 13:24:52.992273 sakkara-0.5.3/sakkara/model/base.py
--rw-r--r--   0        0        0        0 2023-03-07 10:34:12.382440 sakkara-0.5.3/sakkara/model/composable/__init__.py
--rw-r--r--   0        0        0     2451 2023-03-17 09:47:10.624449 sakkara-0.5.3/sakkara/model/composable/base.py
--rw-r--r--   0        0        0     5101 2023-03-17 13:10:31.624195 sakkara-0.5.3/sakkara/model/composable/group.py
--rw-r--r--   0        0        0        0 2023-03-07 10:34:12.481572 sakkara-0.5.3/sakkara/model/composable/hierarchical/__init__.py
--rw-r--r--   0        0        0     2402 2023-03-17 09:47:10.624449 sakkara-0.5.3/sakkara/model/composable/hierarchical/base.py
--rw-r--r--   0        0        0     1002 2023-03-16 08:43:10.158383 sakkara-0.5.3/sakkara/model/composable/hierarchical/deterministic.py
--rw-r--r--   0        0        0     2009 2023-03-14 13:24:52.998285 sakkara-0.5.3/sakkara/model/composable/hierarchical/distribution.py
--rw-r--r--   0        0        0     2982 2023-03-14 13:24:52.999285 sakkara-0.5.3/sakkara/model/composable/hierarchical/likelihood.py
--rw-r--r--   0        0        0        0 2023-03-07 10:34:12.569428 sakkara-0.5.3/sakkara/model/fixed/__init__.py
--rw-r--r--   0        0        0     1753 2023-03-14 13:46:33.663922 sakkara-0.5.3/sakkara/model/fixed/base.py
--rw-r--r--   0        0        0     1683 2023-03-17 09:47:10.624449 sakkara-0.5.3/sakkara/model/fixed/data.py
--rw-r--r--   0        0        0        0 2023-03-17 09:47:10.624449 sakkara-0.5.3/sakkara/model/function/__init__.py
--rw-r--r--   0        0        0     5578 2023-03-17 09:47:10.624449 sakkara-0.5.3/sakkara/model/function/base.py
--rw-r--r--   0        0        0     1559 2023-03-17 09:47:10.624449 sakkara-0.5.3/sakkara/model/function/wrapper.py
--rw-r--r--   0        0        0     1377 2023-03-17 09:47:10.624449 sakkara-0.5.3/sakkara/model/math_op.py
--rw-r--r--   0        0        0     1156 2023-03-14 08:13:04.119000 sakkara-0.5.3/sakkara/model/utils.py
--rw-r--r--   0        0        0        8 2023-03-07 10:34:12.642766 sakkara-0.5.3/sakkara/relation/__init__.py
--rw-r--r--   0        0        0     1821 2023-03-15 10:20:31.774809 sakkara-0.5.3/sakkara/relation/group.py
--rw-r--r--   0        0        0     3522 2023-03-09 13:34:12.016925 sakkara-0.5.3/sakkara/relation/groupset.py
--rw-r--r--   0        0        0    11252 2023-03-17 09:47:10.624449 sakkara-0.5.3/sakkara/relation/representation.py
--rw-r--r--   0        0        0      505 1970-01-01 00:00:00.000000 sakkara-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-03-07 10:34:12.072457 sakkara-0.6.0/LICENSE
+-rw-r--r--   0        0        0      586 2023-05-09 13:13:23.637756 sakkara-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-07 10:34:12.334926 sakkara-0.6.0/sakkara/__init__.py
+-rw-r--r--   0        0        0      601 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/__init__.py
+-rw-r--r--   0        0        0     3226 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/base.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:34:12.382440 sakkara-0.6.0/sakkara/model/composable/__init__.py
+-rw-r--r--   0        0        0     2647 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/composable/base.py
+-rw-r--r--   0        0        0     5101 2023-04-26 14:01:04.108397 sakkara-0.6.0/sakkara/model/composable/group.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:34:12.481572 sakkara-0.6.0/sakkara/model/composable/hierarchical/__init__.py
+-rw-r--r--   0        0        0     2402 2023-03-17 09:47:10.624449 sakkara-0.6.0/sakkara/model/composable/hierarchical/base.py
+-rw-r--r--   0        0        0     1002 2023-03-16 08:43:10.158383 sakkara-0.6.0/sakkara/model/composable/hierarchical/deterministic.py
+-rw-r--r--   0        0        0     2009 2023-03-14 13:24:52.998285 sakkara-0.6.0/sakkara/model/composable/hierarchical/distribution.py
+-rw-r--r--   0        0        0     4337 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/composable/hierarchical/likelihood.py
+-rw-r--r--   0        0        0        0 2023-03-07 10:34:12.569428 sakkara-0.6.0/sakkara/model/fixed/__init__.py
+-rw-r--r--   0        0        0     1871 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/fixed/base.py
+-rw-r--r--   0        0        0     2123 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/fixed/data.py
+-rw-r--r--   0        0        0        0 2023-03-17 09:47:10.624449 sakkara-0.6.0/sakkara/model/function/__init__.py
+-rw-r--r--   0        0        0     6629 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/function/base.py
+-rw-r--r--   0        0        0     1559 2023-03-17 09:47:10.624449 sakkara-0.6.0/sakkara/model/function/wrapper.py
+-rw-r--r--   0        0        0     2043 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/math_op.py
+-rw-r--r--   0        0        0     1940 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/model/minibatch.py
+-rw-r--r--   0        0        0     1156 2023-03-14 08:13:04.119000 sakkara-0.6.0/sakkara/model/utils.py
+-rw-r--r--   0        0        0        8 2023-03-07 10:34:12.642766 sakkara-0.6.0/sakkara/relation/__init__.py
+-rw-r--r--   0        0        0     2389 2023-05-09 13:13:23.637756 sakkara-0.6.0/sakkara/relation/group.py
+-rw-r--r--   0        0        0     3522 2023-05-04 08:07:35.496801 sakkara-0.6.0/sakkara/relation/groupset.py
+-rw-r--r--   0        0        0    11252 2023-05-04 06:57:24.906801 sakkara-0.6.0/sakkara/relation/representation.py
+-rw-r--r--   0        0        0      497 1970-01-01 00:00:00.000000 sakkara-0.6.0/PKG-INFO
```

### Comparing `sakkara-0.5.3/LICENSE` & `sakkara-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sakkara-0.5.3/pyproject.toml` & `sakkara-0.6.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "sakkara"
-version = "0.5.3"
+version = "0.6.0"
 description = "Tools for simplified creation of PyMC models"
 authors = ["Henrik Håkansson <henrik.hakansson@fcc.chalmers.se>", "Anders Sjöberg <anders.sjoberg@fcc.chalmers.se>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pymc = "^5.0.0"
+pymc = "^5"
 numpy = "^1.23"
 pandas = "^1.4"
 pytensor = "^2.9.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
```

### Comparing `sakkara-0.5.3/sakkara/model/base.py` & `sakkara-0.6.0/sakkara/model/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,21 @@
         Build the group of this component, performed after prebuild.
 
         :param groupset: Groups to be used for building all components of the model.
 
         """
         raise NotImplementedError
 
+    @abc.abstractmethod
+    def to_minibatch(self, batch_size: int, group: str) -> 'ModelComponent':
+        """
+        Convert the component to counterpart suitable for mini-batches
+        """
+        raise NotImplementedError
+
     def build(self, groupset: GroupSet) -> None:
         """
         Method to call for building variables from the component. Will chronological order call
         :meth:`ModelComponent.prebuild`, :meth:`ModelComponent.build_representation`, and
         :meth:`ModelComponent.build_variable`
         """
         self.prebuild(groupset)
```

### Comparing `sakkara-0.5.3/sakkara/model/composable/base.py` & `sakkara-0.6.0/sakkara/model/composable/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import abc
 from abc import ABC
 from functools import cache
 from typing import Generic, Optional, Union, Tuple, Any, Dict, Set, TypeVar
 
 from sakkara.model.base import ModelComponent
+from sakkara.model.minibatch import MinibatchComponent
 from sakkara.model.math_op import MathOpBase
 from sakkara.relation.groupset import GroupSet
 
 S = TypeVar('S', bound=Any)
 T = TypeVar('T', bound=ModelComponent)
 
 
@@ -40,14 +41,17 @@
         self.base_representation = None
         self.components_representation = None
 
     @abc.abstractmethod
     def __getitem__(self, item: Any) -> T:
         raise NotImplementedError
 
+    def to_minibatch(self, batch_size: int, group: str) -> 'ModelComponent':
+        return MinibatchComponent(self, batch_size, group)
+
     def get_name(self) -> Optional[str]:
         return self.name
 
     def set_name(self, name: str) -> None:
         self.name = name
 
     def build_components(self, groupset: GroupSet) -> None:
```

### Comparing `sakkara-0.5.3/sakkara/model/composable/group.py` & `sakkara-0.6.0/sakkara/model/composable/group.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.5.3/sakkara/model/composable/hierarchical/base.py` & `sakkara-0.6.0/sakkara/model/composable/hierarchical/base.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.5.3/sakkara/model/composable/hierarchical/deterministic.py` & `sakkara-0.6.0/sakkara/model/composable/hierarchical/deterministic.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.5.3/sakkara/model/composable/hierarchical/distribution.py` & `sakkara-0.6.0/sakkara/model/composable/hierarchical/distribution.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.5.3/sakkara/model/fixed/base.py` & `sakkara-0.6.0/sakkara/model/fixed/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from abc import ABC
 from copy import deepcopy
 from typing import Any, Union, Tuple, Optional, Set
 
-import numpy as np
-
+from sakkara.model.base import ModelComponent
 from sakkara.model.math_op import MathOpBase
 from sakkara.relation.groupset import GroupSet
 
 from sakkara.relation.representation import UnrepeatableRepresentation
 
 
 class FixedValueComponent(MathOpBase, ABC):
@@ -25,33 +24,37 @@
         self.group = (group,) if isinstance(group, str) else group
         self.name = name
         self.values = value
 
     def set_name(self, name: str) -> None:
         self.name = name
 
-    def get_name(self) -> Optional[str]:
-        return self.name if self.name is not None else 'fixed'
-
     def clear(self):
         self.variable = None
         self.representation = None
 
     def prebuild(self, groupset: GroupSet) -> None:
         pass
 
-    def build_variable(self) -> None:
-        self.variable = deepcopy(self.values)
-
     def retrieve_groups(self) -> Set[str]:
         return set(self.group)
 
 
 class UnrepeatableComponent(FixedValueComponent, ABC):
     """
     Class for components that are fixed and cannot be repeated
     """
+
     def __init__(self, value: Any):
         super().__init__(value, 'global')
 
     def build_representation(self, groupset: GroupSet) -> None:
         self.representation = UnrepeatableRepresentation()
+
+    def get_name(self) -> Optional[str]:
+        return self.name if self.name is not None else 'fixed'
+
+    def build_variable(self) -> None:
+        self.variable = self.values
+
+    def to_minibatch(self, batch_size: int, group: str) -> 'ModelComponent':
+        return self
```

### Comparing `sakkara-0.5.3/sakkara/model/fixed/data.py` & `sakkara-0.6.0/sakkara/model/fixed/data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from abc import ABC
-from typing import Dict, Union, Tuple
+from typing import Dict, Union, Tuple, Optional
 
 import pandas as pd
 import numpy as np
 import numpy.typing as npt
+import pymc as pm
 
+from sakkara.model.base import ModelComponent
 from sakkara.model.fixed.base import FixedValueComponent
+from sakkara.model.minibatch import MinibatchComponent
 from sakkara.relation.groupset import GroupSet
 from sakkara.relation.representation import MinimalTensorRepresentation
 
 
 class DataComponent(FixedValueComponent, ABC):
     """
     Wrap data into a component
@@ -22,19 +25,28 @@
 
     def __init__(self, data: Union[npt.NDArray, float, int], group: Union[str, Tuple[str, ...]], name: str = None):
         if isinstance(data, np.ndarray):
             super().__init__(data, group, name)
         else:
             super().__init__(np.array([data]), group, name)
 
+    def get_name(self) -> Optional[str]:
+        return self.name
+
     def build_representation(self, groupset: GroupSet) -> None:
         self.representation = MinimalTensorRepresentation()
         for g in self.group:
             self.representation.add_group(groupset[g])
 
+    def build_variable(self) -> None:
+        self.variable = pm.Data(self.name, self.values)
+
+    def to_minibatch(self, batch_size: int, group: str) -> 'ModelComponent':
+        return MinibatchComponent(self, batch_size, group)
+
 
 def data_components(df: pd.DataFrame, group: Union[str, Tuple[str, ...]] = 'obs') -> Dict[str, DataComponent]:
     """
     Generate :class:`DataComponent` objects from a :class:`pandas.DataFrame`
 
     :param df: DataFrame to generate components from.
     :param group: Group to apply, i.e., each member of the given group corresponds to one row of the dataframe.
```

### Comparing `sakkara-0.5.3/sakkara/model/function/base.py` & `sakkara-0.6.0/sakkara/model/function/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -93,41 +93,64 @@
 
     def retrieve_groups(self) -> Set[str]:
         group = set()
         for component in chain(self.args, self.kwargs.values()):
             group = group.union(component.retrieve_groups())
         return group
 
+    def to_minibatch(self, batch_size: int, group: str) -> 'ModelComponent':
+        self.args = [m.to_minibatch(batch_size, group) for m in self.args]
+        self.kwargs = {k: v.to_minibatch(batch_size, group) for k, v in self.kwargs.items()}
+        return self
+
     @staticmethod
     def math_op(fct: Callable, left: Any, right: Any) -> ModelComponent:
         if isinstance(left, ModelComponent) and isinstance(right, ModelComponent):
             return FunctionComponent(fct, None, left, right)
         if isinstance(left, ModelComponent):
             return FunctionComponent(lambda x: fct(x, right), None, left)
         return FunctionComponent(lambda x: fct(left, x), None, right)
 
     def __add__(self, other: Any) -> ModelComponent:
-        return self.math_op(operator.add, self, other)
+        return FunctionComponent.math_op(operator.add, self, other)
 
-    def __sub__(self, other: Any) -> ModelComponent:
-        return self.math_op(operator.sub, self, other)
+    def __radd__(self, other: Any):
+        return FunctionComponent.math_op(operator.add, other, self)
 
-    def __radd__(self, other):
-        return self.math_op(operator.add, other, self)
+    def __sub__(self, other: Any) -> ModelComponent:
+        return FunctionComponent.math_op(operator.sub, self, other)
 
-    def __rsub__(self, other):
-        return self.math_op(operator.sub, other, self)
+    def __rsub__(self, other: Any):
+        return FunctionComponent.math_op(operator.sub, other, self)
 
     def __mul__(self, other: Any) -> ModelComponent:
-        return self.math_op(operator.mul, self, other)
+        return FunctionComponent.math_op(operator.mul, self, other)
 
     def __rmul__(self, other: Any) -> ModelComponent:
-        return self.math_op(operator.add, other, self)
+        return FunctionComponent.math_op(operator.mul, other, self)
+
+    def __pow__(self, power, modulo=None):
+        return FunctionComponent.math_op(operator.pow, self, power)
+
+    def __rpow__(self, other, modulo=None):
+        return FunctionComponent.math_op(operator.pow, other, self)
+
+    def __mod__(self, other):
+        return FunctionComponent.math_op(operator.mod, self, other)
+
+    def __rmod__(self, other):
+        return FunctionComponent.math_op(operator.mod, other, self)
+
+    def __floordiv__(self, other: Any):
+        return FunctionComponent.math_op(operator.floordiv, self, other)
+
+    def __rfloordiv__(self, other):
+        return FunctionComponent.math_op(operator.floordiv, other, self)
 
     def __truediv__(self, other: Any) -> ModelComponent:
-        return self.math_op(operator.truediv, self, other)
+        return FunctionComponent.math_op(operator.truediv, self, other)
 
     def __rtruediv__(self, other: Any):
-        return self.math_op(operator.truediv, other, self)
+        return FunctionComponent.math_op(operator.truediv, other, self)
 
     def __neg__(self):
         return FunctionComponent(operator.neg, None, self)
```

### Comparing `sakkara-0.5.3/sakkara/model/function/wrapper.py` & `sakkara-0.6.0/sakkara/model/function/wrapper.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.5.3/sakkara/model/utils.py` & `sakkara-0.6.0/sakkara/model/utils.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.5.3/sakkara/relation/group.py` & `sakkara-0.6.0/sakkara/relation/group.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from typing import Set, Any, Tuple, Callable, Union, List
+from typing import Any
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
+import pytensor as pt
+from pymc.data import minibatch_index
 
 
 class Group:
     """
     Class corresponding to a data frame column, with capabilities of handling relations to other groups.
 
     :param name: Name of the group, should be same as the column
@@ -15,14 +17,15 @@
     def __init__(self, name: str, members: npt.NDArray[Any]):
         self.name = name
         self.members = members
         self.parents = set()
         self.children = set()
         self.twins = {self}
         self.mapping = pd.DataFrame(index=members, data={name: np.arange(len(members))})
+        self.minibatch = None
 
     def add_child(self, child: 'Group') -> None:
         """
         Add a child relation to this group
 
         :param child: The child group
         """
@@ -44,14 +47,29 @@
         Add a twin relation to this group
 
         :param twin: The twin group
         """
         self.twins.add(twin)
         self.mapping[twin.name] = np.arange(len(self.mapping))
 
+    def get_minibatch(self, batch_size) -> pt.tensor.TensorVariable:
+        """
+        Get a PyMC minibatch variable created from this group. Creates a new instance if not already created.
+        """
+        if self.minibatch is None:
+            self.minibatch = minibatch_index(0, len(self), size=(batch_size,))
+        return self.minibatch
+
+    def clear_minibatch(self) -> None:
+        """
+        Reset the minibatch variable of this group.
+        """
+        self.minibatch = None
+
+
     def __str__(self):
         return self.name
 
     def __len__(self):
         return len(self.mapping)
 
     def __lt__(self, other) -> bool:
```

### Comparing `sakkara-0.5.3/sakkara/relation/groupset.py` & `sakkara-0.6.0/sakkara/relation/groupset.py`

 * *Files identical despite different names*

### Comparing `sakkara-0.5.3/sakkara/relation/representation.py` & `sakkara-0.6.0/sakkara/relation/representation.py`

 * *Files identical despite different names*

