# Comparing `tmp/MomentumX-2.6.5.tar.gz` & `tmp/MomentumX-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MomentumX-2.6.5.tar", last modified: Mon Apr 24 15:55:41 2023, max compression
+gzip compressed data, was "MomentumX-2.7.0.tar", last modified: Tue May  9 16:22:34 2023, max compression
```

## Comparing `MomentumX-2.6.5.tar` & `MomentumX-2.7.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.847183 MomentumX-2.6.5/
--rw-rw-r--   0 developer  (1000) developer  (1000)      143 2023-02-05 03:27:25.000000 MomentumX-2.6.5/.clang-format
--rw-rw-r--   0 developer  (1000) developer  (1000)       39 2023-01-04 18:56:42.000000 MomentumX-2.6.5/.dockerignore
--rw-rw-r--   0 developer  (1000) developer  (1000)       93 2023-03-02 22:42:30.000000 MomentumX-2.6.5/.gitignore
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.841183 MomentumX-2.6.5/.vscode/
--rw-rw-r--   0 developer  (1000) developer  (1000)      280 2023-03-02 22:42:30.000000 MomentumX-2.6.5/.vscode/settings.json
--rw-rw-r--   0 developer  (1000) developer  (1000)     1968 2023-03-09 18:12:19.000000 MomentumX-2.6.5/CMakeLists.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)    35149 2022-05-19 01:23:36.000000 MomentumX-2.6.5/LICENSE
--rwxrwxr-x   0 developer  (1000) developer  (1000)     6518 2023-01-10 14:44:56.000000 MomentumX-2.6.5/Logo.png
--rw-rw-r--   0 developer  (1000) developer  (1000)     1359 2023-03-09 18:12:19.000000 MomentumX-2.6.5/Makefile
--rw-rw-r--   0 developer  (1000) developer  (1000)     7125 2023-04-24 15:55:41.847183 MomentumX-2.6.5/PKG-INFO
--rw-rw-r--   0 developer  (1000) developer  (1000)     6667 2023-03-10 16:59:42.000000 MomentumX-2.6.5/README.md
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.844183 MomentumX-2.6.5/examples/
--rw-rw-r--   0 developer  (1000) developer  (1000)     1675 2023-03-09 18:12:19.000000 MomentumX-2.6.5/examples/multi.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1120 2023-03-09 18:12:19.000000 MomentumX-2.6.5/examples/stream_reader.py
--rwxrwxr-x   0 developer  (1000) developer  (1000)      865 2023-03-09 18:12:19.000000 MomentumX-2.6.5/examples/stream_writer.py
--rw-rw-r--   0 developer  (1000) developer  (1000)      762 2023-04-12 13:12:35.000000 MomentumX-2.6.5/examples/sync_reader.py
--rwxrwxr-x   0 developer  (1000) developer  (1000)      583 2023-04-12 13:12:35.000000 MomentumX-2.6.5/examples/sync_writer.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     1024 2023-04-24 15:44:52.000000 MomentumX-2.6.5/examples/threaded.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.845183 MomentumX-2.6.5/ext/
--rw-rw-r--   0 developer  (1000) developer  (1000)    22135 2023-04-24 15:44:52.000000 MomentumX-2.6.5/ext/binding.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     6517 2023-03-09 18:12:19.000000 MomentumX-2.6.5/ext/buffer.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     4214 2023-03-09 18:12:19.000000 MomentumX-2.6.5/ext/buffer.h
--rw-rw-r--   0 developer  (1000) developer  (1000)     4748 2023-03-10 15:53:52.000000 MomentumX-2.6.5/ext/context.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     1467 2023-03-10 15:53:52.000000 MomentumX-2.6.5/ext/context.h
--rw-rw-r--   0 developer  (1000) developer  (1000)    21067 2023-04-12 13:12:35.000000 MomentumX-2.6.5/ext/stream.cpp
--rw-rw-r--   0 developer  (1000) developer  (1000)     5141 2023-03-10 15:53:52.000000 MomentumX-2.6.5/ext/stream.h
--rw-rw-r--   0 developer  (1000) developer  (1000)     9498 2023-03-09 18:12:19.000000 MomentumX-2.6.5/ext/utils.h
--rw-rw-r--   0 developer  (1000) developer  (1000)      133 2023-04-24 15:44:52.000000 MomentumX-2.6.5/pyproject.toml
--rw-rw-r--   0 developer  (1000) developer  (1000)       38 2023-04-24 15:55:41.847183 MomentumX-2.6.5/setup.cfg
--rw-rw-r--   0 developer  (1000) developer  (1000)     1023 2023-04-24 15:47:16.000000 MomentumX-2.6.5/setup.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.837183 MomentumX-2.6.5/src/
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.846183 MomentumX-2.6.5/src/MomentumX.egg-info/
--rw-rw-r--   0 developer  (1000) developer  (1000)     7125 2023-04-24 15:55:41.000000 MomentumX-2.6.5/src/MomentumX.egg-info/PKG-INFO
--rw-rw-r--   0 developer  (1000) developer  (1000)      665 2023-04-24 15:55:41.000000 MomentumX-2.6.5/src/MomentumX.egg-info/SOURCES.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)        1 2023-04-24 15:55:41.000000 MomentumX-2.6.5/src/MomentumX.egg-info/dependency_links.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)       21 2023-04-24 15:55:41.000000 MomentumX-2.6.5/src/MomentumX.egg-info/requires.txt
--rw-rw-r--   0 developer  (1000) developer  (1000)       10 2023-04-24 15:55:41.000000 MomentumX-2.6.5/src/MomentumX.egg-info/top_level.txt
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.846183 MomentumX-2.6.5/src/momentumx/
--rw-rw-r--   0 developer  (1000) developer  (1000)       20 2023-03-02 22:39:27.000000 MomentumX-2.6.5/src/momentumx/__init__.py
--rw-rw-r--   0 developer  (1000) developer  (1000)     4607 2023-04-24 15:48:19.000000 MomentumX-2.6.5/src/momentumx/_mx.pyi
--rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-03-17 18:13:12.000000 MomentumX-2.6.5/src/momentumx/cli.py
-drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-04-24 15:55:41.846183 MomentumX-2.6.5/tests/
--rw-rw-r--   0 developer  (1000) developer  (1000)    27378 2023-04-12 13:12:35.000000 MomentumX-2.6.5/tests/test_scenarios.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.316607 MomentumX-2.7.0/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      143 2023-02-05 03:27:25.000000 MomentumX-2.7.0/.clang-format
+-rw-rw-r--   0 developer  (1000) developer  (1000)       39 2023-01-04 18:56:42.000000 MomentumX-2.7.0/.dockerignore
+-rw-rw-r--   0 developer  (1000) developer  (1000)       93 2023-03-02 22:42:30.000000 MomentumX-2.7.0/.gitignore
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.307607 MomentumX-2.7.0/.vscode/
+-rw-rw-r--   0 developer  (1000) developer  (1000)      280 2023-03-02 22:42:30.000000 MomentumX-2.7.0/.vscode/settings.json
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1968 2023-03-09 18:12:19.000000 MomentumX-2.7.0/CMakeLists.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)    35149 2022-05-19 01:23:36.000000 MomentumX-2.7.0/LICENSE
+-rwxrwxr-x   0 developer  (1000) developer  (1000)     6518 2023-01-10 14:44:56.000000 MomentumX-2.7.0/Logo.png
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1513 2023-05-09 13:05:53.000000 MomentumX-2.7.0/Makefile
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6900 2023-05-09 16:22:34.315707 MomentumX-2.7.0/PKG-INFO
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6442 2023-05-09 13:07:32.000000 MomentumX-2.7.0/README.md
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.312107 MomentumX-2.7.0/examples/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1675 2023-03-09 18:12:19.000000 MomentumX-2.7.0/examples/multi.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1120 2023-03-09 18:12:19.000000 MomentumX-2.7.0/examples/stream_reader.py
+-rwxrwxr-x   0 developer  (1000) developer  (1000)      865 2023-03-09 18:12:19.000000 MomentumX-2.7.0/examples/stream_writer.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)      762 2023-04-12 13:12:35.000000 MomentumX-2.7.0/examples/sync_reader.py
+-rwxrwxr-x   0 developer  (1000) developer  (1000)      583 2023-04-12 13:12:35.000000 MomentumX-2.7.0/examples/sync_writer.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1024 2023-04-24 15:44:52.000000 MomentumX-2.7.0/examples/threaded.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.313007 MomentumX-2.7.0/ext/
+-rw-rw-r--   0 developer  (1000) developer  (1000)    22135 2023-04-24 15:44:52.000000 MomentumX-2.7.0/ext/binding.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6517 2023-03-09 18:12:19.000000 MomentumX-2.7.0/ext/buffer.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4214 2023-03-09 18:12:19.000000 MomentumX-2.7.0/ext/buffer.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4748 2023-03-10 15:53:52.000000 MomentumX-2.7.0/ext/context.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1467 2023-03-10 15:53:52.000000 MomentumX-2.7.0/ext/context.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)    21069 2023-05-09 13:05:53.000000 MomentumX-2.7.0/ext/stream.cpp
+-rw-rw-r--   0 developer  (1000) developer  (1000)     5141 2023-03-10 15:53:52.000000 MomentumX-2.7.0/ext/stream.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)    11990 2023-05-09 13:05:53.000000 MomentumX-2.7.0/ext/utils.h
+-rw-rw-r--   0 developer  (1000) developer  (1000)      133 2023-04-24 15:44:52.000000 MomentumX-2.7.0/pyproject.toml
+-rw-rw-r--   0 developer  (1000) developer  (1000)       38 2023-05-09 16:22:34.316607 MomentumX-2.7.0/setup.cfg
+-rw-rw-r--   0 developer  (1000) developer  (1000)     1023 2023-05-09 13:06:09.000000 MomentumX-2.7.0/setup.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.303107 MomentumX-2.7.0/src/
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.313907 MomentumX-2.7.0/src/MomentumX.egg-info/
+-rw-rw-r--   0 developer  (1000) developer  (1000)     6900 2023-05-09 16:22:34.000000 MomentumX-2.7.0/src/MomentumX.egg-info/PKG-INFO
+-rw-rw-r--   0 developer  (1000) developer  (1000)      665 2023-05-09 16:22:34.000000 MomentumX-2.7.0/src/MomentumX.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)        1 2023-05-09 16:22:34.000000 MomentumX-2.7.0/src/MomentumX.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)       21 2023-05-09 16:22:34.000000 MomentumX-2.7.0/src/MomentumX.egg-info/requires.txt
+-rw-rw-r--   0 developer  (1000) developer  (1000)       10 2023-05-09 16:22:34.000000 MomentumX-2.7.0/src/MomentumX.egg-info/top_level.txt
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.314807 MomentumX-2.7.0/src/momentumx/
+-rw-rw-r--   0 developer  (1000) developer  (1000)       20 2023-03-02 22:39:27.000000 MomentumX-2.7.0/src/momentumx/__init__.py
+-rw-rw-r--   0 developer  (1000) developer  (1000)     4607 2023-05-09 16:14:07.000000 MomentumX-2.7.0/src/momentumx/_mx.pyi
+-rw-rw-r--   0 developer  (1000) developer  (1000)        0 2023-03-17 18:13:12.000000 MomentumX-2.7.0/src/momentumx/cli.py
+drwxrwxr-x   0 developer  (1000) developer  (1000)        0 2023-05-09 16:22:34.314807 MomentumX-2.7.0/tests/
+-rw-rw-r--   0 developer  (1000) developer  (1000)    27378 2023-04-12 13:12:35.000000 MomentumX-2.7.0/tests/test_scenarios.py
```

### Comparing `MomentumX-2.6.5/CMakeLists.txt` & `MomentumX-2.7.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/LICENSE` & `MomentumX-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/Logo.png` & `MomentumX-2.7.0/Logo.png`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/Makefile` & `MomentumX-2.7.0/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -42,7 +42,11 @@
 	@cp -uv _skbuild/linux-x86_64*/cmake-install/src/momentumx/_mx.pyi src/momentumx/_mx.pyi
 
 .PHONY: test
 test:
 	@rm -rfv rm -rf /dev/shm/mx.test_echo_mx_stream*
 	@python3 -m pytest tests
 
+.PHONY: test/disable_condition
+test/disable_condition:
+	@rm -rfv rm -rf /dev/shm/mx.test_echo_mx_stream*
+	@MX_DISABLE_CONDITION=1 python3 -m pytest tests
```

