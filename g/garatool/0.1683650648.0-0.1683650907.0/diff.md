# Comparing `tmp/garatool-0.1683650648.0.tar.gz` & `tmp/garatool-0.1683650907.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garatool-0.1683650648.0.tar", last modified: Tue May  9 16:44:08 2023, max compression
+gzip compressed data, was "garatool-0.1683650907.0.tar", last modified: Tue May  9 16:48:27 2023, max compression
```

## Comparing `garatool-0.1683650648.0.tar` & `garatool-0.1683650907.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:44:08.849339 garatool-0.1683650648.0/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:44:08.848932 garatool-0.1683650648.0/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683650648.0/README.md
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:44:08.843804 garatool-0.1683650648.0/garatool/
--rw-r--r--   0 curlyz     (501) staff       (20)     5742 2023-05-09 16:35:34.000000 garatool-0.1683650648.0/garatool/__init__.py
-drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:44:08.848312 garatool-0.1683650648.0/garatool.egg-info/
--rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:44:08.000000 garatool-0.1683650648.0/garatool.egg-info/PKG-INFO
--rw-r--r--   0 curlyz     (501) staff       (20)      198 2023-05-09 16:44:08.000000 garatool-0.1683650648.0/garatool.egg-info/SOURCES.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 16:44:08.000000 garatool-0.1683650648.0/garatool.egg-info/dependency_links.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 16:44:08.000000 garatool-0.1683650648.0/garatool.egg-info/requires.txt
--rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 16:44:08.000000 garatool-0.1683650648.0/garatool.egg-info/top_level.txt
--rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 16:44:08.849439 garatool-0.1683650648.0/setup.cfg
--rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683650648.0/setup.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:48:27.442038 garatool-0.1683650907.0/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:48:27.441700 garatool-0.1683650907.0/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)        0 2023-05-09 14:06:02.000000 garatool-0.1683650907.0/README.md
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:48:27.438640 garatool-0.1683650907.0/garatool/
+-rw-r--r--   0 curlyz     (501) staff       (20)     5845 2023-05-09 16:48:09.000000 garatool-0.1683650907.0/garatool/__init__.py
+-rw-r--r--   0 curlyz     (501) staff       (20)       64 2023-05-09 16:48:25.000000 garatool-0.1683650907.0/garatool/__main__.py
+drwxr-xr-x   0 curlyz     (501) staff       (20)        0 2023-05-09 16:48:27.441165 garatool-0.1683650907.0/garatool.egg-info/
+-rw-r--r--   0 curlyz     (501) staff       (20)      286 2023-05-09 16:48:27.000000 garatool-0.1683650907.0/garatool.egg-info/PKG-INFO
+-rw-r--r--   0 curlyz     (501) staff       (20)      219 2023-05-09 16:48:27.000000 garatool-0.1683650907.0/garatool.egg-info/SOURCES.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        1 2023-05-09 16:48:27.000000 garatool-0.1683650907.0/garatool.egg-info/dependency_links.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       51 2023-05-09 16:48:27.000000 garatool-0.1683650907.0/garatool.egg-info/requires.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)        9 2023-05-09 16:48:27.000000 garatool-0.1683650907.0/garatool.egg-info/top_level.txt
+-rw-r--r--   0 curlyz     (501) staff       (20)       38 2023-05-09 16:48:27.442140 garatool-0.1683650907.0/setup.cfg
+-rw-r--r--   0 curlyz     (501) staff       (20)     1102 2023-05-09 16:41:54.000000 garatool-0.1683650907.0/setup.py
```

### Comparing `garatool-0.1683650648.0/garatool/__init__.py` & `garatool-0.1683650907.0/garatool/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 parser.add_argument('-n', '--name', help='Device name', default='Creator Device')
 parser.add_argument('-s', '--serial', action='store_true', help='Enable Serial debug')
 parser.add_argument('-u', '--upload', help='(Admin) Publish firmware tag',action='store_true')
 parser.add_argument('-k', '--key', help='(Admin) With secret key', default='')
 parser.add_argument('-r', '--root', help='(Admin) Location of firmware', default='')
 
 
