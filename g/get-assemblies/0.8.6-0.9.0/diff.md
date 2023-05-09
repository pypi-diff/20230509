# Comparing `tmp/get_assemblies-0.8.6.tar.gz` & `tmp/get_assemblies-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_assemblies-0.8.6.tar", last modified: Wed Mar 23 05:55:55 2022, max compression
+gzip compressed data, was "get_assemblies-0.9.0.tar", last modified: Wed Mar 23 06:21:53 2022, max compression
```

## Comparing `get_assemblies-0.8.6.tar` & `get_assemblies-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 davised   (1000) davised   (1000)        0 2022-03-23 05:55:55.524160 get_assemblies-0.8.6/
--rw-r--r--   0 davised   (1000) davised   (1000)     1682 2022-03-23 05:43:59.000000 get_assemblies-0.8.6/LICENSE
--rw-r--r--   0 davised   (1000) davised   (1000)       60 2022-03-23 05:43:59.000000 get_assemblies-0.8.6/MANIFEST.in
--rw-r--r--   0 davised   (1000) davised   (1000)    15049 2022-03-23 05:55:55.523160 get_assemblies-0.8.6/PKG-INFO
--rw-r--r--   0 davised   (1000) davised   (1000)    14146 2022-03-23 05:43:59.000000 get_assemblies-0.8.6/README.rst
-drwxr-xr-x   0 davised   (1000) davised   (1000)        0 2022-03-23 05:55:55.520160 get_assemblies-0.8.6/get_assemblies/
--rw-r--r--   0 davised   (1000) davised   (1000)       22 2022-03-23 05:43:59.000000 get_assemblies-0.8.6/get_assemblies/__init__.py
--rwxr-xr-x   0 davised   (1000) davised   (1000)    39361 2022-03-23 05:50:58.000000 get_assemblies-0.8.6/get_assemblies/__main__.py
--rw-------   0 davised   (1000) davised   (1000)       22 2022-03-23 05:55:12.000000 get_assemblies-0.8.6/get_assemblies/__version__.py
--rw-r--r--   0 davised   (1000) davised   (1000)     1909 2022-03-23 05:43:59.000000 get_assemblies-0.8.6/get_assemblies/pbar.py
-drwxr-xr-x   0 davised   (1000) davised   (1000)        0 2022-03-23 05:55:55.523160 get_assemblies-0.8.6/get_assemblies.egg-info/
--rw-r--r--   0 davised   (1000) davised   (1000)    15049 2022-03-23 05:55:55.000000 get_assemblies-0.8.6/get_assemblies.egg-info/PKG-INFO
--rw-r--r--   0 davised   (1000) davised   (1000)      393 2022-03-23 05:55:55.000000 get_assemblies-0.8.6/get_assemblies.egg-info/SOURCES.txt
--rw-r--r--   0 davised   (1000) davised   (1000)        1 2022-03-23 05:55:55.000000 get_assemblies-0.8.6/get_assemblies.egg-info/dependency_links.txt
--rw-r--r--   0 davised   (1000) davised   (1000)       65 2022-03-23 05:55:55.000000 get_assemblies-0.8.6/get_assemblies.egg-info/entry_points.txt
--rw-r--r--   0 davised   (1000) davised   (1000)       13 2022-03-23 05:55:55.000000 get_assemblies-0.8.6/get_assemblies.egg-info/requires.txt
--rw-r--r--   0 davised   (1000) davised   (1000)       15 2022-03-23 05:55:55.000000 get_assemblies-0.8.6/get_assemblies.egg-info/top_level.txt
--rw-r--r--   0 davised   (1000) davised   (1000)       13 2022-03-23 05:43:59.000000 get_assemblies-0.8.6/requirements.txt
--rw-r--r--   0 davised   (1000) davised   (1000)       38 2022-03-23 05:55:55.524160 get_assemblies-0.8.6/setup.cfg
--rw-r--r--   0 davised   (1000) davised   (1000)     1652 2022-03-23 05:43:59.000000 get_assemblies-0.8.6/setup.py
+drwxr-xr-x   0 davised   (1000) davised   (1000)        0 2022-03-23 06:21:53.195482 get_assemblies-0.9.0/
+-rw-r--r--   0 davised   (1000) davised   (1000)     1682 2022-03-23 05:43:59.000000 get_assemblies-0.9.0/LICENSE
+-rw-r--r--   0 davised   (1000) davised   (1000)       60 2022-03-23 05:43:59.000000 get_assemblies-0.9.0/MANIFEST.in
+-rw-r--r--   0 davised   (1000) davised   (1000)    15049 2022-03-23 06:21:53.195482 get_assemblies-0.9.0/PKG-INFO
+-rw-r--r--   0 davised   (1000) davised   (1000)    14146 2022-03-23 05:43:59.000000 get_assemblies-0.9.0/README.rst
+drwxr-xr-x   0 davised   (1000) davised   (1000)        0 2022-03-23 06:21:53.192482 get_assemblies-0.9.0/get_assemblies/
+-rw-r--r--   0 davised   (1000) davised   (1000)       22 2022-03-23 05:43:59.000000 get_assemblies-0.9.0/get_assemblies/__init__.py
+-rwxr-xr-x   0 davised   (1000) davised   (1000)    39063 2022-03-23 06:19:29.000000 get_assemblies-0.9.0/get_assemblies/__main__.py
+-rw-------   0 davised   (1000) davised   (1000)       22 2022-03-23 06:20:21.000000 get_assemblies-0.9.0/get_assemblies/__version__.py
+-rw-r--r--   0 davised   (1000) davised   (1000)     1909 2022-03-23 05:43:59.000000 get_assemblies-0.9.0/get_assemblies/pbar.py
+drwxr-xr-x   0 davised   (1000) davised   (1000)        0 2022-03-23 06:21:53.195482 get_assemblies-0.9.0/get_assemblies.egg-info/
+-rw-r--r--   0 davised   (1000) davised   (1000)    15049 2022-03-23 06:21:52.000000 get_assemblies-0.9.0/get_assemblies.egg-info/PKG-INFO
+-rw-r--r--   0 davised   (1000) davised   (1000)      393 2022-03-23 06:21:52.000000 get_assemblies-0.9.0/get_assemblies.egg-info/SOURCES.txt
+-rw-r--r--   0 davised   (1000) davised   (1000)        1 2022-03-23 06:21:52.000000 get_assemblies-0.9.0/get_assemblies.egg-info/dependency_links.txt
+-rw-r--r--   0 davised   (1000) davised   (1000)       65 2022-03-23 06:21:52.000000 get_assemblies-0.9.0/get_assemblies.egg-info/entry_points.txt
+-rw-r--r--   0 davised   (1000) davised   (1000)       13 2022-03-23 06:21:52.000000 get_assemblies-0.9.0/get_assemblies.egg-info/requires.txt
+-rw-r--r--   0 davised   (1000) davised   (1000)       15 2022-03-23 06:21:52.000000 get_assemblies-0.9.0/get_assemblies.egg-info/top_level.txt
+-rw-r--r--   0 davised   (1000) davised   (1000)       13 2022-03-23 05:43:59.000000 get_assemblies-0.9.0/requirements.txt
+-rw-r--r--   0 davised   (1000) davised   (1000)       38 2022-03-23 06:21:53.196482 get_assemblies-0.9.0/setup.cfg
+-rw-r--r--   0 davised   (1000) davised   (1000)     1652 2022-03-23 05:43:59.000000 get_assemblies-0.9.0/setup.py
```

### Comparing `get_assemblies-0.8.6/LICENSE` & `get_assemblies-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `get_assemblies-0.8.6/PKG-INFO` & `get_assemblies-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get_assemblies
-Version: 0.8.6
+Version: 0.9.0
 Summary: NCBI E-utilities wrapper for assembly downloads
 Home-page: https://github.com/davised/get_assemblies
 Author: Edward Davis
 Author-email: ed@cgrb.oregonstate.edu
 Maintainer: Edward Davis
 Maintainer-email: ed@cgrb.oregonstate.edu
 License: Custom
```