### Comparing `MomentumX-2.6.5/PKG-INFO` & `MomentumX-2.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MomentumX
-Version: 2.6.5
+Version: 2.7.0
 Summary: Zero-copy shared memory IPC library for building complex streaming data pipelines capable of processing large datasets
 Home-page: https://github.com/captivationsoftware/MomentumX
 Author: Captivation Software, LLC
 Keywords: shm,shared memory,zero-copy,numpy,big data,scipy,pubsub,pipeline
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -35,29 +35,20 @@
 Below are some simplified use cases for common MomentumX workflows. Consult the examples in the `examples/` directory for additional details and implementation guidance.
 
 #### Stream Mode
 ```python
 # Producer Process
 import momentumx as mx
 
-# Create a stream with a total capacity of 10MB
+# Create a stream with a total capacity of 10MB (1MB x 10)
 stream = mx.Producer('my_stream', buffer_size=int(1e6), buffer_count=10, sync=False)
 
-# Write the series 0-9 repeatedly to a buffer 1000 times
+# Obtain the next available buffer for writing
 buffer = stream.next_to_send()
 buffer.write(b'1') 
-# buffer data == b'1'
-
-# alternatively, set via array indexing using python ByteArray syntax...
-buffer[1] = ord('2')
-# buffer data == b'12'
-
-# or also set via python slice operator
-buffer[2:3] = b'34'
-# buffer data == b'1234'
 
 buffer.send()
 # NOTE: buffer.send() can also be passed an explicit number of bytes as well. 
 # Otherwise an internally managed cursor will be used.
 ```
 
 ```python
```

