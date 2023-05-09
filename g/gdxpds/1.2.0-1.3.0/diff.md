# Comparing `tmp/gdxpds-1.2.0.tar.gz` & `tmp/gdxpds-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gdxpds-1.2.0.tar", last modified: Fri Sep 18 23:00:36 2020, max compression
+gzip compressed data, was "gdxpds-1.3.0.tar", last modified: Tue May  9 16:49:26 2023, max compression
```

## Comparing `gdxpds-1.2.0.tar` & `gdxpds-1.3.0.tar`

### file list

```diff
@@ -1,32 +1,40 @@
-drwxrwxrwx   0        0        0        0 2020-09-18 23:00:36.000000 gdxpds-1.2.0/
-drwxrwxrwx   0        0        0        0 2020-09-18 23:00:36.000000 gdxpds-1.2.0/bin/
--rw-rw-rw-   0        0        0     4069 2020-09-18 22:56:35.000000 gdxpds-1.2.0/bin/csv_to_gdx.py
--rw-rw-rw-   0        0        0     3286 2020-09-18 22:56:35.000000 gdxpds-1.2.0/bin/gdx_to_csv.py
--rw-rw-rw-   0        0        0     2658 2020-09-18 22:56:35.000000 gdxpds-1.2.0/CHANGES.txt
-drwxrwxrwx   0        0        0        0 2020-09-18 23:00:36.000000 gdxpds-1.2.0/gdxpds/
--rw-rw-rw-   0        0        0    37402 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/gdx.py
--rw-rw-rw-   0        0        0     5174 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/read_gdx.py
--rw-rw-rw-   0        0        0     8660 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/special.py
-drwxrwxrwx   0        0        0        0 2020-09-18 23:00:36.000000 gdxpds-1.2.0/gdxpds/test/
--rw-rw-rw-   0        0        0     2851 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/all_generator_properties_input.gdx
--rw-rw-rw-   0        0        0      507 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/annual_generation.csv
--rw-rw-rw-   0        0        0     1997 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/conftest.py
--rw-rw-rw-   0        0        0   102107 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/CONVqn.gdx
--rw-rw-rw-   0        0        0      507 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/installed_capacity.csv
--rw-rw-rw-   0        0        0   306969 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/OptimalCSPConfig_In.gdx
--rw-rw-rw-   0        0        0  1994352 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/OptimalCSPConfig_Out.gdx
--rw-rw-rw-   0        0        0     6329 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/test_conversions.py
--rw-rw-rw-   0        0        0     3214 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/test_read.py
--rw-rw-rw-   0        0        0     2461 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/test_session.py
--rw-rw-rw-   0        0        0     7171 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/test_specials.py
--rw-rw-rw-   0        0        0    19174 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/test_write.py
--rw-rw-rw-   0        0        0     2843 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/test/__init__.py
--rw-rw-rw-   0        0        0     6996 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/tools.py
--rw-rw-rw-   0        0        0     6260 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/write_gdx.py
--rw-rw-rw-   0        0        0       21 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/_version.py
--rw-rw-rw-   0        0        0     3322 2020-09-18 22:56:35.000000 gdxpds-1.2.0/gdxpds/__init__.py
--rw-rw-rw-   0        0        0     2937 2020-09-18 23:00:36.000000 gdxpds-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2513 2020-09-18 22:56:35.000000 gdxpds-1.2.0/README.md
--rw-rw-rw-   0        0        0     2243 2020-09-18 22:56:35.000000 gdxpds-1.2.0/README.txt
--rw-rw-rw-   0        0        0       75 2020-09-18 22:56:35.000000 gdxpds-1.2.0/requirements.txt
--rw-rw-rw-   0        0        0     2458 2020-09-18 22:56:35.000000 gdxpds-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:49:26.437545 gdxpds-1.3.0/
+-rw-rw-rw-   0        0        0     3065 2023-05-09 16:32:48.000000 gdxpds-1.3.0/CHANGES.txt
+-rw-rw-rw-   0        0        0     1558 2023-05-09 16:32:48.000000 gdxpds-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-05-09 16:32:48.000000 gdxpds-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2214 2023-05-09 16:49:26.436565 gdxpds-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2499 2023-05-09 16:32:48.000000 gdxpds-1.3.0/README.md
+-rw-rw-rw-   0        0        0     1854 2023-05-09 16:43:36.000000 gdxpds-1.3.0/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-09 16:49:26.370910 gdxpds-1.3.0/bin/
+-rw-rw-rw-   0        0        0     2412 2023-05-09 16:32:48.000000 gdxpds-1.3.0/bin/csv_to_gdx.py
+-rw-rw-rw-   0        0        0     1631 2023-05-09 16:32:48.000000 gdxpds-1.3.0/bin/gdx_to_csv.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:49:26.388131 gdxpds-1.3.0/gdxpds/
+-rw-rw-rw-   0        0        0     1598 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/__init__.py
+-rw-rw-rw-   0        0        0      426 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/_version.py
+-rw-rw-rw-   0        0        0    43114 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/gdx.py
+-rw-rw-rw-   0        0        0     4172 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/read_gdx.py
+-rw-rw-rw-   0        0        0     6697 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/special.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:49:26.433545 gdxpds-1.3.0/gdxpds/test/
+-rw-rw-rw-   0        0        0   102107 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/CONVqn.gdx
+-rw-rw-rw-   0        0        0   306969 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/OptimalCSPConfig_In.gdx
+-rw-rw-rw-   0        0        0  1994352 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/OptimalCSPConfig_Out.gdx
+-rw-rw-rw-   0        0        0     1114 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/__init__.py
+-rw-rw-rw-   0        0        0     2851 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/all_generator_properties_input.gdx
+-rw-rw-rw-   0        0        0      507 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/annual_generation.csv
+-rw-rw-rw-   0        0        0      342 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/conftest.py
+-rw-rw-rw-   0        0        0      507 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/installed_capacity.csv
+-rw-rw-rw-   0        0        0     4671 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/test_conversions.py
+-rw-rw-rw-   0        0        0     1559 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/test_read.py
+-rw-rw-rw-   0        0        0      806 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/test_session.py
+-rw-rw-rw-   0        0        0     5999 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/test_specials.py
+-rw-rw-rw-   0        0        0    17494 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/test/test_write.py
+-rw-rw-rw-   0        0        0     5589 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/tools.py
+-rw-rw-rw-   0        0        0     4702 2023-05-09 16:32:48.000000 gdxpds-1.3.0/gdxpds/write_gdx.py
+drwxrwxrwx   0        0        0        0 2023-05-09 16:49:26.398573 gdxpds-1.3.0/gdxpds.egg-info/
+-rw-rw-rw-   0        0        0     2214 2023-05-09 16:49:26.000000 gdxpds-1.3.0/gdxpds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      771 2023-05-09 16:49:26.000000 gdxpds-1.3.0/gdxpds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 16:49:26.000000 gdxpds-1.3.0/gdxpds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2023-05-09 16:49:26.000000 gdxpds-1.3.0/gdxpds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-09 16:49:26.000000 gdxpds-1.3.0/gdxpds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 16:49:26.437545 gdxpds-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1250 2023-05-09 16:40:27.000000 gdxpds-1.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gdxpds-1.2.0/CHANGES.txt` & `gdxpds-1.3.0/CHANGES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+v1.3.0, 05/09/23 -- performance improvements (faster read and write)
+                    GAMS directory finder improvements
+                    documentation improvements
+                    skip over individual GdxSymbols that fail to load
+                    drop support for Python versions < 3.7
+                    various minor improvements and bug fixes                                        
 v1.2.0, 09/18/20 -- search for GAMS in more places, especially on Windows
                     gdxpds.gdx.GdxSymbol.unload method for user-directed memory managment
                     convenience functions gdxpds.gdx.append_set and append_parameter
                     special value handling moved to its own module
                     clarifying that Python 2.X is not longer supported
                     general documentation, pylint, and testing improvements
 v1.1.0, 10/09/18 -- fixes to_dataframes and to_gdx memory leaks, respects
