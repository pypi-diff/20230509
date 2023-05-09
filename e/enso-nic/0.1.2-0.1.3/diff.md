# Comparing `tmp/enso-nic-0.1.2.tar.gz` & `tmp/enso-nic-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enso-nic-0.1.2.tar", last modified: Thu Mar  9 00:05:45 2023, max compression
+gzip compressed data, was "enso-nic-0.1.3.tar", last modified: Tue May  9 14:38:33 2023, max compression
```

## Comparing `enso-nic-0.1.2.tar` & `enso-nic-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2023-03-09 00:05:45.579669 enso-nic-0.1.2/
--rw-r--r--   0 hfreitas (20477) users      (100)     1518 2022-03-10 18:05:05.000000 enso-nic-0.1.2/LICENSE
--rw-r--r--   0 hfreitas (20477) users      (100)     2135 2023-03-09 00:05:45.579669 enso-nic-0.1.2/PKG-INFO
--rw-r--r--   0 hfreitas (20477) users      (100)     1140 2023-03-08 22:48:46.000000 enso-nic-0.1.2/README.md
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2023-03-09 00:05:45.575669 enso-nic-0.1.2/enso/
--rw-r--r--   0 hfreitas (20477) users      (100)      118 2023-03-08 22:41:38.000000 enso-nic-0.1.2/enso/__init__.py
--rw-r--r--   0 hfreitas (20477) users      (100)     3110 2023-03-08 22:45:34.000000 enso-nic-0.1.2/enso/__main__.py
--rw-r--r--   0 hfreitas (20477) users      (100)      463 2023-03-08 22:49:07.000000 enso-nic-0.1.2/enso/consts.py
--rw-r--r--   0 hfreitas (20477) users      (100)     6358 2023-03-08 22:45:37.000000 enso-nic-0.1.2/enso/enso_dataplane.py
--rw-r--r--   0 hfreitas (20477) users      (100)    11601 2023-03-08 22:49:10.000000 enso-nic-0.1.2/enso/enso_pktgen.py
-drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2023-03-09 00:05:45.579669 enso-nic-0.1.2/enso_nic.egg-info/
--rw-r--r--   0 hfreitas (20477) users      (100)     2135 2023-03-09 00:05:45.000000 enso-nic-0.1.2/enso_nic.egg-info/PKG-INFO
--rw-r--r--   0 hfreitas (20477) users      (100)      322 2023-03-09 00:05:45.000000 enso-nic-0.1.2/enso_nic.egg-info/SOURCES.txt
--rw-r--r--   0 hfreitas (20477) users      (100)        1 2023-03-09 00:05:45.000000 enso-nic-0.1.2/enso_nic.egg-info/dependency_links.txt
--rw-r--r--   0 hfreitas (20477) users      (100)       44 2023-03-09 00:05:45.000000 enso-nic-0.1.2/enso_nic.egg-info/entry_points.txt
--rw-r--r--   0 hfreitas (20477) users      (100)       31 2023-03-09 00:05:45.000000 enso-nic-0.1.2/enso_nic.egg-info/requires.txt
--rw-r--r--   0 hfreitas (20477) users      (100)        5 2023-03-09 00:05:45.000000 enso-nic-0.1.2/enso_nic.egg-info/top_level.txt
--rw-r--r--   0 hfreitas (20477) users      (100)      104 2023-03-09 00:05:45.579669 enso-nic-0.1.2/setup.cfg
--rw-r--r--   0 hfreitas (20477) users      (100)     1996 2023-03-09 00:04:38.000000 enso-nic-0.1.2/setup.py
+drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2023-05-09 14:38:33.792859 enso-nic-0.1.3/
+-rw-r--r--   0 hfreitas (20477) users      (100)     1518 2023-04-25 03:44:53.000000 enso-nic-0.1.3/LICENSE
+-rw-r--r--   0 hfreitas (20477) users      (100)     2045 2023-05-09 14:38:33.792859 enso-nic-0.1.3/PKG-INFO
+-rw-r--r--   0 hfreitas (20477) users      (100)     1150 2023-04-25 03:44:53.000000 enso-nic-0.1.3/README.md
+drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2023-05-09 14:38:33.792859 enso-nic-0.1.3/enso/
+-rw-r--r--   0 hfreitas (20477) users      (100)      118 2023-04-25 03:44:53.000000 enso-nic-0.1.3/enso/__init__.py
+-rw-r--r--   0 hfreitas (20477) users      (100)     2961 2023-04-25 03:44:53.000000 enso-nic-0.1.3/enso/__main__.py
+-rw-r--r--   0 hfreitas (20477) users      (100)      450 2023-04-25 03:44:53.000000 enso-nic-0.1.3/enso/consts.py
+-rw-r--r--   0 hfreitas (20477) users      (100)     6142 2023-04-25 03:44:53.000000 enso-nic-0.1.3/enso/enso_nic.py
+-rw-r--r--   0 hfreitas (20477) users      (100)    11442 2023-04-25 03:44:53.000000 enso-nic-0.1.3/enso/ensogen.py
+drwxr-xr-x   0 hfreitas (20477) users      (100)        0 2023-05-09 14:38:33.792859 enso-nic-0.1.3/enso_nic.egg-info/
+-rw-r--r--   0 hfreitas (20477) users      (100)     2045 2023-05-09 14:38:33.000000 enso-nic-0.1.3/enso_nic.egg-info/PKG-INFO
+-rw-r--r--   0 hfreitas (20477) users      (100)      312 2023-05-09 14:38:33.000000 enso-nic-0.1.3/enso_nic.egg-info/SOURCES.txt
+-rw-r--r--   0 hfreitas (20477) users      (100)        1 2023-05-09 14:38:33.000000 enso-nic-0.1.3/enso_nic.egg-info/dependency_links.txt
+-rw-r--r--   0 hfreitas (20477) users      (100)       44 2023-05-09 14:38:33.000000 enso-nic-0.1.3/enso_nic.egg-info/entry_points.txt
+-rw-r--r--   0 hfreitas (20477) users      (100)       32 2023-05-09 14:38:33.000000 enso-nic-0.1.3/enso_nic.egg-info/requires.txt
+-rw-r--r--   0 hfreitas (20477) users      (100)        5 2023-05-09 14:38:33.000000 enso-nic-0.1.3/enso_nic.egg-info/top_level.txt
+-rw-r--r--   0 hfreitas (20477) users      (100)      104 2023-05-09 14:38:33.792859 enso-nic-0.1.3/setup.cfg
+-rw-r--r--   0 hfreitas (20477) users      (100)     1900 2023-04-25 03:44:53.000000 enso-nic-0.1.3/setup.py
```

### Comparing `enso-nic-0.1.2/LICENSE` & `enso-nic-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `enso-nic-0.1.2/PKG-INFO` & `enso-nic-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: enso-nic
-Version: 0.1.2
-Summary: Python frontend for the Ensō dataplane.
-Home-page: https://github.com/hsadok/enso
-Download-URL: https://github.com/hsadok/enso
+Version: 0.1.3
+Summary: Python frontend for the Ensō NIC.
+Home-page: https://github.com/crossroadsfpga/enso
+Download-URL: https://github.com/crossroadsfpga/enso
 Author: Hugo Sadok
 Author-email: sadok@cmu.edu
 License: BSD
-Keywords: network,enso,dataplane,nic
+Keywords: network,enso,nic
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ensō Python Frontend
 
 ## Install
 
 To install the frontend run in the current directory (`frontend`):
 ```bash