### Comparing `get_assemblies-0.8.6/README.rst` & `get_assemblies-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `get_assemblies-0.8.6/get_assemblies/__main__.py` & `get_assemblies-0.9.0/get_assemblies/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 import re
 import shutil
 import gzip
 import json
 from math import ceil
 from urllib.request import urlopen
 from urllib.error import URLError
+
 # from .pbar import track_wide
 from rich.logging import RichHandler
 from rich.console import Console
 from rich.progress import (
     BarColumn,
     SpinnerColumn,
     DownloadColumn,
@@ -60,76 +61,77 @@
     track,
 )
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures import as_completed
 from functools import partial
 from signal import signal, SIGPIPE, SIGINT, SIG_DFL
 from .__version__ import __version__
+
 signal(SIGPIPE, SIG_DFL)
 signal(SIGINT, SIG_DFL)
 
-NOT_WHITESPACE = re.compile(r'[^\s]')
-OUTPUTS = ('fna', 'ffn', 'gff', 'gbk', 'faa')
+NOT_WHITESPACE = re.compile(r"[^\s]")
+OUTPUTS = ("fna", "ffn", "gff", "gbk", "faa")
 
 
 class DownloadEdirect(argparse.Action):
-    def __init__(self, nargs='?', **kw):
+    def __init__(self, nargs=0, **kw):
+        if nargs != 0:
+            raise ValueError("nargs not allowed")
         super().__init__(nargs=nargs, **kw)
 
     def __call__(self, parser, namespace, values, option_string=None):
         init_logger(True)
         logger = logging.getLogger(__name__)
-        if values:
-            prefix = values
-        else:
-            prefix = '~/edirect'
-        if '~' in prefix:
-            prefix = os.path.expanduser(prefix)
+        prefix = os.path.expanduser("~/edirect")
         prefix = os.path.abspath(prefix)
-        if os.path.basename(prefix) == 'edirect':
+        if os.path.basename(prefix) == "edirect":
             dlpath = os.path.dirname(prefix)
         else:
-            prefix = os.path.join(prefix, 'edirect')
+            prefix = os.path.join(prefix, "edirect")
             dlpath = prefix
         if not os.path.exists(dlpath):
             os.makedirs(dlpath)
         os.chdir(dlpath)
-        out_file = os.path.join(dlpath, 'edirect.tar.gz')
-        url = 'ftp://ftp.ncbi.nlm.nih.gov/entrez/entrezdirect/edirect.tar.gz'
+        out_file = os.path.join(dlpath, "install-edirect.sh")
+        url = "ftp://ftp.ncbi.nlm.nih.gov/entrez/entrezdirect/install-edirect.sh"
         dl_file(url, out_file)
-        logger.info(f'Installing edirect in {prefix}.')
-        shutil.unpack_archive(out_file, dlpath, 'gztar')
-        os.remove(out_file)
-        logger.info('Add given directory {} to [green]$PATH[/green] to '
-                    'continue.'.format(prefix), extra={'markup': True})
-        logger.info('This script will find ~/edirect by default.')
-        logger.info('Alternatively, set [green]$EDIRECT[/green] environment '
-                    'variable.', extra={'markup': True})
+        logger.info(f"Installing edirect in {prefix}. Running install-edirect.sh.")
+        subprocess.run(['sh', out_file])
+        logger.info(
+            "Add given directory {} to [green]$PATH[/green] to "
+            "continue.".format(prefix),
+            extra={"markup": True},
+        )
+        logger.info("This script will find ~/edirect by default.")
+        logger.info(
+            "Alternatively, set [green]$EDIRECT[/green] environment " "variable.",
+            extra={"markup": True},
+        )
         parser.exit()
 
 
 def dl_file(url, out_file):
     logger = logging.getLogger(__name__)
-    logger.debug('Downloading file {} to {}'.format(url, out_file))
+    logger.debug("Downloading file {} to {}".format(url, out_file))
     if not os.path.exists(out_file) or os.path.getsize(out_file) == 0:
-        with urlopen(url) as response, open(out_file, 'wb') as tarfh:
+        with urlopen(url) as response, open(out_file, "wb") as tarfh:
             shutil.copyfileobj(response, tarfh)
 
 
 def dl_gzip(pbar, task_id, uri, filename, out, acc, swap):
     try:
         copy_url(pbar, task_id, uri, filename)
     except URLError:
         pbar.reset(task_id, start=False)
-        uri = uri.replace('GCA_', 'GCF_')
-        filename = filename.replace('GCA_', 'GCF_')
+        uri = uri.replace("GCA_", "GCF_")
+        filename = filename.replace("GCA_", "GCF_")
         copy_url(uri, task_id, uri, filename)
         # swap = True
-    with gzip.open(filename, mode='rb') as gzfh,\
-            open(out, 'wb') as outfh:
+    with gzip.open(filename, mode="rb") as gzfh, open(out, "wb") as outfh:
         shutil.copyfileobj(gzfh, outfh, 65536)
     # subprocess.run(['gunzip', dl_gz])
     # dl = dl_gz.replace('.gz', '')
     # os.rename(dl, out)
     if os.path.exists(out):
         # sys.stderr.write('\n')
         os.remove(filename)
@@ -150,167 +152,200 @@
     pbar.update(task_id, visible=False)
 
 
 def extant_file(x):
     """
     'Type' for argparse - checks that file exists but does not open.
     """
-    if not os.path.exists(x) and x != '-':
+    if not os.path.exists(x) and x != "-":
         raise argparse.ArgumentTypeError("{0} does not exist".format(x))
     return x
 
 
 def edirect_dir(x):
     """
     'Type' for argparse - checks that edirect path is present.
     """
     init_logger(True)
     logger = logging.getLogger(__name__)
-    if not os.path.exists(os.path.join(x, 'edirect.pl')):
-        msg = ('Given path [bold magenta]{}[/bold magenta] does '
-               '[bold red]NOT[/bold red] appear to be a valid edirect path.')
-        logger.error(msg.format(x), extra={'markup': True})
-        msg = ('Please specify a valid edirect path with '
-               '[bold magenta]--edirect[/bold magenta] and try again.')
-        logger.error(msg, extra={'markup': True})
+    if not os.path.exists(os.path.join(x, "edirect.pl")):
+        msg = (
+            "Given path [bold magenta]{}[/bold magenta] does "
+            "[bold red]NOT[/bold red] appear to be a valid edirect path."
+        )
+        logger.error(msg.format(x), extra={"markup": True})
+        msg = (
+            "Please specify a valid edirect path with "
+            "[bold magenta]--edirect[/bold magenta] and try again."
+        )
+        logger.error(msg, extra={"markup": True})
         exit()
     return x
 
 
-def init_logger(debug, logfile=''):
+def init_logger(debug, logfile=""):
     logger = logging.getLogger()
 
     ch = RichHandler(rich_tracebacks=True)
     logger.setLevel(logging.DEBUG)
     if debug:
         ch.setLevel(logging.DEBUG)
     else:
         ch.setLevel(logging.INFO)
     logger.addHandler(ch)
 
     if logfile:
-        fh = RichHandler(console=Console(file=open(logfile, 'a')))
+        fh = RichHandler(console=Console(file=open(logfile, "a")))
         logger.addHandler(fh)
 
 
 def run_argparse():
     parser = argparse.ArgumentParser(
-        description='Downloads assemblies & annotations from NCBI.')
-    subparsers = parser.add_subparsers(
-        dest='intype', help='Choose from this list of input types.'
+        description="Downloads assemblies & annotations from NCBI."
     )