```

### Comparing `gdxpds-1.2.0/gdxpds/gdx.py` & `gdxpds-1.3.0/gdxpds/gdx.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,7 @@
-# [LICENSE]
-# Copyright (c) 2020, Alliance for Sustainable Energy.
-# All rights reserved.
-# 
-# Redistribution and use in source and binary forms, 
-# with or without modification, are permitted provided 
-# that the following conditions are met:
-# 
-# 1. Redistributions of source code must retain the above 
-# copyright notice, this list of conditions and the 
-# following disclaimer.
-# 
-# 2. Redistributions in binary form must reproduce the 
-# above copyright notice, this list of conditions and the 
-# following disclaimer in the documentation and/or other 
-# materials provided with the distribution.
-# 
-# 3. Neither the name of the copyright holder nor the 
-# names of its contributors may be used to endorse or 
-# promote products derived from this software without 
-# specific prior written permission.
-# 
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND 
-# CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, 
-# INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF 
-# MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE 
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR 
-# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, 
-# SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, 
-# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR 
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) 
-# HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN 
-# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE 
-# OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-# [/LICENSE]
-
 '''
 Backend functionality for reading and writing GDX files. 
 The GdxFile and GdxSymbol classes are full-featured interfaces
 for going between the GDX format and pandas DataFrames,
 including translation between GDX and numpy special values. 
 '''
 
@@ -70,15 +33,15 @@
 # gdxpds needs to be imported before pandas to try to avoid library conflict on 
 # Linux that causes a segmentation fault.
 from gdxpds import Error
 from gdxpds.tools import NeedsGamsDir
 
 import gdxcc
 import numpy as np
