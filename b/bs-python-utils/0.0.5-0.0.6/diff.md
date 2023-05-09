# Comparing `tmp/bs_python_utils-0.0.5.tar.gz` & `tmp/bs_python_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bs_python_utils-0.0.5.tar", max compression
+gzip compressed data, was "bs_python_utils-0.0.6.tar", max compression
```

## Comparing `bs_python_utils-0.0.5.tar` & `bs_python_utils-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.0.5/LICENSE
--rw-r--r--   0        0        0     1371 2023-05-08 18:46:21.795283 bs_python_utils-0.0.5/README.md
--rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.0.5/bs_python_utils/Timer.py
--rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.0.5/bs_python_utils/__init__.py
--rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.859499 bs_python_utils-0.0.5/bs_python_utils/bs_altair.py
--rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.0.5/bs_python_utils/bs_logging.py
--rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.0.5/bs_python_utils/bs_mathstr.py
--rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.0.5/bs_python_utils/bs_mem.py
--rw-r--r--   0        0        0    13696 2023-04-24 22:48:26.403984 bs_python_utils-0.0.5/bs_python_utils/bs_opt.py
--rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.0.5/bs_python_utils/bs_plots.py
--rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.0.5/bs_python_utils/bs_seaborn.py
--rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.302214 bs_python_utils-0.0.5/bs_python_utils/bs_sparse_gaussian.py
--rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.0.5/bs_python_utils/bsmplutils.py
--rw-r--r--   0        0        0    31781 2023-05-02 17:31:44.506884 bs_python_utils-0.0.5/bs_python_utils/bsnputils.py
--rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.0.5/bs_python_utils/bssputils.py
--rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.0.5/bs_python_utils/bsstats.py
--rw-r--r--   0        0        0     9471 2023-05-08 18:43:13.753098 bs_python_utils-0.0.5/bs_python_utils/bsutils.py
--rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.0.5/bs_python_utils/distance_covariances.py
--rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.733299 bs_python_utils-0.0.5/bs_python_utils/example_opt.py
--rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.344134 bs_python_utils-0.0.5/bs_python_utils/examples_altair.py
--rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.733372 bs_python_utils-0.0.5/bs_python_utils/examples_distance_covariances.py
--rw-r--r--   0        0        0      552 2023-04-24 22:36:28.733335 bs_python_utils-0.0.5/bs_python_utils/examples_mem.py
--rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.0.5/bs_python_utils/examples_seaborn.py
--rw-r--r--   0        0        0      786 2023-04-24 22:36:28.733292 bs_python_utils-0.0.5/bs_python_utils/examples_sklearn.py
--rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.0.5/bs_python_utils/pandas_utils.py
--rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.0.5/bs_python_utils/sklearn_utils.py
--rw-r--r--   0        0        0     1871 2023-05-08 18:45:42.703018 bs_python_utils-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 bs_python_utils-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-21 14:06:07.415664 bs_python_utils-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1414 2023-05-09 18:12:28.311148 bs_python_utils-0.0.6/README.md
+-rw-r--r--   0        0        0     1799 2023-04-24 19:42:58.427840 bs_python_utils-0.0.6/bs_python_utils/Timer.py
+-rw-r--r--   0        0        0        0 2023-04-24 19:42:58.429294 bs_python_utils-0.0.6/bs_python_utils/__init__.py
+-rw-r--r--   0        0        0    28473 2023-04-24 22:57:44.859499 bs_python_utils-0.0.6/bs_python_utils/bs_altair.py
+-rw-r--r--   0        0        0     2976 2023-04-24 20:25:24.489951 bs_python_utils-0.0.6/bs_python_utils/bs_logging.py
+-rw-r--r--   0        0        0     3577 2023-04-24 19:42:58.433666 bs_python_utils-0.0.6/bs_python_utils/bs_mathstr.py
+-rw-r--r--   0        0        0     4338 2023-04-24 21:45:53.142922 bs_python_utils-0.0.6/bs_python_utils/bs_mem.py
+-rw-r--r--   0        0        0    13696 2023-04-24 22:48:26.403984 bs_python_utils-0.0.6/bs_python_utils/bs_opt.py
+-rw-r--r--   0        0        0       36 2023-04-24 19:42:58.438686 bs_python_utils-0.0.6/bs_python_utils/bs_plots.py
+-rw-r--r--   0        0        0     4507 2023-04-24 20:32:13.556809 bs_python_utils-0.0.6/bs_python_utils/bs_seaborn.py
+-rw-r--r--   0        0        0     1391 2023-04-24 22:48:26.302214 bs_python_utils-0.0.6/bs_python_utils/bs_sparse_gaussian.py
+-rw-r--r--   0        0        0      905 2023-04-24 19:42:58.441367 bs_python_utils-0.0.6/bs_python_utils/bsmplutils.py
+-rw-r--r--   0        0        0    31244 2023-05-09 18:04:48.974809 bs_python_utils-0.0.6/bs_python_utils/bsnputils.py
+-rw-r--r--   0        0        0     2132 2023-04-24 20:25:24.253141 bs_python_utils-0.0.6/bs_python_utils/bssputils.py
+-rw-r--r--   0        0        0    15489 2023-04-24 20:25:24.644930 bs_python_utils-0.0.6/bs_python_utils/bsstats.py
+-rw-r--r--   0        0        0     9471 2023-05-08 18:43:13.753098 bs_python_utils-0.0.6/bs_python_utils/bsutils.py
+-rw-r--r--   0        0        0     7801 2023-04-24 21:45:53.165270 bs_python_utils-0.0.6/bs_python_utils/distance_covariances.py
+-rw-r--r--   0        0        0     1350 2023-04-24 22:36:28.733299 bs_python_utils-0.0.6/bs_python_utils/example_opt.py
+-rw-r--r--   0        0        0     3833 2023-04-24 22:48:26.344134 bs_python_utils-0.0.6/bs_python_utils/examples_altair.py
+-rw-r--r--   0        0        0     1013 2023-04-24 22:36:28.733372 bs_python_utils-0.0.6/bs_python_utils/examples_distance_covariances.py
+-rw-r--r--   0        0        0      552 2023-04-24 22:36:28.733335 bs_python_utils-0.0.6/bs_python_utils/examples_mem.py
+-rw-r--r--   0        0        0      771 2023-04-24 21:45:53.146924 bs_python_utils-0.0.6/bs_python_utils/examples_seaborn.py
+-rw-r--r--   0        0        0      786 2023-04-24 22:36:28.733292 bs_python_utils-0.0.6/bs_python_utils/examples_sklearn.py
+-rw-r--r--   0        0        0     7426 2023-04-24 20:25:24.576148 bs_python_utils-0.0.6/bs_python_utils/pandas_utils.py
+-rw-r--r--   0        0        0     1872 2023-04-24 21:46:50.361114 bs_python_utils-0.0.6/bs_python_utils/sklearn_utils.py
+-rw-r--r--   0        0        0     1871 2023-05-09 18:13:15.166890 bs_python_utils-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2386 1970-01-01 00:00:00.000000 bs_python_utils-0.0.6/PKG-INFO
```

### Comparing `bs_python_utils-0.0.5/LICENSE` & `bs_python_utils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/README.md` & `bs_python_utils-0.0.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,19 @@
 My Python utilities.
 
 -   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 -   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
 