-    parser.add_argument(
-        '--debug', help='Turn on debugging messages.', action='store_true'
+    subparsers = parser.add_subparsers(
+        dest="intype", help="Choose from this list of input types."
     )
     parser.add_argument(
-        '--version', action='version', version=__version__
+        "--debug", help="Turn on debugging messages.", action="store_true"
     )
+    parser.add_argument("--version", action="version", version=__version__)
     parser.add_argument(
-        '--dledirect', help='Download edirect to given location. [~/edirect]',
-        action=DownloadEdirect, type=str, nargs='?'
+        "--dledirect", help="Download edirect to ~/edirect", action=DownloadEdirect
     )
 
     # Add input types
-    organism = subparsers.add_parser('organism',
-                                     help='Valid NCBI organism or taxids.')
-    assembly_ids = subparsers.add_parser('assembly_ids',
-                                         help='Valid NCBI assembly IDs.')
-    nuccore_ids = subparsers.add_parser('nuccore_ids',
-                                        help='Valid NCBI nucleotide '
-                                             'accessions.')
-    json_input = subparsers.add_parser('json_input',
-                                       help='Valid NCBI JSON docsums.')
+    organism = subparsers.add_parser("organism", help="Valid NCBI organism or taxids.")
+    assembly_ids = subparsers.add_parser(
+        "assembly_ids", help="Valid NCBI assembly IDs."
+    )
+    nuccore_ids = subparsers.add_parser(
+        "nuccore_ids", help="Valid NCBI nucleotide " "accessions."
+    )
+    json_input = subparsers.add_parser("json_input", help="Valid NCBI JSON docsums.")
 
     p_assemlinks = [organism, assembly_ids, nuccore_ids]
     all_p = [organism, assembly_ids, nuccore_ids, json_input]
 
+    organism.add_argument("query", help="Valid NCBI organism text term or ID", type=str)
     organism.add_argument(
-        'query', help='Valid NCBI organism text term or ID', type=str
-    )
-    organism.add_argument(
-        '--type', help='Input is text term (default) or ID', type=str,
-        choices=['text', 'ID'], default='text'
+        "--type",
+        help="Input is text term (default) or ID",
+        type=str,
+        choices=["text", "ID"],
+        default="text",
     )
 
     assembly_ids.add_argument(
-        'infile', help='Input file with NCBI assembly IDs; "-" for stdin',
-        type=extant_file
+        "infile",
+        help='Input file with NCBI assembly IDs; "-" for stdin',
+        type=extant_file,
     )
     assembly_ids.add_argument(
-        '--type', help='Input is Accession (default) or ID', type=str,
-        choices=['acc', 'uid'], default='acc'
+        "--type",
+        help="Input is Accession (default) or ID",
+        type=str,
+        choices=["acc", "uid"],
+        default="acc",
     )
 
     nuccore_ids.add_argument(
-        'infile', help='Input file with NCBI nuccore IDs; "-" for stdin',
-        type=extant_file
+        "infile",
+        help='Input file with NCBI nuccore IDs; "-" for stdin',
+        type=extant_file,
     )
 
     json_input.add_argument(
-        'jsonfile', help='Input JSON file with docsums; "-" for stdin',
-        type=extant_file, nargs='+'
+        "jsonfile",
+        help='Input JSON file with docsums; "-" for stdin',
+        type=extant_file,
+        nargs="+",
     )
     json_input.add_argument(
-        '--function', help='Download metadata and/or genomes. [metadata]',
-        type=str, default=['metadata'], choices=['metadata', 'genomes'],
-        nargs='+'
+        "--function",
+        help="Download metadata and/or genomes. [metadata]",
+        type=str,
+        default=["metadata"],
+        choices=["metadata", "genomes"],
+        nargs="+",
     )
 
     for p in p_assemlinks:
         p.add_argument(
-            '--function', help='check counts, download metadata,'
-                               ' or genomes. [check]', type=str,
-            default=['check'], choices=['check', 'metadata', 'genomes'],
-            nargs='+'
+            "--function",
+            help="check counts, download metadata," " or genomes. [check]",
+            type=str,
+            default=["check"],
+            choices=["check", "metadata", "genomes"],
+            nargs="+",
         )
 
     for p in all_p:
         p.add_argument(
-            '--annotation', help='Require annotation? False by default,'
-                                 ' True if gbk/faa/ffn requested',
-            action='store_true', default=False
-        )
-        p.add_argument(
-            '--metadata_append', help='Append to metadata, not overwrite.',
-            action='store_true', default=False
+            "--annotation",
+            help="Require annotation? False by default,"
+            " True if gbk/faa/ffn requested",
+            action="store_true",
+            default=False,
         )
         p.add_argument(
-            '--typestrain', help='Only download type strains.',
-            action='store_true', default=False
+            "--metadata_append",
+            help="Append to metadata, not overwrite.",
+            action="store_true",
+            default=False,
         )
         p.add_argument(
-            '--keepmulti', help='By default, genomes from large multi-isolate'
-            'studies are removed.', action='store_true', default=False
+            "--typestrain",
+            help="Only download type strains.",
+            action="store_true",
+            default=False,
         )
         p.add_argument(
-            '-t', '--threads', help='Number of threads to use for downloads.'
-                                    ' 4 or more is recommended [1]',
-            default=1, type=int, metavar='T'
+            "--keepmulti",
+            help="By default, genomes from large multi-isolate" "studies are removed.",
+            action="store_true",
+            default=False,
         )
         p.add_argument(
-            '--force', help='Force download attempt of low-quality genomes.',
-            action='store_true', default=False
+            "-t",
+            "--threads",
+            help="Number of threads to use for downloads."
+            " 4 or more is recommended [1]",
+            default=1,
+            type=int,
+            metavar="T",
         )
         p.add_argument(
-            '-f', '--outformat', help='Output file prefix. [full]', type=str,
-            default='full', choices=['abbr', 'full', 'strain']
+            "--force",
+            help="Force download attempt of low-quality genomes.",
+            action="store_true",
+            default=False,
         )
         p.add_argument(
-            '-o', help='Output file types.', type=str,
-            choices=['fna', 'ffn', 'gff', 'gbk', 'faa', 'all'], nargs='+'
+            "-f",
+            "--outformat",
+            help="Output file prefix. [full]",
+            type=str,
+            default="full",
+            choices=["abbr", "full", "strain"],
         )
         p.add_argument(
-            '--edirect', help='Path to edirect directory.', type=edirect_dir
+            "-o",
+            help="Output file types.",
+            type=str,
+            choices=["fna", "ffn", "gff", "gbk", "faa", "all"],
+            nargs="+",
         )
+        p.add_argument("--edirect", help="Path to edirect directory.", type=edirect_dir)
         p.add_argument(
-            '--debug', help='Turn on debugging messages.', action='store_true'
+            "--debug", help="Turn on debugging messages.", action="store_true"
         )
 
     args = parser.parse_args()
-    init_logger(args.debug, logfile='get_assemblies.log')
+    init_logger(args.debug, logfile="get_assemblies.log")
     if not args.intype:
         parser.print_help()
         exit()
     # if args.debug:
     #     pp.pprint(args)
     return args
 
@@ -328,707 +363,726 @@
             # do something sensible if there's some error
             raise
         yield obj
 
 
 def eutil_critical(name):
     logger = logging.getLogger(__name__)
-    logger.critical(
-        f'Unable to find eutil: {name}'
-    )
-    logger.critical(
-        'Use --dledirect to download the edirect files and try again.'
-    )
+    logger.critical(f"Unable to find eutil: {name}")
+    logger.critical("Use --dledirect to download the edirect files and try again.")
     exit(1)
 
 
 def validate_inputs(args):
     logger = logging.getLogger(__name__)
 
-    if 'genomes' in args.function and 'metadata' not in args.function:
-        if args.intype != 'json_file':
-            args.function.append('metadata')
-
-    if 'genomes' in args.function and not args.o:
-        logger.critical(
-            '--function genomes set, but no outputs chosen using --outputs'
-        )
-        logger.critical(
-            'Check settings (add at least one output) and try again.'
-        )
+    if "genomes" in args.function and "metadata" not in args.function:
+        if args.intype != "json_file":
+            args.function.append("metadata")
+
+    if "genomes" in args.function and not args.o:
+        logger.critical("--function genomes set, but no outputs chosen using --outputs")
+        logger.critical("Check settings (add at least one output) and try again.")
         exit(1)
     else:
         if args.o:
-            if 'all' in args.o:
+            if "all" in args.o:
                 args.o = OUTPUTS
             else:
                 args.o = set(args.o)
 
     if args.o:
         for opt in args.o:
-            if opt in ('ffn', 'gbk', 'faa'):
+            if opt in ("ffn", "gbk", "faa"):
                 args.annotation = True
                 break
 
-    user_edir = os.path.expanduser(os.path.join('~', 'edirect'))
+    user_edir = os.path.expanduser(os.path.join("~", "edirect"))
     if args.edirect:
         edirect_dir = args.edirect
-    elif 'EDIRECT' in os.environ and os.path.exists(os.environ['EDIRECT']):
-        edirect_dir = os.environ['EDIRECT']
+    elif "EDIRECT" in os.environ and os.path.exists(os.environ["EDIRECT"]):
+        edirect_dir = os.environ["EDIRECT"]
     elif os.path.exists(user_edir):
         edirect_dir = user_edir
     else:
-        logger.debug('No edirect dir found.')
-        edirect_dir = ''
+        logger.debug("No edirect dir found.")
+        edirect_dir = ""
 
-    utils = ['esearch', 'efetch', 'xtract', 'efilter', 'elink', 'epost']
+    utils = ["esearch", "efetch", "xtract", "efilter", "elink", "epost"]
     exes = {}
     for util in utils:
         if shutil.which(util):
             exes[util] = util
         elif os.path.exists(edirect_dir):
             check = os.path.join(edirect_dir, util)
             if os.path.isfile(check):
                 exes[util] = check
         else:
             eutil_critical(util)
 
     # logger.debug(pp.pformat(args))
     logger.debug(pp.pformat(args))
     logger.debug(pp.pformat(exes))
-    return(args, exes)
+    return (args, exes)
 
 
 def search_query(esearch, efilter, qtype, query, typestrain):
     logger = logging.getLogger(__name__)
     # returns list of assembly IDs
     # input is organism search or taxid
     command = []
-    if qtype == 'text':
-        query = f'{query}[ORGN]'
-    elif qtype == 'ID':
-        query = f'txid{query}[ORGN]'
+    if qtype == "text":
+        query = f"{query}[ORGN]"
+    elif qtype == "ID":
+        query = f"txid{query}[ORGN]"
 
-    query = query + ' AND latest [PROP] NOT '\
-        'partial-genome-representation [PROP]'
+    query = query + " AND latest [PROP] NOT " "partial-genome-representation [PROP]"
 
     if typestrain:
         query = query + ' AND "from type" [PROP]'
 
-    command = [esearch, '-db', 'assembly', '-query', query]
+    command = [esearch, "-db", "assembly", "-query", query]
 
     # logger.debug('Running command:\n' + ' '.join(command))
-    logger.debug('Running command:\n' + ' '.join(command))
+    logger.debug("Running command:\n" + " ".join(command))
     try:
-        search_res = subprocess.run(command, stdout=subprocess.PIPE, text=True,
-                                    check=True)
+        search_res = subprocess.run(
+            command, stdout=subprocess.PIPE, text=True, check=True
+        )
     except subprocess.CalledProcessError as e:
-        logger.critical('There was an error running esearch.')
+        logger.critical("There was an error running esearch.")
         logger.critical(f'Check the error: "{e}" and try again.')
         exit(1)
 
-    return(search_res.stdout)
+    return search_res.stdout
 
 
 def get_assem_links(epost, infile, qtype):
     # returns list of assembly IDs
     # input is list of assem ids
     logger = logging.getLogger(__name__)
     assem_ids = [x.strip() for x in fileinput.input(infile) if x]
     logger.debug(pp.pformat(assem_ids))
 
-    command = [epost,
-               '-db', 'assembly',
-               '-format', f'{qtype}']
+    command = [epost, "-db", "assembly", "-format", f"{qtype}"]
 
     # command = ' '.join(command)
     try:
-        output = subprocess.run(command, stdout=subprocess.PIPE, shell=False,
-                                text=True, input='\n'.join(assem_ids),
-                                check=True)
+        output = subprocess.run(
+            command,
+            stdout=subprocess.PIPE,
+            shell=False,
+            text=True,
+            input="\n".join(assem_ids),
+            check=True,
+        )
     except subprocess.CalledProcessError as e:
-        logger.critical('There was an error running epost.')
+        logger.critical("There was an error running epost.")
         logger.critical(f'Check the error: "{e}" and try again.')
         exit(1)
-    return(output.stdout)
+    return output.stdout
 
 
 def convert_nuc_to_assem(elink, infile):
     # returns list of assembly IDs
     # input is a list of nucleotide IDs
     logger = logging.getLogger(__name__)
     nuccore_ids = [x.strip() for x in fileinput.input(infile) if x]
     logger.debug(pp.pformat(nuccore_ids))
 
-    command = [elink,
-               '-target', 'assembly',
-               '-format', 'acc',
-               '-db', 'nuccore',
-               '-id',
-               ','.join(nuccore_ids)]
+    command = [
+        elink,
+        "-target",
+        "assembly",
+        "-format",
+        "acc",
+        "-db",
+        "nuccore",
+        "-id",
+        ",".join(nuccore_ids),
+    ]
 
     # command = ' '.join(command)
     try:
-        output = subprocess.run(command, stdout=subprocess.PIPE, shell=False,
-                                text=True, check=True)
+        output = subprocess.run(
+            command, stdout=subprocess.PIPE, shell=False, text=True, check=True
+        )
     except subprocess.CalledProcessError as e:
-        logger.critical('There was an error running elink.')
+        logger.critical("There was an error running elink.")
         logger.critical(f'Check the error: "{e}" and try again.')
         exit(1)
 
-    return(output.stdout)
+    return output.stdout
 
 
-def check_count(assem_links, query='stdin'):
+def check_count(assem_links, query="stdin"):
     logger = logging.getLogger(__name__)
     try:
         entrez_direct = ElementTree.fromstring(assem_links)
     except ElementTree.ParseError:
-        logger.critical(
-            'No output from edirect search.'
-        )
-        logger.critical(
-            'Check input(s) and try again.'
-        )
+        logger.critical("No output from edirect search.")
+        logger.critical("Check input(s) and try again.")
     try:
-        count = entrez_direct.find('Count').text
+        count = entrez_direct.find("Count").text
     except AttributeError:
-        with open('no_hits.txt', 'a') as nohitfh:
-            nohitfh.write(f'{query}\n')
-        logger.critical(
-            f'No genomes found to download with query {query}.'
-        )
-        logger.critical(
-            'Check your query/taxid and try again.'
-        )
-        logger.critical(
-            'Examine no_hits.txt for a record of genomes with no hits.'
-        )
+        with open("no_hits.txt", "a") as nohitfh:
+            nohitfh.write(f"{query}\n")
+        logger.critical(f"No genomes found to download with query {query}.")
+        logger.critical("Check your query/taxid and try again.")
+        logger.critical("Examine no_hits.txt for a record of genomes with no hits.")
         exit(1)
     else:
+        logger.info(f"Found {count} genome(s) to download.")
         logger.info(
-            f'Found {count} genome(s) to download.'
-        )
-        logger.info(
-            f'Expect {int(count)*5} MB to {int(count)*7} MB of data pending '
-            'the chosen file types for download.'
+            f"Expect {int(count)*5} MB to {int(count)*7} MB of data pending "
+            "the chosen file types for download."
         )
     # return(count)
 
 
 def chunks(uidl, n):
     """Yield successive n-sized chunks from list."""
     for i in range(0, len(uidl), n):
-        yield uidl[i:i + n]
+        yield uidl[i : i + n]
 
 
 def fetch_docsums(efetch, assem_links):
     logger = logging.getLogger(__name__)
-    command = [f'{efetch}', '-format', 'uid']
+    command = [f"{efetch}", "-format", "uid"]
     try:
-        uids = subprocess.run(' '.join(command), stdout=subprocess.PIPE,
-                              shell=True, text=True, input=assem_links,
-                              check=True)
+        uids = subprocess.run(
+            " ".join(command),
+            stdout=subprocess.PIPE,
+            shell=True,
+            text=True,
+            input=assem_links,
+            check=True,
+        )
     except subprocess.CalledProcessError as e:
-        logger.critical('There was an error running efetch.')
+        logger.critical("There was an error running efetch.")
         logger.critical(f'Check the error: "{e}" and try again.')
         exit(1)
     # logger.debug('Found these uids:\n' +
     #                   uids.stdout)
     uid_list = sorted(uids.stdout.splitlines())
 
     outputs = []
     i = 0
     nchunk = ceil(len(uid_list) / 500)
     if nchunk > 0:
-        units = 'secs'
+        units = "secs"
         length = nchunk * 10
         if length > 60:
-            units = 'mins'
+            units = "mins"
             length = length / 60
             if length > 60:
-                units = 'hours'
+                units = "hours"
                 length = length / 60
-        logger.info('With {} chunks (500 ids per), this will take around '
-                    '{} {}.'.format(nchunk, int(length), units))
-    for chunk in track(chunks(uid_list, 500), 'chunk', nchunk):
-        command = [f'{efetch}',
-                   '-format', 'docsum',
-                   '-mode', 'json',
-                   '-db', 'assembly',
-                   '-id', ','.join(chunk)]
+        logger.info(
+            "With {} chunks (500 ids per), this will take around "
+            "{} {}.".format(nchunk, int(length), units)
+        )
+    for chunk in track(chunks(uid_list, 500), "chunk", nchunk):
+        command = [
+            f"{efetch}",
+            "-format",
+            "docsum",
+            "-mode",
+            "json",
+            "-db",
+            "assembly",
+            "-id",
+            ",".join(chunk),
+        ]
         # command += ','.join(chunk)
         # logger.debug('Running this command:\n' + ' '.join(command))
-        logger.debug('Running this command: ' + ' '.join(command))
+        logger.debug("Running this command: " + " ".join(command))
         jsondata = []
 
         for j in range(5):
             try:
-                output = subprocess.run(command, stdout=subprocess.PIPE,
-                                        shell=False, text=True, check=True,
-                                        stderr=subprocess.DEVNULL)
+                output = subprocess.run(
+                    command,
+                    stdout=subprocess.PIPE,
+                    shell=False,
+                    text=True,
+                    check=True,
+                    stderr=subprocess.DEVNULL,
+                )
             except subprocess.CalledProcessError as e:
-                logger.critical('There was an error running efetch.')
+                logger.critical("There was an error running efetch.")
                 logger.critical(f'Check the error: "{e}" and try again.')
                 exit(1)
 
             try:
                 jsondata = json.loads(output.stdout)
             except json.JSONDecodeError:
-                msg = 'No JSON output detected. Retrying. ({})'
+                msg = "No JSON output detected. Retrying. ({})"
                 logger.warning(msg.format(j + 1))
             else:
                 break
         if not jsondata:
-            msg = 'Unable to download chunk from NCBI.'
+            msg = "Unable to download chunk from NCBI."
             logger.critical(msg)
-            msg = 'Check settings and try again later.'
+            msg = "Check settings and try again later."
             logger.critical(msg)
             exit(-1)
-        with open(f'docsums{i}.json', 'w') as docsumfh:
+        with open(f"docsums{i}.json", "w") as docsumfh:
             json.dump(jsondata, docsumfh, indent=4)
-            docsumfh.write('\n')
+            docsumfh.write("\n")
         outputs.append(jsondata)
         i += 1
 
     # with open('docsums.json', 'w') as fh:
     #     fh.write(outputs)
     #     fh.write('\n')
 
-    return(outputs)
+    return outputs
 
 
 def get_json_from_file(jsonfiles):
     # returns list of assembly IDs
     # input is list of assem ids
     docsums = []
     for jsonfile in jsonfiles:
-        with open(jsonfile, 'r') as fh:
+        with open(jsonfile, "r") as fh:
             docsum = json.load(fh)
         docsums.append(docsum)
-    return(docsums)
+    return docsums
 
 
 def json_error(datatype, infotype, argument):
     # Print can't find datatype in argument
     logger = logging.getLogger(__name__)
-    logger.critical(f'I cannot find the {datatype} from this {infotype}.')
-    logger.critical(f'{infotype} -- {argument}')
-    logger.critical(
-        f'Check that there are {datatype}s returned and try again')
+    logger.critical(f"I cannot find the {datatype} from this {infotype}.")
+    logger.critical(f"{infotype} -- {argument}")
+    logger.critical(f"Check that there are {datatype}s returned and try again")
     exit(-1)
 
 
 def debugging(datatype, infotype, argument):
     # Print can't find datatype in argument
     logger = logging.getLogger(__name__)
-    logger.debug(f'I cannot find the {datatype} from this {infotype}.')
-    logger.debug(f'{infotype} -- {argument}')
+    logger.debug(f"I cannot find the {datatype} from this {infotype}.")
+    logger.debug(f"{infotype} -- {argument}")
 
 
 def remove_invalid_characters(string):
-    string = string.replace('[', '')
-    string = string.replace(']', '')
-    string = string.replace('/', '_')
-    string = string.replace('(', '')
-    string = string.replace(')', '')
-    string = string.replace(':', '_')
-    string = string.replace(';', '')
-    string = string.replace('%', '')
-    string = string.replace('#', '_')
+    string = string.replace("[", "")
+    string = string.replace("]", "")
+    string = string.replace("/", "_")
+    string = string.replace("(", "")
+    string = string.replace(")", "")
+    string = string.replace(":", "_")
+    string = string.replace(";", "")
+    string = string.replace("%", "")
+    string = string.replace("#", "_")
     return string
 
 
 def replace_spaces(string):
-    string = string.replace(' ', '_')
+    string = string.replace(" ", "_")
     return string
 
 
 def get_prefix(outformat, name, strain, assem_name):
     # Get valid genus and species
     # Omit Candidatus, if present
     logger = logging.getLogger(__name__)
     name = remove_invalid_characters(name)
     strain = remove_invalid_characters(strain)
 
-    name_list = name.split(' ')
-    if name_list[0] == 'Candidatus' or name_list[0] == 'uncultured':
+    name_list = name.split(" ")
+    if name_list[0] == "Candidatus" or name_list[0] == "uncultured":
         if len(name_list) > 2:
             genus = name_list[1]
             species = name_list[2]
             strain_idx = 3
         else:
             genus = name_list[1]
-            species = 'sp'
+            species = "sp"
             strain_idx = 2
     else:
         try:
             genus = name_list[0]
         except IndexError:
-            genus = ''
-            logger.error(f'Unable to find genus for {name}')
+            genus = ""
+            logger.error(f"Unable to find genus for {name}")
         try:
             species = name_list[1]
         except IndexError:
-            species = ''
-            logger.error(f'Unable to find species for {name} {strain}')
+            species = ""
+            logger.error(f"Unable to find species for {name} {strain}")
         strain_idx = 2
 
-    if genus in strain and 'sp.' not in name:
+    if genus in strain and "sp." not in name:
         warn = True
-        logger.debug(f'Seemingly malformed organism name {name} {strain}')
-        logger.debug(f'Strain before {strain}')
+        logger.debug(f"Seemingly malformed organism name {name} {strain}")
+        logger.debug(f"Strain before {strain}")
         try:
-            strain = strain.split(' ', 2)[2]
+            strain = strain.split(" ", 2)[2]
         except IndexError:
-            strain = '-'
-        logger.debug(f'Strain after {strain}')
+            strain = "-"
+        logger.debug(f"Strain after {strain}")
     else:
         warn = False
 
-    if strain == '-':
+    if strain == "-":
         if len(name_list) == strain_idx + 1:
             strain = name_list[strain_idx]
         else:
-            strain = ' '.join(name_list[strain_idx:])
+            strain = " ".join(name_list[strain_idx:])
 
     # Remove spaces
     genus = replace_spaces(genus)
     species = replace_spaces(species)
     strain = replace_spaces(strain)
 
     if not strain:
         strain = assem_name
 
-    if 'substr.' in strain:
-        strain = strain.replace('substr.', 'substr')
+    if "substr." in strain:
+        strain = strain.replace("substr.", "substr")
 
-    if outformat == 'strain' or not species:
+    if outformat == "strain" or not species:
         prefix = strain
-    elif outformat == 'full' or 'sp.' in species:
-        species = species.replace('sp.', 'sp')
-        prefix = '_'.join([genus, species, strain])
-    elif outformat == 'abbr':
-        prefix = '_'.join([genus[0], species, strain])
+    elif outformat == "full" or "sp." in species:
+        species = species.replace("sp.", "sp")
+        prefix = "_".join([genus, species, strain])
+    elif outformat == "abbr":
+        prefix = "_".join([genus[0], species, strain])
 
     if warn:
-        logger.warning(f'Check out this prefix for accuracy: {prefix}')
+        logger.warning(f"Check out this prefix for accuracy: {prefix}")
 
     return prefix
 
 
-def extract_metadata(force, metadata_append, outformat, typestrain, annotation,
-                     docsums, keepmulti):
+def extract_metadata(
+    force, metadata_append, outformat, typestrain, annotation, docsums, keepmulti
+):
     # Return dl_mapping dict at the end
     logger = logging.getLogger(__name__)
     dl_mapping = {}
     # d = json.loads(docsums)
 
-    json_keys = ['uid', 'assemblyname', 'speciesname', 'wgs',
-                 'submitterorganization', 'assemblystatus',
-                 'fromtype', 'lastupdatedate', 'coverage', 'contign50']
-    special_keys = ['isolate/strain', 'sequence_type',
-                    'accession_type', 'accession']
+    json_keys = [
+        "uid",
+        "assemblyname",
+        "speciesname",
+        "wgs",
+        "submitterorganization",
+        "assemblystatus",
+        "fromtype",
+        "lastupdatedate",
+        "coverage",
+        "contign50",
+    ]
+    special_keys = ["isolate/strain", "sequence_type", "accession_type", "accession"]
     prefixes = {}
     metadata = []
-    metadata_file = 'metadata.tab'
+    metadata_file = "metadata.tab"
     if metadata_append:
-        open_mode = 'a'
+        open_mode = "a"
         if not os.path.exists(metadata_file):
-            metadata.append(json_keys + special_keys + ['prefix'])
+            metadata.append(json_keys + special_keys + ["prefix"])
     else:
-        open_mode = 'w'
-        metadata.append(json_keys + special_keys + ['prefix'])
+        open_mode = "w"
+        metadata.append(json_keys + special_keys + ["prefix"])
 
     # for d in decode_stacked_json(docsums):
-    for d in track(docsums, 'docsums', len(docsums)):
+    for d in track(docsums, "docsums", len(docsums)):
         try:
-            json_data = d['result']
+            json_data = d["result"]
         except KeyError:
-            json_error('result', 'json_docsums', docsums)
+            json_error("result", "json_docsums", docsums)
 
         try:
-            uids = json_data['uids']
+            uids = json_data["uids"]
         except KeyError:
-            json_error('uid', 'json_docsums', docsums)
+            json_error("uid", "json_docsums", docsums)
 
         # Keep track of strain names so we don't have dups
 
         for uid in uids:
             # annotation_type = 'genbank'
-            annotation_type = 'refseq'
+            annotation_type = "refseq"
             line = []
             skip = False
             # Standard keys; only str/int return
             for json_key in json_keys:
                 try:
                     item = json_data[uid][json_key]
                 except KeyError:
-                    debugging(json_key, 'uid', uid)
-                    line.append('-')
+                    debugging(json_key, "uid", uid)
+                    line.append("-")
                 else:
                     if item:
                         line.append(str(item))
                     else:
-                        line.append('-')
-                    if json_key == 'fromtype':
+                        line.append("-")
+                    if json_key == "fromtype":
                         if not item and typestrain:
                             skip = True
-                    if json_key == 'speciesname':
+                    if json_key == "speciesname":
                         name = item
-                    elif json_key == 'assemblyname':
-                        assem_name = item.replace(' ', '_')
-                        assem_name = assem_name.replace('#', '_')
-                    elif json_key == 'assemblystatus':
-                        if item == 'Complete Genome':
-                            annotation_type = 'genbank'
+                    elif json_key == "assemblyname":
+                        assem_name = item.replace(" ", "_")
+                        assem_name = assem_name.replace("#", "_")
+                    elif json_key == "assemblystatus":
+                        if item == "Complete Genome":
+                            annotation_type = "genbank"
             if skip:
                 logger.debug(
-                    f'{uid} - {name} {assem_name} not from type and '
-                    '--typestrain set. Skipping...'
+                    f"{uid} - {name} {assem_name} not from type and "
+                    "--typestrain set. Skipping..."
                 )
                 continue
 
             # Special values; need more digging through list/dict
             # sequence_type
-            sequence_type = ''
+            sequence_type = ""
             try:
-                exclfromrefseq = json_data[uid]['exclfromrefseq']
+                exclfromrefseq = json_data[uid]["exclfromrefseq"]
             except KeyError:
-                debugging('exclfromrefseq', 'uid', uid)
+                debugging("exclfromrefseq", "uid", uid)
                 exclfromrefseq = []
             skip = False
-            reason = ''
+            reason = ""
             # https://www.ncbi.nlm.nih.gov/assembly/help/anomnotrefseq/
             for item in exclfromrefseq:
-                annotation_type = 'genbank'
-                if item == 'derived from single cell':
-                    sequence_type = 'SAG'
-                if item == 'derived from metagenome':
-                    sequence_type = 'metagenome'
-                if item == 'derived from environmental source':
-                    sequence_type = 'environmental'
-                if item == 'from large multi-isolate project':
-                    sequence_type = 'multi-isolate'
+                annotation_type = "genbank"
+                if item == "derived from single cell":
+                    sequence_type = "SAG"
+                if item == "derived from metagenome":
+                    sequence_type = "metagenome"
+                if item == "derived from environmental source":
+                    sequence_type = "environmental"
+                if item == "from large multi-isolate project":
+                    sequence_type = "multi-isolate"
                     if not keepmulti:
                         skip = True
                         reason = item
-                if item in ('low contig N50', 'many frameshifted proteins',
-                            'low quality sequence', 'genome length too large',
-                            'contaminated', 'abnormal gene to sequence ratio',
-                            'fragmented assembly', 'genome length too small',
-                            'low gene count', 'missing ribosomal protein '
-                            'genes', 'missing rRNA genes', 'missing tRNA '
-                            'genes', 'partial', 'untrustworthy as type',
-                            'chimeric', 'hybrid', 'misassembled', 'sequence '
-                            'duplications', 'unverified source organism'):
+                if item in (
+                    "low contig N50",
+                    "many frameshifted proteins",
+                    "low quality sequence",
+                    "genome length too large",
+                    "contaminated",
+                    "abnormal gene to sequence ratio",
+                    "fragmented assembly",
+                    "genome length too small",
+                    "low gene count",
+                    "missing ribosomal protein " "genes",
+                    "missing rRNA genes",
+                    "missing tRNA " "genes",
+                    "partial",
+                    "untrustworthy as type",
+                    "chimeric",
+                    "hybrid",
+                    "misassembled",
+                    "sequence " "duplications",
+                    "unverified source organism",
+                ):
                     skip = True
                     reason = item
 
             # Strain
-            strain = ''
-            isolate = ''
-            sub_value = ''
+            strain = ""
+            isolate = ""
+            sub_value = ""
             try:
-                biosource = json_data[uid]['biosource']
+                biosource = json_data[uid]["biosource"]
             except KeyError:
-                strain = '-'
-                debugging('biosource', 'uid', uid)
+                strain = "-"
+                debugging("biosource", "uid", uid)
             else:
                 try:
-                    isolate = biosource['isolate']
+                    isolate = biosource["isolate"]
                 except KeyError:
-                    isolate = ''
-                    debugging('isolate', 'biosource', uid)
-                for item in biosource['infraspecieslist']:
+                    isolate = ""
+                    debugging("isolate", "biosource", uid)
+                for item in biosource["infraspecieslist"]:
                     try:
-                        sub_type = item['sub_type']
+                        sub_type = item["sub_type"]
                     except KeyError:
                         continue
                     else:
-                        if sub_type == 'strain':
+                        if sub_type == "strain":
                             try:
-                                sub_value = item['sub_value']
+                                sub_value = item["sub_value"]
                             except KeyError:
-                                debugging('strain', 'biosource', uid)
-                                sub_value = ''
+                                debugging("strain", "biosource", uid)
+                                sub_value = ""
                 if sub_value:
                     strain = sub_value
                 elif isolate:
-                    logger.debug(
-                        f'Using isolate from {uid} instead of strain.')
+                    logger.debug(f"Using isolate from {uid} instead of strain.")
                     strain = isolate
                 else:
-                    debugging('strain_name', 'biosource', uid)
-                    strain = '-'
+                    debugging("strain_name", "biosource", uid)
+                    strain = "-"
             # try:
             #     seen[strain] += 1
             # except KeyError:
             #     seen[strain] = 0
             # else:
             #     strain = f'{strain}_{seen[strain]}'
             #     logger.debug(f'Adding number to strain {strain}.')
             line.append(strain)
 
             # sequence_type continued
             if skip:
                 if force:
                     logger.warning(
-                        f'Assembly {uid} - {strain} is being skipped due '
+                        f"Assembly {uid} - {strain} is being skipped due "
                         f'to "{reason}". --force enabled; attempting download.'
                     )
                 else:
                     logger.warning(
-                        f'Assembly {uid} - {strain} is being skipped due '
+                        f"Assembly {uid} - {strain} is being skipped due "
                         f'to "{reason}".'
                     )
                     continue
 
             try:
-                propertylist = json_data[uid]['propertylist']
+                propertylist = json_data[uid]["propertylist"]
             except KeyError:
                 annotation_type = False
-                debugging('propertylist', 'uid', uid)
+                debugging("propertylist", "uid", uid)
             else:
-                if 'latest' not in propertylist:
+                if "latest" not in propertylist:
                     if not force:
-                        logger.debug(
-                            f'{strain} -- {uid} not latest. Skipping.'
-                        )
+                        logger.debug(f"{strain} -- {uid} not latest. Skipping.")
                         continue
-                if 'partial-genome-representation' in propertylist:
+                if "partial-genome-representation" in propertylist:
                     if not force:
-                        logger.debug(
-                            f'{strain} -- {uid} is partial genome. Skipping.'
-                        )
+                        logger.debug(f"{strain} -- {uid} is partial genome. Skipping.")
                         continue
 
             if annotation:
-                logger.debug(
-                    f'{strain} -- annotation type: {annotation_type}'
-                )
-                if annotation_type == 'genbank':
-                    if 'genbank_has_annotation' in propertylist:
+                logger.debug(f"{strain} -- annotation type: {annotation_type}")
+                if annotation_type == "genbank":
+                    if "genbank_has_annotation" in propertylist:
                         pass
-                    elif 'refseq_has_annotation' in propertylist:
-                        logger.debug(
-                            f'Switching to refseq annotation for {strain}'
-                        )
-                        annotation_type = 'refseq'
+                    elif "refseq_has_annotation" in propertylist:
+                        logger.debug(f"Switching to refseq annotation for {strain}")
+                        annotation_type = "refseq"
                     else:
                         logger.critical(
-                            f'Unable to find annotation for {strain}.'
-                            ' Skipping...'
+                            f"Unable to find annotation for {strain}." " Skipping..."
                         )
                         continue
-                elif annotation_type == 'refseq':
-                    if 'refseq_has_annotation' in propertylist:
+                elif annotation_type == "refseq":
+                    if "refseq_has_annotation" in propertylist:
                         pass
-                    elif 'genbank_has_annotation' in propertylist:
-                        logger.debug(
-                            f'Switching to genbank annotation for {strain}'
-                        )
-                        annotation_type = 'genbank'
+                    elif "genbank_has_annotation" in propertylist:
+                        logger.debug(f"Switching to genbank annotation for {strain}")
+                        annotation_type = "genbank"
                     else:
                         logger.critical(
-                            f'Unable to find annotation for {strain}.'
-                            ' Skipping...'
+                            f"Unable to find annotation for {strain}." " Skipping..."
                         )
                         continue
 
             if not sequence_type:
-                sequence_type = 'cell culture'
+                sequence_type = "cell culture"
             line.append(sequence_type)
 
             # Accession
-            accession = ''
-            acc_type = 'ftppath_'
+            accession = ""
+            acc_type = "ftppath_"
             try:
-                synonym = json_data[uid]['synonym']
+                synonym = json_data[uid]["synonym"]
             except KeyError:
-                logger.warning(f'Unable to find accession for {uid}.')
-                logger.warning(f'{uid} will be skipped.')
+                logger.warning(f"Unable to find accession for {uid}.")
+                logger.warning(f"{uid} will be skipped.")
                 continue
             try:
                 accession = synonym[annotation_type]
             except KeyError:
-                accession = ''
+                accession = ""
             else:
                 acc_type += annotation_type
             if not accession:
-                logger.warning(f'Unable to find accession for {uid}. '
-                               'Skipping...')
+                logger.warning(f"Unable to find accession for {uid}. " "Skipping...")
                 continue
             else:
                 line.append(annotation_type)
                 line.append(accession)
 
             # Get file prefix
             prefix = get_prefix(outformat, name, strain, assem_name)
             if prefix in prefixes:
-                logger.warning(f'Prefix "{prefix}" has already been seen, '
-                               f'adding assembly name "{assem_name}" to end.')
-                logger.debug('Already seen assembly ID: "{}", new ID "{}"'
-                             .format(prefixes[prefix], accession))
-                prefix = '_'.join([prefix, assem_name])
+                logger.warning(
+                    f'Prefix "{prefix}" has already been seen, '
+                    f'adding assembly name "{assem_name}" to end.'
+                )
+                logger.debug(
+                    'Already seen assembly ID: "{}", new ID "{}"'.format(
+                        prefixes[prefix], accession
+                    )
+                )
+                prefix = "_".join([prefix, assem_name])
             else:
                 prefixes[prefix] = accession
             line.append(prefix)
 
             # Get FTP path
-            ftp_path = ''
+            ftp_path = ""
             try:
                 ftp_path = json_data[uid][acc_type]
             except KeyError:
-                logger.warning(f'Unable to find ftppath for {accession}.')
-                logger.warning(f'{accession} will be skipped.')
+                logger.warning(f"Unable to find ftppath for {accession}.")
+                logger.warning(f"{accession} will be skipped.")
                 continue
 
-            dl_mapping[accession] = {'ftp_path': ftp_path,
-                                     'prefix': prefix,
-                                     'assem_name': assem_name,
-                                     'swap': False}
+            dl_mapping[accession] = {
+                "ftp_path": ftp_path,
+                "prefix": prefix,
+                "assem_name": assem_name,
+                "swap": False,
+            }
             metadata.append(line)
     with open(metadata_file, open_mode) as metadatafh:
         for line in metadata:
-            metadatafh.write('\t'.join(line) + '\n')
+            metadatafh.write("\t".join(line) + "\n")
 
     return dl_mapping
 
 
 def download_genomes(o, dl_mapping, threads):
     logger = logging.getLogger(__name__)
-    filemap = {'faa': 'protein.faa.gz',
-               'fna': 'genomic.fna.gz',
-               'gbk': 'genomic.gbff.gz',
-               'gff': 'genomic.gff.gz',
-               'ffn': 'cds_from_genomic.fna.gz'}
+    filemap = {
+        "faa": "protein.faa.gz",
+        "fna": "genomic.fna.gz",
+        "gbk": "genomic.gbff.gz",
+        "gff": "genomic.gff.gz",
+        "ffn": "cds_from_genomic.fna.gz",
+    }
 
     nacc = len(dl_mapping)
-    logger.info('Downloading {} file(s).'.format(nacc * len(o)))
+    logger.info("Downloading {} file(s).".format(nacc * len(o)))
 
     # Generate urls to download
     urls = []
     for acc in dl_mapping:
-        dl_base = '_'.join([acc, dl_mapping[acc]['assem_name']])
-        dl_base = dl_base.replace(',', '')
+        dl_base = "_".join([acc, dl_mapping[acc]["assem_name"]])
+        dl_base = dl_base.replace(",", "")
         for ft in o:
             # Get output filename
-            out = dl_mapping[acc]['prefix'] + '.' + ft
+            out = dl_mapping[acc]["prefix"] + "." + ft
             if not os.path.exists(out):
-                uri = dl_mapping[acc]['ftp_path'] + \
-                    '/' + dl_base + '_' + filemap[ft]
-                if dl_mapping[acc]['swap']:
-                    uri = uri.replace('GCA_', 'GCF_')
-                logger.debug(f'URL {uri} for {acc} generated.')
-                urls.append((uri, out, acc, dl_mapping[acc]['swap']))
+                uri = dl_mapping[acc]["ftp_path"] + "/" + dl_base + "_" + filemap[ft]
+                if dl_mapping[acc]["swap"]:
+                    uri = uri.replace("GCA_", "GCF_")
+                logger.debug(f"URL {uri} for {acc} generated.")
+                urls.append((uri, out, acc, dl_mapping[acc]["swap"]))
             else:
-                logger.info(
-                    f'{out} already found. Skipping.'
-                )
+                logger.info(f"{out} already found. Skipping.")
 
     progress = Progress(
         SpinnerColumn(),
         TextColumn("[bold blue]{task.fields[filename]}", justify="right"),
         BarColumn(bar_width=None),
         "[progress.percentage]{task.percentage:>3.1f}%",
         "•",
@@ -1039,68 +1093,73 @@
         TimeRemainingColumn(),
     )
 
     results = []
     with progress as pbar:
         with ThreadPoolExecutor(max_workers=threads) as pool:
             for uri, out, acc, swap in urls:
-                logger.debug(
-                    f'Downloading {acc} to {out}.'
-                )
+                logger.debug(f"Downloading {acc} to {out}.")
                 filename = uri.split("/")[-1]
-                task_id = pbar.add_task('download', filename=out, start=False,
-                                        visible=False)
+                task_id = pbar.add_task(
+                    "download", filename=out, start=False, visible=False
+                )
                 future = pool.submit(
-                    dl_gzip, progress, task_id, uri, filename, out, acc, swap)
+                    dl_gzip, progress, task_id, uri, filename, out, acc, swap
+                )
                 results.append(future)
                 # dl_mapping[acc]['swap'] = dl_gzip(
                 #     pbar, task_id, uri, filename, out, acc, swap)
 
     for future in as_completed(results):
         output = future.result()
         if os.path.exists(output):