-import pandas as pds
+import pandas as pd
 
 import gdxpds.special as special
 # Import some things for backward compatibility
 from gdxpds.special import (
     convert_gdx_to_np_svs,
     convert_np_to_gdx_svs,
     gdx_isnan,
@@ -140,14 +103,24 @@
 class GdxFile(MutableSequence, NeedsGamsDir):
 
     def __init__(self,gams_dir=None,lazy_load=True):
         """
         Initializes a GdxFile object by connecting to GAMS and creating a pointer.
 
         Throws a GdxError if either of those operations fail.
+
+        Parameters
+        ----------
+        gams_dir : None or str
+        lazy_load : bool
+            If True, :py:class:`GdxSymbol` data are not automatically loaded when the 
+            symbols are initially :py:meth:`read`. Individual data tables can only be 
+            accessed later after the corresponding calls to :py:meth:`GdxSymbol.load`. 
+            If False, all data are automatically loaded and the full GDX file is 
+            available in memory after the call to :py:meth:`read`.
         """
         self.lazy_load = lazy_load
         self._version = None
         self._producer = None
         self._filename = None
         self._symbols = OrderedDict()
 
@@ -173,37 +146,52 @@
 
     def clone(self):
         """
         Returns a new GdxFile containing clones of the GdxSymbols in this 
         GdxFile. The clone will not be associated with a filename. The clone's
         GdxSymbols will not have indexes. The clone will be ready to write to 
         a new file.
+
+        Returns
+        -------
+        :py:class:`GdxFile`
         """
         result = GdxFile(gams_dir=self.gams_dir,lazy_load=False)
         for symbol in self:
             result.append(symbol.clone())
             result[-1]._file = result
         return result
 
     @property
     def empty(self):
         """
-        Returns True if this GdxFile object contains any symbols.
+        Returns True if this GdxFile object does not contain any symbols.
+
+        Returns
+        -------
+        bool
         """
         return len(self) == 0
 
     @property
     def H(self):
         """
         GDX object handle
         """
         return self._H
 
     @property
     def filename(self):
+        """
+        Filename this :py:class:`GdxFile` is associated with, if any
+
+        Returns
+        -------
+        None or str
+        """
         return self._filename
 
     @property
     def version(self):
         """
         GDX file version
         """
@@ -214,24 +202,35 @@
         """
         What program wrote the GDX file
         """
         return self._producer
 
     @property
     def num_elements(self):
+        """
+        Total number of records present in this file, summed over all symbols.
+
+        Returns
+        -------
+        int
+        """
         return sum([symbol.num_records for symbol in self])
 
     def read(self,filename):
         """
         Opens gdx file at filename and reads meta-data. If not self.lazy_load, 
         also loads all symbols.
 
         Throws an Error if not self.empty.
 
         Throws a GdxError if any calls to gdxcc fail.
+
+        Parameters
+        ----------
+        filename : pathlib.Path or str
         """
         if not self.empty:
             raise Error("GdxFile.read can only be used if the GdxFile is .empty")
 
         # open the file
         rc = gdxcc.gdxOpenRead(self.H,str(filename))
         if not rc[0]:
@@ -240,34 +239,46 @@
 
         # read in meta-data ...
         # ... for the file
         ret, self._version, self._producer = gdxcc.gdxFileVersion(self.H)
         if ret != 1: 
             raise GdxError(self.H,"Could not get file version")
         ret, symbol_count, element_count = gdxcc.gdxSystemInfo(self.H)
-        logger.debug("Opening '{}' with {} symbols and {} elements with lazy_load = {}.".format(filename,symbol_count,element_count,self.lazy_load))
+        logger.debug(f"Opening '{filename}' with {symbol_count} symbols and "
+                     f"{element_count} elements with lazy_load = {self.lazy_load}.")
         # ... for the symbols
         ret, name, dims, data_type = gdxcc.gdxSymbolInfo(self.H,0)
         if ret != 1:
             raise GdxError(self.H,"Could not get symbol info for the universal set")
         self.universal_set = GdxSymbol(name,data_type,dims=dims,file=self,index=0)
         for i in range(symbol_count):
             index = i + 1
             ret, name, dims, data_type = gdxcc.gdxSymbolInfo(self.H,index)
             if ret != 1:
-                raise GdxError(self.H,"Could not get symbol info for symbol {}".format(index))
-            self.append(GdxSymbol(name,data_type,dims=dims,file=self,index=index))
+                raise GdxError(self.H,f"Could not get symbol info for symbol {index}")
+            try:
+                sym = GdxSymbol(name,data_type,dims=dims,file=self,index=index)
+                self.append(sym)
+            except Exception as e:
+                logger.error(f"Unable to initialize GdxSymbol {name!r}, because {e}. SKIPPING.")
 
         # read all symbols if not lazy_load
         if not self.lazy_load:
             for symbol in self:
                 symbol.load()
         return
 
     def write(self,filename):
+        """
+        Writes this :py:class:`GdxFile` to filename
+
+        Parameters
+        ----------
+        filename : pathlib.Path or str
+        """
         # only write if all symbols loaded
         for symbol in self:
             if not symbol.loaded:
                 raise Error("All symbols must be loaded before this file can be written.")
 
         ret = gdxcc.gdxOpenWrite(self.H,str(filename),"gdxpds")
         if not ret:
@@ -299,54 +310,106 @@
             s += sep + str(symbol)
             sep = "\n  "
         return s
 
     def __getitem__(self,key):
         """
         Supports list-like indexing and symbol-based indexing
+
+        Parameters
+        ----------
+        key : int or str
+            If int, the index into the list of symbols. If str, the name of the symbol to 
+            be accessed.
+
+        Returns
+        -------
+        :py:class:`GdxSymbol`
         """
         return self._symbols[self._name_key(key)]
 
     def __setitem__(self,key,value):
+        """
+        Supports overwriting or adding a :py:class:`GdxSymbol` via a list-like interface
+
+        Parameters
+        ----------
+        key : int
+            Must be an index into the list of symbols, within range(len(self)+1)
+        value : :py:class:`GdxSymbol`
+        """
         self._check_insert_setitem(key, value)
         value._file = self
         if key < len(self):
             self._symbols[self._name_key(key)] = value
             self._fixup_name_keys()
             return
         assert key == len(self)
         self._symbols[value.name] = value
         return
 
     def __delitem__(self,key):
+        """
+        Deletes a symbol from this :py:class:`GdxFile`'s collection
+
+        Parameters
+        ----------
+        key : int or str
+            If int, the index into the list of symbols. If str, the name of the symbol to 
+            be accessed.
+        """
         del self._symbols[self._name_key(key)]
         return
 
     def __len__(self):
+        """
+        Number of :py:class:`GdxSymbol`s in this :py:class:`GdxFile`
+        """
         return len(self._symbols)
 
     def insert(self,key,value):
+        """
+        Inserts value at position key
+
+        Parameters
+        ----------
+        key : int
+            Must be an index into the list of symbols, within range(len(self)+1)
+        value : :py:class:`GdxSymbol`
+        """
         self._check_insert_setitem(key, value)
         value._file = self
-        data = [(symbol.name, symbol) for symbol in self]
-        data.insert(key,(value.name,value))
-        self._symbols = OrderedDict(data)
+        if key == len(self) and value.name not in self._symbols:
+            # We can safely append the symbol. This is fast (O(log(n)) complexity)
+            self._symbols[value.name] = value
+        else:
+            # Need to insert inside the sequence. This is slow (O(n) complexity)
+            data = [(symbol.name, symbol) for symbol in self]
+            data.insert(key,(value.name,value))
+            self._symbols = OrderedDict(data)
         return
 
     def __contains__(self,key):
         """
         Returns True if __getitem__ works with key.
         """
         try:
             self.__getitem__(key)
             return True
         except:
             return False
 
     def keys(self):
+        """
+        List of symbol names obtained by iterating through this :py:class:`GdxFile`
+
+        Returns
+        -------
+        list of str
+        """
         return [symbol.name for symbol in self]
 
     def _name_key(self,key):
         name_key = key
         if isinstance(key,int):
             name_key = list(self._symbols.keys())[key]
         return name_key
@@ -397,14 +460,15 @@
     Equality = 53 + gdxcc.GMS_EQUTYPE_E
     GreaterThan = 53 + gdxcc.GMS_EQUTYPE_G
     LessThan = 53 + gdxcc.GMS_EQUTYPE_L
     NothingEnforced = 53 + gdxcc.GMS_EQUTYPE_N
     External = 53 + gdxcc.GMS_EQUTYPE_X
     Conic = 53 + gdxcc.GMS_EQUTYPE_C
 
+
 class GamsValueType(Enum):
     Level = gdxcc.GMS_VAL_LEVEL       # .l
     Marginal = gdxcc.GMS_VAL_MARGINAL # .m
     Lower = gdxcc.GMS_VAL_LOWER       # .lo
     Upper = gdxcc.GMS_VAL_UPPER       # .ub
     Scale = gdxcc.GMS_VAL_SCALE       # .scale
 
@@ -416,42 +480,76 @@
                     return value_type
             if value == 'Value':
                 return GamsValueType(GamsValueType.Level)
         super()._missing_(value)
 
 
 GAMS_VALUE_COLS_MAP = defaultdict(lambda : [('Value',GamsValueType.Level.value)])
+"""
+List of value columns provided for each :py:attr:`GamsValueType`
+"""
 GAMS_VALUE_COLS_MAP[GamsDataType.Variable] = [(value_type.name, value_type.value) for value_type in GamsValueType]
 GAMS_VALUE_COLS_MAP[GamsDataType.Equation] = GAMS_VALUE_COLS_MAP[GamsDataType.Variable]
 
 
 GAMS_VALUE_DEFAULTS = {
     GamsValueType.Level: 0.0,
     GamsValueType.Marginal: 0.0,
     GamsValueType.Lower: -np.inf,
     GamsValueType.Upper: np.inf,
     GamsValueType.Scale: 1.0
 }
+"""
+Default values for each :py:class:`GamsValueType`
+"""
 
 GAMS_VARIABLE_DEFAULT_LOWER_UPPER_BOUNDS = {
     GamsVariableType.Unknown: (-np.inf,np.inf),
     GamsVariableType.Binary: (0.0,1.0),
     GamsVariableType.Integer: (0.0,np.inf),
     GamsVariableType.Positive: (0.0,np.inf),
     GamsVariableType.Negative: (-np.inf,0.0),
     GamsVariableType.Free : (-np.inf,np.inf),
     GamsVariableType.SOS1: (0.0,np.inf),
     GamsVariableType.SOS2: (0.0,np.inf),
     GamsVariableType.Semicont: (1.0,np.inf),
     GamsVariableType.Semiint: (1.0,np.inf)
 }
+"""
+Default lower and upper bounds for each :py:class:`GamsVariableType`
+"""
+
 
 class GdxSymbol(object): 
     def __init__(self,name,data_type,dims=0,file=None,index=None,
                  description='',variable_type=None,equation_type=None): 
+        """
+        In-memory representation of a GAMS GDX Symbol
+
+        Parameters
+        ----------
+        name : str
+        data_type : :py:class:`GamsDataType`
+        dims : int or list of str
+            If dims is set to an int, then that number of dimensions will be created, each 
+            indicated with the wildcard name '*'. Otherwise, a list of strings is expected, 
+            each string being a dimension name.
+        file : None or :py:class:`GdxFile`
+            Users should not set file. File is set by, e.g., :py:meth:`GdxFile.read` and
+            :py:meth:`GdxFile.append`.
+        index : None or int
+            Users should not set file. File is set by, e.g., :py:meth:`GdxFile.read` and
+            :py:meth:`GdxFile.append`.
+        description : str
+            Human readable description for this :py:class:`GdxSymbol`
+        variable_type : None or :py:class:`GamsVariableType`
+            Only expected if data_type == :py:attr:`GamsDataType.Variable`
+        equation_type : None or :py:class:`GamsEquationType`
+            Only expected if data_type == :py:attr:`GamsDataType.Equation`
+        """
         self._name = name
         self.description = description
         self._loaded = False
         self._data_type = GamsDataType(data_type)
         self._variable_type = None; self.variable_type = variable_type
         self._equation_type = None; self.equation_type = equation_type
         self._dataframe = None; self._dims = None
@@ -485,14 +583,21 @@
             return
         
         # writing new symbol
         self._loaded = True
         return
 
     def clone(self):
+        """
+        Create a copy of this :py:class:`GdxSymbol`
+
+        Returns
+        -------
+        :py:class:`GdxSymbol`
+        """
         if not self.loaded:
             raise Error("Symbol {} cannot be cloned because it is not yet loaded.".format(repr(self.name)))
 
         assert self.loaded
         result = GdxSymbol(self.name,self.data_type,
                            dims=self.dims,
                            description=self.description,
@@ -500,39 +605,60 @@
                            equation_type=self.equation_type)
         result.dataframe = copy.deepcopy(self.dataframe)
         assert result.loaded
         return result
 
     @property
     def name(self):
+        """
+        Name of this :py:class:`GdxSymbol`
+
+        Returns
+        -------
+        str
+        """
         return self._name
 
     @name.setter
     def name(self,value):
         self._name = value
         if self.file is not None:
             self.file._fixup_name_keys()
         return
 
     @property
     def data_type(self):
+        """
+        GAMS data type of this :py:class:`GdxSymbol`
+
+        Returns
+        -------
+        :py:class:`GamsDataType`
+        """
         return self._data_type
 
     @data_type.setter
     def data_type(self, value):
         if not self.loaded or self.num_records > 0:
             raise Error("Cannot change the data_type of a GdxSymbol that is yet to be read for file or contains records.")
         self._data_type = GamsDataType(value)
         self.variable_type = None
         self.equation_type = None
         self._init_dataframe()
         return
 
     @property
     def variable_type(self):
+        """
+        Only not none if :py:attr:`data_type` == :py:attr:`GamsDataType.Variable`
+
+        Returns
+        -------
+        None or :py:attr:`GamsDataType.Variable`
+        """
         return self._variable_type
 
     @variable_type.setter
     def variable_type(self,value):
         if self.data_type == GamsDataType.Variable:
             if value is None:
                 # default to Free
@@ -550,14 +676,21 @@
         assert self.data_type != GamsDataType.Variable
         if value is not None:
             logger.warning("GdxSymbol is not a Variable, so setting variable_type to None")
         self._variable_type = None
 
     @property
     def equation_type(self):
+        """
+        Only not none if :py:attr:`data_type` == :py:attr:`GamsDataType.Equation`
+
+        Returns
+        -------
+        None or :py:attr:`GamsDataType.Equation`
+        """
         return self._equation_type
 
     @equation_type.setter
     def equation_type(self,value):
         if self.data_type == GamsDataType.Equation:
             if value is None:
                 # default to Equality
@@ -576,22 +709,33 @@
         if value is not None:
             logger.warning("GdxSymbol is not an Equation, so setting equation_type to None")
         self._equation_type = None
 
     @property
     def value_cols(self):
         """
-        Returns list of (name, GamsValueType.value) tuples that describe the 
-        value columns in the dataframe, that is, those columns that follow the 
-        self.dims.
+        List of (name, GamsValueType.value) tuples that describe the 
+        value columns in the dataframe, that is, the columns that follow the 
+        self.dims columns.
+
+        Returns
+        -------
+        list of (str, int)
         """
         return GAMS_VALUE_COLS_MAP[self.data_type]
 
     @property
     def value_col_names(self):
+        """
+        List of value column names, that is, the columns that follow the self.dims columns.
+
+        Returns
+        -------
+        list of str
+        """
         return [col_name for col_name, col_ind in self.value_cols]    
 
     def get_value_col_default(self,value_col_name):
         if not value_col_name in self.value_col_names:
             raise Error(f"{value_col_name} is not one of the value columns for "
                 f"this GdxSymbol, which is a {self.data_type}")
         value_col = GamsValueType(value_col_name)
@@ -607,34 +751,64 @@
             else:
                 assert value_col == GamsValueType.Upper
                 return ub_default
         return GAMS_VALUE_DEFAULTS[value_col] 
 
     @property
     def file(self):
+        """
+        :py:class:`GdxFile` file that contains this :py:class:`GdxSymbol`, if any
+
+        Returns
+        -------
+        None or :py:class:`GdxFile`
+        """
         return self._file
 
     @property
     def index(self):
+        """
+        Index of this :py:class:`GdxSymbol` in its :py:class:`GdxFile`, if any
+
+        Returns
+        -------
+        None or int
+        """
         return self._index
 
     @property
     def loaded(self):
+        """
+        Whether the data for this symbol has been loaded
+
+        Returns
+        -------
+        bool
+        """
         return self._loaded
 
     @property
     def full_typename(self):
         if self.data_type == GamsDataType.Parameter and self.dims == 0:
             return 'Scalar'
         elif self.data_type == GamsDataType.Variable:
             return self.variable_type.name + " " + self.data_type.name
         return self.data_type.name
 
     @property
     def dims(self):
+        """
+        List of dimension names over which this symbol is defined. If the :py:class:`GdxSymbol` was 
+        constructed with dims set to an integer, all dimension names will be the wildcard '*'.
+
+        Returns
+        -------
+        list of str
+            length of list is equal to :py:attr:`num_dims`
+        """
         return self._dims
 
     @dims.setter
     def dims(self, value):
         if (self._dims is not None) and (self.loaded and ((self.num_dims > 0) or (self.num_records > 0))):
             if not isinstance(value,list) or len(value) != self.num_dims:
                 raise Error(f"Cannot set dims to {value}, because the number of "
@@ -653,33 +827,47 @@
         if self.loaded and self.num_records > 0:
             self._dataframe.columns = self.dims + self.value_col_names
             return
         self._init_dataframe()
 
     @property
     def num_dims(self):
+        """
+        Number of dimensions over which this symbol is defined
+
+        Returns
+        -------
+        int
+        """
         return len(self.dims)        
 
     @property
     def dataframe(self):
+        """
+        Data table for this symbol. Dim columns are followed by value columns, left to right.
+        
+        Returns
+        -------
+        pd.DataFrame
+        """
         return self._dataframe
 
     @dataframe.setter
     def dataframe(self, data):
         try:        
             # get data in common format and start dealing with dimensions    
-            if isinstance(data, pds.DataFrame):
+            if isinstance(data, pd.DataFrame):
                 df = data.copy()
                 has_col_names = True
             else:
-                df = pds.DataFrame(data)
+                df = pd.DataFrame(data)
                 has_col_names = False
                 if df.empty:
                     # clarify dimensionality, as needed for loading empty GdxSymbols
-                    df = pds.DataFrame(data,columns=self.dims + self.value_cols)
+                    df = pd.DataFrame(data,columns=self.dims + self.value_cols)
             
             # finish handling dimensions
             n = len(df.columns)
             if (self.num_dims > 0) or (self.num_records > 0):
                 if not ((n == self.num_dims) or (n == self.num_dims + len(self.value_cols))):
                     raise Error("Cannot set dataframe to {} because the number ".format(df.head()) + \
                         "of dimensions would change. This symbol has {} ".format(self.num_dims) + \
@@ -726,15 +914,15 @@
             raise
 
         if self.data_type == GamsDataType.Set:
             self._fixup_set_value()
         return
 
     def _init_dataframe(self):
-        self._dataframe = pds.DataFrame([],columns=self.dims + self.value_col_names)
+        self._dataframe = pd.DataFrame([],columns=self.dims + self.value_col_names)
         if self.data_type == GamsDataType.Set:
             colname = self._dataframe.columns[-1]
             replace_df_column(self._dataframe,colname,self._dataframe[colname].astype(c_bool))
         return
 
     def _append_default_values(self,df):
         assert len(df.columns) == self.num_dims
@@ -763,14 +951,21 @@
                 "filled:\n{self._dataframe[self._dataframe[colname].isnull()]}")
             replace_df_column(self._dataframe, colname, self._dataframe[colname].fillna(value=True))
         replace_df_column(self._dataframe,colname,self._dataframe[colname].apply(lambda x: c_bool(x)))
         return
 
     @property
     def num_records(self):
+        """
+        Number of rows in the data table, per the DataFrame if :py:attr:`loaded`, or per GAMS.
+
+        Returns
+        -------
+        int
+        """
         if self.loaded:
             return len(self.dataframe.index)
         return self._num_records
 
     def __repr__(self):
         return "GdxSymbol({},{},{},file={},index={},description={},variable_type={},equation_type={})".format(
                    repr(self.name),
@@ -788,49 +983,61 @@
         s += ", " + self.full_typename    
         s += ", {} records".format(self.num_records)
         s += ", {} dims {}".format(self.num_dims, self.dims)
         s += ", loaded" if self.loaded else ", not loaded"
         return s
 
     def load(self):
+        """
+        Loads this :py:class:`GdxSymbol` from its :py:attr:`file`
+        """
         if self.loaded:
             logger.info("Nothing to do. Symbol already loaded.")
             return
         if not self.file:
             raise Error("Cannot load {} because there is no file pointer".format(repr(self)))
         if not self.index:
             raise Error("Cannot load {} because there is no symbol index".format(repr(self)))
 
         if self.data_type == GamsDataType.Parameter and HAVE_GDX2PY:
             self.dataframe = gdx2py.par2list(self.file.filename,self.name) 
             self._loaded = True
             return
 
-        data = []
         _ret, records = gdxcc.gdxDataReadStrStart(self.file.H,self.index)
-        for _i in range(records):
-            _ret, elements, values, _afdim = gdxcc.gdxDataReadStr(self.file.H)
-            # make sure we pick value columns up correctly
-            data.append(elements + [values[col_ind] for col_name, col_ind in self.value_cols])
-            if self.data_type == GamsDataType.Set:
-                data[-1][-1] = True
-                # gdxdict called gdxGetElemText here, but I do not currently see value in doing that
+
+        def reader():
+            handle = self.file.H
+            for i in range(records):
+                yield gdxcc.gdxDataReadStr(handle)
+
+        vc = self.value_cols  # do this for speed in the next line
+        data = [elements + [values[col_ind] for col_name, col_ind in vc] for ret, elements, values, afdim in reader()]
+        # gdxdict called gdxGetElemText here, but I do not currently see value in doing that
         self.dataframe = data
-        if not self.data_type == GamsDataType.Set:
+        if not self.data_type in (GamsDataType.Set, GamsDataType.Alias):
             self.dataframe = special.convert_gdx_to_np_svs(self.dataframe, self.num_dims)
         self._loaded = True
         return
 
     def unload(self):
+        """
+        Drops this :py:class:`GdxSymbol`'s :py:attr:`dataframe`
+        """
         self.dataframe = None
         self._loaded = False
 
     def write(self,index=None): 
+        """
+        Writes this :py:class:`GdxSymbol` to its :py:attr:`file`
+        """
         if not self.loaded:
-            raise Error("Cannot write unloaded symbol {}.".format(repr(self.name)))
+            raise Error(f"Cannot write unloaded symbol {self.name!r}.")
+        if self.file is None:
+            raise Error(f"Cannot write {self!r} because there is no file pointer")
 
         if self.data_type == GamsDataType.Set:
             self._fixup_set_value()
 
         if index is not None:
             self._index = index
 
@@ -860,15 +1067,18 @@
                 if not gdxcc.gdxSymbolSetDomainX(self.file.H,self.index,self.dims):
                     raise GdxError(self.file.H,"Could not set domain information for {}. Domains are {}".format(repr(self.name),repr(self.dims)))
             else:
                 logger.info("Not writing domain information because symbol index is unknown.")
         values = gdxcc.doubleArray(gdxcc.GMS_VAL_MAX)
         # make sure index is clean -- needed for merging in convert_np_to_gdx_svs
         self.dataframe = self.dataframe.reset_index(drop=True)
-        for row in special.convert_np_to_gdx_svs(self.dataframe, self.num_dims).itertuples(index=False, name=None):
+        # convert special numeric values if appropriate
+        to_write = self.dataframe.copy() if (self.data_type in (GamsDataType.Set, GamsDataType.Alias)) else special.convert_np_to_gdx_svs(self.dataframe, self.num_dims)
+        # write each row
+        for row in to_write.itertuples(index=False, name=None):
             dims = [str(x) for x in row[:self.num_dims]]
             vals = row[self.num_dims:]
             for _col_name, col_ind in self.value_cols:
                 values[col_ind] = float(0.0)
                 try:
                     if isinstance(vals[col_ind],Number):
                         values[col_ind] = float(vals[col_ind])
@@ -908,21 +1118,21 @@
         to these names, because the dimension names are taken from the final 
         dataframe, these will also be the dimension names
     description : None or str
         passed directly to :class:`GdxSymbol`
     """
     # ensure df is DataFrame and not Series
     logger.debug(f"Defining set {set_name!r} based on:\n{df!r}")
-    tmp = pds.DataFrame(df)
+    tmp = pd.DataFrame(df)
     # select down to data we actually want
     if cols is not None:
         tmp = tmp[cols]
     if dim_names is not None:
         if tmp.empty:
-            tmp = pds.DataFrame([], columns = dim_names)
+            tmp = pd.DataFrame([], columns = dim_names)
         else:
             tmp.columns = dim_names
     # define the symbol
     gdx_file.append(GdxSymbol(set_name, GamsDataType.Set, 
         dims = list(tmp.columns), description = description))
     # define the data for the symbol
     gdx_file[-1].dataframe = tmp
@@ -946,30 +1156,30 @@
         name of the :class:`GdxSymbol` to be added
     df : pandas.DataFrame
         dataframe or data that can be used to construct a dataframe containing 
         the parameter data. assumes that the last selected column is the 'Value' 
         column
     cols : None or list of str
         if not None, these are the columns in df to be used for the parameter
-        definition
+        definition (dimension columns followed by value column)
     dim_names : None or list of str
         if provided, the columns of a copy of df (or of df[cols]) will be renamed
         to these names + ['Value']. because the dimension names are taken from 
         the final dataframe, these will also be the dimension names
     description : None or str
         passed directly to :class:`GdxSymbol`
     """
     # pre-process the data
     logger.debug(f"Defining parameter {param_name!r} based on:\n{df!r}")
-    tmp = pds.DataFrame(df)
+    tmp = pd.DataFrame(df)
     if cols is not None:
         tmp = tmp[cols]
     if dim_names is not None:
         if tmp.empty:
-            tmp = pds.DataFrame([], columns = dim_names + ['Value'])
+            tmp = pd.DataFrame([], columns = dim_names + ['Value'])
         else:
             tmp.columns = dim_names + ['Value']
     # define the symbol
     gdx_file.append(GdxSymbol(param_name, GamsDataType.Parameter,
         dims = list(tmp.columns)[:-1], description = description))
     # define the data for the symbol
     gdx_file[-1].dataframe = tmp
```

### Comparing `gdxpds-1.2.0/gdxpds/test/all_generator_properties_input.gdx` & `gdxpds-1.3.0/gdxpds/test/all_generator_properties_input.gdx`

 * *Files identical despite different names*

### Comparing `gdxpds-1.2.0/gdxpds/test/conftest.py` & `gdxpds-1.3.0/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,34 @@
-# [LICENSE]
-# Copyright (c) 2020, Alliance for Sustainable Energy.
-# All rights reserved.
-# 
-# Redistribution and use in source and binary forms, 
-# with or without modification, are permitted provided 
-# that the following conditions are met:
-# 
-# 1. Redistributions of source code must retain the above 
-# copyright notice, this list of conditions and the 
-# following disclaimer.
-# 
-# 2. Redistributions in binary form must reproduce the 
-# above copyright notice, this list of conditions and the 
-# following disclaimer in the documentation and/or other 
-# materials provided with the distribution.
-# 
-# 3. Neither the name of the copyright holder nor the 
-# names of its contributors may be used to endorse or 
-# promote products derived from this software without 
-# specific prior written permission.
-# 
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND 
-# CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, 
-# INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF 
-# MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE 
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR 
-# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, 
-# SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, 
-# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR 
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) 
-# HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN 
-# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE 
-# OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-# [/LICENSE]
+Copyright (c) 2023, Alliance for Sustainable Energy.
+All rights reserved.
 
-import pytest
+Redistribution and use in source and binary forms, 
+with or without modification, are permitted provided 
+that the following conditions are met:
 
-def pytest_addoption(parser):
-    parser.addoption(
-        "--no-clean-up", action="store_true", default=False, 
-        help="Pass this option to leave test outputs in place"
-    )
+1. Redistributions of source code must retain the above 
+copyright notice, this list of conditions and the 
+following disclaimer.
 
-@pytest.fixture(scope="session",autouse=True)
-def clean_up(request):
-    return (not request.config.getoption('--no-clean-up'))
-    
+2. Redistributions in binary form must reproduce the 
+above copyright notice, this list of conditions and the 
+following disclaimer in the documentation and/or other 
+materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the 
+names of its contributors may be used to endorse or 
+promote products derived from this software without 
+specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND 
+CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, 
+INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF 
+MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE 
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR 
+CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, 
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, 
+BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR 
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) 
+HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN 
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE 
+OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `gdxpds-1.2.0/gdxpds/test/CONVqn.gdx` & `gdxpds-1.3.0/gdxpds/test/CONVqn.gdx`

 * *Files identical despite different names*

### Comparing `gdxpds-1.2.0/gdxpds/test/OptimalCSPConfig_In.gdx` & `gdxpds-1.3.0/gdxpds/test/OptimalCSPConfig_In.gdx`

 * *Files identical despite different names*

### Comparing `gdxpds-1.2.0/gdxpds/test/OptimalCSPConfig_Out.gdx` & `gdxpds-1.3.0/gdxpds/test/OptimalCSPConfig_Out.gdx`

 * *Files identical despite different names*

### Comparing `gdxpds-1.2.0/gdxpds/test/test_write.py` & `gdxpds-1.3.0/gdxpds/test/test_write.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,14 @@
-# [LICENSE]
-# Copyright (c) 2020, Alliance for Sustainable Energy.
-# All rights reserved.
-# 
-# Redistribution and use in source and binary forms, 
-# with or without modification, are permitted provided 
-# that the following conditions are met:
-# 
-# 1. Redistributions of source code must retain the above 
-# copyright notice, this list of conditions and the 
-# following disclaimer.
-# 
-# 2. Redistributions in binary form must reproduce the 
-# above copyright notice, this list of conditions and the 
-# following disclaimer in the documentation and/or other 
-# materials provided with the distribution.
-# 
-# 3. Neither the name of the copyright holder nor the 
-# names of its contributors may be used to endorse or 
-# promote products derived from this software without 
-# specific prior written permission.
-# 
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND 
-# CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, 
-# INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF 
-# MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE 
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR 
-# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, 
-# SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, 
-# BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR 
-# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) 
-# HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN 
-# CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE 
-# OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-# [/LICENSE]
-
 from ctypes import c_bool
 import copy
 import logging
 import os
 
 import numpy as np
-import pandas as pds
+import pandas as pd
 import pytest
 
 import gdxpds.gdx
 from gdxpds.tools import Error
 from gdxpds.test import base_dir, run_dir
 from gdxpds.test.test_session import manage_rundir
 
@@ -55,41 +18,42 @@
 def test_from_scratch_sets(manage_rundir):
     outdir = os.path.join(run_dir,'from_scratch_sets')
     if not os.path.exists(outdir):
         os.mkdir(outdir)
 
     with gdxpds.gdx.GdxFile() as gdx:
         gdx.append(gdxpds.gdx.GdxSymbol('my_set',gdxpds.gdx.GamsDataType.Set,dims=['u']))
-        data = pds.DataFrame([['u' + str(i)] for i in range(1,11)])
+        data = pd.DataFrame([['u' + str(i)] for i in range(1,11)])
         data['Value'] = True
         gdx[-1].dataframe = data
         assert isinstance(gdx[-1].dataframe[gdx[-1].dataframe.columns[-1]].values[0], c_bool)
         gdx.append(gdxpds.gdx.GdxSymbol('my_other_set',gdxpds.gdx.GamsDataType.Set,dims=['u']))
-        data = pds.DataFrame([['u' + str(i)] for i in range(1,11)],columns=['u'])
+        data = pd.DataFrame([['u' + str(i)] for i in range(1,11)],columns=['u'])
         data['Value'] = True
-        gdx[-1].dataframe = gdx[-1].dataframe.append(data)        
+        gdx[-1].dataframe = pd.concat([gdx[-1].dataframe,data])
         gdx.write(os.path.join(outdir,'my_sets.gdx'))
 
     with gdxpds.gdx.GdxFile(lazy_load=False) as gdx:
         gdx.read(os.path.join(outdir,'my_sets.gdx'))
         for sym in gdx:
             assert sym.num_dims == 1
             assert sym.dims[0] == 'u'
             assert sym.data_type == gdxpds.gdx.GamsDataType.Set
             assert sym.num_records == 10
             assert isinstance(sym.dataframe[sym.dataframe.columns[-1]].values[0],c_bool)
 
 
 def test_unnamed_dimensions(manage_rundir):
-    outdir = os.path.join(run_dir,'unnamed_dimensions')
-    if not os.path.exists(outdir):
-        os.mkdir(outdir)
+    from pathlib import Path
+    outdir = Path(run_dir) / 'unnamed_dimensions'
+    if not outdir.exists():
+        outdir.mkdir()
     # create a gdx file with all symbol types and 4 dimensions named '*'
     cols = ['*'] * 4
-    some_entries = pds.DataFrame([['tech_1','year_2','low','h1'],
+    some_entries = pd.DataFrame([['tech_1','year_2','low','h1'],
                                   ['tech_1','year_2','low','h2'],
                                   ['tech_1','year_2','low','h3'],
                                   ['tech_1','year_2','low','h4']],
                                  columns = cols)
 
     with gdxpds.gdx.GdxFile() as gdx:
         # Set
@@ -98,33 +62,33 @@
         # Parmeter
         a_param = copy.deepcopy(some_entries)
         a_param['Value'] = [1.0, 2.0, 3.0, 4.0]
         gdx.append(gdxpds.gdx.GdxSymbol('star_param',gdxpds.gdx.GamsDataType.Parameter,dims=4))
         gdx[-1].dataframe = a_param
         # Test changing the parameter data
         a_param.iloc[:,0] = 'tech_2'
-        gdx[-1].dataframe = pds.concat([gdx[-1].dataframe,a_param])
+        gdx[-1].dataframe = pd.concat([gdx[-1].dataframe,a_param])
         # Variable
         gdx.append(gdxpds.gdx.GdxSymbol('star_var',gdxpds.gdx.GamsDataType.Variable,dims=4,
                    variable_type=gdxpds.gdx.GamsVariableType.Positive))
         a_var = copy.deepcopy(some_entries)
         for value_col_name in gdx[-1].value_col_names:
             a_var[value_col_name] = gdx[-1].get_value_col_default(value_col_name)
         gdx[-1].dataframe = a_var
         # Equation
         gdx.append(gdxpds.gdx.GdxSymbol('star_eqn',gdxpds.gdx.GamsDataType.Equation,dims=4,
                    equation_type=gdxpds.gdx.GamsEquationType.GreaterThan))
         an_eqn = copy.deepcopy(some_entries)
         for value_col_name in gdx[-1].value_col_names:
             an_eqn[value_col_name] = gdx[-1].get_value_col_default(value_col_name)
         gdx[-1].dataframe = an_eqn
-        gdx.write(os.path.join(outdir,'star_symbols.gdx'))
+        gdx.write(outdir / 'star_symbols.gdx')
         
     with gdxpds.gdx.GdxFile(lazy_load=False) as gdx:
-        gdx.read(os.path.join(outdir,'star_symbols.gdx'))
+        gdx.read(outdir / 'star_symbols.gdx')
         assert gdx['star_set'].num_dims == 4
         assert gdx['star_set'].data_type == gdxpds.gdx.GamsDataType.Set
         assert gdx['star_set'].variable_type is None
         assert gdx['star_set'].equation_type is None
         assert gdx['star_param'].num_dims == 4
         assert gdx['star_param'].data_type == gdxpds.gdx.GamsDataType.Parameter
         assert gdx['star_param'].variable_type is None
@@ -148,15 +112,15 @@
         # reading is tested elsewhere. here go through the different ways to
         # set a dataframe. 
         
         # start with WAYS THAT WORK:
         # 0 dims
         #     full dataframe
         gdx.append(gdxpds.gdx.GdxSymbol('sym_1',gdxpds.gdx.GamsDataType.Parameter))
-        gdx[-1].dataframe = pds.DataFrame([[2.0]])
+        gdx[-1].dataframe = pd.DataFrame([[2.0]])
         assert list(gdx[-1].dataframe.columns) == ['Value']
         #     edit initialized dataframe - Parameter
         gdx.append(gdxpds.gdx.GdxSymbol('sym_2',gdxpds.gdx.GamsDataType.Parameter))
         n = len(gdx[-1].dataframe.columns)
         gdx[-1].dataframe['Value'] = [5.0] # list is required to specify number of rows to make
         assert n == len(gdx[-1].dataframe.columns)
         #     list of lists
@@ -165,22 +129,22 @@
         for value_col_name in gdx[-1].value_col_names:
             if value_col_name == 'Level':
                 continue
             values.append(gdx[-1].get_value_col_default(value_col_name))
         gdx[-1].dataframe = [values]
         #     reset with empty list
         gdx.append(gdxpds.gdx.GdxSymbol('sym_4',gdxpds.gdx.GamsDataType.Parameter))
-        gdx[-1].dataframe = pds.DataFrame([[1.0]])
+        gdx[-1].dataframe = pd.DataFrame([[1.0]])
         gdx[-1].dataframe = []
         assert gdx[-1].num_records == 0
 
         # > 0 dims - GdxSymbol initialized with dims=0
         #     full dataframe
         gdx.append(gdxpds.gdx.GdxSymbol('sym_5',gdxpds.gdx.GamsDataType.Parameter))
-        gdx[-1].dataframe = pds.DataFrame([['u1','CC',8727.2],
+        gdx[-1].dataframe = pd.DataFrame([['u1','CC',8727.2],
                                            ['u2','CC',7500.2],
                                            ['u3','CT',9258.0]], 
                                           columns=['u','q','val'])
         assert gdx[-1].num_dims == 2
         assert gdx[-1].num_records == 3
         #     full list of lists
         gdx.append(gdxpds.gdx.GdxSymbol('sym_6',gdxpds.gdx.GamsDataType.Parameter))
@@ -197,26 +161,26 @@
         assert gdx[-1].num_dims == 2
         assert gdx[-1].num_records == 0
 
         # > 0 dims - GdxSymbol initialized with dims=n
         #     dataframe of dims
         gdx.append(gdxpds.gdx.GdxSymbol('sym_8',gdxpds.gdx.GamsDataType.Variable,
             dims=3,variable_type=gdxpds.gdx.GamsVariableType.Positive))
-        gdx[-1].dataframe = pds.DataFrame([['u0','BES','c2'],
+        gdx[-1].dataframe = pd.DataFrame([['u0','BES','c2'],
                                            ['u0','BES','c1'],
                                            ['u1','BES','c2']])
         assert gdx[-1].num_dims == 3
         assert gdx[-1].dims == ['*','*','*']
         assert len(gdx[-1].dataframe.columns) > 3
         gdx[-1].dataframe.loc[:,gdxpds.gdx.GamsValueType.Level.name] = 1.0
         gdx[-1].dataframe.loc[:,gdxpds.gdx.GamsValueType.Upper.name] = 10.0
         #     full dataframe
         gdx.append(gdxpds.gdx.GdxSymbol('sym_9',gdxpds.gdx.GamsDataType.Parameter,
             dims=3))
-        gdx[-1].dataframe = pds.DataFrame([['u0','BES','c2',2.0],
+        gdx[-1].dataframe = pd.DataFrame([['u0','BES','c2',2.0],
                                            ['u0','BES','c1',1.0],
                                            ['u1','BES','c2',2.0]],
                                           columns=['u','q','c','storage_duration_h'])
         assert list(gdx[-1].dataframe.columns) == ['u','q','c','Value']
         #     list of lists containing dims only
         gdx.append(gdxpds.gdx.GdxSymbol('sym_10',gdxpds.gdx.GamsDataType.Equation,
             dims=4,equation_type=gdxpds.gdx.GamsEquationType.LessThan))
@@ -244,26 +208,26 @@
         assert gdx[-1].dims == ['*'] * 2
         assert gdx[-1].num_records == 0
 
         # > 0 dims - GdxSymbol initialized with dims=[list of actual dims]
         #     dataframe of dims
         gdx.append(gdxpds.gdx.GdxSymbol('sym_13',gdxpds.gdx.GamsDataType.Variable,
             dims=['u','q','c'],variable_type=gdxpds.gdx.GamsVariableType.Positive))
-        gdx[-1].dataframe = pds.DataFrame([['u0','BES','c2'],
+        gdx[-1].dataframe = pd.DataFrame([['u0','BES','c2'],
                                            ['u0','BES','c1'],
                                            ['u1','BES','c2']])
         assert gdx[-1].num_dims == 3
         assert gdx[-1].dims == ['u','q','c']
         assert len(gdx[-1].dataframe.columns) > 3
         gdx[-1].dataframe[gdxpds.gdx.GamsValueType.Level.name] = 1.0
         gdx[-1].dataframe[gdxpds.gdx.GamsValueType.Upper.name] = 10.0
         #     full dataframe
         gdx.append(gdxpds.gdx.GdxSymbol('sym_14',gdxpds.gdx.GamsDataType.Parameter,
             dims=['u','q','c']))
-        gdx[-1].dataframe = pds.DataFrame([['u0','BES','c2',2.0],
+        gdx[-1].dataframe = pd.DataFrame([['u0','BES','c2',2.0],
                                            ['u0','BES','c1',1.0],
                                            ['u1','BES','c2',2.0]],
                                           columns=['u','q','c','storage_duration_h'])
         assert list(gdx[-1].dataframe.columns) == ['u','q','c','Value']
         #     list of lists containing dims only
         gdx.append(gdxpds.gdx.GdxSymbol('sym_15',gdxpds.gdx.GamsDataType.Equation,
             dims=['u','q','c','t'],equation_type=gdxpds.gdx.GamsEquationType.LessThan))
@@ -320,15 +284,15 @@
         with pytest.raises(Exception) as _excinfo:
             gdx[-1].dataframe = tmp
         #     full dataframe of different number of dims
         gdx.append(gdxpds.gdx.GdxSymbol('sym_21',gdxpds.gdx.GamsDataType.Parameter,
             dims=6))
         assert gdx[-1].dims == ['*'] * 6
         with pytest.raises(Exception) as e_info:
-            gdx[-1].dataframe = pds.DataFrame([['1',6.0],
+            gdx[-1].dataframe = pd.DataFrame([['1',6.0],
                                               ['2',7.0],
                                               ['3',-12.0]])
         #     list of lists of varying widths
         gdx.append(gdxpds.gdx.GdxSymbol('sym_22',gdxpds.gdx.GamsDataType.Parameter,
             dims=3))
         with pytest.raises(Exception) as e_info:
             gdx[-1].dataframe = [[1]]
```

### Comparing `gdxpds-1.2.0/PKG-INFO` & `gdxpds-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,56 @@
-Metadata-Version: 1.0
+Metadata-Version: 2.1
 Name: gdxpds
-Version: 1.2.0
-Summary: Python package to translate between gdx (GAMS data) and pandas.
+Version: 1.3.0
+Summary: gdx-pandas is a python package to translate between gdx (GAMS data) and pandas
 Home-page: https://github.com/NREL/gdx-pandas
 Author: Elaine T. Hale
 Author-email: elaine.hale@nrel.gov
-License: UNKNOWN
-Description: gdx-pandas: Python package to translate between gdx (GAMS data) and pandas. 
-        
-        There are two main ways to use gdxpds. The first use case is the one that was 
-        initially supported: direct conversion between GDX files on disk and pandas 
-        DataFrames or a csv version thereof. Starting with the Version 1.0.0 rewrite,
-        there is now a second style of use which involves interfacing with GDX files and 
-        symbols via the `gdxpds.gdx.GdxFile` and `gdxpds.gdx.GdxSymbol` classes.
-        
-        Please visit https://nrel.github.io/gdx-pandas for the latest documentation.
-        
-        
-        DEPENDENCIES
-        
-        - Python 3.4 or 3.6 (gdx-pandas support for Python 2.X has been discontinued; GAMS does not yet support Python 3.7)
-        - pandas (In general you will want the SciPy stack. Anaconda comes with it, or see [my notes for Windows](https://elainethale.wordpress.com/programming-notes/python-environment-set-up/).)
-        - For Python versions < 3.4, enum34. Also **uninstall the enum package** if it is installed.
-        - Install [GAMS](https://www.gams.com/download/)
-        - Put the GAMS directory in your `PATH` and/or assign it to the `GAMS_DIR` environment variable
-        - GAMS Python bindings
-            - See GAMS/win64/XX.X/apifiles/readme.txt on Windows, 
-              GAMS/gamsXX.X_osx_x64_64_sfx/apifiles/readme.txt on Mac, or 
-              /opt/gams/gamsXX.X_linux_x64_64_sfx/apifiles/readme.txt on Linux
-            - Run the following for the correct version of the Python bindings
-                
-                ```bash
-                python setup.py install
-                ```
-        
-                or 
-        
-                ```bash
-                python setup.py build --build-base=/path/to/somwhere/you/have/write/access install
-                ```
-        
-                with the latter being for the case when you can install packages into 
-                Python but don't have GAMS directory write access.
-        
-            - For Python 3.X, use 
-              .../apifiles/Python/api_XX/setup.py. For Python 3.X in particular you will 
-              need GAMS version >= 24.5.1 (Python 3.4, Windows and Linux), 
-              24.7.4 (Python 3.4, Mac OS X), or >= 24.8.4 (Python 3.6)
-        
-        
-        TESTING
-        
-        After installation, you can test the package using pytest:
-        
-        pytest --pyargs gdxpds
-        
-        If the tests fail due to permission IOErrors, apply `chmod g+x` and `chmod a+x` 
-        to the `gdx-pandas/gdxpds/test` folder.
-        
-Platform: UNKNOWN
+Description-Content-Type: text/markdown
+Provides-Extra: test
+Provides-Extra: admin
+License-File: LICENSE
+
+gdx-pandas: Python package to translate between gdx (GAMS data) and pandas. 
+
+There are two main ways to use gdxpds. The first use case is the one that was 
+initially supported: direct conversion between GDX files on disk and pandas 
+DataFrames or a csv version thereof. Starting with the Version 1.0.0 rewrite,
+there is now a second style of use which involves interfacing with GDX files and 
+symbols via the `gdxpds.gdx.GdxFile` and `gdxpds.gdx.GdxSymbol` classes.
+
+Please visit https://nrel.github.io/gdx-pandas for the latest documentation.
+
+
+DEPENDENCIES
+
+- Python 3.7 or higher (exact compatibility might depend on which GAMS version you are using)
+- pandas (In general you will want the SciPy stack. Anaconda comes with it, or see [my notes for Windows](https://elainethale.wordpress.com/programming-notes/python-environment-set-up/).)
+- Install [GAMS](https://www.gams.com/download/)
+- Put the GAMS directory in your `PATH` and/or assign it to the `GAMS_DIR` environment variable
+- GAMS Python bindings
+    - See GAMS/**/apifiles/readme.txt on Windows and Mac, or 
+      /opt/gams/**/apifiles/readme.txt on Linux
+    - Run the following for the correct version of the Python bindings (e.g., from the GAMS/**/apifiles/Python/api_39 folder):
+        
+        ```bash
+        python setup.py install
+        ```
+
+        or 
+
+        ```bash
+        python setup.py build --build-base={temporary-path-where-you-have-write-access} install
+        ```
+
+        with the latter being for the case when you can install packages into 
+        Python but don't have GAMS directory write access.
+
+
+TESTING
+
+After installation, you can test the package using pytest:
+
+pytest --pyargs gdxpds
+
+If the tests fail due to permission IOErrors, apply `chmod g+x` and `chmod a+x` 
+to the `gdx-pandas/gdxpds/test` folder.
```

### Comparing `gdxpds-1.2.0/README.md` & `gdxpds-1.3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,42 +6,36 @@
 
 [Install](#install) | [Documentation](https://nrel.github.io/gdx-pandas) | [Uninstall](#uninstall)
 
 ## Install
 
 ### Preliminaries
 
-- Python 3.4 or 3.6 (gdx-pandas support for Python 2.X has been discontinued; GAMS does not yet support Python 3.7)
+- Python 3.7 or higher (exact compatibility might depend on which GAMS version you are using)
 - pandas (In general you will want the SciPy stack. Anaconda comes with it, or see [my notes for Windows](https://elainethale.wordpress.com/programming-notes/python-environment-set-up/).)
-- For Python versions < 3.4, enum34. Also **uninstall the enum package** if it is installed.
 - Install [GAMS](https://www.gams.com/download/)
 - Put the GAMS directory in your `PATH` and/or assign it to the `GAMS_DIR` environment variable
 - GAMS Python bindings
-    - See GAMS/win64/XX.X/apifiles/readme.txt on Windows, 
-      GAMS/gamsXX.X_osx_x64_64_sfx/apifiles/readme.txt on Mac, or 
-      /opt/gams/gamsXX.X_linux_x64_64_sfx/apifiles/readme.txt on Linux
-    - Run the following for the correct version of the Python bindings
+    - See GAMS/**/apifiles/readme.txt on Windows and Mac, or 
+      /opt/gams/**/apifiles/readme.txt on Linux
+    - Run the following for the correct version of the Python bindings (e.g., from the GAMS/**/apifiles/Python/api_39 folder):
         
         ```bash
         python setup.py install
         ```
 
         or 
 
         ```bash
-        python setup.py build --build-base=/path/to/somwhere/you/have/write/access install
+        python setup.py build --build-base={temporary-path-where-you-have-write-access} install
         ```
 
         with the latter being for the case when you can install packages into 
         Python but don't have GAMS directory write access.
-
-    - For Python 3.X, use 
-      .../apifiles/Python/api_XX/setup.py. For Python 3.X in particular you will 
-      need GAMS version >= 24.5.1 (Python 3.4, Windows and Linux), 
-      24.7.4 (Python 3.4, Mac OS X), or >= 24.8.4 (Python 3.6)
+    - If `import gdxcc` fails (which will also cause `import gdxpds` to fail) because there "is no `_gdxcc` module", one workaround is to copy all the `_*.pyd` (or `_*.so`) files from GAMS/**/apifiles/Python/api_XX/ and paste them into your Python environment next to, e.g., the `gdxcc-8-py3.9.egg` file, which on Anaconda is your environment's lib/site-packages directory.
 
 ### Get the Latest Package
 
 ```bash
 pip install gdxpds
 ```
```

### Comparing `gdxpds-1.2.0/README.txt` & `gdxpds-1.3.0/README.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,43 +7,36 @@
 symbols via the `gdxpds.gdx.GdxFile` and `gdxpds.gdx.GdxSymbol` classes.
 
 Please visit https://nrel.github.io/gdx-pandas for the latest documentation.
 
 
 DEPENDENCIES
 
-- Python 3.4 or 3.6 (gdx-pandas support for Python 2.X has been discontinued; GAMS does not yet support Python 3.7)
+- Python 3.7 or higher (exact compatibility might depend on which GAMS version you are using)
 - pandas (In general you will want the SciPy stack. Anaconda comes with it, or see [my notes for Windows](https://elainethale.wordpress.com/programming-notes/python-environment-set-up/).)
-- For Python versions < 3.4, enum34. Also **uninstall the enum package** if it is installed.
 - Install [GAMS](https://www.gams.com/download/)
 - Put the GAMS directory in your `PATH` and/or assign it to the `GAMS_DIR` environment variable
 - GAMS Python bindings
-    - See GAMS/win64/XX.X/apifiles/readme.txt on Windows, 
-      GAMS/gamsXX.X_osx_x64_64_sfx/apifiles/readme.txt on Mac, or 
-      /opt/gams/gamsXX.X_linux_x64_64_sfx/apifiles/readme.txt on Linux
-    - Run the following for the correct version of the Python bindings
+    - See GAMS/**/apifiles/readme.txt on Windows and Mac, or 
+      /opt/gams/**/apifiles/readme.txt on Linux
+    - Run the following for the correct version of the Python bindings (e.g., from the GAMS/**/apifiles/Python/api_39 folder):
         
         ```bash
         python setup.py install
         ```
 
         or 
 
         ```bash
-        python setup.py build --build-base=/path/to/somwhere/you/have/write/access install
+        python setup.py build --build-base={temporary-path-where-you-have-write-access} install
         ```
 
         with the latter being for the case when you can install packages into 
         Python but don't have GAMS directory write access.
 
-    - For Python 3.X, use 
-      .../apifiles/Python/api_XX/setup.py. For Python 3.X in particular you will 
-      need GAMS version >= 24.5.1 (Python 3.4, Windows and Linux), 
-      24.7.4 (Python 3.4, Mac OS X), or >= 24.8.4 (Python 3.6)
-
 
 TESTING
 
 After installation, you can test the package using pytest:
 
 pytest --pyargs gdxpds
```