-pip3 install -e .
+python3 -m pip install -e .
 ```
 To run the EnsōGen packet generator you also need to have the `capinfos` command installed in the machine you want to use to generate packets.
 
 On Ubuntu (or other Debian-based system) run:
 ```bash
 sudo apt install tshark
 ```
```

### Comparing `enso-nic-0.1.2/README.md` & `enso-nic-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Ensō Python Frontend
 
 ## Install
 
 To install the frontend run in the current directory (`frontend`):
 ```bash
-pip3 install -e .
+python3 -m pip install -e .
 ```
 To run the EnsōGen packet generator you also need to have the `capinfos` command installed in the machine you want to use to generate packets.
 
 On Ubuntu (or other Debian-based system) run:
 ```bash
 sudo apt install tshark
 ```
```

### Comparing `enso-nic-0.1.2/enso/__main__.py` & `enso-nic-0.1.3/enso/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import click
 
 from enso.consts import (
-    DEFAULT_BATCH_SIZE,
     DEFAULT_DSC_BUF_SIZE,
     DEFAULT_ETH_PORT,
     DEFAULT_FPGA,
     DEFAULT_NB_FALLBACK_QUEUES,
     DEFAULT_NB_TX_CREDITS,
     DEFAULT_PKT_BUF_SIZE,
 )