-            logger.info(f'{output} successfully downloaded.')
+            logger.info(f"{output} successfully downloaded.")
         else:
-            logger.error(f'{output} was unable to be downloaded.')
+            logger.error(f"{output} was unable to be downloaded.")
 
 
 def main():
     args = run_argparse()
     args, exes = validate_inputs(args)
 
     # assem_ids is a list of NCBI assembly IDs
-    if args.intype == 'organism':
-        assem_links = search_query(exes['esearch'], exes['efilter'],
-                                   args.type, args.query, args.typestrain)
-    elif args.intype == 'assembly_ids':
-        assem_links = get_assem_links(exes['epost'], args.infile, args.type)
-    elif args.intype == 'nuccore_ids':
-        assem_links = convert_nuc_to_assem(exes['elink'], args.infile)
+    if args.intype == "organism":
+        assem_links = search_query(
+            exes["esearch"], exes["efilter"], args.type, args.query, args.typestrain
+        )
+    elif args.intype == "assembly_ids":
+        assem_links = get_assem_links(exes["epost"], args.infile, args.type)
+    elif args.intype == "nuccore_ids":
+        assem_links = convert_nuc_to_assem(exes["elink"], args.infile)
     try:
-        with open('.assemlinks', 'wt') as afh:
+        with open(".assemlinks", "wt") as afh:
             afh.write(assem_links)
     except UnboundLocalError:
         pass
 