-def get_mac(port: str, nostub: bool) -> str: 
+def get_mac(port: str, nostub: bool) -> str:
     output = subprocess.getoutput(
         cmd(' '.join([
             ESPTOOL,
             '-p', port,
             '--no-stub' if  nostub else ' ',
             'read_mac'
         ]))
@@ -95,54 +95,54 @@
     imei: str = ''
     name: str = 'Creator Device'
     tag: str = ''
     key: str = ''
     event: str = 'build_firmware'
     uuid: str = ''
     files: dict = field(default_factory=dict)
-    
-    
+
+
     root: str = ''
     upload: bool = False
     key: str = ''
     # Segments from server response
     partitions: list = field(default_factory=list)
     status: str = ''
     event: str = ''
-    
-    
+
+
 def request_firmware_build(br: BuildRequest):
     req = requests.post(
         url = 'https://api.garastem.com/api/v1/toolchain/garatool',
         data = msgpack.dumps(asdict(br))
     )
     print(req, flag(req.status_code))
     if req.status_code != 200:
         raise Exception('Problem: ' + req.text)
     response = dacite.from_dict(BuildRequest, msgpack.loads(req.content, raw=False))
     # print('Response', flag(response))
     return response
-    
-    
+
+
 def publish_tag(tag: str, key: str):
     print(step('publishing tag'), flag(tag))
     br.event = 'publish_firmware'
     req = requests.post(
         url = 'https://api.garastem.com/api/v1/toolchain/garatool',
         data = msgpack.dumps(asdict(br))
     )
 
 def program_device(br: BuildRequest):
     for parti in br.partitions:
         print(parti['file'], parti['offset'], len(parti['data']))
         with open(parti['file'], 'wb') as f:
             f.write(parti['data'])
-        
-        
-        
+
+
+
     partition_params = ' '.join([
         f"{p['offset']} {p['file']}" for p in br.partitions
     ])
 
     os.system(cmd(' '.join([
         ESPTOOL,
         '-p', parsed.port,
@@ -152,65 +152,65 @@
         '--after=hard_reset',
         '--chip', 'auto',
         'write_flash',
         '--flash_mode=dio',
         '--flash_size=keep',
         partition_params
     ])))
-    
+
     for parti in br.partitions:
         try:
             os.remove(parti['file'])
         except OSError:
             pass
-    
-    
 
-br = BuildRequest()
-br.event = 'build_firmware'
-br.name = parsed.name
-br.imei = parsed.imei
-br.tag = parsed.tag
-br.key = parsed.key
-br.upload = parsed.upload
-br.key = parsed.key
-br.uuid = str(uuid.uuid4())
-
-if parsed.board == Board.CreatorPlus:
-    br.chipset = 'GENERIC_C3_USB'
-    br.nostub = True
-elif parsed.board == Board.CreatorIoT:
-    br.chipset = 'GENERIC_SPIRAM'
-    br.nostub = False
-
-if parsed.port:
-    print('Port: Connecting to serial ', flag(parsed.port))
-    # if port is available then get the mac
-    br.mac = get_mac(parsed.port, br.nostub)
-
-
-if parsed.upload:
-    # gather list of flat files
-    fws = dict()
-    print('Gathering file from root', flag(parsed.root))
-    for file in os.listdir(parsed.root):
-        if not (file.endswith('.py') or file.endswith('.pym')): continue
-        if file.startswith('__'): continue
-        print(file)
-        content = open(
-            os.path.join(parsed.root, file)
-        , 'rb').read()
-        fws[file] = content
-    br.files = fws
-
-    
+
+def start():
+    br = BuildRequest()
+    br.event = 'build_firmware'
+    br.name = parsed.name
+    br.imei = parsed.imei
+    br.tag = parsed.tag
+    br.key = parsed.key
+    br.upload = parsed.upload
+    br.key = parsed.key
+    br.uuid = str(uuid.uuid4())
+
+    if parsed.board == Board.CreatorPlus:
+        br.chipset = 'GENERIC_C3_USB'
+        br.nostub = True
+    elif parsed.board == Board.CreatorIoT:
+        br.chipset = 'GENERIC_SPIRAM'
+        br.nostub = False
+
+    if parsed.port:
+        print('Port: Connecting to serial ', flag(parsed.port))
+        # if port is available then get the mac
+        br.mac = get_mac(parsed.port, br.nostub)
+
+
+    if parsed.upload:
+        # gather list of flat files
+        fws = dict()
+        print('Gathering file from root', flag(parsed.root))
+        for file in os.listdir(parsed.root):
+            if not (file.endswith('.py') or file.endswith('.pym')): continue
+            if file.startswith('__'): continue
+            print(file)
+            content = open(
+                os.path.join(parsed.root, file)
+            , 'rb').read()
+            fws[file] = content
+        br.files = fws
+
+
 
 
 
-br = request_firmware_build(br)
-# Start burning firmware
-program_device(br)
-
-if parsed.serial:
-    if platform.platform() == 'darwin':
-        os.system('say start')
-        os.system(f'screen {parsed.port} 115200')
+    br = request_firmware_build(br)
+    # Start burning firmware
+    program_device(br)
+
+    if parsed.serial:
+        if platform.platform() == 'darwin':
+            os.system('say start')
+            os.system(f'screen {parsed.port} 115200')
```

### Comparing `garatool-0.1683650648.0/setup.py` & `garatool-0.1683650907.0/setup.py`

 * *Files identical despite different names*