### Comparing `MomentumX-2.6.5/README.md` & `MomentumX-2.7.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,20 @@
 Below are some simplified use cases for common MomentumX workflows. Consult the examples in the `examples/` directory for additional details and implementation guidance.
 
 #### Stream Mode
 ```python
 # Producer Process
 import momentumx as mx
 
-# Create a stream with a total capacity of 10MB
+# Create a stream with a total capacity of 10MB (1MB x 10)
 stream = mx.Producer('my_stream', buffer_size=int(1e6), buffer_count=10, sync=False)
 
-# Write the series 0-9 repeatedly to a buffer 1000 times
+# Obtain the next available buffer for writing
 buffer = stream.next_to_send()
 buffer.write(b'1') 
-# buffer data == b'1'
-
-# alternatively, set via array indexing using python ByteArray syntax...
-buffer[1] = ord('2')
-# buffer data == b'12'
-
-# or also set via python slice operator
-buffer[2:3] = b'34'
-# buffer data == b'1234'
 
 buffer.send()
 # NOTE: buffer.send() can also be passed an explicit number of bytes as well. 
 # Otherwise an internally managed cursor will be used.
 ```
 
 ```python
```

### Comparing `MomentumX-2.6.5/examples/multi.py` & `MomentumX-2.7.0/examples/multi.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/examples/stream_reader.py` & `MomentumX-2.7.0/examples/stream_reader.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/examples/stream_writer.py` & `MomentumX-2.7.0/examples/stream_writer.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/examples/sync_reader.py` & `MomentumX-2.7.0/examples/sync_reader.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/examples/sync_writer.py` & `MomentumX-2.7.0/examples/sync_writer.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/examples/threaded.py` & `MomentumX-2.7.0/examples/threaded.py`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/ext/binding.cpp` & `MomentumX-2.7.0/ext/binding.cpp`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/ext/buffer.cpp` & `MomentumX-2.7.0/ext/buffer.cpp`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/ext/buffer.h` & `MomentumX-2.7.0/ext/buffer.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/ext/context.cpp` & `MomentumX-2.7.0/ext/context.cpp`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/ext/context.h` & `MomentumX-2.7.0/ext/context.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/ext/stream.cpp` & `MomentumX-2.7.0/ext/stream.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -54,18 +54,20 @@
         if (_data == MAP_FAILED) {
             throw std::runtime_error("Failed to mmap shared memory stream file [errno: " + std::to_string(errno) + "]");
         }
 
         _control = reinterpret_cast<ControlBlock*>(_data);
         if (_role == PRODUCER) {
             new (_control) ControlBlock();  // placement construct into shared memory
+
             const auto control_lock = get_control_lock();
             _control->sync = sync;
             _control->buffer_size = buffer_size;
             _control->buffer_count = buffer_count;
+
             Utils::Logger::get_logger().info(std::string("Created Producer Stream (" + std::to_string((uint64_t)this) + ")"));
         } else {
             auto control_lock = get_control_lock();
             if (!_control->is_ready()) {
                 throw std::runtime_error("Attempt to open stream before it is ready");
             }
             _control->subscriber_count++;
```

### Comparing `MomentumX-2.6.5/ext/stream.h` & `MomentumX-2.7.0/ext/stream.h`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/ext/utils.h` & `MomentumX-2.7.0/ext/utils.h`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,24 @@
 #include <fcntl.h>
 #include <signal.h>
 #include <sys/stat.h>
 #include <sys/time.h>
 #include <unistd.h>
 #include <atomic>
 #include <boost/container/static_vector.hpp>
+#include <boost/date_time/posix_time/posix_time.hpp>
+#include <boost/date_time/posix_time/posix_time_types.hpp>
 #include <boost/interprocess/creation_tags.hpp>
 #include <boost/interprocess/sync/interprocess_condition.hpp>
 #include <boost/interprocess/sync/interprocess_sharable_mutex.hpp>
 #include <boost/interprocess/sync/scoped_lock.hpp>
 #include <boost/interprocess/sync/sharable_lock.hpp>
 #include <chrono>
 #include <cmath>
+#include <cstdlib>
 #include <cstring>
 #include <ctime>
 #include <functional>
 #include <initializer_list>
 #include <iostream>
 #include <map>
 #include <memory>
@@ -214,18 +217,78 @@
                 os << ", buffer_path_base: " << paths.buffer_path_base;
                 os << " }";
 
                 return os;
             }
         };
 