-    if args.intype in ['organism',
-                       'assembly_ids',
-                       'nuccore_ids']:
+    if args.intype in ["organism", "assembly_ids", "nuccore_ids"]:
         try:
             check_count(assem_links, args.query)
         except AttributeError:
             check_count(assem_links)
 
-    if 'metadata' in args.function:
-        if args.intype == 'json_input':
+    if "metadata" in args.function:
+        if args.intype == "json_input":
             docsums = get_json_from_file(args.jsonfile)
         else:
-            docsums = fetch_docsums(exes['efetch'], assem_links)
-        dl_mapping = extract_metadata(args.force, args.metadata_append,
-                                      args.outformat, args.typestrain,
-                                      args.annotation, docsums, args.keepmulti)
+            docsums = fetch_docsums(exes["efetch"], assem_links)
+        dl_mapping = extract_metadata(
+            args.force,
+            args.metadata_append,
+            args.outformat,
+            args.typestrain,
+            args.annotation,
+            docsums,
+            args.keepmulti,
+        )
 
-    if 'genomes' in args.function:
+    if "genomes" in args.function:
         download_genomes(args.o, dl_mapping, args.threads)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `get_assemblies-0.8.6/get_assemblies/pbar.py` & `get_assemblies-0.9.0/get_assemblies/pbar.py`

 * *Files identical despite different names*

### Comparing `get_assemblies-0.8.6/get_assemblies.egg-info/PKG-INFO` & `get_assemblies-0.9.0/get_assemblies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-assemblies
-Version: 0.8.6
+Version: 0.9.0
 Summary: NCBI E-utilities wrapper for assembly downloads
 Home-page: https://github.com/davised/get_assemblies
 Author: Edward Davis
 Author-email: ed@cgrb.oregonstate.edu
 Maintainer: Edward Davis
 Maintainer-email: ed@cgrb.oregonstate.edu
 License: Custom
```

### Comparing `get_assemblies-0.8.6/setup.py` & `get_assemblies-0.9.0/setup.py`

 * *Files identical despite different names*