-from enso.enso_dataplane import EnsoDataplane
+from enso.enso_nic import EnsoNic
 
 
 @click.command()
-@click.argument("host")
-@click.argument("remote_enso_path")
+@click.argument("enso_path")
+@click.option(
+    "--host",
+    default="localhost",
+    show_default=True,
+    help="Host to connect to run Ensō on.",
+)
 @click.option(
     "--fpga", default=DEFAULT_FPGA, show_default=True, help="Choose the FPGA."
 )
 @click.option(
     "--dsc-buf-size",
     default=DEFAULT_DSC_BUF_SIZE,
     show_default=True,
@@ -64,66 +68,57 @@
 @click.option(
     "--enable-rr/--disable-rr",
     default=False,
     show_default=True,
     help="Enable/Disable packet round robin to fallback queues.",
 )
 @click.option(
-    "--batch-size",
-    default=DEFAULT_BATCH_SIZE,
-    show_default=True,
-    type=int,
-    help="Number of packets in a batch.",
-)
-@click.option(
     "--latency-opt/--throughput-opt",
     default=False,
     show_default=True,
     help="Optimize for throughput/latency.",
 )
 @click.option(
     "--load-bitstream/--no-load-bitstream",
     default=True,
     show_default=True,
     help="Enable/Disable packet FPGA bitstream reload.",
 )
 def main(
     host,
-    remote_enso_path,
+    enso_path,
     fpga,
     dsc_buf_size,
     pkt_buf_size,
     tx_credits,
     eth_port,
     fallback_queues,
     desc_per_pkt,
     enable_rr,
-    batch_size,
     latency_opt,
     load_bitstream,
 ):
 
-    enso_dp = EnsoDataplane(
+    enso_nic = EnsoNic(
         fpga,
-        host,
-        remote_enso_path,
+        enso_path,
+        host_name=host,
         load_bitstream=load_bitstream,
         ensure_clean=True,
         setup_sw=True,
         dsc_buf_size=dsc_buf_size,
         pkt_buf_size=pkt_buf_size,
         tx_credits=tx_credits,
         ethernet_port=eth_port,
         fallback_queues=fallback_queues,
         desc_per_pkt=desc_per_pkt,
         enable_rr=enable_rr,
-        sw_batch_size=batch_size,
         latency_opt=latency_opt,
         verbose=True,
         log_file=True,
     )
 
-    enso_dp.interactive_shell()
+    enso_nic.interactive_shell()
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `enso-nic-0.1.2/enso/enso_dataplane.py` & `enso-nic-0.1.3/enso/enso_nic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,90 +1,87 @@
-from typing import TextIO, Union
+from typing import TextIO, Union, Optional
 
-from netexp.helpers import RemoteIntelFpga, remote_command, watch_command
+from netexp.helpers import IntelFpga
 
 from enso.consts import (
-    DEFAULT_BATCH_SIZE,
     DEFAULT_DSC_BUF_SIZE,
     DEFAULT_ETH_PORT,
     DEFAULT_NB_FALLBACK_QUEUES,
     DEFAULT_NB_TX_CREDITS,
     DEFAULT_PKT_BUF_SIZE,
     SETUP_SW_CMD,
 )
 
 
-LOAD_BITSTREAM_CMD = "hardware_test/load_bitstream.sh"
-RUN_CONSOLE_CMD = "hardware_test/run_console.sh"
+LOAD_BITSTREAM_CMD = "scripts/load_bitstream.sh"
+RUN_CONSOLE_CMD = "scripts/run_console.sh"
 
 
-class EnsoDataplane(RemoteIntelFpga):
-    """Class to control the Ensō dataplane.
+class EnsoNic(IntelFpga):
+    """Class to control the Ensō NIC.
 
-    This class can automatically load the bitstream, configure the dataplane
-    using JTAG and recompile the library according to the specified parameters.
+    This class can automatically load the bitstream, configure the NIC using
+    JTAG and recompile the library according to the specified parameters.
 
     Attributes:
         fpga_id:
-        host:
-        remote_enso_path:
+        enso_path:
+        host_name:
         load_bitstream:
         ensure_clean:
         setup_sw:
         dsc_buf_size:
         pkt_buf_size:
         tx_credits:
         ethernet_port:
         fallback_queues:
         desc_per_pkt:
         enable_rr:
-        sw_batch_size:
         skip_config:
         verbose:
         log_file:
     """
 
     def __init__(
         self,
         fpga_id: str,
-        host: str,
-        remote_enso_path: str,
+        enso_path: str,
+        host_name: Optional[str] = None,
         load_bitstream: bool = True,
         ensure_clean: bool = True,
         setup_sw: bool = True,
         sw_reset: bool = False,
         dsc_buf_size: int = DEFAULT_DSC_BUF_SIZE,
         pkt_buf_size: int = DEFAULT_PKT_BUF_SIZE,
         tx_credits: int = DEFAULT_NB_TX_CREDITS,
         ethernet_port: int = DEFAULT_ETH_PORT,
         fallback_queues: int = DEFAULT_NB_FALLBACK_QUEUES,
         desc_per_pkt: bool = False,
         enable_rr: bool = False,
-        sw_batch_size: int = DEFAULT_BATCH_SIZE,
         latency_opt: bool = False,
         skip_config: bool = False,
         verbose: bool = False,
         log_file: Union[bool, TextIO] = False,
     ):
         if load_bitstream and verbose:
             print("Loading bitstream, it might take a couple of seconds.")
 
-        load_bitstream_cmd = f"{remote_enso_path}/{LOAD_BITSTREAM_CMD}"
-        run_console_cmd = f"{remote_enso_path}/{RUN_CONSOLE_CMD}"
+        load_bitstream_cmd = f"{enso_path}/{LOAD_BITSTREAM_CMD}"
+        run_console_cmd = f"{enso_path}/{RUN_CONSOLE_CMD}"
 
         super().__init__(
-            host,
             fpga_id,
             run_console_cmd,
             load_bitstream_cmd,
+            host_name=host_name,
             load_bitstream=load_bitstream,
             log_file=log_file,
         )
 
-        self.remote_enso_path = remote_enso_path
+        self.enso_path = enso_path
 
         if ensure_clean and load_bitstream:
             output = self.run_jtag_commands("read_pcie")
             lines = [ln for ln in output.split("\n") if " : 0x" in ln]
             for ln in lines:
                 reg_value = ln.split(" : ")[1]
                 if int(reg_value, 16) != 0:
@@ -113,29 +110,26 @@
                 self.disable_desc_per_pkt()
 
             if enable_rr:
                 self.enable_rr()
             else:
                 self.disable_rr()
 
-        self.sw_batch_size = sw_batch_size
         self.latency_opt = latency_opt
 
         if setup_sw:
             self.setup_sw()
 
     def setup_sw(self):
-        sw_setup = remote_command(
-            self.ssh_client,
-            f"{self.remote_enso_path}/{SETUP_SW_CMD} {self.dsc_buf_size} "
-            f"{self.pkt_buf_size} {self.sw_batch_size} {self.latency_opt}",
+        sw_setup = self.host.run_command(
+            f"{self.enso_path}/{SETUP_SW_CMD} {self.dsc_buf_size} "
+            f"{self.pkt_buf_size} {self.latency_opt}",
             pty=True,
         )
-        watch_command(
-            sw_setup,
+        sw_setup.watch(
             keyboard_int=lambda: sw_setup.send("\x03"),
             stdout=self.log_file,
             stderr=self.log_file,
         )
         status = sw_setup.recv_exit_status()
         if status != 0:
             raise RuntimeError("Error occurred while setting up software")
@@ -144,14 +138,17 @@
         output = self.run_jtag_commands("s")
         start_index = output.find("IN_PKT: ")
         output = output[start_index:]
         stats = {}
         for row in output.split("\r\n"):
             if row.startswith("% "):
                 break
+
+            if ":" not in row:
+                continue
             key, value = row.split(": ")
             stats[key] = int(value)
         return stats
 
     @property
     def dsc_buf_size(self):
         return self._dsc_buf_size
```

### Comparing `enso-nic-0.1.2/enso/enso_pktgen.py` & `enso-nic-0.1.3/enso/ensogen.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 import tempfile
 
 from collections import defaultdict
 from csv import DictReader
 from fractions import Fraction
 from typing import Optional, TextIO, Union
 
-from netexp.helpers import remote_command, watch_command, download_file
-from netexp.pcap import mean_pkt_size_remote_pcap
+from netexp.helpers import download_file
+from netexp.pcap import mean_pkt_size_pcap
 from netexp.pktgen import Pktgen
 
 from enso.consts import (
     FPGA_RATELIMIT_CLOCK,
-    ENSO_PKTGEN_CMD,
+    ENSOGEN_CMD,
     PCAP_GEN_CMD,
     PCAPS_DIR,
 )
-from enso.enso_dataplane import EnsoDataplane
+from enso.enso_nic import EnsoNic
 
 
 ETHERNET_OVERHEAD = 20 + 4  # Includes CRC.
 
 
-class EnsoPktgenStats:
+class EnsoGenStats:
     def __init__(self, file_name: str) -> None:
         self.stats = defaultdict(list)
         self.nb_samples = 0
         with open(file_name, newline="") as f:
             csv_reader = DictReader(f)
             for row in csv_reader:
                 self.nb_samples += 1
@@ -79,77 +79,76 @@
 
 
 class EnsoGen(Pktgen):
     """Python wrapper for the EnsōGen packet generator."""
 
     def __init__(
         self,
-        dataplane: EnsoDataplane,
+        nic: EnsoNic,
         core_id: int = 0,
         queues: int = 4,
-        multicore: bool = False,
+        single_core: bool = False,
         rtt: bool = False,
         rtt_hist: bool = False,
         rtt_hist_offset: Optional[int] = None,
         rtt_hist_len: Optional[int] = None,
         stats_file: Optional[str] = None,
         hist_file: Optional[str] = None,
         stats_delay: Optional[int] = None,
         pcie_addr: Optional[str] = None,
-        verbose: bool = False,
         log_file: Union[bool, TextIO] = False,
         check_tx_rate=False,
     ) -> None:
         super().__init__()
 
-        self.dataplane = dataplane
-        self.dataplane.enable_rr()
-        self.dataplane.fallback_queues = queues
+        self.nic = nic
+        self.nic.enable_rr()
+        self.nic.fallback_queues = queues
 
         self._pcap_path = None
 
         self.core_id = core_id
-        self.multicore = multicore
+        self.single_core = single_core
         self.rtt = rtt
         self.rtt_hist = rtt_hist
         self.rtt_hist_offset = rtt_hist_offset
         self.rtt_hist_len = rtt_hist_len
         self.stats_delay = stats_delay
 
         if pcie_addr is not None and pcie_addr.count(":") == 1:
             pcie_addr = f"0000:{pcie_addr}"  # Add domain.
         self.pcie_addr = pcie_addr
 
         self.stats_file = stats_file or "stats.csv"
         self.hist_file = hist_file or "hist.csv"
 
-        self.verbose = verbose
         self.log_file = log_file
         self.check_tx_rate = check_tx_rate
 
         self.pktgen_cmd = None
 
         self.clean_stats()
 
     def set_params(self, pkt_size: int, nb_src: int, nb_dst: int) -> None:
         nb_pkts = nb_src * nb_dst
 
         pcap_name = f"{nb_pkts}_{pkt_size}_{nb_src}_{nb_dst}.pcap"
 
-        remote_dir_path = Path(self.dataplane.remote_enso_path)
+        remote_dir_path = Path(self.nic.enso_path)
         pcap_dst = remote_dir_path / Path(PCAPS_DIR) / Path(pcap_name)
         pcap_gen_cmd = remote_dir_path / Path(PCAP_GEN_CMD)
         pcap_gen_cmd = (
             f"{pcap_gen_cmd} {nb_pkts} {pkt_size} {nb_src} {nb_dst} {pcap_dst}"
         )
 
-        pcap_gen_cmd = remote_command(
-            self.dataplane.ssh_client, pcap_gen_cmd, print_command=self.verbose
+        pcap_gen_cmd = self.nic.host.run_command(
+            pcap_gen_cmd, print_command=self.log_file
         )
-        watch_command(pcap_gen_cmd, stdout=self.log_file, stderr=self.log_file)
+        pcap_gen_cmd.watch(stdout=self.log_file, stderr=self.log_file)
+
         status = pcap_gen_cmd.recv_exit_status()
         if status != 0:
             raise RuntimeError("Error generating pcap")
 
         self.pcap_path = pcap_dst
 
     def start(self, throughput: float, nb_pkts: int) -> None:
@@ -172,39 +171,36 @@
 
         self.current_throughput = throughput
         self.current_goodput = pkts_per_sec * flits_per_pkt * 512
         self.current_pps = pkts_per_sec
         self.expected_tx_duration = nb_pkts / pkts_per_sec
 
         # Make sure remote stats file does not exist.
-        remote_stats_file = remote_command(
-            self.dataplane.ssh_client,
+        remove_stats_file = self.nic.host.run_command(
             f"rm -f {self.stats_file}",
             print_command=False,
         )
-        watch_command(
-            remote_stats_file, stdout=self.log_file, stderr=self.log_file
-        )
-        status = remote_stats_file.recv_exit_status()
+        remove_stats_file.watch(stdout=self.log_file, stderr=self.log_file)
+        status = remove_stats_file.recv_exit_status()
         if status != 0:
             raise RuntimeError(
                 f"Error removing remote stats file ({self.stats_file})"
             )
 
         command = (
-            f"sudo {self.dataplane.remote_enso_path}/{ENSO_PKTGEN_CMD}"
+            f"sudo {self.nic.enso_path}/{ENSOGEN_CMD}"
             f" {self.pcap_path} {rate_frac.numerator} {rate_frac.denominator}"
             f" --count {nb_pkts}"
             f" --core {self.core_id}"
             f" --queues {self.queues}"
             f" --save {self.stats_file}"
         )
 
-        if self.multicore:
-            command += " --multicore"
+        if self.single_core:
+            command += " --single-core"
 
         if self.rtt:
             command += " --rtt"
 
         if self.rtt_hist:
             command += f" --rtt-hist {self.hist_file}"
 
@@ -216,33 +212,33 @@
 
         if self.stats_delay is not None:
             command += f" --stats-delay {self.stats_delay}"
 
         if self.pcie_addr is not None:
             command += f" --pcie-addr {self.pcie_addr}"
 
-        self.pktgen_cmd = remote_command(
-            self.dataplane.ssh_client,
+        self.pktgen_cmd = self.nic.host.run_command(
             command,
-            print_command=self.verbose,
+            print_command=self.log_file,
             pty=True,
         )
 
     def wait_transmission_done(self) -> None:
-        if self.pktgen_cmd is None:
+        pktgen_cmd = self.pktgen_cmd
+
+        if pktgen_cmd is None:
             # Pktgen is not running.
             return
 
-        watch_command(
-            self.pktgen_cmd,
+        pktgen_cmd.watch(
             stdout=self.log_file,
             stderr=self.log_file,
-            keyboard_int=lambda: self.pktgen_cmd.send(b"\x03"),
+            keyboard_int=lambda: pktgen_cmd.send(b"\x03"),
         )
-        status = self.pktgen_cmd.recv_exit_status()
+        status = pktgen_cmd.recv_exit_status()
         if status != 0:
             raise RuntimeError("Error running EnsōGen")
 
         self.update_stats()
 
         self.pktgen_cmd = None
 
@@ -254,16 +250,17 @@
             and (self.current_throughput > 50e9)
             and (self.expected_tx_duration > 4)
         )
 
         # Retrieve the latest stats.
         with tempfile.TemporaryDirectory() as tmp:
             local_stats = f"{tmp}/stats.csv"
-            download_file(self.dataplane.host, self.stats_file, local_stats)
-            parsed_stats = EnsoPktgenStats(local_stats)
+            download_file(self.nic.host_name, self.stats_file, local_stats,
+                          self.log_file)
+            parsed_stats = EnsoGenStats(local_stats)
 
             stats_summary = parsed_stats.get_summary(calculate_tx_mean)
 
         # Check TX rate.
         if calculate_tx_mean:
             tx_goodput_mbps = stats_summary["tx_mean_goodput_mbps"]
             tx_goodput_gbps = tx_goodput_mbps / 1e3
@@ -293,39 +290,36 @@
 
     @property
     def pcap_path(self) -> None:
         return self._pcap_path
 
     @pcap_path.setter
     def pcap_path(self, pcap_path) -> None:
-        self.mean_pcap_pkt_size = mean_pkt_size_remote_pcap(
-            self.dataplane.ssh_client, pcap_path
-        )
-
+        self.mean_pcap_pkt_size = mean_pkt_size_pcap(self.nic.host, pcap_path)
         self._pcap_path = pcap_path
 
     @property
     def queues(self) -> int:
-        return self.dataplane.fallback_queues
+        return self.nic.fallback_queues
 
     @queues.setter
     def queues(self, queues) -> None:
-        self.dataplane.fallback_queues = queues
+        self.nic.fallback_queues = queues
 
     def get_nb_rx_pkts(self) -> int:
         return self.nb_rx_pkts
 
     def get_nb_tx_pkts(self) -> int:
         return self.nb_tx_pkts
 
     def get_rx_throughput(self) -> int:
-        return self.mean_rx_goodput + self.mean_rx_rate * 20 * 8
+        return self.mean_rx_goodput + self.mean_rx_rate * 24 * 8
 
     def get_tx_throughput(self) -> int:
-        return self.mean_tx_goodput + self.mean_tx_rate * 20 * 8
+        return self.mean_tx_goodput + self.mean_tx_rate * 24 * 8
 
     def clean_stats(self) -> None:
         self.nb_rx_pkts = 0
         self.nb_rx_bytes = 0
         self.mean_rx_goodput = 0
         self.mean_rx_rate = 0
         self.nb_tx_pkts = 0
@@ -335,21 +329,26 @@
         self.mean_rtt = 0
 
     def stop(self) -> None:
         if self.pktgen_cmd is None:
             # Pktgen is not running.
             return
 
+        if self.pktgen_cmd.exit_status_ready():
+            # Pktgen has already exited.
+            self.pktgen_cmd = None
+            return
+
         self.pktgen_cmd.send(b"\x03")
 
-        watch_command(
-            self.pktgen_cmd, stdout=self.log_file, stderr=self.log_file
-        )
+        self.pktgen_cmd.watch(stdout=self.log_file, stderr=self.log_file)
         status = self.pktgen_cmd.recv_exit_status()
         if status != 0:
             raise RuntimeError("Error stopping EnsōGen")
 
         self.update_stats()
 
+        self.pktgen_cmd = None
+
     def close(self) -> None:
         # No need to close here.
         pass
```

### Comparing `enso-nic-0.1.2/enso_nic.egg-info/PKG-INFO` & `enso-nic-0.1.3/enso_nic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 Metadata-Version: 2.1
 Name: enso-nic
-Version: 0.1.2
-Summary: Python frontend for the Ensō dataplane.
-Home-page: https://github.com/hsadok/enso
-Download-URL: https://github.com/hsadok/enso
+Version: 0.1.3
+Summary: Python frontend for the Ensō NIC.
+Home-page: https://github.com/crossroadsfpga/enso
+Download-URL: https://github.com/crossroadsfpga/enso
 Author: Hugo Sadok
 Author-email: sadok@cmu.edu
 License: BSD
-Keywords: network,enso,dataplane,nic
+Keywords: network,enso,nic
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Ensō Python Frontend
 
 ## Install
 
 To install the frontend run in the current directory (`frontend`):
 ```bash
-pip3 install -e .
+python3 -m pip install -e .
 ```
 To run the EnsōGen packet generator you also need to have the `capinfos` command installed in the machine you want to use to generate packets.
 
 On Ubuntu (or other Debian-based system) run:
 ```bash
 sudo apt install tshark
 ```
```

### Comparing `enso-nic-0.1.2/setup.py` & `enso-nic-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,39 +19,37 @@
         io.open(f"{name}/__init__.py", encoding="utf_8_sig").read(),
     ).group(1)
 
 
 setup(
     name=package_name,
     version=find_meta("__version__"),
-    description="Python frontend for the Ensō dataplane.",
+    description="Python frontend for the Ensō NIC.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
-    url="https://github.com/hsadok/enso",
-    download_url="https://github.com/hsadok/enso",
+    url="https://github.com/crossroadsfpga/enso",
+    download_url="https://github.com/crossroadsfpga/enso",
     license="BSD",
     author=find_meta("__author__"),
     author_email=find_meta("__email__"),
-    keywords=["network", "enso", "dataplane", "nic"],
-    python_requires=">=3.7",
+    keywords=["network", "enso", "nic"],
+    python_requires=">=3.9",
     entry_points={"console_scripts": ["enso=enso.__main__:main"]},
     include_package_data=True,
-    install_requires=["click>=8.0", "netexp==0.1.12", "tqdm"],
-    setup_requires=["pytest-runner"],
-    tests_require=["pytest"],
+    install_requires=["click>=8.0", "netexp==0.1.17", "scapy"],
+    # setup_requires=["pytest-runner"],
+    # tests_require=["pytest"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: System :: Networking",
         "Topic :: System :: Systems Administration",
     ],
 )
```