+        inline bool is_condition_enabled() {
+            const static bool disable = [] {
+                // stuff this into a static subroutine, so it only is initialized/logged once
+                const char* disable_str = std::getenv("MX_DISABLE_CONDITION");
+                const bool disable = disable_str != nullptr && std::strcmp(disable_str, "1") == 0;
+                if (disable) {
+                    Utils::Logger::get_logger().info(std::string("Disabling condition variables for all producers"));
+                }
+                return disable;
+            }();
+
+            return !disable;
+        }
+
         using OmniMutex = bip::interprocess_mutex;
-        using OmniReadLock = bip::sharable_lock<OmniMutex>;
         using OmniWriteLock = bip::scoped_lock<OmniMutex>;
-        using OmniCondition = bip::interprocess_condition;
+        struct OmniCondition {
+            OmniCondition() = default;
+
+            bip::interprocess_condition inner{};
+
+            /// Compatibility flag to disable conditional and fall back to polling.
+            /// This is enabled or disabled based on the environment of the producer,
+            /// but the consumer will use the same value since it's stored in shared memory.
+            ///
+            /// If true, notify and conditional wait is used. If false, polling is used.
+            bool enabled{is_condition_enabled()};
+
+            inline void notify_one() {
+                if (enabled) {
+                    inner.notify_one();
+                }
+            }
+
+            inline void notify_all() {
+                if (enabled) {
+                    inner.notify_all();
+                }
+            }
+
+            template <typename L, class TimePoint, typename Pr>
+            inline bool timed_wait(L& lock, const TimePoint& abs_time, Pr pred) {
+                if (enabled) {
+                    return inner.timed_wait(lock, abs_time, pred);
+                } else {
+                    // Always check first before looping check
+                    if (pred()) {
+                        return true;
+                    }
+                    constexpr auto increment_dur = std::chrono::milliseconds(50);  // arbitrary
+
+                    // Incrementally sleep until we hit our cutoff time
+                    while (boost::posix_time::microsec_clock::universal_time() < abs_time) {
+                        lock.unlock();
+                        std::this_thread::sleep_for(increment_dur);
+                        lock.lock();
+                        if (pred()) {
+                            return true;
+                        }
+                    }
+                    return false;
+                }
+            }
+        };
 
         template <typename T, size_t Capacity>
         using StaticVector = boost::container::static_vector<T, Capacity>;
     }  // namespace Utils
 
     template <typename T, size_t Capacity>
     inline std::ostream& operator<<(std::ostream& os, const boost::container::static_vector<T, Capacity>& vec) {
```

### Comparing `MomentumX-2.6.5/setup.py` & `MomentumX-2.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages
 from skbuild import setup
 
-__version__ = "2.6.5"
+__version__ = "2.7.0"
 
 from pathlib import Path
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="MomentumX",
     version=__version__,
```

### Comparing `MomentumX-2.6.5/src/MomentumX.egg-info/PKG-INFO` & `MomentumX-2.7.0/src/MomentumX.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MomentumX
-Version: 2.6.5
+Version: 2.7.0
 Summary: Zero-copy shared memory IPC library for building complex streaming data pipelines capable of processing large datasets
 Home-page: https://github.com/captivationsoftware/MomentumX
 Author: Captivation Software, LLC
 Keywords: shm,shared memory,zero-copy,numpy,big data,scipy,pubsub,pipeline
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
@@ -35,29 +35,20 @@
 Below are some simplified use cases for common MomentumX workflows. Consult the examples in the `examples/` directory for additional details and implementation guidance.
 
 #### Stream Mode
 ```python
 # Producer Process
 import momentumx as mx
 
-# Create a stream with a total capacity of 10MB
+# Create a stream with a total capacity of 10MB (1MB x 10)
 stream = mx.Producer('my_stream', buffer_size=int(1e6), buffer_count=10, sync=False)
 
-# Write the series 0-9 repeatedly to a buffer 1000 times
+# Obtain the next available buffer for writing
 buffer = stream.next_to_send()
 buffer.write(b'1') 
-# buffer data == b'1'
-
-# alternatively, set via array indexing using python ByteArray syntax...
-buffer[1] = ord('2')
-# buffer data == b'12'
-
-# or also set via python slice operator
-buffer[2:3] = b'34'
-# buffer data == b'1234'
 
 buffer.send()
 # NOTE: buffer.send() can also be passed an explicit number of bytes as well. 
 # Otherwise an internally managed cursor will be used.
 ```
 
 ```python
```

### Comparing `MomentumX-2.6.5/src/MomentumX.egg-info/SOURCES.txt` & `MomentumX-2.7.0/src/MomentumX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/src/momentumx/_mx.pyi` & `MomentumX-2.7.0/src/momentumx/_mx.pyi`

 * *Files identical despite different names*

### Comparing `MomentumX-2.6.5/tests/test_scenarios.py` & `MomentumX-2.7.0/tests/test_scenarios.py`

 * *Files identical despite different names*