+
+#### 0.0.6 (May 9, 2023)
+
+Improved docs.
+
 #### 0.0.5 (May 8, 2023)
 
 Added `final_s` in `bsutils`.
 
 #### 0.0.4 (May 2, 2023)
 
 Added Legendre polynomials and quantile routines in `bsnputils`.
```

### Comparing `bs_python_utils-0.0.5/bs_python_utils/Timer.py` & `bs_python_utils-0.0.6/bs_python_utils/Timer.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/bs_altair.py` & `bs_python_utils-0.0.6/bs_python_utils/bs_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/bs_logging.py` & `bs_python_utils-0.0.6/bs_python_utils/bs_logging.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/bs_mathstr.py` & `bs_python_utils-0.0.6/bs_python_utils/bs_mathstr.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/bs_mem.py` & `bs_python_utils-0.0.6/bs_python_utils/bs_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/bs_opt.py` & `bs_python_utils-0.0.6/bs_python_utils/bs_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/bs_seaborn.py` & `bs_python_utils-0.0.6/bs_python_utils/bs_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/bs_sparse_gaussian.py` & `bs_python_utils-0.0.6/bs_python_utils/bs_sparse_gaussian.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/bsmplutils.py` & `bs_python_utils-0.0.6/bs_python_utils/bsmplutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/bsnputils.py` & `bs_python_utils-0.0.6/bs_python_utils/bsnputils.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,123 @@
 ThreeArrays = tuple[np.ndarray, np.ndarray, np.ndarray]
 FourArrays = tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]
 SixArrays = tuple[
     np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray
 ]
 
 
