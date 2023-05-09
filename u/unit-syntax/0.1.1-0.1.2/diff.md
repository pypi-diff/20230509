# Comparing `tmp/unit_syntax-0.1.1.tar.gz` & `tmp/unit_syntax-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unit_syntax-0.1.1.tar", max compression
+gzip compressed data, was "unit_syntax-0.1.2.tar", max compression
```

## Comparing `unit_syntax-0.1.1.tar` & `unit_syntax-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     5212 2023-05-02 04:55:17.995066 unit_syntax-0.1.1/README.md
--rw-r--r--   0        0        0      641 2023-05-02 04:55:17.995066 unit_syntax-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      689 2023-05-02 04:55:17.995066 unit_syntax-0.1.1/unit_syntax/__init__.py
--rw-r--r--   0        0        0   149012 2023-05-02 04:55:17.995066 unit_syntax-0.1.1/unit_syntax/parser.py
--rw-r--r--   0        0        0     4608 2023-05-02 04:55:17.995066 unit_syntax-0.1.1/unit_syntax/transform.py
--rw-r--r--   0        0        0     5895 1970-01-01 00:00:00.000000 unit_syntax-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     5227 2023-05-09 21:09:01.462892 unit_syntax-0.1.2/README.md
+-rw-r--r--   0        0        0      641 2023-05-09 21:09:01.466893 unit_syntax-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      689 2023-05-09 21:09:01.466893 unit_syntax-0.1.2/unit_syntax/__init__.py
+-rw-r--r--   0        0        0   149332 2023-05-09 21:09:01.466893 unit_syntax-0.1.2/unit_syntax/parser.py
+-rw-r--r--   0        0        0     4608 2023-05-09 21:09:01.466893 unit_syntax-0.1.2/unit_syntax/transform.py
+-rw-r--r--   0        0        0     5910 1970-01-01 00:00:00.000000 unit_syntax-0.1.2/PKG-INFO
```

### Comparing `unit_syntax-0.1.1/README.md` & `unit_syntax-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,29 @@
+Metadata-Version: 2.1
+Name: unit-syntax
+Version: 0.1.2
+Summary: Literal physical units for Jupyter and IPython
+Home-page: https://github.com/ahupp/unit-syntax
+Author: Adam Hupp
+Author-email: adam@hupp.org
+Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Pint (>=0.20,<0.21)
+Requires-Dist: ipython (>=7)
+Requires-Dist: pegen (>=0.2,<0.3)
+Project-URL: Repository, https://github.com/ahupp/unit-syntax
+Description-Content-Type: text/markdown
+
 `unit-syntax` extends the Python language in Jupyter/IPython to support expressions with physical units:
 
 ```python
->>> import unit_syntax.ipython
 >>> speed = 5 meters/second
 >>> 2 seconds * speed
 10 meter
 ```
 
 Behind the scenes this is translated into standard Python that uses the excellent [Pint](https://pint.readthedocs.io/) units library.
 
@@ -32,15 +50,15 @@
 
 Units apply to the preceding value (a literal, variable, function call or indexing), and have higher precedence than other operators:
 
 ```python
 x * 1.21 gigawatts
 ```
 
-This is equivalent to `x * (1.21 gigawatts)`, and desugars to something like `x * Quantity(1.21, "gigawatts")`.  The high precedence means units apply to the literal not the whole expression.
+This is equivalent to `x * (1.21 gigawatts)`, and desugars to something like `x * Quantity(1.21, "gigawatts")`. The high precedence means units apply to the literal not the whole expression.
 
 Values can be converted to another measurement system:
 
 ```python
 (88 miles / hour) furlongs / fortnight
 ```
 
@@ -48,60 +66,62 @@
 
 ```python
 velocity = [5, 7] meters/second**2
 location = velocity * 2 seconds
 distance_traveled = numpy.linalg.norm(location)
 ```
 
+## The Grammar
+
 The units term follows this grammar:
 
 ```
 units:
-    | NAME '/' units
-    | NAME '*' units
-    | NAME units
+    | NAME '/' units_group
+    | NAME '*' units_group
+    | NAME units_group
     | NAME '**' NUMBER
     | NAME
+
+units_group:
+    | '(' units ')'
+    | units
 ```
 
-## Why?  How?
+## Why? How?
 
 I like using Python+[Jupyter Notebook](https://jupyter.org/) as a calculator for physical problems and often wish it had the clarity and type checking of explicit units. [Pint](https://pint.readthedocs.io/) is great, but (IMO) its necessary verbosity makes it hard to see the underlying calculation that's going.
 
-`unit-syntax` is an IPython/Jupyter [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) that rewrites expressions with units into calls to `pint.Quantity`.
-
-This is possible without ambiguity in the python grammar because it's otherwise invalid for a "primary" (literal, function call etc) to be immediately followed by 
+`unit-syntax` is an IPython/Jupyter [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) that rewrites expressions with units into calls to `pint.Quantity`. The parser is a lightly modified version of the Python grammar using the same parser generator ([pegen](https://github.com/we-like-parsers/pegen)) as Python itself.
 
 `unit-syntax` cannot (currently) be used for standalone python scripts outside of IPython/Jupyter, but that's in principle possible through [meta_path import hooks](https://docs.python.org/3/reference/import.html#the-meta-path).
 
 The syntax takes advantage of the fact that that in python its illegal for a NAME to follow a "primary" (literal, function call etc), so there's no ambiguity.
 
-
 ## Prior Art
 
-The immediate inspriration of `unit-syntax` is a language called [Fortress](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.6323&rep=rep1&type=pdf
-) from Sun Microsystems.  Fortress was intended as a modern Fortran, and had first-class support for units in both the syntax and type system.
+The immediate inspriration of `unit-syntax` is a language called [Fortress](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.6323&rep=rep1&type=pdf) from Sun Microsystems. Fortress was intended as a modern Fortran, and had first-class support for units in both the syntax and type system.
 
 F# (an OCaml derivative from Microsoft) also [has first class support for units](https://en.wikibooks.org/wiki/F_Sharp_Programming/Units_of_Measure).
 
 The Julia package [Unitful.jl](http://painterqubits.github.io/Unitful.jl/stable/)
 
 ## Open questions and future work
 
- * Fortress uses an `in` operator to apply units to a non-literal value, e.g `x in meters`.  This has the advantage of being unambiguous regardless of parenthesization.  In python this would conflcit with `value in [a, b, c]`, but `as` is
+- Fortress uses an `in` operator to apply units to a non-literal value, e.g `x in meters`. This has the advantage of being unambiguous regardless of parenthesization. In python this would conflcit with `value in [a, b, c]`, but `as` is
 
- * Move to tree-sitter, which will be simpler and has a chance of providing syntax highlighting
- * Test against various ipython and python versions
- * Support standalone scripts through sys.meta_path
- * Check units at parse time
- * Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable).  More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
- * Pint does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
- * Demo colab notebook: https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV
- * Describe parsing ambuguity like `1 meters * sin(45 degrees)`
- * Figure out story around parenthesization
+- Move to tree-sitter, which will be simpler and has a chance of providing syntax highlighting
+- Test against various ipython and python versions
+- Support standalone scripts through sys.meta_path
+- Check units at parse time
+- Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
+- Pint does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
+- Demo colab notebook: https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV
+- Describe parsing ambuguity like `1 meters * sin(45 degrees)`
+- Figure out story around parenthesization
 
 ## Development
 
 To regenerate the parser:
 
 `python -m pegen grammar.txt -o unit_syntax/parser.py`
 
@@ -110,20 +130,18 @@
 ```
  $ poetry install --with dev
  $ poetry run pytest
 ```
 
 ## Future work and open questions
 
- * Parenthisized units expressions
- * Demo colab notebook
- * Move to tree-sitter so there's a chance of getting syntax highlighting
- * Jupyter syntax checks
- * Typography of output
- * Test against various ipython and python versions
- * Support standalone scripts through sys.meta_path
- * Check units at parse time
- * Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable).  More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166) 
- * Does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
-
+- Parenthisized units expressions
+- Demo colab notebook
+- Move to tree-sitter so there's a chance of getting syntax highlighting
+- Jupyter syntax checks
+- Typography of output
+- Test against various ipython and python versions
+- Support standalone scripts through sys.meta_path
+- Check units at parse time
+- Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
+- Does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
 
-
```

### Comparing `unit_syntax-0.1.1/unit_syntax/__init__.py` & `unit_syntax-0.1.2/unit_syntax/__init__.py`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.1.1/unit_syntax/parser.py` & `unit_syntax-0.1.2/unit_syntax/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -2273,49 +2273,40 @@
         ):
             return sum;
         self._reset(mark)
         return None;
 
     @memoize
     def units(self) -> Optional[Any]:
-        # units: '(' units ')' | NAME '/' units | NAME '*' units | NAME units | NAME '**' NUMBER | NAME
+        # units: NAME '/' units_group | NAME '*' units_group | NAME units_group | NAME '**' NUMBER | NAME
         mark = self._mark()
         if (
-            (literal := self.expect('('))
-            and
-            (units := self.units())
-            and
-            (literal_1 := self.expect(')'))
-        ):
-            return [literal, units, literal_1];
-        self._reset(mark)
-        if (
             (name := self.name())
             and
             (literal := self.expect('/'))
             and
-            (units := self.units())
+            (units_group := self.units_group())
         ):
-            return [name, literal, units];
+            return [name, literal, units_group];
         self._reset(mark)
         if (
             (name := self.name())
             and
             (literal := self.expect('*'))
             and
-            (units := self.units())
+            (units_group := self.units_group())
         ):
-            return [name, literal, units];
+            return [name, literal, units_group];
         self._reset(mark)
         if (
             (name := self.name())
             and
-            (units := self.units())
+            (units_group := self.units_group())
         ):
-            return [name, units];
+            return [name, units_group];
         self._reset(mark)
         if (
             (name := self.name())
             and
             (literal := self.expect('**'))
             and
             (number := self.number())
@@ -2325,14 +2316,34 @@
         if (
             (name := self.name())
         ):
             return name;
         self._reset(mark)
         return None;
 
+    @memoize
+    def units_group(self) -> Optional[Any]:
+        # units_group: '(' units ')' | units
+        mark = self._mark()
+        if (
+            (literal := self.expect('('))
+            and
+            (units := self.units())
+            and
+            (literal_1 := self.expect(')'))
+        ):
+            return [literal, units, literal_1];
+        self._reset(mark)
+        if (
+            (units := self.units())
+        ):
+            return units;
+        self._reset(mark)
+        return None;
+
     @memoize_left_rec
     def sum(self) -> Optional[Any]:
         # sum: sum '+' term | sum '-' term | term
         mark = self._mark()
         if (
             (sum := self.sum())
             and
```

### Comparing `unit_syntax-0.1.1/unit_syntax/transform.py` & `unit_syntax-0.1.2/unit_syntax/transform.py`

 * *Files identical despite different names*

### Comparing `unit_syntax-0.1.1/PKG-INFO` & `unit_syntax-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,10 @@
-Metadata-Version: 2.1
-Name: unit-syntax
-Version: 0.1.1
-Summary: Literal physical units for Jupyter and IPython
-Home-page: https://github.com/ahupp/unit-syntax
-Author: Adam Hupp
-Author-email: adam@hupp.org
-Requires-Python: >=3.8,<4
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pint (>=0.20,<0.21)
-Requires-Dist: ipython (>=7)
-Requires-Dist: pegen (>=0.2,<0.3)
-Project-URL: Repository, https://github.com/ahupp/unit-syntax
-Description-Content-Type: text/markdown
-
 `unit-syntax` extends the Python language in Jupyter/IPython to support expressions with physical units:
 
 ```python
->>> import unit_syntax.ipython
 >>> speed = 5 meters/second
 >>> 2 seconds * speed
 10 meter
 ```
 
 Behind the scenes this is translated into standard Python that uses the excellent [Pint](https://pint.readthedocs.io/) units library.
 
@@ -51,15 +31,15 @@
 
 Units apply to the preceding value (a literal, variable, function call or indexing), and have higher precedence than other operators:
 
 ```python
 x * 1.21 gigawatts
 ```
 
-This is equivalent to `x * (1.21 gigawatts)`, and desugars to something like `x * Quantity(1.21, "gigawatts")`.  The high precedence means units apply to the literal not the whole expression.
+This is equivalent to `x * (1.21 gigawatts)`, and desugars to something like `x * Quantity(1.21, "gigawatts")`. The high precedence means units apply to the literal not the whole expression.
 
 Values can be converted to another measurement system:
 
 ```python
 (88 miles / hour) furlongs / fortnight
 ```
 
@@ -67,60 +47,62 @@
 
 ```python
 velocity = [5, 7] meters/second**2
 location = velocity * 2 seconds
 distance_traveled = numpy.linalg.norm(location)
 ```
 
+## The Grammar
+
 The units term follows this grammar:
 
 ```
 units:
-    | NAME '/' units
-    | NAME '*' units
-    | NAME units
+    | NAME '/' units_group
+    | NAME '*' units_group
+    | NAME units_group
     | NAME '**' NUMBER
     | NAME
+
+units_group:
+    | '(' units ')'
+    | units
 ```
 
-## Why?  How?
+## Why? How?
 
 I like using Python+[Jupyter Notebook](https://jupyter.org/) as a calculator for physical problems and often wish it had the clarity and type checking of explicit units. [Pint](https://pint.readthedocs.io/) is great, but (IMO) its necessary verbosity makes it hard to see the underlying calculation that's going.
 
-`unit-syntax` is an IPython/Jupyter [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) that rewrites expressions with units into calls to `pint.Quantity`.
-
-This is possible without ambiguity in the python grammar because it's otherwise invalid for a "primary" (literal, function call etc) to be immediately followed by 
+`unit-syntax` is an IPython/Jupyter [custom input transformer](https://ipython.readthedocs.io/en/stable/config/inputtransforms.html) that rewrites expressions with units into calls to `pint.Quantity`. The parser is a lightly modified version of the Python grammar using the same parser generator ([pegen](https://github.com/we-like-parsers/pegen)) as Python itself.
 
 `unit-syntax` cannot (currently) be used for standalone python scripts outside of IPython/Jupyter, but that's in principle possible through [meta_path import hooks](https://docs.python.org/3/reference/import.html#the-meta-path).
 
 The syntax takes advantage of the fact that that in python its illegal for a NAME to follow a "primary" (literal, function call etc), so there's no ambiguity.
 
-
 ## Prior Art
 
-The immediate inspriration of `unit-syntax` is a language called [Fortress](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.6323&rep=rep1&type=pdf
-) from Sun Microsystems.  Fortress was intended as a modern Fortran, and had first-class support for units in both the syntax and type system.
+The immediate inspriration of `unit-syntax` is a language called [Fortress](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.180.6323&rep=rep1&type=pdf) from Sun Microsystems. Fortress was intended as a modern Fortran, and had first-class support for units in both the syntax and type system.
 
 F# (an OCaml derivative from Microsoft) also [has first class support for units](https://en.wikibooks.org/wiki/F_Sharp_Programming/Units_of_Measure).
 
 The Julia package [Unitful.jl](http://painterqubits.github.io/Unitful.jl/stable/)
 
 ## Open questions and future work
 
- * Fortress uses an `in` operator to apply units to a non-literal value, e.g `x in meters`.  This has the advantage of being unambiguous regardless of parenthesization.  In python this would conflcit with `value in [a, b, c]`, but `as` is
+- Fortress uses an `in` operator to apply units to a non-literal value, e.g `x in meters`. This has the advantage of being unambiguous regardless of parenthesization. In python this would conflcit with `value in [a, b, c]`, but `as` is
 
- * Move to tree-sitter, which will be simpler and has a chance of providing syntax highlighting
- * Test against various ipython and python versions
- * Support standalone scripts through sys.meta_path
- * Check units at parse time
- * Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable).  More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
- * Pint does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
- * Demo colab notebook: https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV
- * Describe parsing ambuguity like `1 meters * sin(45 degrees)`
- * Figure out story around parenthesization
+- Move to tree-sitter, which will be simpler and has a chance of providing syntax highlighting
+- Test against various ipython and python versions
+- Support standalone scripts through sys.meta_path
+- Check units at parse time
+- Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
+- Pint does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
+- Demo colab notebook: https://colab.research.google.com/drive/1PInyLGZHnUzEuUVgMsLrUUNdCurXK7v1#scrollTo=JszzXmATY0TV
+- Describe parsing ambuguity like `1 meters * sin(45 degrees)`
+- Figure out story around parenthesization
 
 ## Development
 
 To regenerate the parser:
 
 `python -m pegen grammar.txt -o unit_syntax/parser.py`
 
@@ -129,21 +111,17 @@
 ```
  $ poetry install --with dev
  $ poetry run pytest
 ```
 
 ## Future work and open questions
 
- * Parenthisized units expressions
- * Demo colab notebook
- * Move to tree-sitter so there's a chance of getting syntax highlighting
- * Jupyter syntax checks
- * Typography of output
- * Test against various ipython and python versions
- * Support standalone scripts through sys.meta_path
- * Check units at parse time
- * Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable).  More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166) 
- * Does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
-
-
- 
-
+- Parenthisized units expressions
+- Demo colab notebook
+- Move to tree-sitter so there's a chance of getting syntax highlighting
+- Jupyter syntax checks
+- Typography of output
+- Test against various ipython and python versions
+- Support standalone scripts through sys.meta_path
+- Check units at parse time
+- Unit type hints, maybe checked with [@runtime_checkable](https://docs.python.org/3/library/typing.html#typing.runtime_checkable). More Pint typechecking [discussion](https://github.com/hgrecco/pint/issues/1166)
+- Does not do the right thing when applied to generator expressions, e.g `(a for a in range(0, 4)) meters`
```