+def check_vector(v: Any, fun_name: str = None) -> int:
+    """
+    test that `v` is a vector; aborts otherwise
+
+    Args:
+        v: a vector, we hope
+        fun_name: name of the calling function
+
+    Returns:
+        the size if successful
+    """
+    fun_str = ["" if fun_name is None else fun_name + ":"]
+    if not isinstance(v, np.ndarray):
+        bs_error_abort(f"{fun_str} v should be a Numpy array")
+    v = cast(np.ndarray, v)
+    ndims_v = v.ndim
+    if ndims_v != 1:
+        bs_error_abort(f"{fun_str} v should have one dimension, not {ndims_v}")
+    return cast(int, v.size)
+
+
+def check_matrix(x: Any, fun_name: str = None) -> tuple[int, int]:
+    """
+    test that `x` is a matrix; aborts otherwise
+
+    Args:
+        x: a matrix, we hope
+        fun_name: name of the calling function
+
+    Returns:
+        the shape if successful
+    """
+    fun_str = ["" if fun_name is None else fun_name + ":"]
+    if not isinstance(x, np.ndarray):
+        bs_error_abort(f"{fun_str} Xx should be a Numpy array")
+    x = cast(np.ndarray, x)
+    ndims_x = x.ndim
+    if ndims_x != 2:
+        bs_error_abort(f"{fun_str} x should have two dimensions, not {ndims_x}")
+    return cast(tuple[int, int], x.shape)
+
+
+def check_vector_or_matrix(x: Any, fun_name: str = None) -> int:
+    """
+    test that `x` is a vector or a matrix; aborts otherwise
+
+    Args:
+        x: a vector or matrix, we hope
+        fun_name: name of the calling function
+
+    Returns:
+        the number of dimensions of `x` (1 or 2)
+    """
+    fun_str = ["" if fun_name is None else fun_name + ":"]
+    if not isinstance(x, np.ndarray):
+        bs_error_abort(f"{fun_str} X should be a Numpy array")
+    x = cast(np.ndarray, x)
+    ndims_x = x.ndim
+    if ndims_x != 1 and ndims_x != 2:
+        bs_error_abort(f"{fun_str} x should have at most two dimensions, not {ndims_x}")
+    return cast(int, ndims_x)
+
+
+def check_square(A: Any, fun_name: str = None) -> int:
+    """
+    test that an object used in `fun_name` is a square matrix
+
+    Args:
+        A: square matrix, we hope
+        fun_name: the name of the calling function
+
+    Returns:
+        the number of rows and columns of `A`
+    """
+    fun_str = ["" if fun_name is None else fun_name + ":"]
+    if not isinstance(A, np.ndarray):
+        bs_error_abort(f"{fun_str} A should be a Numpy array")
+    A = cast(np.ndarray, A)
+    if A.ndim == 2:
+        n, nv = A.shape
+        if nv != n:
+            bs_error_abort(f"{fun_str} The matrix A should be square, not {A.shape}")
+    else:
+        bs_error_abort(f"{fun_name} A should have  two dimensions, not {A.ndim}")
+    return cast(int, n)
+
+
+def check_tensor(x: Any, n_dims: int, fun_name: str = None) -> tuple[int, ...]:
+    """
+    test that `x` is an `n_dims` dimensional array; aborts otherwise
+
+    Args:
+        x: an `n_dims` dimensional array, we hope
+        fun_name: name of the calling function
+
+    Returns:
+        the shape if successful
+    """
+    fun_str = ["" if fun_name is None else fun_name + ":"]
+    if not isinstance(x, np.ndarray):
+        bs_error_abort(f"{fun_str} x should be a Numpy array")
+    x = cast(np.ndarray, x)
+    ndims_x = x.ndim
+    if ndims_x != n_dims:
+        bs_error_abort(f"{fun_str} x should have {n_dims} dimensions, not {ndims_x}")
+        return (0,)  # for mypy
+    return cast(tuple[int, ...], x.shape)
+
+
 # Numpy parallel RNG
 def generate_RNG_streams(
     nsim: int, initial_seed: int = 13091962
 ) -> list[np.random.Generator]:
     """
     return `nsim` RNGs
 
@@ -200,24 +309,24 @@
 def nplog(
     arr: np.ndarray,
     eps: float = 1e-30,
     deriv: int = 0,
     verbose: bool = False,
 ) -> np.ndarray | TwoArrays | ThreeArrays:
     """
-    `C^2` extension of  `\\ln(a)` below `eps`, perhaps with derivatives
+    $C^2$ extension of  $\\ln(a)$ below `eps`, perhaps with derivatives
 
     Args:
         arr: any Numpy array
         eps: lower bound
         deriv: if 1, compute derivative, if 2, second derivative
         verbose: prints debugging info
 
     Returns:
-        `\\ln(a)` `C^2`-extended below `eps`, perhaps with derivatives
+        $\\ln(a)$  $C^2$-extended below `eps`, perhaps with derivatives
     """
     if deriv not in [0, 1, 2]:
         bs_error_abort(f"deriv can only be 0, 1, or 2; not {deriv}")
     if np.min(arr) > eps:
         if deriv == 0:
             return cast(np.ndarray, np.log(arr))
         elif deriv == 1:
@@ -256,27 +365,27 @@
     arr: np.ndarray,
     bigx: float = 50.0,
     lowx: float = -50.0,
     deriv: int = 0,
     verbose: bool = False,
 ) -> np.ndarray | TwoArrays | ThreeArrays:
     """
-    `C^2` extension of  `\\exp(a)` above `bigx` and below `lowx`,
+    $C^2$ extension of  $\\exp(a)$ above `bigx` and below `lowx`,
     perhaps with derivatives
 
     Args:
         arr: any Numpy array
         bigx: upper bound
         lowx: lower bound
         deriv: if 1, compute derivative, if 2, second derivative
         verbose: prints debugging info
 
 
     Returns:
-        `\\exp(a)`  `C^2`-extended above `bigx` and below `lowx`,
+        $\\exp(a)$  $C^2$-extended above `bigx` and below `lowx`,
         perhaps with derivatives
     """
     if deriv not in [0, 1, 2]:
         bs_error_abort(f"deriv can only be 0, 1, or 2; not {deriv}")
     min_arr, max_arr = np.min(arr), np.max(arr)
     if max_arr <= bigx and min_arr >= lowx:
         exparr = np.exp(arr)
@@ -479,89 +588,14 @@
     m = check_vector(v)
     n = check_vector(w)
     m, n = v.size, w.size
     v1 = np.repeat(v, n)
     v2 = np.tile(w, m)
     return np.column_stack((v1, v2))
 
-    """
-    This is a Python function that tests whether a given input is a vector and returns its size if
-    successful.
-    
-    :param v: `v` is a numpy array that is expected to be a vector
-    :type v: np.ndarray
-    :param fun_name: `fun_name` is an optional parameter that represents the name of the calling
-    function. If provided, it will be used in error messages to indicate which function caused the
-    error. If not provided, the error message will not include the function name
-    :type fun_name: Optional[str]
-    """
-
-
-def check_vector(v: Any, fun_name: str = None) -> int:
-    """
-    test that `v` is a vector; aborts otherwise
-
-    Args:
-        v: a vector, we hope
-        fun_name: name of the calling function
-
-    Returns:
-        the size if successful
-    """
-    fun_str = ["" if fun_name is None else fun_name + ":"]
-    if not isinstance(v, np.ndarray):
-        bs_error_abort(f"{fun_str} v should be a Numpy array")
-    v = cast(np.ndarray, v)
-    ndims_v = v.ndim
-    if ndims_v != 1:
-        bs_error_abort(f"{fun_str} v should have one dimension, not {ndims_v}")
-    return cast(int, v.size)
-
-
-def check_matrix(x: Any, fun_name: str = None) -> tuple[int, int]:
-    """
-    test that `x` is a matrix; aborts otherwise
-
-    Args:
-        x: a matrix, we hope
-        fun_name: name of the calling function
-
-    Returns:
-        the shape if successful
-    """
-    fun_str = ["" if fun_name is None else fun_name + ":"]
-    if not isinstance(x, np.ndarray):
-        bs_error_abort(f"{fun_str} Xx should be a Numpy array")
-    x = cast(np.ndarray, x)
-    ndims_x = x.ndim
-    if ndims_x != 2:
-        bs_error_abort(f"{fun_str} x should have two dimensions, not {ndims_x}")
-    return cast(tuple[int, int], x.shape)
-
-
-def check_vector_or_matrix(x: Any, fun_name: str = None) -> int:
-    """
-    test that `x` is a vector or a matrix; aborts otherwise
-
-    Args:
-        x: a vector or matrix, we hope
-        fun_name: name of the calling function
-
-    Returns:
-        the number of dimensions of `x` (1 or 2)
-    """
-    fun_str = ["" if fun_name is None else fun_name + ":"]
-    if not isinstance(x, np.ndarray):
-        bs_error_abort(f"{fun_str} X should be a Numpy array")
-    x = cast(np.ndarray, x)
-    ndims_x = x.ndim
-    if ndims_x != 1 and ndims_x != 2:
-        bs_error_abort(f"{fun_str} x should have at most two dimensions, not {ndims_x}")
-    return cast(int, ndims_x)
-
 
 def bs_sqrt_pdmatrix(m: np.ndarray) -> np.ndarray:
     """
     square root of a positive definite matrix
 
     Args:
         m: a positive definite matrix
@@ -574,60 +608,14 @@
     eigval = np.maximum(eigval, 0.0)
     eigval_sqrt = np.sqrt(eigval)
     eigval_sqrt_diag = np.diag(eigval_sqrt)
     res = eigvec @ eigval_sqrt_diag @ eigvec.T
     return cast(np.ndarray, res)
 
 
-def check_square(A: Any, fun_name: str | None) -> int:
-    """
-    test that an object used in `fun_name` is a square matrix
-
-    Args:
-        A: square matrix, we hope
-        fun_name: the name of the calling function
-
-    Returns:
-        the number of rows and columns of `A`
-    """
-    fun_str = ["" if fun_name is None else fun_name + ":"]
-    if not isinstance(A, np.ndarray):
-        bs_error_abort(f"{fun_str} A should be a Numpy array")
-    A = cast(np.ndarray, A)
-    if A.ndim == 2:
-        n, nv = A.shape
-        if nv != n:
-            bs_error_abort(f"{fun_str} The matrix A should be square, not {A.shape}")
-    else:
-        bs_error_abort(f"{fun_name} A should have  two dimensions, not {A.ndim}")
-    return cast(int, n)
-
-
-def check_tensor(x: Any, n_dims: int, fun_name: str | None) -> tuple[int, ...]:
-    """
-    test that `x` is an `n_dims` dimensional array; aborts otherwise
-
-    Args:
-        x: an `n_dims` dimensional array, we hope
-        fun_name: name of the calling function
-
-    Returns:
-        the shape if successful
-    """
-    fun_str = ["" if fun_name is None else fun_name + ":"]
-    if not isinstance(x, np.ndarray):
-        bs_error_abort(f"{fun_str} x should be a Numpy array")
-    x = cast(np.ndarray, x)
-    ndims_x = x.ndim
-    if ndims_x != n_dims:
-        bs_error_abort(f"{fun_str} x should have {n_dims} dimensions, not {ndims_x}")
-        return (0,)  # for mypy
-    return cast(tuple[int, ...], x.shape)
-
-
 def make_lexico_grid(arr: np.ndarray) -> np.ndarray:
     """
     make a lexicographic grid
 
     Args:
         arr: `nr`-vector or `(nr,nc)` matrix; `nc` must be 1, 2 or 3
 
@@ -766,24 +754,24 @@
 def npxlogx(
     arr: np.ndarray,
     eps: float = 1e-30,
     deriv: int = 0,
     verbose: bool = False,
 ) -> np.ndarray | TwoArrays | ThreeArrays:
     """
-    C^2` extension of  `a\\ln(a)` below `eps`, perhaps with derivatives
+    $C^2$ extension of  $a\\ln(a)$ below `eps`, perhaps with derivatives
 
     Args:
         arr: a Numpy array
         eps: lower bound
         deriv: if 1, compute derivative, if 2, second derivative
         verbose: prints debugging info
 
     Returns:
-        `a\\ln(a)`  `C^2`-extended  below `eps`, perhaps with derivatives
+        $a\\ln(a)$  $C^2$-extended  below `eps`, perhaps with derivatives
     """
     if deriv not in [0, 1, 2]:
         bs_error_abort(f"deriv must be 0, 1, or 2; not {deriv}")
     if np.min(arr) > eps:
         return cast(np.ndarray, arr * np.log(arr))
     else:
         logeps = log(eps)
```

### Comparing `bs_python_utils-0.0.5/bs_python_utils/bssputils.py` & `bs_python_utils-0.0.6/bs_python_utils/bssputils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/bsstats.py` & `bs_python_utils-0.0.6/bs_python_utils/bsstats.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/bsutils.py` & `bs_python_utils-0.0.6/bs_python_utils/bsutils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/distance_covariances.py` & `bs_python_utils-0.0.6/bs_python_utils/distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/example_opt.py` & `bs_python_utils-0.0.6/bs_python_utils/example_opt.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/examples_altair.py` & `bs_python_utils-0.0.6/bs_python_utils/examples_altair.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/examples_distance_covariances.py` & `bs_python_utils-0.0.6/bs_python_utils/examples_distance_covariances.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/examples_mem.py` & `bs_python_utils-0.0.6/bs_python_utils/examples_mem.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/examples_seaborn.py` & `bs_python_utils-0.0.6/bs_python_utils/examples_seaborn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/examples_sklearn.py` & `bs_python_utils-0.0.6/bs_python_utils/examples_sklearn.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/pandas_utils.py` & `bs_python_utils-0.0.6/bs_python_utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/bs_python_utils/sklearn_utils.py` & `bs_python_utils-0.0.6/bs_python_utils/sklearn_utils.py`

 * *Files identical despite different names*

### Comparing `bs_python_utils-0.0.5/pyproject.toml` & `bs_python_utils-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bs_python_utils"
-version = "0.0.5"
+version = "0.0.6"
 description = "my Python utilities"
 authors = ["Bernard Salanie <fbsalanie@columbia.edu>"]
 repository = "https://github.com/bsalanie/bs-python-utils"
 documentation = "https://bsalanie.github.io/bs-python-utils/"
 readme = "README.md"
 packages = [
   {include = "bs_python_utils"}
```

### Comparing `bs_python_utils-0.0.5/PKG-INFO` & `bs_python_utils-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bs-python-utils
-Version: 0.0.5
+Version: 0.0.6
 Summary: my Python utilities
 Home-page: https://github.com/bsalanie/bs-python-utils
 Author: Bernard Salanie
 Author-email: fbsalanie@columbia.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -33,14 +33,19 @@
 My Python utilities.
 
 -   **Github repository**: <https://github.com/bsalanie/bs-python-utils/>
 -   **Documentation** <https://bsalanie.github.io/bs-python-utils/>
 
 ### Release notes
 
+
+#### 0.0.6 (May 9, 2023)
+
+Improved docs.
+
 #### 0.0.5 (May 8, 2023)
 
 Added `final_s` in `bsutils`.
 
 #### 0.0.4 (May 2, 2023)
 
 Added Legendre polynomials and quantile routines in `bsnputils`.
```

