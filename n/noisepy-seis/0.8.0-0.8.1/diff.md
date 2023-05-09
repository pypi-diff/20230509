# Comparing `tmp/noisepy_seis-0.8.0.tar.gz` & `tmp/noisepy_seis-0.8.1.tar.gz`

## Comparing `noisepy_seis-0.8.0.tar` & `noisepy_seis-0.8.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11984 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    12728 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    16328 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/asdfstore.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/channelcatalog.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/datatypes.py
--rw-r--r--   0        0        0     6841 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   112952 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    35394 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/scedc_s3store.py
--rw-r--r--   0        0        0     1994 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/stores.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/utils.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6880 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/LICENSE
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/README.md
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 noisepy_seis-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    13464 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    15939 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/asdfstore.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/channelcatalog.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/datatypes.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   112958 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    35085 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/scedc_s3store.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/stores.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/utils.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/LICENSE
+-rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/README.md
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/PKG-INFO
```

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.8.1/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     downsampling and trimming to a day length;
     3) saves data into ASDF format (see Krischer et al., 2016 for
     more details on the data structure);
     4) parallelize the downloading processes with MPI.
     5) avoids downloading data for stations that already have 1 or 3 channels
 
 Authors: Chengxin Jiang (chengxin_jiang@fas.harvard.edu)
-         Marine Denolle (mdenolle@fas.harvard.edu)
+         Marine Denolle (mdenolle@uw.edu)
 
 NOTE:
     0. MOST occasions you just need to change parameters followed
     with detailed explanations to run the script.
     1. to avoid segmentation fault later in cross-correlation
     calculations due to too large data in memory, a rough
     estimation of the memory needs is made in the beginning of the
@@ -58,32 +58,35 @@
 
 Enjoy the NoisePy journey!
 """
 
 #########################################################
 ################ PARAMETER SECTION ######################
 #########################################################
-tt0 = time.time()
 
 # download parameters
-client = Client("SCEDC")  # client/data center. see https://docs.obspy.org/packages/obspy.clients.fdsn.html for a list
 
 # get rough estimate of memory needs to ensure it now below up in S1
 MAX_MEM = 5.0  # maximum memory allowed per core in GB
 
 ##################################################
 # we expect no parameters need to be changed below
 
 
 def download(
     direc: str,
     chan_list: List[str],
     sta_list: List[str],
     prepro_para: ConfigParameters,
+    client_url_key: str = "SCEDC",
 ):
+    # client/data center. see https://docs.obspy.org/packages/obspy.clients.fdsn.html for a list
+    client = Client(client_url_key)
+
+    tt0 = time.time()
     dlist = os.path.join(direc, "station.txt")  # CSV file for station location info
     prepro_para.respdir = os.path.join(
         direc, "../resp"
     )  # directory where resp files are located (required if rm_resp is neither 'no' nor 'inv')
     # time tags
     starttime = obspy.UTCDateTime(prepro_para.start_date)
     endtime = obspy.UTCDateTime(prepro_para.end_date)
```

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.8.1/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.8.1/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,17 +96,20 @@
     for ick in range(rank, splits, size):
         t10 = time.time()
         ts = timespans[ick]
         if cc_store.is_done(ts):
             continue
 
         # ###########LOADING NOISE DATA AND DO FFT##################
+        t0 = time.time()
         channels = raw_store.get_channels(ts)
         ch_data_tuples = _read_channels(ts, raw_store, channels, fft_params.samp_freq)
+        t01 = time.time()
         ch_data_tuples = preprocess(ch_data_tuples, raw_store, fft_params, ts)
+        t02 = time.time()
 
         nchannels = len(ch_data_tuples)
         nseg_chunk = check_memory(fft_params, nchannels)
         nnfft = int(next_fast_len(int(fft_params.cc_len * fft_params.samp_freq)))  # samp_freq should be sampling_rate
         # open array to store fft data/info in memory
         fft_array = np.zeros((nchannels, nseg_chunk * (nnfft // 2)), dtype=np.complex64)
         fft_std = np.zeros((nchannels, nseg_chunk), dtype=np.float32)
@@ -127,28 +130,34 @@
 
         # check whether array size is enough
         if np.sum(fft_flag) != nchannels:
             logger.warning("it seems some stations miss data in download step, but it is OKAY!")
 
         # ###########PERFORM CROSS-CORRELATION##################
         for iiS in range(nchannels):  # looping over the channel source
-            src_chan = channels[iiS]
+            src_chan = channels[iiS]  # this is the name of the source channel
             fft1 = fft_array[iiS]
-            source_std = fft_std[iiS]
+            source_std = fft_std[iiS]  # this is the array of data metrics
+
+            # this finds the windows of "good" noise
             sou_ind = np.where((source_std < fft_params.max_over_std) & (source_std > 0) & (np.isnan(source_std) == 0))[
                 0
             ]
             if not fft_flag[iiS] or not len(sou_ind):
                 continue
-            t0 = time.time()
-            # -----------get the smoothed source spectrum for decon later----------
-            sfft1 = noise_module.smooth_source_spect(fft_params, fft1)
-            sfft1 = sfft1.reshape(N, Nfft2)
-            t1 = time.time()
-            logger.debug("smoothing source takes %6.4fs" % (t1 - t0))
+            # in the case of pure deconvolution, we recommend smoothing anyway.
+            if fft_params.cc_method == "deconv":
+                t00 = time.time()
+                # -----------get the smoothed source spectrum for decon later----------
+                sfft1 = noise_module.smooth_source_spect(fft_params, fft1)
+                sfft1 = sfft1.reshape(N, Nfft2)
+                t10 = time.time()
+                logger.debug("smoothing source takes %6.4fs" % (t10 - t00))
+            else:
+                sfft1 = fft1.reshape(N, Nfft2)
 
             # get index right for auto/cross correlation
             istart = iiS  # start at the channel source / only fills the upper right triangle matrix of channel pairs
             iend = nchannels
             #             if ncomp==1:
             #                 iend=np.minimum(iiS+ncomp,iii)
             #             else:
@@ -180,42 +189,49 @@
                         continue
                 logger.debug(f"receiver: {rec_chan}")
                 if not fft_flag[iiR]:
                     continue
                 if cc_store.contains(ts, src_chan, rec_chan, fft_params):
                     continue
 
+                # read the receiver data
                 fft2 = fft_array[iiR]
                 sfft2 = fft2.reshape(N, Nfft2)
                 receiver_std = fft_std[iiR]
 
-                # ---------- check the existence of earthquakes ----------
+                # ---------- check the existence of earthquakes or spikes ----------
                 rec_ind = np.where(
                     (receiver_std < fft_params.max_over_std) & (receiver_std > 0) & (np.isnan(receiver_std) == 0)
                 )[0]
                 bb = np.intersect1d(sou_ind, rec_ind)
                 if len(bb) == 0:
                     continue
 
+                # ----------- GAME TIME: cross correlation step ---------------
                 t2 = time.time()
                 corr, tcorr, ncorr = noise_module.correlate(
                     sfft1[bb, :], sfft2[bb, :], fft_params, Nfft, fft_time[iiR][bb]
                 )
                 t3 = time.time()
+
+                # ---------- OUTPUT: store metadata and data into file ------------
                 coor = {
                     "lonS": src_chan.station.lon,
                     "latS": src_chan.station.lat,
                     "lonR": rec_chan.station.lon,
                     "latR": rec_chan.station.lat,
                 }
                 comp = src_chan.type.get_orientation() + rec_chan.type.get_orientation()
                 parameters = noise_module.cc_parameters(fft_params, coor, tcorr, ncorr, comp)
                 cc_store.append(ts, src_chan, rec_chan, fft_params, parameters, corr)
                 t4 = time.time()
-                logger.debug("read S %6.4fs, cc %6.4fs, write cc %6.4fs" % ((t1 - t0), (t3 - t2), (t4 - t3)))
+                logger.debug(
+                    "read S %6.4fs, process %6.4fs, cc %6.4fs, write cc %6.4fs"
+                    % ((t01 - t0), (t02 - t01), (t3 - t2), (t4 - t3))
+                )
 
                 del fft2, sfft2, receiver_std
             del fft1, sfft1, source_std
 
         fft_array = []
         fft_std = []
         fft_flag = []
```

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.8.1/src/noisepy/seis/S2_stacking.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import glob
 import logging
 import os
 import sys
 import time
+from typing import List
 
 import numpy as np
 import pandas as pd
 import pyasdf
 from mpi4py import MPI
 
 from . import noise_module
@@ -50,28 +51,21 @@
 correction = False  # angle correction due to mis-orientation
 
 # maximum memory allowed per core in GB
 MAX_MEM = 4.0
 
 
 # TODO: make stack_method an enum
-def stack(raw_dir: str, ccf_dir: str, stack_dir: str, stack_method: str):
+def stack(sta: List[str], ccf_dir: str, stack_dir: str, stack_method: str):
     if rotation and correction:
         corrfile = os.path.join(ccf_dir, "../meso_angles.txt")  # csv file containing angle info to be corrected
         locs = pd.read_csv(corrfile)
     else:
         locs = []
 
-    # absolute path parameters
-    locations = os.path.join(
-        raw_dir, "station.txt"
-    )  # station info including network,station,channel,latitude,longitude,elevation
-    if not os.path.isfile(locations):
-        raise ValueError("Abort! station info is needed for this script")
-
     ##################################################
     # we expect no parameters need to be changed below
 
     # load fc_para parameters from Step1
     fc_metadata = os.path.join(ccf_dir, "fft_cc_data.txt")
     fc_para = eval(open(fc_metadata).read())
     ncomp = fc_para["ncomp"]
@@ -130,17 +124,14 @@
         fout.write(str(stack_para))
         fout.close()
 
         # cross-correlation files
         ccfiles = sorted(glob.glob(os.path.join(ccf_dir, "*.h5")))
         logger.debug(ccfiles)
 
-        # load station info
-        tlocs = pd.read_csv(locations)
-        sta = sorted(np.unique(tlocs["network"] + "." + tlocs["station"]))
         for ii in range(len(sta)):
             tmp = os.path.join(stack_dir, sta[ii])
             if not os.path.isdir(tmp):
                 os.mkdir(tmp)
 
         # station-pairs
         pairs_all = []
@@ -261,15 +252,15 @@
                     cc_comp[iseg] = tcmp1 + tcmp2
                     iseg += 1
 
         t1 = time.time()
         logger.debug("loading CCF data takes %6.2fs" % (t1 - t0))
 
         # continue when there is no data or for auto-correlation
-        if iseg <= 1 or fauto == 1:
+        if iseg <= 1 and fauto == 1:
             continue
         outfn = pairs_all[ipair] + ".h5"
         logger.debug("ready to output to %s" % (outfn))
 
         # matrix used for rotation
         if rotation:
             bigstack = np.zeros(shape=(9, npts_segmt), dtype=np.float32)
@@ -277,15 +268,15 @@
             bigstack1 = np.zeros(shape=(9, npts_segmt), dtype=np.float32)
             bigstack2 = np.zeros(shape=(9, npts_segmt), dtype=np.float32)
 
         # loop through cross-component for stacking
         iflag = 1
         for icomp in range(nccomp):
             comp = enz_system[icomp]
-            indx = np.where(cc_comp == comp)[0]
+            indx = np.where(cc_comp.lower() == comp.lower())[0]
             logger.debug(f"index to find the comp: {indx}")
 
             # jump if there are not enough data
             if len(indx) < 2:
                 iflag = 0
                 break
```

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/__init__.py` & `noisepy_seis-0.8.1/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/asdfstore.py` & `noisepy_seis-0.8.1/src/noisepy/seis/asdfstore.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     def _parse_timespans(self, filename: str) -> DateTimeRange:
         parts = os.path.splitext(os.path.basename(filename))[0].split("T")
         dates = [obspy.UTCDateTime(p).datetime.replace(tzinfo=datetime.timezone.utc) for p in parts]
         return DateTimeRange(dates[0], dates[1])
 
     def _create_station(self, timespan: DateTimeRange, name: str) -> Optional[Station]:
-        # What should we do if there's not StationXML?
+        # What should we do if there's no StationXML?
         try:
             inventory = self.get_dataset(str(timespan)).waveforms[name]["StationXML"]
             sta, net, lon, lat, elv, loc = noise_module.sta_info_from_inv(inventory)
             return Station(net, sta, lat, lon, elv, loc)
         except Exception as e:
             logger.warning(f"Missing StationXML for station {name}. {e}")
             return None
```

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/channelcatalog.py` & `noisepy_seis-0.8.1/src/noisepy/seis/channelcatalog.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/datatypes.py` & `noisepy_seis-0.8.1/src/noisepy/seis/datatypes.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/main.py` & `noisepy_seis-0.8.1/src/noisepy/seis/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,40 +76,48 @@
         else:
             raise ValueError(f"Either an --xml_path argument or a {STATION_FILE} must be provided")
 
         return SCEDCS3DataStore(raw_dir, catalog, get_channel_filter(sta_list))
 
 
 def main(args: typing.Any):
+    raw_dir = args.raw_data_path
+
+    def get_raw_store():
+        stations = args.stations if "stations" in args else []
+        xml_path = args.xml_path if "xml_path" in args else None
+        return create_raw_store(raw_dir, stations, xml_path)
+
     def run_cross_correlation():
-        raw_dir = args.raw_data_path
         ccf_dir = args.ccf_path
         fft_params = initialize_fft_params(raw_dir)
         fft_params.freq_norm = args.freq_norm
         cc_store = ASDFCCStore(ccf_dir)
-        raw_store = create_raw_store(raw_dir, args.stations, args.xml_path)
+        raw_store = get_raw_store()
         cross_correlate(raw_store, fft_params, cc_store)
 
     def run_download():
         params = ConfigParameters()
         params.start_date = args.start
         params.end_date = args.end
         params.inc_hours = args.inc_hours
         download(args.raw_data_path, args.channels, args.stations, params)
 
     if args.step == Step.DOWNLOAD:
         run_download()
     if args.step == Step.CROSS_CORRELATE:
         run_cross_correlation()
     if args.step == Step.STACK:
-        stack(args.raw_data_path, args.ccf_path, args.stack_path, args.method)
+        raw_store = get_raw_store()
+        stack(raw_store.get_station_list(), args.ccf_path, args.stack_path, args.method)
     if args.step == Step.ALL:
         run_download()
         run_cross_correlation()
-        stack(args.raw_data_path, args.ccf_path, args.stack_path, args.method)
+        raw_store = get_raw_store()
+        stack(raw_store.get_station_list(), args.ccf_path, args.stack_path, args.method)
 
 
 def add_download_args(down_parser: argparse.ArgumentParser):
     down_parser.add_argument(
         "--start",
         type=valid_date,
         required=True,
```

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.8.1/src/noisepy/seis/noise_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -717,6344 +717,6344 @@
 00002cc0: 222c 0a20 2020 2020 2020 2020 2020 207d  ",.            }
 00002cd0: 0a20 2020 2020 2020 2020 2020 2073 742e  .            st.
 00002ce0: 7369 6d75 6c61 7465 2870 617a 5f72 656d  simulate(paz_rem
 00002cf0: 6f76 653d 4e6f 6e65 2c20 7072 655f 6669  ove=None, pre_fi
 00002d00: 6c74 3d70 7265 5f66 696c 742c 2073 6565  lt=pre_filt, see
 00002d10: 6472 6573 703d 7365 6564 7265 7370 290a  dresp=seedresp).
 00002d20: 0a20 2020 2020 2020 2065 6c69 6620 726d  .        elif rm
-00002d30: 5f72 6573 7020 3d3d 2022 706f 6c6f 7a65  _resp == "poloze
-00002d40: 726f 7322 3a0a 2020 2020 2020 2020 2020  ros":.          
-00002d50: 2020 7072 696e 7428 2272 656d 6f76 6520    print("remove 
-00002d60: 7265 7370 6f6e 7365 2075 7369 6e67 2070  response using p
-00002d70: 6f6c 6f73 2061 6e64 207a 6572 6f73 2229  olos and zeros")
-00002d80: 0a20 2020 2020 2020 2020 2020 2070 617a  .            paz
-00002d90: 5f73 7473 203d 2067 6c6f 622e 676c 6f62  _sts = glob.glob
-00002da0: 286f 732e 7061 7468 2e6a 6f69 6e28 7265  (os.path.join(re
-00002db0: 7370 6469 722c 2022 2a22 202b 2073 7461  spdir, "*" + sta
-00002dc0: 7469 6f6e 202b 2022 2a22 2929 0a20 2020  tion + "*")).   
-00002dd0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00002de0: 7061 7a5f 7374 7329 203d 3d20 303a 0a20  paz_sts) == 0:. 
-00002df0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00002e00: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00002e10: 226e 6f20 706f 6c6f 7a65 726f 7320 666f  "no polozeros fo
-00002e20: 756e 6420 666f 7220 2573 2220 2520 7374  und for %s" % st
-00002e30: 6174 696f 6e29 0a20 2020 2020 2020 2020  ation).         
-00002e40: 2020 2073 742e 7369 6d75 6c61 7465 2870     st.simulate(p
-00002e50: 617a 5f72 656d 6f76 653d 7061 7a5f 7374  az_remove=paz_st
-00002e60: 735b 305d 2c20 7072 655f 6669 6c74 3d70  s[0], pre_filt=p
-00002e70: 7265 5f66 696c 7429 0a0a 2020 2020 2020  re_filt)..      
-00002e80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00002e90: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00002ea0: 7272 6f72 2822 6e6f 2073 7563 6820 6f70  rror("no such op
-00002eb0: 7469 6f6e 2066 6f72 2072 6d5f 7265 7370  tion for rm_resp
-00002ec0: 2120 706c 6561 7365 2064 6f75 626c 6520  ! please double 
-00002ed0: 6368 6563 6b21 2229 0a0a 2020 2020 6e74  check!")..    nt
-00002ee0: 7220 3d20 6f62 7370 792e 5374 7265 616d  r = obspy.Stream
-00002ef0: 2829 0a20 2020 2023 2074 7269 6d20 6120  ().    # trim a 
-00002f00: 636f 6e74 696e 6f75 7320 7365 676d 656e  continous segmen
-00002f10: 7420 696e 746f 2075 7365 722d 6465 6669  t into user-defi
-00002f20: 6e65 6420 7365 7175 656e 6365 730a 2020  ned sequences.  
-00002f30: 2020 7374 5b30 5d2e 7472 696d 280a 2020    st[0].trim(.  
-00002f40: 2020 2020 2020 7374 6172 7474 696d 653d        starttime=
-00002f50: 7374 6172 7474 696d 652c 0a20 2020 2020  starttime,.     
-00002f60: 2020 2065 6e64 7469 6d65 3d65 6e64 7469     endtime=endti
-00002f70: 6d65 2c0a 2020 2020 2020 2020 7061 643d  me,.        pad=
-00002f80: 5472 7565 2c0a 2020 2020 2020 2020 6669  True,.        fi
-00002f90: 6c6c 5f76 616c 7565 3d30 2c0a 2020 2020  ll_value=0,.    
-00002fa0: 290a 2020 2020 6e74 722e 6170 7065 6e64  ).    ntr.append
-00002fb0: 2873 745b 305d 290a 0a20 2020 2072 6574  (st[0])..    ret
-00002fc0: 7572 6e20 6e74 720a 0a0a 6465 6620 7374  urn ntr...def st
-00002fd0: 6174 7332 696e 7628 7374 6174 732c 2070  ats2inv(stats, p
-00002fe0: 7265 7072 6f5f 7061 7261 2c20 6c6f 6373  repro_para, locs
-00002ff0: 3d4e 6f6e 6529 3a0a 2020 2020 2222 220a  =None):.    """.
-00003000: 2020 2020 7468 6973 2066 756e 6374 696f      this functio
-00003010: 6e20 6372 6561 7465 7320 696e 7665 6e74  n creates invent
-00003020: 6f72 7920 6769 7665 6e20 7468 6520 7374  ory given the st
-00003030: 6174 7320 7061 7261 6d65 7465 7273 2069  ats parameters i
-00003040: 6e20 616e 206f 6273 7079 2073 7472 6561  n an obspy strea
-00003050: 6d20 6f72 2061 2073 7461 7469 6f6e 206c  m or a station l
-00003060: 6973 742e 0a20 2020 2028 7573 6564 2069  ist..    (used i
-00003070: 6e20 5330 4229 0a20 2020 2050 4152 414d  n S0B).    PARAM
-00003080: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
+00002d30: 5f72 6573 7020 3d3d 2022 706f 6c65 737a  _resp == "polesz
+00002d40: 6572 6f73 223a 0a20 2020 2020 2020 2020  eros":.         
+00002d50: 2020 2070 7269 6e74 2822 7265 6d6f 7665     print("remove
+00002d60: 2072 6573 706f 6e73 6520 7573 696e 6720   response using 
+00002d70: 706f 6c65 7320 616e 6420 7a65 726f 7322  poles and zeros"
+00002d80: 290a 2020 2020 2020 2020 2020 2020 7061  ).            pa
+00002d90: 7a5f 7374 7320 3d20 676c 6f62 2e67 6c6f  z_sts = glob.glo
+00002da0: 6228 6f73 2e70 6174 682e 6a6f 696e 2872  b(os.path.join(r
+00002db0: 6573 7064 6972 2c20 222a 2220 2b20 7374  espdir, "*" + st
+00002dc0: 6174 696f 6e20 2b20 222a 2229 290a 2020  ation + "*")).  
+00002dd0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00002de0: 2870 617a 5f73 7473 2920 3d3d 2030 3a0a  (paz_sts) == 0:.
+00002df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e00: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00002e10: 2822 6e6f 2070 6f6c 6573 7a65 726f 7320  ("no poleszeros 
+00002e20: 666f 756e 6420 666f 7220 2573 2220 2520  found for %s" % 
+00002e30: 7374 6174 696f 6e29 0a20 2020 2020 2020  station).       
+00002e40: 2020 2020 2073 742e 7369 6d75 6c61 7465       st.simulate
+00002e50: 2870 617a 5f72 656d 6f76 653d 7061 7a5f  (paz_remove=paz_
+00002e60: 7374 735b 305d 2c20 7072 655f 6669 6c74  sts[0], pre_filt
+00002e70: 3d70 7265 5f66 696c 7429 0a0a 2020 2020  =pre_filt)..    
+00002e80: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00002e90: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00002ea0: 6545 7272 6f72 2822 6e6f 2073 7563 6820  eError("no such 
+00002eb0: 6f70 7469 6f6e 2066 6f72 2072 6d5f 7265  option for rm_re
+00002ec0: 7370 2120 706c 6561 7365 2064 6f75 626c  sp! please doubl
+00002ed0: 6520 6368 6563 6b21 2229 0a0a 2020 2020  e check!")..    
+00002ee0: 6e74 7220 3d20 6f62 7370 792e 5374 7265  ntr = obspy.Stre
+00002ef0: 616d 2829 0a20 2020 2023 2074 7269 6d20  am().    # trim 
+00002f00: 6120 636f 6e74 696e 6f75 7320 7365 676d  a continous segm
+00002f10: 656e 7420 696e 746f 2075 7365 722d 6465  ent into user-de
+00002f20: 6669 6e65 6420 7365 7175 656e 6365 730a  fined sequences.
+00002f30: 2020 2020 7374 5b30 5d2e 7472 696d 280a      st[0].trim(.
+00002f40: 2020 2020 2020 2020 7374 6172 7474 696d          starttim
+00002f50: 653d 7374 6172 7474 696d 652c 0a20 2020  e=starttime,.   
+00002f60: 2020 2020 2065 6e64 7469 6d65 3d65 6e64       endtime=end
+00002f70: 7469 6d65 2c0a 2020 2020 2020 2020 7061  time,.        pa
+00002f80: 643d 5472 7565 2c0a 2020 2020 2020 2020  d=True,.        
+00002f90: 6669 6c6c 5f76 616c 7565 3d30 2c0a 2020  fill_value=0,.  
+00002fa0: 2020 290a 2020 2020 6e74 722e 6170 7065    ).    ntr.appe
+00002fb0: 6e64 2873 745b 305d 290a 0a20 2020 2072  nd(st[0])..    r
+00002fc0: 6574 7572 6e20 6e74 720a 0a0a 6465 6620  eturn ntr...def 
+00002fd0: 7374 6174 7332 696e 7628 7374 6174 732c  stats2inv(stats,
+00002fe0: 2070 7265 7072 6f5f 7061 7261 2c20 6c6f   prepro_para, lo
+00002ff0: 6373 3d4e 6f6e 6529 3a0a 2020 2020 2222  cs=None):.    ""
+00003000: 220a 2020 2020 7468 6973 2066 756e 6374  ".    this funct
+00003010: 696f 6e20 6372 6561 7465 7320 696e 7665  ion creates inve
+00003020: 6e74 6f72 7920 6769 7665 6e20 7468 6520  ntory given the 
+00003030: 7374 6174 7320 7061 7261 6d65 7465 7273  stats parameters
+00003040: 2069 6e20 616e 206f 6273 7079 2073 7472   in an obspy str
+00003050: 6561 6d20 6f72 2061 2073 7461 7469 6f6e  eam or a station
+00003060: 206c 6973 742e 0a20 2020 2028 7573 6564   list..    (used
+00003070: 2069 6e20 5330 4229 0a20 2020 2050 4152   in S0B).    PAR
+00003080: 414d 4554 4552 533a 0a20 2020 202d 2d2d  AMETERS:.    ---
 00003090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000030a0: 2d2d 2d0a 2020 2020 7374 6174 733a 206f  ---.    stats: o
-000030b0: 6273 7079 2074 7261 6365 2073 7461 7473  bspy trace stats
-000030c0: 206f 626a 6563 7420 636f 6e74 6169 6e69   object containi
-000030d0: 6e67 2061 6c6c 2073 7461 7469 6f6e 2068  ng all station h
-000030e0: 6561 6465 7220 696e 666f 0a20 2020 2070  eader info.    p
-000030f0: 7265 7072 6f5f 7061 7261 3a20 6469 6374  repro_para: dict
-00003100: 2063 6f6e 7461 696e 696e 6720 6666 7420   containing fft 
-00003110: 7061 7261 6d65 7465 7273 2c20 7375 6368  parameters, such
-00003120: 2061 7320 6672 6571 7565 6e63 7920 6261   as frequency ba
-00003130: 6e64 7320 616e 6420 7365 6c65 6374 696f  nds and selectio
-00003140: 6e20 666f 7220 696e 7374 7275 6d65 6e74  n for instrument
-00003150: 0a20 2020 2072 6573 706f 6e73 6520 7265  .    response re
-00003160: 6d6f 7661 6c20 6574 632e 0a20 2020 206c  moval etc..    l
-00003170: 6f63 733a 2020 7061 6e64 6120 6461 7461  ocs:  panda data
-00003180: 2066 7261 6d65 206f 6620 7468 6520 7374   frame of the st
-00003190: 6174 696f 6e20 6c69 7374 2e20 6974 2069  ation list. it i
-000031a0: 7320 6e65 6564 6564 2066 6f72 2063 6f6e  s needed for con
-000031b0: 7665 7269 6e67 206d 696e 6973 6565 6420  vering miniseed 
-000031c0: 6669 6c65 7320 696e 746f 2041 5344 460a  files into ASDF.
-000031d0: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
-000031e0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-000031f0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 696e  ---------.    in
-00003200: 763a 206f 6273 7079 2069 6e76 656e 746f  v: obspy invento
-00003210: 7279 206f 626a 6563 7420 6f66 2061 6c6c  ry object of all
-00003220: 2073 7461 7469 6f6e 2069 6e66 6f20 746f   station info to
-00003230: 2062 6520 7573 6564 206c 6174 6572 0a20   be used later. 
-00003240: 2020 2022 2222 0a20 2020 2073 7461 786d     """.    staxm
-00003250: 6c20 3d20 7072 6570 726f 5f70 6172 615b  l = prepro_para[
-00003260: 2273 7461 7469 6f6e 786d 6c22 5d0a 2020  "stationxml"].  
-00003270: 2020 7265 7370 6469 7220 3d20 7072 6570    respdir = prep
-00003280: 726f 5f70 6172 615b 2272 6573 7064 6972  ro_para["respdir
-00003290: 225d 0a20 2020 2069 6e70 7574 5f66 6d74  "].    input_fmt
-000032a0: 203d 2070 7265 7072 6f5f 7061 7261 5b22   = prepro_para["
-000032b0: 696e 7075 745f 666d 7422 5d0a 2020 2020  input_fmt"].    
-000032c0: 6966 2073 7461 786d 6c3a 0a20 2020 2020  if staxml:.     
-000032d0: 2020 2072 6574 7572 6e20 7374 6174 7332     return stats2
-000032e0: 496e 765f 7374 6178 6d6c 2873 7461 7473  Inv_staxml(stats
-000032f0: 2c20 7265 7370 6469 7229 0a20 2020 2069  , respdir).    i
-00003300: 6620 696e 7075 745f 666d 7420 3d3d 2022  f input_fmt == "
-00003310: 7361 6322 3a0a 2020 2020 2020 2020 7265  sac":.        re
-00003320: 7475 726e 2073 7461 7473 3269 6e76 5f73  turn stats2inv_s
-00003330: 6163 2873 7461 7473 290a 2020 2020 656c  ac(stats).    el
-00003340: 6966 2069 6e70 7574 5f66 6d74 203d 3d20  if input_fmt == 
-00003350: 226d 7365 6564 223a 0a20 2020 2020 2020  "mseed":.       
-00003360: 2072 6574 7572 6e20 7374 6174 7332 696e   return stats2in
-00003370: 765f 6d73 6565 6428 7374 6174 732c 206c  v_mseed(stats, l
-00003380: 6f63 7329 0a0a 0a64 6566 2073 7461 7473  ocs)...def stats
-00003390: 3249 6e76 5f73 7461 786d 6c28 7374 6174  2Inv_staxml(stat
-000033a0: 732c 2072 6573 7064 6972 2920 2d3e 2049  s, respdir) -> I
-000033b0: 6e76 656e 746f 7279 3a0a 2020 2020 6966  nventory:.    if
-000033c0: 206e 6f74 2072 6573 7064 6972 3a0a 2020   not respdir:.  
-000033d0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-000033e0: 6545 7272 6f72 2822 4162 6f72 7421 2073  eError("Abort! s
-000033f0: 7461 786d 6c20 6973 2073 656c 6563 7465  taxml is selecte
-00003400: 6420 6275 7420 6e6f 2064 6972 6563 746f  d but no directo
-00003410: 7279 2069 7320 6769 7665 6e20 746f 2061  ry is given to a
-00003420: 6363 6573 7320 7468 6520 6669 6c65 7322  ccess the files"
-00003430: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-00003440: 2020 2020 696e 7666 696c 656c 6973 7420      invfilelist 
-00003450: 3d20 676c 6f62 2e67 6c6f 6228 6f73 2e70  = glob.glob(os.p
-00003460: 6174 682e 6a6f 696e 2872 6573 7064 6972  ath.join(respdir
-00003470: 2c20 222a 2220 2b20 7374 6174 732e 7374  , "*" + stats.st
-00003480: 6174 696f 6e20 2b20 222a 2229 290a 2020  ation + "*")).  
-00003490: 2020 2020 2020 6966 206c 656e 2869 6e76        if len(inv
-000034a0: 6669 6c65 6c69 7374 2920 3e20 303a 0a20  filelist) > 0:. 
-000034b0: 2020 2020 2020 2020 2020 2069 6e76 6669             invfi
-000034c0: 6c65 203d 2069 6e76 6669 6c65 6c69 7374  le = invfilelist
-000034d0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
-000034e0: 6966 206c 656e 2869 6e76 6669 6c65 6c69  if len(invfileli
-000034f0: 7374 2920 3e20 313a 0a20 2020 2020 2020  st) > 1:.       
-00003500: 2020 2020 2020 2020 2070 7269 6e74 280a           print(.
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
-00003530: 2020 2020 2020 2020 2020 2020 2020 2257                "W
-00003540: 6172 6e69 6e67 2120 4d6f 7265 2074 6861  arning! More tha
-00003550: 6e20 6f6e 6520 5374 6174 696f 6e58 4d4c  n one StationXML
-00003560: 2066 696c 6520 7761 7320 666f 756e 6420   file was found 
-00003570: 666f 7220 7374 6174 696f 6e20 2573 2e22  for station %s."
-00003580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003590: 2020 2020 2020 2020 202b 2022 4b65 6570           + "Keep
-000035a0: 696e 6720 7468 6520 6669 7273 7420 6669  ing the first fi
-000035b0: 6c65 2069 6e20 6c69 7374 2e22 0a20 2020  le in list.".   
+000030a0: 2d2d 2d2d 2d0a 2020 2020 7374 6174 733a  -----.    stats:
+000030b0: 206f 6273 7079 2074 7261 6365 2073 7461   obspy trace sta
+000030c0: 7473 206f 626a 6563 7420 636f 6e74 6169  ts object contai
+000030d0: 6e69 6e67 2061 6c6c 2073 7461 7469 6f6e  ning all station
+000030e0: 2068 6561 6465 7220 696e 666f 0a20 2020   header info.   
+000030f0: 2070 7265 7072 6f5f 7061 7261 3a20 6469   prepro_para: di
+00003100: 6374 2063 6f6e 7461 696e 696e 6720 6666  ct containing ff
+00003110: 7420 7061 7261 6d65 7465 7273 2c20 7375  t parameters, su
+00003120: 6368 2061 7320 6672 6571 7565 6e63 7920  ch as frequency 
+00003130: 6261 6e64 7320 616e 6420 7365 6c65 6374  bands and select
+00003140: 696f 6e20 666f 7220 696e 7374 7275 6d65  ion for instrume
+00003150: 6e74 0a20 2020 2072 6573 706f 6e73 6520  nt.    response 
+00003160: 7265 6d6f 7661 6c20 6574 632e 0a20 2020  removal etc..   
+00003170: 206c 6f63 733a 2020 7061 6e64 6120 6461   locs:  panda da
+00003180: 7461 2066 7261 6d65 206f 6620 7468 6520  ta frame of the 
+00003190: 7374 6174 696f 6e20 6c69 7374 2e20 6974  station list. it
+000031a0: 2069 7320 6e65 6564 6564 2066 6f72 2063   is needed for c
+000031b0: 6f6e 7665 7269 6e67 206d 696e 6973 6565  onvering minisee
+000031c0: 6420 6669 6c65 7320 696e 746f 2041 5344  d files into ASD
+000031d0: 460a 2020 2020 5245 5455 524e 533a 0a20  F.    RETURNS:. 
+000031e0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+000031f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00003200: 696e 763a 206f 6273 7079 2069 6e76 656e  inv: obspy inven
+00003210: 746f 7279 206f 626a 6563 7420 6f66 2061  tory object of a
+00003220: 6c6c 2073 7461 7469 6f6e 2069 6e66 6f20  ll station info 
+00003230: 746f 2062 6520 7573 6564 206c 6174 6572  to be used later
+00003240: 0a20 2020 2022 2222 0a20 2020 2073 7461  .    """.    sta
+00003250: 786d 6c20 3d20 7072 6570 726f 5f70 6172  xml = prepro_par
+00003260: 615b 2273 7461 7469 6f6e 786d 6c22 5d0a  a["stationxml"].
+00003270: 2020 2020 7265 7370 6469 7220 3d20 7072      respdir = pr
+00003280: 6570 726f 5f70 6172 615b 2272 6573 7064  epro_para["respd
+00003290: 6972 225d 0a20 2020 2069 6e70 7574 5f66  ir"].    input_f
+000032a0: 6d74 203d 2070 7265 7072 6f5f 7061 7261  mt = prepro_para
+000032b0: 5b22 696e 7075 745f 666d 7422 5d0a 2020  ["input_fmt"].  
+000032c0: 2020 6966 2073 7461 786d 6c3a 0a20 2020    if staxml:.   
+000032d0: 2020 2020 2072 6574 7572 6e20 7374 6174       return stat
+000032e0: 7332 496e 765f 7374 6178 6d6c 2873 7461  s2Inv_staxml(sta
+000032f0: 7473 2c20 7265 7370 6469 7229 0a20 2020  ts, respdir).   
+00003300: 2069 6620 696e 7075 745f 666d 7420 3d3d   if input_fmt ==
+00003310: 2022 7361 6322 3a0a 2020 2020 2020 2020   "sac":.        
+00003320: 7265 7475 726e 2073 7461 7473 3269 6e76  return stats2inv
+00003330: 5f73 6163 2873 7461 7473 290a 2020 2020  _sac(stats).    
+00003340: 656c 6966 2069 6e70 7574 5f66 6d74 203d  elif input_fmt =
+00003350: 3d20 226d 7365 6564 223a 0a20 2020 2020  = "mseed":.     
+00003360: 2020 2072 6574 7572 6e20 7374 6174 7332     return stats2
+00003370: 696e 765f 6d73 6565 6428 7374 6174 732c  inv_mseed(stats,
+00003380: 206c 6f63 7329 0a0a 0a64 6566 2073 7461   locs)...def sta
+00003390: 7473 3249 6e76 5f73 7461 786d 6c28 7374  ts2Inv_staxml(st
+000033a0: 6174 732c 2072 6573 7064 6972 2920 2d3e  ats, respdir) ->
+000033b0: 2049 6e76 656e 746f 7279 3a0a 2020 2020   Inventory:.    
+000033c0: 6966 206e 6f74 2072 6573 7064 6972 3a0a  if not respdir:.
+000033d0: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+000033e0: 6c75 6545 7272 6f72 2822 4162 6f72 7421  lueError("Abort!
+000033f0: 2073 7461 786d 6c20 6973 2073 656c 6563   staxml is selec
+00003400: 7465 6420 6275 7420 6e6f 2064 6972 6563  ted but no direc
+00003410: 746f 7279 2069 7320 6769 7665 6e20 746f  tory is given to
+00003420: 2061 6363 6573 7320 7468 6520 6669 6c65   access the file
+00003430: 7322 290a 2020 2020 656c 7365 3a0a 2020  s").    else:.  
+00003440: 2020 2020 2020 696e 7666 696c 656c 6973        invfilelis
+00003450: 7420 3d20 676c 6f62 2e67 6c6f 6228 6f73  t = glob.glob(os
+00003460: 2e70 6174 682e 6a6f 696e 2872 6573 7064  .path.join(respd
+00003470: 6972 2c20 222a 2220 2b20 7374 6174 732e  ir, "*" + stats.
+00003480: 7374 6174 696f 6e20 2b20 222a 2229 290a  station + "*")).
+00003490: 2020 2020 2020 2020 6966 206c 656e 2869          if len(i
+000034a0: 6e76 6669 6c65 6c69 7374 2920 3e20 303a  nvfilelist) > 0:
+000034b0: 0a20 2020 2020 2020 2020 2020 2069 6e76  .            inv
+000034c0: 6669 6c65 203d 2069 6e76 6669 6c65 6c69  file = invfileli
+000034d0: 7374 5b30 5d0a 2020 2020 2020 2020 2020  st[0].          
+000034e0: 2020 6966 206c 656e 2869 6e76 6669 6c65    if len(invfile
+000034f0: 6c69 7374 2920 3e20 313a 0a20 2020 2020  list) > 1:.     
+00003500: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00003510: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00003520: 2020 2020 2020 280a 2020 2020 2020 2020        (.        
+00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003540: 2257 6172 6e69 6e67 2120 4d6f 7265 2074  "Warning! More t
+00003550: 6861 6e20 6f6e 6520 5374 6174 696f 6e58  han one StationX
+00003560: 4d4c 2066 696c 6520 7761 7320 666f 756e  ML file was foun
+00003570: 6420 666f 7220 7374 6174 696f 6e20 2573  d for station %s
+00003580: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
+00003590: 2020 2020 2020 2020 2020 202b 2022 4b65             + "Ke
+000035a0: 6570 696e 6720 7468 6520 6669 7273 7420  eping the first 
+000035b0: 6669 6c65 2069 6e20 6c69 7374 2e22 0a20  file in list.". 
 000035c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035d0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-000035e0: 2020 2020 2020 2025 2073 7461 7473 2e73         % stats.s
-000035f0: 7461 7469 6f6e 0a20 2020 2020 2020 2020  tation.         
-00003600: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00003610: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
-00003620: 6973 6669 6c65 2873 7472 2869 6e76 6669  isfile(str(invfi
-00003630: 6c65 2929 3a0a 2020 2020 2020 2020 2020  le)):.          
-00003640: 2020 2020 2020 696e 7620 3d20 6f62 7370        inv = obsp
-00003650: 792e 7265 6164 5f69 6e76 656e 746f 7279  y.read_inventory
-00003660: 2869 6e76 6669 6c65 290a 2020 2020 2020  (invfile).      
-00003670: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00003680: 2069 6e76 0a20 2020 2020 2020 2065 6c73   inv.        els
-00003690: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000036a0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-000036b0: 2243 6f75 6c64 206e 6f74 2066 696e 6420  "Could not find 
-000036c0: 6120 5374 6174 696f 6e58 4d4c 2066 696c  a StationXML fil
-000036d0: 6520 666f 7220 7374 6174 696f 6e3a 2025  e for station: %
-000036e0: 732e 2220 2520 7374 6174 732e 7374 6174  s." % stats.stat
-000036f0: 696f 6e29 0a0a 0a64 6566 2073 7461 7473  ion)...def stats
-00003700: 3269 6e76 5f73 6163 2873 7461 7473 293a  2inv_sac(stats):
-00003710: 0a20 2020 2069 6e76 203d 2049 6e76 656e  .    inv = Inven
-00003720: 746f 7279 286e 6574 776f 726b 733d 5b5d  tory(networks=[]
-00003730: 2c20 736f 7572 6365 3d22 686f 6d65 6772  , source="homegr
-00003740: 6f77 6e22 290a 2020 2020 6e65 7420 3d20  own").    net = 
-00003750: 4e65 7477 6f72 6b28 0a20 2020 2020 2020  Network(.       
-00003760: 2023 2054 6869 7320 6973 2074 6865 206e   # This is the n
-00003770: 6574 776f 726b 2063 6f64 6520 6163 636f  etwork code acco
-00003780: 7264 696e 6720 746f 2074 6865 2053 4545  rding to the SEE
-00003790: 4420 7374 616e 6461 7264 2e0a 2020 2020  D standard..    
-000037a0: 2020 2020 636f 6465 3d73 7461 7473 2e6e      code=stats.n
-000037b0: 6574 776f 726b 2c0a 2020 2020 2020 2020  etwork,.        
-000037c0: 7374 6174 696f 6e73 3d5b 5d2c 0a20 2020  stations=[],.   
-000037d0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-000037e0: 3d22 6372 6561 7465 6420 6672 6f6d 2053  ="created from S
-000037f0: 4143 2061 6e64 2072 6573 7020 6669 6c65  AC and resp file
-00003800: 7322 2c0a 2020 2020 2020 2020 7374 6172  s",.        star
-00003810: 745f 6461 7465 3d73 7461 7473 2e73 7461  t_date=stats.sta
-00003820: 7274 7469 6d65 2c0a 2020 2020 290a 0a20  rttime,.    ).. 
-00003830: 2020 2073 7461 203d 2053 7461 7469 6f6e     sta = Station
-00003840: 280a 2020 2020 2020 2020 2320 5468 6973  (.        # This
-00003850: 2069 7320 7468 6520 7374 6174 696f 6e20   is the station 
-00003860: 636f 6465 2061 6363 6f72 6469 6e67 2074  code according t
-00003870: 6f20 7468 6520 5345 4544 2073 7461 6e64  o the SEED stand
-00003880: 6172 642e 0a20 2020 2020 2020 2063 6f64  ard..        cod
-00003890: 653d 7374 6174 732e 7374 6174 696f 6e2c  e=stats.station,
-000038a0: 0a20 2020 2020 2020 206c 6174 6974 7564  .        latitud
-000038b0: 653d 7374 6174 732e 7361 635b 2273 746c  e=stats.sac["stl
-000038c0: 6122 5d2c 0a20 2020 2020 2020 206c 6f6e  a"],.        lon
-000038d0: 6769 7475 6465 3d73 7461 7473 2e73 6163  gitude=stats.sac
-000038e0: 5b22 7374 6c6f 225d 2c0a 2020 2020 2020  ["stlo"],.      
-000038f0: 2020 656c 6576 6174 696f 6e3d 7374 6174    elevation=stat
-00003900: 732e 7361 635b 2273 7465 6c22 5d2c 0a20  s.sac["stel"],. 
-00003910: 2020 2020 2020 2063 7265 6174 696f 6e5f         creation_
-00003920: 6461 7465 3d73 7461 7473 2e73 7461 7274  date=stats.start
-00003930: 7469 6d65 2c0a 2020 2020 2020 2020 7369  time,.        si
-00003940: 7465 3d53 6974 6528 6e61 6d65 3d22 4669  te=Site(name="Fi
-00003950: 7273 7420 7374 6174 696f 6e22 292c 0a20  rst station"),. 
-00003960: 2020 2029 0a0a 2020 2020 6368 6120 3d20     )..    cha = 
-00003970: 4368 616e 6e65 6c28 0a20 2020 2020 2020  Channel(.       
-00003980: 2023 2054 6869 7320 6973 2074 6865 2063   # This is the c
-00003990: 6861 6e6e 656c 2063 6f64 6520 6163 636f  hannel code acco
-000039a0: 7264 696e 6720 746f 2074 6865 2053 4545  rding to the SEE
-000039b0: 4420 7374 616e 6461 7264 2e0a 2020 2020  D standard..    
-000039c0: 2020 2020 636f 6465 3d73 7461 7473 2e63      code=stats.c
-000039d0: 6861 6e6e 656c 2c0a 2020 2020 2020 2020  hannel,.        
-000039e0: 2320 5468 6973 2069 7320 7468 6520 6c6f  # This is the lo
-000039f0: 6361 7469 6f6e 2063 6f64 6520 6163 636f  cation code acco
-00003a00: 7264 696e 6720 746f 2074 6865 2053 4545  rding to the SEE
-00003a10: 4420 7374 616e 6461 7264 2e0a 2020 2020  D standard..    
-00003a20: 2020 2020 6c6f 6361 7469 6f6e 5f63 6f64      location_cod
-00003a30: 653d 7374 6174 732e 6c6f 6361 7469 6f6e  e=stats.location
-00003a40: 2c0a 2020 2020 2020 2020 2320 4e6f 7465  ,.        # Note
-00003a50: 2074 6861 7420 7468 6573 6520 636f 6f72   that these coor
-00003a60: 6469 6e61 7465 7320 6361 6e20 6469 6666  dinates can diff
-00003a70: 6572 2066 726f 6d20 7468 6520 7374 6174  er from the stat
-00003a80: 696f 6e20 636f 6f72 6469 6e61 7465 732e  ion coordinates.
-00003a90: 0a20 2020 2020 2020 206c 6174 6974 7564  .        latitud
-00003aa0: 653d 7374 6174 732e 7361 635b 2273 746c  e=stats.sac["stl
-00003ab0: 6122 5d2c 0a20 2020 2020 2020 206c 6f6e  a"],.        lon
-00003ac0: 6769 7475 6465 3d73 7461 7473 2e73 6163  gitude=stats.sac
-00003ad0: 5b22 7374 6c6f 225d 2c0a 2020 2020 2020  ["stlo"],.      
-00003ae0: 2020 656c 6576 6174 696f 6e3d 7374 6174    elevation=stat
-00003af0: 732e 7361 635b 2273 7465 6c22 5d2c 0a20  s.sac["stel"],. 
-00003b00: 2020 2020 2020 2064 6570 7468 3d2d 7374         depth=-st
-00003b10: 6174 732e 7361 635b 2273 7465 6c22 5d2c  ats.sac["stel"],
-00003b20: 0a20 2020 2020 2020 2061 7a69 6d75 7468  .        azimuth
-00003b30: 3d73 7461 7473 2e73 6163 5b22 636d 7061  =stats.sac["cmpa
-00003b40: 7a22 5d2c 0a20 2020 2020 2020 2064 6970  z"],.        dip
-00003b50: 3d73 7461 7473 2e73 6163 5b22 636d 7069  =stats.sac["cmpi
-00003b60: 6e63 225d 2c0a 2020 2020 2020 2020 7361  nc"],.        sa
-00003b70: 6d70 6c65 5f72 6174 653d 7374 6174 732e  mple_rate=stats.
-00003b80: 7361 6d70 6c69 6e67 5f72 6174 652c 0a20  sampling_rate,. 
-00003b90: 2020 2029 0a20 2020 2072 6573 706f 6e73     ).    respons
-00003ba0: 6520 3d20 6f62 7370 792e 636f 7265 2e69  e = obspy.core.i
-00003bb0: 6e76 656e 746f 7279 2e72 6573 706f 6e73  nventory.respons
-00003bc0: 652e 5265 7370 6f6e 7365 2829 0a0a 2020  e.Response()..  
-00003bd0: 2020 2320 4e6f 7720 7469 6520 6974 2061    # Now tie it a
-00003be0: 6c6c 2074 6f67 6574 6865 722e 0a20 2020  ll together..   
-00003bf0: 2063 6861 2e72 6573 706f 6e73 6520 3d20   cha.response = 
-00003c00: 7265 7370 6f6e 7365 0a20 2020 2073 7461  response.    sta
-00003c10: 2e63 6861 6e6e 656c 732e 6170 7065 6e64  .channels.append
-00003c20: 2863 6861 290a 2020 2020 6e65 742e 7374  (cha).    net.st
-00003c30: 6174 696f 6e73 2e61 7070 656e 6428 7374  ations.append(st
-00003c40: 6129 0a20 2020 2069 6e76 2e6e 6574 776f  a).    inv.netwo
-00003c50: 726b 732e 6170 7065 6e64 286e 6574 290a  rks.append(net).
-00003c60: 0a20 2020 2072 6574 7572 6e20 696e 760a  .    return inv.
-00003c70: 0a0a 6465 6620 7374 6174 7332 696e 765f  ..def stats2inv_
-00003c80: 6d73 6565 6428 7374 6174 732c 206c 6f63  mseed(stats, loc
-00003c90: 733a 2070 642e 4461 7461 4672 616d 6529  s: pd.DataFrame)
-00003ca0: 202d 3e20 496e 7665 6e74 6f72 793a 0a20   -> Inventory:. 
-00003cb0: 2020 2069 6e76 203d 2049 6e76 656e 746f     inv = Invento
-00003cc0: 7279 286e 6574 776f 726b 733d 5b5d 2c20  ry(networks=[], 
-00003cd0: 736f 7572 6365 3d22 686f 6d65 6772 6f77  source="homegrow
-00003ce0: 6e22 290a 2020 2020 6973 7461 203d 206c  n").    ista = l
-00003cf0: 6f63 735b 6c6f 6373 5b22 7374 6174 696f  ocs[locs["statio
-00003d00: 6e22 5d20 3d3d 2073 7461 7473 2e73 7461  n"] == stats.sta
-00003d10: 7469 6f6e 5d2e 696e 6465 782e 7661 6c75  tion].index.valu
-00003d20: 6573 2e61 7374 7970 6528 2269 6e74 3634  es.astype("int64
-00003d30: 2229 5b30 5d0a 0a20 2020 206e 6574 203d  ")[0]..    net =
-00003d40: 204e 6574 776f 726b 280a 2020 2020 2020   Network(.      
-00003d50: 2020 2320 5468 6973 2069 7320 7468 6520    # This is the 
-00003d60: 6e65 7477 6f72 6b20 636f 6465 2061 6363  network code acc
-00003d70: 6f72 6469 6e67 2074 6f20 7468 6520 5345  ording to the SE
-00003d80: 4544 2073 7461 6e64 6172 642e 0a20 2020  ED standard..   
-00003d90: 2020 2020 2063 6f64 653d 6c6f 6373 2e69       code=locs.i
-00003da0: 6c6f 635b 6973 7461 5d5b 226e 6574 776f  loc[ista]["netwo
-00003db0: 726b 225d 2c0a 2020 2020 2020 2020 7374  rk"],.        st
-00003dc0: 6174 696f 6e73 3d5b 5d2c 0a20 2020 2020  ations=[],.     
-00003dd0: 2020 2064 6573 6372 6970 7469 6f6e 3d22     description="
-00003de0: 6372 6561 7465 6420 6672 6f6d 2053 4143  created from SAC
-00003df0: 2061 6e64 2072 6573 7020 6669 6c65 7322   and resp files"
-00003e00: 2c0a 2020 2020 2020 2020 7374 6172 745f  ,.        start_
-00003e10: 6461 7465 3d73 7461 7473 2e73 7461 7274  date=stats.start
-00003e20: 7469 6d65 2c0a 2020 2020 290a 0a20 2020  time,.    )..   
-00003e30: 2073 7461 203d 2053 7461 7469 6f6e 280a   sta = Station(.
-00003e40: 2020 2020 2020 2020 2320 5468 6973 2069          # This i
-00003e50: 7320 7468 6520 7374 6174 696f 6e20 636f  s the station co
-00003e60: 6465 2061 6363 6f72 6469 6e67 2074 6f20  de according to 
-00003e70: 7468 6520 5345 4544 2073 7461 6e64 6172  the SEED standar
-00003e80: 642e 0a20 2020 2020 2020 2063 6f64 653d  d..        code=
-00003e90: 6c6f 6373 2e69 6c6f 635b 6973 7461 5d5b  locs.iloc[ista][
-00003ea0: 2273 7461 7469 6f6e 225d 2c0a 2020 2020  "station"],.    
-00003eb0: 2020 2020 6c61 7469 7475 6465 3d6c 6f63      latitude=loc
-00003ec0: 732e 696c 6f63 5b69 7374 615d 5b22 6c61  s.iloc[ista]["la
-00003ed0: 7469 7475 6465 225d 2c0a 2020 2020 2020  titude"],.      
-00003ee0: 2020 6c6f 6e67 6974 7564 653d 6c6f 6373    longitude=locs
-00003ef0: 2e69 6c6f 635b 6973 7461 5d5b 226c 6f6e  .iloc[ista]["lon
-00003f00: 6769 7475 6465 225d 2c0a 2020 2020 2020  gitude"],.      
-00003f10: 2020 656c 6576 6174 696f 6e3d 6c6f 6373    elevation=locs
-00003f20: 2e69 6c6f 635b 6973 7461 5d5b 2265 6c65  .iloc[ista]["ele
-00003f30: 7661 7469 6f6e 225d 2c0a 2020 2020 2020  vation"],.      
-00003f40: 2020 6372 6561 7469 6f6e 5f64 6174 653d    creation_date=
-00003f50: 7374 6174 732e 7374 6172 7474 696d 652c  stats.starttime,
-00003f60: 0a20 2020 2020 2020 2073 6974 653d 5369  .        site=Si
-00003f70: 7465 286e 616d 653d 2246 6972 7374 2073  te(name="First s
-00003f80: 7461 7469 6f6e 2229 2c0a 2020 2020 290a  tation"),.    ).
-00003f90: 0a20 2020 2063 6861 203d 2043 6861 6e6e  .    cha = Chann
-00003fa0: 656c 280a 2020 2020 2020 2020 636f 6465  el(.        code
-00003fb0: 3d73 7461 7473 2e63 6861 6e6e 656c 2c0a  =stats.channel,.
-00003fc0: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
-00003fd0: 5f63 6f64 653d 7374 6174 732e 6c6f 6361  _code=stats.loca
-00003fe0: 7469 6f6e 2c0a 2020 2020 2020 2020 6c61  tion,.        la
-00003ff0: 7469 7475 6465 3d6c 6f63 732e 696c 6f63  titude=locs.iloc
-00004000: 5b69 7374 615d 5b22 6c61 7469 7475 6465  [ista]["latitude
-00004010: 225d 2c0a 2020 2020 2020 2020 6c6f 6e67  "],.        long
-00004020: 6974 7564 653d 6c6f 6373 2e69 6c6f 635b  itude=locs.iloc[
-00004030: 6973 7461 5d5b 226c 6f6e 6769 7475 6465  ista]["longitude
-00004040: 225d 2c0a 2020 2020 2020 2020 656c 6576  "],.        elev
-00004050: 6174 696f 6e3d 6c6f 6373 2e69 6c6f 635b  ation=locs.iloc[
-00004060: 6973 7461 5d5b 2265 6c65 7661 7469 6f6e  ista]["elevation
-00004070: 225d 2c0a 2020 2020 2020 2020 6465 7074  "],.        dept
-00004080: 683d 2d6c 6f63 732e 696c 6f63 5b69 7374  h=-locs.iloc[ist
-00004090: 615d 5b22 656c 6576 6174 696f 6e22 5d2c  a]["elevation"],
-000040a0: 0a20 2020 2020 2020 2061 7a69 6d75 7468  .        azimuth
-000040b0: 3d30 2c0a 2020 2020 2020 2020 6469 703d  =0,.        dip=
-000040c0: 302c 0a20 2020 2020 2020 2073 616d 706c  0,.        sampl
-000040d0: 655f 7261 7465 3d73 7461 7473 2e73 616d  e_rate=stats.sam
-000040e0: 706c 696e 675f 7261 7465 2c0a 2020 2020  pling_rate,.    
-000040f0: 290a 0a20 2020 2072 6573 706f 6e73 6520  )..    response 
-00004100: 3d20 6f62 7370 792e 636f 7265 2e69 6e76  = obspy.core.inv
-00004110: 656e 746f 7279 2e72 6573 706f 6e73 652e  entory.response.
-00004120: 5265 7370 6f6e 7365 2829 0a0a 2020 2020  Response()..    
-00004130: 2320 4e6f 7720 7469 6520 6974 2061 6c6c  # Now tie it all
-00004140: 2074 6f67 6574 6865 722e 0a20 2020 2063   together..    c
-00004150: 6861 2e72 6573 706f 6e73 6520 3d20 7265  ha.response = re
-00004160: 7370 6f6e 7365 0a20 2020 2073 7461 2e63  sponse.    sta.c
-00004170: 6861 6e6e 656c 732e 6170 7065 6e64 2863  hannels.append(c
-00004180: 6861 290a 2020 2020 6e65 742e 7374 6174  ha).    net.stat
-00004190: 696f 6e73 2e61 7070 656e 6428 7374 6129  ions.append(sta)
-000041a0: 0a20 2020 2069 6e76 2e6e 6574 776f 726b  .    inv.network
-000041b0: 732e 6170 7065 6e64 286e 6574 290a 0a20  s.append(net).. 
-000041c0: 2020 2072 6574 7572 6e20 696e 760a 0a0a     return inv...
-000041d0: 6465 6620 7374 615f 696e 666f 5f66 726f  def sta_info_fro
-000041e0: 6d5f 696e 7628 696e 763a 206f 6273 7079  m_inv(inv: obspy
-000041f0: 2e63 6f72 652e 696e 7665 6e74 6f72 792e  .core.inventory.
-00004200: 696e 7665 6e74 6f72 792e 496e 7665 6e74  inventory.Invent
-00004210: 6f72 7929 3a0a 2020 2020 2222 220a 2020  ory):.    """.  
-00004220: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
-00004230: 6f75 7470 7574 7320 7374 6174 696f 6e20  outputs station 
-00004240: 696e 666f 2066 726f 6d20 7468 6520 6f62  info from the ob
-00004250: 7370 7920 696e 7665 6e74 6f72 7920 6f62  spy inventory ob
-00004260: 6a65 6374 0a20 2020 2028 7573 6564 2069  ject.    (used i
-00004270: 6e20 5330 4229 0a20 2020 2050 4152 414d  n S0B).    PARAM
-00004280: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
+000035d0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000035e0: 2020 2020 2020 2020 2025 2073 7461 7473           % stats
+000035f0: 2e73 7461 7469 6f6e 0a20 2020 2020 2020  .station.       
+00003600: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00003610: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
+00003620: 682e 6973 6669 6c65 2873 7472 2869 6e76  h.isfile(str(inv
+00003630: 6669 6c65 2929 3a0a 2020 2020 2020 2020  file)):.        
+00003640: 2020 2020 2020 2020 696e 7620 3d20 6f62          inv = ob
+00003650: 7370 792e 7265 6164 5f69 6e76 656e 746f  spy.read_invento
+00003660: 7279 2869 6e76 6669 6c65 290a 2020 2020  ry(invfile).    
+00003670: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00003680: 726e 2069 6e76 0a20 2020 2020 2020 2065  rn inv.        e
+00003690: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000036a0: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+000036b0: 7228 2243 6f75 6c64 206e 6f74 2066 696e  r("Could not fin
+000036c0: 6420 6120 5374 6174 696f 6e58 4d4c 2066  d a StationXML f
+000036d0: 696c 6520 666f 7220 7374 6174 696f 6e3a  ile for station:
+000036e0: 2025 732e 2220 2520 7374 6174 732e 7374   %s." % stats.st
+000036f0: 6174 696f 6e29 0a0a 0a64 6566 2073 7461  ation)...def sta
+00003700: 7473 3269 6e76 5f73 6163 2873 7461 7473  ts2inv_sac(stats
+00003710: 293a 0a20 2020 2069 6e76 203d 2049 6e76  ):.    inv = Inv
+00003720: 656e 746f 7279 286e 6574 776f 726b 733d  entory(networks=
+00003730: 5b5d 2c20 736f 7572 6365 3d22 686f 6d65  [], source="home
+00003740: 6772 6f77 6e22 290a 2020 2020 6e65 7420  grown").    net 
+00003750: 3d20 4e65 7477 6f72 6b28 0a20 2020 2020  = Network(.     
+00003760: 2020 2023 2054 6869 7320 6973 2074 6865     # This is the
+00003770: 206e 6574 776f 726b 2063 6f64 6520 6163   network code ac
+00003780: 636f 7264 696e 6720 746f 2074 6865 2053  cording to the S
+00003790: 4545 4420 7374 616e 6461 7264 2e0a 2020  EED standard..  
+000037a0: 2020 2020 2020 636f 6465 3d73 7461 7473        code=stats
+000037b0: 2e6e 6574 776f 726b 2c0a 2020 2020 2020  .network,.      
+000037c0: 2020 7374 6174 696f 6e73 3d5b 5d2c 0a20    stations=[],. 
+000037d0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+000037e0: 6f6e 3d22 6372 6561 7465 6420 6672 6f6d  on="created from
+000037f0: 2053 4143 2061 6e64 2072 6573 7020 6669   SAC and resp fi
+00003800: 6c65 7322 2c0a 2020 2020 2020 2020 7374  les",.        st
+00003810: 6172 745f 6461 7465 3d73 7461 7473 2e73  art_date=stats.s
+00003820: 7461 7274 7469 6d65 2c0a 2020 2020 290a  tarttime,.    ).
+00003830: 0a20 2020 2073 7461 203d 2053 7461 7469  .    sta = Stati
+00003840: 6f6e 280a 2020 2020 2020 2020 2320 5468  on(.        # Th
+00003850: 6973 2069 7320 7468 6520 7374 6174 696f  is is the statio
+00003860: 6e20 636f 6465 2061 6363 6f72 6469 6e67  n code according
+00003870: 2074 6f20 7468 6520 5345 4544 2073 7461   to the SEED sta
+00003880: 6e64 6172 642e 0a20 2020 2020 2020 2063  ndard..        c
+00003890: 6f64 653d 7374 6174 732e 7374 6174 696f  ode=stats.statio
+000038a0: 6e2c 0a20 2020 2020 2020 206c 6174 6974  n,.        latit
+000038b0: 7564 653d 7374 6174 732e 7361 635b 2273  ude=stats.sac["s
+000038c0: 746c 6122 5d2c 0a20 2020 2020 2020 206c  tla"],.        l
+000038d0: 6f6e 6769 7475 6465 3d73 7461 7473 2e73  ongitude=stats.s
+000038e0: 6163 5b22 7374 6c6f 225d 2c0a 2020 2020  ac["stlo"],.    
+000038f0: 2020 2020 656c 6576 6174 696f 6e3d 7374      elevation=st
+00003900: 6174 732e 7361 635b 2273 7465 6c22 5d2c  ats.sac["stel"],
+00003910: 0a20 2020 2020 2020 2063 7265 6174 696f  .        creatio
+00003920: 6e5f 6461 7465 3d73 7461 7473 2e73 7461  n_date=stats.sta
+00003930: 7274 7469 6d65 2c0a 2020 2020 2020 2020  rttime,.        
+00003940: 7369 7465 3d53 6974 6528 6e61 6d65 3d22  site=Site(name="
+00003950: 4669 7273 7420 7374 6174 696f 6e22 292c  First station"),
+00003960: 0a20 2020 2029 0a0a 2020 2020 6368 6120  .    )..    cha 
+00003970: 3d20 4368 616e 6e65 6c28 0a20 2020 2020  = Channel(.     
+00003980: 2020 2023 2054 6869 7320 6973 2074 6865     # This is the
+00003990: 2063 6861 6e6e 656c 2063 6f64 6520 6163   channel code ac
+000039a0: 636f 7264 696e 6720 746f 2074 6865 2053  cording to the S
+000039b0: 4545 4420 7374 616e 6461 7264 2e0a 2020  EED standard..  
+000039c0: 2020 2020 2020 636f 6465 3d73 7461 7473        code=stats
+000039d0: 2e63 6861 6e6e 656c 2c0a 2020 2020 2020  .channel,.      
+000039e0: 2020 2320 5468 6973 2069 7320 7468 6520    # This is the 
+000039f0: 6c6f 6361 7469 6f6e 2063 6f64 6520 6163  location code ac
+00003a00: 636f 7264 696e 6720 746f 2074 6865 2053  cording to the S
+00003a10: 4545 4420 7374 616e 6461 7264 2e0a 2020  EED standard..  
+00003a20: 2020 2020 2020 6c6f 6361 7469 6f6e 5f63        location_c
+00003a30: 6f64 653d 7374 6174 732e 6c6f 6361 7469  ode=stats.locati
+00003a40: 6f6e 2c0a 2020 2020 2020 2020 2320 4e6f  on,.        # No
+00003a50: 7465 2074 6861 7420 7468 6573 6520 636f  te that these co
+00003a60: 6f72 6469 6e61 7465 7320 6361 6e20 6469  ordinates can di
+00003a70: 6666 6572 2066 726f 6d20 7468 6520 7374  ffer from the st
+00003a80: 6174 696f 6e20 636f 6f72 6469 6e61 7465  ation coordinate
+00003a90: 732e 0a20 2020 2020 2020 206c 6174 6974  s..        latit
+00003aa0: 7564 653d 7374 6174 732e 7361 635b 2273  ude=stats.sac["s
+00003ab0: 746c 6122 5d2c 0a20 2020 2020 2020 206c  tla"],.        l
+00003ac0: 6f6e 6769 7475 6465 3d73 7461 7473 2e73  ongitude=stats.s
+00003ad0: 6163 5b22 7374 6c6f 225d 2c0a 2020 2020  ac["stlo"],.    
+00003ae0: 2020 2020 656c 6576 6174 696f 6e3d 7374      elevation=st
+00003af0: 6174 732e 7361 635b 2273 7465 6c22 5d2c  ats.sac["stel"],
+00003b00: 0a20 2020 2020 2020 2064 6570 7468 3d2d  .        depth=-
+00003b10: 7374 6174 732e 7361 635b 2273 7465 6c22  stats.sac["stel"
+00003b20: 5d2c 0a20 2020 2020 2020 2061 7a69 6d75  ],.        azimu
+00003b30: 7468 3d73 7461 7473 2e73 6163 5b22 636d  th=stats.sac["cm
+00003b40: 7061 7a22 5d2c 0a20 2020 2020 2020 2064  paz"],.        d
+00003b50: 6970 3d73 7461 7473 2e73 6163 5b22 636d  ip=stats.sac["cm
+00003b60: 7069 6e63 225d 2c0a 2020 2020 2020 2020  pinc"],.        
+00003b70: 7361 6d70 6c65 5f72 6174 653d 7374 6174  sample_rate=stat
+00003b80: 732e 7361 6d70 6c69 6e67 5f72 6174 652c  s.sampling_rate,
+00003b90: 0a20 2020 2029 0a20 2020 2072 6573 706f  .    ).    respo
+00003ba0: 6e73 6520 3d20 6f62 7370 792e 636f 7265  nse = obspy.core
+00003bb0: 2e69 6e76 656e 746f 7279 2e72 6573 706f  .inventory.respo
+00003bc0: 6e73 652e 5265 7370 6f6e 7365 2829 0a0a  nse.Response()..
+00003bd0: 2020 2020 2320 4e6f 7720 7469 6520 6974      # Now tie it
+00003be0: 2061 6c6c 2074 6f67 6574 6865 722e 0a20   all together.. 
+00003bf0: 2020 2063 6861 2e72 6573 706f 6e73 6520     cha.response 
+00003c00: 3d20 7265 7370 6f6e 7365 0a20 2020 2073  = response.    s
+00003c10: 7461 2e63 6861 6e6e 656c 732e 6170 7065  ta.channels.appe
+00003c20: 6e64 2863 6861 290a 2020 2020 6e65 742e  nd(cha).    net.
+00003c30: 7374 6174 696f 6e73 2e61 7070 656e 6428  stations.append(
+00003c40: 7374 6129 0a20 2020 2069 6e76 2e6e 6574  sta).    inv.net
+00003c50: 776f 726b 732e 6170 7065 6e64 286e 6574  works.append(net
+00003c60: 290a 0a20 2020 2072 6574 7572 6e20 696e  )..    return in
+00003c70: 760a 0a0a 6465 6620 7374 6174 7332 696e  v...def stats2in
+00003c80: 765f 6d73 6565 6428 7374 6174 732c 206c  v_mseed(stats, l
+00003c90: 6f63 733a 2070 642e 4461 7461 4672 616d  ocs: pd.DataFram
+00003ca0: 6529 202d 3e20 496e 7665 6e74 6f72 793a  e) -> Inventory:
+00003cb0: 0a20 2020 2069 6e76 203d 2049 6e76 656e  .    inv = Inven
+00003cc0: 746f 7279 286e 6574 776f 726b 733d 5b5d  tory(networks=[]
+00003cd0: 2c20 736f 7572 6365 3d22 686f 6d65 6772  , source="homegr
+00003ce0: 6f77 6e22 290a 2020 2020 6973 7461 203d  own").    ista =
+00003cf0: 206c 6f63 735b 6c6f 6373 5b22 7374 6174   locs[locs["stat
+00003d00: 696f 6e22 5d20 3d3d 2073 7461 7473 2e73  ion"] == stats.s
+00003d10: 7461 7469 6f6e 5d2e 696e 6465 782e 7661  tation].index.va
+00003d20: 6c75 6573 2e61 7374 7970 6528 2269 6e74  lues.astype("int
+00003d30: 3634 2229 5b30 5d0a 0a20 2020 206e 6574  64")[0]..    net
+00003d40: 203d 204e 6574 776f 726b 280a 2020 2020   = Network(.    
+00003d50: 2020 2020 2320 5468 6973 2069 7320 7468      # This is th
+00003d60: 6520 6e65 7477 6f72 6b20 636f 6465 2061  e network code a
+00003d70: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
+00003d80: 5345 4544 2073 7461 6e64 6172 642e 0a20  SEED standard.. 
+00003d90: 2020 2020 2020 2063 6f64 653d 6c6f 6373         code=locs
+00003da0: 2e69 6c6f 635b 6973 7461 5d5b 226e 6574  .iloc[ista]["net
+00003db0: 776f 726b 225d 2c0a 2020 2020 2020 2020  work"],.        
+00003dc0: 7374 6174 696f 6e73 3d5b 5d2c 0a20 2020  stations=[],.   
+00003dd0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00003de0: 3d22 6372 6561 7465 6420 6672 6f6d 2053  ="created from S
+00003df0: 4143 2061 6e64 2072 6573 7020 6669 6c65  AC and resp file
+00003e00: 7322 2c0a 2020 2020 2020 2020 7374 6172  s",.        star
+00003e10: 745f 6461 7465 3d73 7461 7473 2e73 7461  t_date=stats.sta
+00003e20: 7274 7469 6d65 2c0a 2020 2020 290a 0a20  rttime,.    ).. 
+00003e30: 2020 2073 7461 203d 2053 7461 7469 6f6e     sta = Station
+00003e40: 280a 2020 2020 2020 2020 2320 5468 6973  (.        # This
+00003e50: 2069 7320 7468 6520 7374 6174 696f 6e20   is the station 
+00003e60: 636f 6465 2061 6363 6f72 6469 6e67 2074  code according t
+00003e70: 6f20 7468 6520 5345 4544 2073 7461 6e64  o the SEED stand
+00003e80: 6172 642e 0a20 2020 2020 2020 2063 6f64  ard..        cod
+00003e90: 653d 6c6f 6373 2e69 6c6f 635b 6973 7461  e=locs.iloc[ista
+00003ea0: 5d5b 2273 7461 7469 6f6e 225d 2c0a 2020  ]["station"],.  
+00003eb0: 2020 2020 2020 6c61 7469 7475 6465 3d6c        latitude=l
+00003ec0: 6f63 732e 696c 6f63 5b69 7374 615d 5b22  ocs.iloc[ista]["
+00003ed0: 6c61 7469 7475 6465 225d 2c0a 2020 2020  latitude"],.    
+00003ee0: 2020 2020 6c6f 6e67 6974 7564 653d 6c6f      longitude=lo
+00003ef0: 6373 2e69 6c6f 635b 6973 7461 5d5b 226c  cs.iloc[ista]["l
+00003f00: 6f6e 6769 7475 6465 225d 2c0a 2020 2020  ongitude"],.    
+00003f10: 2020 2020 656c 6576 6174 696f 6e3d 6c6f      elevation=lo
+00003f20: 6373 2e69 6c6f 635b 6973 7461 5d5b 2265  cs.iloc[ista]["e
+00003f30: 6c65 7661 7469 6f6e 225d 2c0a 2020 2020  levation"],.    
+00003f40: 2020 2020 6372 6561 7469 6f6e 5f64 6174      creation_dat
+00003f50: 653d 7374 6174 732e 7374 6172 7474 696d  e=stats.starttim
+00003f60: 652c 0a20 2020 2020 2020 2073 6974 653d  e,.        site=
+00003f70: 5369 7465 286e 616d 653d 2246 6972 7374  Site(name="First
+00003f80: 2073 7461 7469 6f6e 2229 2c0a 2020 2020   station"),.    
+00003f90: 290a 0a20 2020 2063 6861 203d 2043 6861  )..    cha = Cha
+00003fa0: 6e6e 656c 280a 2020 2020 2020 2020 636f  nnel(.        co
+00003fb0: 6465 3d73 7461 7473 2e63 6861 6e6e 656c  de=stats.channel
+00003fc0: 2c0a 2020 2020 2020 2020 6c6f 6361 7469  ,.        locati
+00003fd0: 6f6e 5f63 6f64 653d 7374 6174 732e 6c6f  on_code=stats.lo
+00003fe0: 6361 7469 6f6e 2c0a 2020 2020 2020 2020  cation,.        
+00003ff0: 6c61 7469 7475 6465 3d6c 6f63 732e 696c  latitude=locs.il
+00004000: 6f63 5b69 7374 615d 5b22 6c61 7469 7475  oc[ista]["latitu
+00004010: 6465 225d 2c0a 2020 2020 2020 2020 6c6f  de"],.        lo
+00004020: 6e67 6974 7564 653d 6c6f 6373 2e69 6c6f  ngitude=locs.ilo
+00004030: 635b 6973 7461 5d5b 226c 6f6e 6769 7475  c[ista]["longitu
+00004040: 6465 225d 2c0a 2020 2020 2020 2020 656c  de"],.        el
+00004050: 6576 6174 696f 6e3d 6c6f 6373 2e69 6c6f  evation=locs.ilo
+00004060: 635b 6973 7461 5d5b 2265 6c65 7661 7469  c[ista]["elevati
+00004070: 6f6e 225d 2c0a 2020 2020 2020 2020 6465  on"],.        de
+00004080: 7074 683d 2d6c 6f63 732e 696c 6f63 5b69  pth=-locs.iloc[i
+00004090: 7374 615d 5b22 656c 6576 6174 696f 6e22  sta]["elevation"
+000040a0: 5d2c 0a20 2020 2020 2020 2061 7a69 6d75  ],.        azimu
+000040b0: 7468 3d30 2c0a 2020 2020 2020 2020 6469  th=0,.        di
+000040c0: 703d 302c 0a20 2020 2020 2020 2073 616d  p=0,.        sam
+000040d0: 706c 655f 7261 7465 3d73 7461 7473 2e73  ple_rate=stats.s
+000040e0: 616d 706c 696e 675f 7261 7465 2c0a 2020  ampling_rate,.  
+000040f0: 2020 290a 0a20 2020 2072 6573 706f 6e73    )..    respons
+00004100: 6520 3d20 6f62 7370 792e 636f 7265 2e69  e = obspy.core.i
+00004110: 6e76 656e 746f 7279 2e72 6573 706f 6e73  nventory.respons
+00004120: 652e 5265 7370 6f6e 7365 2829 0a0a 2020  e.Response()..  
+00004130: 2020 2320 4e6f 7720 7469 6520 6974 2061    # Now tie it a
+00004140: 6c6c 2074 6f67 6574 6865 722e 0a20 2020  ll together..   
+00004150: 2063 6861 2e72 6573 706f 6e73 6520 3d20   cha.response = 
+00004160: 7265 7370 6f6e 7365 0a20 2020 2073 7461  response.    sta
+00004170: 2e63 6861 6e6e 656c 732e 6170 7065 6e64  .channels.append
+00004180: 2863 6861 290a 2020 2020 6e65 742e 7374  (cha).    net.st
+00004190: 6174 696f 6e73 2e61 7070 656e 6428 7374  ations.append(st
+000041a0: 6129 0a20 2020 2069 6e76 2e6e 6574 776f  a).    inv.netwo
+000041b0: 726b 732e 6170 7065 6e64 286e 6574 290a  rks.append(net).
+000041c0: 0a20 2020 2072 6574 7572 6e20 696e 760a  .    return inv.
+000041d0: 0a0a 6465 6620 7374 615f 696e 666f 5f66  ..def sta_info_f
+000041e0: 726f 6d5f 696e 7628 696e 763a 206f 6273  rom_inv(inv: obs
+000041f0: 7079 2e63 6f72 652e 696e 7665 6e74 6f72  py.core.inventor
+00004200: 792e 696e 7665 6e74 6f72 792e 496e 7665  y.inventory.Inve
+00004210: 6e74 6f72 7929 3a0a 2020 2020 2222 220a  ntory):.    """.
+00004220: 2020 2020 7468 6973 2066 756e 6374 696f      this functio
+00004230: 6e20 6f75 7470 7574 7320 7374 6174 696f  n outputs statio
+00004240: 6e20 696e 666f 2066 726f 6d20 7468 6520  n info from the 
+00004250: 6f62 7370 7920 696e 7665 6e74 6f72 7920  obspy inventory 
+00004260: 6f62 6a65 6374 0a20 2020 2028 7573 6564  object.    (used
+00004270: 2069 6e20 5330 4229 0a20 2020 2050 4152   in S0B).    PAR
+00004280: 414d 4554 4552 533a 0a20 2020 202d 2d2d  AMETERS:.    ---
 00004290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000042a0: 2d0a 2020 2020 696e 763a 206f 6273 7079  -.    inv: obspy
-000042b0: 2069 6e76 656e 746f 7279 206f 626a 6563   inventory objec
-000042c0: 740a 2020 2020 5245 5455 524e 533a 0a20  t.    RETURNS:. 
-000042d0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-000042e0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7374  ---------.    st
-000042f0: 613a 2073 7461 7469 6f6e 206e 616d 650a  a: station name.
-00004300: 2020 2020 6e65 743a 206e 6574 6f77 726b      net: netowrk
-00004310: 206e 616d 650a 2020 2020 6c6f 6e3a 206c   name.    lon: l
-00004320: 6f6e 6769 7475 6465 206f 6620 7468 6520  ongitude of the 
-00004330: 7374 6174 696f 6e0a 2020 2020 6c61 743a  station.    lat:
-00004340: 206c 6174 6974 7564 6520 6f66 2074 6865   latitude of the
-00004350: 2073 7461 7469 6f6e 0a20 2020 2065 6c76   station.    elv
-00004360: 3a20 656c 6576 6174 696f 6e20 6f66 2074  : elevation of t
-00004370: 6865 2073 7461 7469 6f6e 0a20 2020 206c  he station.    l
-00004380: 6f63 6174 696f 6e3a 206c 6f63 6174 696f  ocation: locatio
-00004390: 6e20 636f 6465 206f 6620 7468 6520 7374  n code of the st
-000043a0: 6174 696f 6e0a 2020 2020 2222 220a 2020  ation.    """.  
-000043b0: 2020 2320 6c6f 6164 2066 726f 6d20 7374    # load from st
-000043c0: 6174 696f 6e20 696e 7665 6e74 6f72 790a  ation inventory.
-000043d0: 2020 2020 7374 6120 3d20 696e 765b 305d      sta = inv[0]
-000043e0: 5b30 5d2e 636f 6465 0a20 2020 206e 6574  [0].code.    net
-000043f0: 203d 2069 6e76 5b30 5d2e 636f 6465 0a20   = inv[0].code. 
-00004400: 2020 206c 6f6e 203d 2069 6e76 5b30 5d5b     lon = inv[0][
-00004410: 305d 2e6c 6f6e 6769 7475 6465 0a20 2020  0].longitude.   
-00004420: 206c 6174 203d 2069 6e76 5b30 5d5b 305d   lat = inv[0][0]
-00004430: 2e6c 6174 6974 7564 650a 2020 2020 6966  .latitude.    if
-00004440: 2069 6e76 5b30 5d5b 305d 2e65 6c65 7661   inv[0][0].eleva
-00004450: 7469 6f6e 3a0a 2020 2020 2020 2020 656c  tion:.        el
-00004460: 7620 3d20 696e 765b 305d 5b30 5d2e 656c  v = inv[0][0].el
-00004470: 6576 6174 696f 6e0a 2020 2020 656c 7365  evation.    else
-00004480: 3a0a 2020 2020 2020 2020 656c 7620 3d20  :.        elv = 
-00004490: 302e 300a 0a20 2020 2069 6620 696e 765b  0.0..    if inv[
-000044a0: 305d 5b30 5d5b 305d 2e6c 6f63 6174 696f  0][0][0].locatio
-000044b0: 6e5f 636f 6465 3a0a 2020 2020 2020 2020  n_code:.        
-000044c0: 6c6f 6361 7469 6f6e 203d 2069 6e76 5b30  location = inv[0
-000044d0: 5d5b 305d 5b30 5d2e 6c6f 6361 7469 6f6e  ][0][0].location
-000044e0: 5f63 6f64 650a 2020 2020 656c 7365 3a0a  _code.    else:.
-000044f0: 2020 2020 2020 2020 6c6f 6361 7469 6f6e          location
-00004500: 203d 2022 3030 220a 0a20 2020 2072 6574   = "00"..    ret
-00004510: 7572 6e20 7374 612c 206e 6574 2c20 6c6f  urn sta, net, lo
-00004520: 6e2c 206c 6174 2c20 656c 762c 206c 6f63  n, lat, elv, loc
-00004530: 6174 696f 6e0a 0a0a 6465 6620 6375 745f  ation...def cut_
-00004540: 7472 6163 655f 6d61 6b65 5f73 7461 7428  trace_make_stat(
-00004550: 6663 5f70 6172 613a 2043 6f6e 6669 6750  fc_para: ConfigP
-00004560: 6172 616d 6574 6572 732c 2063 685f 6461  arameters, ch_da
-00004570: 7461 3a20 4368 616e 6e65 6c44 6174 6129  ta: ChannelData)
-00004580: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
-00004590: 6973 2066 756e 6374 696f 6e20 6375 7473  is function cuts
-000045a0: 2063 6f6e 7469 6e6f 7573 206e 6f69 7365   continous noise
-000045b0: 2064 6174 6120 696e 746f 2075 7365 722d   data into user-
-000045c0: 6465 6669 6e65 6420 7365 676d 656e 7473  defined segments
-000045d0: 2c20 6573 7469 6d61 7465 2074 6865 2073  , estimate the s
-000045e0: 7461 7469 7374 6963 7320 6f66 0a20 2020  tatistics of.   
-000045f0: 2065 6163 6820 7365 676d 656e 7420 616e   each segment an
-00004600: 6420 6b65 6570 2074 696d 6573 7461 6d70  d keep timestamp
-00004610: 206f 6620 6561 6368 2073 6567 6d65 6e74   of each segment
-00004620: 2066 6f72 206c 6174 6572 2075 7365 2e20   for later use. 
-00004630: 2875 7365 6420 696e 2053 3129 0a20 2020  (used in S1).   
-00004640: 2050 4152 414d 4554 4552 533a 0a20 2020   PARAMETERS:.   
-00004650: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-00004660: 2d2d 2d2d 2d2d 2d0a 2020 2020 6666 745f  -------.    fft_
-00004670: 7061 7261 3a20 4120 6469 6374 696f 6e61  para: A dictiona
-00004680: 7279 2063 6f6e 7461 696e 696e 6720 616c  ry containing al
-00004690: 6c20 6666 7420 616e 6420 6363 2070 6172  l fft and cc par
-000046a0: 616d 6574 6572 732e 0a20 2020 2073 6f75  ameters..    sou
-000046b0: 7263 653a 206f 6273 7079 2073 7472 6561  rce: obspy strea
-000046c0: 6d20 6f62 6a65 6374 0a20 2020 2052 4554  m object.    RET
-000046d0: 5552 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d  URNS:.    ------
+000042a0: 2d2d 2d0a 2020 2020 696e 763a 206f 6273  ---.    inv: obs
+000042b0: 7079 2069 6e76 656e 746f 7279 206f 626a  py inventory obj
+000042c0: 6563 740a 2020 2020 5245 5455 524e 533a  ect.    RETURNS:
+000042d0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+000042e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+000042f0: 7374 613a 2073 7461 7469 6f6e 206e 616d  sta: station nam
+00004300: 650a 2020 2020 6e65 743a 206e 6574 6f77  e.    net: netow
+00004310: 726b 206e 616d 650a 2020 2020 6c6f 6e3a  rk name.    lon:
+00004320: 206c 6f6e 6769 7475 6465 206f 6620 7468   longitude of th
+00004330: 6520 7374 6174 696f 6e0a 2020 2020 6c61  e station.    la
+00004340: 743a 206c 6174 6974 7564 6520 6f66 2074  t: latitude of t
+00004350: 6865 2073 7461 7469 6f6e 0a20 2020 2065  he station.    e
+00004360: 6c76 3a20 656c 6576 6174 696f 6e20 6f66  lv: elevation of
+00004370: 2074 6865 2073 7461 7469 6f6e 0a20 2020   the station.   
+00004380: 206c 6f63 6174 696f 6e3a 206c 6f63 6174   location: locat
+00004390: 696f 6e20 636f 6465 206f 6620 7468 6520  ion code of the 
+000043a0: 7374 6174 696f 6e0a 2020 2020 2222 220a  station.    """.
+000043b0: 2020 2020 2320 6c6f 6164 2066 726f 6d20      # load from 
+000043c0: 7374 6174 696f 6e20 696e 7665 6e74 6f72  station inventor
+000043d0: 790a 2020 2020 7374 6120 3d20 696e 765b  y.    sta = inv[
+000043e0: 305d 5b30 5d2e 636f 6465 0a20 2020 206e  0][0].code.    n
+000043f0: 6574 203d 2069 6e76 5b30 5d2e 636f 6465  et = inv[0].code
+00004400: 0a20 2020 206c 6f6e 203d 2069 6e76 5b30  .    lon = inv[0
+00004410: 5d5b 305d 2e6c 6f6e 6769 7475 6465 0a20  ][0].longitude. 
+00004420: 2020 206c 6174 203d 2069 6e76 5b30 5d5b     lat = inv[0][
+00004430: 305d 2e6c 6174 6974 7564 650a 2020 2020  0].latitude.    
+00004440: 6966 2069 6e76 5b30 5d5b 305d 2e65 6c65  if inv[0][0].ele
+00004450: 7661 7469 6f6e 3a0a 2020 2020 2020 2020  vation:.        
+00004460: 656c 7620 3d20 696e 765b 305d 5b30 5d2e  elv = inv[0][0].
+00004470: 656c 6576 6174 696f 6e0a 2020 2020 656c  elevation.    el
+00004480: 7365 3a0a 2020 2020 2020 2020 656c 7620  se:.        elv 
+00004490: 3d20 302e 300a 0a20 2020 2069 6620 696e  = 0.0..    if in
+000044a0: 765b 305d 5b30 5d5b 305d 2e6c 6f63 6174  v[0][0][0].locat
+000044b0: 696f 6e5f 636f 6465 3a0a 2020 2020 2020  ion_code:.      
+000044c0: 2020 6c6f 6361 7469 6f6e 203d 2069 6e76    location = inv
+000044d0: 5b30 5d5b 305d 5b30 5d2e 6c6f 6361 7469  [0][0][0].locati
+000044e0: 6f6e 5f63 6f64 650a 2020 2020 656c 7365  on_code.    else
+000044f0: 3a0a 2020 2020 2020 2020 6c6f 6361 7469  :.        locati
+00004500: 6f6e 203d 2022 3030 220a 0a20 2020 2072  on = "00"..    r
+00004510: 6574 7572 6e20 7374 612c 206e 6574 2c20  eturn sta, net, 
+00004520: 6c6f 6e2c 206c 6174 2c20 656c 762c 206c  lon, lat, elv, l
+00004530: 6f63 6174 696f 6e0a 0a0a 6465 6620 6375  ocation...def cu
+00004540: 745f 7472 6163 655f 6d61 6b65 5f73 7461  t_trace_make_sta
+00004550: 7428 6663 5f70 6172 613a 2043 6f6e 6669  t(fc_para: Confi
+00004560: 6750 6172 616d 6574 6572 732c 2063 685f  gParameters, ch_
+00004570: 6461 7461 3a20 4368 616e 6e65 6c44 6174  data: ChannelDat
+00004580: 6129 3a0a 2020 2020 2222 220a 2020 2020  a):.    """.    
+00004590: 7468 6973 2066 756e 6374 696f 6e20 6375  this function cu
+000045a0: 7473 2063 6f6e 7469 6e6f 7573 206e 6f69  ts continous noi
+000045b0: 7365 2064 6174 6120 696e 746f 2075 7365  se data into use
+000045c0: 722d 6465 6669 6e65 6420 7365 676d 656e  r-defined segmen
+000045d0: 7473 2c20 6573 7469 6d61 7465 2074 6865  ts, estimate the
+000045e0: 2073 7461 7469 7374 6963 7320 6f66 0a20   statistics of. 
+000045f0: 2020 2065 6163 6820 7365 676d 656e 7420     each segment 
+00004600: 616e 6420 6b65 6570 2074 696d 6573 7461  and keep timesta
+00004610: 6d70 206f 6620 6561 6368 2073 6567 6d65  mp of each segme
+00004620: 6e74 2066 6f72 206c 6174 6572 2075 7365  nt for later use
+00004630: 2e20 2875 7365 6420 696e 2053 3129 0a20  . (used in S1). 
+00004640: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
+00004650: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00004660: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6666  ---------.    ff
+00004670: 745f 7061 7261 3a20 4120 6469 6374 696f  t_para: A dictio
+00004680: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+00004690: 616c 6c20 6666 7420 616e 6420 6363 2070  all fft and cc p
+000046a0: 6172 616d 6574 6572 732e 0a20 2020 2073  arameters..    s
+000046b0: 6f75 7263 653a 206f 6273 7079 2073 7472  ource: obspy str
+000046c0: 6561 6d20 6f62 6a65 6374 0a20 2020 2052  eam object.    R
+000046d0: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
 000046e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000046f0: 0a20 2020 2074 7261 6365 5f73 7464 533a  .    trace_stdS:
-00004700: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
-00004710: 696f 6e20 6f66 2074 6865 206e 6f69 7365  ion of the noise
-00004720: 2061 6d70 6c69 7475 6465 206f 6620 6561   amplitude of ea
-00004730: 6368 2073 6567 6d65 6e74 0a20 2020 2064  ch segment.    d
-00004740: 6174 6153 5f74 3a20 2020 2074 696d 6573  ataS_t:    times
-00004750: 7461 6d70 7320 6f66 2065 6163 6820 7365  tamps of each se
-00004760: 676d 656e 740a 2020 2020 6461 7461 533a  gment.    dataS:
-00004770: 2020 2020 2020 3244 206d 6174 7269 7820        2D matrix 
-00004780: 6f66 2074 6865 2073 6567 6d65 6e74 6564  of the segmented
-00004790: 2064 6174 610a 2020 2020 2222 220a 2020   data.    """.  
-000047a0: 2020 2320 6465 6669 6e65 2072 6574 7572    # define retur
-000047b0: 6e20 7661 7269 6162 6c65 7320 6669 7273  n variables firs
-000047c0: 740a 2020 2020 736f 7572 6365 5f70 6172  t.    source_par
-000047d0: 616d 7320 3d20 5b5d 0a20 2020 2064 6174  ams = [].    dat
-000047e0: 6153 5f74 203d 205b 5d0a 2020 2020 6461  aS_t = [].    da
-000047f0: 7461 5320 3d20 5b5d 0a0a 2020 2020 2320  taS = []..    # 
-00004800: 7573 6566 756c 2070 6172 616d 6574 6572  useful parameter
-00004810: 7320 666f 7220 7472 6163 6520 736c 6964  s for trace slid
-00004820: 696e 670a 2020 2020 6e73 6567 203d 2069  ing.    nseg = i
-00004830: 6e74 286e 702e 666c 6f6f 7228 2866 635f  nt(np.floor((fc_
-00004840: 7061 7261 2e69 6e63 5f68 6f75 7273 202f  para.inc_hours /
-00004850: 2032 3420 2a20 3836 3430 3020 2d20 6663   24 * 86400 - fc
-00004860: 5f70 6172 612e 6363 5f6c 656e 2920 2f20  _para.cc_len) / 
-00004870: 6663 5f70 6172 612e 7374 6570 2929 0a20  fc_para.step)). 
-00004880: 2020 2073 7073 203d 2069 6e74 2863 685f     sps = int(ch_
-00004890: 6461 7461 2e73 616d 706c 696e 675f 7261  data.sampling_ra
-000048a0: 7465 290a 2020 2020 7374 6172 7474 696d  te).    starttim
-000048b0: 6520 3d20 6368 5f64 6174 612e 7374 6172  e = ch_data.star
-000048c0: 745f 7469 6d65 7374 616d 700a 2020 2020  t_timestamp.    
-000048d0: 2320 636f 7079 2064 6174 6120 696e 746f  # copy data into
-000048e0: 2061 7272 6179 0a20 2020 2064 6174 6120   array.    data 
-000048f0: 3d20 6368 5f64 6174 612e 6461 7461 0a0a  = ch_data.data..
-00004900: 2020 2020 2320 6966 2074 6865 2064 6174      # if the dat
-00004910: 6120 6973 2073 686f 7274 6572 2074 6861  a is shorter tha
-00004920: 6e20 7468 6520 7469 6d20 6368 756e 636b  n the tim chunck
-00004930: 2c20 7265 7475 726e 207a 6572 6f20 7661  , return zero va
-00004940: 6c75 6573 0a20 2020 2069 6620 6461 7461  lues.    if data
-00004950: 2e73 697a 6520 3c20 7370 7320 2a20 6663  .size < sps * fc
-00004960: 5f70 6172 612e 696e 635f 686f 7572 7320  _para.inc_hours 
-00004970: 2a20 3336 3030 3a0a 2020 2020 2020 2020  * 3600:.        
-00004980: 7265 7475 726e 2073 6f75 7263 655f 7061  return source_pa
-00004990: 7261 6d73 2c20 6461 7461 535f 742c 2064  rams, dataS_t, d
-000049a0: 6174 6153 0a0a 2020 2020 2320 7374 6174  ataS..    # stat
-000049b0: 6973 7469 6320 746f 2064 6574 6563 7420  istic to detect 
-000049c0: 7365 676d 656e 7473 2074 6861 7420 6d61  segments that ma
-000049d0: 7920 6265 2061 7373 6f63 6961 7465 6420  y be associated 
-000049e0: 7769 7468 2065 6172 7468 7175 616b 6573  with earthquakes
-000049f0: 0a20 2020 2061 6c6c 5f6d 6164 5320 3d20  .    all_madS = 
-00004a00: 6d61 6428 6461 7461 2920 2023 206d 6564  mad(data)  # med
-00004a10: 6961 6e20 6162 736f 6c75 7465 2064 6576  ian absolute dev
-00004a20: 6961 7469 6f6e 206f 7665 7220 616c 6c20  iation over all 
-00004a30: 6e6f 6973 6520 7769 6e64 6f77 0a20 2020  noise window.   
-00004a40: 2061 6c6c 5f73 7464 5320 3d20 6e70 2e73   all_stdS = np.s
-00004a50: 7464 2864 6174 6129 2020 2320 7374 616e  td(data)  # stan
-00004a60: 6461 7264 2064 6576 6961 7469 6f6e 206f  dard deviation o
-00004a70: 7665 7220 616c 6c20 6e6f 6973 6520 7769  ver all noise wi
-00004a80: 6e64 6f77 0a20 2020 2069 6620 616c 6c5f  ndow.    if all_
-00004a90: 6d61 6453 203d 3d20 3020 6f72 2061 6c6c  madS == 0 or all
-00004aa0: 5f73 7464 5320 3d3d 2030 206f 7220 6e70  _stdS == 0 or np
-00004ab0: 2e69 736e 616e 2861 6c6c 5f6d 6164 5329  .isnan(all_madS)
-00004ac0: 206f 7220 6e70 2e69 736e 616e 2861 6c6c   or np.isnan(all
-00004ad0: 5f73 7464 5329 3a0a 2020 2020 2020 2020  _stdS):.        
-00004ae0: 7072 696e 7428 2263 6f6e 7469 6e75 6521  print("continue!
-00004af0: 206d 6164 5320 6f72 2073 7464 5320 6571   madS or stdS eq
-00004b00: 7561 6c73 2074 6f20 3020 666f 7220 2573  uals to 0 for %s
-00004b10: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-00004b20: 6e20 736f 7572 6365 5f70 6172 616d 732c  n source_params,
-00004b30: 2064 6174 6153 5f74 2c20 6461 7461 530a   dataS_t, dataS.
-00004b40: 0a20 2020 2023 2069 6e69 7469 616c 697a  .    # initializ
-00004b50: 6520 7661 7269 6162 6c65 730a 2020 2020  e variables.    
-00004b60: 6e70 7473 203d 2069 6e74 2866 635f 7061  npts = int(fc_pa
-00004b70: 7261 2e63 635f 6c65 6e20 2a20 7370 7329  ra.cc_len * sps)
-00004b80: 0a20 2020 2023 2074 7261 6365 5f6d 6164  .    # trace_mad
-00004b90: 5320 3d20 6e70 2e7a 6572 6f73 286e 7365  S = np.zeros(nse
-00004ba0: 672c 6474 7970 653d 6e70 2e66 6c6f 6174  g,dtype=np.float
-00004bb0: 3332 290a 2020 2020 7472 6163 655f 7374  32).    trace_st
-00004bc0: 6453 203d 206e 702e 7a65 726f 7328 6e73  dS = np.zeros(ns
-00004bd0: 6567 2c20 6474 7970 653d 6e70 2e66 6c6f  eg, dtype=np.flo
-00004be0: 6174 3332 290a 2020 2020 6461 7461 5320  at32).    dataS 
-00004bf0: 3d20 6e70 2e7a 6572 6f73 2873 6861 7065  = np.zeros(shape
-00004c00: 3d28 696e 7428 6e73 6567 292c 2069 6e74  =(int(nseg), int
-00004c10: 286e 7074 7329 292c 2064 7479 7065 3d6e  (npts)), dtype=n
-00004c20: 702e 666c 6f61 7433 3229 0a20 2020 2064  p.float32).    d
-00004c30: 6174 6153 5f74 203d 206e 702e 7a65 726f  ataS_t = np.zero
-00004c40: 7328 6e73 6567 2c20 6474 7970 653d 6e70  s(nseg, dtype=np
-00004c50: 2e66 6c6f 6174 3332 290a 0a20 2020 2069  .float32)..    i
-00004c60: 6e64 7831 203d 2030 0a20 2020 2066 6f72  ndx1 = 0.    for
-00004c70: 2069 7365 6720 696e 2072 616e 6765 286e   iseg in range(n
-00004c80: 7365 6729 3a0a 2020 2020 2020 2020 696e  seg):.        in
-00004c90: 6478 3220 3d20 696e 6478 3120 2b20 6e70  dx2 = indx1 + np
-00004ca0: 7473 0a20 2020 2020 2020 2064 6174 6153  ts.        dataS
-00004cb0: 5b69 7365 675d 203d 2064 6174 615b 696e  [iseg] = data[in
-00004cc0: 6478 313a 696e 6478 325d 0a20 2020 2020  dx1:indx2].     
-00004cd0: 2020 2023 2074 7261 6365 5f6d 6164 535b     # trace_madS[
-00004ce0: 6973 6567 5d20 3d20 286e 702e 6d61 7828  iseg] = (np.max(
-00004cf0: 6e70 2e61 6273 2864 6174 6153 5b69 7365  np.abs(dataS[ise
-00004d00: 675d 2929 2f61 6c6c 5f6d 6164 5329 0a20  g]))/all_madS). 
-00004d10: 2020 2020 2020 2074 7261 6365 5f73 7464         trace_std
-00004d20: 535b 6973 6567 5d20 3d20 6e70 2e6d 6178  S[iseg] = np.max
-00004d30: 286e 702e 6162 7328 6461 7461 535b 6973  (np.abs(dataS[is
-00004d40: 6567 5d29 2920 2f20 616c 6c5f 7374 6453  eg])) / all_stdS
-00004d50: 0a20 2020 2020 2020 2064 6174 6153 5f74  .        dataS_t
-00004d60: 5b69 7365 675d 203d 2073 7461 7274 7469  [iseg] = startti
-00004d70: 6d65 202b 2066 635f 7061 7261 2e73 7465  me + fc_para.ste
-00004d80: 7020 2a20 6973 6567 0a20 2020 2020 2020  p * iseg.       
-00004d90: 2069 6e64 7831 203d 2069 6e64 7831 202b   indx1 = indx1 +
-00004da0: 2069 6e74 2866 635f 7061 7261 2e73 7465   int(fc_para.ste
-00004db0: 7029 202a 2073 7073 0a0a 2020 2020 2320  p) * sps..    # 
-00004dc0: 3244 2061 7272 6179 2070 726f 6365 7373  2D array process
-00004dd0: 696e 670a 2020 2020 6461 7461 5320 3d20  ing.    dataS = 
-00004de0: 6465 6d65 616e 2864 6174 6153 290a 2020  demean(dataS).  
-00004df0: 2020 6461 7461 5320 3d20 6465 7472 656e    dataS = detren
-00004e00: 6428 6461 7461 5329 0a20 2020 2064 6174  d(dataS).    dat
-00004e10: 6153 203d 2074 6170 6572 2864 6174 6153  aS = taper(dataS
-00004e20: 290a 0a20 2020 2072 6574 7572 6e20 7472  )..    return tr
-00004e30: 6163 655f 7374 6453 2c20 6461 7461 535f  ace_stdS, dataS_
-00004e40: 742c 2064 6174 6153 0a0a 0a64 6566 206e  t, dataS...def n
-00004e50: 6f69 7365 5f70 726f 6365 7373 696e 6728  oise_processing(
-00004e60: 6666 745f 7061 7261 2c20 6461 7461 5329  fft_para, dataS)
-00004e70: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
-00004e80: 6973 2066 756e 6374 696f 6e20 7065 7266  is function perf
-00004e90: 6f72 6d73 2074 696d 6520 646f 6d61 696e  orms time domain
-00004ea0: 2061 6e64 2066 7265 7175 656e 6379 2064   and frequency d
-00004eb0: 6f6d 6169 6e20 6e6f 726d 616c 697a 6174  omain normalizat
-00004ec0: 696f 6e20 6966 206e 6565 6465 642e 2069  ion if needed. i
-00004ed0: 6e20 7265 616c 2063 6173 652c 2077 6520  n real case, we 
-00004ee0: 7072 6566 6572 2075 7365 2069 6e63 6c75  prefer use inclu
-00004ef0: 6465 0a20 2020 2074 6865 206e 6f72 6d61  de.    the norma
-00004f00: 6c69 7a61 7469 6f6e 2069 6e20 7468 6520  lization in the 
-00004f10: 6372 6f73 732d 636f 7272 6561 6c74 696f  cross-correaltio
-00004f20: 6e20 7374 6570 7320 6279 2073 656c 6563  n steps by selec
-00004f30: 7469 6e67 2063 6f68 6572 656e 6379 206f  ting coherency o
-00004f40: 7220 6465 636f 6e0a 2020 2020 2850 7269  r decon.    (Pri
-00004f50: 6574 6f20 6574 2061 6c2c 2032 3030 382c  eto et al, 2008,
-00004f60: 2032 3030 393b 2044 656e 6f6c 6c65 2065   2009; Denolle e
-00004f70: 7420 616c 2c20 3230 3133 290a 2020 2020  t al, 2013).    
-00004f80: 5041 524d 4145 5445 5253 3a0a 2020 2020  PARMAETERS:.    
-00004f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00004fa0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066 6674  --------.    fft
-00004fb0: 5f70 6172 613a 2064 6963 7469 6f6e 6172  _para: dictionar
-00004fc0: 7920 636f 6e74 6169 6e69 6e67 2061 6c6c  y containing all
-00004fd0: 2075 7365 6675 6c20 7661 7269 6162 6c65   useful variable
-00004fe0: 7320 7573 6564 2066 6f72 2066 6674 2061  s used for fft a
-00004ff0: 6e64 2063 630a 2020 2020 6461 7461 533a  nd cc.    dataS:
-00005000: 2032 4420 6d61 7472 6978 206f 6620 616c   2D matrix of al
-00005010: 6c20 7365 676d 656e 7465 6420 6e6f 6973  l segmented nois
-00005020: 6520 6461 7461 0a20 2020 2023 204f 5554  e data.    # OUT
-00005030: 5055 5420 5641 5249 4142 4c45 533a 0a20  PUT VARIABLES:. 
-00005040: 2020 2073 6f75 7263 655f 7768 6974 653a     source_white:
-00005050: 2032 4420 6d61 7472 6978 206f 6620 6461   2D matrix of da
-00005060: 7461 2073 7065 6374 7261 0a20 2020 2022  ta spectra.    "
-00005070: 2222 0a20 2020 2023 206c 6f61 6420 7061  "".    # load pa
-00005080: 7261 6d65 7465 7273 2066 6972 7374 0a20  rameters first. 
-00005090: 2020 2074 696d 655f 6e6f 726d 203d 2066     time_norm = f
-000050a0: 6674 5f70 6172 615b 2274 696d 655f 6e6f  ft_para["time_no
-000050b0: 726d 225d 0a20 2020 2066 7265 715f 6e6f  rm"].    freq_no
-000050c0: 726d 203d 2066 6674 5f70 6172 615b 2266  rm = fft_para["f
-000050d0: 7265 715f 6e6f 726d 225d 0a20 2020 2073  req_norm"].    s
-000050e0: 6d6f 6f74 685f 4e20 3d20 6666 745f 7061  mooth_N = fft_pa
-000050f0: 7261 5b22 736d 6f6f 7468 5f4e 225d 0a20  ra["smooth_N"]. 
-00005100: 2020 204e 203d 2064 6174 6153 2e73 6861     N = dataS.sha
-00005110: 7065 5b30 5d0a 0a20 2020 2023 202d 2d2d  pe[0]..    # ---
-00005120: 2d2d 2d74 6f20 6e6f 726d 616c 697a 6520  ---to normalize 
-00005130: 696e 2074 696d 6520 6f72 206e 6f74 2d2d  in time or not--
-00005140: 2d2d 2d2d 0a20 2020 2069 6620 7469 6d65  ----.    if time
-00005150: 5f6e 6f72 6d20 213d 2022 6e6f 223a 0a20  _norm != "no":. 
-00005160: 2020 2020 2020 2069 6620 7469 6d65 5f6e         if time_n
-00005170: 6f72 6d20 3d3d 2022 6f6e 655f 6269 7422  orm == "one_bit"
-00005180: 3a20 2023 2073 6967 6e20 6e6f 726d 616c  :  # sign normal
-00005190: 697a 6174 696f 6e0a 2020 2020 2020 2020  ization.        
-000051a0: 2020 2020 7768 6974 6520 3d20 6e70 2e73      white = np.s
-000051b0: 6967 6e28 6461 7461 5329 0a20 2020 2020  ign(dataS).     
-000051c0: 2020 2065 6c69 6620 7469 6d65 5f6e 6f72     elif time_nor
-000051d0: 6d20 3d3d 2022 726d 6122 3a20 2023 2072  m == "rma":  # r
-000051e0: 756e 6e69 6e67 206d 6561 6e3a 206e 6f72  unning mean: nor
-000051f0: 6d61 6c69 7a61 7469 6f6e 206f 7665 7220  malization over 
-00005200: 736d 6f6f 7468 6564 2061 6273 6f6c 7574  smoothed absolut
-00005210: 6520 6176 6572 6167 650a 2020 2020 2020  e average.      
-00005220: 2020 2020 2020 7768 6974 6520 3d20 6e70        white = np
-00005230: 2e7a 6572 6f73 2873 6861 7065 3d64 6174  .zeros(shape=dat
-00005240: 6153 2e73 6861 7065 2c20 6474 7970 653d  aS.shape, dtype=
-00005250: 6461 7461 532e 6474 7970 6529 0a20 2020  dataS.dtype).   
-00005260: 2020 2020 2020 2020 2066 6f72 206b 6b6b           for kkk
-00005270: 2069 6e20 7261 6e67 6528 4e29 3a0a 2020   in range(N):.  
-00005280: 2020 2020 2020 2020 2020 2020 2020 7768                wh
-00005290: 6974 655b 6b6b 6b2c 203a 5d20 3d20 6461  ite[kkk, :] = da
-000052a0: 7461 535b 6b6b 6b2c 203a 5d20 2f20 6d6f  taS[kkk, :] / mo
-000052b0: 7669 6e67 5f61 7665 286e 702e 6162 7328  ving_ave(np.abs(
-000052c0: 6461 7461 535b 6b6b 6b2c 203a 5d29 2c20  dataS[kkk, :]), 
-000052d0: 736d 6f6f 7468 5f4e 290a 0a20 2020 2065  smooth_N)..    e
-000052e0: 6c73 653a 2020 2320 646f 6e27 7420 6e6f  lse:  # don't no
-000052f0: 726d 616c 697a 650a 2020 2020 2020 2020  rmalize.        
-00005300: 7768 6974 6520 3d20 6461 7461 530a 0a20  white = dataS.. 
-00005310: 2020 2023 202d 2d2d 2d2d 746f 2077 6869     # -----to whi
-00005320: 7465 6e20 6f72 206e 6f74 2d2d 2d2d 2d2d  ten or not------
-00005330: 0a20 2020 2069 6620 6672 6571 5f6e 6f72  .    if freq_nor
-00005340: 6d20 213d 2022 6e6f 223a 0a20 2020 2020  m != "no":.     
-00005350: 2020 2073 6f75 7263 655f 7768 6974 6520     source_white 
-00005360: 3d20 7768 6974 656e 2877 6869 7465 2c20  = whiten(white, 
-00005370: 6666 745f 7061 7261 2920 2023 2077 6869  fft_para)  # whi
-00005380: 7465 6e20 616e 6420 7265 7475 726e 2046  ten and return F
-00005390: 4654 0a20 2020 2065 6c73 653a 0a20 2020  FT.    else:.   
-000053a0: 2020 2020 204e 6666 7420 3d20 696e 7428       Nfft = int(
-000053b0: 6e65 7874 5f66 6173 745f 6c65 6e28 696e  next_fast_len(in
-000053c0: 7428 6461 7461 532e 7368 6170 655b 315d  t(dataS.shape[1]
-000053d0: 2929 290a 2020 2020 2020 2020 736f 7572  ))).        sour
-000053e0: 6365 5f77 6869 7465 203d 2073 6369 7079  ce_white = scipy
-000053f0: 2e66 6674 7061 636b 2e66 6674 2877 6869  .fftpack.fft(whi
-00005400: 7465 2c20 4e66 6674 2c20 6178 6973 3d31  te, Nfft, axis=1
-00005410: 2920 2023 2072 6574 7572 6e20 4646 540a  )  # return FFT.
-00005420: 0a20 2020 2072 6574 7572 6e20 736f 7572  .    return sour
-00005430: 6365 5f77 6869 7465 0a0a 0a64 6566 2073  ce_white...def s
-00005440: 6d6f 6f74 685f 736f 7572 6365 5f73 7065  mooth_source_spe
-00005450: 6374 2863 635f 7061 7261 2c20 6666 7431  ct(cc_para, fft1
-00005460: 293a 0a20 2020 2022 2222 0a20 2020 2074  ):.    """.    t
-00005470: 6869 7320 6675 6e63 7469 6f6e 2073 6d6f  his function smo
-00005480: 6f74 6865 7320 616d 706c 6974 7564 6520  othes amplitude 
-00005490: 7370 6563 7472 756d 206f 6620 7468 6520  spectrum of the 
-000054a0: 3244 2073 7065 6374 7261 6c20 6d61 7472  2D spectral matr
-000054b0: 6978 2e20 2875 7365 6420 696e 2053 3129  ix. (used in S1)
-000054c0: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
-000054d0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-000054e0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063  ----------.    c
-000054f0: 635f 7061 7261 3a20 6469 6374 696f 6e61  c_para: dictiona
-00005500: 7279 2063 6f6e 7461 696e 696e 6720 7573  ry containing us
-00005510: 6566 756c 2063 6320 7061 7261 6d65 7465  eful cc paramete
-00005520: 7273 0a20 2020 2066 6674 313a 2020 2020  rs.    fft1:    
-00005530: 736f 7572 6365 2073 7065 6374 7275 6d20  source spectrum 
-00005540: 6d61 7472 6978 0a0a 2020 2020 5245 5455  matrix..    RETU
-00005550: 524e 533a 0a20 2020 202d 2d2d 2d2d 2d2d  RNS:.    -------
-00005560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-00005570: 2020 2073 6666 7431 3a20 636f 6d70 6c65     sfft1: comple
-00005580: 7820 6e75 6d70 7920 6172 7261 7920 7769  x numpy array wi
-00005590: 7468 206e 6f72 6d61 6c69 7a65 6420 7370  th normalized sp
-000055a0: 6563 7472 756d 0a20 2020 2022 2222 0a20  ectrum.    """. 
-000055b0: 2020 2063 635f 6d65 7468 6f64 203d 2063     cc_method = c
-000055c0: 635f 7061 7261 5b22 6363 5f6d 6574 686f  c_para["cc_metho
-000055d0: 6422 5d0a 2020 2020 736d 6f6f 7468 7370  d"].    smoothsp
-000055e0: 6563 745f 4e20 3d20 6363 5f70 6172 615b  ect_N = cc_para[
-000055f0: 2273 6d6f 6f74 6873 7065 6374 5f4e 225d  "smoothspect_N"]
-00005600: 0a0a 2020 2020 6966 2063 635f 6d65 7468  ..    if cc_meth
-00005610: 6f64 203d 3d20 2264 6563 6f6e 7622 3a0a  od == "deconv":.
-00005620: 2020 2020 2020 2020 2320 2d2d 2d2d 2d6e          # -----n
-00005630: 6f72 6d61 6c69 7a65 2073 696e 676c 652d  ormalize single-
-00005640: 7374 6174 696f 6e20 6363 2074 6f20 7a20  station cc to z 
-00005650: 636f 6d70 6f6e 656e 742d 2d2d 2d2d 0a20  component-----. 
-00005660: 2020 2020 2020 2074 656d 7020 3d20 6d6f         temp = mo
-00005670: 7669 6e67 5f61 7665 286e 702e 6162 7328  ving_ave(np.abs(
-00005680: 6666 7431 292c 2073 6d6f 6f74 6873 7065  fft1), smoothspe
-00005690: 6374 5f4e 290a 2020 2020 2020 2020 7472  ct_N).        tr
-000056a0: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-000056b0: 6666 7431 203d 206e 702e 636f 6e6a 2866  fft1 = np.conj(f
-000056c0: 6674 3129 202f 2074 656d 702a 2a32 0a20  ft1) / temp**2. 
-000056d0: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-000056e0: 6365 7074 696f 6e3a 0a20 2020 2020 2020  ception:.       
-000056f0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00005700: 4572 726f 7228 2273 6d6f 6f74 6865 6420  Error("smoothed 
-00005710: 7370 6563 7472 756d 2068 6173 207a 6572  spectrum has zer
-00005720: 6f20 7661 6c75 6573 2229 0a0a 2020 2020  o values")..    
-00005730: 656c 6966 2063 635f 6d65 7468 6f64 203d  elif cc_method =
-00005740: 3d20 2263 6f68 6572 656e 6379 223a 0a20  = "coherency":. 
-00005750: 2020 2020 2020 2074 656d 7020 3d20 6d6f         temp = mo
-00005760: 7669 6e67 5f61 7665 286e 702e 6162 7328  ving_ave(np.abs(
-00005770: 6666 7431 292c 2073 6d6f 6f74 6873 7065  fft1), smoothspe
-00005780: 6374 5f4e 290a 2020 2020 2020 2020 7472  ct_N).        tr
-00005790: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-000057a0: 6666 7431 203d 206e 702e 636f 6e6a 2866  fft1 = np.conj(f
-000057b0: 6674 3129 202f 2074 656d 700a 2020 2020  ft1) / temp.    
-000057c0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-000057d0: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-000057e0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-000057f0: 6f72 2822 736d 6f6f 7468 6564 2073 7065  or("smoothed spe
-00005800: 6374 7275 6d20 6861 7320 7a65 726f 2076  ctrum has zero v
-00005810: 616c 7565 7322 290a 0a20 2020 2065 6c69  alues")..    eli
-00005820: 6620 6363 5f6d 6574 686f 6420 3d3d 2022  f cc_method == "
-00005830: 7863 6f72 7222 3a0a 2020 2020 2020 2020  xcorr":.        
-00005840: 7366 6674 3120 3d20 6e70 2e63 6f6e 6a28  sfft1 = np.conj(
-00005850: 6666 7431 290a 0a20 2020 2065 6c73 653a  fft1)..    else:
-00005860: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-00005870: 616c 7565 4572 726f 7228 226e 6f20 636f  alueError("no co
-00005880: 7272 6563 7469 6f6e 2063 6f72 7265 6c61  rrection correla
-00005890: 7469 6f6e 206d 6574 686f 6420 6973 2073  tion method is s
-000058a0: 656c 6563 7465 6420 6174 204c 3539 2229  elected at L59")
-000058b0: 0a0a 2020 2020 7265 7475 726e 2073 6666  ..    return sff
-000058c0: 7431 0a0a 0a64 6566 2063 6f72 7265 6c61  t1...def correla
-000058d0: 7465 2866 6674 315f 736d 6f6f 7468 6564  te(fft1_smoothed
-000058e0: 5f61 6273 2c20 6666 7432 2c20 442c 204e  _abs, fft2, D, N
-000058f0: 6666 742c 2064 6174 6153 5f74 293a 0a20  fft, dataS_t):. 
-00005900: 2020 2022 2222 0a20 2020 2074 6869 7320     """.    this 
-00005910: 6675 6e63 7469 6f6e 2064 6f65 7320 7468  function does th
-00005920: 6520 6372 6f73 732d 636f 7272 656c 6174  e cross-correlat
-00005930: 696f 6e20 696e 2066 7265 7120 646f 6d61  ion in freq doma
-00005940: 696e 2061 6e64 2068 6173 2074 6865 206f  in and has the o
-00005950: 7074 696f 6e20 746f 206b 6565 7020 7375  ption to keep su
-00005960: 622d 7374 6163 6b73 206f 660a 2020 2020  b-stacks of.    
-00005970: 7468 6520 6372 6f73 732d 636f 7272 656c  the cross-correl
-00005980: 6174 696f 6e20 6966 206e 6565 6465 642e  ation if needed.
-00005990: 2069 7420 7461 6b65 7320 6164 7661 6e74   it takes advant
-000059a0: 6167 6520 6f66 2074 6865 206c 696e 6561  age of the linea
-000059b0: 7220 7265 6c61 7469 6f6e 7368 6970 206f  r relationship o
-000059c0: 6620 6966 6674 2c20 736f 2074 6861 740a  f ifft, so that.
-000059d0: 2020 2020 7374 6163 6b69 6e67 2069 7320      stacking is 
-000059e0: 7065 7266 6f72 6d65 6420 696e 2073 7065  performed in spe
-000059f0: 6374 7275 6d20 646f 6d61 696e 2066 6972  ctrum domain fir
-00005a00: 7374 2074 6f20 7265 6475 6365 2074 6865  st to reduce the
-00005a10: 2074 6f74 616c 206e 756d 6265 7220 6f66   total number of
-00005a20: 2069 6666 742e 2028 7573 6564 2069 6e20   ifft. (used in 
-00005a30: 5331 290a 2020 2020 5041 5241 4d45 5445  S1).    PARAMETE
-00005a40: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
-00005a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00005a60: 2020 6666 7431 5f73 6d6f 6f74 6865 645f    fft1_smoothed_
-00005a70: 6162 733a 2073 6d6f 6f74 6865 6420 706f  abs: smoothed po
-00005a80: 7765 7220 7370 6563 7472 616c 2064 656e  wer spectral den
-00005a90: 7369 7479 206f 6620 7468 6520 4646 5420  sity of the FFT 
-00005aa0: 666f 7220 7468 6520 736f 7572 6365 2073  for the source s
-00005ab0: 7461 7469 6f6e 0a20 2020 2066 6674 323a  tation.    fft2:
-00005ac0: 2072 6177 2046 4654 2073 7065 6374 7275   raw FFT spectru
-00005ad0: 6d20 6f66 2074 6865 2072 6563 6569 7665  m of the receive
-00005ae0: 7220 7374 6174 696f 6e0a 2020 2020 443a  r station.    D:
-00005af0: 2064 6963 7469 6f6e 6172 7920 636f 6e74   dictionary cont
-00005b00: 6169 6e69 6e67 2066 6f6c 6c6f 7769 6e67  aining following
-00005b10: 2070 6172 616d 6574 6572 733a 0a20 2020   parameters:.   
-00005b20: 2020 2020 206d 6178 6c61 673a 2020 6d61       maxlag:  ma
-00005b30: 7869 6d75 6d20 6c61 6773 2074 6f20 6b65  ximum lags to ke
-00005b40: 6570 2069 6e20 7468 6520 6372 6f73 7320  ep in the cross 
-00005b50: 636f 7272 656c 6174 696f 6e0a 2020 2020  correlation.    
-00005b60: 2020 2020 6474 3a20 2020 2020 2073 616d      dt:      sam
-00005b70: 706c 696e 6720 7261 7465 2028 696e 2073  pling rate (in s
-00005b80: 290a 2020 2020 2020 2020 6e77 696e 3a20  ).        nwin: 
-00005b90: 2020 206e 756d 6265 7220 6f66 2073 6567     number of seg
-00005ba0: 6d65 6e74 7320 696e 2074 6865 2032 4420  ments in the 2D 
-00005bb0: 6d61 7472 6978 0a20 2020 2020 2020 206d  matrix.        m
-00005bc0: 6574 686f 643a 2020 6372 6f73 732d 636f  ethod:  cross-co
-00005bd0: 7272 656c 6174 696f 6e20 6d65 7468 6f64  rrelation method
-00005be0: 7320 7365 6c65 6374 6564 2062 7920 7468  s selected by th
-00005bf0: 6520 7573 6572 0a20 2020 2020 2020 2066  e user.        f
-00005c00: 7265 716d 696e 3a20 6d69 6e69 6d75 6d20  reqmin: minimum 
-00005c10: 6672 6571 7565 6e63 7920 2848 7a29 0a20  frequency (Hz). 
-00005c20: 2020 2020 2020 2066 7265 716d 6178 3a20         freqmax: 
-00005c30: 6d61 7869 6d75 6d20 6672 6571 7565 6e63  maximum frequenc
-00005c40: 7920 2848 7a29 0a20 2020 204e 6666 743a  y (Hz).    Nfft:
-00005c50: 2020 2020 6e75 6d62 6572 206f 6620 6672      number of fr
-00005c60: 6571 7565 6e63 7920 706f 696e 7473 2066  equency points f
-00005c70: 6f72 2069 6666 740a 2020 2020 6461 7461  or ifft.    data
-00005c80: 535f 743a 206d 6174 7269 7820 6f66 2064  S_t: matrix of d
-00005c90: 6174 6574 696d 6520 6f62 6a65 6374 2e0a  atetime object..
-00005ca0: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
-00005cb0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-00005cc0: 2d2d 2d2d 2d2d 2d0a 2020 2020 735f 636f  -------.    s_co
-00005cd0: 7272 3a20 3144 206f 7220 3244 206d 6174  rr: 1D or 2D mat
-00005ce0: 7269 7820 6f66 2074 6865 2061 7665 7261  rix of the avera
-00005cf0: 6765 6420 6f72 2073 7562 2d73 7461 636b  ged or sub-stack
-00005d00: 7320 6f66 2063 726f 7373 2d63 6f72 7265  s of cross-corre
-00005d10: 6c61 7469 6f6e 2066 756e 6374 696f 6e73  lation functions
-00005d20: 2069 6e20 7469 6d65 2064 6f6d 6169 6e0a   in time domain.
-00005d30: 2020 2020 745f 636f 7272 3a20 7469 6d65      t_corr: time
-00005d40: 7374 616d 7020 666f 7220 6561 6368 2073  stamp for each s
-00005d50: 7562 2d73 7461 636b 206f 7220 6176 6572  ub-stack or aver
-00005d60: 6167 6564 2066 756e 6374 696f 6e0a 2020  aged function.  
-00005d70: 2020 6e5f 636f 7272 3a20 6e75 6d62 6572    n_corr: number
-00005d80: 206f 6620 696e 636c 7564 6564 2073 6567   of included seg
-00005d90: 6d65 6e74 7320 666f 7220 6561 6368 2073  ments for each s
-00005da0: 7562 2d73 7461 636b 206f 7220 6176 6572  ub-stack or aver
-00005db0: 6167 6564 2066 756e 6374 696f 6e0a 0a20  aged function.. 
-00005dc0: 2020 204d 4f44 4946 4943 4154 494f 4e53     MODIFICATIONS
-00005dd0: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-00005de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-00005df0: 6f75 7470 7574 2074 6865 206c 696e 6561  output the linea
-00005e00: 7220 7374 6163 6b20 6f66 2065 6163 6820  r stack of each 
-00005e10: 7469 6d65 2063 6875 6e6b 2065 7665 6e20  time chunk even 
-00005e20: 7768 656e 2073 7562 7374 6163 6b20 6973  when substack is
-00005e30: 2073 656c 6563 7465 6420 2862 7920 4368   selected (by Ch
-00005e40: 656e 6778 696e 2040 4175 6732 3032 3029  engxin @Aug2020)
-00005e50: 0a20 2020 2022 2222 0a20 2020 2023 202d  .    """.    # -
-00005e60: 2d2d 2d6c 6f61 6420 7061 7261 6d74 6572  ---load paramter
-00005e70: 732d 2d2d 2d0a 2020 2020 6474 203d 2044  s----.    dt = D
-00005e80: 5b22 6474 225d 0a20 2020 206d 6178 6c61  ["dt"].    maxla
-00005e90: 6720 3d20 445b 226d 6178 6c61 6722 5d0a  g = D["maxlag"].
-00005ea0: 2020 2020 6d65 7468 6f64 203d 2044 5b22      method = D["
-00005eb0: 6363 5f6d 6574 686f 6422 5d0a 2020 2020  cc_method"].    
-00005ec0: 6363 5f6c 656e 203d 2044 5b22 6363 5f6c  cc_len = D["cc_l
-00005ed0: 656e 225d 0a20 2020 2073 7562 7374 6163  en"].    substac
-00005ee0: 6b20 3d20 445b 2273 7562 7374 6163 6b22  k = D["substack"
-00005ef0: 5d0a 2020 2020 7375 6273 7461 636b 5f6c  ].    substack_l
-00005f00: 656e 203d 2044 5b22 7375 6273 7461 636b  en = D["substack
-00005f10: 5f6c 656e 225d 0a20 2020 2073 6d6f 6f74  _len"].    smoot
-00005f20: 6873 7065 6374 5f4e 203d 2044 5b22 736d  hspect_N = D["sm
-00005f30: 6f6f 7468 7370 6563 745f 4e22 5d0a 0a20  oothspect_N"].. 
-00005f40: 2020 206e 7769 6e20 3d20 6666 7431 5f73     nwin = fft1_s
-00005f50: 6d6f 6f74 6865 645f 6162 732e 7368 6170  moothed_abs.shap
-00005f60: 655b 305d 0a20 2020 204e 6666 7432 203d  e[0].    Nfft2 =
-00005f70: 2066 6674 315f 736d 6f6f 7468 6564 5f61   fft1_smoothed_a
-00005f80: 6273 2e73 6861 7065 5b31 5d0a 0a20 2020  bs.shape[1]..   
-00005f90: 2023 202d 2d2d 2d2d 2d63 6f6e 7665 7274   # ------convert
-00005fa0: 2061 6c6c 2032 4420 6172 7261 7973 2069   all 2D arrays i
-00005fb0: 6e74 6f20 3144 2074 6f20 7370 6565 6420  nto 1D to speed 
-00005fc0: 7570 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063  up--------.    c
-00005fd0: 6f72 7220 3d20 6e70 2e7a 6572 6f73 286e  orr = np.zeros(n
-00005fe0: 7769 6e20 2a20 4e66 6674 322c 2064 7479  win * Nfft2, dty
-00005ff0: 7065 3d6e 702e 636f 6d70 6c65 7836 3429  pe=np.complex64)
-00006000: 0a20 2020 2063 6f72 7220 3d20 6666 7431  .    corr = fft1
-00006010: 5f73 6d6f 6f74 6865 645f 6162 732e 7265  _smoothed_abs.re
-00006020: 7368 6170 6528 0a20 2020 2020 2020 2066  shape(.        f
-00006030: 6674 315f 736d 6f6f 7468 6564 5f61 6273  ft1_smoothed_abs
-00006040: 2e73 697a 652c 0a20 2020 2029 202a 2066  .size,.    ) * f
-00006050: 6674 322e 7265 7368 6170 6528 0a20 2020  ft2.reshape(.   
-00006060: 2020 2020 2066 6674 322e 7369 7a65 2c0a       fft2.size,.
-00006070: 2020 2020 290a 0a20 2020 2069 6620 6d65      )..    if me
-00006080: 7468 6f64 203d 3d20 2263 6f68 6572 656e  thod == "coheren
-00006090: 6379 223a 0a20 2020 2020 2020 2074 656d  cy":.        tem
-000060a0: 7020 3d20 6d6f 7669 6e67 5f61 7665 280a  p = moving_ave(.
-000060b0: 2020 2020 2020 2020 2020 2020 6e70 2e61              np.a
-000060c0: 6273 280a 2020 2020 2020 2020 2020 2020  bs(.            
-000060d0: 2020 2020 6666 7432 2e72 6573 6861 7065      fft2.reshape
-000060e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000060f0: 2020 2020 2020 6666 7432 2e73 697a 652c        fft2.size,
-00006100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006110: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
-00006120: 2c0a 2020 2020 2020 2020 2020 2020 736d  ,.            sm
-00006130: 6f6f 7468 7370 6563 745f 4e2c 0a20 2020  oothspect_N,.   
-00006140: 2020 2020 2029 0a20 2020 2020 2020 2063       ).        c
-00006150: 6f72 7220 2f3d 2074 656d 700a 2020 2020  orr /= temp.    
-00006160: 636f 7272 203d 2063 6f72 722e 7265 7368  corr = corr.resh
-00006170: 6170 6528 6e77 696e 2c20 4e66 6674 3229  ape(nwin, Nfft2)
-00006180: 0a0a 2020 2020 6966 2073 7562 7374 6163  ..    if substac
-00006190: 6b3a 0a20 2020 2020 2020 2069 6620 7375  k:.        if su
-000061a0: 6273 7461 636b 5f6c 656e 203d 3d20 6363  bstack_len == cc
-000061b0: 5f6c 656e 3a0a 2020 2020 2020 2020 2020  _len:.          
-000061c0: 2020 2320 6368 6f6f 7365 2074 6f20 6b65    # choose to ke
-000061d0: 6570 2061 6c6c 2066 6674 2064 6174 6120  ep all fft data 
-000061e0: 666f 7220 6120 6461 790a 2020 2020 2020  for a day.      
-000061f0: 2020 2020 2020 735f 636f 7272 203d 206e        s_corr = n
-00006200: 702e 7a65 726f 7328 7368 6170 653d 286e  p.zeros(shape=(n
-00006210: 7769 6e2c 204e 6666 7429 2c20 6474 7970  win, Nfft), dtyp
-00006220: 653d 6e70 2e66 6c6f 6174 3332 2920 2023  e=np.float32)  #
-00006230: 2073 7461 636b 6564 2063 6f72 7265 6c61   stacked correla
-00006240: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00006250: 2061 6d70 6d61 7820 3d20 6e70 2e7a 6572   ampmax = np.zer
-00006260: 6f73 286e 7769 6e2c 2064 7479 7065 3d6e  os(nwin, dtype=n
-00006270: 702e 666c 6f61 7433 3229 0a20 2020 2020  p.float32).     
-00006280: 2020 2020 2020 206e 5f63 6f72 7220 3d20         n_corr = 
-00006290: 6e70 2e7a 6572 6f73 286e 7769 6e2c 2064  np.zeros(nwin, d
-000062a0: 7479 7065 3d6e 702e 696e 7431 3629 2020  type=np.int16)  
-000062b0: 2320 6e75 6d62 6572 206f 6620 636f 7272  # number of corr
-000062c0: 656c 6174 696f 6e73 2066 6f72 2065 6163  elations for eac
-000062d0: 6820 7375 6273 7461 636b 0a20 2020 2020  h substack.     
-000062e0: 2020 2020 2020 2074 5f63 6f72 7220 3d20         t_corr = 
-000062f0: 6461 7461 535f 7420 2023 2074 696d 6573  dataS_t  # times
-00006300: 7461 6d70 0a20 2020 2020 2020 2020 2020  tamp.           
-00006310: 2063 7261 7020 3d20 6e70 2e7a 6572 6f73   crap = np.zeros
-00006320: 284e 6666 742c 2064 7479 7065 3d6e 702e  (Nfft, dtype=np.
-00006330: 636f 6d70 6c65 7836 3429 0a20 2020 2020  complex64).     
-00006340: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00006350: 7261 6e67 6528 6e77 696e 293a 0a20 2020  range(nwin):.   
-00006360: 2020 2020 2020 2020 2020 2020 206e 5f63               n_c
-00006370: 6f72 725b 695d 203d 2031 0a20 2020 2020  orr[i] = 1.     
-00006380: 2020 2020 2020 2020 2020 2063 7261 705b             crap[
-00006390: 3a4e 6666 7432 5d20 3d20 636f 7272 5b69  :Nfft2] = corr[i
-000063a0: 2c20 3a5d 0a20 2020 2020 2020 2020 2020  , :].           
-000063b0: 2020 2020 2063 7261 705b 3a4e 6666 7432       crap[:Nfft2
-000063c0: 5d20 3d20 6372 6170 5b3a 4e66 6674 325d  ] = crap[:Nfft2]
-000063d0: 202d 206e 702e 6d65 616e 2863 7261 705b   - np.mean(crap[
-000063e0: 3a4e 6666 7432 5d29 2020 2320 7265 6d6f  :Nfft2])  # remo
-000063f0: 7665 2074 6865 206d 6561 6e20 696e 2066  ve the mean in f
-00006400: 7265 7120 646f 6d61 696e 2028 7370 696b  req domain (spik
-00006410: 6520 6174 2074 3d30 290a 2020 2020 2020  e at t=0).      
-00006420: 2020 2020 2020 2020 2020 6372 6170 5b2d            crap[-
-00006430: 284e 6666 7432 2920 2b20 3120 3a5d 203d  (Nfft2) + 1 :] =
-00006440: 206e 702e 666c 6970 286e 702e 636f 6e6a   np.flip(np.conj
-00006450: 2863 7261 705b 313a 284e 6666 7432 295d  (crap[1:(Nfft2)]
-00006460: 292c 2061 7869 733d 3029 0a20 2020 2020  ), axis=0).     
-00006470: 2020 2020 2020 2020 2020 2063 7261 705b             crap[
-00006480: 305d 203d 2063 6f6d 706c 6578 2830 2c20  0] = complex(0, 
-00006490: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
-000064a0: 2020 2073 5f63 6f72 725b 692c 203a 5d20     s_corr[i, :] 
-000064b0: 3d20 6e70 2e72 6561 6c28 6e70 2e66 6674  = np.real(np.fft
-000064c0: 2e69 6666 7473 6869 6674 2873 6369 7079  .ifftshift(scipy
-000064d0: 2e66 6674 7061 636b 2e69 6666 7428 6372  .fftpack.ifft(cr
-000064e0: 6170 2c20 4e66 6674 2c20 6178 6973 3d30  ap, Nfft, axis=0
-000064f0: 2929 290a 0a20 2020 2020 2020 2020 2020  )))..           
-00006500: 2023 2072 656d 6f76 6520 6162 6e6f 726d   # remove abnorm
-00006510: 616c 2064 6174 610a 2020 2020 2020 2020  al data.        
-00006520: 2020 2020 616d 706d 6178 203d 206e 702e      ampmax = np.
-00006530: 6d61 7828 735f 636f 7272 2c20 6178 6973  max(s_corr, axis
-00006540: 3d31 290a 2020 2020 2020 2020 2020 2020  =1).            
-00006550: 7469 6e64 7820 3d20 6e70 2e77 6865 7265  tindx = np.where
-00006560: 2828 616d 706d 6178 203c 2032 3020 2a20  ((ampmax < 20 * 
-00006570: 6e70 2e6d 6564 6961 6e28 616d 706d 6178  np.median(ampmax
-00006580: 2929 2026 2028 616d 706d 6178 203e 2030  )) & (ampmax > 0
-00006590: 2929 5b30 5d0a 2020 2020 2020 2020 2020  ))[0].          
-000065a0: 2020 735f 636f 7272 203d 2073 5f63 6f72    s_corr = s_cor
-000065b0: 725b 7469 6e64 782c 203a 5d0a 2020 2020  r[tindx, :].    
-000065c0: 2020 2020 2020 2020 745f 636f 7272 203d          t_corr =
-000065d0: 2074 5f63 6f72 725b 7469 6e64 785d 0a20   t_corr[tindx]. 
-000065e0: 2020 2020 2020 2020 2020 206e 5f63 6f72             n_cor
-000065f0: 7220 3d20 6e5f 636f 7272 5b74 696e 6478  r = n_corr[tindx
-00006600: 5d0a 0a20 2020 2020 2020 2065 6c73 653a  ]..        else:
-00006610: 0a20 2020 2020 2020 2020 2020 2023 2067  .            # g
-00006620: 6574 2074 696d 6520 696e 666f 726d 6174  et time informat
-00006630: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00006640: 5474 6f74 616c 203d 2064 6174 6153 5f74  Ttotal = dataS_t
-00006650: 5b2d 315d 202d 2064 6174 6153 5f74 5b30  [-1] - dataS_t[0
-00006660: 5d20 2023 2074 6f74 616c 2064 7572 6174  ]  # total durat
-00006670: 696f 6e20 6f66 2077 6861 7420 7765 2068  ion of what we h
-00006680: 6176 6520 6e6f 770a 2020 2020 2020 2020  ave now.        
-00006690: 2020 2020 7473 7461 7274 203d 2064 6174      tstart = dat
-000066a0: 6153 5f74 5b30 5d0a 0a20 2020 2020 2020  aS_t[0]..       
-000066b0: 2020 2020 206e 7374 6163 6b20 3d20 696e       nstack = in
-000066c0: 7428 6e70 2e72 6f75 6e64 2854 746f 7461  t(np.round(Ttota
-000066d0: 6c20 2f20 7375 6273 7461 636b 5f6c 656e  l / substack_len
-000066e0: 2929 0a20 2020 2020 2020 2020 2020 2061  )).            a
-000066f0: 6d70 6d61 7820 3d20 6e70 2e7a 6572 6f73  mpmax = np.zeros
-00006700: 286e 7374 6163 6b2c 2064 7479 7065 3d6e  (nstack, dtype=n
-00006710: 702e 666c 6f61 7433 3229 0a20 2020 2020  p.float32).     
-00006720: 2020 2020 2020 2073 5f63 6f72 7220 3d20         s_corr = 
-00006730: 6e70 2e7a 6572 6f73 2873 6861 7065 3d28  np.zeros(shape=(
-00006740: 6e73 7461 636b 2c20 4e66 6674 292c 2064  nstack, Nfft), d
-00006750: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00006760: 0a20 2020 2020 2020 2020 2020 206e 5f63  .            n_c
-00006770: 6f72 7220 3d20 6e70 2e7a 6572 6f73 286e  orr = np.zeros(n
-00006780: 7374 6163 6b2c 2064 7479 7065 3d6e 702e  stack, dtype=np.
-00006790: 696e 7429 0a20 2020 2020 2020 2020 2020  int).           
-000067a0: 2074 5f63 6f72 7220 3d20 6e70 2e7a 6572   t_corr = np.zer
-000067b0: 6f73 286e 7374 6163 6b2c 2064 7479 7065  os(nstack, dtype
-000067c0: 3d6e 702e 666c 6f61 7429 0a20 2020 2020  =np.float).     
-000067d0: 2020 2020 2020 2063 7261 7020 3d20 6e70         crap = np
-000067e0: 2e7a 6572 6f73 284e 6666 742c 2064 7479  .zeros(Nfft, dty
-000067f0: 7065 3d6e 702e 636f 6d70 6c65 7836 3429  pe=np.complex64)
-00006800: 0a0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00006810: 7220 6973 7461 636b 2069 6e20 7261 6e67  r istack in rang
-00006820: 6528 6e73 7461 636b 293a 0a20 2020 2020  e(nstack):.     
-00006830: 2020 2020 2020 2020 2020 2023 2066 696e             # fin
-00006840: 6420 7468 6520 696e 6465 7865 7320 6f66  d the indexes of
-00006850: 2061 6c6c 206f 6620 7468 6520 7769 6e64   all of the wind
-00006860: 6f77 7320 7468 6174 2073 7461 7274 206f  ows that start o
-00006870: 7220 656e 6420 7769 7468 696e 0a20 2020  r end within.   
-00006880: 2020 2020 2020 2020 2020 2020 2069 7469               iti
-00006890: 6d65 203d 206e 702e 7768 6572 6528 2864  me = np.where((d
-000068a0: 6174 6153 5f74 203e 3d20 7473 7461 7274  ataS_t >= tstart
-000068b0: 2920 2620 2864 6174 6153 5f74 203c 2074  ) & (dataS_t < t
-000068c0: 7374 6172 7420 2b20 7375 6273 7461 636b  start + substack
-000068d0: 5f6c 656e 2929 5b30 5d0a 2020 2020 2020  _len))[0].      
-000068e0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-000068f0: 2869 7469 6d65 2920 3d3d 2030 3a0a 2020  (itime) == 0:.  
-00006900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006910: 2020 7473 7461 7274 202b 3d20 7375 6273    tstart += subs
-00006920: 7461 636b 5f6c 656e 0a20 2020 2020 2020  tack_len.       
-00006930: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00006940: 7469 6e75 650a 0a20 2020 2020 2020 2020  tinue..         
-00006950: 2020 2020 2020 2063 7261 705b 3a4e 6666         crap[:Nff
-00006960: 7432 5d20 3d20 6e70 2e6d 6561 6e28 636f  t2] = np.mean(co
-00006970: 7272 5b69 7469 6d65 2c20 3a5d 2c20 6178  rr[itime, :], ax
-00006980: 6973 3d30 2920 2023 206c 696e 6561 7220  is=0)  # linear 
-00006990: 6176 6572 6167 6520 6f66 2074 6865 2063  average of the c
-000069a0: 6f72 7265 6c61 7469 6f6e 0a20 2020 2020  orrelation.     
-000069b0: 2020 2020 2020 2020 2020 2063 7261 705b             crap[
-000069c0: 3a4e 6666 7432 5d20 3d20 6372 6170 5b3a  :Nfft2] = crap[:
-000069d0: 4e66 6674 325d 202d 206e 702e 6d65 616e  Nfft2] - np.mean
-000069e0: 2863 7261 705b 3a4e 6666 7432 5d29 2020  (crap[:Nfft2])  
-000069f0: 2320 7265 6d6f 7665 2074 6865 206d 6561  # remove the mea
-00006a00: 6e20 696e 2066 7265 7120 646f 6d61 696e  n in freq domain
-00006a10: 2028 7370 696b 6520 6174 2074 3d30 290a   (spike at t=0).
-00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a30: 6372 6170 5b2d 284e 6666 7432 2920 2b20  crap[-(Nfft2) + 
-00006a40: 3120 3a5d 203d 206e 702e 666c 6970 286e  1 :] = np.flip(n
-00006a50: 702e 636f 6e6a 2863 7261 705b 313a 284e  p.conj(crap[1:(N
-00006a60: 6666 7432 295d 292c 2061 7869 733d 3029  fft2)]), axis=0)
-00006a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006a80: 2063 7261 705b 305d 203d 2063 6f6d 706c   crap[0] = compl
-00006a90: 6578 2830 2c20 3029 0a20 2020 2020 2020  ex(0, 0).       
-00006aa0: 2020 2020 2020 2020 2073 5f63 6f72 725b           s_corr[
-00006ab0: 6973 7461 636b 2c20 3a5d 203d 206e 702e  istack, :] = np.
-00006ac0: 7265 616c 286e 702e 6666 742e 6966 6674  real(np.fft.ifft
-00006ad0: 7368 6966 7428 7363 6970 792e 6666 7470  shift(scipy.fftp
-00006ae0: 6163 6b2e 6966 6674 2863 7261 702c 204e  ack.ifft(crap, N
-00006af0: 6666 742c 2061 7869 733d 3029 2929 0a20  fft, axis=0))). 
-00006b00: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00006b10: 5f63 6f72 725b 6973 7461 636b 5d20 3d20  _corr[istack] = 
-00006b20: 6c65 6e28 6974 696d 6529 2020 2320 6e75  len(itime)  # nu
-00006b30: 6d62 6572 206f 6620 7769 6e64 6f77 7320  mber of windows 
-00006b40: 7374 6163 6b73 0a20 2020 2020 2020 2020  stacks.         
-00006b50: 2020 2020 2020 2074 5f63 6f72 725b 6973         t_corr[is
-00006b60: 7461 636b 5d20 3d20 7473 7461 7274 2020  tack] = tstart  
-00006b70: 2320 7361 7665 2074 6865 2074 696d 6520  # save the time 
-00006b80: 7374 616d 7073 0a20 2020 2020 2020 2020  stamps.         
-00006b90: 2020 2020 2020 2074 7374 6172 7420 2b3d         tstart +=
-00006ba0: 2073 7562 7374 6163 6b5f 6c65 6e0a 2020   substack_len.  
-00006bb0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00006bc0: 7072 696e 7428 2763 6f72 7265 6c61 7469  print('correlati
-00006bd0: 6f6e 2064 6f6e 6520 616e 6420 7374 6163  on done and stac
-00006be0: 6b65 6420 6174 2074 696d 6520 2573 2720  ked at time %s' 
-00006bf0: 2520 7374 7228 745f 636f 7272 5b69 7374  % str(t_corr[ist
-00006c00: 6163 6b5d 2929 0a0a 2020 2020 2020 2020  ack]))..        
-00006c10: 2020 2020 2320 7265 6d6f 7665 2061 626e      # remove abn
-00006c20: 6f72 6d61 6c20 6461 7461 0a20 2020 2020  ormal data.     
-00006c30: 2020 2020 2020 2061 6d70 6d61 7820 3d20         ampmax = 
-00006c40: 6e70 2e6d 6178 2873 5f63 6f72 722c 2061  np.max(s_corr, a
-00006c50: 7869 733d 3129 0a20 2020 2020 2020 2020  xis=1).         
-00006c60: 2020 2074 696e 6478 203d 206e 702e 7768     tindx = np.wh
-00006c70: 6572 6528 2861 6d70 6d61 7820 3c20 3230  ere((ampmax < 20
-00006c80: 202a 206e 702e 6d65 6469 616e 2861 6d70   * np.median(amp
-00006c90: 6d61 7829 2920 2620 2861 6d70 6d61 7820  max)) & (ampmax 
-00006ca0: 3e20 3029 295b 305d 0a20 2020 2020 2020  > 0))[0].       
-00006cb0: 2020 2020 2073 5f63 6f72 7220 3d20 735f       s_corr = s_
-00006cc0: 636f 7272 5b74 696e 6478 2c20 3a5d 0a20  corr[tindx, :]. 
-00006cd0: 2020 2020 2020 2020 2020 2074 5f63 6f72             t_cor
-00006ce0: 7220 3d20 745f 636f 7272 5b74 696e 6478  r = t_corr[tindx
-00006cf0: 5d0a 2020 2020 2020 2020 2020 2020 6e5f  ].            n_
-00006d00: 636f 7272 203d 206e 5f63 6f72 725b 7469  corr = n_corr[ti
-00006d10: 6e64 785d 0a0a 2020 2020 656c 7365 3a0a  ndx]..    else:.
-00006d20: 2020 2020 2020 2020 2320 6176 6572 6167          # averag
-00006d30: 6520 6461 696c 7920 6372 6f73 7320 636f  e daily cross co
-00006d40: 7272 656c 6174 696f 6e20 6675 6e63 7469  rrelation functi
-00006d50: 6f6e 730a 2020 2020 2020 2020 616d 706d  ons.        ampm
-00006d60: 6178 203d 206e 702e 6d61 7828 636f 7272  ax = np.max(corr
-00006d70: 2c20 6178 6973 3d31 290a 2020 2020 2020  , axis=1).      
-00006d80: 2020 7469 6e64 7820 3d20 6e70 2e77 6865    tindx = np.whe
-00006d90: 7265 2828 616d 706d 6178 203c 2032 3020  re((ampmax < 20 
-00006da0: 2a20 6e70 2e6d 6564 6961 6e28 616d 706d  * np.median(ampm
-00006db0: 6178 2929 2026 2028 616d 706d 6178 203e  ax)) & (ampmax >
-00006dc0: 2030 2929 5b30 5d0a 2020 2020 2020 2020   0))[0].        
-00006dd0: 6e5f 636f 7272 203d 206e 7769 6e0a 2020  n_corr = nwin.  
-00006de0: 2020 2020 2020 735f 636f 7272 203d 206e        s_corr = n
-00006df0: 702e 7a65 726f 7328 4e66 6674 2c20 6474  p.zeros(Nfft, dt
-00006e00: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
-00006e10: 2020 2020 2020 2020 745f 636f 7272 203d          t_corr =
-00006e20: 2064 6174 6153 5f74 5b30 5d0a 2020 2020   dataS_t[0].    
-00006e30: 2020 2020 6372 6170 203d 206e 702e 7a65      crap = np.ze
-00006e40: 726f 7328 4e66 6674 2c20 6474 7970 653d  ros(Nfft, dtype=
-00006e50: 6e70 2e63 6f6d 706c 6578 3634 290a 2020  np.complex64).  
-00006e60: 2020 2020 2020 6372 6170 5b3a 4e66 6674        crap[:Nfft
-00006e70: 325d 203d 206e 702e 6d65 616e 2863 6f72  2] = np.mean(cor
-00006e80: 725b 7469 6e64 785d 2c20 6178 6973 3d30  r[tindx], axis=0
-00006e90: 290a 2020 2020 2020 2020 6372 6170 5b3a  ).        crap[:
-00006ea0: 4e66 6674 325d 203d 2063 7261 705b 3a4e  Nfft2] = crap[:N
-00006eb0: 6666 7432 5d20 2d20 6e70 2e6d 6561 6e28  fft2] - np.mean(
-00006ec0: 6372 6170 5b3a 4e66 6674 325d 2c20 6178  crap[:Nfft2], ax
-00006ed0: 6973 3d30 290a 2020 2020 2020 2020 6372  is=0).        cr
-00006ee0: 6170 5b2d 284e 6666 7432 2920 2b20 3120  ap[-(Nfft2) + 1 
-00006ef0: 3a5d 203d 206e 702e 666c 6970 286e 702e  :] = np.flip(np.
-00006f00: 636f 6e6a 2863 7261 705b 313a 284e 6666  conj(crap[1:(Nff
-00006f10: 7432 295d 292c 2061 7869 733d 3029 0a20  t2)]), axis=0). 
-00006f20: 2020 2020 2020 2073 5f63 6f72 7220 3d20         s_corr = 
-00006f30: 6e70 2e72 6561 6c28 6e70 2e66 6674 2e69  np.real(np.fft.i
-00006f40: 6666 7473 6869 6674 2873 6369 7079 2e66  fftshift(scipy.f
-00006f50: 6674 7061 636b 2e69 6666 7428 6372 6170  ftpack.ifft(crap
-00006f60: 2c20 4e66 6674 2c20 6178 6973 3d30 2929  , Nfft, axis=0))
-00006f70: 290a 0a20 2020 2023 2074 7269 6d20 7468  )..    # trim th
-00006f80: 6520 4343 4673 2069 6e20 5b2d 6d61 786c  e CCFs in [-maxl
-00006f90: 6167 206d 6178 6c61 675d 0a20 2020 2074  ag maxlag].    t
-00006fa0: 203d 206e 702e 6172 616e 6765 282d 4e66   = np.arange(-Nf
-00006fb0: 6674 3220 2b20 312c 204e 6666 7432 2920  ft2 + 1, Nfft2) 
-00006fc0: 2a20 6474 0a20 2020 2069 6e64 203d 206e  * dt.    ind = n
-00006fd0: 702e 7768 6572 6528 6e70 2e61 6273 2874  p.where(np.abs(t
-00006fe0: 2920 3c3d 206d 6178 6c61 6729 5b30 5d0a  ) <= maxlag)[0].
-00006ff0: 2020 2020 6966 2073 5f63 6f72 722e 6e64      if s_corr.nd
-00007000: 696d 203d 3d20 313a 0a20 2020 2020 2020  im == 1:.       
-00007010: 2073 5f63 6f72 7220 3d20 735f 636f 7272   s_corr = s_corr
-00007020: 5b69 6e64 5d0a 2020 2020 656c 6966 2073  [ind].    elif s
-00007030: 5f63 6f72 722e 6e64 696d 203d 3d20 323a  _corr.ndim == 2:
-00007040: 0a20 2020 2020 2020 2073 5f63 6f72 7220  .        s_corr 
-00007050: 3d20 735f 636f 7272 5b3a 2c20 696e 645d  = s_corr[:, ind]
-00007060: 0a20 2020 2072 6574 7572 6e20 735f 636f  .    return s_co
-00007070: 7272 2c20 745f 636f 7272 2c20 6e5f 636f  rr, t_corr, n_co
-00007080: 7272 0a0a 0a64 6566 2063 6f72 7265 6c61  rr...def correla
-00007090: 7465 5f6e 6f6e 6c69 6e65 6172 5f73 7461  te_nonlinear_sta
-000070a0: 636b 2866 6674 315f 736d 6f6f 7468 6564  ck(fft1_smoothed
-000070b0: 5f61 6273 2c20 6666 7432 2c20 442c 204e  _abs, fft2, D, N
-000070c0: 6666 742c 2064 6174 6153 5f74 293a 0a20  fft, dataS_t):. 
-000070d0: 2020 2022 2222 0a20 2020 2074 6869 7320     """.    this 
-000070e0: 6675 6e63 7469 6f6e 2064 6f65 7320 7468  function does th
-000070f0: 6520 6372 6f73 732d 636f 7272 656c 6174  e cross-correlat
-00007100: 696f 6e20 696e 2066 7265 7120 646f 6d61  ion in freq doma
-00007110: 696e 2061 6e64 2068 6173 2074 6865 206f  in and has the o
-00007120: 7074 696f 6e20 746f 206b 6565 7020 7375  ption to keep su
-00007130: 622d 7374 6163 6b73 206f 660a 2020 2020  b-stacks of.    
-00007140: 7468 6520 6372 6f73 732d 636f 7272 656c  the cross-correl
-00007150: 6174 696f 6e20 6966 206e 6565 6465 642e  ation if needed.
-00007160: 2069 7420 7461 6b65 7320 6164 7661 6e74   it takes advant
-00007170: 6167 6520 6f66 2074 6865 206c 696e 6561  age of the linea
-00007180: 7220 7265 6c61 7469 6f6e 7368 6970 206f  r relationship o
-00007190: 6620 6966 6674 2c20 736f 2074 6861 740a  f ifft, so that.
-000071a0: 2020 2020 7374 6163 6b69 6e67 2069 7320      stacking is 
-000071b0: 7065 7266 6f72 6d65 6420 696e 2073 7065  performed in spe
-000071c0: 6374 7275 6d20 646f 6d61 696e 2066 6972  ctrum domain fir
-000071d0: 7374 2074 6f20 7265 6475 6365 2074 6865  st to reduce the
-000071e0: 2074 6f74 616c 206e 756d 6265 7220 6f66   total number of
-000071f0: 2069 6666 742e 2028 7573 6564 2069 6e20   ifft. (used in 
-00007200: 5331 290a 2020 2020 5041 5241 4d45 5445  S1).    PARAMETE
-00007210: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
-00007220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00007230: 2020 6666 7431 5f73 6d6f 6f74 6865 645f    fft1_smoothed_
-00007240: 6162 733a 2073 6d6f 6f74 6865 6420 706f  abs: smoothed po
-00007250: 7765 7220 7370 6563 7472 616c 2064 656e  wer spectral den
-00007260: 7369 7479 206f 6620 7468 6520 4646 5420  sity of the FFT 
-00007270: 666f 7220 7468 6520 736f 7572 6365 2073  for the source s
-00007280: 7461 7469 6f6e 0a20 2020 2066 6674 323a  tation.    fft2:
-00007290: 2072 6177 2046 4654 2073 7065 6374 7275   raw FFT spectru
-000072a0: 6d20 6f66 2074 6865 2072 6563 6569 7665  m of the receive
-000072b0: 7220 7374 6174 696f 6e0a 2020 2020 443a  r station.    D:
-000072c0: 2064 6963 7469 6f6e 6172 7920 636f 6e74   dictionary cont
-000072d0: 6169 6e69 6e67 2066 6f6c 6c6f 7769 6e67  aining following
-000072e0: 2070 6172 616d 6574 6572 733a 0a20 2020   parameters:.   
-000072f0: 2020 2020 206d 6178 6c61 673a 2020 6d61       maxlag:  ma
-00007300: 7869 6d75 6d20 6c61 6773 2074 6f20 6b65  ximum lags to ke
-00007310: 6570 2069 6e20 7468 6520 6372 6f73 7320  ep in the cross 
-00007320: 636f 7272 656c 6174 696f 6e0a 2020 2020  correlation.    
-00007330: 2020 2020 6474 3a20 2020 2020 2073 616d      dt:      sam
-00007340: 706c 696e 6720 7261 7465 2028 696e 2073  pling rate (in s
-00007350: 290a 2020 2020 2020 2020 6e77 696e 3a20  ).        nwin: 
-00007360: 2020 206e 756d 6265 7220 6f66 2073 6567     number of seg
-00007370: 6d65 6e74 7320 696e 2074 6865 2032 4420  ments in the 2D 
-00007380: 6d61 7472 6978 0a20 2020 2020 2020 206d  matrix.        m
-00007390: 6574 686f 643a 2020 6372 6f73 732d 636f  ethod:  cross-co
-000073a0: 7272 656c 6174 696f 6e20 6d65 7468 6f64  rrelation method
-000073b0: 7320 7365 6c65 6374 6564 2062 7920 7468  s selected by th
-000073c0: 6520 7573 6572 0a20 2020 2020 2020 2066  e user.        f
-000073d0: 7265 716d 696e 3a20 6d69 6e69 6d75 6d20  reqmin: minimum 
-000073e0: 6672 6571 7565 6e63 7920 2848 7a29 0a20  frequency (Hz). 
-000073f0: 2020 2020 2020 2066 7265 716d 6178 3a20         freqmax: 
-00007400: 6d61 7869 6d75 6d20 6672 6571 7565 6e63  maximum frequenc
-00007410: 7920 2848 7a29 0a20 2020 204e 6666 743a  y (Hz).    Nfft:
-00007420: 2020 2020 6e75 6d62 6572 206f 6620 6672      number of fr
-00007430: 6571 7565 6e63 7920 706f 696e 7473 2066  equency points f
-00007440: 6f72 2069 6666 740a 2020 2020 6461 7461  or ifft.    data
-00007450: 535f 743a 206d 6174 7269 7820 6f66 2064  S_t: matrix of d
-00007460: 6174 6574 696d 6520 6f62 6a65 6374 2e0a  atetime object..
-00007470: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
-00007480: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-00007490: 2d2d 2d2d 2d2d 0a20 2020 2073 5f63 6f72  ------.    s_cor
-000074a0: 723a 2031 4420 6f72 2032 4420 6d61 7472  r: 1D or 2D matr
-000074b0: 6978 206f 6620 7468 6520 6176 6572 6167  ix of the averag
-000074c0: 6564 206f 7220 7375 622d 7374 6163 6b73  ed or sub-stacks
-000074d0: 206f 6620 6372 6f73 732d 636f 7272 656c   of cross-correl
-000074e0: 6174 696f 6e20 6675 6e63 7469 6f6e 7320  ation functions 
-000074f0: 696e 2074 696d 6520 646f 6d61 696e 0a20  in time domain. 
-00007500: 2020 2074 5f63 6f72 723a 2074 696d 6573     t_corr: times
-00007510: 7461 6d70 2066 6f72 2065 6163 6820 7375  tamp for each su
-00007520: 622d 7374 6163 6b20 6f72 2061 7665 7261  b-stack or avera
-00007530: 6765 6420 6675 6e63 7469 6f6e 0a20 2020  ged function.   
-00007540: 206e 5f63 6f72 723a 206e 756d 6265 7220   n_corr: number 
-00007550: 6f66 2069 6e63 6c75 6465 6420 7365 676d  of included segm
-00007560: 656e 7473 2066 6f72 2065 6163 6820 7375  ents for each su
-00007570: 622d 7374 6163 6b20 6f72 2061 7665 7261  b-stack or avera
-00007580: 6765 6420 6675 6e63 7469 6f6e 0a20 2020  ged function.   
-00007590: 2022 2222 0a20 2020 2023 202d 2d2d 2d6c   """.    # ----l
-000075a0: 6f61 6420 7061 7261 6d74 6572 732d 2d2d  oad paramters---
-000075b0: 2d0a 2020 2020 6474 203d 2044 5b22 6474  -.    dt = D["dt
-000075c0: 225d 0a20 2020 206d 6178 6c61 6720 3d20  "].    maxlag = 
-000075d0: 445b 226d 6178 6c61 6722 5d0a 2020 2020  D["maxlag"].    
-000075e0: 6d65 7468 6f64 203d 2044 5b22 6363 5f6d  method = D["cc_m
-000075f0: 6574 686f 6422 5d0a 2020 2020 6363 5f6c  ethod"].    cc_l
-00007600: 656e 203d 2044 5b22 6363 5f6c 656e 225d  en = D["cc_len"]
-00007610: 0a20 2020 2073 7562 7374 6163 6b20 3d20  .    substack = 
-00007620: 445b 2273 7562 7374 6163 6b22 5d0a 2020  D["substack"].  
-00007630: 2020 7374 6163 6b5f 6d65 7468 6f64 203d    stack_method =
-00007640: 2044 5b22 7374 6163 6b5f 6d65 7468 6f64   D["stack_method
-00007650: 225d 0a20 2020 2073 7562 7374 6163 6b5f  "].    substack_
-00007660: 6c65 6e20 3d20 445b 2273 7562 7374 6163  len = D["substac
-00007670: 6b5f 6c65 6e22 5d0a 2020 2020 736d 6f6f  k_len"].    smoo
-00007680: 7468 7370 6563 745f 4e20 3d20 445b 2273  thspect_N = D["s
-00007690: 6d6f 6f74 6873 7065 6374 5f4e 225d 0a0a  moothspect_N"]..
-000076a0: 2020 2020 6e77 696e 203d 2066 6674 315f      nwin = fft1_
-000076b0: 736d 6f6f 7468 6564 5f61 6273 2e73 6861  smoothed_abs.sha
-000076c0: 7065 5b30 5d0a 2020 2020 4e66 6674 3220  pe[0].    Nfft2 
-000076d0: 3d20 6666 7431 5f73 6d6f 6f74 6865 645f  = fft1_smoothed_
-000076e0: 6162 732e 7368 6170 655b 315d 0a0a 2020  abs.shape[1]..  
-000076f0: 2020 2320 2d2d 2d2d 2d2d 636f 6e76 6572    # ------conver
-00007700: 7420 616c 6c20 3244 2061 7272 6179 7320  t all 2D arrays 
-00007710: 696e 746f 2031 4420 746f 2073 7065 6564  into 1D to speed
-00007720: 2075 702d 2d2d 2d2d 2d2d 2d0a 2020 2020   up--------.    
-00007730: 636f 7272 203d 206e 702e 7a65 726f 7328  corr = np.zeros(
-00007740: 6e77 696e 202a 204e 6666 7432 2c20 6474  nwin * Nfft2, dt
-00007750: 7970 653d 6e70 2e63 6f6d 706c 6578 3634  ype=np.complex64
-00007760: 290a 2020 2020 636f 7272 203d 2066 6674  ).    corr = fft
-00007770: 315f 736d 6f6f 7468 6564 5f61 6273 2e72  1_smoothed_abs.r
-00007780: 6573 6861 7065 280a 2020 2020 2020 2020  eshape(.        
-00007790: 6666 7431 5f73 6d6f 6f74 6865 645f 6162  fft1_smoothed_ab
-000077a0: 732e 7369 7a65 2c0a 2020 2020 2920 2a20  s.size,.    ) * 
-000077b0: 6666 7432 2e72 6573 6861 7065 280a 2020  fft2.reshape(.  
-000077c0: 2020 2020 2020 6666 7432 2e73 697a 652c        fft2.size,
-000077d0: 0a20 2020 2029 0a0a 2020 2020 2320 6e6f  .    )..    # no
-000077e0: 726d 616c 697a 6520 6279 2072 6563 6569  rmalize by recei
-000077f0: 7665 7220 7370 6563 7472 616c 2066 6f72  ver spectral for
-00007800: 2063 6f68 6572 656e 6379 0a20 2020 2069   coherency.    i
-00007810: 6620 6d65 7468 6f64 203d 3d20 2263 6f68  f method == "coh
-00007820: 6572 656e 6379 223a 0a20 2020 2020 2020  erency":.       
-00007830: 2074 656d 7020 3d20 6d6f 7669 6e67 5f61   temp = moving_a
-00007840: 7665 280a 2020 2020 2020 2020 2020 2020  ve(.            
-00007850: 6e70 2e61 6273 280a 2020 2020 2020 2020  np.abs(.        
-00007860: 2020 2020 2020 2020 6666 7432 2e72 6573          fft2.res
-00007870: 6861 7065 280a 2020 2020 2020 2020 2020  hape(.          
-00007880: 2020 2020 2020 2020 2020 6666 7432 2e73            fft2.s
-00007890: 697a 652c 0a20 2020 2020 2020 2020 2020  ize,.           
-000078a0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-000078b0: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-000078c0: 2020 736d 6f6f 7468 7370 6563 745f 4e2c    smoothspect_N,
-000078d0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
-000078e0: 2020 2063 6f72 7220 2f3d 2074 656d 700a     corr /= temp.
-000078f0: 2020 2020 636f 7272 203d 2063 6f72 722e      corr = corr.
-00007900: 7265 7368 6170 6528 6e77 696e 2c20 4e66  reshape(nwin, Nf
-00007910: 6674 3229 0a0a 2020 2020 2320 7472 616e  ft2)..    # tran
-00007920: 7366 6f72 6d20 6261 636b 2074 6f20 7469  sform back to ti
-00007930: 6d65 2064 6f6d 6169 6e20 7761 7665 666f  me domain wavefo
-00007940: 726d 730a 2020 2020 735f 636f 7272 203d  rms.    s_corr =
-00007950: 206e 702e 7a65 726f 7328 7368 6170 653d   np.zeros(shape=
-00007960: 286e 7769 6e2c 204e 6666 7429 2c20 6474  (nwin, Nfft), dt
-00007970: 7970 653d 6e70 2e66 6c6f 6174 3332 2920  ype=np.float32) 
-00007980: 2023 2073 7461 636b 6564 2063 6f72 7265   # stacked corre
-00007990: 6c61 7469 6f6e 0a20 2020 2061 6d70 6d61  lation.    ampma
-000079a0: 7820 3d20 6e70 2e7a 6572 6f73 286e 7769  x = np.zeros(nwi
-000079b0: 6e2c 2064 7479 7065 3d6e 702e 666c 6f61  n, dtype=np.floa
-000079c0: 7433 3229 0a20 2020 206e 5f63 6f72 7220  t32).    n_corr 
-000079d0: 3d20 6e70 2e7a 6572 6f73 286e 7769 6e2c  = np.zeros(nwin,
-000079e0: 2064 7479 7065 3d6e 702e 696e 7431 3629   dtype=np.int16)
-000079f0: 2020 2320 6e75 6d62 6572 206f 6620 636f    # number of co
-00007a00: 7272 656c 6174 696f 6e73 2066 6f72 2065  rrelations for e
-00007a10: 6163 6820 7375 6273 7461 636b 0a20 2020  ach substack.   
-00007a20: 2074 5f63 6f72 7220 3d20 6461 7461 535f   t_corr = dataS_
-00007a30: 7420 2023 2074 696d 6573 7461 6d70 0a20  t  # timestamp. 
-00007a40: 2020 2063 7261 7020 3d20 6e70 2e7a 6572     crap = np.zer
-00007a50: 6f73 284e 6666 742c 2064 7479 7065 3d6e  os(Nfft, dtype=n
-00007a60: 702e 636f 6d70 6c65 7836 3429 0a20 2020  p.complex64).   
-00007a70: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00007a80: 6e77 696e 293a 0a20 2020 2020 2020 206e  nwin):.        n
-00007a90: 5f63 6f72 725b 695d 203d 2031 0a20 2020  _corr[i] = 1.   
-00007aa0: 2020 2020 2063 7261 705b 3a4e 6666 7432       crap[:Nfft2
-00007ab0: 5d20 3d20 636f 7272 5b69 2c20 3a5d 0a20  ] = corr[i, :]. 
-00007ac0: 2020 2020 2020 2063 7261 705b 3a4e 6666         crap[:Nff
-00007ad0: 7432 5d20 3d20 6372 6170 5b3a 4e66 6674  t2] = crap[:Nfft
-00007ae0: 325d 202d 206e 702e 6d65 616e 2863 7261  2] - np.mean(cra
-00007af0: 705b 3a4e 6666 7432 5d29 2020 2320 7265  p[:Nfft2])  # re
-00007b00: 6d6f 7665 2074 6865 206d 6561 6e20 696e  move the mean in
-00007b10: 2066 7265 7120 646f 6d61 696e 2028 7370   freq domain (sp
-00007b20: 696b 6520 6174 2074 3d30 290a 2020 2020  ike at t=0).    
-00007b30: 2020 2020 6372 6170 5b2d 284e 6666 7432      crap[-(Nfft2
-00007b40: 2920 2b20 3120 3a5d 203d 206e 702e 666c  ) + 1 :] = np.fl
-00007b50: 6970 286e 702e 636f 6e6a 2863 7261 705b  ip(np.conj(crap[
-00007b60: 313a 284e 6666 7432 295d 292c 2061 7869  1:(Nfft2)]), axi
-00007b70: 733d 3029 0a20 2020 2020 2020 2063 7261  s=0).        cra
-00007b80: 705b 305d 203d 2063 6f6d 706c 6578 2830  p[0] = complex(0
-00007b90: 2c20 3029 0a20 2020 2020 2020 2073 5f63  , 0).        s_c
-00007ba0: 6f72 725b 692c 203a 5d20 3d20 6e70 2e72  orr[i, :] = np.r
-00007bb0: 6561 6c28 6e70 2e66 6674 2e69 6666 7473  eal(np.fft.iffts
-00007bc0: 6869 6674 2873 6369 7079 2e66 6674 7061  hift(scipy.fftpa
-00007bd0: 636b 2e69 6666 7428 6372 6170 2c20 4e66  ck.ifft(crap, Nf
-00007be0: 6674 2c20 6178 6973 3d30 2929 290a 0a20  ft, axis=0))).. 
-00007bf0: 2020 206e 735f 636f 7272 203d 2073 5f63     ns_corr = s_c
-00007c00: 6f72 720a 2020 2020 666f 7220 6969 6920  orr.    for iii 
-00007c10: 696e 2072 616e 6765 286e 735f 636f 7272  in range(ns_corr
-00007c20: 2e73 6861 7065 5b30 5d29 3a0a 2020 2020  .shape[0]):.    
-00007c30: 2020 2020 6e73 5f63 6f72 725b 6969 695d      ns_corr[iii]
-00007c40: 202f 3d20 6e70 2e6d 6178 286e 702e 6162   /= np.max(np.ab
-00007c50: 7328 6e73 5f63 6f72 725b 6969 695d 2929  s(ns_corr[iii]))
-00007c60: 0a0a 2020 2020 6966 2073 7562 7374 6163  ..    if substac
-00007c70: 6b3a 0a20 2020 2020 2020 2069 6620 7375  k:.        if su
-00007c80: 6273 7461 636b 5f6c 656e 203d 3d20 6363  bstack_len == cc
-00007c90: 5f6c 656e 3a0a 2020 2020 2020 2020 2020  _len:.          
-00007ca0: 2020 2320 7265 6d6f 7665 2061 626e 6f72    # remove abnor
-00007cb0: 6d61 6c20 6461 7461 0a20 2020 2020 2020  mal data.       
-00007cc0: 2020 2020 2061 6d70 6d61 7820 3d20 6e70       ampmax = np
-00007cd0: 2e6d 6178 2873 5f63 6f72 722c 2061 7869  .max(s_corr, axi
-00007ce0: 733d 3129 0a20 2020 2020 2020 2020 2020  s=1).           
-00007cf0: 2074 696e 6478 203d 206e 702e 7768 6572   tindx = np.wher
-00007d00: 6528 2861 6d70 6d61 7820 3c20 3230 202a  e((ampmax < 20 *
-00007d10: 206e 702e 6d65 6469 616e 2861 6d70 6d61   np.median(ampma
-00007d20: 7829 2920 2620 2861 6d70 6d61 7820 3e20  x)) & (ampmax > 
-00007d30: 3029 295b 305d 0a20 2020 2020 2020 2020  0))[0].         
-00007d40: 2020 2073 5f63 6f72 7220 3d20 735f 636f     s_corr = s_co
-00007d50: 7272 5b74 696e 6478 2c20 3a5d 0a20 2020  rr[tindx, :].   
-00007d60: 2020 2020 2020 2020 2074 5f63 6f72 7220           t_corr 
-00007d70: 3d20 745f 636f 7272 5b74 696e 6478 5d0a  = t_corr[tindx].
-00007d80: 2020 2020 2020 2020 2020 2020 6e5f 636f              n_co
-00007d90: 7272 203d 206e 5f63 6f72 725b 7469 6e64  rr = n_corr[tind
-00007da0: 785d 0a0a 2020 2020 2020 2020 656c 7365  x]..        else
-00007db0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00007dc0: 6765 7420 7469 6d65 2069 6e66 6f72 6d61  get time informa
-00007dd0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00007de0: 2054 746f 7461 6c20 3d20 6461 7461 535f   Ttotal = dataS_
-00007df0: 745b 2d31 5d20 2d20 6461 7461 535f 745b  t[-1] - dataS_t[
-00007e00: 305d 2020 2320 746f 7461 6c20 6475 7261  0]  # total dura
-00007e10: 7469 6f6e 206f 6620 7768 6174 2077 6520  tion of what we 
-00007e20: 6861 7665 206e 6f77 0a20 2020 2020 2020  have now.       
-00007e30: 2020 2020 2074 7374 6172 7420 3d20 6461       tstart = da
-00007e40: 7461 535f 745b 305d 0a0a 2020 2020 2020  taS_t[0]..      
-00007e50: 2020 2020 2020 6e73 7461 636b 203d 2069        nstack = i
-00007e60: 6e74 286e 702e 726f 756e 6428 5474 6f74  nt(np.round(Ttot
-00007e70: 616c 202f 2073 7562 7374 6163 6b5f 6c65  al / substack_le
-00007e80: 6e29 290a 2020 2020 2020 2020 2020 2020  n)).            
-00007e90: 616d 706d 6178 203d 206e 702e 7a65 726f  ampmax = np.zero
-00007ea0: 7328 6e73 7461 636b 2c20 6474 7970 653d  s(nstack, dtype=
-00007eb0: 6e70 2e66 6c6f 6174 3332 290a 2020 2020  np.float32).    
-00007ec0: 2020 2020 2020 2020 735f 636f 7272 203d          s_corr =
-00007ed0: 206e 702e 7a65 726f 7328 7368 6170 653d   np.zeros(shape=
-00007ee0: 286e 7374 6163 6b2c 204e 6666 7429 2c20  (nstack, Nfft), 
-00007ef0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-00007f00: 290a 2020 2020 2020 2020 2020 2020 6e5f  ).            n_
-00007f10: 636f 7272 203d 206e 702e 7a65 726f 7328  corr = np.zeros(
-00007f20: 6e73 7461 636b 2c20 6474 7970 653d 6e70  nstack, dtype=np
-00007f30: 2e69 6e74 290a 2020 2020 2020 2020 2020  .int).          
-00007f40: 2020 745f 636f 7272 203d 206e 702e 7a65    t_corr = np.ze
-00007f50: 726f 7328 6e73 7461 636b 2c20 6474 7970  ros(nstack, dtyp
-00007f60: 653d 6e70 2e66 6c6f 6174 290a 2020 2020  e=np.float).    
-00007f70: 2020 2020 2020 2020 6372 6170 203d 206e          crap = n
-00007f80: 702e 7a65 726f 7328 4e66 6674 2c20 6474  p.zeros(Nfft, dt
-00007f90: 7970 653d 6e70 2e63 6f6d 706c 6578 3634  ype=np.complex64
-00007fa0: 290a 0a20 2020 2020 2020 2020 2020 2066  )..            f
-00007fb0: 6f72 2069 7374 6163 6b20 696e 2072 616e  or istack in ran
-00007fc0: 6765 286e 7374 6163 6b29 3a0a 2020 2020  ge(nstack):.    
-00007fd0: 2020 2020 2020 2020 2020 2020 2320 6669              # fi
-00007fe0: 6e64 2074 6865 2069 6e64 6578 6573 206f  nd the indexes o
-00007ff0: 6620 616c 6c20 6f66 2074 6865 2077 696e  f all of the win
-00008000: 646f 7773 2074 6861 7420 7374 6172 7420  dows that start 
-00008010: 6f72 2065 6e64 2077 6974 6869 6e0a 2020  or end within.  
-00008020: 2020 2020 2020 2020 2020 2020 2020 6974                it
-00008030: 696d 6520 3d20 6e70 2e77 6865 7265 2828  ime = np.where((
-00008040: 6461 7461 535f 7420 3e3d 2074 7374 6172  dataS_t >= tstar
-00008050: 7429 2026 2028 6461 7461 535f 7420 3c20  t) & (dataS_t < 
-00008060: 7473 7461 7274 202b 2073 7562 7374 6163  tstart + substac
-00008070: 6b5f 6c65 6e29 295b 305d 0a20 2020 2020  k_len))[0].     
-00008080: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-00008090: 6e28 6974 696d 6529 203d 3d20 303a 0a20  n(itime) == 0:. 
-000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080b0: 2020 2074 7374 6172 7420 2b3d 2073 7562     tstart += sub
-000080c0: 7374 6163 6b5f 6c65 6e0a 2020 2020 2020  stack_len.      
-000080d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000080e0: 6e74 696e 7565 0a0a 2020 2020 2020 2020  ntinue..        
-000080f0: 2020 2020 2020 2020 6372 6170 5b3a 4e66          crap[:Nf
-00008100: 6674 325d 203d 206e 702e 6d65 616e 2863  ft2] = np.mean(c
-00008110: 6f72 725b 6974 696d 652c 203a 5d2c 2061  orr[itime, :], a
-00008120: 7869 733d 3029 2020 2320 6c69 6e65 6172  xis=0)  # linear
-00008130: 2061 7665 7261 6765 206f 6620 7468 6520   average of the 
-00008140: 636f 7272 656c 6174 696f 6e0a 2020 2020  correlation.    
-00008150: 2020 2020 2020 2020 2020 2020 6372 6170              crap
-00008160: 5b3a 4e66 6674 325d 203d 2063 7261 705b  [:Nfft2] = crap[
-00008170: 3a4e 6666 7432 5d20 2d20 6e70 2e6d 6561  :Nfft2] - np.mea
-00008180: 6e28 6372 6170 5b3a 4e66 6674 325d 2920  n(crap[:Nfft2]) 
-00008190: 2023 2072 656d 6f76 6520 7468 6520 6d65   # remove the me
-000081a0: 616e 2069 6e20 6672 6571 2064 6f6d 6169  an in freq domai
-000081b0: 6e20 2873 7069 6b65 2061 7420 743d 3029  n (spike at t=0)
-000081c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000081d0: 2063 7261 705b 2d28 4e66 6674 3229 202b   crap[-(Nfft2) +
-000081e0: 2031 203a 5d20 3d20 6e70 2e66 6c69 7028   1 :] = np.flip(
-000081f0: 6e70 2e63 6f6e 6a28 6372 6170 5b31 3a28  np.conj(crap[1:(
-00008200: 4e66 6674 3229 5d29 2c20 6178 6973 3d30  Nfft2)]), axis=0
-00008210: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008220: 2020 6372 6170 5b30 5d20 3d20 636f 6d70    crap[0] = comp
-00008230: 6c65 7828 302c 2030 290a 2020 2020 2020  lex(0, 0).      
-00008240: 2020 2020 2020 2020 2020 735f 636f 7272            s_corr
-00008250: 5b69 7374 6163 6b2c 203a 5d20 3d20 6e70  [istack, :] = np
-00008260: 2e72 6561 6c28 6e70 2e66 6674 2e69 6666  .real(np.fft.iff
-00008270: 7473 6869 6674 2873 6369 7079 2e66 6674  tshift(scipy.fft
-00008280: 7061 636b 2e69 6666 7428 6372 6170 2c20  pack.ifft(crap, 
-00008290: 4e66 6674 2c20 6178 6973 3d30 2929 290a  Nfft, axis=0))).
-000082a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082b0: 6e5f 636f 7272 5b69 7374 6163 6b5d 203d  n_corr[istack] =
-000082c0: 206c 656e 2869 7469 6d65 2920 2023 206e   len(itime)  # n
-000082d0: 756d 6265 7220 6f66 2077 696e 646f 7773  umber of windows
-000082e0: 2073 7461 636b 730a 2020 2020 2020 2020   stacks.        
-000082f0: 2020 2020 2020 2020 745f 636f 7272 5b69          t_corr[i
-00008300: 7374 6163 6b5d 203d 2074 7374 6172 7420  stack] = tstart 
-00008310: 2023 2073 6176 6520 7468 6520 7469 6d65   # save the time
-00008320: 2073 7461 6d70 730a 2020 2020 2020 2020   stamps.        
-00008330: 2020 2020 2020 2020 7473 7461 7274 202b          tstart +
-00008340: 3d20 7375 6273 7461 636b 5f6c 656e 0a20  = substack_len. 
-00008350: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00008360: 2070 7269 6e74 2827 636f 7272 656c 6174   print('correlat
-00008370: 696f 6e20 646f 6e65 2061 6e64 2073 7461  ion done and sta
-00008380: 636b 6564 2061 7420 7469 6d65 2025 7327  cked at time %s'
-00008390: 2025 2073 7472 2874 5f63 6f72 725b 6973   % str(t_corr[is
-000083a0: 7461 636b 5d29 290a 0a20 2020 2020 2020  tack]))..       
-000083b0: 2020 2020 2023 2072 656d 6f76 6520 6162       # remove ab
-000083c0: 6e6f 726d 616c 2064 6174 610a 2020 2020  normal data.    
-000083d0: 2020 2020 2020 2020 616d 706d 6178 203d          ampmax =
-000083e0: 206e 702e 6d61 7828 735f 636f 7272 2c20   np.max(s_corr, 
-000083f0: 6178 6973 3d31 290a 2020 2020 2020 2020  axis=1).        
-00008400: 2020 2020 7469 6e64 7820 3d20 6e70 2e77      tindx = np.w
-00008410: 6865 7265 2828 616d 706d 6178 203c 2032  here((ampmax < 2
-00008420: 3020 2a20 6e70 2e6d 6564 6961 6e28 616d  0 * np.median(am
-00008430: 706d 6178 2929 2026 2028 616d 706d 6178  pmax)) & (ampmax
-00008440: 203e 2030 2929 5b30 5d0a 2020 2020 2020   > 0))[0].      
-00008450: 2020 2020 2020 735f 636f 7272 203d 2073        s_corr = s
-00008460: 5f63 6f72 725b 7469 6e64 782c 203a 5d0a  _corr[tindx, :].
-00008470: 2020 2020 2020 2020 2020 2020 745f 636f              t_co
-00008480: 7272 203d 2074 5f63 6f72 725b 7469 6e64  rr = t_corr[tind
-00008490: 785d 0a20 2020 2020 2020 2020 2020 206e  x].            n
-000084a0: 5f63 6f72 7220 3d20 6e5f 636f 7272 5b74  _corr = n_corr[t
-000084b0: 696e 6478 5d0a 0a20 2020 2065 6c73 653a  indx]..    else:
-000084c0: 0a20 2020 2020 2020 2023 2061 7665 7261  .        # avera
-000084d0: 6765 2064 6169 6c79 2063 726f 7373 2063  ge daily cross c
-000084e0: 6f72 7265 6c61 7469 6f6e 2066 756e 6374  orrelation funct
-000084f0: 696f 6e73 0a20 2020 2020 2020 2069 6620  ions.        if 
-00008500: 7374 6163 6b5f 6d65 7468 6f64 203d 3d20  stack_method == 
-00008510: 226c 696e 6561 7222 3a0a 2020 2020 2020  "linear":.      
-00008520: 2020 2020 2020 616d 706d 6178 203d 206e        ampmax = n
-00008530: 702e 6d61 7828 735f 636f 7272 2c20 6178  p.max(s_corr, ax
-00008540: 6973 3d31 290a 2020 2020 2020 2020 2020  is=1).          
-00008550: 2020 7469 6e64 7820 3d20 6e70 2e77 6865    tindx = np.whe
-00008560: 7265 2828 616d 706d 6178 203c 2032 3020  re((ampmax < 20 
-00008570: 2a20 6e70 2e6d 6564 6961 6e28 616d 706d  * np.median(ampm
-00008580: 6178 2929 2026 2028 616d 706d 6178 203e  ax)) & (ampmax >
-00008590: 2030 2929 5b30 5d0a 2020 2020 2020 2020   0))[0].        
-000085a0: 2020 2020 735f 636f 7272 203d 206e 702e      s_corr = np.
-000085b0: 6d65 616e 2873 5f63 6f72 725b 7469 6e64  mean(s_corr[tind
-000085c0: 785d 2c20 6178 6973 3d30 290a 2020 2020  x], axis=0).    
-000085d0: 2020 2020 2020 2020 745f 636f 7272 203d          t_corr =
-000085e0: 2064 6174 6153 5f74 5b30 5d0a 2020 2020   dataS_t[0].    
-000085f0: 2020 2020 2020 2020 6e5f 636f 7272 203d          n_corr =
-00008600: 206c 656e 2874 696e 6478 290a 2020 2020   len(tindx).    
-00008610: 2020 2020 656c 6966 2073 7461 636b 5f6d      elif stack_m
-00008620: 6574 686f 6420 3d3d 2022 726f 6275 7374  ethod == "robust
-00008630: 223a 0a20 2020 2020 2020 2020 2020 2070  ":.            p
-00008640: 7269 6e74 2822 646f 2072 6f62 7573 7420  rint("do robust 
-00008650: 7375 6273 7461 636b 696e 6722 290a 2020  substacking").  
-00008660: 2020 2020 2020 2020 2020 735f 636f 7272            s_corr
-00008670: 203d 2072 6f62 7573 745f 7374 6163 6b28   = robust_stack(
-00008680: 735f 636f 7272 2c20 302e 3030 3129 0a20  s_corr, 0.001). 
-00008690: 2020 2020 2020 2020 2020 2074 5f63 6f72             t_cor
-000086a0: 7220 3d20 6461 7461 535f 745b 305d 0a20  r = dataS_t[0]. 
-000086b0: 2020 2020 2020 2020 2020 206e 5f63 6f72             n_cor
-000086c0: 7220 3d20 6e77 696e 0a20 2020 2023 2020  r = nwin.    #  
-000086d0: 656c 6966 2073 7461 636b 5f6d 6574 686f  elif stack_metho
-000086e0: 6420 3d3d 2027 7365 6c65 6374 6976 6527  d == 'selective'
-000086f0: 3a0a 2020 2020 2320 2020 2020 2070 7269  :.    #      pri
-00008700: 6e74 2827 646f 2073 656c 6563 7469 7665  nt('do selective
-00008710: 2073 7562 7374 6163 6b69 6e67 2729 0a20   substacking'). 
-00008720: 2020 2023 2020 2020 2020 735f 636f 7272     #      s_corr
-00008730: 203d 2073 656c 6563 7469 7665 5f73 7461   = selective_sta
-00008740: 636b 2873 5f63 6f72 722c 302e 3030 3129  ck(s_corr,0.001)
-00008750: 0a20 2020 2023 2020 2020 2020 745f 636f  .    #      t_co
-00008760: 7272 203d 2064 6174 6153 5f74 5b30 5d0a  rr = dataS_t[0].
-00008770: 2020 2020 2320 2020 2020 206e 5f63 6f72      #      n_cor
-00008780: 7220 3d20 6e77 696e 0a0a 2020 2020 2320  r = nwin..    # 
-00008790: 7472 696d 2074 6865 2043 4346 7320 696e  trim the CCFs in
-000087a0: 205b 2d6d 6178 6c61 6720 6d61 786c 6167   [-maxlag maxlag
-000087b0: 5d0a 2020 2020 7420 3d20 6e70 2e61 7261  ].    t = np.ara
-000087c0: 6e67 6528 2d4e 6666 7432 202b 2031 2c20  nge(-Nfft2 + 1, 
-000087d0: 4e66 6674 3229 202a 2064 740a 2020 2020  Nfft2) * dt.    
-000087e0: 696e 6420 3d20 6e70 2e77 6865 7265 286e  ind = np.where(n
-000087f0: 702e 6162 7328 7429 203c 3d20 6d61 786c  p.abs(t) <= maxl
-00008800: 6167 295b 305d 0a20 2020 2069 6620 735f  ag)[0].    if s_
-00008810: 636f 7272 2e6e 6469 6d20 3d3d 2031 3a0a  corr.ndim == 1:.
-00008820: 2020 2020 2020 2020 735f 636f 7272 203d          s_corr =
-00008830: 2073 5f63 6f72 725b 696e 645d 0a20 2020   s_corr[ind].   
-00008840: 2065 6c69 6620 735f 636f 7272 2e6e 6469   elif s_corr.ndi
-00008850: 6d20 3d3d 2032 3a0a 2020 2020 2020 2020  m == 2:.        
-00008860: 735f 636f 7272 203d 2073 5f63 6f72 725b  s_corr = s_corr[
-00008870: 3a2c 2069 6e64 5d0a 2020 2020 7265 7475  :, ind].    retu
-00008880: 726e 2073 5f63 6f72 722c 2074 5f63 6f72  rn s_corr, t_cor
-00008890: 722c 206e 5f63 6f72 722c 206e 735f 636f  r, n_corr, ns_co
-000088a0: 7272 5b3a 2c20 696e 645d 0a0a 0a64 6566  rr[:, ind]...def
-000088b0: 2063 635f 7061 7261 6d65 7465 7273 2863   cc_parameters(c
-000088c0: 635f 7061 7261 2c20 636f 6f72 2c20 7463  c_para, coor, tc
-000088d0: 6f72 722c 206e 636f 7272 2c20 636f 6d70  orr, ncorr, comp
-000088e0: 293a 0a20 2020 2022 2222 0a20 2020 2074  ):.    """.    t
-000088f0: 6869 7320 6675 6e63 7469 6f6e 2061 7373  his function ass
-00008900: 656d 626c 6573 2074 6865 2070 6172 616d  embles the param
-00008910: 6574 6572 7320 666f 7220 7468 6520 6363  eters for the cc
-00008920: 2066 756e 6374 696f 6e2c 2077 6869 6368   function, which
-00008930: 2069 7320 7573 6564 0a20 2020 2077 6865   is used.    whe
-00008940: 6e20 7772 6974 696e 6720 7468 656d 2069  n writing them i
-00008950: 6e74 6f20 4153 4446 2066 696c 6573 0a20  nto ASDF files. 
-00008960: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
-00008970: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-00008980: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063 635f  --------.    cc_
-00008990: 7061 7261 3a20 6469 6374 2063 6f6e 7461  para: dict conta
-000089a0: 696e 696e 6720 7061 7261 6d65 7465 7273  ining parameters
-000089b0: 2075 7365 6420 696e 2074 6865 2066 6674   used in the fft
-000089c0: 5f63 6320 7374 6570 0a20 2020 2063 6f6f  _cc step.    coo
-000089d0: 723a 2020 2020 6469 6374 2063 6f6e 7461  r:    dict conta
-000089e0: 696e 696e 6720 636f 6f72 6469 6e61 7465  ining coordinate
-000089f0: 7320 696e 666f 206f 6620 7468 6520 736f  s info of the so
-00008a00: 7572 6365 2061 6e64 2072 6563 6569 7665  urce and receive
-00008a10: 7220 7374 6174 696f 6e73 0a20 2020 2074  r stations.    t
-00008a20: 636f 7272 3a20 2020 7469 6d65 7374 616d  corr:   timestam
-00008a30: 7020 6d61 7472 6978 0a20 2020 206e 636f  p matrix.    nco
-00008a40: 7272 3a20 2020 6d61 7472 6978 206f 6620  rr:   matrix of 
-00008a50: 6e75 6d62 6572 206f 6620 676f 6f64 2073  number of good s
-00008a60: 6567 6d65 6e74 7320 666f 7220 6561 6368  egments for each
-00008a70: 2073 7562 2d73 7461 636b 2f66 696e 616c   sub-stack/final
-00008a80: 2073 7461 636b 0a20 2020 2063 6f6d 703a   stack.    comp:
-00008a90: 2020 2020 3220 6368 6172 6163 7465 7220      2 character 
-00008aa0: 7374 7269 6e67 7320 666f 7220 7468 6520  strings for the 
-00008ab0: 6372 6f73 7320 636f 7272 656c 6174 696f  cross correlatio
-00008ac0: 6e20 636f 6d70 6f6e 656e 740a 2020 2020  n component.    
-00008ad0: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
-00008ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00008af0: 2020 2020 7061 7261 6d65 7465 7273 3a20      parameters: 
-00008b00: 6469 6374 2063 6f6e 7461 696e 696e 6720  dict containing 
-00008b10: 6162 6f76 6520 696e 666f 2075 7365 6420  above info used 
-00008b20: 666f 7220 6c61 7465 7220 7374 6163 6b69  for later stacki
-00008b30: 6e67 2f70 6c6f 7474 696e 670a 2020 2020  ng/plotting.    
-00008b40: 2222 220a 2020 2020 6c61 7453 203d 2063  """.    latS = c
-00008b50: 6f6f 725b 226c 6174 5322 5d0a 2020 2020  oor["latS"].    
-00008b60: 6c6f 6e53 203d 2063 6f6f 725b 226c 6f6e  lonS = coor["lon
-00008b70: 5322 5d0a 2020 2020 6c61 7452 203d 2063  S"].    latR = c
-00008b80: 6f6f 725b 226c 6174 5222 5d0a 2020 2020  oor["latR"].    
-00008b90: 6c6f 6e52 203d 2063 6f6f 725b 226c 6f6e  lonR = coor["lon
-00008ba0: 5222 5d0a 2020 2020 6474 203d 2063 635f  R"].    dt = cc_
-00008bb0: 7061 7261 5b22 6474 225d 0a20 2020 206d  para["dt"].    m
-00008bc0: 6178 6c61 6720 3d20 6363 5f70 6172 615b  axlag = cc_para[
-00008bd0: 226d 6178 6c61 6722 5d0a 2020 2020 7375  "maxlag"].    su
-00008be0: 6273 7461 636b 203d 2063 635f 7061 7261  bstack = cc_para
-00008bf0: 5b22 7375 6273 7461 636b 225d 0a20 2020  ["substack"].   
-00008c00: 2063 635f 6d65 7468 6f64 203d 2063 635f   cc_method = cc_
-00008c10: 7061 7261 5b22 6363 5f6d 6574 686f 6422  para["cc_method"
-00008c20: 5d0a 0a20 2020 2064 6973 742c 2061 7a69  ]..    dist, azi
-00008c30: 2c20 6261 7a20 3d20 6f62 7370 792e 6765  , baz = obspy.ge
-00008c40: 6f64 6574 6963 732e 6261 7365 2e67 7073  odetics.base.gps
-00008c50: 3264 6973 745f 617a 696d 7574 6828 6c61  2dist_azimuth(la
-00008c60: 7453 2c20 6c6f 6e53 2c20 6c61 7452 2c20  tS, lonS, latR, 
-00008c70: 6c6f 6e52 290a 2020 2020 7061 7261 6d65  lonR).    parame
-00008c80: 7465 7273 203d 207b 0a20 2020 2020 2020  ters = {.       
-00008c90: 2022 6474 223a 2064 742c 0a20 2020 2020   "dt": dt,.     
-00008ca0: 2020 2022 6d61 786c 6167 223a 2069 6e74     "maxlag": int
-00008cb0: 286d 6178 6c61 6729 2c0a 2020 2020 2020  (maxlag),.      
-00008cc0: 2020 2264 6973 7422 3a20 6e70 2e66 6c6f    "dist": np.flo
-00008cd0: 6174 3332 2864 6973 7420 2f20 3130 3030  at32(dist / 1000
-00008ce0: 292c 0a20 2020 2020 2020 2022 617a 6922  ),.        "azi"
-00008cf0: 3a20 6e70 2e66 6c6f 6174 3332 2861 7a69  : np.float32(azi
-00008d00: 292c 0a20 2020 2020 2020 2022 6261 7a22  ),.        "baz"
-00008d10: 3a20 6e70 2e66 6c6f 6174 3332 2862 617a  : np.float32(baz
-00008d20: 292c 0a20 2020 2020 2020 2022 6c6f 6e53  ),.        "lonS
-00008d30: 223a 206e 702e 666c 6f61 7433 3228 6c6f  ": np.float32(lo
-00008d40: 6e53 292c 0a20 2020 2020 2020 2022 6c61  nS),.        "la
-00008d50: 7453 223a 206e 702e 666c 6f61 7433 3228  tS": np.float32(
-00008d60: 6c61 7453 292c 0a20 2020 2020 2020 2022  latS),.        "
-00008d70: 6c6f 6e52 223a 206e 702e 666c 6f61 7433  lonR": np.float3
-00008d80: 3228 6c6f 6e52 292c 0a20 2020 2020 2020  2(lonR),.       
-00008d90: 2022 6c61 7452 223a 206e 702e 666c 6f61   "latR": np.floa
-00008da0: 7433 3228 6c61 7452 292c 0a20 2020 2020  t32(latR),.     
-00008db0: 2020 2022 6e67 6f6f 6422 3a20 6e63 6f72     "ngood": ncor
-00008dc0: 722c 0a20 2020 2020 2020 2022 6363 5f6d  r,.        "cc_m
-00008dd0: 6574 686f 6422 3a20 6363 5f6d 6574 686f  ethod": cc_metho
-00008de0: 642c 0a20 2020 2020 2020 2022 7469 6d65  d,.        "time
-00008df0: 223a 2074 636f 7272 2c0a 2020 2020 2020  ": tcorr,.      
-00008e00: 2020 2273 7562 7374 6163 6b22 3a20 7375    "substack": su
-00008e10: 6273 7461 636b 2c0a 2020 2020 2020 2020  bstack,.        
-00008e20: 2263 6f6d 7022 3a20 636f 6d70 2c0a 2020  "comp": comp,.  
-00008e30: 2020 7d0a 2020 2020 7265 7475 726e 2070    }.    return p
-00008e40: 6172 616d 6574 6572 730a 0a0a 6465 6620  arameters...def 
-00008e50: 7374 6163 6b69 6e67 2863 635f 6172 7261  stacking(cc_arra
-00008e60: 792c 2063 635f 7469 6d65 2c20 6363 5f6e  y, cc_time, cc_n
-00008e70: 676f 6f64 2c20 7374 6163 6b5f 7061 7261  good, stack_para
-00008e80: 293a 0a20 2020 2022 2222 0a20 2020 2074  ):.    """.    t
-00008e90: 6869 7320 6675 6e63 7469 6f6e 2073 7461  his function sta
-00008ea0: 636b 7320 7468 6520 6372 6f73 7320 636f  cks the cross co
-00008eb0: 7272 656c 6174 696f 6e20 6461 7461 2061  rrelation data a
-00008ec0: 6363 6f72 6469 6e67 2074 6f20 7468 6520  ccording to the 
-00008ed0: 7573 6572 2d64 6566 696e 6564 2073 7562  user-defined sub
-00008ee0: 7374 6163 6b5f 6c65 6e20 7061 7261 6d65  stack_len parame
-00008ef0: 7465 720a 0a20 2020 2050 4152 414d 4554  ter..    PARAMET
-00008f00: 4552 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ERS:.    -------
-00008f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00008f20: 2020 2020 6363 5f61 7272 6179 3a20 3244      cc_array: 2D
-00008f30: 206e 756d 7079 2066 6c6f 6174 3332 206d   numpy float32 m
-00008f40: 6174 7269 7820 636f 6e74 6169 6e69 6e67  atrix containing
-00008f50: 2061 6c6c 2073 6567 6d65 6e74 6564 2063   all segmented c
-00008f60: 726f 7373 2d63 6f72 7265 6c61 7469 6f6e  ross-correlation
-00008f70: 2064 6174 610a 2020 2020 6363 5f74 696d   data.    cc_tim
-00008f80: 653a 2020 3144 206e 756d 7079 2061 7272  e:  1D numpy arr
-00008f90: 6179 206f 6620 7469 6d65 7374 616d 7073  ay of timestamps
-00008fa0: 2066 6f72 2065 6163 6820 7365 676d 656e   for each segmen
-00008fb0: 7420 6f66 2063 635f 6172 7261 790a 2020  t of cc_array.  
-00008fc0: 2020 6363 5f6e 676f 6f64 3a20 3144 206e    cc_ngood: 1D n
-00008fd0: 756d 7079 2069 6e74 3136 206d 6174 7269  umpy int16 matri
-00008fe0: 7820 7368 6f77 696e 6720 7468 6520 6e75  x showing the nu
-00008ff0: 6d62 6572 206f 6620 7365 676d 656e 7473  mber of segments
-00009000: 2066 6f72 2065 6163 6820 7375 622d 7374   for each sub-st
-00009010: 6163 6b20 616e 642f 6f72 2066 756c 6c20  ack and/or full 
-00009020: 7374 6163 6b0a 2020 2020 7374 6163 6b5f  stack.    stack_
-00009030: 7061 7261 3a20 6120 6469 6374 2063 6f6e  para: a dict con
-00009040: 7461 696e 696e 6720 616c 6c20 7374 6163  taining all stac
-00009050: 6b69 6e67 2070 6172 616d 6574 6572 730a  king parameters.
-00009060: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
-00009070: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-00009080: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063 635f  --------.    cc_
-00009090: 6172 7261 792c 2063 635f 6e67 6f6f 642c  array, cc_ngood,
-000090a0: 2063 635f 7469 6d65 3a20 7361 6d65 2074   cc_time: same t
-000090b0: 6f20 7468 6520 696e 7075 7420 7061 7261  o the input para
-000090c0: 6d65 7465 7273 2062 7574 2077 6974 6820  meters but with 
-000090d0: 6162 6e6f 726d 616c 2063 726f 7373 2d63  abnormal cross-c
-000090e0: 6f72 7265 616c 7469 6f6e 7320 7265 6d6f  orrealtions remo
-000090f0: 7665 640a 2020 2020 616c 6c73 7461 636b  ved.    allstack
-00009100: 7331 3a20 3144 206d 6174 7269 7820 6f66  s1: 1D matrix of
-00009110: 2073 7461 636b 6564 2063 726f 7373 2d63   stacked cross-c
-00009120: 6f72 7265 6c61 7469 6f6e 2066 756e 6374  orrelation funct
-00009130: 696f 6e73 206f 7665 7220 616c 6c20 7468  ions over all th
-00009140: 6520 7365 676d 656e 7473 0a20 2020 206e  e segments.    n
-00009150: 7374 6163 6b73 3a20 2020 206e 756d 6265  stacks:    numbe
-00009160: 7220 6f66 206f 7665 7261 6c6c 2073 6567  r of overall seg
-00009170: 6d65 6e74 7320 666f 7220 7468 6520 6669  ments for the fi
-00009180: 6e61 6c20 7374 6163 6b73 0a20 2020 2022  nal stacks.    "
-00009190: 2222 0a20 2020 2023 206c 6f61 6420 7573  "".    # load us
-000091a0: 6566 756c 2070 6172 616d 6574 6572 7320  eful parameters 
-000091b0: 6672 6f6d 2064 6963 740a 2020 2020 7361  from dict.    sa
-000091c0: 6d70 5f66 7265 7120 3d20 7374 6163 6b5f  mp_freq = stack_
-000091d0: 7061 7261 5b22 7361 6d70 5f66 7265 7122  para["samp_freq"
-000091e0: 5d0a 2020 2020 736d 6574 686f 6420 3d20  ].    smethod = 
-000091f0: 7374 6163 6b5f 7061 7261 5b22 7374 6163  stack_para["stac
-00009200: 6b5f 6d65 7468 6f64 225d 0a20 2020 206e  k_method"].    n
-00009210: 7074 7320 3d20 6363 5f61 7272 6179 2e73  pts = cc_array.s
-00009220: 6861 7065 5b31 5d0a 0a20 2020 2023 2072  hape[1]..    # r
-00009230: 656d 6f76 6520 6162 6e6f 726d 616c 2064  emove abnormal d
-00009240: 6174 610a 2020 2020 616d 706d 6178 203d  ata.    ampmax =
-00009250: 206e 702e 6d61 7828 6363 5f61 7272 6179   np.max(cc_array
-00009260: 2c20 6178 6973 3d31 290a 2020 2020 7469  , axis=1).    ti
-00009270: 6e64 7820 3d20 6e70 2e77 6865 7265 2828  ndx = np.where((
-00009280: 616d 706d 6178 203c 2032 3020 2a20 6e70  ampmax < 20 * np
-00009290: 2e6d 6564 6961 6e28 616d 706d 6178 2929  .median(ampmax))
-000092a0: 2026 2028 616d 706d 6178 203e 2030 2929   & (ampmax > 0))
-000092b0: 5b30 5d0a 2020 2020 6966 206e 6f74 206c  [0].    if not l
-000092c0: 656e 2874 696e 6478 293a 0a20 2020 2020  en(tindx):.     
-000092d0: 2020 2061 6c6c 7374 6163 6b73 3120 3d20     allstacks1 = 
-000092e0: 5b5d 0a20 2020 2020 2020 2061 6c6c 7374  [].        allst
-000092f0: 6163 6b73 3220 3d20 5b5d 0a20 2020 2020  acks2 = [].     
-00009300: 2020 2061 6c6c 7374 6163 6b73 3320 3d20     allstacks3 = 
-00009310: 5b5d 0a20 2020 2020 2020 206e 7374 6163  [].        nstac
-00009320: 6b73 203d 2030 0a20 2020 2020 2020 2063  ks = 0.        c
-00009330: 635f 6172 7261 7920 3d20 5b5d 0a20 2020  c_array = [].   
-00009340: 2020 2020 2063 635f 6e67 6f6f 6420 3d20       cc_ngood = 
-00009350: 5b5d 0a20 2020 2020 2020 2063 635f 7469  [].        cc_ti
-00009360: 6d65 203d 205b 5d0a 2020 2020 2020 2020  me = [].        
-00009370: 7265 7475 726e 2063 635f 6172 7261 792c  return cc_array,
-00009380: 2063 635f 6e67 6f6f 642c 2063 635f 7469   cc_ngood, cc_ti
-00009390: 6d65 2c20 616c 6c73 7461 636b 7331 2c20  me, allstacks1, 
-000093a0: 616c 6c73 7461 636b 7332 2c20 616c 6c73  allstacks2, alls
-000093b0: 7461 636b 7333 2c20 6e73 7461 636b 730a  tacks3, nstacks.
-000093c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000093d0: 2020 2320 7265 6d6f 7665 206f 6e65 7320    # remove ones 
-000093e0: 7769 7468 2062 6164 2061 6d70 6c69 7475  with bad amplitu
-000093f0: 6465 0a20 2020 2020 2020 2063 635f 6172  de.        cc_ar
-00009400: 7261 7920 3d20 6363 5f61 7272 6179 5b74  ray = cc_array[t
-00009410: 696e 6478 2c20 3a5d 0a20 2020 2020 2020  indx, :].       
-00009420: 2063 635f 7469 6d65 203d 2063 635f 7469   cc_time = cc_ti
-00009430: 6d65 5b74 696e 6478 5d0a 2020 2020 2020  me[tindx].      
-00009440: 2020 6363 5f6e 676f 6f64 203d 2063 635f    cc_ngood = cc_
-00009450: 6e67 6f6f 645b 7469 6e64 785d 0a0a 2020  ngood[tindx]..  
-00009460: 2020 2020 2020 2320 646f 2073 7461 636b        # do stack
-00009470: 696e 670a 2020 2020 2020 2020 616c 6c73  ing.        alls
-00009480: 7461 636b 7331 203d 206e 702e 7a65 726f  tacks1 = np.zero
-00009490: 7328 6e70 7473 2c20 6474 7970 653d 6e70  s(npts, dtype=np
-000094a0: 2e66 6c6f 6174 3332 290a 2020 2020 2020  .float32).      
-000094b0: 2020 616c 6c73 7461 636b 7332 203d 206e    allstacks2 = n
-000094c0: 702e 7a65 726f 7328 6e70 7473 2c20 6474  p.zeros(npts, dt
-000094d0: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
-000094e0: 2020 2020 2020 2020 616c 6c73 7461 636b          allstack
-000094f0: 7333 203d 206e 702e 7a65 726f 7328 6e70  s3 = np.zeros(np
-00009500: 7473 2c20 6474 7970 653d 6e70 2e66 6c6f  ts, dtype=np.flo
-00009510: 6174 3332 290a 0a20 2020 2020 2020 2069  at32)..        i
-00009520: 6620 736d 6574 686f 6420 3d3d 2022 6c69  f smethod == "li
-00009530: 6e65 6172 223a 0a20 2020 2020 2020 2020  near":.         
-00009540: 2020 2061 6c6c 7374 6163 6b73 3120 3d20     allstacks1 = 
-00009550: 6e70 2e6d 6561 6e28 6363 5f61 7272 6179  np.mean(cc_array
-00009560: 2c20 6178 6973 3d30 290a 2020 2020 2020  , axis=0).      
-00009570: 2020 656c 6966 2073 6d65 7468 6f64 203d    elif smethod =
-00009580: 3d20 2270 7773 223a 0a20 2020 2020 2020  = "pws":.       
-00009590: 2020 2020 2061 6c6c 7374 6163 6b73 3120       allstacks1 
-000095a0: 3d20 7077 7328 6363 5f61 7272 6179 2c20  = pws(cc_array, 
-000095b0: 7361 6d70 5f66 7265 7129 0a20 2020 2020  samp_freq).     
-000095c0: 2020 2065 6c69 6620 736d 6574 686f 6420     elif smethod 
-000095d0: 3d3d 2022 726f 6275 7374 223a 0a20 2020  == "robust":.   
-000095e0: 2020 2020 2020 2020 2061 6c6c 7374 6163           allstac
-000095f0: 6b73 312c 2077 2c20 6e73 7465 7020 3d20  ks1, w, nstep = 
-00009600: 726f 6275 7374 5f73 7461 636b 2863 635f  robust_stack(cc_
-00009610: 6172 7261 792c 2030 2e30 3031 290a 2020  array, 0.001).  
-00009620: 2020 2020 2020 656c 6966 2073 6d65 7468        elif smeth
-00009630: 6f64 203d 3d20 2261 7574 6f5f 636f 7661  od == "auto_cova
-00009640: 7269 616e 6365 223a 0a20 2020 2020 2020  riance":.       
-00009650: 2020 2020 2061 6c6c 7374 6163 6b73 3120       allstacks1 
-00009660: 3d20 6164 6170 7469 7665 5f66 696c 7465  = adaptive_filte
-00009670: 7228 6363 5f61 7272 6179 2c20 3129 0a20  r(cc_array, 1). 
-00009680: 2020 2020 2020 2065 6c69 6620 736d 6574         elif smet
-00009690: 686f 6420 3d3d 2022 6e72 6f6f 7422 3a0a  hod == "nroot":.
-000096a0: 2020 2020 2020 2020 2020 2020 616c 6c73              alls
-000096b0: 7461 636b 7331 203d 206e 726f 6f74 5f73  tacks1 = nroot_s
-000096c0: 7461 636b 2863 635f 6172 7261 792c 2032  tack(cc_array, 2
-000096d0: 290a 2020 2020 2020 2020 656c 6966 2073  ).        elif s
-000096e0: 6d65 7468 6f64 203d 3d20 2261 6c6c 223a  method == "all":
-000096f0: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
-00009700: 7374 6163 6b73 3120 3d20 6e70 2e6d 6561  stacks1 = np.mea
-00009710: 6e28 6363 5f61 7272 6179 2c20 6178 6973  n(cc_array, axis
-00009720: 3d30 290a 2020 2020 2020 2020 2020 2020  =0).            
-00009730: 616c 6c73 7461 636b 7332 203d 2070 7773  allstacks2 = pws
-00009740: 2863 635f 6172 7261 792c 2073 616d 705f  (cc_array, samp_
-00009750: 6672 6571 290a 2020 2020 2020 2020 2020  freq).          
-00009760: 2020 616c 6c73 7461 636b 7333 2c20 772c    allstacks3, w,
-00009770: 206e 7374 6570 203d 2072 6f62 7573 745f   nstep = robust_
-00009780: 7374 6163 6b28 6363 5f61 7272 6179 2c20  stack(cc_array, 
-00009790: 302e 3030 3129 0a20 2020 2020 2020 206e  0.001).        n
-000097a0: 7374 6163 6b73 203d 206e 702e 7375 6d28  stacks = np.sum(
-000097b0: 6363 5f6e 676f 6f64 290a 0a20 2020 2023  cc_ngood)..    #
-000097c0: 2067 6f6f 6420 746f 2072 6574 7572 6e0a   good to return.
-000097d0: 2020 2020 7265 7475 726e 2063 635f 6172      return cc_ar
-000097e0: 7261 792c 2063 635f 6e67 6f6f 642c 2063  ray, cc_ngood, c
-000097f0: 635f 7469 6d65 2c20 616c 6c73 7461 636b  c_time, allstack
-00009800: 7331 2c20 616c 6c73 7461 636b 7332 2c20  s1, allstacks2, 
-00009810: 616c 6c73 7461 636b 7333 2c20 6e73 7461  allstacks3, nsta
-00009820: 636b 730a 0a0a 6465 6620 7374 6163 6b69  cks...def stacki
-00009830: 6e67 5f72 6d61 2863 635f 6172 7261 792c  ng_rma(cc_array,
-00009840: 2063 635f 7469 6d65 2c20 6363 5f6e 676f   cc_time, cc_ngo
-00009850: 6f64 2c20 7374 6163 6b5f 7061 7261 293a  od, stack_para):
-00009860: 0a20 2020 2022 2222 0a20 2020 2074 6869  .    """.    thi
-00009870: 7320 6675 6e63 7469 6f6e 2073 7461 636b  s function stack
-00009880: 7320 7468 6520 6372 6f73 7320 636f 7272  s the cross corr
-00009890: 656c 6174 696f 6e20 6461 7461 2061 6363  elation data acc
-000098a0: 6f72 6469 6e67 2074 6f20 7468 6520 7573  ording to the us
-000098b0: 6572 2d64 6566 696e 6564 2073 7562 7374  er-defined subst
-000098c0: 6163 6b5f 6c65 6e20 7061 7261 6d65 7465  ack_len paramete
-000098d0: 720a 2020 2020 5041 5241 4d45 5445 5253  r.    PARAMETERS
-000098e0: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-000098f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00009900: 2063 635f 6172 7261 793a 2032 4420 6e75   cc_array: 2D nu
-00009910: 6d70 7920 666c 6f61 7433 3220 6d61 7472  mpy float32 matr
-00009920: 6978 2063 6f6e 7461 696e 696e 6720 616c  ix containing al
-00009930: 6c20 7365 676d 656e 7465 6420 6372 6f73  l segmented cros
-00009940: 732d 636f 7272 656c 6174 696f 6e20 6461  s-correlation da
-00009950: 7461 0a20 2020 2063 635f 7469 6d65 3a20  ta.    cc_time: 
-00009960: 2031 4420 6e75 6d70 7920 6172 7261 7920   1D numpy array 
-00009970: 6f66 2074 696d 6573 7461 6d70 7320 666f  of timestamps fo
-00009980: 7220 6561 6368 2073 6567 6d65 6e74 206f  r each segment o
-00009990: 6620 6363 5f61 7272 6179 0a20 2020 2063  f cc_array.    c
-000099a0: 635f 6e67 6f6f 643a 2031 4420 6e75 6d70  c_ngood: 1D nump
-000099b0: 7920 696e 7431 3620 6d61 7472 6978 2073  y int16 matrix s
-000099c0: 686f 7769 6e67 2074 6865 206e 756d 6265  howing the numbe
-000099d0: 7220 6f66 2073 6567 6d65 6e74 7320 666f  r of segments fo
-000099e0: 7220 6561 6368 2073 7562 2d73 7461 636b  r each sub-stack
-000099f0: 2061 6e64 2f6f 7220 6675 6c6c 2073 7461   and/or full sta
-00009a00: 636b 0a20 2020 2073 7461 636b 5f70 6172  ck.    stack_par
-00009a10: 613a 2061 2064 6963 7420 636f 6e74 6169  a: a dict contai
-00009a20: 6e69 6e67 2061 6c6c 2073 7461 636b 696e  ning all stackin
-00009a30: 6720 7061 7261 6d65 7465 7273 0a20 2020  g parameters.   
-00009a40: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
-00009a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00009a60: 2d2d 2d2d 0a20 2020 2063 635f 6172 7261  ----.    cc_arra
-00009a70: 792c 2063 635f 6e67 6f6f 642c 2063 635f  y, cc_ngood, cc_
-00009a80: 7469 6d65 3a20 7361 6d65 2074 6f20 7468  time: same to th
-00009a90: 6520 696e 7075 7420 7061 7261 6d65 7465  e input paramete
-00009aa0: 7273 2062 7574 2077 6974 6820 6162 6e6f  rs but with abno
-00009ab0: 726d 616c 2063 726f 7373 2d63 6f72 7265  rmal cross-corre
-00009ac0: 616c 7469 6f6e 7320 7265 6d6f 7665 640a  altions removed.
-00009ad0: 2020 2020 616c 6c73 7461 636b 7331 3a20      allstacks1: 
-00009ae0: 3144 206d 6174 7269 7820 6f66 2073 7461  1D matrix of sta
-00009af0: 636b 6564 2063 726f 7373 2d63 6f72 7265  cked cross-corre
-00009b00: 6c61 7469 6f6e 2066 756e 6374 696f 6e73  lation functions
-00009b10: 206f 7665 7220 616c 6c20 7468 6520 7365   over all the se
-00009b20: 676d 656e 7473 0a20 2020 206e 7374 6163  gments.    nstac
-00009b30: 6b73 3a20 2020 206e 756d 6265 7220 6f66  ks:    number of
-00009b40: 206f 7665 7261 6c6c 2073 6567 6d65 6e74   overall segment
-00009b50: 7320 666f 7220 7468 6520 6669 6e61 6c20  s for the final 
-00009b60: 7374 6163 6b73 0a20 2020 2022 2222 0a20  stacks.    """. 
-00009b70: 2020 2023 206c 6f61 6420 7573 6566 756c     # load useful
-00009b80: 2070 6172 616d 6574 6572 7320 6672 6f6d   parameters from
-00009b90: 2064 6963 740a 2020 2020 7361 6d70 5f66   dict.    samp_f
-00009ba0: 7265 7120 3d20 7374 6163 6b5f 7061 7261  req = stack_para
-00009bb0: 5b22 7361 6d70 5f66 7265 7122 5d0a 2020  ["samp_freq"].  
-00009bc0: 2020 736d 6574 686f 6420 3d20 7374 6163    smethod = stac
-00009bd0: 6b5f 7061 7261 5b22 7374 6163 6b5f 6d65  k_para["stack_me
-00009be0: 7468 6f64 225d 0a20 2020 2072 6d61 5f73  thod"].    rma_s
-00009bf0: 7562 7374 6163 6b20 3d20 7374 6163 6b5f  ubstack = stack_
-00009c00: 7061 7261 5b22 726d 615f 7375 6273 7461  para["rma_substa
-00009c10: 636b 225d 0a20 2020 2072 6d61 5f73 7465  ck"].    rma_ste
-00009c20: 7020 3d20 7374 6163 6b5f 7061 7261 5b22  p = stack_para["
-00009c30: 726d 615f 7374 6570 225d 0a20 2020 2073  rma_step"].    s
-00009c40: 7461 7274 5f64 6174 6520 3d20 7374 6163  tart_date = stac
-00009c50: 6b5f 7061 7261 5b22 7374 6172 745f 6461  k_para["start_da
-00009c60: 7465 225d 0a20 2020 2065 6e64 5f64 6174  te"].    end_dat
-00009c70: 6520 3d20 7374 6163 6b5f 7061 7261 5b22  e = stack_para["
-00009c80: 656e 645f 6461 7465 225d 0a20 2020 206e  end_date"].    n
-00009c90: 7074 7320 3d20 6363 5f61 7272 6179 2e73  pts = cc_array.s
-00009ca0: 6861 7065 5b31 5d0a 0a20 2020 2023 2072  hape[1]..    # r
-00009cb0: 656d 6f76 6520 6162 6e6f 726d 616c 2064  emove abnormal d
-00009cc0: 6174 610a 2020 2020 616d 706d 6178 203d  ata.    ampmax =
-00009cd0: 206e 702e 6d61 7828 6363 5f61 7272 6179   np.max(cc_array
-00009ce0: 2c20 6178 6973 3d31 290a 2020 2020 7469  , axis=1).    ti
-00009cf0: 6e64 7820 3d20 6e70 2e77 6865 7265 2828  ndx = np.where((
-00009d00: 616d 706d 6178 203c 2032 3020 2a20 6e70  ampmax < 20 * np
-00009d10: 2e6d 6564 6961 6e28 616d 706d 6178 2929  .median(ampmax))
-00009d20: 2026 2028 616d 706d 6178 203e 2030 2929   & (ampmax > 0))
-00009d30: 5b30 5d0a 2020 2020 6966 206e 6f74 206c  [0].    if not l
-00009d40: 656e 2874 696e 6478 293a 0a20 2020 2020  en(tindx):.     
-00009d50: 2020 2061 6c6c 7374 6163 6b73 3120 3d20     allstacks1 = 
-00009d60: 5b5d 0a20 2020 2020 2020 2061 6c6c 7374  [].        allst
-00009d70: 6163 6b73 3220 3d20 5b5d 0a20 2020 2020  acks2 = [].     
-00009d80: 2020 206e 7374 6163 6b73 203d 2030 0a20     nstacks = 0. 
-00009d90: 2020 2020 2020 2063 635f 6172 7261 7920         cc_array 
-00009da0: 3d20 5b5d 0a20 2020 2020 2020 2063 635f  = [].        cc_
-00009db0: 6e67 6f6f 6420 3d20 5b5d 0a20 2020 2020  ngood = [].     
-00009dc0: 2020 2063 635f 7469 6d65 203d 205b 5d0a     cc_time = [].
-00009dd0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00009de0: 635f 6172 7261 792c 2063 635f 6e67 6f6f  c_array, cc_ngoo
-00009df0: 642c 2063 635f 7469 6d65 2c20 616c 6c73  d, cc_time, alls
-00009e00: 7461 636b 7331 2c20 616c 6c73 7461 636b  tacks1, allstack
-00009e10: 7332 2c20 6e73 7461 636b 730a 2020 2020  s2, nstacks.    
-00009e20: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
-00009e30: 7265 6d6f 7665 206f 6e65 7320 7769 7468  remove ones with
-00009e40: 2062 6164 2061 6d70 6c69 7475 6465 0a20   bad amplitude. 
-00009e50: 2020 2020 2020 2063 635f 6172 7261 7920         cc_array 
-00009e60: 3d20 6363 5f61 7272 6179 5b74 696e 6478  = cc_array[tindx
-00009e70: 2c20 3a5d 0a20 2020 2020 2020 2063 635f  , :].        cc_
-00009e80: 7469 6d65 203d 2063 635f 7469 6d65 5b74  time = cc_time[t
-00009e90: 696e 6478 5d0a 2020 2020 2020 2020 6363  indx].        cc
-00009ea0: 5f6e 676f 6f64 203d 2063 635f 6e67 6f6f  _ngood = cc_ngoo
-00009eb0: 645b 7469 6e64 785d 0a0a 2020 2020 2020  d[tindx]..      
-00009ec0: 2020 2320 646f 2073 7562 7374 6163 6b73    # do substacks
-00009ed0: 0a20 2020 2020 2020 2069 6620 726d 615f  .        if rma_
-00009ee0: 7375 6273 7461 636b 3a0a 2020 2020 2020  substack:.      
-00009ef0: 2020 2020 2020 7473 7461 7274 203d 206f        tstart = o
-00009f00: 6273 7079 2e55 5443 4461 7465 5469 6d65  bspy.UTCDateTime
-00009f10: 2873 7461 7274 5f64 6174 6529 202d 206f  (start_date) - o
-00009f20: 6273 7079 2e55 5443 4461 7465 5469 6d65  bspy.UTCDateTime
-00009f30: 2831 3937 302c 2031 2c20 3129 0a20 2020  (1970, 1, 1).   
-00009f40: 2020 2020 2020 2020 2074 656e 6420 3d20           tend = 
-00009f50: 6f62 7370 792e 5554 4344 6174 6554 696d  obspy.UTCDateTim
-00009f60: 6528 656e 645f 6461 7465 2920 2d20 6f62  e(end_date) - ob
-00009f70: 7370 792e 5554 4344 6174 6554 696d 6528  spy.UTCDateTime(
-00009f80: 3139 3730 2c20 312c 2031 290a 2020 2020  1970, 1, 1).    
-00009f90: 2020 2020 2020 2020 7474 696d 6520 3d20          ttime = 
-00009fa0: 7473 7461 7274 0a20 2020 2020 2020 2020  tstart.         
-00009fb0: 2020 206e 7374 6163 6b20 3d20 696e 7428     nstack = int(
-00009fc0: 6e70 2e72 6f75 6e64 2828 7465 6e64 202d  np.round((tend -
-00009fd0: 2074 7374 6172 7429 202f 2028 726d 615f   tstart) / (rma_
-00009fe0: 7374 6570 202a 2033 3630 3029 2929 0a20  step * 3600))). 
-00009ff0: 2020 2020 2020 2020 2020 206e 6363 5f61             ncc_a
-0000a000: 7272 6179 203d 206e 702e 7a65 726f 7328  rray = np.zeros(
-0000a010: 7368 6170 653d 286e 7374 6163 6b2c 206e  shape=(nstack, n
-0000a020: 7074 7329 2c20 6474 7970 653d 6e70 2e66  pts), dtype=np.f
-0000a030: 6c6f 6174 3332 290a 2020 2020 2020 2020  loat32).        
-0000a040: 2020 2020 6e63 635f 7469 6d65 203d 206e      ncc_time = n
-0000a050: 702e 7a65 726f 7328 6e73 7461 636b 2c20  p.zeros(nstack, 
-0000a060: 6474 7970 653d 6e70 2e66 6c6f 6174 290a  dtype=np.float).
-0000a070: 2020 2020 2020 2020 2020 2020 6e63 635f              ncc_
-0000a080: 6e67 6f6f 6420 3d20 6e70 2e7a 6572 6f73  ngood = np.zeros
-0000a090: 286e 7374 6163 6b2c 2064 7479 7065 3d6e  (nstack, dtype=n
-0000a0a0: 702e 696e 7429 0a0a 2020 2020 2020 2020  p.int)..        
-0000a0b0: 2020 2020 2320 6c6f 6f70 2074 6872 6f75      # loop throu
-0000a0c0: 6768 2065 6163 6820 7469 6d65 0a20 2020  gh each time.   
-0000a0d0: 2020 2020 2020 2020 2066 6f72 2069 6920           for ii 
-0000a0e0: 696e 2072 616e 6765 286e 7374 6163 6b29  in range(nstack)
-0000a0f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a100: 2020 7369 6e64 7820 3d20 6e70 2e77 6865    sindx = np.whe
-0000a110: 7265 2828 6363 5f74 696d 6520 3e3d 2074  re((cc_time >= t
-0000a120: 7469 6d65 2920 2620 2863 635f 7469 6d65  time) & (cc_time
-0000a130: 203c 2074 7469 6d65 202b 2072 6d61 5f73   < ttime + rma_s
-0000a140: 7562 7374 6163 6b20 2a20 3336 3030 2929  ubstack * 3600))
-0000a150: 5b30 5d0a 0a20 2020 2020 2020 2020 2020  [0]..           
-0000a160: 2020 2020 2023 2077 6865 6e20 7468 6572       # when ther
-0000a170: 6520 6172 6520 6461 7461 2069 6e20 7468  e are data in th
-0000a180: 6520 7469 6d65 2077 696e 646f 770a 2020  e time window.  
-0000a190: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000a1a0: 206c 656e 2873 696e 6478 293a 0a20 2020   len(sindx):.   
-0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1c0: 206e 6363 5f61 7272 6179 5b69 695d 203d   ncc_array[ii] =
-0000a1d0: 206e 702e 6d65 616e 2863 635f 6172 7261   np.mean(cc_arra
-0000a1e0: 795b 7369 6e64 785d 2c20 6178 6973 3d30  y[sindx], axis=0
-0000a1f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a200: 2020 2020 2020 6e63 635f 7469 6d65 5b69        ncc_time[i
-0000a210: 695d 203d 2074 7469 6d65 0a20 2020 2020  i] = ttime.     
-0000a220: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-0000a230: 6363 5f6e 676f 6f64 5b69 695d 203d 206e  cc_ngood[ii] = n
-0000a240: 702e 7375 6d28 6363 5f6e 676f 6f64 5b73  p.sum(cc_ngood[s
-0000a250: 696e 6478 5d2c 2061 7869 733d 3029 0a20  indx], axis=0). 
-0000a260: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000a270: 7469 6d65 202b 3d20 726d 615f 7374 6570  time += rma_step
-0000a280: 202a 2033 3630 300a 0a20 2020 2020 2020   * 3600..       
-0000a290: 2020 2020 2023 2072 656d 6f76 6520 6261       # remove ba
-0000a2a0: 6420 6f6e 6573 0a20 2020 2020 2020 2020  d ones.         
-0000a2b0: 2020 2074 696e 6478 203d 206e 702e 7768     tindx = np.wh
-0000a2c0: 6572 6528 6e63 635f 6e67 6f6f 6420 3e20  ere(ncc_ngood > 
-0000a2d0: 3029 5b30 5d0a 2020 2020 2020 2020 2020  0)[0].          
-0000a2e0: 2020 6e63 635f 6172 7261 7920 3d20 6e63    ncc_array = nc
-0000a2f0: 635f 6172 7261 795b 7469 6e64 785d 0a20  c_array[tindx]. 
-0000a300: 2020 2020 2020 2020 2020 206e 6363 5f74             ncc_t
-0000a310: 696d 6520 3d20 6e63 635f 7469 6d65 5b74  ime = ncc_time[t
-0000a320: 696e 6478 5d0a 2020 2020 2020 2020 2020  indx].          
-0000a330: 2020 6e63 635f 6e67 6f6f 6420 3d20 6e63    ncc_ngood = nc
-0000a340: 635f 6e67 6f6f 645b 7469 6e64 785d 0a0a  c_ngood[tindx]..
-0000a350: 2020 2020 2020 2020 2320 646f 2073 7461          # do sta
-0000a360: 636b 696e 670a 2020 2020 2020 2020 616c  cking.        al
-0000a370: 6c73 7461 636b 7331 203d 206e 702e 7a65  lstacks1 = np.ze
-0000a380: 726f 7328 6e70 7473 2c20 6474 7970 653d  ros(npts, dtype=
-0000a390: 6e70 2e66 6c6f 6174 3332 290a 2020 2020  np.float32).    
-0000a3a0: 2020 2020 616c 6c73 7461 636b 7332 203d      allstacks2 =
-0000a3b0: 206e 702e 7a65 726f 7328 6e70 7473 2c20   np.zeros(npts, 
-0000a3c0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-0000a3d0: 290a 2020 2020 2020 2020 616c 6c73 7461  ).        allsta
-0000a3e0: 636b 7333 203d 206e 702e 7a65 726f 7328  cks3 = np.zeros(
-0000a3f0: 6e70 7473 2c20 6474 7970 653d 6e70 2e66  npts, dtype=np.f
-0000a400: 6c6f 6174 3332 290a 2020 2020 2020 2020  loat32).        
-0000a410: 616c 6c73 7461 636b 7334 203d 206e 702e  allstacks4 = np.
-0000a420: 7a65 726f 7328 6e70 7473 2c20 6474 7970  zeros(npts, dtyp
-0000a430: 653d 6e70 2e66 6c6f 6174 3332 290a 0a20  e=np.float32).. 
-0000a440: 2020 2020 2020 2069 6620 736d 6574 686f         if smetho
-0000a450: 6420 3d3d 2022 6c69 6e65 6172 223a 0a20  d == "linear":. 
-0000a460: 2020 2020 2020 2020 2020 2061 6c6c 7374             allst
-0000a470: 6163 6b73 3120 3d20 6e70 2e6d 6561 6e28  acks1 = np.mean(
-0000a480: 6363 5f61 7272 6179 2c20 6178 6973 3d30  cc_array, axis=0
-0000a490: 290a 2020 2020 2020 2020 656c 6966 2073  ).        elif s
-0000a4a0: 6d65 7468 6f64 203d 3d20 2270 7773 223a  method == "pws":
-0000a4b0: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
-0000a4c0: 7374 6163 6b73 3120 3d20 7077 7328 6363  stacks1 = pws(cc
-0000a4d0: 5f61 7272 6179 2c20 7361 6d70 5f66 7265  _array, samp_fre
-0000a4e0: 7129 0a20 2020 2020 2020 2065 6c69 6620  q).        elif 
-0000a4f0: 736d 6574 686f 6420 3d3d 2022 726f 6275  smethod == "robu
-0000a500: 7374 223a 0a20 2020 2020 2020 2020 2020  st":.           
-0000a510: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-0000a520: 2020 2061 6c6c 7374 6163 6b73 312c 0a20     allstacks1,. 
-0000a530: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000a540: 2c0a 2020 2020 2020 2020 2020 2020 2920  ,.            ) 
-0000a550: 3d20 726f 6275 7374 5f73 7461 636b 2863  = robust_stack(c
-0000a560: 635f 6172 7261 792c 2030 2e30 3031 290a  c_array, 0.001).
-0000a570: 2020 2020 2020 2020 656c 6966 2073 6d65          elif sme
-0000a580: 7468 6f64 203d 3d20 2273 656c 6563 7469  thod == "selecti
-0000a590: 7665 223a 0a20 2020 2020 2020 2020 2020  ve":.           
-0000a5a0: 2061 6c6c 7374 6163 6b73 3120 3d20 7365   allstacks1 = se
-0000a5b0: 6c65 6374 6976 655f 7374 6163 6b28 6363  lective_stack(cc
-0000a5c0: 5f61 7272 6179 2c20 302e 3030 3129 0a20  _array, 0.001). 
-0000a5d0: 2020 2020 2020 2065 6c69 6620 736d 6574         elif smet
-0000a5e0: 686f 6420 3d3d 2022 616c 6c22 3a0a 2020  hod == "all":.  
-0000a5f0: 2020 2020 2020 2020 2020 616c 6c73 7461            allsta
-0000a600: 636b 7331 203d 206e 702e 6d65 616e 2863  cks1 = np.mean(c
-0000a610: 635f 6172 7261 792c 2061 7869 733d 3029  c_array, axis=0)
-0000a620: 0a20 2020 2020 2020 2020 2020 2061 6c6c  .            all
-0000a630: 7374 6163 6b73 3220 3d20 7077 7328 6363  stacks2 = pws(cc
-0000a640: 5f61 7272 6179 2c20 7361 6d70 5f66 7265  _array, samp_fre
-0000a650: 7129 0a20 2020 2020 2020 2020 2020 2061  q).            a
-0000a660: 6c6c 7374 6163 6b73 3320 3d20 726f 6275  llstacks3 = robu
-0000a670: 7374 5f73 7461 636b 2863 635f 6172 7261  st_stack(cc_arra
-0000a680: 792c 2030 2e30 3031 290a 2020 2020 2020  y, 0.001).      
-0000a690: 2020 2020 2020 616c 6c73 7461 636b 7334        allstacks4
-0000a6a0: 203d 2073 656c 6563 7469 7665 5f73 7461   = selective_sta
-0000a6b0: 636b 2863 635f 6172 7261 792c 2030 2e30  ck(cc_array, 0.0
-0000a6c0: 3031 290a 2020 2020 2020 2020 6e73 7461  01).        nsta
-0000a6d0: 636b 7320 3d20 6e70 2e73 756d 2863 635f  cks = np.sum(cc_
-0000a6e0: 6e67 6f6f 6429 0a0a 2020 2020 2320 7265  ngood)..    # re
-0000a6f0: 706c 6163 6520 7468 6520 6172 7261 7920  place the array 
-0000a700: 666f 7220 7375 6273 7461 636b 730a 2020  for substacks.  
-0000a710: 2020 6966 2072 6d61 5f73 7562 7374 6163    if rma_substac
-0000a720: 6b3a 0a20 2020 2020 2020 2063 635f 6172  k:.        cc_ar
-0000a730: 7261 7920 3d20 6e63 635f 6172 7261 790a  ray = ncc_array.
-0000a740: 2020 2020 2020 2020 6363 5f74 696d 6520          cc_time 
-0000a750: 3d20 6e63 635f 7469 6d65 0a20 2020 2020  = ncc_time.     
-0000a760: 2020 2063 635f 6e67 6f6f 6420 3d20 6e63     cc_ngood = nc
-0000a770: 635f 6e67 6f6f 640a 0a20 2020 2023 2067  c_ngood..    # g
-0000a780: 6f6f 6420 746f 2072 6574 7572 6e0a 2020  ood to return.  
-0000a790: 2020 7265 7475 726e 2028 0a20 2020 2020    return (.     
-0000a7a0: 2020 2063 635f 6172 7261 792c 0a20 2020     cc_array,.   
-0000a7b0: 2020 2020 2063 635f 6e67 6f6f 642c 0a20       cc_ngood,. 
-0000a7c0: 2020 2020 2020 2063 635f 7469 6d65 2c0a         cc_time,.
-0000a7d0: 2020 2020 2020 2020 616c 6c73 7461 636b          allstack
-0000a7e0: 7331 2c0a 2020 2020 2020 2020 616c 6c73  s1,.        alls
-0000a7f0: 7461 636b 7332 2c0a 2020 2020 2020 2020  tacks2,.        
-0000a800: 616c 6c73 7461 636b 7333 2c0a 2020 2020  allstacks3,.    
-0000a810: 2020 2020 616c 6c73 7461 636b 7334 2c0a      allstacks4,.
-0000a820: 2020 2020 2020 2020 6e73 7461 636b 732c          nstacks,
-0000a830: 0a20 2020 2029 0a0a 0a64 6566 2072 6f74  .    )...def rot
-0000a840: 6174 696f 6e28 6269 6773 7461 636b 2c20  ation(bigstack, 
-0000a850: 7061 7261 6d65 7465 7273 2c20 6c6f 6373  parameters, locs
-0000a860: 293a 0a20 2020 2022 2222 0a20 2020 2074  ):.    """.    t
-0000a870: 6869 7320 6675 6e63 7469 6f6e 2074 7261  his function tra
-0000a880: 6e73 6665 7273 2074 6865 2047 7265 656e  nsfers the Green
-0000a890: 2773 2074 656e 736f 7220 6672 6f6d 2061  's tensor from a
-0000a8a0: 2045 2d4e 2d5a 2073 7973 7465 6d20 696e   E-N-Z system in
-0000a8b0: 746f 2061 2052 2d54 2d5a 206f 6e65 0a0a  to a R-T-Z one..
-0000a8c0: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
-0000a8d0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-0000a8e0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6269 6773  -------.    bigs
-0000a8f0: 7461 636b 3a20 2020 3920 636f 6d70 6f6e  tack:   9 compon
-0000a900: 656e 7420 4772 6565 6e27 7320 7465 6e73  ent Green's tens
-0000a910: 6f72 2069 6e20 452d 4e2d 5a20 7379 7374  or in E-N-Z syst
-0000a920: 656d 0a20 2020 2070 6172 616d 6574 6572  em.    parameter
-0000a930: 733a 2064 6963 7420 636f 6e74 6169 6e69  s: dict containi
-0000a940: 6e67 2061 6c6c 2070 6172 616d 6574 6572  ng all parameter
-0000a950: 7320 7361 7665 6420 696e 2041 5344 4620  s saved in ASDF 
-0000a960: 6669 6c65 0a20 2020 206c 6f63 733a 2020  file.    locs:  
-0000a970: 2020 2020 2064 6963 7420 636f 6e74 6169       dict contai
-0000a980: 6e69 6e67 2073 7461 7469 6f6e 2061 6e67  ning station ang
-0000a990: 6c65 2069 6e66 6f20 666f 7220 636f 7272  le info for corr
-0000a9a0: 6563 7469 6f6e 2070 7572 706f 7365 0a20  ection purpose. 
-0000a9b0: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
-0000a9c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000a9d0: 2d2d 2d0a 2020 2020 7463 6f72 723a 2039  ---.    tcorr: 9
-0000a9e0: 2063 6f6d 706f 6e65 6e74 2047 7265 656e   component Green
-0000a9f0: 2773 2074 656e 736f 7220 696e 2052 2d54  's tensor in R-T
-0000aa00: 2d5a 2073 7973 7465 6d0a 2020 2020 2222  -Z system.    ""
-0000aa10: 220a 2020 2020 2320 6c6f 6164 2070 6172  ".    # load par
-0000aa20: 616d 6574 6572 2064 6963 0a20 2020 2070  ameter dic.    p
-0000aa30: 6920 3d20 6e70 2e70 690a 2020 2020 617a  i = np.pi.    az
-0000aa40: 6920 3d20 7061 7261 6d65 7465 7273 5b22  i = parameters["
-0000aa50: 617a 6922 5d0a 2020 2020 6261 7a20 3d20  azi"].    baz = 
-0000aa60: 7061 7261 6d65 7465 7273 5b22 6261 7a22  parameters["baz"
-0000aa70: 5d0a 2020 2020 6e63 6f6d 702c 206e 7074  ].    ncomp, npt
-0000aa80: 7320 3d20 6269 6773 7461 636b 2e73 6861  s = bigstack.sha
-0000aa90: 7065 0a20 2020 2069 6620 6e63 6f6d 7020  pe.    if ncomp 
-0000aaa0: 3c20 393a 0a20 2020 2020 2020 2070 7269  < 9:.        pri
-0000aab0: 6e74 2822 6372 6170 2064 6964 206e 6f74  nt("crap did not
-0000aac0: 2067 6574 2065 6e6f 7567 6820 636f 6d70   get enough comp
-0000aad0: 6f6e 656e 7473 2229 0a20 2020 2020 2020  onents").       
-0000aae0: 2074 636f 7272 203d 205b 5d0a 2020 2020   tcorr = [].    
-0000aaf0: 2020 2020 7265 7475 726e 2074 636f 7272      return tcorr
-0000ab00: 0a20 2020 2073 7461 5320 3d20 7061 7261  .    staS = para
-0000ab10: 6d65 7465 7273 5b22 7374 6174 696f 6e5f  meters["station_
-0000ab20: 736f 7572 6365 225d 0a20 2020 2073 7461  source"].    sta
-0000ab30: 5220 3d20 7061 7261 6d65 7465 7273 5b22  R = parameters["
-0000ab40: 7374 6174 696f 6e5f 7265 6365 6976 6572  station_receiver
-0000ab50: 225d 0a0a 2020 2020 6966 206c 656e 286c  "]..    if len(l
-0000ab60: 6f63 7329 3a0a 2020 2020 2020 2020 7374  ocs):.        st
-0000ab70: 615f 6c69 7374 203d 206c 6973 7428 6c6f  a_list = list(lo
-0000ab80: 6373 5b22 7374 6174 696f 6e22 5d29 0a20  cs["station"]). 
-0000ab90: 2020 2020 2020 2061 6e67 6c65 7320 3d20         angles = 
-0000aba0: 6c69 7374 286c 6f63 735b 2261 6e67 6c65  list(locs["angle
-0000abb0: 225d 290a 2020 2020 2020 2020 2320 6765  "]).        # ge
-0000abc0: 7420 7374 6174 696f 6e20 696e 666f 2066  t station info f
-0000abd0: 726f 6d20 7468 6520 6e61 6d65 206f 6620  rom the name of 
-0000abe0: 4153 4446 2066 696c 650a 2020 2020 2020  ASDF file.      
-0000abf0: 2020 696e 6420 3d20 7374 615f 6c69 7374    ind = sta_list
-0000ac00: 2e69 6e64 6578 2873 7461 5329 0a20 2020  .index(staS).   
-0000ac10: 2020 2020 2061 636f 7272 203d 2061 6e67       acorr = ang
-0000ac20: 6c65 735b 696e 645d 0a20 2020 2020 2020  les[ind].       
-0000ac30: 2069 6e64 203d 2073 7461 5f6c 6973 742e   ind = sta_list.
-0000ac40: 696e 6465 7828 7374 6152 290a 2020 2020  index(staR).    
-0000ac50: 2020 2020 6263 6f72 7220 3d20 616e 676c      bcorr = angl
-0000ac60: 6573 5b69 6e64 5d0a 0a20 2020 2023 202d  es[ind]..    # -
-0000ac70: 2d2d 616e 676c 6573 2074 6f20 6265 2063  --angles to be c
-0000ac80: 6f72 7265 6374 6564 2d2d 2d2d 0a20 2020  orrected----.   
-0000ac90: 2069 6620 6c65 6e28 6c6f 6373 293a 0a20   if len(locs):. 
-0000aca0: 2020 2020 2020 2063 6f73 6120 3d20 6e70         cosa = np
-0000acb0: 2e63 6f73 2828 617a 6920 2b20 6163 6f72  .cos((azi + acor
-0000acc0: 7229 202a 2070 6920 2f20 3138 3029 0a20  r) * pi / 180). 
-0000acd0: 2020 2020 2020 2073 696e 6120 3d20 6e70         sina = np
-0000ace0: 2e73 696e 2828 617a 6920 2b20 6163 6f72  .sin((azi + acor
-0000acf0: 7229 202a 2070 6920 2f20 3138 3029 0a20  r) * pi / 180). 
-0000ad00: 2020 2020 2020 2063 6f73 6220 3d20 6e70         cosb = np
-0000ad10: 2e63 6f73 2828 6261 7a20 2b20 6263 6f72  .cos((baz + bcor
-0000ad20: 7229 202a 2070 6920 2f20 3138 3029 0a20  r) * pi / 180). 
-0000ad30: 2020 2020 2020 2073 696e 6220 3d20 6e70         sinb = np
-0000ad40: 2e73 696e 2828 6261 7a20 2b20 6263 6f72  .sin((baz + bcor
-0000ad50: 7229 202a 2070 6920 2f20 3138 3029 0a20  r) * pi / 180). 
-0000ad60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000ad70: 2063 6f73 6120 3d20 6e70 2e63 6f73 2861   cosa = np.cos(a
-0000ad80: 7a69 202a 2070 6920 2f20 3138 3029 0a20  zi * pi / 180). 
-0000ad90: 2020 2020 2020 2073 696e 6120 3d20 6e70         sina = np
-0000ada0: 2e73 696e 2861 7a69 202a 2070 6920 2f20  .sin(azi * pi / 
-0000adb0: 3138 3029 0a20 2020 2020 2020 2063 6f73  180).        cos
-0000adc0: 6220 3d20 6e70 2e63 6f73 2862 617a 202a  b = np.cos(baz *
-0000add0: 2070 6920 2f20 3138 3029 0a20 2020 2020   pi / 180).     
-0000ade0: 2020 2073 696e 6220 3d20 6e70 2e73 696e     sinb = np.sin
-0000adf0: 2862 617a 202a 2070 6920 2f20 3138 3029  (baz * pi / 180)
-0000ae00: 0a0a 2020 2020 2320 7274 7a5f 636f 6d70  ..    # rtz_comp
-0000ae10: 6f6e 656e 7473 203d 205b 275a 5227 2c27  onents = ['ZR','
-0000ae20: 5a54 272c 275a 5a27 2c27 5252 272c 2752  ZT','ZZ','RR','R
-0000ae30: 5427 2c27 525a 272c 2754 5227 2c27 5454  T','RZ','TR','TT
-0000ae40: 272c 2754 5a27 5d0a 2020 2020 7463 6f72  ','TZ'].    tcor
-0000ae50: 7220 3d20 6e70 2e7a 6572 6f73 2873 6861  r = np.zeros(sha
-0000ae60: 7065 3d28 392c 206e 7074 7329 2c20 6474  pe=(9, npts), dt
-0000ae70: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
-0000ae80: 2020 2020 7463 6f72 725b 305d 203d 202d      tcorr[0] = -
-0000ae90: 636f 7362 202a 2062 6967 7374 6163 6b5b  cosb * bigstack[
-0000aea0: 375d 202d 2073 696e 6220 2a20 6269 6773  7] - sinb * bigs
-0000aeb0: 7461 636b 5b36 5d0a 2020 2020 7463 6f72  tack[6].    tcor
-0000aec0: 725b 315d 203d 2073 696e 6220 2a20 6269  r[1] = sinb * bi
-0000aed0: 6773 7461 636b 5b37 5d20 2d20 636f 7362  gstack[7] - cosb
-0000aee0: 202a 2062 6967 7374 6163 6b5b 365d 0a20   * bigstack[6]. 
-0000aef0: 2020 2074 636f 7272 5b32 5d20 3d20 6269     tcorr[2] = bi
-0000af00: 6773 7461 636b 5b38 5d0a 2020 2020 7463  gstack[8].    tc
-0000af10: 6f72 725b 335d 203d 2028 0a20 2020 2020  orr[3] = (.     
-0000af20: 2020 202d 636f 7361 202a 2063 6f73 6220     -cosa * cosb 
-0000af30: 2a20 6269 6773 7461 636b 5b34 5d20 2d20  * bigstack[4] - 
-0000af40: 636f 7361 202a 2073 696e 6220 2a20 6269  cosa * sinb * bi
-0000af50: 6773 7461 636b 5b33 5d20 2d20 7369 6e61  gstack[3] - sina
-0000af60: 202a 2063 6f73 6220 2a20 6269 6773 7461   * cosb * bigsta
-0000af70: 636b 5b31 5d20 2d20 7369 6e61 202a 2073  ck[1] - sina * s
-0000af80: 696e 6220 2a20 6269 6773 7461 636b 5b30  inb * bigstack[0
-0000af90: 5d0a 2020 2020 290a 2020 2020 7463 6f72  ].    ).    tcor
-0000afa0: 725b 345d 203d 2028 0a20 2020 2020 2020  r[4] = (.       
-0000afb0: 2063 6f73 6120 2a20 7369 6e62 202a 2062   cosa * sinb * b
-0000afc0: 6967 7374 6163 6b5b 345d 202d 2063 6f73  igstack[4] - cos
-0000afd0: 6120 2a20 636f 7362 202a 2062 6967 7374  a * cosb * bigst
-0000afe0: 6163 6b5b 335d 202b 2073 696e 6120 2a20  ack[3] + sina * 
-0000aff0: 7369 6e62 202a 2062 6967 7374 6163 6b5b  sinb * bigstack[
-0000b000: 315d 202d 2073 696e 6120 2a20 636f 7362  1] - sina * cosb
-0000b010: 202a 2062 6967 7374 6163 6b5b 305d 0a20   * bigstack[0]. 
-0000b020: 2020 2029 0a20 2020 2074 636f 7272 5b35     ).    tcorr[5
-0000b030: 5d20 3d20 636f 7361 202a 2062 6967 7374  ] = cosa * bigst
-0000b040: 6163 6b5b 355d 202b 2073 696e 6120 2a20  ack[5] + sina * 
-0000b050: 6269 6773 7461 636b 5b32 5d0a 2020 2020  bigstack[2].    
-0000b060: 7463 6f72 725b 365d 203d 2028 0a20 2020  tcorr[6] = (.   
-0000b070: 2020 2020 2073 696e 6120 2a20 636f 7362       sina * cosb
-0000b080: 202a 2062 6967 7374 6163 6b5b 345d 202b   * bigstack[4] +
-0000b090: 2073 696e 6120 2a20 7369 6e62 202a 2062   sina * sinb * b
-0000b0a0: 6967 7374 6163 6b5b 335d 202d 2063 6f73  igstack[3] - cos
-0000b0b0: 6120 2a20 636f 7362 202a 2062 6967 7374  a * cosb * bigst
-0000b0c0: 6163 6b5b 315d 202d 2063 6f73 6120 2a20  ack[1] - cosa * 
-0000b0d0: 7369 6e62 202a 2062 6967 7374 6163 6b5b  sinb * bigstack[
-0000b0e0: 305d 0a20 2020 2029 0a20 2020 2074 636f  0].    ).    tco
-0000b0f0: 7272 5b37 5d20 3d20 280a 2020 2020 2020  rr[7] = (.      
-0000b100: 2020 2d73 696e 6120 2a20 7369 6e62 202a    -sina * sinb *
-0000b110: 2062 6967 7374 6163 6b5b 345d 202b 2073   bigstack[4] + s
-0000b120: 696e 6120 2a20 636f 7362 202a 2062 6967  ina * cosb * big
-0000b130: 7374 6163 6b5b 335d 202b 2063 6f73 6120  stack[3] + cosa 
-0000b140: 2a20 7369 6e62 202a 2062 6967 7374 6163  * sinb * bigstac
-0000b150: 6b5b 315d 202d 2063 6f73 6120 2a20 636f  k[1] - cosa * co
-0000b160: 7362 202a 2062 6967 7374 6163 6b5b 305d  sb * bigstack[0]
-0000b170: 0a20 2020 2029 0a20 2020 2074 636f 7272  .    ).    tcorr
-0000b180: 5b38 5d20 3d20 2d73 696e 6120 2a20 6269  [8] = -sina * bi
-0000b190: 6773 7461 636b 5b35 5d20 2b20 636f 7361  gstack[5] + cosa
-0000b1a0: 202a 2062 6967 7374 6163 6b5b 325d 0a0a   * bigstack[2]..
-0000b1b0: 2020 2020 7265 7475 726e 2074 636f 7272      return tcorr
-0000b1c0: 0a0a 0a23 2323 2323 2323 2323 2323 2323  ...#############
+000046f0: 2d2d 0a20 2020 2074 7261 6365 5f73 7464  --.    trace_std
+00004700: 533a 2073 7461 6e64 6172 6420 6465 7669  S: standard devi
+00004710: 6174 696f 6e20 6f66 2074 6865 206e 6f69  ation of the noi
+00004720: 7365 2061 6d70 6c69 7475 6465 206f 6620  se amplitude of 
+00004730: 6561 6368 2073 6567 6d65 6e74 0a20 2020  each segment.   
+00004740: 2064 6174 6153 5f74 3a20 2020 2074 696d   dataS_t:    tim
+00004750: 6573 7461 6d70 7320 6f66 2065 6163 6820  estamps of each 
+00004760: 7365 676d 656e 740a 2020 2020 6461 7461  segment.    data
+00004770: 533a 2020 2020 2020 3244 206d 6174 7269  S:      2D matri
+00004780: 7820 6f66 2074 6865 2073 6567 6d65 6e74  x of the segment
+00004790: 6564 2064 6174 610a 2020 2020 2222 220a  ed data.    """.
+000047a0: 2020 2020 2320 6465 6669 6e65 2072 6574      # define ret
+000047b0: 7572 6e20 7661 7269 6162 6c65 7320 6669  urn variables fi
+000047c0: 7273 740a 2020 2020 736f 7572 6365 5f70  rst.    source_p
+000047d0: 6172 616d 7320 3d20 5b5d 0a20 2020 2064  arams = [].    d
+000047e0: 6174 6153 5f74 203d 205b 5d0a 2020 2020  ataS_t = [].    
+000047f0: 6461 7461 5320 3d20 5b5d 0a0a 2020 2020  dataS = []..    
+00004800: 2320 7573 6566 756c 2070 6172 616d 6574  # useful paramet
+00004810: 6572 7320 666f 7220 7472 6163 6520 736c  ers for trace sl
+00004820: 6964 696e 670a 2020 2020 6e73 6567 203d  iding.    nseg =
+00004830: 2069 6e74 286e 702e 666c 6f6f 7228 2866   int(np.floor((f
+00004840: 635f 7061 7261 2e69 6e63 5f68 6f75 7273  c_para.inc_hours
+00004850: 202f 2032 3420 2a20 3836 3430 3020 2d20   / 24 * 86400 - 
+00004860: 6663 5f70 6172 612e 6363 5f6c 656e 2920  fc_para.cc_len) 
+00004870: 2f20 6663 5f70 6172 612e 7374 6570 2929  / fc_para.step))
+00004880: 0a20 2020 2073 7073 203d 2069 6e74 2863  .    sps = int(c
+00004890: 685f 6461 7461 2e73 616d 706c 696e 675f  h_data.sampling_
+000048a0: 7261 7465 290a 2020 2020 7374 6172 7474  rate).    startt
+000048b0: 696d 6520 3d20 6368 5f64 6174 612e 7374  ime = ch_data.st
+000048c0: 6172 745f 7469 6d65 7374 616d 700a 2020  art_timestamp.  
+000048d0: 2020 2320 636f 7079 2064 6174 6120 696e    # copy data in
+000048e0: 746f 2061 7272 6179 0a20 2020 2064 6174  to array.    dat
+000048f0: 6120 3d20 6368 5f64 6174 612e 6461 7461  a = ch_data.data
+00004900: 0a0a 2020 2020 2320 6966 2074 6865 2064  ..    # if the d
+00004910: 6174 6120 6973 2073 686f 7274 6572 2074  ata is shorter t
+00004920: 6861 6e20 7468 6520 7469 6d20 6368 756e  han the tim chun
+00004930: 636b 2c20 7265 7475 726e 207a 6572 6f20  ck, return zero 
+00004940: 7661 6c75 6573 0a20 2020 2069 6620 6461  values.    if da
+00004950: 7461 2e73 697a 6520 3c20 7370 7320 2a20  ta.size < sps * 
+00004960: 6663 5f70 6172 612e 696e 635f 686f 7572  fc_para.inc_hour
+00004970: 7320 2a20 3336 3030 3a0a 2020 2020 2020  s * 3600:.      
+00004980: 2020 7265 7475 726e 2073 6f75 7263 655f    return source_
+00004990: 7061 7261 6d73 2c20 6461 7461 535f 742c  params, dataS_t,
+000049a0: 2064 6174 6153 0a0a 2020 2020 2320 7374   dataS..    # st
+000049b0: 6174 6973 7469 6320 746f 2064 6574 6563  atistic to detec
+000049c0: 7420 7365 676d 656e 7473 2074 6861 7420  t segments that 
+000049d0: 6d61 7920 6265 2061 7373 6f63 6961 7465  may be associate
+000049e0: 6420 7769 7468 2065 6172 7468 7175 616b  d with earthquak
+000049f0: 6573 0a20 2020 2061 6c6c 5f6d 6164 5320  es.    all_madS 
+00004a00: 3d20 6d61 6428 6461 7461 2920 2023 206d  = mad(data)  # m
+00004a10: 6564 6961 6e20 6162 736f 6c75 7465 2064  edian absolute d
+00004a20: 6576 6961 7469 6f6e 206f 7665 7220 616c  eviation over al
+00004a30: 6c20 6e6f 6973 6520 7769 6e64 6f77 0a20  l noise window. 
+00004a40: 2020 2061 6c6c 5f73 7464 5320 3d20 6e70     all_stdS = np
+00004a50: 2e73 7464 2864 6174 6129 2020 2320 7374  .std(data)  # st
+00004a60: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
+00004a70: 206f 7665 7220 616c 6c20 6e6f 6973 6520   over all noise 
+00004a80: 7769 6e64 6f77 0a20 2020 2069 6620 616c  window.    if al
+00004a90: 6c5f 6d61 6453 203d 3d20 3020 6f72 2061  l_madS == 0 or a
+00004aa0: 6c6c 5f73 7464 5320 3d3d 2030 206f 7220  ll_stdS == 0 or 
+00004ab0: 6e70 2e69 736e 616e 2861 6c6c 5f6d 6164  np.isnan(all_mad
+00004ac0: 5329 206f 7220 6e70 2e69 736e 616e 2861  S) or np.isnan(a
+00004ad0: 6c6c 5f73 7464 5329 3a0a 2020 2020 2020  ll_stdS):.      
+00004ae0: 2020 7072 696e 7428 2263 6f6e 7469 6e75    print("continu
+00004af0: 6521 206d 6164 5320 6f72 2073 7464 5320  e! madS or stdS 
+00004b00: 6571 7561 6c73 2074 6f20 3020 666f 7220  equals to 0 for 
+00004b10: 2573 2229 0a20 2020 2020 2020 2072 6574  %s").        ret
+00004b20: 7572 6e20 736f 7572 6365 5f70 6172 616d  urn source_param
+00004b30: 732c 2064 6174 6153 5f74 2c20 6461 7461  s, dataS_t, data
+00004b40: 530a 0a20 2020 2023 2069 6e69 7469 616c  S..    # initial
+00004b50: 697a 6520 7661 7269 6162 6c65 730a 2020  ize variables.  
+00004b60: 2020 6e70 7473 203d 2069 6e74 2866 635f    npts = int(fc_
+00004b70: 7061 7261 2e63 635f 6c65 6e20 2a20 7370  para.cc_len * sp
+00004b80: 7329 0a20 2020 2023 2074 7261 6365 5f6d  s).    # trace_m
+00004b90: 6164 5320 3d20 6e70 2e7a 6572 6f73 286e  adS = np.zeros(n
+00004ba0: 7365 672c 6474 7970 653d 6e70 2e66 6c6f  seg,dtype=np.flo
+00004bb0: 6174 3332 290a 2020 2020 7472 6163 655f  at32).    trace_
+00004bc0: 7374 6453 203d 206e 702e 7a65 726f 7328  stdS = np.zeros(
+00004bd0: 6e73 6567 2c20 6474 7970 653d 6e70 2e66  nseg, dtype=np.f
+00004be0: 6c6f 6174 3332 290a 2020 2020 6461 7461  loat32).    data
+00004bf0: 5320 3d20 6e70 2e7a 6572 6f73 2873 6861  S = np.zeros(sha
+00004c00: 7065 3d28 696e 7428 6e73 6567 292c 2069  pe=(int(nseg), i
+00004c10: 6e74 286e 7074 7329 292c 2064 7479 7065  nt(npts)), dtype
+00004c20: 3d6e 702e 666c 6f61 7433 3229 0a20 2020  =np.float32).   
+00004c30: 2064 6174 6153 5f74 203d 206e 702e 7a65   dataS_t = np.ze
+00004c40: 726f 7328 6e73 6567 2c20 6474 7970 653d  ros(nseg, dtype=
+00004c50: 6e70 2e66 6c6f 6174 3332 290a 0a20 2020  np.float32)..   
+00004c60: 2069 6e64 7831 203d 2030 0a20 2020 2066   indx1 = 0.    f
+00004c70: 6f72 2069 7365 6720 696e 2072 616e 6765  or iseg in range
+00004c80: 286e 7365 6729 3a0a 2020 2020 2020 2020  (nseg):.        
+00004c90: 696e 6478 3220 3d20 696e 6478 3120 2b20  indx2 = indx1 + 
+00004ca0: 6e70 7473 0a20 2020 2020 2020 2064 6174  npts.        dat
+00004cb0: 6153 5b69 7365 675d 203d 2064 6174 615b  aS[iseg] = data[
+00004cc0: 696e 6478 313a 696e 6478 325d 0a20 2020  indx1:indx2].   
+00004cd0: 2020 2020 2023 2074 7261 6365 5f6d 6164       # trace_mad
+00004ce0: 535b 6973 6567 5d20 3d20 286e 702e 6d61  S[iseg] = (np.ma
+00004cf0: 7828 6e70 2e61 6273 2864 6174 6153 5b69  x(np.abs(dataS[i
+00004d00: 7365 675d 2929 2f61 6c6c 5f6d 6164 5329  seg]))/all_madS)
+00004d10: 0a20 2020 2020 2020 2074 7261 6365 5f73  .        trace_s
+00004d20: 7464 535b 6973 6567 5d20 3d20 6e70 2e6d  tdS[iseg] = np.m
+00004d30: 6178 286e 702e 6162 7328 6461 7461 535b  ax(np.abs(dataS[
+00004d40: 6973 6567 5d29 2920 2f20 616c 6c5f 7374  iseg])) / all_st
+00004d50: 6453 0a20 2020 2020 2020 2064 6174 6153  dS.        dataS
+00004d60: 5f74 5b69 7365 675d 203d 2073 7461 7274  _t[iseg] = start
+00004d70: 7469 6d65 202b 2066 635f 7061 7261 2e73  time + fc_para.s
+00004d80: 7465 7020 2a20 6973 6567 0a20 2020 2020  tep * iseg.     
+00004d90: 2020 2069 6e64 7831 203d 2069 6e64 7831     indx1 = indx1
+00004da0: 202b 2069 6e74 2866 635f 7061 7261 2e73   + int(fc_para.s
+00004db0: 7465 7029 202a 2073 7073 0a0a 2020 2020  tep) * sps..    
+00004dc0: 2320 3244 2061 7272 6179 2070 726f 6365  # 2D array proce
+00004dd0: 7373 696e 670a 2020 2020 6461 7461 5320  ssing.    dataS 
+00004de0: 3d20 6465 6d65 616e 2864 6174 6153 290a  = demean(dataS).
+00004df0: 2020 2020 6461 7461 5320 3d20 6465 7472      dataS = detr
+00004e00: 656e 6428 6461 7461 5329 0a20 2020 2064  end(dataS).    d
+00004e10: 6174 6153 203d 2074 6170 6572 2864 6174  ataS = taper(dat
+00004e20: 6153 290a 0a20 2020 2072 6574 7572 6e20  aS)..    return 
+00004e30: 7472 6163 655f 7374 6453 2c20 6461 7461  trace_stdS, data
+00004e40: 535f 742c 2064 6174 6153 0a0a 0a64 6566  S_t, dataS...def
+00004e50: 206e 6f69 7365 5f70 726f 6365 7373 696e   noise_processin
+00004e60: 6728 6666 745f 7061 7261 2c20 6461 7461  g(fft_para, data
+00004e70: 5329 3a0a 2020 2020 2222 220a 2020 2020  S):.    """.    
+00004e80: 7468 6973 2066 756e 6374 696f 6e20 7065  this function pe
+00004e90: 7266 6f72 6d73 2074 696d 6520 646f 6d61  rforms time doma
+00004ea0: 696e 2061 6e64 2066 7265 7175 656e 6379  in and frequency
+00004eb0: 2064 6f6d 6169 6e20 6e6f 726d 616c 697a   domain normaliz
+00004ec0: 6174 696f 6e20 6966 206e 6565 6465 642e  ation if needed.
+00004ed0: 2069 6e20 7265 616c 2063 6173 652c 2077   in real case, w
+00004ee0: 6520 7072 6566 6572 2075 7365 2069 6e63  e prefer use inc
+00004ef0: 6c75 6465 0a20 2020 2074 6865 206e 6f72  lude.    the nor
+00004f00: 6d61 6c69 7a61 7469 6f6e 2069 6e20 7468  malization in th
+00004f10: 6520 6372 6f73 732d 636f 7272 6561 6c74  e cross-correalt
+00004f20: 696f 6e20 7374 6570 7320 6279 2073 656c  ion steps by sel
+00004f30: 6563 7469 6e67 2063 6f68 6572 656e 6379  ecting coherency
+00004f40: 206f 7220 6465 636f 6e0a 2020 2020 2850   or decon.    (P
+00004f50: 7269 6574 6f20 6574 2061 6c2c 2032 3030  rieto et al, 200
+00004f60: 382c 2032 3030 393b 2044 656e 6f6c 6c65  8, 2009; Denolle
+00004f70: 2065 7420 616c 2c20 3230 3133 290a 2020   et al, 2013).  
+00004f80: 2020 5041 524d 4145 5445 5253 3a0a 2020    PARMAETERS:.  
+00004f90: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00004fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2066  ----------.    f
+00004fb0: 6674 5f70 6172 613a 2064 6963 7469 6f6e  ft_para: diction
+00004fc0: 6172 7920 636f 6e74 6169 6e69 6e67 2061  ary containing a
+00004fd0: 6c6c 2075 7365 6675 6c20 7661 7269 6162  ll useful variab
+00004fe0: 6c65 7320 7573 6564 2066 6f72 2066 6674  les used for fft
+00004ff0: 2061 6e64 2063 630a 2020 2020 6461 7461   and cc.    data
+00005000: 533a 2032 4420 6d61 7472 6978 206f 6620  S: 2D matrix of 
+00005010: 616c 6c20 7365 676d 656e 7465 6420 6e6f  all segmented no
+00005020: 6973 6520 6461 7461 0a20 2020 2023 204f  ise data.    # O
+00005030: 5554 5055 5420 5641 5249 4142 4c45 533a  UTPUT VARIABLES:
+00005040: 0a20 2020 2073 6f75 7263 655f 7768 6974  .    source_whit
+00005050: 653a 2032 4420 6d61 7472 6978 206f 6620  e: 2D matrix of 
+00005060: 6461 7461 2073 7065 6374 7261 0a20 2020  data spectra.   
+00005070: 2022 2222 0a20 2020 2023 206c 6f61 6420   """.    # load 
+00005080: 7061 7261 6d65 7465 7273 2066 6972 7374  parameters first
+00005090: 0a20 2020 2074 696d 655f 6e6f 726d 203d  .    time_norm =
+000050a0: 2066 6674 5f70 6172 615b 2274 696d 655f   fft_para["time_
+000050b0: 6e6f 726d 225d 0a20 2020 2066 7265 715f  norm"].    freq_
+000050c0: 6e6f 726d 203d 2066 6674 5f70 6172 615b  norm = fft_para[
+000050d0: 2266 7265 715f 6e6f 726d 225d 0a20 2020  "freq_norm"].   
+000050e0: 2073 6d6f 6f74 685f 4e20 3d20 6666 745f   smooth_N = fft_
+000050f0: 7061 7261 5b22 736d 6f6f 7468 5f4e 225d  para["smooth_N"]
+00005100: 0a20 2020 204e 203d 2064 6174 6153 2e73  .    N = dataS.s
+00005110: 6861 7065 5b30 5d0a 0a20 2020 2023 202d  hape[0]..    # -
+00005120: 2d2d 2d2d 2d74 6f20 6e6f 726d 616c 697a  -----to normaliz
+00005130: 6520 696e 2074 696d 6520 6f72 206e 6f74  e in time or not
+00005140: 2d2d 2d2d 2d2d 0a20 2020 2069 6620 7469  ------.    if ti
+00005150: 6d65 5f6e 6f72 6d20 213d 2022 6e6f 223a  me_norm != "no":
+00005160: 0a20 2020 2020 2020 2069 6620 7469 6d65  .        if time
+00005170: 5f6e 6f72 6d20 3d3d 2022 6f6e 655f 6269  _norm == "one_bi
+00005180: 7422 3a20 2023 2073 6967 6e20 6e6f 726d  t":  # sign norm
+00005190: 616c 697a 6174 696f 6e0a 2020 2020 2020  alization.      
+000051a0: 2020 2020 2020 7768 6974 6520 3d20 6e70        white = np
+000051b0: 2e73 6967 6e28 6461 7461 5329 0a20 2020  .sign(dataS).   
+000051c0: 2020 2020 2065 6c69 6620 7469 6d65 5f6e       elif time_n
+000051d0: 6f72 6d20 3d3d 2022 726d 6122 3a20 2023  orm == "rma":  #
+000051e0: 2072 756e 6e69 6e67 206d 6561 6e3a 206e   running mean: n
+000051f0: 6f72 6d61 6c69 7a61 7469 6f6e 206f 7665  ormalization ove
+00005200: 7220 736d 6f6f 7468 6564 2061 6273 6f6c  r smoothed absol
+00005210: 7574 6520 6176 6572 6167 650a 2020 2020  ute average.    
+00005220: 2020 2020 2020 2020 7768 6974 6520 3d20          white = 
+00005230: 6e70 2e7a 6572 6f73 2873 6861 7065 3d64  np.zeros(shape=d
+00005240: 6174 6153 2e73 6861 7065 2c20 6474 7970  ataS.shape, dtyp
+00005250: 653d 6461 7461 532e 6474 7970 6529 0a20  e=dataS.dtype). 
+00005260: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
+00005270: 6b6b 2069 6e20 7261 6e67 6528 4e29 3a0a  kk in range(N):.
+00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005290: 7768 6974 655b 6b6b 6b2c 203a 5d20 3d20  white[kkk, :] = 
+000052a0: 6461 7461 535b 6b6b 6b2c 203a 5d20 2f20  dataS[kkk, :] / 
+000052b0: 6d6f 7669 6e67 5f61 7665 286e 702e 6162  moving_ave(np.ab
+000052c0: 7328 6461 7461 535b 6b6b 6b2c 203a 5d29  s(dataS[kkk, :])
+000052d0: 2c20 736d 6f6f 7468 5f4e 290a 0a20 2020  , smooth_N)..   
+000052e0: 2065 6c73 653a 2020 2320 646f 6e27 7420   else:  # don't 
+000052f0: 6e6f 726d 616c 697a 650a 2020 2020 2020  normalize.      
+00005300: 2020 7768 6974 6520 3d20 6461 7461 530a    white = dataS.
+00005310: 0a20 2020 2023 202d 2d2d 2d2d 746f 2077  .    # -----to w
+00005320: 6869 7465 6e20 6f72 206e 6f74 2d2d 2d2d  hiten or not----
+00005330: 2d2d 0a20 2020 2069 6620 6672 6571 5f6e  --.    if freq_n
+00005340: 6f72 6d20 213d 2022 6e6f 223a 0a20 2020  orm != "no":.   
+00005350: 2020 2020 2073 6f75 7263 655f 7768 6974       source_whit
+00005360: 6520 3d20 7768 6974 656e 2877 6869 7465  e = whiten(white
+00005370: 2c20 6666 745f 7061 7261 2920 2023 2077  , fft_para)  # w
+00005380: 6869 7465 6e20 616e 6420 7265 7475 726e  hiten and return
+00005390: 2046 4654 0a20 2020 2065 6c73 653a 0a20   FFT.    else:. 
+000053a0: 2020 2020 2020 204e 6666 7420 3d20 696e         Nfft = in
+000053b0: 7428 6e65 7874 5f66 6173 745f 6c65 6e28  t(next_fast_len(
+000053c0: 696e 7428 6461 7461 532e 7368 6170 655b  int(dataS.shape[
+000053d0: 315d 2929 290a 2020 2020 2020 2020 736f  1]))).        so
+000053e0: 7572 6365 5f77 6869 7465 203d 2073 6369  urce_white = sci
+000053f0: 7079 2e66 6674 7061 636b 2e66 6674 2877  py.fftpack.fft(w
+00005400: 6869 7465 2c20 4e66 6674 2c20 6178 6973  hite, Nfft, axis
+00005410: 3d31 2920 2023 2072 6574 7572 6e20 4646  =1)  # return FF
+00005420: 540a 0a20 2020 2072 6574 7572 6e20 736f  T..    return so
+00005430: 7572 6365 5f77 6869 7465 0a0a 0a64 6566  urce_white...def
+00005440: 2073 6d6f 6f74 685f 736f 7572 6365 5f73   smooth_source_s
+00005450: 7065 6374 2863 635f 7061 7261 2c20 6666  pect(cc_para, ff
+00005460: 7431 293a 0a20 2020 2022 2222 0a20 2020  t1):.    """.   
+00005470: 2074 6869 7320 6675 6e63 7469 6f6e 2073   this function s
+00005480: 6d6f 6f74 6865 7320 616d 706c 6974 7564  moothes amplitud
+00005490: 6520 7370 6563 7472 756d 206f 6620 7468  e spectrum of th
+000054a0: 6520 3244 2073 7065 6374 7261 6c20 6d61  e 2D spectral ma
+000054b0: 7472 6978 2e20 2875 7365 6420 696e 2053  trix. (used in S
+000054c0: 3129 0a20 2020 2050 4152 414d 4554 4552  1).    PARAMETER
+000054d0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+000054e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+000054f0: 2063 635f 7061 7261 3a20 6469 6374 696f   cc_para: dictio
+00005500: 6e61 7279 2063 6f6e 7461 696e 696e 6720  nary containing 
+00005510: 7573 6566 756c 2063 6320 7061 7261 6d65  useful cc parame
+00005520: 7465 7273 0a20 2020 2066 6674 313a 2020  ters.    fft1:  
+00005530: 2020 736f 7572 6365 2073 7065 6374 7275    source spectru
+00005540: 6d20 6d61 7472 6978 0a0a 2020 2020 5245  m matrix..    RE
+00005550: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
+00005560: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00005570: 0a20 2020 2073 6666 7431 3a20 636f 6d70  .    sfft1: comp
+00005580: 6c65 7820 6e75 6d70 7920 6172 7261 7920  lex numpy array 
+00005590: 7769 7468 206e 6f72 6d61 6c69 7a65 6420  with normalized 
+000055a0: 7370 6563 7472 756d 0a20 2020 2022 2222  spectrum.    """
+000055b0: 0a20 2020 2063 635f 6d65 7468 6f64 203d  .    cc_method =
+000055c0: 2063 635f 7061 7261 5b22 6363 5f6d 6574   cc_para["cc_met
+000055d0: 686f 6422 5d0a 2020 2020 736d 6f6f 7468  hod"].    smooth
+000055e0: 7370 6563 745f 4e20 3d20 6363 5f70 6172  spect_N = cc_par
+000055f0: 615b 2273 6d6f 6f74 6873 7065 6374 5f4e  a["smoothspect_N
+00005600: 225d 0a0a 2020 2020 6966 2063 635f 6d65  "]..    if cc_me
+00005610: 7468 6f64 203d 3d20 2264 6563 6f6e 7622  thod == "deconv"
+00005620: 3a0a 2020 2020 2020 2020 2320 2d2d 2d2d  :.        # ----
+00005630: 2d6e 6f72 6d61 6c69 7a65 2073 696e 676c  -normalize singl
+00005640: 652d 7374 6174 696f 6e20 6363 2074 6f20  e-station cc to 
+00005650: 7a20 636f 6d70 6f6e 656e 742d 2d2d 2d2d  z component-----
+00005660: 0a20 2020 2020 2020 2074 656d 7020 3d20  .        temp = 
+00005670: 6d6f 7669 6e67 5f61 7665 286e 702e 6162  moving_ave(np.ab
+00005680: 7328 6666 7431 292c 2073 6d6f 6f74 6873  s(fft1), smooths
+00005690: 7065 6374 5f4e 290a 2020 2020 2020 2020  pect_N).        
+000056a0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+000056b0: 2073 6666 7431 203d 206e 702e 636f 6e6a   sfft1 = np.conj
+000056c0: 2866 6674 3129 202f 2074 656d 702a 2a32  (fft1) / temp**2
+000056d0: 0a20 2020 2020 2020 2065 7863 6570 7420  .        except 
+000056e0: 4578 6365 7074 696f 6e3a 0a20 2020 2020  Exception:.     
+000056f0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00005700: 7565 4572 726f 7228 2273 6d6f 6f74 6865  ueError("smoothe
+00005710: 6420 7370 6563 7472 756d 2068 6173 207a  d spectrum has z
+00005720: 6572 6f20 7661 6c75 6573 2229 0a0a 2020  ero values")..  
+00005730: 2020 656c 6966 2063 635f 6d65 7468 6f64    elif cc_method
+00005740: 203d 3d20 2263 6f68 6572 656e 6379 223a   == "coherency":
+00005750: 0a20 2020 2020 2020 2074 656d 7020 3d20  .        temp = 
+00005760: 6d6f 7669 6e67 5f61 7665 286e 702e 6162  moving_ave(np.ab
+00005770: 7328 6666 7431 292c 2073 6d6f 6f74 6873  s(fft1), smooths
+00005780: 7065 6374 5f4e 290a 2020 2020 2020 2020  pect_N).        
+00005790: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+000057a0: 2073 6666 7431 203d 206e 702e 636f 6e6a   sfft1 = np.conj
+000057b0: 2866 6674 3129 202f 2074 656d 700a 2020  (fft1) / temp.  
+000057c0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+000057d0: 6570 7469 6f6e 3a0a 2020 2020 2020 2020  eption:.        
+000057e0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+000057f0: 7272 6f72 2822 736d 6f6f 7468 6564 2073  rror("smoothed s
+00005800: 7065 6374 7275 6d20 6861 7320 7a65 726f  pectrum has zero
+00005810: 2076 616c 7565 7322 290a 0a20 2020 2065   values")..    e
+00005820: 6c69 6620 6363 5f6d 6574 686f 6420 3d3d  lif cc_method ==
+00005830: 2022 7863 6f72 7222 3a0a 2020 2020 2020   "xcorr":.      
+00005840: 2020 7366 6674 3120 3d20 6e70 2e63 6f6e    sfft1 = np.con
+00005850: 6a28 6666 7431 290a 0a20 2020 2065 6c73  j(fft1)..    els
+00005860: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
+00005870: 2056 616c 7565 4572 726f 7228 226e 6f20   ValueError("no 
+00005880: 636f 7272 6563 7469 6f6e 2063 6f72 7265  correction corre
+00005890: 6c61 7469 6f6e 206d 6574 686f 6420 6973  lation method is
+000058a0: 2073 656c 6563 7465 6420 6174 204c 3539   selected at L59
+000058b0: 2229 0a0a 2020 2020 7265 7475 726e 2073  ")..    return s
+000058c0: 6666 7431 0a0a 0a64 6566 2063 6f72 7265  fft1...def corre
+000058d0: 6c61 7465 2866 6674 315f 736d 6f6f 7468  late(fft1_smooth
+000058e0: 6564 5f61 6273 2c20 6666 7432 2c20 442c  ed_abs, fft2, D,
+000058f0: 204e 6666 742c 2064 6174 6153 5f74 293a   Nfft, dataS_t):
+00005900: 0a20 2020 2022 2222 0a20 2020 2074 6869  .    """.    thi
+00005910: 7320 6675 6e63 7469 6f6e 2064 6f65 7320  s function does 
+00005920: 7468 6520 6372 6f73 732d 636f 7272 656c  the cross-correl
+00005930: 6174 696f 6e20 696e 2066 7265 7120 646f  ation in freq do
+00005940: 6d61 696e 2061 6e64 2068 6173 2074 6865  main and has the
+00005950: 206f 7074 696f 6e20 746f 206b 6565 7020   option to keep 
+00005960: 7375 622d 7374 6163 6b73 206f 660a 2020  sub-stacks of.  
+00005970: 2020 7468 6520 6372 6f73 732d 636f 7272    the cross-corr
+00005980: 656c 6174 696f 6e20 6966 206e 6565 6465  elation if neede
+00005990: 642e 2069 7420 7461 6b65 7320 6164 7661  d. it takes adva
+000059a0: 6e74 6167 6520 6f66 2074 6865 206c 696e  ntage of the lin
+000059b0: 6561 7220 7265 6c61 7469 6f6e 7368 6970  ear relationship
+000059c0: 206f 6620 6966 6674 2c20 736f 2074 6861   of ifft, so tha
+000059d0: 740a 2020 2020 7374 6163 6b69 6e67 2069  t.    stacking i
+000059e0: 7320 7065 7266 6f72 6d65 6420 696e 2073  s performed in s
+000059f0: 7065 6374 7275 6d20 646f 6d61 696e 2066  pectrum domain f
+00005a00: 6972 7374 2074 6f20 7265 6475 6365 2074  irst to reduce t
+00005a10: 6865 2074 6f74 616c 206e 756d 6265 7220  he total number 
+00005a20: 6f66 2069 6666 742e 2028 7573 6564 2069  of ifft. (used i
+00005a30: 6e20 5331 290a 2020 2020 5041 5241 4d45  n S1).    PARAME
+00005a40: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
+00005a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00005a60: 2020 2020 6666 7431 5f73 6d6f 6f74 6865      fft1_smoothe
+00005a70: 645f 6162 733a 2073 6d6f 6f74 6865 6420  d_abs: smoothed 
+00005a80: 706f 7765 7220 7370 6563 7472 616c 2064  power spectral d
+00005a90: 656e 7369 7479 206f 6620 7468 6520 4646  ensity of the FF
+00005aa0: 5420 666f 7220 7468 6520 736f 7572 6365  T for the source
+00005ab0: 2073 7461 7469 6f6e 0a20 2020 2066 6674   station.    fft
+00005ac0: 323a 2072 6177 2046 4654 2073 7065 6374  2: raw FFT spect
+00005ad0: 7275 6d20 6f66 2074 6865 2072 6563 6569  rum of the recei
+00005ae0: 7665 7220 7374 6174 696f 6e0a 2020 2020  ver station.    
+00005af0: 443a 2064 6963 7469 6f6e 6172 7920 636f  D: dictionary co
+00005b00: 6e74 6169 6e69 6e67 2066 6f6c 6c6f 7769  ntaining followi
+00005b10: 6e67 2070 6172 616d 6574 6572 733a 0a20  ng parameters:. 
+00005b20: 2020 2020 2020 206d 6178 6c61 673a 2020         maxlag:  
+00005b30: 6d61 7869 6d75 6d20 6c61 6773 2074 6f20  maximum lags to 
+00005b40: 6b65 6570 2069 6e20 7468 6520 6372 6f73  keep in the cros
+00005b50: 7320 636f 7272 656c 6174 696f 6e0a 2020  s correlation.  
+00005b60: 2020 2020 2020 6474 3a20 2020 2020 2073        dt:      s
+00005b70: 616d 706c 696e 6720 7261 7465 2028 696e  ampling rate (in
+00005b80: 2073 290a 2020 2020 2020 2020 6e77 696e   s).        nwin
+00005b90: 3a20 2020 206e 756d 6265 7220 6f66 2073  :    number of s
+00005ba0: 6567 6d65 6e74 7320 696e 2074 6865 2032  egments in the 2
+00005bb0: 4420 6d61 7472 6978 0a20 2020 2020 2020  D matrix.       
+00005bc0: 206d 6574 686f 643a 2020 6372 6f73 732d   method:  cross-
+00005bd0: 636f 7272 656c 6174 696f 6e20 6d65 7468  correlation meth
+00005be0: 6f64 7320 7365 6c65 6374 6564 2062 7920  ods selected by 
+00005bf0: 7468 6520 7573 6572 0a20 2020 2020 2020  the user.       
+00005c00: 2066 7265 716d 696e 3a20 6d69 6e69 6d75   freqmin: minimu
+00005c10: 6d20 6672 6571 7565 6e63 7920 2848 7a29  m frequency (Hz)
+00005c20: 0a20 2020 2020 2020 2066 7265 716d 6178  .        freqmax
+00005c30: 3a20 6d61 7869 6d75 6d20 6672 6571 7565  : maximum freque
+00005c40: 6e63 7920 2848 7a29 0a20 2020 204e 6666  ncy (Hz).    Nff
+00005c50: 743a 2020 2020 6e75 6d62 6572 206f 6620  t:    number of 
+00005c60: 6672 6571 7565 6e63 7920 706f 696e 7473  frequency points
+00005c70: 2066 6f72 2069 6666 740a 2020 2020 6461   for ifft.    da
+00005c80: 7461 535f 743a 206d 6174 7269 7820 6f66  taS_t: matrix of
+00005c90: 2064 6174 6574 696d 6520 6f62 6a65 6374   datetime object
+00005ca0: 2e0a 0a20 2020 2052 4554 5552 4e53 3a0a  ...    RETURNS:.
+00005cb0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+00005cc0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 735f  ---------.    s_
+00005cd0: 636f 7272 3a20 3144 206f 7220 3244 206d  corr: 1D or 2D m
+00005ce0: 6174 7269 7820 6f66 2074 6865 2061 7665  atrix of the ave
+00005cf0: 7261 6765 6420 6f72 2073 7562 2d73 7461  raged or sub-sta
+00005d00: 636b 7320 6f66 2063 726f 7373 2d63 6f72  cks of cross-cor
+00005d10: 7265 6c61 7469 6f6e 2066 756e 6374 696f  relation functio
+00005d20: 6e73 2069 6e20 7469 6d65 2064 6f6d 6169  ns in time domai
+00005d30: 6e0a 2020 2020 745f 636f 7272 3a20 7469  n.    t_corr: ti
+00005d40: 6d65 7374 616d 7020 666f 7220 6561 6368  mestamp for each
+00005d50: 2073 7562 2d73 7461 636b 206f 7220 6176   sub-stack or av
+00005d60: 6572 6167 6564 2066 756e 6374 696f 6e0a  eraged function.
+00005d70: 2020 2020 6e5f 636f 7272 3a20 6e75 6d62      n_corr: numb
+00005d80: 6572 206f 6620 696e 636c 7564 6564 2073  er of included s
+00005d90: 6567 6d65 6e74 7320 666f 7220 6561 6368  egments for each
+00005da0: 2073 7562 2d73 7461 636b 206f 7220 6176   sub-stack or av
+00005db0: 6572 6167 6564 2066 756e 6374 696f 6e0a  eraged function.
+00005dc0: 0a20 2020 204d 4f44 4946 4943 4154 494f  .    MODIFICATIO
+00005dd0: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
+00005de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+00005df0: 2020 6f75 7470 7574 2074 6865 206c 696e    output the lin
+00005e00: 6561 7220 7374 6163 6b20 6f66 2065 6163  ear stack of eac
+00005e10: 6820 7469 6d65 2063 6875 6e6b 2065 7665  h time chunk eve
+00005e20: 6e20 7768 656e 2073 7562 7374 6163 6b20  n when substack 
+00005e30: 6973 2073 656c 6563 7465 6420 2862 7920  is selected (by 
+00005e40: 4368 656e 6778 696e 2040 4175 6732 3032  Chengxin @Aug202
+00005e50: 3029 0a20 2020 2022 2222 0a20 2020 2023  0).    """.    #
+00005e60: 202d 2d2d 2d6c 6f61 6420 7061 7261 6d74   ----load paramt
+00005e70: 6572 732d 2d2d 2d0a 2020 2020 6474 203d  ers----.    dt =
+00005e80: 2044 5b22 6474 225d 0a20 2020 206d 6178   D["dt"].    max
+00005e90: 6c61 6720 3d20 445b 226d 6178 6c61 6722  lag = D["maxlag"
+00005ea0: 5d0a 2020 2020 6d65 7468 6f64 203d 2044  ].    method = D
+00005eb0: 5b22 6363 5f6d 6574 686f 6422 5d0a 2020  ["cc_method"].  
+00005ec0: 2020 6363 5f6c 656e 203d 2044 5b22 6363    cc_len = D["cc
+00005ed0: 5f6c 656e 225d 0a20 2020 2073 7562 7374  _len"].    subst
+00005ee0: 6163 6b20 3d20 445b 2273 7562 7374 6163  ack = D["substac
+00005ef0: 6b22 5d0a 2020 2020 7375 6273 7461 636b  k"].    substack
+00005f00: 5f6c 656e 203d 2044 5b22 7375 6273 7461  _len = D["substa
+00005f10: 636b 5f6c 656e 225d 0a20 2020 2073 6d6f  ck_len"].    smo
+00005f20: 6f74 6873 7065 6374 5f4e 203d 2044 5b22  othspect_N = D["
+00005f30: 736d 6f6f 7468 7370 6563 745f 4e22 5d0a  smoothspect_N"].
+00005f40: 0a20 2020 206e 7769 6e20 3d20 6666 7431  .    nwin = fft1
+00005f50: 5f73 6d6f 6f74 6865 645f 6162 732e 7368  _smoothed_abs.sh
+00005f60: 6170 655b 305d 0a20 2020 204e 6666 7432  ape[0].    Nfft2
+00005f70: 203d 2066 6674 315f 736d 6f6f 7468 6564   = fft1_smoothed
+00005f80: 5f61 6273 2e73 6861 7065 5b31 5d0a 0a20  _abs.shape[1].. 
+00005f90: 2020 2023 202d 2d2d 2d2d 2d63 6f6e 7665     # ------conve
+00005fa0: 7274 2061 6c6c 2032 4420 6172 7261 7973  rt all 2D arrays
+00005fb0: 2069 6e74 6f20 3144 2074 6f20 7370 6565   into 1D to spee
+00005fc0: 6420 7570 2d2d 2d2d 2d2d 2d2d 0a20 2020  d up--------.   
+00005fd0: 2063 6f72 7220 3d20 6e70 2e7a 6572 6f73   corr = np.zeros
+00005fe0: 286e 7769 6e20 2a20 4e66 6674 322c 2064  (nwin * Nfft2, d
+00005ff0: 7479 7065 3d6e 702e 636f 6d70 6c65 7836  type=np.complex6
+00006000: 3429 0a20 2020 2063 6f72 7220 3d20 6666  4).    corr = ff
+00006010: 7431 5f73 6d6f 6f74 6865 645f 6162 732e  t1_smoothed_abs.
+00006020: 7265 7368 6170 6528 0a20 2020 2020 2020  reshape(.       
+00006030: 2066 6674 315f 736d 6f6f 7468 6564 5f61   fft1_smoothed_a
+00006040: 6273 2e73 697a 652c 0a20 2020 2029 202a  bs.size,.    ) *
+00006050: 2066 6674 322e 7265 7368 6170 6528 0a20   fft2.reshape(. 
+00006060: 2020 2020 2020 2066 6674 322e 7369 7a65         fft2.size
+00006070: 2c0a 2020 2020 290a 0a20 2020 2069 6620  ,.    )..    if 
+00006080: 6d65 7468 6f64 203d 3d20 2263 6f68 6572  method == "coher
+00006090: 656e 6379 223a 0a20 2020 2020 2020 2074  ency":.        t
+000060a0: 656d 7020 3d20 6d6f 7669 6e67 5f61 7665  emp = moving_ave
+000060b0: 280a 2020 2020 2020 2020 2020 2020 6e70  (.            np
+000060c0: 2e61 6273 280a 2020 2020 2020 2020 2020  .abs(.          
+000060d0: 2020 2020 2020 6666 7432 2e72 6573 6861        fft2.resha
+000060e0: 7065 280a 2020 2020 2020 2020 2020 2020  pe(.            
+000060f0: 2020 2020 2020 2020 6666 7432 2e73 697a          fft2.siz
+00006100: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00006110: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00006120: 2029 2c0a 2020 2020 2020 2020 2020 2020   ),.            
+00006130: 736d 6f6f 7468 7370 6563 745f 4e2c 0a20  smoothspect_N,. 
+00006140: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00006150: 2063 6f72 7220 2f3d 2074 656d 700a 2020   corr /= temp.  
+00006160: 2020 636f 7272 203d 2063 6f72 722e 7265    corr = corr.re
+00006170: 7368 6170 6528 6e77 696e 2c20 4e66 6674  shape(nwin, Nfft
+00006180: 3229 0a0a 2020 2020 6966 2073 7562 7374  2)..    if subst
+00006190: 6163 6b3a 0a20 2020 2020 2020 2069 6620  ack:.        if 
+000061a0: 7375 6273 7461 636b 5f6c 656e 203d 3d20  substack_len == 
+000061b0: 6363 5f6c 656e 3a0a 2020 2020 2020 2020  cc_len:.        
+000061c0: 2020 2020 2320 6368 6f6f 7365 2074 6f20      # choose to 
+000061d0: 6b65 6570 2061 6c6c 2066 6674 2064 6174  keep all fft dat
+000061e0: 6120 666f 7220 6120 6461 790a 2020 2020  a for a day.    
+000061f0: 2020 2020 2020 2020 735f 636f 7272 203d          s_corr =
+00006200: 206e 702e 7a65 726f 7328 7368 6170 653d   np.zeros(shape=
+00006210: 286e 7769 6e2c 204e 6666 7429 2c20 6474  (nwin, Nfft), dt
+00006220: 7970 653d 6e70 2e66 6c6f 6174 3332 2920  ype=np.float32) 
+00006230: 2023 2073 7461 636b 6564 2063 6f72 7265   # stacked corre
+00006240: 6c61 7469 6f6e 0a20 2020 2020 2020 2020  lation.         
+00006250: 2020 2061 6d70 6d61 7820 3d20 6e70 2e7a     ampmax = np.z
+00006260: 6572 6f73 286e 7769 6e2c 2064 7479 7065  eros(nwin, dtype
+00006270: 3d6e 702e 666c 6f61 7433 3229 0a20 2020  =np.float32).   
+00006280: 2020 2020 2020 2020 206e 5f63 6f72 7220           n_corr 
+00006290: 3d20 6e70 2e7a 6572 6f73 286e 7769 6e2c  = np.zeros(nwin,
+000062a0: 2064 7479 7065 3d6e 702e 696e 7431 3629   dtype=np.int16)
+000062b0: 2020 2320 6e75 6d62 6572 206f 6620 636f    # number of co
+000062c0: 7272 656c 6174 696f 6e73 2066 6f72 2065  rrelations for e
+000062d0: 6163 6820 7375 6273 7461 636b 0a20 2020  ach substack.   
+000062e0: 2020 2020 2020 2020 2074 5f63 6f72 7220           t_corr 
+000062f0: 3d20 6461 7461 535f 7420 2023 2074 696d  = dataS_t  # tim
+00006300: 6573 7461 6d70 0a20 2020 2020 2020 2020  estamp.         
+00006310: 2020 2063 7261 7020 3d20 6e70 2e7a 6572     crap = np.zer
+00006320: 6f73 284e 6666 742c 2064 7479 7065 3d6e  os(Nfft, dtype=n
+00006330: 702e 636f 6d70 6c65 7836 3429 0a20 2020  p.complex64).   
+00006340: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+00006350: 6e20 7261 6e67 6528 6e77 696e 293a 0a20  n range(nwin):. 
+00006360: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00006370: 5f63 6f72 725b 695d 203d 2031 0a20 2020  _corr[i] = 1.   
+00006380: 2020 2020 2020 2020 2020 2020 2063 7261               cra
+00006390: 705b 3a4e 6666 7432 5d20 3d20 636f 7272  p[:Nfft2] = corr
+000063a0: 5b69 2c20 3a5d 0a20 2020 2020 2020 2020  [i, :].         
+000063b0: 2020 2020 2020 2063 7261 705b 3a4e 6666         crap[:Nff
+000063c0: 7432 5d20 3d20 6372 6170 5b3a 4e66 6674  t2] = crap[:Nfft
+000063d0: 325d 202d 206e 702e 6d65 616e 2863 7261  2] - np.mean(cra
+000063e0: 705b 3a4e 6666 7432 5d29 2020 2320 7265  p[:Nfft2])  # re
+000063f0: 6d6f 7665 2074 6865 206d 6561 6e20 696e  move the mean in
+00006400: 2066 7265 7120 646f 6d61 696e 2028 7370   freq domain (sp
+00006410: 696b 6520 6174 2074 3d30 290a 2020 2020  ike at t=0).    
+00006420: 2020 2020 2020 2020 2020 2020 6372 6170              crap
+00006430: 5b2d 284e 6666 7432 2920 2b20 3120 3a5d  [-(Nfft2) + 1 :]
+00006440: 203d 206e 702e 666c 6970 286e 702e 636f   = np.flip(np.co
+00006450: 6e6a 2863 7261 705b 313a 284e 6666 7432  nj(crap[1:(Nfft2
+00006460: 295d 292c 2061 7869 733d 3029 0a20 2020  )]), axis=0).   
+00006470: 2020 2020 2020 2020 2020 2020 2063 7261               cra
+00006480: 705b 305d 203d 2063 6f6d 706c 6578 2830  p[0] = complex(0
+00006490: 2c20 3029 0a20 2020 2020 2020 2020 2020  , 0).           
+000064a0: 2020 2020 2073 5f63 6f72 725b 692c 203a       s_corr[i, :
+000064b0: 5d20 3d20 6e70 2e72 6561 6c28 6e70 2e66  ] = np.real(np.f
+000064c0: 6674 2e69 6666 7473 6869 6674 2873 6369  ft.ifftshift(sci
+000064d0: 7079 2e66 6674 7061 636b 2e69 6666 7428  py.fftpack.ifft(
+000064e0: 6372 6170 2c20 4e66 6674 2c20 6178 6973  crap, Nfft, axis
+000064f0: 3d30 2929 290a 0a20 2020 2020 2020 2020  =0)))..         
+00006500: 2020 2023 2072 656d 6f76 6520 6162 6e6f     # remove abno
+00006510: 726d 616c 2064 6174 610a 2020 2020 2020  rmal data.      
+00006520: 2020 2020 2020 616d 706d 6178 203d 206e        ampmax = n
+00006530: 702e 6d61 7828 735f 636f 7272 2c20 6178  p.max(s_corr, ax
+00006540: 6973 3d31 290a 2020 2020 2020 2020 2020  is=1).          
+00006550: 2020 7469 6e64 7820 3d20 6e70 2e77 6865    tindx = np.whe
+00006560: 7265 2828 616d 706d 6178 203c 2032 3020  re((ampmax < 20 
+00006570: 2a20 6e70 2e6d 6564 6961 6e28 616d 706d  * np.median(ampm
+00006580: 6178 2929 2026 2028 616d 706d 6178 203e  ax)) & (ampmax >
+00006590: 2030 2929 5b30 5d0a 2020 2020 2020 2020   0))[0].        
+000065a0: 2020 2020 735f 636f 7272 203d 2073 5f63      s_corr = s_c
+000065b0: 6f72 725b 7469 6e64 782c 203a 5d0a 2020  orr[tindx, :].  
+000065c0: 2020 2020 2020 2020 2020 745f 636f 7272            t_corr
+000065d0: 203d 2074 5f63 6f72 725b 7469 6e64 785d   = t_corr[tindx]
+000065e0: 0a20 2020 2020 2020 2020 2020 206e 5f63  .            n_c
+000065f0: 6f72 7220 3d20 6e5f 636f 7272 5b74 696e  orr = n_corr[tin
+00006600: 6478 5d0a 0a20 2020 2020 2020 2065 6c73  dx]..        els
+00006610: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
+00006620: 2067 6574 2074 696d 6520 696e 666f 726d   get time inform
+00006630: 6174 696f 6e0a 2020 2020 2020 2020 2020  ation.          
+00006640: 2020 5474 6f74 616c 203d 2064 6174 6153    Ttotal = dataS
+00006650: 5f74 5b2d 315d 202d 2064 6174 6153 5f74  _t[-1] - dataS_t
+00006660: 5b30 5d20 2023 2074 6f74 616c 2064 7572  [0]  # total dur
+00006670: 6174 696f 6e20 6f66 2077 6861 7420 7765  ation of what we
+00006680: 2068 6176 6520 6e6f 770a 2020 2020 2020   have now.      
+00006690: 2020 2020 2020 7473 7461 7274 203d 2064        tstart = d
+000066a0: 6174 6153 5f74 5b30 5d0a 0a20 2020 2020  ataS_t[0]..     
+000066b0: 2020 2020 2020 206e 7374 6163 6b20 3d20         nstack = 
+000066c0: 696e 7428 6e70 2e72 6f75 6e64 2854 746f  int(np.round(Tto
+000066d0: 7461 6c20 2f20 7375 6273 7461 636b 5f6c  tal / substack_l
+000066e0: 656e 2929 0a20 2020 2020 2020 2020 2020  en)).           
+000066f0: 2061 6d70 6d61 7820 3d20 6e70 2e7a 6572   ampmax = np.zer
+00006700: 6f73 286e 7374 6163 6b2c 2064 7479 7065  os(nstack, dtype
+00006710: 3d6e 702e 666c 6f61 7433 3229 0a20 2020  =np.float32).   
+00006720: 2020 2020 2020 2020 2073 5f63 6f72 7220           s_corr 
+00006730: 3d20 6e70 2e7a 6572 6f73 2873 6861 7065  = np.zeros(shape
+00006740: 3d28 6e73 7461 636b 2c20 4e66 6674 292c  =(nstack, Nfft),
+00006750: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+00006760: 3229 0a20 2020 2020 2020 2020 2020 206e  2).            n
+00006770: 5f63 6f72 7220 3d20 6e70 2e7a 6572 6f73  _corr = np.zeros
+00006780: 286e 7374 6163 6b2c 2064 7479 7065 3d6e  (nstack, dtype=n
+00006790: 702e 696e 7431 3629 0a20 2020 2020 2020  p.int16).       
+000067a0: 2020 2020 2074 5f63 6f72 7220 3d20 6e70       t_corr = np
+000067b0: 2e7a 6572 6f73 286e 7374 6163 6b2c 2064  .zeros(nstack, d
+000067c0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
+000067d0: 0a20 2020 2020 2020 2020 2020 2063 7261  .            cra
+000067e0: 7020 3d20 6e70 2e7a 6572 6f73 284e 6666  p = np.zeros(Nff
+000067f0: 742c 2064 7479 7065 3d6e 702e 636f 6d70  t, dtype=np.comp
+00006800: 6c65 7836 3429 0a0a 2020 2020 2020 2020  lex64)..        
+00006810: 2020 2020 666f 7220 6973 7461 636b 2069      for istack i
+00006820: 6e20 7261 6e67 6528 6e73 7461 636b 293a  n range(nstack):
+00006830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006840: 2023 2066 696e 6420 7468 6520 696e 6465   # find the inde
+00006850: 7865 7320 6f66 2061 6c6c 206f 6620 7468  xes of all of th
+00006860: 6520 7769 6e64 6f77 7320 7468 6174 2073  e windows that s
+00006870: 7461 7274 206f 7220 656e 6420 7769 7468  tart or end with
+00006880: 696e 0a20 2020 2020 2020 2020 2020 2020  in.             
+00006890: 2020 2069 7469 6d65 203d 206e 702e 7768     itime = np.wh
+000068a0: 6572 6528 2864 6174 6153 5f74 203e 3d20  ere((dataS_t >= 
+000068b0: 7473 7461 7274 2920 2620 2864 6174 6153  tstart) & (dataS
+000068c0: 5f74 203c 2074 7374 6172 7420 2b20 7375  _t < tstart + su
+000068d0: 6273 7461 636b 5f6c 656e 2929 5b30 5d0a  bstack_len))[0].
+000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068f0: 6966 206c 656e 2869 7469 6d65 2920 3d3d  if len(itime) ==
+00006900: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00006910: 2020 2020 2020 2020 7473 7461 7274 202b          tstart +
+00006920: 3d20 7375 6273 7461 636b 5f6c 656e 0a20  = substack_len. 
+00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006940: 2020 2063 6f6e 7469 6e75 650a 0a20 2020     continue..   
+00006950: 2020 2020 2020 2020 2020 2020 2063 7261               cra
+00006960: 705b 3a4e 6666 7432 5d20 3d20 6e70 2e6d  p[:Nfft2] = np.m
+00006970: 6561 6e28 636f 7272 5b69 7469 6d65 2c20  ean(corr[itime, 
+00006980: 3a5d 2c20 6178 6973 3d30 2920 2023 206c  :], axis=0)  # l
+00006990: 696e 6561 7220 6176 6572 6167 6520 6f66  inear average of
+000069a0: 2074 6865 2063 6f72 7265 6c61 7469 6f6e   the correlation
+000069b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000069c0: 2063 7261 705b 3a4e 6666 7432 5d20 3d20   crap[:Nfft2] = 
+000069d0: 6372 6170 5b3a 4e66 6674 325d 202d 206e  crap[:Nfft2] - n
+000069e0: 702e 6d65 616e 2863 7261 705b 3a4e 6666  p.mean(crap[:Nff
+000069f0: 7432 5d29 2020 2320 7265 6d6f 7665 2074  t2])  # remove t
+00006a00: 6865 206d 6561 6e20 696e 2066 7265 7120  he mean in freq 
+00006a10: 646f 6d61 696e 2028 7370 696b 6520 6174  domain (spike at
+00006a20: 2074 3d30 290a 2020 2020 2020 2020 2020   t=0).          
+00006a30: 2020 2020 2020 6372 6170 5b2d 284e 6666        crap[-(Nff
+00006a40: 7432 2920 2b20 3120 3a5d 203d 206e 702e  t2) + 1 :] = np.
+00006a50: 666c 6970 286e 702e 636f 6e6a 2863 7261  flip(np.conj(cra
+00006a60: 705b 313a 284e 6666 7432 295d 292c 2061  p[1:(Nfft2)]), a
+00006a70: 7869 733d 3029 0a20 2020 2020 2020 2020  xis=0).         
+00006a80: 2020 2020 2020 2063 7261 705b 305d 203d         crap[0] =
+00006a90: 2063 6f6d 706c 6578 2830 2c20 3029 0a20   complex(0, 0). 
+00006aa0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00006ab0: 5f63 6f72 725b 6973 7461 636b 2c20 3a5d  _corr[istack, :]
+00006ac0: 203d 206e 702e 7265 616c 286e 702e 6666   = np.real(np.ff
+00006ad0: 742e 6966 6674 7368 6966 7428 7363 6970  t.ifftshift(scip
+00006ae0: 792e 6666 7470 6163 6b2e 6966 6674 2863  y.fftpack.ifft(c
+00006af0: 7261 702c 204e 6666 742c 2061 7869 733d  rap, Nfft, axis=
+00006b00: 3029 2929 0a20 2020 2020 2020 2020 2020  0))).           
+00006b10: 2020 2020 206e 5f63 6f72 725b 6973 7461       n_corr[ista
+00006b20: 636b 5d20 3d20 6c65 6e28 6974 696d 6529  ck] = len(itime)
+00006b30: 2020 2320 6e75 6d62 6572 206f 6620 7769    # number of wi
+00006b40: 6e64 6f77 7320 7374 6163 6b73 0a20 2020  ndows stacks.   
+00006b50: 2020 2020 2020 2020 2020 2020 2074 5f63               t_c
+00006b60: 6f72 725b 6973 7461 636b 5d20 3d20 7473  orr[istack] = ts
+00006b70: 7461 7274 2020 2320 7361 7665 2074 6865  tart  # save the
+00006b80: 2074 696d 6520 7374 616d 7073 0a20 2020   time stamps.   
+00006b90: 2020 2020 2020 2020 2020 2020 2074 7374               tst
+00006ba0: 6172 7420 2b3d 2073 7562 7374 6163 6b5f  art += substack_
+00006bb0: 6c65 6e0a 2020 2020 2020 2020 2020 2020  len.            
+00006bc0: 2020 2020 2320 7072 696e 7428 2763 6f72      # print('cor
+00006bd0: 7265 6c61 7469 6f6e 2064 6f6e 6520 616e  relation done an
+00006be0: 6420 7374 6163 6b65 6420 6174 2074 696d  d stacked at tim
+00006bf0: 6520 2573 2720 2520 7374 7228 745f 636f  e %s' % str(t_co
+00006c00: 7272 5b69 7374 6163 6b5d 2929 0a0a 2020  rr[istack]))..  
+00006c10: 2020 2020 2020 2020 2020 2320 7265 6d6f            # remo
+00006c20: 7665 2061 626e 6f72 6d61 6c20 6461 7461  ve abnormal data
+00006c30: 0a20 2020 2020 2020 2020 2020 2061 6d70  .            amp
+00006c40: 6d61 7820 3d20 6e70 2e6d 6178 2873 5f63  max = np.max(s_c
+00006c50: 6f72 722c 2061 7869 733d 3129 0a20 2020  orr, axis=1).   
+00006c60: 2020 2020 2020 2020 2074 696e 6478 203d           tindx =
+00006c70: 206e 702e 7768 6572 6528 2861 6d70 6d61   np.where((ampma
+00006c80: 7820 3c20 3230 202a 206e 702e 6d65 6469  x < 20 * np.medi
+00006c90: 616e 2861 6d70 6d61 7829 2920 2620 2861  an(ampmax)) & (a
+00006ca0: 6d70 6d61 7820 3e20 3029 295b 305d 0a20  mpmax > 0))[0]. 
+00006cb0: 2020 2020 2020 2020 2020 2073 5f63 6f72             s_cor
+00006cc0: 7220 3d20 735f 636f 7272 5b74 696e 6478  r = s_corr[tindx
+00006cd0: 2c20 3a5d 0a20 2020 2020 2020 2020 2020  , :].           
+00006ce0: 2074 5f63 6f72 7220 3d20 745f 636f 7272   t_corr = t_corr
+00006cf0: 5b74 696e 6478 5d0a 2020 2020 2020 2020  [tindx].        
+00006d00: 2020 2020 6e5f 636f 7272 203d 206e 5f63      n_corr = n_c
+00006d10: 6f72 725b 7469 6e64 785d 0a0a 2020 2020  orr[tindx]..    
+00006d20: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
+00006d30: 6176 6572 6167 6520 6461 696c 7920 6372  average daily cr
+00006d40: 6f73 7320 636f 7272 656c 6174 696f 6e20  oss correlation 
+00006d50: 6675 6e63 7469 6f6e 730a 2020 2020 2020  functions.      
+00006d60: 2020 616d 706d 6178 203d 206e 702e 6d61    ampmax = np.ma
+00006d70: 7828 636f 7272 2c20 6178 6973 3d31 290a  x(corr, axis=1).
+00006d80: 2020 2020 2020 2020 7469 6e64 7820 3d20          tindx = 
+00006d90: 6e70 2e77 6865 7265 2828 616d 706d 6178  np.where((ampmax
+00006da0: 203c 2032 3020 2a20 6e70 2e6d 6564 6961   < 20 * np.media
+00006db0: 6e28 616d 706d 6178 2929 2026 2028 616d  n(ampmax)) & (am
+00006dc0: 706d 6178 203e 2030 2929 5b30 5d0a 2020  pmax > 0))[0].  
+00006dd0: 2020 2020 2020 6e5f 636f 7272 203d 206e        n_corr = n
+00006de0: 7769 6e0a 2020 2020 2020 2020 735f 636f  win.        s_co
+00006df0: 7272 203d 206e 702e 7a65 726f 7328 4e66  rr = np.zeros(Nf
+00006e00: 6674 2c20 6474 7970 653d 6e70 2e66 6c6f  ft, dtype=np.flo
+00006e10: 6174 3332 290a 2020 2020 2020 2020 745f  at32).        t_
+00006e20: 636f 7272 203d 2064 6174 6153 5f74 5b30  corr = dataS_t[0
+00006e30: 5d0a 2020 2020 2020 2020 6372 6170 203d  ].        crap =
+00006e40: 206e 702e 7a65 726f 7328 4e66 6674 2c20   np.zeros(Nfft, 
+00006e50: 6474 7970 653d 6e70 2e63 6f6d 706c 6578  dtype=np.complex
+00006e60: 3634 290a 2020 2020 2020 2020 6372 6170  64).        crap
+00006e70: 5b3a 4e66 6674 325d 203d 206e 702e 6d65  [:Nfft2] = np.me
+00006e80: 616e 2863 6f72 725b 7469 6e64 785d 2c20  an(corr[tindx], 
+00006e90: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
+00006ea0: 6372 6170 5b3a 4e66 6674 325d 203d 2063  crap[:Nfft2] = c
+00006eb0: 7261 705b 3a4e 6666 7432 5d20 2d20 6e70  rap[:Nfft2] - np
+00006ec0: 2e6d 6561 6e28 6372 6170 5b3a 4e66 6674  .mean(crap[:Nfft
+00006ed0: 325d 2c20 6178 6973 3d30 290a 2020 2020  2], axis=0).    
+00006ee0: 2020 2020 6372 6170 5b2d 284e 6666 7432      crap[-(Nfft2
+00006ef0: 2920 2b20 3120 3a5d 203d 206e 702e 666c  ) + 1 :] = np.fl
+00006f00: 6970 286e 702e 636f 6e6a 2863 7261 705b  ip(np.conj(crap[
+00006f10: 313a 284e 6666 7432 295d 292c 2061 7869  1:(Nfft2)]), axi
+00006f20: 733d 3029 0a20 2020 2020 2020 2073 5f63  s=0).        s_c
+00006f30: 6f72 7220 3d20 6e70 2e72 6561 6c28 6e70  orr = np.real(np
+00006f40: 2e66 6674 2e69 6666 7473 6869 6674 2873  .fft.ifftshift(s
+00006f50: 6369 7079 2e66 6674 7061 636b 2e69 6666  cipy.fftpack.iff
+00006f60: 7428 6372 6170 2c20 4e66 6674 2c20 6178  t(crap, Nfft, ax
+00006f70: 6973 3d30 2929 290a 0a20 2020 2023 2074  is=0)))..    # t
+00006f80: 7269 6d20 7468 6520 4343 4673 2069 6e20  rim the CCFs in 
+00006f90: 5b2d 6d61 786c 6167 206d 6178 6c61 675d  [-maxlag maxlag]
+00006fa0: 0a20 2020 2074 203d 206e 702e 6172 616e  .    t = np.aran
+00006fb0: 6765 282d 4e66 6674 3220 2b20 312c 204e  ge(-Nfft2 + 1, N
+00006fc0: 6666 7432 2920 2a20 6474 0a20 2020 2069  fft2) * dt.    i
+00006fd0: 6e64 203d 206e 702e 7768 6572 6528 6e70  nd = np.where(np
+00006fe0: 2e61 6273 2874 2920 3c3d 206d 6178 6c61  .abs(t) <= maxla
+00006ff0: 6729 5b30 5d0a 2020 2020 6966 2073 5f63  g)[0].    if s_c
+00007000: 6f72 722e 6e64 696d 203d 3d20 313a 0a20  orr.ndim == 1:. 
+00007010: 2020 2020 2020 2073 5f63 6f72 7220 3d20         s_corr = 
+00007020: 735f 636f 7272 5b69 6e64 5d0a 2020 2020  s_corr[ind].    
+00007030: 656c 6966 2073 5f63 6f72 722e 6e64 696d  elif s_corr.ndim
+00007040: 203d 3d20 323a 0a20 2020 2020 2020 2073   == 2:.        s
+00007050: 5f63 6f72 7220 3d20 735f 636f 7272 5b3a  _corr = s_corr[:
+00007060: 2c20 696e 645d 0a20 2020 2072 6574 7572  , ind].    retur
+00007070: 6e20 735f 636f 7272 2c20 745f 636f 7272  n s_corr, t_corr
+00007080: 2c20 6e5f 636f 7272 0a0a 0a64 6566 2063  , n_corr...def c
+00007090: 6f72 7265 6c61 7465 5f6e 6f6e 6c69 6e65  orrelate_nonline
+000070a0: 6172 5f73 7461 636b 2866 6674 315f 736d  ar_stack(fft1_sm
+000070b0: 6f6f 7468 6564 5f61 6273 2c20 6666 7432  oothed_abs, fft2
+000070c0: 2c20 442c 204e 6666 742c 2064 6174 6153  , D, Nfft, dataS
+000070d0: 5f74 293a 0a20 2020 2022 2222 0a20 2020  _t):.    """.   
+000070e0: 2074 6869 7320 6675 6e63 7469 6f6e 2064   this function d
+000070f0: 6f65 7320 7468 6520 6372 6f73 732d 636f  oes the cross-co
+00007100: 7272 656c 6174 696f 6e20 696e 2066 7265  rrelation in fre
+00007110: 7120 646f 6d61 696e 2061 6e64 2068 6173  q domain and has
+00007120: 2074 6865 206f 7074 696f 6e20 746f 206b   the option to k
+00007130: 6565 7020 7375 622d 7374 6163 6b73 206f  eep sub-stacks o
+00007140: 660a 2020 2020 7468 6520 6372 6f73 732d  f.    the cross-
+00007150: 636f 7272 656c 6174 696f 6e20 6966 206e  correlation if n
+00007160: 6565 6465 642e 2069 7420 7461 6b65 7320  eeded. it takes 
+00007170: 6164 7661 6e74 6167 6520 6f66 2074 6865  advantage of the
+00007180: 206c 696e 6561 7220 7265 6c61 7469 6f6e   linear relation
+00007190: 7368 6970 206f 6620 6966 6674 2c20 736f  ship of ifft, so
+000071a0: 2074 6861 740a 2020 2020 7374 6163 6b69   that.    stacki
+000071b0: 6e67 2069 7320 7065 7266 6f72 6d65 6420  ng is performed 
+000071c0: 696e 2073 7065 6374 7275 6d20 646f 6d61  in spectrum doma
+000071d0: 696e 2066 6972 7374 2074 6f20 7265 6475  in first to redu
+000071e0: 6365 2074 6865 2074 6f74 616c 206e 756d  ce the total num
+000071f0: 6265 7220 6f66 2069 6666 742e 2028 7573  ber of ifft. (us
+00007200: 6564 2069 6e20 5331 290a 2020 2020 5041  ed in S1).    PA
+00007210: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
+00007220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007230: 2d2d 2d0a 2020 2020 6666 7431 5f73 6d6f  ---.    fft1_smo
+00007240: 6f74 6865 645f 6162 733a 2073 6d6f 6f74  othed_abs: smoot
+00007250: 6865 6420 706f 7765 7220 7370 6563 7472  hed power spectr
+00007260: 616c 2064 656e 7369 7479 206f 6620 7468  al density of th
+00007270: 6520 4646 5420 666f 7220 7468 6520 736f  e FFT for the so
+00007280: 7572 6365 2073 7461 7469 6f6e 0a20 2020  urce station.   
+00007290: 2066 6674 323a 2072 6177 2046 4654 2073   fft2: raw FFT s
+000072a0: 7065 6374 7275 6d20 6f66 2074 6865 2072  pectrum of the r
+000072b0: 6563 6569 7665 7220 7374 6174 696f 6e0a  eceiver station.
+000072c0: 2020 2020 443a 2064 6963 7469 6f6e 6172      D: dictionar
+000072d0: 7920 636f 6e74 6169 6e69 6e67 2066 6f6c  y containing fol
+000072e0: 6c6f 7769 6e67 2070 6172 616d 6574 6572  lowing parameter
+000072f0: 733a 0a20 2020 2020 2020 206d 6178 6c61  s:.        maxla
+00007300: 673a 2020 6d61 7869 6d75 6d20 6c61 6773  g:  maximum lags
+00007310: 2074 6f20 6b65 6570 2069 6e20 7468 6520   to keep in the 
+00007320: 6372 6f73 7320 636f 7272 656c 6174 696f  cross correlatio
+00007330: 6e0a 2020 2020 2020 2020 6474 3a20 2020  n.        dt:   
+00007340: 2020 2073 616d 706c 696e 6720 7261 7465     sampling rate
+00007350: 2028 696e 2073 290a 2020 2020 2020 2020   (in s).        
+00007360: 6e77 696e 3a20 2020 206e 756d 6265 7220  nwin:    number 
+00007370: 6f66 2073 6567 6d65 6e74 7320 696e 2074  of segments in t
+00007380: 6865 2032 4420 6d61 7472 6978 0a20 2020  he 2D matrix.   
+00007390: 2020 2020 206d 6574 686f 643a 2020 6372       method:  cr
+000073a0: 6f73 732d 636f 7272 656c 6174 696f 6e20  oss-correlation 
+000073b0: 6d65 7468 6f64 7320 7365 6c65 6374 6564  methods selected
+000073c0: 2062 7920 7468 6520 7573 6572 0a20 2020   by the user.   
+000073d0: 2020 2020 2066 7265 716d 696e 3a20 6d69       freqmin: mi
+000073e0: 6e69 6d75 6d20 6672 6571 7565 6e63 7920  nimum frequency 
+000073f0: 2848 7a29 0a20 2020 2020 2020 2066 7265  (Hz).        fre
+00007400: 716d 6178 3a20 6d61 7869 6d75 6d20 6672  qmax: maximum fr
+00007410: 6571 7565 6e63 7920 2848 7a29 0a20 2020  equency (Hz).   
+00007420: 204e 6666 743a 2020 2020 6e75 6d62 6572   Nfft:    number
+00007430: 206f 6620 6672 6571 7565 6e63 7920 706f   of frequency po
+00007440: 696e 7473 2066 6f72 2069 6666 740a 2020  ints for ifft.  
+00007450: 2020 6461 7461 535f 743a 206d 6174 7269    dataS_t: matri
+00007460: 7820 6f66 2064 6174 6574 696d 6520 6f62  x of datetime ob
+00007470: 6a65 6374 2e0a 2020 2020 5245 5455 524e  ject..    RETURN
+00007480: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+00007490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+000074a0: 2073 5f63 6f72 723a 2031 4420 6f72 2032   s_corr: 1D or 2
+000074b0: 4420 6d61 7472 6978 206f 6620 7468 6520  D matrix of the 
+000074c0: 6176 6572 6167 6564 206f 7220 7375 622d  averaged or sub-
+000074d0: 7374 6163 6b73 206f 6620 6372 6f73 732d  stacks of cross-
+000074e0: 636f 7272 656c 6174 696f 6e20 6675 6e63  correlation func
+000074f0: 7469 6f6e 7320 696e 2074 696d 6520 646f  tions in time do
+00007500: 6d61 696e 0a20 2020 2074 5f63 6f72 723a  main.    t_corr:
+00007510: 2074 696d 6573 7461 6d70 2066 6f72 2065   timestamp for e
+00007520: 6163 6820 7375 622d 7374 6163 6b20 6f72  ach sub-stack or
+00007530: 2061 7665 7261 6765 6420 6675 6e63 7469   averaged functi
+00007540: 6f6e 0a20 2020 206e 5f63 6f72 723a 206e  on.    n_corr: n
+00007550: 756d 6265 7220 6f66 2069 6e63 6c75 6465  umber of include
+00007560: 6420 7365 676d 656e 7473 2066 6f72 2065  d segments for e
+00007570: 6163 6820 7375 622d 7374 6163 6b20 6f72  ach sub-stack or
+00007580: 2061 7665 7261 6765 6420 6675 6e63 7469   averaged functi
+00007590: 6f6e 0a20 2020 2022 2222 0a20 2020 2023  on.    """.    #
+000075a0: 202d 2d2d 2d6c 6f61 6420 7061 7261 6d74   ----load paramt
+000075b0: 6572 732d 2d2d 2d0a 2020 2020 6474 203d  ers----.    dt =
+000075c0: 2044 5b22 6474 225d 0a20 2020 206d 6178   D["dt"].    max
+000075d0: 6c61 6720 3d20 445b 226d 6178 6c61 6722  lag = D["maxlag"
+000075e0: 5d0a 2020 2020 6d65 7468 6f64 203d 2044  ].    method = D
+000075f0: 5b22 6363 5f6d 6574 686f 6422 5d0a 2020  ["cc_method"].  
+00007600: 2020 6363 5f6c 656e 203d 2044 5b22 6363    cc_len = D["cc
+00007610: 5f6c 656e 225d 0a20 2020 2073 7562 7374  _len"].    subst
+00007620: 6163 6b20 3d20 445b 2273 7562 7374 6163  ack = D["substac
+00007630: 6b22 5d0a 2020 2020 7374 6163 6b5f 6d65  k"].    stack_me
+00007640: 7468 6f64 203d 2044 5b22 7374 6163 6b5f  thod = D["stack_
+00007650: 6d65 7468 6f64 225d 0a20 2020 2073 7562  method"].    sub
+00007660: 7374 6163 6b5f 6c65 6e20 3d20 445b 2273  stack_len = D["s
+00007670: 7562 7374 6163 6b5f 6c65 6e22 5d0a 2020  ubstack_len"].  
+00007680: 2020 736d 6f6f 7468 7370 6563 745f 4e20    smoothspect_N 
+00007690: 3d20 445b 2273 6d6f 6f74 6873 7065 6374  = D["smoothspect
+000076a0: 5f4e 225d 0a0a 2020 2020 6e77 696e 203d  _N"]..    nwin =
+000076b0: 2066 6674 315f 736d 6f6f 7468 6564 5f61   fft1_smoothed_a
+000076c0: 6273 2e73 6861 7065 5b30 5d0a 2020 2020  bs.shape[0].    
+000076d0: 4e66 6674 3220 3d20 6666 7431 5f73 6d6f  Nfft2 = fft1_smo
+000076e0: 6f74 6865 645f 6162 732e 7368 6170 655b  othed_abs.shape[
+000076f0: 315d 0a0a 2020 2020 2320 2d2d 2d2d 2d2d  1]..    # ------
+00007700: 636f 6e76 6572 7420 616c 6c20 3244 2061  convert all 2D a
+00007710: 7272 6179 7320 696e 746f 2031 4420 746f  rrays into 1D to
+00007720: 2073 7065 6564 2075 702d 2d2d 2d2d 2d2d   speed up-------
+00007730: 2d0a 2020 2020 636f 7272 203d 206e 702e  -.    corr = np.
+00007740: 7a65 726f 7328 6e77 696e 202a 204e 6666  zeros(nwin * Nff
+00007750: 7432 2c20 6474 7970 653d 6e70 2e63 6f6d  t2, dtype=np.com
+00007760: 706c 6578 3634 290a 2020 2020 636f 7272  plex64).    corr
+00007770: 203d 2066 6674 315f 736d 6f6f 7468 6564   = fft1_smoothed
+00007780: 5f61 6273 2e72 6573 6861 7065 280a 2020  _abs.reshape(.  
+00007790: 2020 2020 2020 6666 7431 5f73 6d6f 6f74        fft1_smoot
+000077a0: 6865 645f 6162 732e 7369 7a65 2c0a 2020  hed_abs.size,.  
+000077b0: 2020 2920 2a20 6666 7432 2e72 6573 6861    ) * fft2.resha
+000077c0: 7065 280a 2020 2020 2020 2020 6666 7432  pe(.        fft2
+000077d0: 2e73 697a 652c 0a20 2020 2029 0a0a 2020  .size,.    )..  
+000077e0: 2020 2320 6e6f 726d 616c 697a 6520 6279    # normalize by
+000077f0: 2072 6563 6569 7665 7220 7370 6563 7472   receiver spectr
+00007800: 616c 2066 6f72 2063 6f68 6572 656e 6379  al for coherency
+00007810: 0a20 2020 2069 6620 6d65 7468 6f64 203d  .    if method =
+00007820: 3d20 2263 6f68 6572 656e 6379 223a 0a20  = "coherency":. 
+00007830: 2020 2020 2020 2074 656d 7020 3d20 6d6f         temp = mo
+00007840: 7669 6e67 5f61 7665 280a 2020 2020 2020  ving_ave(.      
+00007850: 2020 2020 2020 6e70 2e61 6273 280a 2020        np.abs(.  
+00007860: 2020 2020 2020 2020 2020 2020 2020 6666                ff
+00007870: 7432 2e72 6573 6861 7065 280a 2020 2020  t2.reshape(.    
+00007880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007890: 6666 7432 2e73 697a 652c 0a20 2020 2020  fft2.size,.     
+000078a0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000078b0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+000078c0: 2020 2020 2020 2020 736d 6f6f 7468 7370          smoothsp
+000078d0: 6563 745f 4e2c 0a20 2020 2020 2020 2029  ect_N,.        )
+000078e0: 0a20 2020 2020 2020 2063 6f72 7220 2f3d  .        corr /=
+000078f0: 2074 656d 700a 2020 2020 636f 7272 203d   temp.    corr =
+00007900: 2063 6f72 722e 7265 7368 6170 6528 6e77   corr.reshape(nw
+00007910: 696e 2c20 4e66 6674 3229 0a0a 2020 2020  in, Nfft2)..    
+00007920: 2320 7472 616e 7366 6f72 6d20 6261 636b  # transform back
+00007930: 2074 6f20 7469 6d65 2064 6f6d 6169 6e20   to time domain 
+00007940: 7761 7665 666f 726d 730a 2020 2020 735f  waveforms.    s_
+00007950: 636f 7272 203d 206e 702e 7a65 726f 7328  corr = np.zeros(
+00007960: 7368 6170 653d 286e 7769 6e2c 204e 6666  shape=(nwin, Nff
+00007970: 7429 2c20 6474 7970 653d 6e70 2e66 6c6f  t), dtype=np.flo
+00007980: 6174 3332 2920 2023 2073 7461 636b 6564  at32)  # stacked
+00007990: 2063 6f72 7265 6c61 7469 6f6e 0a20 2020   correlation.   
+000079a0: 2061 6d70 6d61 7820 3d20 6e70 2e7a 6572   ampmax = np.zer
+000079b0: 6f73 286e 7769 6e2c 2064 7479 7065 3d6e  os(nwin, dtype=n
+000079c0: 702e 666c 6f61 7433 3229 0a20 2020 206e  p.float32).    n
+000079d0: 5f63 6f72 7220 3d20 6e70 2e7a 6572 6f73  _corr = np.zeros
+000079e0: 286e 7769 6e2c 2064 7479 7065 3d6e 702e  (nwin, dtype=np.
+000079f0: 696e 7431 3629 2020 2320 6e75 6d62 6572  int16)  # number
+00007a00: 206f 6620 636f 7272 656c 6174 696f 6e73   of correlations
+00007a10: 2066 6f72 2065 6163 6820 7375 6273 7461   for each substa
+00007a20: 636b 0a20 2020 2074 5f63 6f72 7220 3d20  ck.    t_corr = 
+00007a30: 6461 7461 535f 7420 2023 2074 696d 6573  dataS_t  # times
+00007a40: 7461 6d70 0a20 2020 2063 7261 7020 3d20  tamp.    crap = 
+00007a50: 6e70 2e7a 6572 6f73 284e 6666 742c 2064  np.zeros(Nfft, d
+00007a60: 7479 7065 3d6e 702e 636f 6d70 6c65 7836  type=np.complex6
+00007a70: 3429 0a20 2020 2066 6f72 2069 2069 6e20  4).    for i in 
+00007a80: 7261 6e67 6528 6e77 696e 293a 0a20 2020  range(nwin):.   
+00007a90: 2020 2020 206e 5f63 6f72 725b 695d 203d       n_corr[i] =
+00007aa0: 2031 0a20 2020 2020 2020 2063 7261 705b   1.        crap[
+00007ab0: 3a4e 6666 7432 5d20 3d20 636f 7272 5b69  :Nfft2] = corr[i
+00007ac0: 2c20 3a5d 0a20 2020 2020 2020 2063 7261  , :].        cra
+00007ad0: 705b 3a4e 6666 7432 5d20 3d20 6372 6170  p[:Nfft2] = crap
+00007ae0: 5b3a 4e66 6674 325d 202d 206e 702e 6d65  [:Nfft2] - np.me
+00007af0: 616e 2863 7261 705b 3a4e 6666 7432 5d29  an(crap[:Nfft2])
+00007b00: 2020 2320 7265 6d6f 7665 2074 6865 206d    # remove the m
+00007b10: 6561 6e20 696e 2066 7265 7120 646f 6d61  ean in freq doma
+00007b20: 696e 2028 7370 696b 6520 6174 2074 3d30  in (spike at t=0
+00007b30: 290a 2020 2020 2020 2020 6372 6170 5b2d  ).        crap[-
+00007b40: 284e 6666 7432 2920 2b20 3120 3a5d 203d  (Nfft2) + 1 :] =
+00007b50: 206e 702e 666c 6970 286e 702e 636f 6e6a   np.flip(np.conj
+00007b60: 2863 7261 705b 313a 284e 6666 7432 295d  (crap[1:(Nfft2)]
+00007b70: 292c 2061 7869 733d 3029 0a20 2020 2020  ), axis=0).     
+00007b80: 2020 2063 7261 705b 305d 203d 2063 6f6d     crap[0] = com
+00007b90: 706c 6578 2830 2c20 3029 0a20 2020 2020  plex(0, 0).     
+00007ba0: 2020 2073 5f63 6f72 725b 692c 203a 5d20     s_corr[i, :] 
+00007bb0: 3d20 6e70 2e72 6561 6c28 6e70 2e66 6674  = np.real(np.fft
+00007bc0: 2e69 6666 7473 6869 6674 2873 6369 7079  .ifftshift(scipy
+00007bd0: 2e66 6674 7061 636b 2e69 6666 7428 6372  .fftpack.ifft(cr
+00007be0: 6170 2c20 4e66 6674 2c20 6178 6973 3d30  ap, Nfft, axis=0
+00007bf0: 2929 290a 0a20 2020 206e 735f 636f 7272  )))..    ns_corr
+00007c00: 203d 2073 5f63 6f72 720a 2020 2020 666f   = s_corr.    fo
+00007c10: 7220 6969 6920 696e 2072 616e 6765 286e  r iii in range(n
+00007c20: 735f 636f 7272 2e73 6861 7065 5b30 5d29  s_corr.shape[0])
+00007c30: 3a0a 2020 2020 2020 2020 6e73 5f63 6f72  :.        ns_cor
+00007c40: 725b 6969 695d 202f 3d20 6e70 2e6d 6178  r[iii] /= np.max
+00007c50: 286e 702e 6162 7328 6e73 5f63 6f72 725b  (np.abs(ns_corr[
+00007c60: 6969 695d 2929 0a0a 2020 2020 6966 2073  iii]))..    if s
+00007c70: 7562 7374 6163 6b3a 0a20 2020 2020 2020  ubstack:.       
+00007c80: 2069 6620 7375 6273 7461 636b 5f6c 656e   if substack_len
+00007c90: 203d 3d20 6363 5f6c 656e 3a0a 2020 2020   == cc_len:.    
+00007ca0: 2020 2020 2020 2020 2320 7265 6d6f 7665          # remove
+00007cb0: 2061 626e 6f72 6d61 6c20 6461 7461 0a20   abnormal data. 
+00007cc0: 2020 2020 2020 2020 2020 2061 6d70 6d61             ampma
+00007cd0: 7820 3d20 6e70 2e6d 6178 2873 5f63 6f72  x = np.max(s_cor
+00007ce0: 722c 2061 7869 733d 3129 0a20 2020 2020  r, axis=1).     
+00007cf0: 2020 2020 2020 2074 696e 6478 203d 206e         tindx = n
+00007d00: 702e 7768 6572 6528 2861 6d70 6d61 7820  p.where((ampmax 
+00007d10: 3c20 3230 202a 206e 702e 6d65 6469 616e  < 20 * np.median
+00007d20: 2861 6d70 6d61 7829 2920 2620 2861 6d70  (ampmax)) & (amp
+00007d30: 6d61 7820 3e20 3029 295b 305d 0a20 2020  max > 0))[0].   
+00007d40: 2020 2020 2020 2020 2073 5f63 6f72 7220           s_corr 
+00007d50: 3d20 735f 636f 7272 5b74 696e 6478 2c20  = s_corr[tindx, 
+00007d60: 3a5d 0a20 2020 2020 2020 2020 2020 2074  :].            t
+00007d70: 5f63 6f72 7220 3d20 745f 636f 7272 5b74  _corr = t_corr[t
+00007d80: 696e 6478 5d0a 2020 2020 2020 2020 2020  indx].          
+00007d90: 2020 6e5f 636f 7272 203d 206e 5f63 6f72    n_corr = n_cor
+00007da0: 725b 7469 6e64 785d 0a0a 2020 2020 2020  r[tindx]..      
+00007db0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00007dc0: 2020 2020 2320 6765 7420 7469 6d65 2069      # get time i
+00007dd0: 6e66 6f72 6d61 7469 6f6e 0a20 2020 2020  nformation.     
+00007de0: 2020 2020 2020 2054 746f 7461 6c20 3d20         Ttotal = 
+00007df0: 6461 7461 535f 745b 2d31 5d20 2d20 6461  dataS_t[-1] - da
+00007e00: 7461 535f 745b 305d 2020 2320 746f 7461  taS_t[0]  # tota
+00007e10: 6c20 6475 7261 7469 6f6e 206f 6620 7768  l duration of wh
+00007e20: 6174 2077 6520 6861 7665 206e 6f77 0a20  at we have now. 
+00007e30: 2020 2020 2020 2020 2020 2074 7374 6172             tstar
+00007e40: 7420 3d20 6461 7461 535f 745b 305d 0a0a  t = dataS_t[0]..
+00007e50: 2020 2020 2020 2020 2020 2020 6e73 7461              nsta
+00007e60: 636b 203d 2069 6e74 286e 702e 726f 756e  ck = int(np.roun
+00007e70: 6428 5474 6f74 616c 202f 2073 7562 7374  d(Ttotal / subst
+00007e80: 6163 6b5f 6c65 6e29 290a 2020 2020 2020  ack_len)).      
+00007e90: 2020 2020 2020 616d 706d 6178 203d 206e        ampmax = n
+00007ea0: 702e 7a65 726f 7328 6e73 7461 636b 2c20  p.zeros(nstack, 
+00007eb0: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+00007ec0: 290a 2020 2020 2020 2020 2020 2020 735f  ).            s_
+00007ed0: 636f 7272 203d 206e 702e 7a65 726f 7328  corr = np.zeros(
+00007ee0: 7368 6170 653d 286e 7374 6163 6b2c 204e  shape=(nstack, N
+00007ef0: 6666 7429 2c20 6474 7970 653d 6e70 2e66  fft), dtype=np.f
+00007f00: 6c6f 6174 3332 290a 2020 2020 2020 2020  loat32).        
+00007f10: 2020 2020 6e5f 636f 7272 203d 206e 702e      n_corr = np.
+00007f20: 7a65 726f 7328 6e73 7461 636b 2c20 6474  zeros(nstack, dt
+00007f30: 7970 653d 6e70 2e69 6e74 290a 2020 2020  ype=np.int).    
+00007f40: 2020 2020 2020 2020 745f 636f 7272 203d          t_corr =
+00007f50: 206e 702e 7a65 726f 7328 6e73 7461 636b   np.zeros(nstack
+00007f60: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00007f70: 290a 2020 2020 2020 2020 2020 2020 6372  ).            cr
+00007f80: 6170 203d 206e 702e 7a65 726f 7328 4e66  ap = np.zeros(Nf
+00007f90: 6674 2c20 6474 7970 653d 6e70 2e63 6f6d  ft, dtype=np.com
+00007fa0: 706c 6578 3634 290a 0a20 2020 2020 2020  plex64)..       
+00007fb0: 2020 2020 2066 6f72 2069 7374 6163 6b20       for istack 
+00007fc0: 696e 2072 616e 6765 286e 7374 6163 6b29  in range(nstack)
+00007fd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007fe0: 2020 2320 6669 6e64 2074 6865 2069 6e64    # find the ind
+00007ff0: 6578 6573 206f 6620 616c 6c20 6f66 2074  exes of all of t
+00008000: 6865 2077 696e 646f 7773 2074 6861 7420  he windows that 
+00008010: 7374 6172 7420 6f72 2065 6e64 2077 6974  start or end wit
+00008020: 6869 6e0a 2020 2020 2020 2020 2020 2020  hin.            
+00008030: 2020 2020 6974 696d 6520 3d20 6e70 2e77      itime = np.w
+00008040: 6865 7265 2828 6461 7461 535f 7420 3e3d  here((dataS_t >=
+00008050: 2074 7374 6172 7429 2026 2028 6461 7461   tstart) & (data
+00008060: 535f 7420 3c20 7473 7461 7274 202b 2073  S_t < tstart + s
+00008070: 7562 7374 6163 6b5f 6c65 6e29 295b 305d  ubstack_len))[0]
+00008080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008090: 2069 6620 6c65 6e28 6974 696d 6529 203d   if len(itime) =
+000080a0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+000080b0: 2020 2020 2020 2020 2074 7374 6172 7420           tstart 
+000080c0: 2b3d 2073 7562 7374 6163 6b5f 6c65 6e0a  += substack_len.
+000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080e0: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
+000080f0: 2020 2020 2020 2020 2020 2020 2020 6372                cr
+00008100: 6170 5b3a 4e66 6674 325d 203d 206e 702e  ap[:Nfft2] = np.
+00008110: 6d65 616e 2863 6f72 725b 6974 696d 652c  mean(corr[itime,
+00008120: 203a 5d2c 2061 7869 733d 3029 2020 2320   :], axis=0)  # 
+00008130: 6c69 6e65 6172 2061 7665 7261 6765 206f  linear average o
+00008140: 6620 7468 6520 636f 7272 656c 6174 696f  f the correlatio
+00008150: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+00008160: 2020 6372 6170 5b3a 4e66 6674 325d 203d    crap[:Nfft2] =
+00008170: 2063 7261 705b 3a4e 6666 7432 5d20 2d20   crap[:Nfft2] - 
+00008180: 6e70 2e6d 6561 6e28 6372 6170 5b3a 4e66  np.mean(crap[:Nf
+00008190: 6674 325d 2920 2023 2072 656d 6f76 6520  ft2])  # remove 
+000081a0: 7468 6520 6d65 616e 2069 6e20 6672 6571  the mean in freq
+000081b0: 2064 6f6d 6169 6e20 2873 7069 6b65 2061   domain (spike a
+000081c0: 7420 743d 3029 0a20 2020 2020 2020 2020  t t=0).         
+000081d0: 2020 2020 2020 2063 7261 705b 2d28 4e66         crap[-(Nf
+000081e0: 6674 3229 202b 2031 203a 5d20 3d20 6e70  ft2) + 1 :] = np
+000081f0: 2e66 6c69 7028 6e70 2e63 6f6e 6a28 6372  .flip(np.conj(cr
+00008200: 6170 5b31 3a28 4e66 6674 3229 5d29 2c20  ap[1:(Nfft2)]), 
+00008210: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
+00008220: 2020 2020 2020 2020 6372 6170 5b30 5d20          crap[0] 
+00008230: 3d20 636f 6d70 6c65 7828 302c 2030 290a  = complex(0, 0).
+00008240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008250: 735f 636f 7272 5b69 7374 6163 6b2c 203a  s_corr[istack, :
+00008260: 5d20 3d20 6e70 2e72 6561 6c28 6e70 2e66  ] = np.real(np.f
+00008270: 6674 2e69 6666 7473 6869 6674 2873 6369  ft.ifftshift(sci
+00008280: 7079 2e66 6674 7061 636b 2e69 6666 7428  py.fftpack.ifft(
+00008290: 6372 6170 2c20 4e66 6674 2c20 6178 6973  crap, Nfft, axis
+000082a0: 3d30 2929 290a 2020 2020 2020 2020 2020  =0))).          
+000082b0: 2020 2020 2020 6e5f 636f 7272 5b69 7374        n_corr[ist
+000082c0: 6163 6b5d 203d 206c 656e 2869 7469 6d65  ack] = len(itime
+000082d0: 2920 2023 206e 756d 6265 7220 6f66 2077  )  # number of w
+000082e0: 696e 646f 7773 2073 7461 636b 730a 2020  indows stacks.  
+000082f0: 2020 2020 2020 2020 2020 2020 2020 745f                t_
+00008300: 636f 7272 5b69 7374 6163 6b5d 203d 2074  corr[istack] = t
+00008310: 7374 6172 7420 2023 2073 6176 6520 7468  start  # save th
+00008320: 6520 7469 6d65 2073 7461 6d70 730a 2020  e time stamps.  
+00008330: 2020 2020 2020 2020 2020 2020 2020 7473                ts
+00008340: 7461 7274 202b 3d20 7375 6273 7461 636b  tart += substack
+00008350: 5f6c 656e 0a20 2020 2020 2020 2020 2020  _len.           
+00008360: 2020 2020 2023 2070 7269 6e74 2827 636f       # print('co
+00008370: 7272 656c 6174 696f 6e20 646f 6e65 2061  rrelation done a
+00008380: 6e64 2073 7461 636b 6564 2061 7420 7469  nd stacked at ti
+00008390: 6d65 2025 7327 2025 2073 7472 2874 5f63  me %s' % str(t_c
+000083a0: 6f72 725b 6973 7461 636b 5d29 290a 0a20  orr[istack])).. 
+000083b0: 2020 2020 2020 2020 2020 2023 2072 656d             # rem
+000083c0: 6f76 6520 6162 6e6f 726d 616c 2064 6174  ove abnormal dat
+000083d0: 610a 2020 2020 2020 2020 2020 2020 616d  a.            am
+000083e0: 706d 6178 203d 206e 702e 6d61 7828 735f  pmax = np.max(s_
+000083f0: 636f 7272 2c20 6178 6973 3d31 290a 2020  corr, axis=1).  
+00008400: 2020 2020 2020 2020 2020 7469 6e64 7820            tindx 
+00008410: 3d20 6e70 2e77 6865 7265 2828 616d 706d  = np.where((ampm
+00008420: 6178 203c 2032 3020 2a20 6e70 2e6d 6564  ax < 20 * np.med
+00008430: 6961 6e28 616d 706d 6178 2929 2026 2028  ian(ampmax)) & (
+00008440: 616d 706d 6178 203e 2030 2929 5b30 5d0a  ampmax > 0))[0].
+00008450: 2020 2020 2020 2020 2020 2020 735f 636f              s_co
+00008460: 7272 203d 2073 5f63 6f72 725b 7469 6e64  rr = s_corr[tind
+00008470: 782c 203a 5d0a 2020 2020 2020 2020 2020  x, :].          
+00008480: 2020 745f 636f 7272 203d 2074 5f63 6f72    t_corr = t_cor
+00008490: 725b 7469 6e64 785d 0a20 2020 2020 2020  r[tindx].       
+000084a0: 2020 2020 206e 5f63 6f72 7220 3d20 6e5f       n_corr = n_
+000084b0: 636f 7272 5b74 696e 6478 5d0a 0a20 2020  corr[tindx]..   
+000084c0: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
+000084d0: 2061 7665 7261 6765 2064 6169 6c79 2063   average daily c
+000084e0: 726f 7373 2063 6f72 7265 6c61 7469 6f6e  ross correlation
+000084f0: 2066 756e 6374 696f 6e73 0a20 2020 2020   functions.     
+00008500: 2020 2069 6620 7374 6163 6b5f 6d65 7468     if stack_meth
+00008510: 6f64 203d 3d20 226c 696e 6561 7222 3a0a  od == "linear":.
+00008520: 2020 2020 2020 2020 2020 2020 616d 706d              ampm
+00008530: 6178 203d 206e 702e 6d61 7828 735f 636f  ax = np.max(s_co
+00008540: 7272 2c20 6178 6973 3d31 290a 2020 2020  rr, axis=1).    
+00008550: 2020 2020 2020 2020 7469 6e64 7820 3d20          tindx = 
+00008560: 6e70 2e77 6865 7265 2828 616d 706d 6178  np.where((ampmax
+00008570: 203c 2032 3020 2a20 6e70 2e6d 6564 6961   < 20 * np.media
+00008580: 6e28 616d 706d 6178 2929 2026 2028 616d  n(ampmax)) & (am
+00008590: 706d 6178 203e 2030 2929 5b30 5d0a 2020  pmax > 0))[0].  
+000085a0: 2020 2020 2020 2020 2020 735f 636f 7272            s_corr
+000085b0: 203d 206e 702e 6d65 616e 2873 5f63 6f72   = np.mean(s_cor
+000085c0: 725b 7469 6e64 785d 2c20 6178 6973 3d30  r[tindx], axis=0
+000085d0: 290a 2020 2020 2020 2020 2020 2020 745f  ).            t_
+000085e0: 636f 7272 203d 2064 6174 6153 5f74 5b30  corr = dataS_t[0
+000085f0: 5d0a 2020 2020 2020 2020 2020 2020 6e5f  ].            n_
+00008600: 636f 7272 203d 206c 656e 2874 696e 6478  corr = len(tindx
+00008610: 290a 2020 2020 2020 2020 656c 6966 2073  ).        elif s
+00008620: 7461 636b 5f6d 6574 686f 6420 3d3d 2022  tack_method == "
+00008630: 726f 6275 7374 223a 0a20 2020 2020 2020  robust":.       
+00008640: 2020 2020 2070 7269 6e74 2822 646f 2072       print("do r
+00008650: 6f62 7573 7420 7375 6273 7461 636b 696e  obust substackin
+00008660: 6722 290a 2020 2020 2020 2020 2020 2020  g").            
+00008670: 735f 636f 7272 203d 2072 6f62 7573 745f  s_corr = robust_
+00008680: 7374 6163 6b28 735f 636f 7272 2c20 302e  stack(s_corr, 0.
+00008690: 3030 3129 0a20 2020 2020 2020 2020 2020  001).           
+000086a0: 2074 5f63 6f72 7220 3d20 6461 7461 535f   t_corr = dataS_
+000086b0: 745b 305d 0a20 2020 2020 2020 2020 2020  t[0].           
+000086c0: 206e 5f63 6f72 7220 3d20 6e77 696e 0a20   n_corr = nwin. 
+000086d0: 2020 2023 2020 656c 6966 2073 7461 636b     #  elif stack
+000086e0: 5f6d 6574 686f 6420 3d3d 2027 7365 6c65  _method == 'sele
+000086f0: 6374 6976 6527 3a0a 2020 2020 2320 2020  ctive':.    #   
+00008700: 2020 2070 7269 6e74 2827 646f 2073 656c     print('do sel
+00008710: 6563 7469 7665 2073 7562 7374 6163 6b69  ective substacki
+00008720: 6e67 2729 0a20 2020 2023 2020 2020 2020  ng').    #      
+00008730: 735f 636f 7272 203d 2073 656c 6563 7469  s_corr = selecti
+00008740: 7665 5f73 7461 636b 2873 5f63 6f72 722c  ve_stack(s_corr,
+00008750: 302e 3030 3129 0a20 2020 2023 2020 2020  0.001).    #    
+00008760: 2020 745f 636f 7272 203d 2064 6174 6153    t_corr = dataS
+00008770: 5f74 5b30 5d0a 2020 2020 2320 2020 2020  _t[0].    #     
+00008780: 206e 5f63 6f72 7220 3d20 6e77 696e 0a0a   n_corr = nwin..
+00008790: 2020 2020 2320 7472 696d 2074 6865 2043      # trim the C
+000087a0: 4346 7320 696e 205b 2d6d 6178 6c61 6720  CFs in [-maxlag 
+000087b0: 6d61 786c 6167 5d0a 2020 2020 7420 3d20  maxlag].    t = 
+000087c0: 6e70 2e61 7261 6e67 6528 2d4e 6666 7432  np.arange(-Nfft2
+000087d0: 202b 2031 2c20 4e66 6674 3229 202a 2064   + 1, Nfft2) * d
+000087e0: 740a 2020 2020 696e 6420 3d20 6e70 2e77  t.    ind = np.w
+000087f0: 6865 7265 286e 702e 6162 7328 7429 203c  here(np.abs(t) <
+00008800: 3d20 6d61 786c 6167 295b 305d 0a20 2020  = maxlag)[0].   
+00008810: 2069 6620 735f 636f 7272 2e6e 6469 6d20   if s_corr.ndim 
+00008820: 3d3d 2031 3a0a 2020 2020 2020 2020 735f  == 1:.        s_
+00008830: 636f 7272 203d 2073 5f63 6f72 725b 696e  corr = s_corr[in
+00008840: 645d 0a20 2020 2065 6c69 6620 735f 636f  d].    elif s_co
+00008850: 7272 2e6e 6469 6d20 3d3d 2032 3a0a 2020  rr.ndim == 2:.  
+00008860: 2020 2020 2020 735f 636f 7272 203d 2073        s_corr = s
+00008870: 5f63 6f72 725b 3a2c 2069 6e64 5d0a 2020  _corr[:, ind].  
+00008880: 2020 7265 7475 726e 2073 5f63 6f72 722c    return s_corr,
+00008890: 2074 5f63 6f72 722c 206e 5f63 6f72 722c   t_corr, n_corr,
+000088a0: 206e 735f 636f 7272 5b3a 2c20 696e 645d   ns_corr[:, ind]
+000088b0: 0a0a 0a64 6566 2063 635f 7061 7261 6d65  ...def cc_parame
+000088c0: 7465 7273 2863 635f 7061 7261 2c20 636f  ters(cc_para, co
+000088d0: 6f72 2c20 7463 6f72 722c 206e 636f 7272  or, tcorr, ncorr
+000088e0: 2c20 636f 6d70 293a 0a20 2020 2022 2222  , comp):.    """
+000088f0: 0a20 2020 2074 6869 7320 6675 6e63 7469  .    this functi
+00008900: 6f6e 2061 7373 656d 626c 6573 2074 6865  on assembles the
+00008910: 2070 6172 616d 6574 6572 7320 666f 7220   parameters for 
+00008920: 7468 6520 6363 2066 756e 6374 696f 6e2c  the cc function,
+00008930: 2077 6869 6368 2069 7320 7573 6564 0a20   which is used. 
+00008940: 2020 2077 6865 6e20 7772 6974 696e 6720     when writing 
+00008950: 7468 656d 2069 6e74 6f20 4153 4446 2066  them into ASDF f
+00008960: 696c 6573 0a20 2020 2050 4152 414d 4554  iles.    PARAMET
+00008970: 4552 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ERS:.    -------
+00008980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00008990: 2020 2063 635f 7061 7261 3a20 6469 6374     cc_para: dict
+000089a0: 2063 6f6e 7461 696e 696e 6720 7061 7261   containing para
+000089b0: 6d65 7465 7273 2075 7365 6420 696e 2074  meters used in t
+000089c0: 6865 2066 6674 5f63 6320 7374 6570 0a20  he fft_cc step. 
+000089d0: 2020 2063 6f6f 723a 2020 2020 6469 6374     coor:    dict
+000089e0: 2063 6f6e 7461 696e 696e 6720 636f 6f72   containing coor
+000089f0: 6469 6e61 7465 7320 696e 666f 206f 6620  dinates info of 
+00008a00: 7468 6520 736f 7572 6365 2061 6e64 2072  the source and r
+00008a10: 6563 6569 7665 7220 7374 6174 696f 6e73  eceiver stations
+00008a20: 0a20 2020 2074 636f 7272 3a20 2020 7469  .    tcorr:   ti
+00008a30: 6d65 7374 616d 7020 6d61 7472 6978 0a20  mestamp matrix. 
+00008a40: 2020 206e 636f 7272 3a20 2020 6d61 7472     ncorr:   matr
+00008a50: 6978 206f 6620 6e75 6d62 6572 206f 6620  ix of number of 
+00008a60: 676f 6f64 2073 6567 6d65 6e74 7320 666f  good segments fo
+00008a70: 7220 6561 6368 2073 7562 2d73 7461 636b  r each sub-stack
+00008a80: 2f66 696e 616c 2073 7461 636b 0a20 2020  /final stack.   
+00008a90: 2063 6f6d 703a 2020 2020 3220 6368 6172   comp:    2 char
+00008aa0: 6163 7465 7220 7374 7269 6e67 7320 666f  acter strings fo
+00008ab0: 7220 7468 6520 6372 6f73 7320 636f 7272  r the cross corr
+00008ac0: 656c 6174 696f 6e20 636f 6d70 6f6e 656e  elation componen
+00008ad0: 740a 2020 2020 5245 5455 524e 533a 0a20  t.    RETURNS:. 
+00008ae0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00008af0: 2d2d 2d2d 2d0a 2020 2020 7061 7261 6d65  -----.    parame
+00008b00: 7465 7273 3a20 6469 6374 2063 6f6e 7461  ters: dict conta
+00008b10: 696e 696e 6720 6162 6f76 6520 696e 666f  ining above info
+00008b20: 2075 7365 6420 666f 7220 6c61 7465 7220   used for later 
+00008b30: 7374 6163 6b69 6e67 2f70 6c6f 7474 696e  stacking/plottin
+00008b40: 670a 2020 2020 2222 220a 2020 2020 6c61  g.    """.    la
+00008b50: 7453 203d 2063 6f6f 725b 226c 6174 5322  tS = coor["latS"
+00008b60: 5d0a 2020 2020 6c6f 6e53 203d 2063 6f6f  ].    lonS = coo
+00008b70: 725b 226c 6f6e 5322 5d0a 2020 2020 6c61  r["lonS"].    la
+00008b80: 7452 203d 2063 6f6f 725b 226c 6174 5222  tR = coor["latR"
+00008b90: 5d0a 2020 2020 6c6f 6e52 203d 2063 6f6f  ].    lonR = coo
+00008ba0: 725b 226c 6f6e 5222 5d0a 2020 2020 6474  r["lonR"].    dt
+00008bb0: 203d 2063 635f 7061 7261 5b22 6474 225d   = cc_para["dt"]
+00008bc0: 0a20 2020 206d 6178 6c61 6720 3d20 6363  .    maxlag = cc
+00008bd0: 5f70 6172 615b 226d 6178 6c61 6722 5d0a  _para["maxlag"].
+00008be0: 2020 2020 7375 6273 7461 636b 203d 2063      substack = c
+00008bf0: 635f 7061 7261 5b22 7375 6273 7461 636b  c_para["substack
+00008c00: 225d 0a20 2020 2063 635f 6d65 7468 6f64  "].    cc_method
+00008c10: 203d 2063 635f 7061 7261 5b22 6363 5f6d   = cc_para["cc_m
+00008c20: 6574 686f 6422 5d0a 0a20 2020 2064 6973  ethod"]..    dis
+00008c30: 742c 2061 7a69 2c20 6261 7a20 3d20 6f62  t, azi, baz = ob
+00008c40: 7370 792e 6765 6f64 6574 6963 732e 6261  spy.geodetics.ba
+00008c50: 7365 2e67 7073 3264 6973 745f 617a 696d  se.gps2dist_azim
+00008c60: 7574 6828 6c61 7453 2c20 6c6f 6e53 2c20  uth(latS, lonS, 
+00008c70: 6c61 7452 2c20 6c6f 6e52 290a 2020 2020  latR, lonR).    
+00008c80: 7061 7261 6d65 7465 7273 203d 207b 0a20  parameters = {. 
+00008c90: 2020 2020 2020 2022 6474 223a 2064 742c         "dt": dt,
+00008ca0: 0a20 2020 2020 2020 2022 6d61 786c 6167  .        "maxlag
+00008cb0: 223a 2069 6e74 286d 6178 6c61 6729 2c0a  ": int(maxlag),.
+00008cc0: 2020 2020 2020 2020 2264 6973 7422 3a20          "dist": 
+00008cd0: 6e70 2e66 6c6f 6174 3332 2864 6973 7420  np.float32(dist 
+00008ce0: 2f20 3130 3030 292c 0a20 2020 2020 2020  / 1000),.       
+00008cf0: 2022 617a 6922 3a20 6e70 2e66 6c6f 6174   "azi": np.float
+00008d00: 3332 2861 7a69 292c 0a20 2020 2020 2020  32(azi),.       
+00008d10: 2022 6261 7a22 3a20 6e70 2e66 6c6f 6174   "baz": np.float
+00008d20: 3332 2862 617a 292c 0a20 2020 2020 2020  32(baz),.       
+00008d30: 2022 6c6f 6e53 223a 206e 702e 666c 6f61   "lonS": np.floa
+00008d40: 7433 3228 6c6f 6e53 292c 0a20 2020 2020  t32(lonS),.     
+00008d50: 2020 2022 6c61 7453 223a 206e 702e 666c     "latS": np.fl
+00008d60: 6f61 7433 3228 6c61 7453 292c 0a20 2020  oat32(latS),.   
+00008d70: 2020 2020 2022 6c6f 6e52 223a 206e 702e       "lonR": np.
+00008d80: 666c 6f61 7433 3228 6c6f 6e52 292c 0a20  float32(lonR),. 
+00008d90: 2020 2020 2020 2022 6c61 7452 223a 206e         "latR": n
+00008da0: 702e 666c 6f61 7433 3228 6c61 7452 292c  p.float32(latR),
+00008db0: 0a20 2020 2020 2020 2022 6e67 6f6f 6422  .        "ngood"
+00008dc0: 3a20 6e63 6f72 722c 0a20 2020 2020 2020  : ncorr,.       
+00008dd0: 2022 6363 5f6d 6574 686f 6422 3a20 6363   "cc_method": cc
+00008de0: 5f6d 6574 686f 642c 0a20 2020 2020 2020  _method,.       
+00008df0: 2022 7469 6d65 223a 2074 636f 7272 2c0a   "time": tcorr,.
+00008e00: 2020 2020 2020 2020 2273 7562 7374 6163          "substac
+00008e10: 6b22 3a20 7375 6273 7461 636b 2c0a 2020  k": substack,.  
+00008e20: 2020 2020 2020 2263 6f6d 7022 3a20 636f        "comp": co
+00008e30: 6d70 2c0a 2020 2020 7d0a 2020 2020 7265  mp,.    }.    re
+00008e40: 7475 726e 2070 6172 616d 6574 6572 730a  turn parameters.
+00008e50: 0a0a 6465 6620 7374 6163 6b69 6e67 2863  ..def stacking(c
+00008e60: 635f 6172 7261 792c 2063 635f 7469 6d65  c_array, cc_time
+00008e70: 2c20 6363 5f6e 676f 6f64 2c20 7374 6163  , cc_ngood, stac
+00008e80: 6b5f 7061 7261 293a 0a20 2020 2022 2222  k_para):.    """
+00008e90: 0a20 2020 2074 6869 7320 6675 6e63 7469  .    this functi
+00008ea0: 6f6e 2073 7461 636b 7320 7468 6520 6372  on stacks the cr
+00008eb0: 6f73 7320 636f 7272 656c 6174 696f 6e20  oss correlation 
+00008ec0: 6461 7461 2061 6363 6f72 6469 6e67 2074  data according t
+00008ed0: 6f20 7468 6520 7573 6572 2d64 6566 696e  o the user-defin
+00008ee0: 6564 2073 7562 7374 6163 6b5f 6c65 6e20  ed substack_len 
+00008ef0: 7061 7261 6d65 7465 720a 0a20 2020 2050  parameter..    P
+00008f00: 4152 414d 4554 4552 533a 0a20 2020 202d  ARAMETERS:.    -
+00008f10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008f20: 2d2d 2d2d 2d0a 2020 2020 6363 5f61 7272  -----.    cc_arr
+00008f30: 6179 3a20 3244 206e 756d 7079 2066 6c6f  ay: 2D numpy flo
+00008f40: 6174 3332 206d 6174 7269 7820 636f 6e74  at32 matrix cont
+00008f50: 6169 6e69 6e67 2061 6c6c 2073 6567 6d65  aining all segme
+00008f60: 6e74 6564 2063 726f 7373 2d63 6f72 7265  nted cross-corre
+00008f70: 6c61 7469 6f6e 2064 6174 610a 2020 2020  lation data.    
+00008f80: 6363 5f74 696d 653a 2020 3144 206e 756d  cc_time:  1D num
+00008f90: 7079 2061 7272 6179 206f 6620 7469 6d65  py array of time
+00008fa0: 7374 616d 7073 2066 6f72 2065 6163 6820  stamps for each 
+00008fb0: 7365 676d 656e 7420 6f66 2063 635f 6172  segment of cc_ar
+00008fc0: 7261 790a 2020 2020 6363 5f6e 676f 6f64  ray.    cc_ngood
+00008fd0: 3a20 3144 206e 756d 7079 2069 6e74 3136  : 1D numpy int16
+00008fe0: 206d 6174 7269 7820 7368 6f77 696e 6720   matrix showing 
+00008ff0: 7468 6520 6e75 6d62 6572 206f 6620 7365  the number of se
+00009000: 676d 656e 7473 2066 6f72 2065 6163 6820  gments for each 
+00009010: 7375 622d 7374 6163 6b20 616e 642f 6f72  sub-stack and/or
+00009020: 2066 756c 6c20 7374 6163 6b0a 2020 2020   full stack.    
+00009030: 7374 6163 6b5f 7061 7261 3a20 6120 6469  stack_para: a di
+00009040: 6374 2063 6f6e 7461 696e 696e 6720 616c  ct containing al
+00009050: 6c20 7374 6163 6b69 6e67 2070 6172 616d  l stacking param
+00009060: 6574 6572 730a 0a20 2020 2052 4554 5552  eters..    RETUR
+00009070: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
+00009080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00009090: 2020 2063 635f 6172 7261 792c 2063 635f     cc_array, cc_
+000090a0: 6e67 6f6f 642c 2063 635f 7469 6d65 3a20  ngood, cc_time: 
+000090b0: 7361 6d65 2074 6f20 7468 6520 696e 7075  same to the inpu
+000090c0: 7420 7061 7261 6d65 7465 7273 2062 7574  t parameters but
+000090d0: 2077 6974 6820 6162 6e6f 726d 616c 2063   with abnormal c
+000090e0: 726f 7373 2d63 6f72 7265 616c 7469 6f6e  ross-correaltion
+000090f0: 7320 7265 6d6f 7665 640a 2020 2020 616c  s removed.    al
+00009100: 6c73 7461 636b 7331 3a20 3144 206d 6174  lstacks1: 1D mat
+00009110: 7269 7820 6f66 2073 7461 636b 6564 2063  rix of stacked c
+00009120: 726f 7373 2d63 6f72 7265 6c61 7469 6f6e  ross-correlation
+00009130: 2066 756e 6374 696f 6e73 206f 7665 7220   functions over 
+00009140: 616c 6c20 7468 6520 7365 676d 656e 7473  all the segments
+00009150: 0a20 2020 206e 7374 6163 6b73 3a20 2020  .    nstacks:   
+00009160: 206e 756d 6265 7220 6f66 206f 7665 7261   number of overa
+00009170: 6c6c 2073 6567 6d65 6e74 7320 666f 7220  ll segments for 
+00009180: 7468 6520 6669 6e61 6c20 7374 6163 6b73  the final stacks
+00009190: 0a20 2020 2022 2222 0a20 2020 2023 206c  .    """.    # l
+000091a0: 6f61 6420 7573 6566 756c 2070 6172 616d  oad useful param
+000091b0: 6574 6572 7320 6672 6f6d 2064 6963 740a  eters from dict.
+000091c0: 2020 2020 7361 6d70 5f66 7265 7120 3d20      samp_freq = 
+000091d0: 7374 6163 6b5f 7061 7261 5b22 7361 6d70  stack_para["samp
+000091e0: 5f66 7265 7122 5d0a 2020 2020 736d 6574  _freq"].    smet
+000091f0: 686f 6420 3d20 7374 6163 6b5f 7061 7261  hod = stack_para
+00009200: 5b22 7374 6163 6b5f 6d65 7468 6f64 225d  ["stack_method"]
+00009210: 0a20 2020 206e 7074 7320 3d20 6363 5f61  .    npts = cc_a
+00009220: 7272 6179 2e73 6861 7065 5b31 5d0a 0a20  rray.shape[1].. 
+00009230: 2020 2023 2072 656d 6f76 6520 6162 6e6f     # remove abno
+00009240: 726d 616c 2064 6174 610a 2020 2020 616d  rmal data.    am
+00009250: 706d 6178 203d 206e 702e 6d61 7828 6363  pmax = np.max(cc
+00009260: 5f61 7272 6179 2c20 6178 6973 3d31 290a  _array, axis=1).
+00009270: 2020 2020 7469 6e64 7820 3d20 6e70 2e77      tindx = np.w
+00009280: 6865 7265 2828 616d 706d 6178 203c 2032  here((ampmax < 2
+00009290: 3020 2a20 6e70 2e6d 6564 6961 6e28 616d  0 * np.median(am
+000092a0: 706d 6178 2929 2026 2028 616d 706d 6178  pmax)) & (ampmax
+000092b0: 203e 2030 2929 5b30 5d0a 2020 2020 6966   > 0))[0].    if
+000092c0: 206e 6f74 206c 656e 2874 696e 6478 293a   not len(tindx):
+000092d0: 0a20 2020 2020 2020 2061 6c6c 7374 6163  .        allstac
+000092e0: 6b73 3120 3d20 5b5d 0a20 2020 2020 2020  ks1 = [].       
+000092f0: 2061 6c6c 7374 6163 6b73 3220 3d20 5b5d   allstacks2 = []
+00009300: 0a20 2020 2020 2020 2061 6c6c 7374 6163  .        allstac
+00009310: 6b73 3320 3d20 5b5d 0a20 2020 2020 2020  ks3 = [].       
+00009320: 206e 7374 6163 6b73 203d 2030 0a20 2020   nstacks = 0.   
+00009330: 2020 2020 2063 635f 6172 7261 7920 3d20       cc_array = 
+00009340: 5b5d 0a20 2020 2020 2020 2063 635f 6e67  [].        cc_ng
+00009350: 6f6f 6420 3d20 5b5d 0a20 2020 2020 2020  ood = [].       
+00009360: 2063 635f 7469 6d65 203d 205b 5d0a 2020   cc_time = [].  
+00009370: 2020 2020 2020 7265 7475 726e 2063 635f        return cc_
+00009380: 6172 7261 792c 2063 635f 6e67 6f6f 642c  array, cc_ngood,
+00009390: 2063 635f 7469 6d65 2c20 616c 6c73 7461   cc_time, allsta
+000093a0: 636b 7331 2c20 616c 6c73 7461 636b 7332  cks1, allstacks2
+000093b0: 2c20 616c 6c73 7461 636b 7333 2c20 6e73  , allstacks3, ns
+000093c0: 7461 636b 730a 2020 2020 656c 7365 3a0a  tacks.    else:.
+000093d0: 2020 2020 2020 2020 2320 7265 6d6f 7665          # remove
+000093e0: 206f 6e65 7320 7769 7468 2062 6164 2061   ones with bad a
+000093f0: 6d70 6c69 7475 6465 0a20 2020 2020 2020  mplitude.       
+00009400: 2063 635f 6172 7261 7920 3d20 6363 5f61   cc_array = cc_a
+00009410: 7272 6179 5b74 696e 6478 2c20 3a5d 0a20  rray[tindx, :]. 
+00009420: 2020 2020 2020 2063 635f 7469 6d65 203d         cc_time =
+00009430: 2063 635f 7469 6d65 5b74 696e 6478 5d0a   cc_time[tindx].
+00009440: 2020 2020 2020 2020 6363 5f6e 676f 6f64          cc_ngood
+00009450: 203d 2063 635f 6e67 6f6f 645b 7469 6e64   = cc_ngood[tind
+00009460: 785d 0a0a 2020 2020 2020 2020 2320 646f  x]..        # do
+00009470: 2073 7461 636b 696e 670a 2020 2020 2020   stacking.      
+00009480: 2020 616c 6c73 7461 636b 7331 203d 206e    allstacks1 = n
+00009490: 702e 7a65 726f 7328 6e70 7473 2c20 6474  p.zeros(npts, dt
+000094a0: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
+000094b0: 2020 2020 2020 2020 616c 6c73 7461 636b          allstack
+000094c0: 7332 203d 206e 702e 7a65 726f 7328 6e70  s2 = np.zeros(np
+000094d0: 7473 2c20 6474 7970 653d 6e70 2e66 6c6f  ts, dtype=np.flo
+000094e0: 6174 3332 290a 2020 2020 2020 2020 616c  at32).        al
+000094f0: 6c73 7461 636b 7333 203d 206e 702e 7a65  lstacks3 = np.ze
+00009500: 726f 7328 6e70 7473 2c20 6474 7970 653d  ros(npts, dtype=
+00009510: 6e70 2e66 6c6f 6174 3332 290a 0a20 2020  np.float32)..   
+00009520: 2020 2020 2069 6620 736d 6574 686f 6420       if smethod 
+00009530: 3d3d 2022 6c69 6e65 6172 223a 0a20 2020  == "linear":.   
+00009540: 2020 2020 2020 2020 2061 6c6c 7374 6163           allstac
+00009550: 6b73 3120 3d20 6e70 2e6d 6561 6e28 6363  ks1 = np.mean(cc
+00009560: 5f61 7272 6179 2c20 6178 6973 3d30 290a  _array, axis=0).
+00009570: 2020 2020 2020 2020 656c 6966 2073 6d65          elif sme
+00009580: 7468 6f64 203d 3d20 2270 7773 223a 0a20  thod == "pws":. 
+00009590: 2020 2020 2020 2020 2020 2061 6c6c 7374             allst
+000095a0: 6163 6b73 3120 3d20 7077 7328 6363 5f61  acks1 = pws(cc_a
+000095b0: 7272 6179 2c20 7361 6d70 5f66 7265 7129  rray, samp_freq)
+000095c0: 0a20 2020 2020 2020 2065 6c69 6620 736d  .        elif sm
+000095d0: 6574 686f 6420 3d3d 2022 726f 6275 7374  ethod == "robust
+000095e0: 223a 0a20 2020 2020 2020 2020 2020 2061  ":.            a
+000095f0: 6c6c 7374 6163 6b73 312c 2077 2c20 6e73  llstacks1, w, ns
+00009600: 7465 7020 3d20 726f 6275 7374 5f73 7461  tep = robust_sta
+00009610: 636b 2863 635f 6172 7261 792c 2030 2e30  ck(cc_array, 0.0
+00009620: 3031 290a 2020 2020 2020 2020 656c 6966  01).        elif
+00009630: 2073 6d65 7468 6f64 203d 3d20 2261 7574   smethod == "aut
+00009640: 6f5f 636f 7661 7269 616e 6365 223a 0a20  o_covariance":. 
+00009650: 2020 2020 2020 2020 2020 2061 6c6c 7374             allst
+00009660: 6163 6b73 3120 3d20 6164 6170 7469 7665  acks1 = adaptive
+00009670: 5f66 696c 7465 7228 6363 5f61 7272 6179  _filter(cc_array
+00009680: 2c20 3129 0a20 2020 2020 2020 2065 6c69  , 1).        eli
+00009690: 6620 736d 6574 686f 6420 3d3d 2022 6e72  f smethod == "nr
+000096a0: 6f6f 7422 3a0a 2020 2020 2020 2020 2020  oot":.          
+000096b0: 2020 616c 6c73 7461 636b 7331 203d 206e    allstacks1 = n
+000096c0: 726f 6f74 5f73 7461 636b 2863 635f 6172  root_stack(cc_ar
+000096d0: 7261 792c 2032 290a 2020 2020 2020 2020  ray, 2).        
+000096e0: 656c 6966 2073 6d65 7468 6f64 203d 3d20  elif smethod == 
+000096f0: 2261 6c6c 223a 0a20 2020 2020 2020 2020  "all":.         
+00009700: 2020 2061 6c6c 7374 6163 6b73 3120 3d20     allstacks1 = 
+00009710: 6e70 2e6d 6561 6e28 6363 5f61 7272 6179  np.mean(cc_array
+00009720: 2c20 6178 6973 3d30 290a 2020 2020 2020  , axis=0).      
+00009730: 2020 2020 2020 616c 6c73 7461 636b 7332        allstacks2
+00009740: 203d 2070 7773 2863 635f 6172 7261 792c   = pws(cc_array,
+00009750: 2073 616d 705f 6672 6571 290a 2020 2020   samp_freq).    
+00009760: 2020 2020 2020 2020 616c 6c73 7461 636b          allstack
+00009770: 7333 2c20 772c 206e 7374 6570 203d 2072  s3, w, nstep = r
+00009780: 6f62 7573 745f 7374 6163 6b28 6363 5f61  obust_stack(cc_a
+00009790: 7272 6179 2c20 302e 3030 3129 0a20 2020  rray, 0.001).   
+000097a0: 2020 2020 206e 7374 6163 6b73 203d 206e       nstacks = n
+000097b0: 702e 7375 6d28 6363 5f6e 676f 6f64 290a  p.sum(cc_ngood).
+000097c0: 0a20 2020 2023 2067 6f6f 6420 746f 2072  .    # good to r
+000097d0: 6574 7572 6e0a 2020 2020 7265 7475 726e  eturn.    return
+000097e0: 2063 635f 6172 7261 792c 2063 635f 6e67   cc_array, cc_ng
+000097f0: 6f6f 642c 2063 635f 7469 6d65 2c20 616c  ood, cc_time, al
+00009800: 6c73 7461 636b 7331 2c20 616c 6c73 7461  lstacks1, allsta
+00009810: 636b 7332 2c20 616c 6c73 7461 636b 7333  cks2, allstacks3
+00009820: 2c20 6e73 7461 636b 730a 0a0a 6465 6620  , nstacks...def 
+00009830: 7374 6163 6b69 6e67 5f72 6d61 2863 635f  stacking_rma(cc_
+00009840: 6172 7261 792c 2063 635f 7469 6d65 2c20  array, cc_time, 
+00009850: 6363 5f6e 676f 6f64 2c20 7374 6163 6b5f  cc_ngood, stack_
+00009860: 7061 7261 293a 0a20 2020 2022 2222 0a20  para):.    """. 
+00009870: 2020 2074 6869 7320 6675 6e63 7469 6f6e     this function
+00009880: 2073 7461 636b 7320 7468 6520 6372 6f73   stacks the cros
+00009890: 7320 636f 7272 656c 6174 696f 6e20 6461  s correlation da
+000098a0: 7461 2061 6363 6f72 6469 6e67 2074 6f20  ta according to 
+000098b0: 7468 6520 7573 6572 2d64 6566 696e 6564  the user-defined
+000098c0: 2073 7562 7374 6163 6b5f 6c65 6e20 7061   substack_len pa
+000098d0: 7261 6d65 7465 720a 2020 2020 5041 5241  rameter.    PARA
+000098e0: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
+000098f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00009900: 2d2d 0a20 2020 2063 635f 6172 7261 793a  --.    cc_array:
+00009910: 2032 4420 6e75 6d70 7920 666c 6f61 7433   2D numpy float3
+00009920: 3220 6d61 7472 6978 2063 6f6e 7461 696e  2 matrix contain
+00009930: 696e 6720 616c 6c20 7365 676d 656e 7465  ing all segmente
+00009940: 6420 6372 6f73 732d 636f 7272 656c 6174  d cross-correlat
+00009950: 696f 6e20 6461 7461 0a20 2020 2063 635f  ion data.    cc_
+00009960: 7469 6d65 3a20 2031 4420 6e75 6d70 7920  time:  1D numpy 
+00009970: 6172 7261 7920 6f66 2074 696d 6573 7461  array of timesta
+00009980: 6d70 7320 666f 7220 6561 6368 2073 6567  mps for each seg
+00009990: 6d65 6e74 206f 6620 6363 5f61 7272 6179  ment of cc_array
+000099a0: 0a20 2020 2063 635f 6e67 6f6f 643a 2031  .    cc_ngood: 1
+000099b0: 4420 6e75 6d70 7920 696e 7431 3620 6d61  D numpy int16 ma
+000099c0: 7472 6978 2073 686f 7769 6e67 2074 6865  trix showing the
+000099d0: 206e 756d 6265 7220 6f66 2073 6567 6d65   number of segme
+000099e0: 6e74 7320 666f 7220 6561 6368 2073 7562  nts for each sub
+000099f0: 2d73 7461 636b 2061 6e64 2f6f 7220 6675  -stack and/or fu
+00009a00: 6c6c 2073 7461 636b 0a20 2020 2073 7461  ll stack.    sta
+00009a10: 636b 5f70 6172 613a 2061 2064 6963 7420  ck_para: a dict 
+00009a20: 636f 6e74 6169 6e69 6e67 2061 6c6c 2073  containing all s
+00009a30: 7461 636b 696e 6720 7061 7261 6d65 7465  tacking paramete
+00009a40: 7273 0a20 2020 2052 4554 5552 4e53 3a0a  rs.    RETURNS:.
+00009a50: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+00009a60: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063  ----------.    c
+00009a70: 635f 6172 7261 792c 2063 635f 6e67 6f6f  c_array, cc_ngoo
+00009a80: 642c 2063 635f 7469 6d65 3a20 7361 6d65  d, cc_time: same
+00009a90: 2074 6f20 7468 6520 696e 7075 7420 7061   to the input pa
+00009aa0: 7261 6d65 7465 7273 2062 7574 2077 6974  rameters but wit
+00009ab0: 6820 6162 6e6f 726d 616c 2063 726f 7373  h abnormal cross
+00009ac0: 2d63 6f72 7265 616c 7469 6f6e 7320 7265  -correaltions re
+00009ad0: 6d6f 7665 640a 2020 2020 616c 6c73 7461  moved.    allsta
+00009ae0: 636b 7331 3a20 3144 206d 6174 7269 7820  cks1: 1D matrix 
+00009af0: 6f66 2073 7461 636b 6564 2063 726f 7373  of stacked cross
+00009b00: 2d63 6f72 7265 6c61 7469 6f6e 2066 756e  -correlation fun
+00009b10: 6374 696f 6e73 206f 7665 7220 616c 6c20  ctions over all 
+00009b20: 7468 6520 7365 676d 656e 7473 0a20 2020  the segments.   
+00009b30: 206e 7374 6163 6b73 3a20 2020 206e 756d   nstacks:    num
+00009b40: 6265 7220 6f66 206f 7665 7261 6c6c 2073  ber of overall s
+00009b50: 6567 6d65 6e74 7320 666f 7220 7468 6520  egments for the 
+00009b60: 6669 6e61 6c20 7374 6163 6b73 0a20 2020  final stacks.   
+00009b70: 2022 2222 0a20 2020 2023 206c 6f61 6420   """.    # load 
+00009b80: 7573 6566 756c 2070 6172 616d 6574 6572  useful parameter
+00009b90: 7320 6672 6f6d 2064 6963 740a 2020 2020  s from dict.    
+00009ba0: 7361 6d70 5f66 7265 7120 3d20 7374 6163  samp_freq = stac
+00009bb0: 6b5f 7061 7261 5b22 7361 6d70 5f66 7265  k_para["samp_fre
+00009bc0: 7122 5d0a 2020 2020 736d 6574 686f 6420  q"].    smethod 
+00009bd0: 3d20 7374 6163 6b5f 7061 7261 5b22 7374  = stack_para["st
+00009be0: 6163 6b5f 6d65 7468 6f64 225d 0a20 2020  ack_method"].   
+00009bf0: 2072 6d61 5f73 7562 7374 6163 6b20 3d20   rma_substack = 
+00009c00: 7374 6163 6b5f 7061 7261 5b22 726d 615f  stack_para["rma_
+00009c10: 7375 6273 7461 636b 225d 0a20 2020 2072  substack"].    r
+00009c20: 6d61 5f73 7465 7020 3d20 7374 6163 6b5f  ma_step = stack_
+00009c30: 7061 7261 5b22 726d 615f 7374 6570 225d  para["rma_step"]
+00009c40: 0a20 2020 2073 7461 7274 5f64 6174 6520  .    start_date 
+00009c50: 3d20 7374 6163 6b5f 7061 7261 5b22 7374  = stack_para["st
+00009c60: 6172 745f 6461 7465 225d 0a20 2020 2065  art_date"].    e
+00009c70: 6e64 5f64 6174 6520 3d20 7374 6163 6b5f  nd_date = stack_
+00009c80: 7061 7261 5b22 656e 645f 6461 7465 225d  para["end_date"]
+00009c90: 0a20 2020 206e 7074 7320 3d20 6363 5f61  .    npts = cc_a
+00009ca0: 7272 6179 2e73 6861 7065 5b31 5d0a 0a20  rray.shape[1].. 
+00009cb0: 2020 2023 2072 656d 6f76 6520 6162 6e6f     # remove abno
+00009cc0: 726d 616c 2064 6174 610a 2020 2020 616d  rmal data.    am
+00009cd0: 706d 6178 203d 206e 702e 6d61 7828 6363  pmax = np.max(cc
+00009ce0: 5f61 7272 6179 2c20 6178 6973 3d31 290a  _array, axis=1).
+00009cf0: 2020 2020 7469 6e64 7820 3d20 6e70 2e77      tindx = np.w
+00009d00: 6865 7265 2828 616d 706d 6178 203c 2032  here((ampmax < 2
+00009d10: 3020 2a20 6e70 2e6d 6564 6961 6e28 616d  0 * np.median(am
+00009d20: 706d 6178 2929 2026 2028 616d 706d 6178  pmax)) & (ampmax
+00009d30: 203e 2030 2929 5b30 5d0a 2020 2020 6966   > 0))[0].    if
+00009d40: 206e 6f74 206c 656e 2874 696e 6478 293a   not len(tindx):
+00009d50: 0a20 2020 2020 2020 2061 6c6c 7374 6163  .        allstac
+00009d60: 6b73 3120 3d20 5b5d 0a20 2020 2020 2020  ks1 = [].       
+00009d70: 2061 6c6c 7374 6163 6b73 3220 3d20 5b5d   allstacks2 = []
+00009d80: 0a20 2020 2020 2020 206e 7374 6163 6b73  .        nstacks
+00009d90: 203d 2030 0a20 2020 2020 2020 2063 635f   = 0.        cc_
+00009da0: 6172 7261 7920 3d20 5b5d 0a20 2020 2020  array = [].     
+00009db0: 2020 2063 635f 6e67 6f6f 6420 3d20 5b5d     cc_ngood = []
+00009dc0: 0a20 2020 2020 2020 2063 635f 7469 6d65  .        cc_time
+00009dd0: 203d 205b 5d0a 2020 2020 2020 2020 7265   = [].        re
+00009de0: 7475 726e 2063 635f 6172 7261 792c 2063  turn cc_array, c
+00009df0: 635f 6e67 6f6f 642c 2063 635f 7469 6d65  c_ngood, cc_time
+00009e00: 2c20 616c 6c73 7461 636b 7331 2c20 616c  , allstacks1, al
+00009e10: 6c73 7461 636b 7332 2c20 6e73 7461 636b  lstacks2, nstack
+00009e20: 730a 2020 2020 656c 7365 3a0a 2020 2020  s.    else:.    
+00009e30: 2020 2020 2320 7265 6d6f 7665 206f 6e65      # remove one
+00009e40: 7320 7769 7468 2062 6164 2061 6d70 6c69  s with bad ampli
+00009e50: 7475 6465 0a20 2020 2020 2020 2063 635f  tude.        cc_
+00009e60: 6172 7261 7920 3d20 6363 5f61 7272 6179  array = cc_array
+00009e70: 5b74 696e 6478 2c20 3a5d 0a20 2020 2020  [tindx, :].     
+00009e80: 2020 2063 635f 7469 6d65 203d 2063 635f     cc_time = cc_
+00009e90: 7469 6d65 5b74 696e 6478 5d0a 2020 2020  time[tindx].    
+00009ea0: 2020 2020 6363 5f6e 676f 6f64 203d 2063      cc_ngood = c
+00009eb0: 635f 6e67 6f6f 645b 7469 6e64 785d 0a0a  c_ngood[tindx]..
+00009ec0: 2020 2020 2020 2020 2320 646f 2073 7562          # do sub
+00009ed0: 7374 6163 6b73 0a20 2020 2020 2020 2069  stacks.        i
+00009ee0: 6620 726d 615f 7375 6273 7461 636b 3a0a  f rma_substack:.
+00009ef0: 2020 2020 2020 2020 2020 2020 7473 7461              tsta
+00009f00: 7274 203d 206f 6273 7079 2e55 5443 4461  rt = obspy.UTCDa
+00009f10: 7465 5469 6d65 2873 7461 7274 5f64 6174  teTime(start_dat
+00009f20: 6529 202d 206f 6273 7079 2e55 5443 4461  e) - obspy.UTCDa
+00009f30: 7465 5469 6d65 2831 3937 302c 2031 2c20  teTime(1970, 1, 
+00009f40: 3129 0a20 2020 2020 2020 2020 2020 2074  1).            t
+00009f50: 656e 6420 3d20 6f62 7370 792e 5554 4344  end = obspy.UTCD
+00009f60: 6174 6554 696d 6528 656e 645f 6461 7465  ateTime(end_date
+00009f70: 2920 2d20 6f62 7370 792e 5554 4344 6174  ) - obspy.UTCDat
+00009f80: 6554 696d 6528 3139 3730 2c20 312c 2031  eTime(1970, 1, 1
+00009f90: 290a 2020 2020 2020 2020 2020 2020 7474  ).            tt
+00009fa0: 696d 6520 3d20 7473 7461 7274 0a20 2020  ime = tstart.   
+00009fb0: 2020 2020 2020 2020 206e 7374 6163 6b20           nstack 
+00009fc0: 3d20 696e 7428 6e70 2e72 6f75 6e64 2828  = int(np.round((
+00009fd0: 7465 6e64 202d 2074 7374 6172 7429 202f  tend - tstart) /
+00009fe0: 2028 726d 615f 7374 6570 202a 2033 3630   (rma_step * 360
+00009ff0: 3029 2929 0a20 2020 2020 2020 2020 2020  0))).           
+0000a000: 206e 6363 5f61 7272 6179 203d 206e 702e   ncc_array = np.
+0000a010: 7a65 726f 7328 7368 6170 653d 286e 7374  zeros(shape=(nst
+0000a020: 6163 6b2c 206e 7074 7329 2c20 6474 7970  ack, npts), dtyp
+0000a030: 653d 6e70 2e66 6c6f 6174 3332 290a 2020  e=np.float32).  
+0000a040: 2020 2020 2020 2020 2020 6e63 635f 7469            ncc_ti
+0000a050: 6d65 203d 206e 702e 7a65 726f 7328 6e73  me = np.zeros(ns
+0000a060: 7461 636b 2c20 6474 7970 653d 6e70 2e66  tack, dtype=np.f
+0000a070: 6c6f 6174 290a 2020 2020 2020 2020 2020  loat).          
+0000a080: 2020 6e63 635f 6e67 6f6f 6420 3d20 6e70    ncc_ngood = np
+0000a090: 2e7a 6572 6f73 286e 7374 6163 6b2c 2064  .zeros(nstack, d
+0000a0a0: 7479 7065 3d6e 702e 696e 7429 0a0a 2020  type=np.int)..  
+0000a0b0: 2020 2020 2020 2020 2020 2320 6c6f 6f70            # loop
+0000a0c0: 2074 6872 6f75 6768 2065 6163 6820 7469   through each ti
+0000a0d0: 6d65 0a20 2020 2020 2020 2020 2020 2066  me.            f
+0000a0e0: 6f72 2069 6920 696e 2072 616e 6765 286e  or ii in range(n
+0000a0f0: 7374 6163 6b29 3a0a 2020 2020 2020 2020  stack):.        
+0000a100: 2020 2020 2020 2020 7369 6e64 7820 3d20          sindx = 
+0000a110: 6e70 2e77 6865 7265 2828 6363 5f74 696d  np.where((cc_tim
+0000a120: 6520 3e3d 2074 7469 6d65 2920 2620 2863  e >= ttime) & (c
+0000a130: 635f 7469 6d65 203c 2074 7469 6d65 202b  c_time < ttime +
+0000a140: 2072 6d61 5f73 7562 7374 6163 6b20 2a20   rma_substack * 
+0000a150: 3336 3030 2929 5b30 5d0a 0a20 2020 2020  3600))[0]..     
+0000a160: 2020 2020 2020 2020 2020 2023 2077 6865             # whe
+0000a170: 6e20 7468 6572 6520 6172 6520 6461 7461  n there are data
+0000a180: 2069 6e20 7468 6520 7469 6d65 2077 696e   in the time win
+0000a190: 646f 770a 2020 2020 2020 2020 2020 2020  dow.            
+0000a1a0: 2020 2020 6966 206c 656e 2873 696e 6478      if len(sindx
+0000a1b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000a1c0: 2020 2020 2020 206e 6363 5f61 7272 6179         ncc_array
+0000a1d0: 5b69 695d 203d 206e 702e 6d65 616e 2863  [ii] = np.mean(c
+0000a1e0: 635f 6172 7261 795b 7369 6e64 785d 2c20  c_array[sindx], 
+0000a1f0: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
+0000a200: 2020 2020 2020 2020 2020 2020 6e63 635f              ncc_
+0000a210: 7469 6d65 5b69 695d 203d 2074 7469 6d65  time[ii] = ttime
+0000a220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a230: 2020 2020 206e 6363 5f6e 676f 6f64 5b69       ncc_ngood[i
+0000a240: 695d 203d 206e 702e 7375 6d28 6363 5f6e  i] = np.sum(cc_n
+0000a250: 676f 6f64 5b73 696e 6478 5d2c 2061 7869  good[sindx], axi
+0000a260: 733d 3029 0a20 2020 2020 2020 2020 2020  s=0).           
+0000a270: 2020 2020 2074 7469 6d65 202b 3d20 726d       ttime += rm
+0000a280: 615f 7374 6570 202a 2033 3630 300a 0a20  a_step * 3600.. 
+0000a290: 2020 2020 2020 2020 2020 2023 2072 656d             # rem
+0000a2a0: 6f76 6520 6261 6420 6f6e 6573 0a20 2020  ove bad ones.   
+0000a2b0: 2020 2020 2020 2020 2074 696e 6478 203d           tindx =
+0000a2c0: 206e 702e 7768 6572 6528 6e63 635f 6e67   np.where(ncc_ng
+0000a2d0: 6f6f 6420 3e20 3029 5b30 5d0a 2020 2020  ood > 0)[0].    
+0000a2e0: 2020 2020 2020 2020 6e63 635f 6172 7261          ncc_arra
+0000a2f0: 7920 3d20 6e63 635f 6172 7261 795b 7469  y = ncc_array[ti
+0000a300: 6e64 785d 0a20 2020 2020 2020 2020 2020  ndx].           
+0000a310: 206e 6363 5f74 696d 6520 3d20 6e63 635f   ncc_time = ncc_
+0000a320: 7469 6d65 5b74 696e 6478 5d0a 2020 2020  time[tindx].    
+0000a330: 2020 2020 2020 2020 6e63 635f 6e67 6f6f          ncc_ngoo
+0000a340: 6420 3d20 6e63 635f 6e67 6f6f 645b 7469  d = ncc_ngood[ti
+0000a350: 6e64 785d 0a0a 2020 2020 2020 2020 2320  ndx]..        # 
+0000a360: 646f 2073 7461 636b 696e 670a 2020 2020  do stacking.    
+0000a370: 2020 2020 616c 6c73 7461 636b 7331 203d      allstacks1 =
+0000a380: 206e 702e 7a65 726f 7328 6e70 7473 2c20   np.zeros(npts, 
+0000a390: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
+0000a3a0: 290a 2020 2020 2020 2020 616c 6c73 7461  ).        allsta
+0000a3b0: 636b 7332 203d 206e 702e 7a65 726f 7328  cks2 = np.zeros(
+0000a3c0: 6e70 7473 2c20 6474 7970 653d 6e70 2e66  npts, dtype=np.f
+0000a3d0: 6c6f 6174 3332 290a 2020 2020 2020 2020  loat32).        
+0000a3e0: 616c 6c73 7461 636b 7333 203d 206e 702e  allstacks3 = np.
+0000a3f0: 7a65 726f 7328 6e70 7473 2c20 6474 7970  zeros(npts, dtyp
+0000a400: 653d 6e70 2e66 6c6f 6174 3332 290a 2020  e=np.float32).  
+0000a410: 2020 2020 2020 616c 6c73 7461 636b 7334        allstacks4
+0000a420: 203d 206e 702e 7a65 726f 7328 6e70 7473   = np.zeros(npts
+0000a430: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+0000a440: 3332 290a 0a20 2020 2020 2020 2069 6620  32)..        if 
+0000a450: 736d 6574 686f 6420 3d3d 2022 6c69 6e65  smethod == "line
+0000a460: 6172 223a 0a20 2020 2020 2020 2020 2020  ar":.           
+0000a470: 2061 6c6c 7374 6163 6b73 3120 3d20 6e70   allstacks1 = np
+0000a480: 2e6d 6561 6e28 6363 5f61 7272 6179 2c20  .mean(cc_array, 
+0000a490: 6178 6973 3d30 290a 2020 2020 2020 2020  axis=0).        
+0000a4a0: 656c 6966 2073 6d65 7468 6f64 203d 3d20  elif smethod == 
+0000a4b0: 2270 7773 223a 0a20 2020 2020 2020 2020  "pws":.         
+0000a4c0: 2020 2061 6c6c 7374 6163 6b73 3120 3d20     allstacks1 = 
+0000a4d0: 7077 7328 6363 5f61 7272 6179 2c20 7361  pws(cc_array, sa
+0000a4e0: 6d70 5f66 7265 7129 0a20 2020 2020 2020  mp_freq).       
+0000a4f0: 2065 6c69 6620 736d 6574 686f 6420 3d3d   elif smethod ==
+0000a500: 2022 726f 6275 7374 223a 0a20 2020 2020   "robust":.     
+0000a510: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
+0000a520: 2020 2020 2020 2020 2061 6c6c 7374 6163           allstac
+0000a530: 6b73 312c 0a20 2020 2020 2020 2020 2020  ks1,.           
+0000a540: 2020 2020 2077 2c0a 2020 2020 2020 2020       w,.        
+0000a550: 2020 2020 2920 3d20 726f 6275 7374 5f73      ) = robust_s
+0000a560: 7461 636b 2863 635f 6172 7261 792c 2030  tack(cc_array, 0
+0000a570: 2e30 3031 290a 2020 2020 2020 2020 656c  .001).        el
+0000a580: 6966 2073 6d65 7468 6f64 203d 3d20 2273  if smethod == "s
+0000a590: 656c 6563 7469 7665 223a 0a20 2020 2020  elective":.     
+0000a5a0: 2020 2020 2020 2061 6c6c 7374 6163 6b73         allstacks
+0000a5b0: 3120 3d20 7365 6c65 6374 6976 655f 7374  1 = selective_st
+0000a5c0: 6163 6b28 6363 5f61 7272 6179 2c20 302e  ack(cc_array, 0.
+0000a5d0: 3030 3129 0a20 2020 2020 2020 2065 6c69  001).        eli
+0000a5e0: 6620 736d 6574 686f 6420 3d3d 2022 616c  f smethod == "al
+0000a5f0: 6c22 3a0a 2020 2020 2020 2020 2020 2020  l":.            
+0000a600: 616c 6c73 7461 636b 7331 203d 206e 702e  allstacks1 = np.
+0000a610: 6d65 616e 2863 635f 6172 7261 792c 2061  mean(cc_array, a
+0000a620: 7869 733d 3029 0a20 2020 2020 2020 2020  xis=0).         
+0000a630: 2020 2061 6c6c 7374 6163 6b73 3220 3d20     allstacks2 = 
+0000a640: 7077 7328 6363 5f61 7272 6179 2c20 7361  pws(cc_array, sa
+0000a650: 6d70 5f66 7265 7129 0a20 2020 2020 2020  mp_freq).       
+0000a660: 2020 2020 2061 6c6c 7374 6163 6b73 3320       allstacks3 
+0000a670: 3d20 726f 6275 7374 5f73 7461 636b 2863  = robust_stack(c
+0000a680: 635f 6172 7261 792c 2030 2e30 3031 290a  c_array, 0.001).
+0000a690: 2020 2020 2020 2020 2020 2020 616c 6c73              alls
+0000a6a0: 7461 636b 7334 203d 2073 656c 6563 7469  tacks4 = selecti
+0000a6b0: 7665 5f73 7461 636b 2863 635f 6172 7261  ve_stack(cc_arra
+0000a6c0: 792c 2030 2e30 3031 290a 2020 2020 2020  y, 0.001).      
+0000a6d0: 2020 6e73 7461 636b 7320 3d20 6e70 2e73    nstacks = np.s
+0000a6e0: 756d 2863 635f 6e67 6f6f 6429 0a0a 2020  um(cc_ngood)..  
+0000a6f0: 2020 2320 7265 706c 6163 6520 7468 6520    # replace the 
+0000a700: 6172 7261 7920 666f 7220 7375 6273 7461  array for substa
+0000a710: 636b 730a 2020 2020 6966 2072 6d61 5f73  cks.    if rma_s
+0000a720: 7562 7374 6163 6b3a 0a20 2020 2020 2020  ubstack:.       
+0000a730: 2063 635f 6172 7261 7920 3d20 6e63 635f   cc_array = ncc_
+0000a740: 6172 7261 790a 2020 2020 2020 2020 6363  array.        cc
+0000a750: 5f74 696d 6520 3d20 6e63 635f 7469 6d65  _time = ncc_time
+0000a760: 0a20 2020 2020 2020 2063 635f 6e67 6f6f  .        cc_ngoo
+0000a770: 6420 3d20 6e63 635f 6e67 6f6f 640a 0a20  d = ncc_ngood.. 
+0000a780: 2020 2023 2067 6f6f 6420 746f 2072 6574     # good to ret
+0000a790: 7572 6e0a 2020 2020 7265 7475 726e 2028  urn.    return (
+0000a7a0: 0a20 2020 2020 2020 2063 635f 6172 7261  .        cc_arra
+0000a7b0: 792c 0a20 2020 2020 2020 2063 635f 6e67  y,.        cc_ng
+0000a7c0: 6f6f 642c 0a20 2020 2020 2020 2063 635f  ood,.        cc_
+0000a7d0: 7469 6d65 2c0a 2020 2020 2020 2020 616c  time,.        al
+0000a7e0: 6c73 7461 636b 7331 2c0a 2020 2020 2020  lstacks1,.      
+0000a7f0: 2020 616c 6c73 7461 636b 7332 2c0a 2020    allstacks2,.  
+0000a800: 2020 2020 2020 616c 6c73 7461 636b 7333        allstacks3
+0000a810: 2c0a 2020 2020 2020 2020 616c 6c73 7461  ,.        allsta
+0000a820: 636b 7334 2c0a 2020 2020 2020 2020 6e73  cks4,.        ns
+0000a830: 7461 636b 732c 0a20 2020 2029 0a0a 0a64  tacks,.    )...d
+0000a840: 6566 2072 6f74 6174 696f 6e28 6269 6773  ef rotation(bigs
+0000a850: 7461 636b 2c20 7061 7261 6d65 7465 7273  tack, parameters
+0000a860: 2c20 6c6f 6373 293a 0a20 2020 2022 2222  , locs):.    """
+0000a870: 0a20 2020 2074 6869 7320 6675 6e63 7469  .    this functi
+0000a880: 6f6e 2074 7261 6e73 6665 7273 2074 6865  on transfers the
+0000a890: 2047 7265 656e 2773 2074 656e 736f 7220   Green's tensor 
+0000a8a0: 6672 6f6d 2061 2045 2d4e 2d5a 2073 7973  from a E-N-Z sys
+0000a8b0: 7465 6d20 696e 746f 2061 2052 2d54 2d5a  tem into a R-T-Z
+0000a8c0: 206f 6e65 0a0a 2020 2020 5041 5241 4d45   one..    PARAME
+0000a8d0: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
+0000a8e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0000a8f0: 2020 6269 6773 7461 636b 3a20 2020 3920    bigstack:   9 
+0000a900: 636f 6d70 6f6e 656e 7420 4772 6565 6e27  component Green'
+0000a910: 7320 7465 6e73 6f72 2069 6e20 452d 4e2d  s tensor in E-N-
+0000a920: 5a20 7379 7374 656d 0a20 2020 2070 6172  Z system.    par
+0000a930: 616d 6574 6572 733a 2064 6963 7420 636f  ameters: dict co
+0000a940: 6e74 6169 6e69 6e67 2061 6c6c 2070 6172  ntaining all par
+0000a950: 616d 6574 6572 7320 7361 7665 6420 696e  ameters saved in
+0000a960: 2041 5344 4620 6669 6c65 0a20 2020 206c   ASDF file.    l
+0000a970: 6f63 733a 2020 2020 2020 2064 6963 7420  ocs:       dict 
+0000a980: 636f 6e74 6169 6e69 6e67 2073 7461 7469  containing stati
+0000a990: 6f6e 2061 6e67 6c65 2069 6e66 6f20 666f  on angle info fo
+0000a9a0: 7220 636f 7272 6563 7469 6f6e 2070 7572  r correction pur
+0000a9b0: 706f 7365 0a20 2020 2052 4554 5552 4e53  pose.    RETURNS
+0000a9c0: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
+0000a9d0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7463  ---------.    tc
+0000a9e0: 6f72 723a 2039 2063 6f6d 706f 6e65 6e74  orr: 9 component
+0000a9f0: 2047 7265 656e 2773 2074 656e 736f 7220   Green's tensor 
+0000aa00: 696e 2052 2d54 2d5a 2073 7973 7465 6d0a  in R-T-Z system.
+0000aa10: 2020 2020 2222 220a 2020 2020 2320 6c6f      """.    # lo
+0000aa20: 6164 2070 6172 616d 6574 6572 2064 6963  ad parameter dic
+0000aa30: 0a20 2020 2070 6920 3d20 6e70 2e70 690a  .    pi = np.pi.
+0000aa40: 2020 2020 617a 6920 3d20 7061 7261 6d65      azi = parame
+0000aa50: 7465 7273 5b22 617a 6922 5d0a 2020 2020  ters["azi"].    
+0000aa60: 6261 7a20 3d20 7061 7261 6d65 7465 7273  baz = parameters
+0000aa70: 5b22 6261 7a22 5d0a 2020 2020 6e63 6f6d  ["baz"].    ncom
+0000aa80: 702c 206e 7074 7320 3d20 6269 6773 7461  p, npts = bigsta
+0000aa90: 636b 2e73 6861 7065 0a20 2020 2069 6620  ck.shape.    if 
+0000aaa0: 6e63 6f6d 7020 3c20 393a 0a20 2020 2020  ncomp < 9:.     
+0000aab0: 2020 2070 7269 6e74 2822 6372 6170 2064     print("crap d
+0000aac0: 6964 206e 6f74 2067 6574 2065 6e6f 7567  id not get enoug
+0000aad0: 6820 636f 6d70 6f6e 656e 7473 2229 0a20  h components"). 
+0000aae0: 2020 2020 2020 2074 636f 7272 203d 205b         tcorr = [
+0000aaf0: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
+0000ab00: 2074 636f 7272 0a20 2020 2073 7461 5320   tcorr.    staS 
+0000ab10: 3d20 7061 7261 6d65 7465 7273 5b22 7374  = parameters["st
+0000ab20: 6174 696f 6e5f 736f 7572 6365 225d 0a20  ation_source"]. 
+0000ab30: 2020 2073 7461 5220 3d20 7061 7261 6d65     staR = parame
+0000ab40: 7465 7273 5b22 7374 6174 696f 6e5f 7265  ters["station_re
+0000ab50: 6365 6976 6572 225d 0a0a 2020 2020 6966  ceiver"]..    if
+0000ab60: 206c 656e 286c 6f63 7329 3a0a 2020 2020   len(locs):.    
+0000ab70: 2020 2020 7374 615f 6c69 7374 203d 206c      sta_list = l
+0000ab80: 6973 7428 6c6f 6373 5b22 7374 6174 696f  ist(locs["statio
+0000ab90: 6e22 5d29 0a20 2020 2020 2020 2061 6e67  n"]).        ang
+0000aba0: 6c65 7320 3d20 6c69 7374 286c 6f63 735b  les = list(locs[
+0000abb0: 2261 6e67 6c65 225d 290a 2020 2020 2020  "angle"]).      
+0000abc0: 2020 2320 6765 7420 7374 6174 696f 6e20    # get station 
+0000abd0: 696e 666f 2066 726f 6d20 7468 6520 6e61  info from the na
+0000abe0: 6d65 206f 6620 4153 4446 2066 696c 650a  me of ASDF file.
+0000abf0: 2020 2020 2020 2020 696e 6420 3d20 7374          ind = st
+0000ac00: 615f 6c69 7374 2e69 6e64 6578 2873 7461  a_list.index(sta
+0000ac10: 5329 0a20 2020 2020 2020 2061 636f 7272  S).        acorr
+0000ac20: 203d 2061 6e67 6c65 735b 696e 645d 0a20   = angles[ind]. 
+0000ac30: 2020 2020 2020 2069 6e64 203d 2073 7461         ind = sta
+0000ac40: 5f6c 6973 742e 696e 6465 7828 7374 6152  _list.index(staR
+0000ac50: 290a 2020 2020 2020 2020 6263 6f72 7220  ).        bcorr 
+0000ac60: 3d20 616e 676c 6573 5b69 6e64 5d0a 0a20  = angles[ind].. 
+0000ac70: 2020 2023 202d 2d2d 616e 676c 6573 2074     # ---angles t
+0000ac80: 6f20 6265 2063 6f72 7265 6374 6564 2d2d  o be corrected--
+0000ac90: 2d2d 0a20 2020 2069 6620 6c65 6e28 6c6f  --.    if len(lo
+0000aca0: 6373 293a 0a20 2020 2020 2020 2063 6f73  cs):.        cos
+0000acb0: 6120 3d20 6e70 2e63 6f73 2828 617a 6920  a = np.cos((azi 
+0000acc0: 2b20 6163 6f72 7229 202a 2070 6920 2f20  + acorr) * pi / 
+0000acd0: 3138 3029 0a20 2020 2020 2020 2073 696e  180).        sin
+0000ace0: 6120 3d20 6e70 2e73 696e 2828 617a 6920  a = np.sin((azi 
+0000acf0: 2b20 6163 6f72 7229 202a 2070 6920 2f20  + acorr) * pi / 
+0000ad00: 3138 3029 0a20 2020 2020 2020 2063 6f73  180).        cos
+0000ad10: 6220 3d20 6e70 2e63 6f73 2828 6261 7a20  b = np.cos((baz 
+0000ad20: 2b20 6263 6f72 7229 202a 2070 6920 2f20  + bcorr) * pi / 
+0000ad30: 3138 3029 0a20 2020 2020 2020 2073 696e  180).        sin
+0000ad40: 6220 3d20 6e70 2e73 696e 2828 6261 7a20  b = np.sin((baz 
+0000ad50: 2b20 6263 6f72 7229 202a 2070 6920 2f20  + bcorr) * pi / 
+0000ad60: 3138 3029 0a20 2020 2065 6c73 653a 0a20  180).    else:. 
+0000ad70: 2020 2020 2020 2063 6f73 6120 3d20 6e70         cosa = np
+0000ad80: 2e63 6f73 2861 7a69 202a 2070 6920 2f20  .cos(azi * pi / 
+0000ad90: 3138 3029 0a20 2020 2020 2020 2073 696e  180).        sin
+0000ada0: 6120 3d20 6e70 2e73 696e 2861 7a69 202a  a = np.sin(azi *
+0000adb0: 2070 6920 2f20 3138 3029 0a20 2020 2020   pi / 180).     
+0000adc0: 2020 2063 6f73 6220 3d20 6e70 2e63 6f73     cosb = np.cos
+0000add0: 2862 617a 202a 2070 6920 2f20 3138 3029  (baz * pi / 180)
+0000ade0: 0a20 2020 2020 2020 2073 696e 6220 3d20  .        sinb = 
+0000adf0: 6e70 2e73 696e 2862 617a 202a 2070 6920  np.sin(baz * pi 
+0000ae00: 2f20 3138 3029 0a0a 2020 2020 2320 7274  / 180)..    # rt
+0000ae10: 7a5f 636f 6d70 6f6e 656e 7473 203d 205b  z_components = [
+0000ae20: 275a 5227 2c27 5a54 272c 275a 5a27 2c27  'ZR','ZT','ZZ','
+0000ae30: 5252 272c 2752 5427 2c27 525a 272c 2754  RR','RT','RZ','T
+0000ae40: 5227 2c27 5454 272c 2754 5a27 5d0a 2020  R','TT','TZ'].  
+0000ae50: 2020 7463 6f72 7220 3d20 6e70 2e7a 6572    tcorr = np.zer
+0000ae60: 6f73 2873 6861 7065 3d28 392c 206e 7074  os(shape=(9, npt
+0000ae70: 7329 2c20 6474 7970 653d 6e70 2e66 6c6f  s), dtype=np.flo
+0000ae80: 6174 3332 290a 2020 2020 7463 6f72 725b  at32).    tcorr[
+0000ae90: 305d 203d 202d 636f 7362 202a 2062 6967  0] = -cosb * big
+0000aea0: 7374 6163 6b5b 375d 202d 2073 696e 6220  stack[7] - sinb 
+0000aeb0: 2a20 6269 6773 7461 636b 5b36 5d0a 2020  * bigstack[6].  
+0000aec0: 2020 7463 6f72 725b 315d 203d 2073 696e    tcorr[1] = sin
+0000aed0: 6220 2a20 6269 6773 7461 636b 5b37 5d20  b * bigstack[7] 
+0000aee0: 2d20 636f 7362 202a 2062 6967 7374 6163  - cosb * bigstac
+0000aef0: 6b5b 365d 0a20 2020 2074 636f 7272 5b32  k[6].    tcorr[2
+0000af00: 5d20 3d20 6269 6773 7461 636b 5b38 5d0a  ] = bigstack[8].
+0000af10: 2020 2020 7463 6f72 725b 335d 203d 2028      tcorr[3] = (
+0000af20: 0a20 2020 2020 2020 202d 636f 7361 202a  .        -cosa *
+0000af30: 2063 6f73 6220 2a20 6269 6773 7461 636b   cosb * bigstack
+0000af40: 5b34 5d20 2d20 636f 7361 202a 2073 696e  [4] - cosa * sin
+0000af50: 6220 2a20 6269 6773 7461 636b 5b33 5d20  b * bigstack[3] 
+0000af60: 2d20 7369 6e61 202a 2063 6f73 6220 2a20  - sina * cosb * 
+0000af70: 6269 6773 7461 636b 5b31 5d20 2d20 7369  bigstack[1] - si
+0000af80: 6e61 202a 2073 696e 6220 2a20 6269 6773  na * sinb * bigs
+0000af90: 7461 636b 5b30 5d0a 2020 2020 290a 2020  tack[0].    ).  
+0000afa0: 2020 7463 6f72 725b 345d 203d 2028 0a20    tcorr[4] = (. 
+0000afb0: 2020 2020 2020 2063 6f73 6120 2a20 7369         cosa * si
+0000afc0: 6e62 202a 2062 6967 7374 6163 6b5b 345d  nb * bigstack[4]
+0000afd0: 202d 2063 6f73 6120 2a20 636f 7362 202a   - cosa * cosb *
+0000afe0: 2062 6967 7374 6163 6b5b 335d 202b 2073   bigstack[3] + s
+0000aff0: 696e 6120 2a20 7369 6e62 202a 2062 6967  ina * sinb * big
+0000b000: 7374 6163 6b5b 315d 202d 2073 696e 6120  stack[1] - sina 
+0000b010: 2a20 636f 7362 202a 2062 6967 7374 6163  * cosb * bigstac
+0000b020: 6b5b 305d 0a20 2020 2029 0a20 2020 2074  k[0].    ).    t
+0000b030: 636f 7272 5b35 5d20 3d20 636f 7361 202a  corr[5] = cosa *
+0000b040: 2062 6967 7374 6163 6b5b 355d 202b 2073   bigstack[5] + s
+0000b050: 696e 6120 2a20 6269 6773 7461 636b 5b32  ina * bigstack[2
+0000b060: 5d0a 2020 2020 7463 6f72 725b 365d 203d  ].    tcorr[6] =
+0000b070: 2028 0a20 2020 2020 2020 2073 696e 6120   (.        sina 
+0000b080: 2a20 636f 7362 202a 2062 6967 7374 6163  * cosb * bigstac
+0000b090: 6b5b 345d 202b 2073 696e 6120 2a20 7369  k[4] + sina * si
+0000b0a0: 6e62 202a 2062 6967 7374 6163 6b5b 335d  nb * bigstack[3]
+0000b0b0: 202d 2063 6f73 6120 2a20 636f 7362 202a   - cosa * cosb *
+0000b0c0: 2062 6967 7374 6163 6b5b 315d 202d 2063   bigstack[1] - c
+0000b0d0: 6f73 6120 2a20 7369 6e62 202a 2062 6967  osa * sinb * big
+0000b0e0: 7374 6163 6b5b 305d 0a20 2020 2029 0a20  stack[0].    ). 
+0000b0f0: 2020 2074 636f 7272 5b37 5d20 3d20 280a     tcorr[7] = (.
+0000b100: 2020 2020 2020 2020 2d73 696e 6120 2a20          -sina * 
+0000b110: 7369 6e62 202a 2062 6967 7374 6163 6b5b  sinb * bigstack[
+0000b120: 345d 202b 2073 696e 6120 2a20 636f 7362  4] + sina * cosb
+0000b130: 202a 2062 6967 7374 6163 6b5b 335d 202b   * bigstack[3] +
+0000b140: 2063 6f73 6120 2a20 7369 6e62 202a 2062   cosa * sinb * b
+0000b150: 6967 7374 6163 6b5b 315d 202d 2063 6f73  igstack[1] - cos
+0000b160: 6120 2a20 636f 7362 202a 2062 6967 7374  a * cosb * bigst
+0000b170: 6163 6b5b 305d 0a20 2020 2029 0a20 2020  ack[0].    ).   
+0000b180: 2074 636f 7272 5b38 5d20 3d20 2d73 696e   tcorr[8] = -sin
+0000b190: 6120 2a20 6269 6773 7461 636b 5b35 5d20  a * bigstack[5] 
+0000b1a0: 2b20 636f 7361 202a 2062 6967 7374 6163  + cosa * bigstac
+0000b1b0: 6b5b 325d 0a0a 2020 2020 7265 7475 726e  k[2]..    return
+0000b1c0: 2074 636f 7272 0a0a 0a23 2323 2323 2323   tcorr...#######
 0000b1d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000b1e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000b1f0: 2323 2323 2323 230a 2323 2323 2323 2323  #######.########
-0000b200: 2323 2323 2323 2055 5449 4c49 5459 2046  ###### UTILITY F
-0000b210: 554e 4354 494f 4e53 2023 2323 2323 2323  UNCTIONS #######
-0000b220: 2323 2323 2323 2323 2323 2323 0a23 2323  ############.###
-0000b230: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b1f0: 2323 2323 2323 2323 2323 2323 230a 2323  #############.##
+0000b200: 2323 2323 2323 2323 2323 2323 2055 5449  ############ UTI
+0000b210: 4c49 5459 2046 554e 4354 494f 4e53 2023  LITY FUNCTIONS #
+0000b220: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b230: 2323 0a23 2323 2323 2323 2323 2323 2323  ##.#############
 0000b240: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0000b250: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000b260: 230a 0a0a 6465 6620 6368 6563 6b5f 7361  #...def check_sa
-0000b270: 6d70 6c65 5f67 6170 7328 7374 7265 616d  mple_gaps(stream
-0000b280: 3a20 6f62 7370 792e 5374 7265 616d 2c20  : obspy.Stream, 
-0000b290: 7374 6172 7474 696d 653a 206f 6273 7079  starttime: obspy
-0000b2a0: 2e55 5443 4461 7465 5469 6d65 2c20 656e  .UTCDateTime, en
-0000b2b0: 6474 696d 653a 206f 6273 7079 2e55 5443  dtime: obspy.UTC
-0000b2c0: 4461 7465 5469 6d65 293a 0a20 2020 2022  DateTime):.    "
-0000b2d0: 2222 0a20 2020 2074 6869 7320 6675 6e63  "".    this func
-0000b2e0: 7469 6f6e 2063 6865 636b 7320 7361 6d70  tion checks samp
-0000b2f0: 6c69 6e67 2072 6174 6520 616e 6420 6669  ling rate and fi
-0000b300: 6e64 2067 6170 7320 6f66 2061 6c6c 2074  nd gaps of all t
-0000b310: 7261 6365 7320 696e 2073 7472 6561 6d2e  races in stream.
-0000b320: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
-0000b330: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-0000b340: 2d2d 2d2d 2d2d 0a20 2020 2073 7472 6561  ------.    strea
-0000b350: 6d3a 206f 6273 7079 2073 7472 6561 6d20  m: obspy stream 
-0000b360: 6f62 6a65 6374 2e0a 2020 2020 6461 7465  object..    date
-0000b370: 5f69 6e66 6f3a 2064 6963 7420 6f66 2073  _info: dict of s
-0000b380: 7461 7274 696e 6720 616e 6420 656e 6469  tarting and endi
-0000b390: 6e67 2074 696d 6520 6f66 2074 6865 2073  ng time of the s
-0000b3a0: 7472 6561 6d0a 0a20 2020 2052 4554 5552  tream..    RETUR
-0000b3b0: 454e 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ENS:.    -------
-0000b3c0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073  ----------.    s
-0000b3d0: 7472 6561 6d3a 204c 6973 7420 6f66 2067  tream: List of g
-0000b3e0: 6f6f 6420 7472 6163 6573 2069 6e20 7468  ood traces in th
-0000b3f0: 6520 7374 7265 616d 0a20 2020 2022 2222  e stream.    """
-0000b400: 0a20 2020 2023 2072 656d 6f76 6520 656d  .    # remove em
-0000b410: 7074 792f 6269 6720 7472 6163 6573 0a20  pty/big traces. 
-0000b420: 2020 2069 6620 6c65 6e28 7374 7265 616d     if len(stream
-0000b430: 2920 3d3d 2030 206f 7220 6c65 6e28 7374  ) == 0 or len(st
-0000b440: 7265 616d 2920 3e20 3130 303a 0a20 2020  ream) > 100:.   
-0000b450: 2020 2020 2073 7472 6561 6d20 3d20 5b5d       stream = []
-0000b460: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000b470: 7374 7265 616d 0a0a 2020 2020 2320 7265  stream..    # re
-0000b480: 6d6f 7665 2074 7261 6365 7320 7769 7468  move traces with
-0000b490: 2062 6967 2067 6170 730a 2020 2020 6966   big gaps.    if
-0000b4a0: 2070 6f72 7469 6f6e 5f67 6170 7328 7374   portion_gaps(st
-0000b4b0: 7265 616d 2c20 7374 6172 7474 696d 652c  ream, starttime,
-0000b4c0: 2065 6e64 7469 6d65 2920 3e20 302e 333a   endtime) > 0.3:
-0000b4d0: 0a20 2020 2020 2020 2073 7472 6561 6d20  .        stream 
-0000b4e0: 3d20 5b5d 0a20 2020 2020 2020 2072 6574  = [].        ret
-0000b4f0: 7572 6e20 7374 7265 616d 0a0a 2020 2020  urn stream..    
-0000b500: 6672 6571 7320 3d20 5b5d 0a20 2020 2066  freqs = [].    f
-0000b510: 6f72 2074 7220 696e 2073 7472 6561 6d3a  or tr in stream:
-0000b520: 0a20 2020 2020 2020 2066 7265 7173 2e61  .        freqs.a
-0000b530: 7070 656e 6428 696e 7428 7472 2e73 7461  ppend(int(tr.sta
-0000b540: 7473 2e73 616d 706c 696e 675f 7261 7465  ts.sampling_rate
-0000b550: 2929 0a20 2020 2066 7265 7120 3d20 6d61  )).    freq = ma
-0000b560: 7828 6672 6571 7329 0a20 2020 2066 6f72  x(freqs).    for
-0000b570: 2074 7220 696e 2073 7472 6561 6d3a 0a20   tr in stream:. 
-0000b580: 2020 2020 2020 2069 6620 696e 7428 7472         if int(tr
-0000b590: 2e73 7461 7473 2e73 616d 706c 696e 675f  .stats.sampling_
-0000b5a0: 7261 7465 2920 213d 2066 7265 713a 0a20  rate) != freq:. 
-0000b5b0: 2020 2020 2020 2020 2020 2073 7472 6561             strea
-0000b5c0: 6d2e 7265 6d6f 7665 2874 7229 0a20 2020  m.remove(tr).   
-0000b5d0: 2020 2020 2069 6620 7472 2e73 7461 7473       if tr.stats
-0000b5e0: 2e6e 7074 7320 3c20 3130 3a0a 2020 2020  .npts < 10:.    
-0000b5f0: 2020 2020 2020 2020 7374 7265 616d 2e72          stream.r
-0000b600: 656d 6f76 6528 7472 290a 0a20 2020 2072  emove(tr)..    r
-0000b610: 6574 7572 6e20 7374 7265 616d 0a0a 0a64  eturn stream...d
-0000b620: 6566 2070 6f72 7469 6f6e 5f67 6170 7328  ef portion_gaps(
-0000b630: 7374 7265 616d 2c20 7374 6172 7474 696d  stream, starttim
-0000b640: 653a 206f 6273 7079 2e55 5443 4461 7465  e: obspy.UTCDate
-0000b650: 5469 6d65 2c20 656e 6474 696d 653a 206f  Time, endtime: o
-0000b660: 6273 7079 2e55 5443 4461 7465 5469 6d65  bspy.UTCDateTime
-0000b670: 293a 0a20 2020 2022 2222 0a20 2020 2074  ):.    """.    t
-0000b680: 6869 7320 6675 6e63 7469 6f6e 2074 7261  his function tra
-0000b690: 636b 7320 7468 6520 6761 7073 2028 6e70  cks the gaps (np
-0000b6a0: 7473 2920 6672 6f6d 2074 6865 2061 6363  ts) from the acc
-0000b6b0: 756d 756c 6174 6564 2064 6966 6665 7265  umulated differe
-0000b6c0: 6e63 6520 6265 7477 6565 6e20 7374 6172  nce between star
-0000b6d0: 7474 696d 6520 616e 6420 656e 6474 696d  ttime and endtim
-0000b6e0: 650a 2020 2020 6f66 2065 6163 6820 7374  e.    of each st
-0000b6f0: 7265 616d 2074 7261 6365 2e20 6974 2072  ream trace. it r
-0000b700: 656d 6f76 6573 2074 7261 6365 2077 6974  emoves trace wit
-0000b710: 6820 6761 7020 6c65 6e67 7468 203e 2033  h gap length > 3
-0000b720: 3025 206f 6620 7472 6163 6520 7369 7a65  0% of trace size
-0000b730: 2e0a 2020 2020 5041 5241 4d45 5445 5253  ..    PARAMETERS
-0000b740: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-0000b750: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7374  ---------.    st
-0000b760: 7265 616d 3a20 6f62 7370 7920 7374 7265  ream: obspy stre
-0000b770: 616d 206f 626a 6563 740a 2020 2020 6461  am object.    da
-0000b780: 7465 5f69 6e66 6f3a 2064 6963 7420 6f66  te_info: dict of
-0000b790: 2073 7461 7274 696e 6720 616e 6420 656e   starting and en
-0000b7a0: 6469 6e67 2074 696d 6520 6f66 2074 6865  ding time of the
-0000b7b0: 2073 7472 6561 6d0a 0a20 2020 2052 4554   stream..    RET
-0000b7c0: 5552 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d  URNS:.    ------
-0000b7d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-0000b7e0: 7067 6170 733a 2070 726f 706f 7274 696f  pgaps: proportio
-0000b7f0: 6e20 6f66 2067 6170 732f 616c 6c5f 7074  n of gaps/all_pt
-0000b800: 7320 696e 2073 7472 6561 6d0a 2020 2020  s in stream.    
-0000b810: 2222 220a 2020 2020 2320 6964 6561 6c20  """.    # ideal 
-0000b820: 6475 7261 7469 6f6e 206f 6620 6461 7461  duration of data
-0000b830: 0a20 2020 206e 7074 7320 3d20 2865 6e64  .    npts = (end
-0000b840: 7469 6d65 202d 2073 7461 7274 7469 6d65  time - starttime
-0000b850: 2920 2a20 7374 7265 616d 5b30 5d2e 7374  ) * stream[0].st
-0000b860: 6174 732e 7361 6d70 6c69 6e67 5f72 6174  ats.sampling_rat
-0000b870: 650a 0a20 2020 2070 6761 7073 203d 2030  e..    pgaps = 0
-0000b880: 0a20 2020 2023 206c 6f6f 7020 7468 726f  .    # loop thro
-0000b890: 7567 6820 616c 6c20 7472 6163 6520 746f  ugh all trace to
-0000b8a0: 2061 6363 756d 756c 6174 6520 6761 7073   accumulate gaps
-0000b8b0: 0a20 2020 2066 6f72 2069 6920 696e 2072  .    for ii in r
-0000b8c0: 616e 6765 286c 656e 2873 7472 6561 6d29  ange(len(stream)
-0000b8d0: 202d 2031 293a 0a20 2020 2020 2020 2070   - 1):.        p
-0000b8e0: 6761 7073 202b 3d20 2873 7472 6561 6d5b  gaps += (stream[
-0000b8f0: 6969 202b 2031 5d2e 7374 6174 732e 7374  ii + 1].stats.st
-0000b900: 6172 7474 696d 6520 2d20 7374 7265 616d  arttime - stream
-0000b910: 5b69 695d 2e73 7461 7473 2e65 6e64 7469  [ii].stats.endti
-0000b920: 6d65 2920 2a20 7374 7265 616d 5b69 695d  me) * stream[ii]
-0000b930: 2e73 7461 7473 2e73 616d 706c 696e 675f  .stats.sampling_
-0000b940: 7261 7465 0a20 2020 2069 6620 6e70 7473  rate.    if npts
-0000b950: 2021 3d20 303a 0a20 2020 2020 2020 2070   != 0:.        p
-0000b960: 6761 7073 203d 2070 6761 7073 202f 206e  gaps = pgaps / n
-0000b970: 7074 730a 2020 2020 6966 206e 7074 7320  pts.    if npts 
-0000b980: 3d3d 2030 3a0a 2020 2020 2020 2020 7067  == 0:.        pg
-0000b990: 6170 7320 3d20 310a 2020 2020 7265 7475  aps = 1.    retu
-0000b9a0: 726e 2070 6761 7073 0a0a 0a40 6a69 7428  rn pgaps...@jit(
-0000b9b0: 2266 6c6f 6174 3332 5b3a 5d28 666c 6f61  "float32[:](floa
-0000b9c0: 7433 325b 3a5d 2c66 6c6f 6174 3332 2922  t32[:],float32)"
-0000b9d0: 290a 6465 6620 7365 676d 656e 745f 696e  ).def segment_in
-0000b9e0: 7465 7270 6f6c 6174 6528 7369 6731 2c20  terpolate(sig1, 
-0000b9f0: 6e66 7269 6329 3a0a 2020 2020 2222 220a  nfric):.    """.
-0000ba00: 2020 2020 7468 6973 2066 756e 6374 696f      this functio
-0000ba10: 6e20 696e 7465 7270 6f6c 6174 6573 2074  n interpolates t
-0000ba20: 6865 2064 6174 6120 746f 2065 6e73 7572  he data to ensur
-0000ba30: 6520 616c 6c20 706f 696e 7473 206c 6f63  e all points loc
-0000ba40: 6174 6564 206f 6e20 696e 7465 7267 6572  ated on interger
-0000ba50: 2074 696d 6573 206f 6620 7468 650a 2020   times of the.  
-0000ba60: 2020 7361 6d70 6c69 6e67 2072 6174 6520    sampling rate 
-0000ba70: 2865 2e67 2e2c 2073 7461 7274 7469 6d65  (e.g., starttime
-0000ba80: 203d 2030 303a 3030 3a30 302e 3031 352c   = 00:00:00.015,
-0000ba90: 2064 656c 7461 203d 2030 2e30 352e 290a   delta = 0.05.).
-0000baa0: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
-0000bab0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-0000bac0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073  ----------.    s
-0000bad0: 6967 313a 2020 7365 6973 6d69 6320 7265  ig1:  seismic re
-0000bae0: 636f 7264 696e 6773 2069 6e20 6120 3144  cordings in a 1D
-0000baf0: 2061 7272 6179 0a20 2020 206e 6672 6963   array.    nfric
-0000bb00: 3a20 7468 6520 616d 6f75 6e74 206f 6620  : the amount of 
-0000bb10: 7469 6d65 2064 6966 6665 7265 6e63 6520  time difference 
-0000bb20: 6265 7477 6565 6e20 7468 6520 706f 696e  between the poin
-0000bb30: 7420 616e 6420 7468 6520 6164 6a61 6365  t and the adjace
-0000bb40: 6e74 2061 7373 756d 6564 2073 616d 706c  nt assumed sampl
-0000bb50: 6573 0a20 2020 2052 4554 5552 4e53 3a0a  es.    RETURNS:.
-0000bb60: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-0000bb70: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073  ----------.    s
-0000bb80: 6967 323a 2020 696e 7465 7270 6f6c 6174  ig2:  interpolat
-0000bb90: 6564 2073 6569 736d 6963 2072 6563 6f72  ed seismic recor
-0000bba0: 6469 6e67 7320 6f6e 2074 6865 2073 616d  dings on the sam
-0000bbb0: 706c 696e 6720 706f 696e 7473 0a20 2020  pling points.   
-0000bbc0: 2022 2222 0a20 2020 206e 7074 7320 3d20   """.    npts = 
-0000bbd0: 6c65 6e28 7369 6731 290a 2020 2020 7369  len(sig1).    si
-0000bbe0: 6732 203d 206e 702e 7a65 726f 7328 6e70  g2 = np.zeros(np
-0000bbf0: 7473 2c20 6474 7970 653d 6e70 2e66 6c6f  ts, dtype=np.flo
-0000bc00: 6174 3332 290a 0a20 2020 2023 202d 2d2d  at32)..    # ---
-0000bc10: 2d69 6e73 7465 6164 206f 6620 7368 6966  -instead of shif
-0000bc20: 7469 6e67 2c20 646f 2061 2069 6e74 6572  ting, do a inter
-0000bc30: 706f 6c61 7469 6f6e 2d2d 2d2d 2d2d 0a20  polation------. 
-0000bc40: 2020 2066 6f72 2069 6920 696e 2072 616e     for ii in ran
-0000bc50: 6765 286e 7074 7329 3a0a 2020 2020 2020  ge(npts):.      
-0000bc60: 2020 2320 2d2d 2d2d 6465 616c 2077 6974    # ----deal wit
-0000bc70: 6820 6564 6765 732d 2d2d 2d2d 0a20 2020  h edges-----.   
-0000bc80: 2020 2020 2069 6620 6969 203d 3d20 3020       if ii == 0 
-0000bc90: 6f72 2069 6920 3d3d 206e 7074 7320 2d20  or ii == npts - 
-0000bca0: 313a 0a20 2020 2020 2020 2020 2020 2073  1:.            s
-0000bcb0: 6967 325b 6969 5d20 3d20 7369 6731 5b69  ig2[ii] = sig1[i
-0000bcc0: 695d 0a20 2020 2020 2020 2065 6c73 653a  i].        else:
-0000bcd0: 0a20 2020 2020 2020 2020 2020 2023 202d  .            # -
-0000bce0: 2d2d 2d2d 2d69 6e74 6572 706f 6c61 7465  -----interpolate
-0000bcf0: 2075 7369 6e67 2061 2068 6174 2066 756e   using a hat fun
-0000bd00: 6374 696f 6e2d 2d2d 2d2d 2d0a 2020 2020  ction------.    
-0000bd10: 2020 2020 2020 2020 7369 6732 5b69 695d          sig2[ii]
-0000bd20: 203d 2028 3120 2d20 6e66 7269 6329 202a   = (1 - nfric) *
-0000bd30: 2073 6967 315b 6969 202b 2031 5d20 2b20   sig1[ii + 1] + 
-0000bd40: 6e66 7269 6320 2a20 7369 6731 5b69 695d  nfric * sig1[ii]
-0000bd50: 0a0a 2020 2020 7265 7475 726e 2073 6967  ..    return sig
-0000bd60: 320a 0a0a 6465 6620 7265 7370 5f73 7065  2...def resp_spe
-0000bd70: 6374 7275 6d28 736f 7572 6365 2c20 7265  ctrum(source, re
-0000bd80: 7370 5f66 696c 652c 2064 6f77 6e73 616d  sp_file, downsam
-0000bd90: 705f 6672 6571 2c20 7072 655f 6669 6c74  p_freq, pre_filt
-0000bda0: 3d4e 6f6e 6529 3a0a 2020 2020 2222 220a  =None):.    """.
-0000bdb0: 2020 2020 7468 6973 2066 756e 6374 696f      this functio
-0000bdc0: 6e20 7265 6d6f 7665 7320 7468 6520 696e  n removes the in
-0000bdd0: 7374 7275 6d65 6e74 2072 6573 706f 6e73  strument respons
-0000bde0: 6520 7573 696e 6720 7265 7370 6f6e 7365  e using response
-0000bdf0: 2073 7065 6374 7275 6d20 6672 6f6d 2065   spectrum from e
-0000be00: 7661 6c72 6573 702e 0a20 2020 2074 6865  valresp..    the
-0000be10: 2072 6573 706f 6e73 6520 7370 6563 7472   response spectr
-0000be20: 756d 2069 7320 6576 616c 7561 7465 6420  um is evaluated 
-0000be30: 6261 7365 6420 6f6e 2052 4553 502f 505a  based on RESP/PZ
-0000be40: 2066 696c 6573 2062 6566 6f72 6520 696e   files before in
-0000be50: 7665 7274 6564 2075 7369 6e67 2074 6865  verted using the
-0000be60: 206f 6273 7079 0a20 2020 2066 756e 6374   obspy.    funct
-0000be70: 696f 6e20 6f66 2069 6e76 6572 745f 7370  ion of invert_sp
-0000be80: 6563 7472 756d 2e20 6120 6d6f 6475 6c65  ectrum. a module
-0000be90: 206f 6620 6372 6561 7465 5f72 6573 702e   of create_resp.
-0000bea0: 7079 2069 7320 7072 6f76 6964 6564 2069  py is provided i
-0000beb0: 6e20 6469 7265 6374 6f72 7920 6f66 2027  n directory of '
-0000bec0: 6164 6469 7469 6f6e 616c 5f6d 6f64 756c  additional_modul
-0000bed0: 6573 270a 2020 2020 746f 2063 7265 6174  es'.    to creat
-0000bee0: 6520 7468 6520 7265 7370 6f6e 7365 2073  e the response s
-0000bef0: 7065 6374 7275 6d0a 2020 2020 5041 5241  pectrum.    PARA
-0000bf00: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
-0000bf10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000bf20: 2d2d 0a20 2020 2073 6f75 7263 653a 206f  --.    source: o
-0000bf30: 6273 7079 2073 7472 6561 6d20 6f62 6a65  bspy stream obje
-0000bf40: 6374 206f 6620 7461 7267 6574 6564 206e  ct of targeted n
-0000bf50: 6f69 7365 2064 6174 610a 2020 2020 7265  oise data.    re
-0000bf60: 7370 5f66 696c 653a 206e 756d 7079 2064  sp_file: numpy d
-0000bf70: 6174 6120 6669 6c65 206f 6620 7265 7370  ata file of resp
-0000bf80: 6f6e 7365 2073 7065 6374 7275 6d0a 2020  onse spectrum.  
-0000bf90: 2020 646f 776e 7361 6d70 5f66 7265 713a    downsamp_freq:
-0000bfa0: 2073 616d 706c 696e 6720 7261 7465 206f   sampling rate o
-0000bfb0: 6620 7468 6520 736f 7572 6365 2064 6174  f the source dat
-0000bfc0: 610a 2020 2020 7072 655f 6669 6c74 3a20  a.    pre_filt: 
-0000bfd0: 7072 652d 6465 6669 6e65 6420 6669 6c74  pre-defined filt
-0000bfe0: 6572 2070 6172 616d 6574 6572 730a 2020  er parameters.  
-0000bff0: 2020 5245 5455 524e 533a 0a20 2020 202d    RETURNS:.    -
-0000c000: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000c010: 2d2d 2d2d 2d0a 2020 2020 736f 7572 6365  -----.    source
-0000c020: 3a20 6f62 7370 7920 7374 7265 616d 206f  : obspy stream o
-0000c030: 626a 6563 7420 6f66 206e 6f69 7365 2064  bject of noise d
-0000c040: 6174 6120 7769 7468 2069 6e73 7472 756d  ata with instrum
-0000c050: 656e 7420 7265 7370 6f6e 7365 2072 656d  ent response rem
-0000c060: 6f76 6564 0a20 2020 2022 2222 0a20 2020  oved.    """.   
-0000c070: 2023 202d 2d2d 2d2d 2d2d 2d72 6573 705f   # --------resp_
-0000c080: 6669 6c65 2069 7320 7468 6520 696e 7665  file is the inve
-0000c090: 7274 6564 2073 7065 6374 7275 6d20 7265  rted spectrum re
-0000c0a0: 7370 6f6e 7365 2d2d 2d2d 2d2d 2d2d 2d0a  sponse---------.
-0000c0b0: 2020 2020 7265 7370 7a20 3d20 6e70 2e6c      respz = np.l
-0000c0c0: 6f61 6428 7265 7370 5f66 696c 6529 0a20  oad(resp_file). 
-0000c0d0: 2020 206e 7265 7370 7a20 3d20 7265 7370     nrespz = resp
-0000c0e0: 7a5b 315d 5b3a 5d0a 2020 2020 7370 6563  z[1][:].    spec
-0000c0f0: 5f66 7265 7120 3d20 6d61 7828 7265 7370  _freq = max(resp
-0000c100: 7a5b 305d 290a 0a20 2020 2023 202d 2d2d  z[0])..    # ---
-0000c110: 2d2d 2d2d 6f6e 2063 7572 7265 6e74 2074  ----on current t
-0000c120: 7261 6365 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  race----------. 
-0000c130: 2020 206e 6666 7420 3d20 5f6e 7074 7332     nfft = _npts2
-0000c140: 6e66 6674 2873 6f75 7263 655b 305d 2e73  nfft(source[0].s
-0000c150: 7461 7473 2e6e 7074 7329 0a20 2020 2073  tats.npts).    s
-0000c160: 7073 203d 2069 6e74 2873 6f75 7263 655b  ps = int(source[
-0000c170: 305d 2e73 7461 7473 2e73 616d 706c 696e  0].stats.samplin
-0000c180: 675f 7261 7465 290a 0a20 2020 2023 202d  g_rate)..    # -
-0000c190: 2d2d 2d2d 2d2d 2d2d 646f 2074 6865 2069  --------do the i
-0000c1a0: 6e74 6572 706f 6c61 7469 6f6e 2069 6620  nterpolation if 
-0000c1b0: 6e65 6564 6564 2d2d 2d2d 2d2d 2d2d 0a20  needed--------. 
-0000c1c0: 2020 2069 6620 7370 6563 5f66 7265 7120     if spec_freq 
-0000c1d0: 3c20 302e 3520 2a20 7370 733a 0a20 2020  < 0.5 * sps:.   
-0000c1e0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0000c1f0: 4572 726f 7228 2273 7065 6374 7275 6d20  Error("spectrum 
-0000c200: 6669 6c65 2068 6173 2070 6561 6b20 6672  file has peak fr
-0000c210: 6571 2073 6d61 6c6c 6572 2074 6861 6e20  eq smaller than 
-0000c220: 7468 6520 6461 7461 2c20 6162 6f72 7421  the data, abort!
-0000c230: 2229 0a20 2020 2065 6c73 653a 0a20 2020  ").    else:.   
-0000c240: 2020 2020 2069 6e64 7820 3d20 6e70 2e77       indx = np.w
-0000c250: 6865 7265 2872 6573 707a 5b30 5d20 3c3d  here(respz[0] <=
-0000c260: 2030 2e35 202a 2073 7073 290a 2020 2020   0.5 * sps).    
-0000c270: 2020 2020 6e66 7265 7120 3d20 6e70 2e6c      nfreq = np.l
-0000c280: 696e 7370 6163 6528 302c 2030 2e35 202a  inspace(0, 0.5 *
-0000c290: 2073 7073 2c20 6e66 6674 202f 2f20 3220   sps, nfft // 2 
-0000c2a0: 2b20 3129 0a20 2020 2020 2020 206e 7265  + 1).        nre
-0000c2b0: 7370 7a20 3d20 6e70 2e69 6e74 6572 7028  spz = np.interp(
-0000c2c0: 6e66 7265 712c 206e 702e 7265 616c 2872  nfreq, np.real(r
-0000c2d0: 6573 707a 5b30 5d5b 696e 6478 5d29 2c20  espz[0][indx]), 
-0000c2e0: 7265 7370 7a5b 315d 5b69 6e64 785d 290a  respz[1][indx]).
-0000c2f0: 0a20 2020 2023 202d 2d2d 2d64 6f20 696e  .    # ----do in
-0000c300: 7465 7270 6f6c 6174 696f 6e20 6966 206e  terpolation if n
-0000c310: 6563 6573 7361 7279 2d2d 2d2d 2d0a 2020  ecessary-----.  
-0000c320: 2020 736f 7572 6365 5f73 7065 6374 203d    source_spect =
-0000c330: 206e 702e 6666 742e 7266 6674 2873 6f75   np.fft.rfft(sou
-0000c340: 7263 655b 305d 2e64 6174 612c 206e 3d6e  rce[0].data, n=n
-0000c350: 6666 7429 0a0a 2020 2020 2320 2d2d 2d2d  fft)..    # ----
-0000c360: 2d6e 7265 7370 7a20 6973 2069 6e76 6572  -nrespz is inver
-0000c370: 7365 6420 2877 6174 6572 2d6c 6576 656c  sed (water-level
-0000c380: 6564 2920 7370 6563 7472 756d 2d2d 2d2d  ed) spectrum----
-0000c390: 2d0a 2020 2020 736f 7572 6365 5f73 7065  -.    source_spe
-0000c3a0: 6374 202a 3d20 6e72 6573 707a 0a20 2020  ct *= nrespz.   
-0000c3b0: 2073 6f75 7263 655b 305d 2e64 6174 6120   source[0].data 
-0000c3c0: 3d20 6e70 2e66 6674 2e69 7266 6674 2873  = np.fft.irfft(s
-0000c3d0: 6f75 7263 655f 7370 6563 7429 5b30 203a  ource_spect)[0 :
-0000c3e0: 2073 6f75 7263 655b 305d 2e73 7461 7473   source[0].stats
-0000c3f0: 2e6e 7074 735d 0a0a 2020 2020 6966 2070  .npts]..    if p
-0000c400: 7265 5f66 696c 7420 6973 206e 6f74 204e  re_filt is not N
-0000c410: 6f6e 653a 0a20 2020 2020 2020 2073 6f75  one:.        sou
-0000c420: 7263 655b 305d 2e64 6174 6120 3d20 6e70  rce[0].data = np
-0000c430: 2e66 6c6f 6174 3332 280a 2020 2020 2020  .float32(.      
-0000c440: 2020 2020 2020 6261 6e64 7061 7373 280a        bandpass(.
-0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 736f 7572 6365 5b30 5d2e 6461 7461 2c0a  source[0].data,.
-0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c480: 7072 655f 6669 6c74 5b30 5d2c 0a20 2020  pre_filt[0],.   
-0000c490: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-0000c4a0: 5f66 696c 745b 2d31 5d2c 0a20 2020 2020  _filt[-1],.     
-0000c4b0: 2020 2020 2020 2020 2020 2064 663d 7370             df=sp
-0000c4c0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000c4d0: 2020 2063 6f72 6e65 7273 3d34 2c0a 2020     corners=4,.  
-0000c4e0: 2020 2020 2020 2020 2020 2020 2020 7a65                ze
-0000c4f0: 726f 7068 6173 653d 5472 7565 2c0a 2020  rophase=True,.  
-0000c500: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000c510: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
-0000c520: 6e20 736f 7572 6365 0a0a 0a64 6566 206d  n source...def m
-0000c530: 6164 2861 7272 293a 0a20 2020 2022 2222  ad(arr):.    """
-0000c540: 0a20 2020 204d 6564 6961 6e20 4162 736f  .    Median Abso
-0000c550: 6c75 7465 2044 6576 6961 7469 6f6e 3a20  lute Deviation: 
-0000c560: 4d41 4420 3d20 6d65 6469 616e 287c 5869  MAD = median(|Xi
-0000c570: 2d20 6d65 6469 616e 2858 297c 290a 2020  - median(X)|).  
-0000c580: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
-0000c590: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-0000c5a0: 2d2d 2d2d 2d0a 2020 2020 6172 723a 206e  -----.    arr: n
-0000c5b0: 756d 7079 2e6e 6461 7272 6179 2c20 7365  umpy.ndarray, se
-0000c5c0: 6973 6d69 6320 7472 6163 6520 6461 7461  ismic trace data
-0000c5d0: 2061 7272 6179 0a20 2020 2052 4554 5552   array.    RETUR
-0000c5e0: 4e53 3a0a 2020 2020 6461 7461 3a20 4d65  NS:.    data: Me
-0000c5f0: 6469 616e 2041 6273 6f6c 7574 6520 4465  dian Absolute De
-0000c600: 7669 6174 696f 6e20 6f66 2064 6174 610a  viation of data.
-0000c610: 2020 2020 2222 220a 2020 2020 6966 206e      """.    if n
-0000c620: 6f74 206e 702e 6d61 2e69 735f 6d61 736b  ot np.ma.is_mask
-0000c630: 6564 2861 7272 293a 0a20 2020 2020 2020  ed(arr):.       
-0000c640: 206d 6564 203d 206e 702e 6d65 6469 616e   med = np.median
-0000c650: 2861 7272 290a 2020 2020 2020 2020 6461  (arr).        da
-0000c660: 7461 203d 206e 702e 6d65 6469 616e 286e  ta = np.median(n
-0000c670: 702e 6162 7328 6172 7220 2d20 6d65 6429  p.abs(arr - med)
-0000c680: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
-0000c690: 2020 2020 6d65 6420 3d20 6e70 2e6d 612e      med = np.ma.
-0000c6a0: 6d65 6469 616e 2861 7272 290a 2020 2020  median(arr).    
-0000c6b0: 2020 2020 6461 7461 203d 206e 702e 6d61      data = np.ma
-0000c6c0: 2e6d 6564 6961 6e28 6e70 2e6d 612e 6162  .median(np.ma.ab
-0000c6d0: 7328 6172 7220 2d20 6d65 6429 290a 2020  s(arr - med)).  
-0000c6e0: 2020 7265 7475 726e 2064 6174 610a 0a0a    return data...
-0000c6f0: 6465 6620 6465 7472 656e 6428 6461 7461  def detrend(data
-0000c700: 293a 0a20 2020 2022 2222 0a20 2020 2074  ):.    """.    t
-0000c710: 6869 7320 6675 6e63 7469 6f6e 2072 656d  his function rem
-0000c720: 6f76 6573 2074 6865 2073 6967 6e61 6c20  oves the signal 
-0000c730: 7472 656e 6420 6261 7365 6420 6f6e 2051  trend based on Q
-0000c740: 5220 6465 636f 6d70 6f73 696f 6e0a 2020  R decomposion.  
-0000c750: 2020 4e4f 5445 3a20 5152 2069 7320 6120    NOTE: QR is a 
-0000c760: 6c6f 7420 6661 7374 6572 2074 6861 6e20  lot faster than 
-0000c770: 7468 6520 6c65 6173 7420 7371 7561 7265  the least square
-0000c780: 2069 6e76 6572 7369 6f6e 2075 7365 6420   inversion used 
-0000c790: 6279 0a20 2020 2073 6369 7079 2028 616c  by.    scipy (al
-0000c7a0: 736f 2069 6e20 6f62 7370 7929 2e0a 2020  so in obspy)..  
-0000c7b0: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
-0000c7c0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-0000c7d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6461 7461  -------.    data
-0000c7e0: 3a20 696e 7075 7420 6461 7461 206d 6174  : input data mat
-0000c7f0: 7269 780a 2020 2020 5245 5455 524e 533a  rix.    RETURNS:
-0000c800: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-0000c810: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
-0000c820: 6174 613a 2064 6174 6120 6d61 7472 6978  ata: data matrix
-0000c830: 2077 6974 6820 7472 656e 6420 7265 6d6f   with trend remo
-0000c840: 7665 640a 2020 2020 2222 220a 2020 2020  ved.    """.    
-0000c850: 2320 6e64 6174 6120 3d20 6e70 2e7a 6572  # ndata = np.zer
-0000c860: 6f73 2873 6861 7065 3d64 6174 612e 7368  os(shape=data.sh
-0000c870: 6170 652c 6474 7970 653d 6461 7461 2e64  ape,dtype=data.d
-0000c880: 7479 7065 290a 2020 2020 6966 2064 6174  type).    if dat
-0000c890: 612e 6e64 696d 203d 3d20 313a 0a20 2020  a.ndim == 1:.   
-0000c8a0: 2020 2020 206e 7074 7320 3d20 6461 7461       npts = data
-0000c8b0: 2e73 6861 7065 5b30 5d0a 2020 2020 2020  .shape[0].      
-0000c8c0: 2020 5820 3d20 6e70 2e6f 6e65 7328 286e    X = np.ones((n
-0000c8d0: 7074 732c 2032 2929 0a20 2020 2020 2020  pts, 2)).       
-0000c8e0: 2058 5b3a 2c20 305d 203d 206e 702e 6172   X[:, 0] = np.ar
-0000c8f0: 616e 6765 2830 2c20 6e70 7473 2920 2f20  ange(0, npts) / 
-0000c900: 6e70 7473 0a20 2020 2020 2020 2051 2c20  npts.        Q, 
-0000c910: 5220 3d20 6e70 2e6c 696e 616c 672e 7172  R = np.linalg.qr
-0000c920: 2858 290a 2020 2020 2020 2020 7271 203d  (X).        rq =
-0000c930: 206e 702e 646f 7428 6e70 2e6c 696e 616c   np.dot(np.linal
-0000c940: 672e 696e 7628 5229 2c20 512e 7472 616e  g.inv(R), Q.tran
-0000c950: 7370 6f73 6528 2929 0a20 2020 2020 2020  spose()).       
-0000c960: 2063 6f65 6666 203d 206e 702e 646f 7428   coeff = np.dot(
-0000c970: 7271 2c20 6461 7461 290a 2020 2020 2020  rq, data).      
-0000c980: 2020 6461 7461 203d 2064 6174 6120 2d20    data = data - 
-0000c990: 6e70 2e64 6f74 2858 2c20 636f 6566 6629  np.dot(X, coeff)
-0000c9a0: 0a20 2020 2065 6c69 6620 6461 7461 2e6e  .    elif data.n
-0000c9b0: 6469 6d20 3d3d 2032 3a0a 2020 2020 2020  dim == 2:.      
-0000c9c0: 2020 6e70 7473 203d 2064 6174 612e 7368    npts = data.sh
-0000c9d0: 6170 655b 315d 0a20 2020 2020 2020 2058  ape[1].        X
-0000c9e0: 203d 206e 702e 6f6e 6573 2828 6e70 7473   = np.ones((npts
-0000c9f0: 2c20 3229 290a 2020 2020 2020 2020 585b  , 2)).        X[
-0000ca00: 3a2c 2030 5d20 3d20 6e70 2e61 7261 6e67  :, 0] = np.arang
-0000ca10: 6528 302c 206e 7074 7329 202f 206e 7074  e(0, npts) / npt
-0000ca20: 730a 2020 2020 2020 2020 512c 2052 203d  s.        Q, R =
-0000ca30: 206e 702e 6c69 6e61 6c67 2e71 7228 5829   np.linalg.qr(X)
-0000ca40: 0a20 2020 2020 2020 2072 7120 3d20 6e70  .        rq = np
-0000ca50: 2e64 6f74 286e 702e 6c69 6e61 6c67 2e69  .dot(np.linalg.i
-0000ca60: 6e76 2852 292c 2051 2e74 7261 6e73 706f  nv(R), Q.transpo
-0000ca70: 7365 2829 290a 2020 2020 2020 2020 666f  se()).        fo
-0000ca80: 7220 6969 2069 6e20 7261 6e67 6528 6461  r ii in range(da
-0000ca90: 7461 2e73 6861 7065 5b30 5d29 3a0a 2020  ta.shape[0]):.  
-0000caa0: 2020 2020 2020 2020 2020 636f 6566 6620            coeff 
-0000cab0: 3d20 6e70 2e64 6f74 2872 712c 2064 6174  = np.dot(rq, dat
-0000cac0: 615b 6969 5d29 0a20 2020 2020 2020 2020  a[ii]).         
-0000cad0: 2020 2064 6174 615b 6969 5d20 3d20 6461     data[ii] = da
-0000cae0: 7461 5b69 695d 202d 206e 702e 646f 7428  ta[ii] - np.dot(
-0000caf0: 582c 2063 6f65 6666 290a 2020 2020 7265  X, coeff).    re
-0000cb00: 7475 726e 2064 6174 610a 0a0a 6465 6620  turn data...def 
-0000cb10: 6465 6d65 616e 2864 6174 6129 3a0a 2020  demean(data):.  
-0000cb20: 2020 2222 220a 2020 2020 7468 6973 2066    """.    this f
-0000cb30: 756e 6374 696f 6e20 7265 6d6f 7665 2074  unction remove t
-0000cb40: 6865 206d 6561 6e20 6f66 2074 6865 2073  he mean of the s
-0000cb50: 6967 6e61 6c0a 2020 2020 5041 5241 4d45  ignal.    PARAME
-0000cb60: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
-0000cb70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-0000cb80: 2020 2020 6461 7461 3a20 696e 7075 7420      data: input 
-0000cb90: 6461 7461 206d 6174 7269 780a 2020 2020  data matrix.    
-0000cba0: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
-0000cbb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000cbc0: 2d2d 0a20 2020 2064 6174 613a 2064 6174  --.    data: dat
-0000cbd0: 6120 6d61 7472 6978 2077 6974 6820 6d65  a matrix with me
-0000cbe0: 616e 2072 656d 6f76 6564 0a20 2020 2022  an removed.    "
-0000cbf0: 2222 0a20 2020 2023 206e 6461 7461 203d  "".    # ndata =
-0000cc00: 206e 702e 7a65 726f 7328 7368 6170 653d   np.zeros(shape=
-0000cc10: 6461 7461 2e73 6861 7065 2c64 7479 7065  data.shape,dtype
-0000cc20: 3d64 6174 612e 6474 7970 6529 0a20 2020  =data.dtype).   
-0000cc30: 2069 6620 6461 7461 2e6e 6469 6d20 3d3d   if data.ndim ==
-0000cc40: 2031 3a0a 2020 2020 2020 2020 6461 7461   1:.        data
-0000cc50: 203d 2064 6174 6120 2d20 6e70 2e6d 6561   = data - np.mea
-0000cc60: 6e28 6461 7461 290a 2020 2020 656c 6966  n(data).    elif
-0000cc70: 2064 6174 612e 6e64 696d 203d 3d20 323a   data.ndim == 2:
-0000cc80: 0a20 2020 2020 2020 2066 6f72 2069 6920  .        for ii 
-0000cc90: 696e 2072 616e 6765 2864 6174 612e 7368  in range(data.sh
-0000cca0: 6170 655b 305d 293a 0a20 2020 2020 2020  ape[0]):.       
-0000ccb0: 2020 2020 2064 6174 615b 6969 5d20 3d20       data[ii] = 
-0000ccc0: 6461 7461 5b69 695d 202d 206e 702e 6d65  data[ii] - np.me
-0000ccd0: 616e 2864 6174 615b 6969 5d29 0a20 2020  an(data[ii]).   
-0000cce0: 2072 6574 7572 6e20 6461 7461 0a0a 0a64   return data...d
-0000ccf0: 6566 2074 6170 6572 2864 6174 6129 3a0a  ef taper(data):.
-0000cd00: 2020 2020 2222 220a 2020 2020 7468 6973      """.    this
-0000cd10: 2066 756e 6374 696f 6e20 6170 706c 6965   function applie
-0000cd20: 7320 6120 636f 7369 6e65 2074 6170 6572  s a cosine taper
-0000cd30: 2075 7369 6e67 206f 6273 7079 2066 756e   using obspy fun
-0000cd40: 6374 696f 6e73 0a20 2020 2050 4152 414d  ctions.    PARAM
-0000cd50: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
-0000cd60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000cd70: 0a20 2020 2064 6174 613a 2069 6e70 7574  .    data: input
-0000cd80: 2064 6174 6120 6d61 7472 6978 0a20 2020   data matrix.   
-0000cd90: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
-0000cda0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000cdb0: 2d2d 2d0a 2020 2020 6461 7461 3a20 6461  ---.    data: da
-0000cdc0: 7461 206d 6174 7269 7820 7769 7468 2074  ta matrix with t
-0000cdd0: 6170 6572 2061 7070 6c69 6564 0a20 2020  aper applied.   
-0000cde0: 2022 2222 0a20 2020 2023 206e 6461 7461   """.    # ndata
-0000cdf0: 203d 206e 702e 7a65 726f 7328 7368 6170   = np.zeros(shap
-0000ce00: 653d 6461 7461 2e73 6861 7065 2c64 7479  e=data.shape,dty
-0000ce10: 7065 3d64 6174 612e 6474 7970 6529 0a20  pe=data.dtype). 
-0000ce20: 2020 2069 6620 6461 7461 2e6e 6469 6d20     if data.ndim 
-0000ce30: 3d3d 2031 3a0a 2020 2020 2020 2020 6e70  == 1:.        np
-0000ce40: 7473 203d 2064 6174 612e 7368 6170 655b  ts = data.shape[
-0000ce50: 305d 0a20 2020 2020 2020 2023 2077 696e  0].        # win
-0000ce60: 646f 7720 6c65 6e67 7468 0a20 2020 2020  dow length.     
-0000ce70: 2020 2069 6620 6e70 7473 202a 2030 2e30     if npts * 0.0
-0000ce80: 3520 3e20 3230 3a0a 2020 2020 2020 2020  5 > 20:.        
-0000ce90: 2020 2020 776c 656e 203d 2032 300a 2020      wlen = 20.  
-0000cea0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-0000ceb0: 2020 2020 2020 2020 776c 656e 203d 206e          wlen = n
-0000cec0: 7074 7320 2a20 302e 3035 0a20 2020 2020  pts * 0.05.     
-0000ced0: 2020 2023 2074 6170 6572 2076 616c 7565     # taper value
-0000cee0: 730a 2020 2020 2020 2020 6675 6e63 203d  s.        func =
-0000cef0: 205f 6765 745f 6675 6e63 7469 6f6e 5f66   _get_function_f
-0000cf00: 726f 6d5f 656e 7472 795f 706f 696e 7428  rom_entry_point(
-0000cf10: 2274 6170 6572 222c 2022 6861 6e6e 2229  "taper", "hann")
-0000cf20: 0a20 2020 2020 2020 2069 6620 3220 2a20  .        if 2 * 
-0000cf30: 776c 656e 203d 3d20 6e70 7473 3a0a 2020  wlen == npts:.  
-0000cf40: 2020 2020 2020 2020 2020 7461 7065 725f            taper_
-0000cf50: 7369 6465 7320 3d20 6675 6e63 2832 202a  sides = func(2 *
-0000cf60: 2077 6c65 6e29 0a20 2020 2020 2020 2065   wlen).        e
-0000cf70: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000cf80: 2074 6170 6572 5f73 6964 6573 203d 2066   taper_sides = f
-0000cf90: 756e 6328 3220 2a20 776c 656e 202b 2031  unc(2 * wlen + 1
-0000cfa0: 290a 2020 2020 2020 2020 2320 7461 7065  ).        # tape
-0000cfb0: 7220 7769 6e64 6f77 0a20 2020 2020 2020  r window.       
-0000cfc0: 2077 696e 203d 206e 702e 6873 7461 636b   win = np.hstack
-0000cfd0: 280a 2020 2020 2020 2020 2020 2020 280a  (.            (.
-0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cff0: 7461 7065 725f 7369 6465 735b 3a77 6c65  taper_sides[:wle
-0000d000: 6e5d 2c0a 2020 2020 2020 2020 2020 2020  n],.            
-0000d010: 2020 2020 6e70 2e6f 6e65 7328 6e70 7473      np.ones(npts
-0000d020: 202d 2032 202a 2077 6c65 6e29 2c0a 2020   - 2 * wlen),.  
-0000d030: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-0000d040: 7065 725f 7369 6465 735b 6c65 6e28 7461  per_sides[len(ta
-0000d050: 7065 725f 7369 6465 7329 202d 2077 6c65  per_sides) - wle
-0000d060: 6e20 3a5d 2c0a 2020 2020 2020 2020 2020  n :],.          
-0000d070: 2020 290a 2020 2020 2020 2020 290a 2020    ).        ).  
-0000d080: 2020 2020 2020 6461 7461 202a 3d20 7769        data *= wi
-0000d090: 6e0a 2020 2020 656c 6966 2064 6174 612e  n.    elif data.
-0000d0a0: 6e64 696d 203d 3d20 323a 0a20 2020 2020  ndim == 2:.     
-0000d0b0: 2020 206e 7074 7320 3d20 6461 7461 2e73     npts = data.s
-0000d0c0: 6861 7065 5b31 5d0a 2020 2020 2020 2020  hape[1].        
-0000d0d0: 2320 7769 6e64 6f77 206c 656e 6774 680a  # window length.
-0000d0e0: 2020 2020 2020 2020 6966 206e 7074 7320          if npts 
-0000d0f0: 2a20 302e 3035 203e 2032 303a 0a20 2020  * 0.05 > 20:.   
-0000d100: 2020 2020 2020 2020 2077 6c65 6e20 3d20           wlen = 
-0000d110: 3230 0a20 2020 2020 2020 2065 6c73 653a  20.        else:
-0000d120: 0a20 2020 2020 2020 2020 2020 2077 6c65  .            wle
-0000d130: 6e20 3d20 6e70 7473 202a 2030 2e30 350a  n = npts * 0.05.
-0000d140: 2020 2020 2020 2020 2320 7461 7065 7220          # taper 
-0000d150: 7661 6c75 6573 0a20 2020 2020 2020 2066  values.        f
-0000d160: 756e 6320 3d20 5f67 6574 5f66 756e 6374  unc = _get_funct
-0000d170: 696f 6e5f 6672 6f6d 5f65 6e74 7279 5f70  ion_from_entry_p
-0000d180: 6f69 6e74 2822 7461 7065 7222 2c20 2268  oint("taper", "h
-0000d190: 616e 6e22 290a 2020 2020 2020 2020 6966  ann").        if
-0000d1a0: 2032 202a 2077 6c65 6e20 3d3d 206e 7074   2 * wlen == npt
-0000d1b0: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
-0000d1c0: 6170 6572 5f73 6964 6573 203d 2066 756e  aper_sides = fun
-0000d1d0: 6328 3220 2a20 776c 656e 290a 2020 2020  c(2 * wlen).    
-0000d1e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000d1f0: 2020 2020 2020 7461 7065 725f 7369 6465        taper_side
-0000d200: 7320 3d20 6675 6e63 2832 202a 2077 6c65  s = func(2 * wle
-0000d210: 6e20 2b20 3129 0a20 2020 2020 2020 2023  n + 1).        #
-0000d220: 2074 6170 6572 2077 696e 646f 770a 2020   taper window.  
-0000d230: 2020 2020 2020 7769 6e20 3d20 6e70 2e68        win = np.h
-0000d240: 7374 6163 6b28 0a20 2020 2020 2020 2020  stack(.         
-0000d250: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
-0000d260: 2020 2020 2074 6170 6572 5f73 6964 6573       taper_sides
-0000d270: 5b3a 776c 656e 5d2c 0a20 2020 2020 2020  [:wlen],.       
-0000d280: 2020 2020 2020 2020 206e 702e 6f6e 6573           np.ones
-0000d290: 286e 7074 7320 2d20 3220 2a20 776c 656e  (npts - 2 * wlen
-0000d2a0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000d2b0: 2020 2074 6170 6572 5f73 6964 6573 5b6c     taper_sides[l
-0000d2c0: 656e 2874 6170 6572 5f73 6964 6573 2920  en(taper_sides) 
-0000d2d0: 2d20 776c 656e 203a 5d2c 0a20 2020 2020  - wlen :],.     
-0000d2e0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000d2f0: 2029 0a20 2020 2020 2020 2066 6f72 2069   ).        for i
-0000d300: 6920 696e 2072 616e 6765 2864 6174 612e  i in range(data.
-0000d310: 7368 6170 655b 305d 293a 0a20 2020 2020  shape[0]):.     
-0000d320: 2020 2020 2020 2064 6174 615b 6969 5d20         data[ii] 
-0000d330: 2a3d 2077 696e 0a20 2020 2072 6574 7572  *= win.    retur
-0000d340: 6e20 6461 7461 0a0a 0a23 2040 6a69 7428  n data...# @jit(
-0000d350: 6e6f 7079 7468 6f6e 203d 2054 7275 6529  nopython = True)
-0000d360: 0a0a 0a23 2063 6861 6e67 6520 7468 6520  ...# change the 
-0000d370: 6d6f 7669 6e67 2061 7665 7261 6765 2063  moving average c
-0000d380: 616c 6375 6c61 7469 6f6e 2074 6f20 7461  alculation to ta
-0000d390: 6b65 2061 7320 696e 7075 7420 4e20 7468  ke as input N th
-0000d3a0: 6520 6675 6c6c 2077 696e 646f 7720 6c65  e full window le
-0000d3b0: 6e67 7468 2074 6f20 736d 6f6f 7468 0a64  ngth to smooth.d
-0000d3c0: 6566 206d 6f76 696e 675f 6176 6528 412c  ef moving_ave(A,
-0000d3d0: 204e 293a 0a20 2020 2022 2222 0a20 2020   N):.    """.   
-0000d3e0: 2041 6c74 6572 6e61 7469 7665 2066 756e   Alternative fun
-0000d3f0: 6374 696f 6e20 666f 7220 6d6f 7669 6e67  ction for moving
-0000d400: 2061 7665 7261 6765 2066 6f72 2061 6e20   average for an 
-0000d410: 6172 7261 792e 0a20 2020 2050 4152 414d  array..    PARAM
-0000d420: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
-0000d430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000d440: 0a20 2020 2041 3a20 312d 4420 6172 7261  .    A: 1-D arra
-0000d450: 7920 6f66 2064 6174 6120 746f 2062 6520  y of data to be 
-0000d460: 736d 6f6f 7468 6564 0a20 2020 204e 3a20  smoothed.    N: 
-0000d470: 696e 7465 6765 722c 2069 7420 6465 6669  integer, it defi
-0000d480: 6e65 7320 7468 6520 6675 6c6c 2121 2077  nes the full!! w
-0000d490: 696e 646f 7720 6c65 6e67 7468 2074 6f20  indow length to 
-0000d4a0: 736d 6f6f 7468 0a20 2020 2052 4554 5552  smooth.    RETUR
-0000d4b0: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
-0000d4c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-0000d4d0: 2020 423a 2031 2d44 2061 7272 6179 2077    B: 1-D array w
-0000d4e0: 6974 6820 736d 6f6f 7468 6564 2064 6174  ith smoothed dat
-0000d4f0: 610a 2020 2020 2222 220a 2020 2020 2320  a.    """.    # 
-0000d500: 6465 6669 6e65 7320 616e 2061 7272 6179  defines an array
-0000d510: 2077 6974 6820 4e20 6578 7472 6120 7361   with N extra sa
-0000d520: 6d70 6c65 7320 6174 2065 6974 6865 7220  mples at either 
-0000d530: 7369 6465 0a20 2020 2074 656d 7020 3d20  side.    temp = 
-0000d540: 6e70 2e7a 6572 6f73 286c 656e 2841 2920  np.zeros(len(A) 
-0000d550: 2b20 3220 2a20 4e29 0a20 2020 2023 2073  + 2 * N).    # s
-0000d560: 6574 2074 6865 2063 656e 7472 616c 2070  et the central p
-0000d570: 6f72 7469 6f6e 206f 6620 7468 6520 6172  ortion of the ar
-0000d580: 7261 7920 746f 2041 0a20 2020 2074 656d  ray to A.    tem
-0000d590: 705b 4e3a 2d4e 5d20 3d20 410a 2020 2020  p[N:-N] = A.    
-0000d5a0: 2320 6c65 6164 696e 6720 7361 6d70 6c65  # leading sample
-0000d5b0: 733a 2065 7175 616c 2074 6f20 6669 7273  s: equal to firs
-0000d5c0: 7420 7361 6d70 6c65 206f 6620 6163 7475  t sample of actu
-0000d5d0: 616c 2061 7272 6179 0a20 2020 2074 656d  al array.    tem
-0000d5e0: 705b 303a 4e5d 203d 2074 656d 705b 4e5d  p[0:N] = temp[N]
-0000d5f0: 0a20 2020 2023 2074 7261 696c 696e 6720  .    # trailing 
-0000d600: 7361 6d70 6c65 733a 2045 7175 616c 2074  samples: Equal t
-0000d610: 6f20 6c61 7374 2073 616d 706c 6520 6f66  o last sample of
-0000d620: 2061 6374 7561 6c20 6172 7261 790a 2020   actual array.  
-0000d630: 2020 7465 6d70 5b2d 4e3a 5d20 3d20 7465    temp[-N:] = te
-0000d640: 6d70 5b2d 4e20 2d20 315d 0a20 2020 2023  mp[-N - 1].    #
-0000d650: 2063 6f6e 766f 6c76 6520 7769 7468 2061   convolve with a
-0000d660: 2062 6f78 6361 7220 616e 6420 6e6f 726d   boxcar and norm
-0000d670: 616c 697a 652c 2061 6e64 2075 7365 206f  alize, and use o
-0000d680: 6e6c 7920 6365 6e74 7261 6c20 706f 7274  nly central port
-0000d690: 696f 6e20 6f66 2074 6865 2072 6573 756c  ion of the resul
-0000d6a0: 740a 2020 2020 2320 7769 7468 206c 656e  t.    # with len
-0000d6b0: 6774 6820 6571 7561 6c20 746f 2074 6865  gth equal to the
-0000d6c0: 206f 7269 6769 6e61 6c20 6172 7261 792c   original array,
-0000d6d0: 2064 6973 6361 7264 696e 6720 7468 6520   discarding the 
-0000d6e0: 6164 6465 6420 6c65 6164 696e 6720 616e  added leading an
-0000d6f0: 6420 7472 6169 6c69 6e67 2073 616d 706c  d trailing sampl
-0000d700: 6573 0a20 2020 2042 203d 206e 702e 636f  es.    B = np.co
-0000d710: 6e76 6f6c 7665 2874 656d 702c 206e 702e  nvolve(temp, np.
-0000d720: 6f6e 6573 284e 2920 2f20 4e2c 206d 6f64  ones(N) / N, mod
-0000d730: 653d 2273 616d 6522 295b 4e3a 2d4e 5d0a  e="same")[N:-N].
-0000d740: 2020 2020 7265 7475 726e 2042 0a0a 0a23      return B...#
-0000d750: 2063 6861 6e67 6520 7468 6520 6d6f 7669   change the movi
-0000d760: 6e67 2061 7665 7261 6765 2063 616c 6375  ng average calcu
-0000d770: 6c61 7469 6f6e 2074 6f20 7461 6b65 2061  lation to take a
-0000d780: 7320 696e 7075 7420 4e20 7468 6520 6675  s input N the fu
-0000d790: 6c6c 2077 696e 646f 7720 6c65 6e67 7468  ll window length
-0000d7a0: 2074 6f20 736d 6f6f 7468 0a64 6566 206d   to smooth.def m
-0000d7b0: 6f76 696e 675f 6176 655f 3244 2841 2c20  oving_ave_2D(A, 
-0000d7c0: 4e29 3a0a 2020 2020 2222 220a 2020 2020  N):.    """.    
-0000d7d0: 416c 7465 726e 6174 6976 6520 6675 6e63  Alternative func
-0000d7e0: 7469 6f6e 2066 6f72 206d 6f76 696e 6720  tion for moving 
-0000d7f0: 6176 6572 6167 6520 666f 7220 616e 2061  average for an a
-0000d800: 7272 6179 2e0a 2020 2020 5041 5241 4d45  rray..    PARAME
-0000d810: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
-0000d820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-0000d830: 2020 2020 413a 2032 2d44 2061 7272 6179      A: 2-D array
-0000d840: 206f 6620 6461 7461 2074 6f20 6265 2073   of data to be s
-0000d850: 6d6f 6f74 6865 640a 2020 2020 4e3a 2069  moothed.    N: i
-0000d860: 6e74 6567 6572 2c20 6974 2064 6566 696e  nteger, it defin
-0000d870: 6573 2074 6865 2066 756c 6c21 2120 7769  es the full!! wi
-0000d880: 6e64 6f77 206c 656e 6774 6820 746f 2073  ndow length to s
-0000d890: 6d6f 6f74 680a 2020 2020 5245 5455 524e  mooth.    RETURN
-0000d8a0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-0000d8b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-0000d8c0: 2042 3a20 322d 4420 6172 7261 7920 7769   B: 2-D array wi
-0000d8d0: 7468 2073 6d6f 6f74 6865 6420 6461 7461  th smoothed data
-0000d8e0: 0a20 2020 2022 2222 0a20 2020 206e 7463  .    """.    ntc
-0000d8f0: 2c20 6e73 7074 203d 2041 2e73 6861 7065  , nspt = A.shape
-0000d900: 0a20 2020 2023 2064 6566 696e 6573 2061  .    # defines a
-0000d910: 6e20 6172 7261 7920 7769 7468 204e 2065  n array with N e
-0000d920: 7874 7261 2073 616d 706c 6573 2061 7420  xtra samples at 
-0000d930: 6569 7468 6572 2073 6964 650a 2020 2020  either side.    
-0000d940: 7465 6d70 203d 206e 702e 7a65 726f 7328  temp = np.zeros(
-0000d950: 5b6e 7463 2c20 6e73 7074 202b 2032 202a  [ntc, nspt + 2 *
-0000d960: 204e 5d29 0a20 2020 2023 2073 6574 2074   N]).    # set t
-0000d970: 6865 2063 656e 7472 616c 2070 6f72 7469  he central porti
-0000d980: 6f6e 206f 6620 7468 6520 6172 7261 7920  on of the array 
-0000d990: 746f 2041 0a20 2020 2074 656d 705b 3a2c  to A.    temp[:,
-0000d9a0: 204e 3a2d 4e5d 203d 2041 0a20 2020 2023   N:-N] = A.    #
-0000d9b0: 206c 6561 6469 6e67 2073 616d 706c 6573   leading samples
-0000d9c0: 3a20 6571 7561 6c20 746f 2066 6972 7374  : equal to first
-0000d9d0: 2073 616d 706c 6520 6f66 2061 6374 7561   sample of actua
-0000d9e0: 6c20 6172 7261 790a 2020 2020 7465 6d70  l array.    temp
-0000d9f0: 5b3a 2c20 303a 4e5d 203d 206e 702e 7265  [:, 0:N] = np.re
-0000da00: 7065 6174 286e 702e 6578 7061 6e64 5f64  peat(np.expand_d
-0000da10: 696d 7328 7465 6d70 5b3a 2c20 4e5d 2c20  ims(temp[:, N], 
-0000da20: 6178 6973 3d2d 3129 2c20 4e2c 2061 7869  axis=-1), N, axi
-0000da30: 733d 2d31 290a 2020 2020 2320 7472 6169  s=-1).    # trai
-0000da40: 6c69 6e67 2073 616d 706c 6573 3a20 4571  ling samples: Eq
-0000da50: 7561 6c20 746f 206c 6173 7420 7361 6d70  ual to last samp
-0000da60: 6c65 206f 6620 6163 7475 616c 2061 7272  le of actual arr
-0000da70: 6179 0a20 2020 2074 656d 705b 3a2c 202d  ay.    temp[:, -
-0000da80: 4e3a 5d20 3d20 6e70 2e72 6570 6561 7428  N:] = np.repeat(
-0000da90: 6e70 2e65 7870 616e 645f 6469 6d73 2874  np.expand_dims(t
-0000daa0: 656d 705b 3a2c 202d 4e20 2d20 315d 2c20  emp[:, -N - 1], 
-0000dab0: 6178 6973 3d2d 3129 2c20 4e2c 2061 7869  axis=-1), N, axi
-0000dac0: 733d 2d31 290a 2020 2020 2320 636f 6e76  s=-1).    # conv
-0000dad0: 6f6c 7665 2077 6974 6820 6120 626f 7863  olve with a boxc
-0000dae0: 6172 2061 6e64 206e 6f72 6d61 6c69 7a65  ar and normalize
-0000daf0: 2c20 616e 6420 7573 6520 6f6e 6c79 2063  , and use only c
-0000db00: 656e 7472 616c 2070 6f72 7469 6f6e 206f  entral portion o
-0000db10: 6620 7468 6520 7265 7375 6c74 0a20 2020  f the result.   
-0000db20: 2023 2077 6974 6820 6c65 6e67 7468 2065   # with length e
-0000db30: 7175 616c 2074 6f20 7468 6520 6f72 6967  qual to the orig
-0000db40: 696e 616c 2061 7272 6179 2c20 6469 7363  inal array, disc
-0000db50: 6172 6469 6e67 2074 6865 2061 6464 6564  arding the added
-0000db60: 206c 6561 6469 6e67 2061 6e64 2074 7261   leading and tra
-0000db70: 696c 696e 6720 7361 6d70 6c65 730a 2020  iling samples.  
-0000db80: 2020 4220 3d20 7363 6970 792e 7369 676e    B = scipy.sign
-0000db90: 616c 2e63 6f6e 766f 6c76 6532 6428 7465  al.convolve2d(te
-0000dba0: 6d70 2c20 6e70 2e65 7870 616e 645f 6469  mp, np.expand_di
-0000dbb0: 6d73 286e 702e 6f6e 6573 284e 2920 2f20  ms(np.ones(N) / 
-0000dbc0: 4e2c 2061 7869 733d 3029 2c20 6d6f 6465  N, axis=0), mode
-0000dbd0: 3d22 7361 6d65 2229 5b3a 2c20 4e3a 2d4e  ="same")[:, N:-N
-0000dbe0: 5d0a 2020 2020 7265 7475 726e 2042 0a0a  ].    return B..
-0000dbf0: 0a64 6566 2072 6f62 7573 745f 7374 6163  .def robust_stac
-0000dc00: 6b28 6363 5f61 7272 6179 2c20 6570 7369  k(cc_array, epsi
-0000dc10: 6c6f 6e29 3a0a 2020 2020 2222 220a 2020  lon):.    """.  
-0000dc20: 2020 7468 6973 2069 7320 6120 726f 6275    this is a robu
-0000dc30: 7374 2073 7461 636b 696e 6720 616c 676f  st stacking algo
-0000dc40: 7269 7468 6d20 6465 7363 7269 6265 6420  rithm described 
-0000dc50: 696e 2050 616c 7669 7320 616e 6420 5665  in Palvis and Ve
-0000dc60: 726e 6f6e 2032 3031 300a 0a20 2020 2050  rnon 2010..    P
-0000dc70: 4152 414d 4554 4552 533a 0a20 2020 202d  ARAMETERS:.    -
-0000dc80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000dc90: 2d2d 2d2d 2d0a 2020 2020 6363 5f61 7272  -----.    cc_arr
-0000dca0: 6179 3a20 6e75 6d70 792e 6e64 6172 7261  ay: numpy.ndarra
-0000dcb0: 7920 636f 6e74 6169 6e73 2074 6865 2032  y contains the 2
-0000dcc0: 4420 6372 6f73 7320 636f 7272 656c 6174  D cross correlat
-0000dcd0: 696f 6e20 6d61 7472 6978 0a20 2020 2065  ion matrix.    e
-0000dce0: 7073 696c 6f6e 3a20 7265 7369 6475 616c  psilon: residual
-0000dcf0: 2074 6872 6568 6f6c 6420 746f 2071 7569   threhold to qui
-0000dd00: 7420 7468 6520 6974 6572 6174 696f 6e0a  t the iteration.
-0000dd10: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
-0000dd20: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-0000dd30: 2d2d 2d2d 2d2d 2d0a 2020 2020 6e65 7773  -------.    news
-0000dd40: 7461 636b 3a20 6e75 6d70 7920 7665 6374  tack: numpy vect
-0000dd50: 6f72 2063 6f6e 7461 696e 7320 7468 6520  or contains the 
-0000dd60: 7374 6163 6b65 6420 6372 6f73 7320 636f  stacked cross co
-0000dd70: 7272 656c 6174 696f 6e0a 0a20 2020 2057  rrelation..    W
-0000dd80: 7269 7474 656e 2062 7920 4d61 7269 6e65  ritten by Marine
-0000dd90: 2044 656e 6f6c 6c65 0a20 2020 2022 2222   Denolle.    """
-0000dda0: 0a20 2020 2072 6573 203d 2039 6539 2020  .    res = 9e9  
-0000ddb0: 2320 7265 7369 6475 616c 730a 2020 2020  # residuals.    
-0000ddc0: 7720 3d20 6e70 2e6f 6e65 7328 6363 5f61  w = np.ones(cc_a
-0000ddd0: 7272 6179 2e73 6861 7065 5b30 5d29 0a20  rray.shape[0]). 
-0000dde0: 2020 206e 7374 6570 203d 2030 0a20 2020     nstep = 0.   
-0000ddf0: 206e 6577 7374 6163 6b20 3d20 6e70 2e6d   newstack = np.m
-0000de00: 6564 6961 6e28 6363 5f61 7272 6179 2c20  edian(cc_array, 
-0000de10: 6178 6973 3d30 290a 2020 2020 7768 696c  axis=0).    whil
-0000de20: 6520 7265 7320 3e20 6570 7369 6c6f 6e3a  e res > epsilon:
-0000de30: 0a20 2020 2020 2020 2073 7461 636b 203d  .        stack =
-0000de40: 206e 6577 7374 6163 6b0a 2020 2020 2020   newstack.      
-0000de50: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-0000de60: 2863 635f 6172 7261 792e 7368 6170 655b  (cc_array.shape[
-0000de70: 305d 293a 0a20 2020 2020 2020 2020 2020  0]):.           
-0000de80: 2063 7261 7020 3d20 6e70 2e6d 756c 7469   crap = np.multi
-0000de90: 706c 7928 7374 6163 6b2c 2063 635f 6172  ply(stack, cc_ar
-0000dea0: 7261 795b 692c 203a 5d2e 5429 0a20 2020  ray[i, :].T).   
-0000deb0: 2020 2020 2020 2020 2063 7261 705f 646f           crap_do
-0000dec0: 7420 3d20 6e70 2e73 756d 2863 7261 7029  t = np.sum(crap)
-0000ded0: 0a20 2020 2020 2020 2020 2020 2064 695f  .            di_
-0000dee0: 6e6f 726d 203d 206e 702e 6c69 6e61 6c67  norm = np.linalg
-0000def0: 2e6e 6f72 6d28 6363 5f61 7272 6179 5b69  .norm(cc_array[i
-0000df00: 2c20 3a5d 290a 2020 2020 2020 2020 2020  , :]).          
-0000df10: 2020 7269 203d 2063 635f 6172 7261 795b    ri = cc_array[
-0000df20: 692c 203a 5d20 2d20 6372 6170 5f64 6f74  i, :] - crap_dot
-0000df30: 202a 2073 7461 636b 0a20 2020 2020 2020   * stack.       
-0000df40: 2020 2020 2072 695f 6e6f 726d 203d 206e       ri_norm = n
-0000df50: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 7269  p.linalg.norm(ri
-0000df60: 290a 2020 2020 2020 2020 2020 2020 775b  ).            w[
-0000df70: 695d 203d 206e 702e 6162 7328 6372 6170  i] = np.abs(crap
-0000df80: 5f64 6f74 2920 2f20 6469 5f6e 6f72 6d20  _dot) / di_norm 
-0000df90: 2f20 7269 5f6e 6f72 6d20 2023 202f 6c65  / ri_norm  # /le
-0000dfa0: 6e28 6363 5f61 7272 6179 5b3a 2c31 5d29  n(cc_array[:,1])
-0000dfb0: 0a20 2020 2020 2020 2023 2070 7269 6e74  .        # print
-0000dfc0: 2877 290a 2020 2020 2020 2020 7720 3d20  (w).        w = 
-0000dfd0: 7720 2f20 6e70 2e73 756d 2877 290a 2020  w / np.sum(w).  
-0000dfe0: 2020 2020 2020 6e65 7773 7461 636b 203d        newstack =
-0000dff0: 206e 702e 7375 6d28 2877 202a 2063 635f   np.sum((w * cc_
-0000e000: 6172 7261 792e 5429 2e54 2c20 6178 6973  array.T).T, axis
-0000e010: 3d30 2920 2023 202f 6c65 6e28 6363 5f61  =0)  # /len(cc_a
-0000e020: 7272 6179 5b3a 2c31 5d29 0a20 2020 2020  rray[:,1]).     
-0000e030: 2020 2072 6573 203d 206e 702e 6c69 6e61     res = np.lina
-0000e040: 6c67 2e6e 6f72 6d28 6e65 7773 7461 636b  lg.norm(newstack
-0000e050: 202d 2073 7461 636b 2c20 6f72 643d 3129   - stack, ord=1)
-0000e060: 202f 206e 702e 6c69 6e61 6c67 2e6e 6f72   / np.linalg.nor
-0000e070: 6d28 6e65 7773 7461 636b 2920 2f20 6c65  m(newstack) / le
-0000e080: 6e28 6363 5f61 7272 6179 5b3a 2c20 315d  n(cc_array[:, 1]
-0000e090: 290a 2020 2020 2020 2020 6e73 7465 7020  ).        nstep 
-0000e0a0: 2b3d 2031 0a20 2020 2020 2020 2069 6620  += 1.        if 
-0000e0b0: 6e73 7465 7020 3e20 3130 3a0a 2020 2020  nstep > 10:.    
-0000e0c0: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-0000e0d0: 6577 7374 6163 6b2c 2077 2c20 6e73 7465  ewstack, w, nste
-0000e0e0: 700a 2020 2020 7265 7475 726e 206e 6577  p.    return new
-0000e0f0: 7374 6163 6b2c 2077 2c20 6e73 7465 700a  stack, w, nstep.
-0000e100: 0a0a 6465 6620 7365 6c65 6374 6976 655f  ..def selective_
-0000e110: 7374 6163 6b28 6363 5f61 7272 6179 2c20  stack(cc_array, 
-0000e120: 6570 7369 6c6f 6e29 3a0a 2020 2020 2222  epsilon):.    ""
-0000e130: 220a 2020 2020 7468 6973 2069 7320 6120  ".    this is a 
-0000e140: 7365 6c65 6374 6976 6520 7374 6163 6b69  selective stacki
-0000e150: 6e67 2061 6c67 6f72 6974 686d 2064 6576  ng algorithm dev
-0000e160: 656c 6f70 6564 2062 7920 4a61 7265 6420  eloped by Jared 
-0000e170: 4272 7961 6e2e 0a0a 2020 2020 5041 5241  Bryan...    PARA
-0000e180: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
-0000e190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000e1a0: 2d2d 0a20 2020 2063 635f 6172 7261 793a  --.    cc_array:
-0000e1b0: 206e 756d 7079 2e6e 6461 7272 6179 2063   numpy.ndarray c
-0000e1c0: 6f6e 7461 696e 7320 7468 6520 3244 2063  ontains the 2D c
-0000e1d0: 726f 7373 2063 6f72 7265 6c61 7469 6f6e  ross correlation
-0000e1e0: 206d 6174 7269 780a 2020 2020 6570 7369   matrix.    epsi
-0000e1f0: 6c6f 6e3a 2072 6573 6964 7561 6c20 7468  lon: residual th
-0000e200: 7265 686f 6c64 2074 6f20 7175 6974 2074  rehold to quit t
-0000e210: 6865 2069 7465 7261 7469 6f6e 0a20 2020  he iteration.   
-0000e220: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
-0000e230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000e240: 2d2d 2d2d 0a20 2020 206e 6577 7374 6163  ----.    newstac
-0000e250: 6b3a 206e 756d 7079 2076 6563 746f 7220  k: numpy vector 
-0000e260: 636f 6e74 6169 6e73 2074 6865 2073 7461  contains the sta
-0000e270: 636b 6564 2063 726f 7373 2063 6f72 7265  cked cross corre
-0000e280: 6c61 7469 6f6e 0a0a 2020 2020 5772 6974  lation..    Writ
-0000e290: 7465 6e20 6279 204d 6172 696e 6520 4465  ten by Marine De
-0000e2a0: 6e6f 6c6c 650a 2020 2020 2222 220a 2020  nolle.    """.  
-0000e2b0: 2020 6363 203d 206e 702e 6f6e 6573 2863    cc = np.ones(c
-0000e2c0: 635f 6172 7261 792e 7368 6170 655b 305d  c_array.shape[0]
-0000e2d0: 290a 2020 2020 6e65 7773 7461 636b 203d  ).    newstack =
-0000e2e0: 206e 702e 6d65 616e 2863 635f 6172 7261   np.mean(cc_arra
-0000e2f0: 792c 2061 7869 733d 3029 0a20 2020 2066  y, axis=0).    f
-0000e300: 6f72 2069 2069 6e20 7261 6e67 6528 6363  or i in range(cc
-0000e310: 5f61 7272 6179 2e73 6861 7065 5b30 5d29  _array.shape[0])
-0000e320: 3a0a 2020 2020 2020 2020 6363 5b69 5d20  :.        cc[i] 
-0000e330: 3d20 6e70 2e73 756d 286e 702e 6d75 6c74  = np.sum(np.mult
-0000e340: 6970 6c79 286e 6577 7374 6163 6b2c 2063  iply(newstack, c
-0000e350: 635f 6172 7261 795b 692c 203a 5d2e 5429  c_array[i, :].T)
-0000e360: 290a 2020 2020 696b 203d 206e 702e 7768  ).    ik = np.wh
-0000e370: 6572 6528 6363 203e 3d20 6570 7369 6c6f  ere(cc >= epsilo
-0000e380: 6e29 5b30 5d0a 2020 2020 6e65 7773 7461  n)[0].    newsta
-0000e390: 636b 203d 206e 702e 6d65 616e 2863 635f  ck = np.mean(cc_
-0000e3a0: 6172 7261 795b 696b 2c20 3a5d 2c20 6178  array[ik, :], ax
-0000e3b0: 6973 3d30 290a 0a20 2020 2072 6574 7572  is=0)..    retur
-0000e3c0: 6e20 6e65 7773 7461 636b 2c20 6363 0a0a  n newstack, cc..
-0000e3d0: 0a64 6566 2077 6869 7465 6e5f 3144 2874  .def whiten_1D(t
-0000e3e0: 696d 6573 6572 6965 732c 2066 6674 5f70  imeseries, fft_p
-0000e3f0: 6172 612c 206e 5f74 6170 6572 293a 0a20  ara, n_taper):. 
-0000e400: 2020 2022 2222 0a20 2020 2054 6869 7320     """.    This 
-0000e410: 6675 6e63 7469 6f6e 2074 616b 6573 2061  function takes a
-0000e420: 2031 2d64 696d 656e 7369 6f6e 616c 2074   1-dimensional t
-0000e430: 696d 6573 6572 6965 7320 6172 7261 792c  imeseries array,
-0000e440: 2074 7261 6e73 666f 726d 7320 746f 2066   transforms to f
-0000e450: 7265 7175 656e 6379 2064 6f6d 6169 6e20  requency domain 
-0000e460: 7573 696e 6720 6666 742c 0a20 2020 2077  using fft,.    w
-0000e470: 6869 7465 6e73 2074 6865 2061 6d70 6c69  hitens the ampli
-0000e480: 7475 6465 206f 6620 7468 6520 7370 6563  tude of the spec
-0000e490: 7472 756d 2069 6e20 6672 6571 7565 6e63  trum in frequenc
-0000e4a0: 7920 646f 6d61 696e 2062 6574 7765 656e  y domain between
-0000e4b0: 202a 6672 6571 6d69 6e2a 2061 6e64 202a   *freqmin* and *
-0000e4c0: 6672 6571 6d61 782a 0a20 2020 2061 6e64  freqmax*.    and
-0000e4d0: 2072 6574 7572 6e73 2074 6865 2077 6869   returns the whi
-0000e4e0: 7465 6e65 6420 6666 742e 0a20 2020 2050  tened fft..    P
-0000e4f0: 4152 414d 4554 4552 533a 0a20 2020 202d  ARAMETERS:.    -
-0000e500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000e510: 2d2d 2d2d 2d0a 2020 2020 6461 7461 3a20  -----.    data: 
-0000e520: 6e75 6d70 792e 6e64 6172 7261 7920 636f  numpy.ndarray co
-0000e530: 6e74 6169 6e73 2074 6865 2031 4420 7469  ntains the 1D ti
-0000e540: 6d65 2073 6572 6965 7320 746f 2077 6869  me series to whi
-0000e550: 7465 6e0a 2020 2020 6666 745f 7061 7261  ten.    fft_para
-0000e560: 3a20 6469 6374 2063 6f6e 7461 696e 696e  : dict containin
-0000e570: 6720 616c 6c20 6666 745f 6363 2070 6172  g all fft_cc par
-0000e580: 616d 6574 6572 7320 7375 6368 2061 730a  ameters such as.
-0000e590: 2020 2020 2020 2020 6474 3a20 5468 6520          dt: The 
-0000e5a0: 7361 6d70 6c69 6e67 2073 7061 6365 206f  sampling space o
-0000e5b0: 6620 7468 6520 6064 6174 6160 0a20 2020  f the `data`.   
-0000e5c0: 2020 2020 2066 7265 716d 696e 3a20 5468       freqmin: Th
-0000e5d0: 6520 6c6f 7765 7220 6672 6571 7565 6e63  e lower frequenc
-0000e5e0: 7920 626f 756e 640a 2020 2020 2020 2020  y bound.        
-0000e5f0: 6672 6571 6d61 783a 2054 6865 2075 7070  freqmax: The upp
-0000e600: 6572 2066 7265 7175 656e 6379 2062 6f75  er frequency bou
-0000e610: 6e64 0a20 2020 2020 2020 2073 6d6f 6f74  nd.        smoot
-0000e620: 685f 4e3a 2069 6e74 6567 6572 2c20 6974  h_N: integer, it
-0000e630: 2064 6566 696e 6573 2074 6865 2068 616c   defines the hal
-0000e640: 6620 7769 6e64 6f77 206c 656e 6774 6820  f window length 
-0000e650: 746f 2073 6d6f 6f74 680a 2020 2020 2020  to smooth.      
-0000e660: 2020 6e5f 7461 7065 722c 206f 7074 696f    n_taper, optio
-0000e670: 6e61 6c3a 2069 6e74 6567 6572 2c20 6465  nal: integer, de
-0000e680: 6669 6e65 2074 6865 2077 6964 7468 206f  fine the width o
-0000e690: 6620 7468 6520 7461 7065 7220 696e 2073  f the taper in s
-0000e6a0: 616d 706c 6573 0a20 2020 2052 4554 5552  amples.    RETUR
-0000e6b0: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
-0000e6c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-0000e6d0: 2020 2046 4654 5261 7753 6967 6e3a 206e     FFTRawSign: n
-0000e6e0: 756d 7079 2e6e 6461 7272 6179 2063 6f6e  umpy.ndarray con
-0000e6f0: 7461 696e 7320 7468 6520 4646 5420 6f66  tains the FFT of
-0000e700: 2074 6865 2077 6869 7465 6e65 6420 696e   the whitened in
-0000e710: 7075 7420 7472 6163 6520 6265 7477 6565  put trace betwee
-0000e720: 6e20 7468 6520 6672 6571 7565 6e63 7920  n the frequency 
-0000e730: 626f 756e 6473 0a20 2020 2022 2222 0a20  bounds.    """. 
-0000e740: 2020 2023 206c 6f61 6420 7061 7261 6d65     # load parame
-0000e750: 7465 7273 0a20 2020 2064 656c 7461 203d  ters.    delta =
-0000e760: 2066 6674 5f70 6172 615b 2264 7422 5d0a   fft_para["dt"].
-0000e770: 2020 2020 6672 6571 6d69 6e20 3d20 6666      freqmin = ff
-0000e780: 745f 7061 7261 5b22 6672 6571 6d69 6e22  t_para["freqmin"
-0000e790: 5d0a 2020 2020 6672 6571 6d61 7820 3d20  ].    freqmax = 
-0000e7a0: 6666 745f 7061 7261 5b22 6672 6571 6d61  fft_para["freqma
-0000e7b0: 7822 5d0a 2020 2020 736d 6f6f 7468 5f4e  x"].    smooth_N
-0000e7c0: 203d 2066 6674 5f70 6172 615b 2273 6d6f   = fft_para["smo
-0000e7d0: 6f74 685f 4e22 5d0a 0a20 2020 206e 6666  oth_N"]..    nff
-0000e7e0: 7420 3d20 6e65 7874 5f66 6173 745f 6c65  t = next_fast_le
-0000e7f0: 6e28 6c65 6e28 7469 6d65 7365 7269 6573  n(len(timeseries
-0000e800: 2929 0a20 2020 2073 7065 6320 3d20 6e70  )).    spec = np
-0000e810: 2e66 6674 2e66 6674 2874 696d 6573 6572  .fft.fft(timeser
-0000e820: 6965 732c 206e 6666 7429 0a20 2020 2066  ies, nfft).    f
-0000e830: 7265 7120 3d20 6e70 2e66 6674 2e66 6674  req = np.fft.fft
-0000e840: 6672 6571 286e 6666 742c 2064 3d64 656c  freq(nfft, d=del
-0000e850: 7461 290a 0a20 2020 2069 7830 203d 206e  ta)..    ix0 = n
-0000e860: 702e 6172 676d 696e 286e 702e 6162 7328  p.argmin(np.abs(
-0000e870: 6672 6571 202d 2066 7265 716d 696e 2929  freq - freqmin))
-0000e880: 0a20 2020 2069 7831 203d 206e 702e 6172  .    ix1 = np.ar
-0000e890: 676d 696e 286e 702e 6162 7328 6672 6571  gmin(np.abs(freq
-0000e8a0: 202d 2066 7265 716d 6178 2929 0a0a 2020   - freqmax))..  
-0000e8b0: 2020 6966 2069 7831 202b 206e 5f74 6170    if ix1 + n_tap
-0000e8c0: 6572 203e 206e 6666 743a 0a20 2020 2020  er > nfft:.     
-0000e8d0: 2020 2069 7831 3120 3d20 6e66 6674 0a20     ix11 = nfft. 
-0000e8e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000e8f0: 2069 7831 3120 3d20 6978 3120 2b20 6e5f   ix11 = ix1 + n_
-0000e900: 7461 7065 720a 0a20 2020 2069 6620 6978  taper..    if ix
-0000e910: 3020 2d20 6e5f 7461 7065 7220 3c20 303a  0 - n_taper < 0:
-0000e920: 0a20 2020 2020 2020 2069 7830 3020 3d20  .        ix00 = 
-0000e930: 300a 2020 2020 656c 7365 3a0a 2020 2020  0.    else:.    
-0000e940: 2020 2020 6978 3030 203d 2069 7830 202d      ix00 = ix0 -
-0000e950: 206e 5f74 6170 6572 0a0a 2020 2020 7370   n_taper..    sp
-0000e960: 6563 5f6f 7574 203d 2073 7065 632e 636f  ec_out = spec.co
-0000e970: 7079 2829 0a20 2020 2073 7065 635f 6f75  py().    spec_ou
-0000e980: 745b 303a 6978 3030 5d20 3d20 302e 3020  t[0:ix00] = 0.0 
-0000e990: 2b20 302e 306a 0a20 2020 2073 7065 635f  + 0.0j.    spec_
-0000e9a0: 6f75 745b 6978 3131 3a5d 203d 2030 2e30  out[ix11:] = 0.0
-0000e9b0: 202b 2030 2e30 6a0a 0a20 2020 2069 6620   + 0.0j..    if 
-0000e9c0: 736d 6f6f 7468 5f4e 203c 3d20 313a 0a20  smooth_N <= 1:. 
-0000e9d0: 2020 2020 2020 2073 7065 635f 6f75 745b         spec_out[
-0000e9e0: 6978 3030 3a69 7831 315d 203d 206e 702e  ix00:ix11] = np.
-0000e9f0: 6578 7028 312e 306a 202a 206e 702e 616e  exp(1.0j * np.an
-0000ea00: 676c 6528 7370 6563 5f6f 7574 5b69 7830  gle(spec_out[ix0
-0000ea10: 303a 6978 3131 5d29 290a 2020 2020 656c  0:ix11])).    el
-0000ea20: 7365 3a0a 2020 2020 2020 2020 7370 6563  se:.        spec
-0000ea30: 5f6f 7574 5b69 7830 303a 6978 3131 5d20  _out[ix00:ix11] 
-0000ea40: 2f3d 206d 6f76 696e 675f 6176 6528 6e70  /= moving_ave(np
-0000ea50: 2e61 6273 2873 7065 635f 6f75 745b 6978  .abs(spec_out[ix
-0000ea60: 3030 3a69 7831 315d 292c 2073 6d6f 6f74  00:ix11]), smoot
-0000ea70: 685f 4e29 0a0a 2020 2020 7820 3d20 6e70  h_N)..    x = np
-0000ea80: 2e6c 696e 7370 6163 6528 6e70 2e70 6920  .linspace(np.pi 
-0000ea90: 2f20 322e 302c 206e 702e 7069 2c20 6978  / 2.0, np.pi, ix
-0000eaa0: 3020 2d20 6978 3030 290a 2020 2020 7370  0 - ix00).    sp
-0000eab0: 6563 5f6f 7574 5b69 7830 303a 6978 305d  ec_out[ix00:ix0]
-0000eac0: 202a 3d20 6e70 2e63 6f73 2878 2920 2a2a   *= np.cos(x) **
-0000ead0: 2032 0a0a 2020 2020 7820 3d20 6e70 2e6c   2..    x = np.l
-0000eae0: 696e 7370 6163 6528 302e 302c 206e 702e  inspace(0.0, np.
-0000eaf0: 7069 202f 2032 2e30 2c20 6978 3131 202d  pi / 2.0, ix11 -
-0000eb00: 2069 7831 290a 2020 2020 7370 6563 5f6f   ix1).    spec_o
-0000eb10: 7574 5b69 7831 3a69 7831 315d 202a 3d20  ut[ix1:ix11] *= 
-0000eb20: 6e70 2e63 6f73 2878 2920 2a2a 2032 0a0a  np.cos(x) ** 2..
-0000eb30: 2020 2020 7265 7475 726e 2073 7065 635f      return spec_
-0000eb40: 6f75 740a 0a0a 6465 6620 7768 6974 656e  out...def whiten
-0000eb50: 5f32 4428 7469 6d65 7365 7269 6573 2c20  _2D(timeseries, 
-0000eb60: 6666 745f 7061 7261 2c20 6e5f 7461 7065  fft_para, n_tape
-0000eb70: 7229 3a0a 2020 2020 2222 220a 2020 2020  r):.    """.    
-0000eb80: 5468 6973 2066 756e 6374 696f 6e20 7461  This function ta
-0000eb90: 6b65 7320 6120 322d 6469 6d65 6e73 696f  kes a 2-dimensio
-0000eba0: 6e61 6c20 7469 6d65 7365 7269 6573 2061  nal timeseries a
-0000ebb0: 7272 6179 2c20 7472 616e 7366 6f72 6d73  rray, transforms
-0000ebc0: 2074 6f20 6672 6571 7565 6e63 7920 646f   to frequency do
-0000ebd0: 6d61 696e 2075 7369 6e67 2066 6674 2c0a  main using fft,.
-0000ebe0: 2020 2020 7768 6974 656e 7320 7468 6520      whitens the 
-0000ebf0: 616d 706c 6974 7564 6520 6f66 2074 6865  amplitude of the
-0000ec00: 2073 7065 6374 7275 6d20 696e 2066 7265   spectrum in fre
-0000ec10: 7175 656e 6379 2064 6f6d 6169 6e20 6265  quency domain be
-0000ec20: 7477 6565 6e20 2a66 7265 716d 696e 2a20  tween *freqmin* 
-0000ec30: 616e 6420 2a66 7265 716d 6178 2a0a 2020  and *freqmax*.  
-0000ec40: 2020 616e 6420 7265 7475 726e 7320 7468    and returns th
-0000ec50: 6520 7768 6974 656e 6564 2066 6674 2e0a  e whitened fft..
-0000ec60: 2020 2020 5041 5241 4d45 5445 5253 3a0a      PARAMETERS:.
-0000ec70: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-0000ec80: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064  ----------.    d
-0000ec90: 6174 613a 206e 756d 7079 2e6e 6461 7272  ata: numpy.ndarr
-0000eca0: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
-0000ecb0: 3144 2074 696d 6520 7365 7269 6573 2074  1D time series t
-0000ecc0: 6f20 7768 6974 656e 0a20 2020 2066 6674  o whiten.    fft
-0000ecd0: 5f70 6172 613a 2064 6963 7420 636f 6e74  _para: dict cont
-0000ece0: 6169 6e69 6e67 2061 6c6c 2066 6674 5f63  aining all fft_c
-0000ecf0: 6320 7061 7261 6d65 7465 7273 2073 7563  c parameters suc
-0000ed00: 6820 6173 0a20 2020 2020 2020 2064 743a  h as.        dt:
-0000ed10: 2054 6865 2073 616d 706c 696e 6720 7370   The sampling sp
-0000ed20: 6163 6520 6f66 2074 6865 2060 6461 7461  ace of the `data
-0000ed30: 600a 2020 2020 2020 2020 6672 6571 6d69  `.        freqmi
-0000ed40: 6e3a 2054 6865 206c 6f77 6572 2066 7265  n: The lower fre
-0000ed50: 7175 656e 6379 2062 6f75 6e64 0a20 2020  quency bound.   
-0000ed60: 2020 2020 2066 7265 716d 6178 3a20 5468       freqmax: Th
-0000ed70: 6520 7570 7065 7220 6672 6571 7565 6e63  e upper frequenc
-0000ed80: 7920 626f 756e 640a 2020 2020 2020 2020  y bound.        
-0000ed90: 736d 6f6f 7468 5f4e 3a20 696e 7465 6765  smooth_N: intege
-0000eda0: 722c 2069 7420 6465 6669 6e65 7320 7468  r, it defines th
-0000edb0: 6520 6861 6c66 2077 696e 646f 7720 6c65  e half window le
-0000edc0: 6e67 7468 2074 6f20 736d 6f6f 7468 0a20  ngth to smooth. 
-0000edd0: 2020 2020 2020 206e 5f74 6170 6572 2c20         n_taper, 
-0000ede0: 6f70 7469 6f6e 616c 3a20 696e 7465 6765  optional: intege
-0000edf0: 722c 2064 6566 696e 6520 7468 6520 7769  r, define the wi
-0000ee00: 6474 6820 6f66 2074 6865 2074 6170 6572  dth of the taper
-0000ee10: 2069 6e20 7361 6d70 6c65 730a 2020 2020   in samples.    
-0000ee20: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
-0000ee30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000ee40: 2d2d 2d0a 2020 2020 4646 5452 6177 5369  ---.    FFTRawSi
-0000ee50: 676e 3a20 6e75 6d70 792e 6e64 6172 7261  gn: numpy.ndarra
-0000ee60: 7920 636f 6e74 6169 6e73 2074 6865 2046  y contains the F
-0000ee70: 4654 206f 6620 7468 6520 7768 6974 656e  FT of the whiten
-0000ee80: 6564 2069 6e70 7574 2074 7261 6365 2062  ed input trace b
-0000ee90: 6574 7765 656e 2074 6865 2066 7265 7175  etween the frequ
-0000eea0: 656e 6379 2062 6f75 6e64 730a 2020 2020  ency bounds.    
-0000eeb0: 2222 220a 2020 2020 2320 6c6f 6164 2070  """.    # load p
-0000eec0: 6172 616d 6574 6572 730a 2020 2020 6465  arameters.    de
-0000eed0: 6c74 6120 3d20 6666 745f 7061 7261 5b22  lta = fft_para["
-0000eee0: 6474 225d 0a20 2020 2066 7265 716d 696e  dt"].    freqmin
-0000eef0: 203d 2066 6674 5f70 6172 615b 2266 7265   = fft_para["fre
-0000ef00: 716d 696e 225d 0a20 2020 2066 7265 716d  qmin"].    freqm
-0000ef10: 6178 203d 2066 6674 5f70 6172 615b 2266  ax = fft_para["f
-0000ef20: 7265 716d 6178 225d 0a20 2020 2073 6d6f  reqmax"].    smo
-0000ef30: 6f74 685f 4e20 3d20 6666 745f 7061 7261  oth_N = fft_para
-0000ef40: 5b22 736d 6f6f 7468 5f4e 225d 0a0a 2020  ["smooth_N"]..  
-0000ef50: 2020 6e66 6674 203d 206e 6578 745f 6661    nfft = next_fa
-0000ef60: 7374 5f6c 656e 2874 696d 6573 6572 6965  st_len(timeserie
-0000ef70: 732e 7368 6170 655b 315d 290a 2020 2020  s.shape[1]).    
-0000ef80: 7370 6563 203d 206e 702e 6666 742e 6666  spec = np.fft.ff
-0000ef90: 746e 2874 696d 6573 6572 6965 732c 2073  tn(timeseries, s
-0000efa0: 3d5b 6e66 6674 5d29 0a20 2020 2066 7265  =[nfft]).    fre
-0000efb0: 7120 3d20 6e70 2e66 6674 2e66 6674 6672  q = np.fft.fftfr
-0000efc0: 6571 286e 6666 742c 2064 3d64 656c 7461  eq(nfft, d=delta
-0000efd0: 290a 0a20 2020 2069 7830 203d 206e 702e  )..    ix0 = np.
-0000efe0: 6172 676d 696e 286e 702e 6162 7328 6672  argmin(np.abs(fr
-0000eff0: 6571 202d 2066 7265 716d 696e 2929 0a20  eq - freqmin)). 
-0000f000: 2020 2069 7831 203d 206e 702e 6172 676d     ix1 = np.argm
-0000f010: 696e 286e 702e 6162 7328 6672 6571 202d  in(np.abs(freq -
-0000f020: 2066 7265 716d 6178 2929 0a0a 2020 2020   freqmax))..    
-0000f030: 6966 2069 7831 202b 206e 5f74 6170 6572  if ix1 + n_taper
-0000f040: 203e 206e 6666 743a 0a20 2020 2020 2020   > nfft:.       
-0000f050: 2069 7831 3120 3d20 6e66 6674 0a20 2020   ix11 = nfft.   
-0000f060: 2065 6c73 653a 0a20 2020 2020 2020 2069   else:.        i
-0000f070: 7831 3120 3d20 6978 3120 2b20 6e5f 7461  x11 = ix1 + n_ta
-0000f080: 7065 720a 0a20 2020 2069 6620 6978 3020  per..    if ix0 
-0000f090: 2d20 6e5f 7461 7065 7220 3c20 303a 0a20  - n_taper < 0:. 
-0000f0a0: 2020 2020 2020 2069 7830 3020 3d20 300a         ix00 = 0.
-0000f0b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000f0c0: 2020 6978 3030 203d 2069 7830 202d 206e    ix00 = ix0 - n
-0000f0d0: 5f74 6170 6572 0a0a 2020 2020 7370 6563  _taper..    spec
-0000f0e0: 5f6f 7574 203d 2073 7065 632e 636f 7079  _out = spec.copy
-0000f0f0: 2829 2020 2320 6d61 7920 6265 2069 6e63  ()  # may be inc
-0000f100: 6f6e 7665 6e69 656e 7420 6475 6520 746f  onvenient due to
-0000f110: 2068 6967 6865 7220 6d65 6d6f 7279 2075   higher memory u
-0000f120: 7361 6765 0a20 2020 2073 7065 635f 6f75  sage.    spec_ou
-0000f130: 745b 3a2c 2030 3a69 7830 305d 203d 2030  t[:, 0:ix00] = 0
-0000f140: 2e30 202b 2030 2e30 6a0a 2020 2020 7370  .0 + 0.0j.    sp
-0000f150: 6563 5f6f 7574 5b3a 2c20 6978 3131 3a5d  ec_out[:, ix11:]
-0000f160: 203d 2030 2e30 202b 2030 2e30 6a0a 0a20   = 0.0 + 0.0j.. 
-0000f170: 2020 2069 6620 736d 6f6f 7468 5f4e 203c     if smooth_N <
-0000f180: 3d20 313a 0a20 2020 2020 2020 2073 7065  = 1:.        spe
-0000f190: 635f 6f75 745b 3a2c 2069 7830 303a 6978  c_out[:, ix00:ix
-0000f1a0: 3131 5d20 3d20 6e70 2e65 7870 2831 2e30  11] = np.exp(1.0
-0000f1b0: 6a20 2a20 6e70 2e61 6e67 6c65 2873 7065  j * np.angle(spe
-0000f1c0: 635f 6f75 745b 3a2c 2069 7830 303a 6978  c_out[:, ix00:ix
-0000f1d0: 3131 5d29 290a 2020 2020 656c 7365 3a0a  11])).    else:.
-0000f1e0: 2020 2020 2020 2020 7370 6563 5f6f 7574          spec_out
-0000f1f0: 5b3a 2c20 6978 3030 3a69 7831 315d 202f  [:, ix00:ix11] /
-0000f200: 3d20 6d6f 7669 6e67 5f61 7665 5f32 4428  = moving_ave_2D(
-0000f210: 6e70 2e61 6273 2873 7065 635f 6f75 745b  np.abs(spec_out[
-0000f220: 3a2c 2069 7830 303a 6978 3131 5d29 2c20  :, ix00:ix11]), 
-0000f230: 736d 6f6f 7468 5f4e 290a 0a20 2020 2078  smooth_N)..    x
-0000f240: 203d 206e 702e 6c69 6e73 7061 6365 286e   = np.linspace(n
-0000f250: 702e 7069 202f 2032 2e30 2c20 6e70 2e70  p.pi / 2.0, np.p
-0000f260: 692c 2069 7830 202d 2069 7830 3029 0a20  i, ix0 - ix00). 
-0000f270: 2020 2073 7065 635f 6f75 745b 3a2c 2069     spec_out[:, i
-0000f280: 7830 303a 6978 305d 202a 3d20 6e70 2e63  x00:ix0] *= np.c
-0000f290: 6f73 2878 2920 2a2a 2032 0a0a 2020 2020  os(x) ** 2..    
-0000f2a0: 7820 3d20 6e70 2e6c 696e 7370 6163 6528  x = np.linspace(
-0000f2b0: 302e 302c 206e 702e 7069 202f 2032 2e30  0.0, np.pi / 2.0
-0000f2c0: 2c20 6978 3131 202d 2069 7831 290a 2020  , ix11 - ix1).  
-0000f2d0: 2020 7370 6563 5f6f 7574 5b3a 2c20 6978    spec_out[:, ix
-0000f2e0: 313a 6978 3131 5d20 2a3d 206e 702e 636f  1:ix11] *= np.co
-0000f2f0: 7328 7829 202a 2a20 320a 0a20 2020 2072  s(x) ** 2..    r
-0000f300: 6574 7572 6e20 7370 6563 5f6f 7574 0a0a  eturn spec_out..
-0000f310: 0a64 6566 2077 6869 7465 6e28 6461 7461  .def whiten(data
-0000f320: 2c20 6666 745f 7061 7261 2c20 6e5f 7461  , fft_para, n_ta
-0000f330: 7065 723d 3130 3029 3a0a 2020 2020 2222  per=100):.    ""
-0000f340: 220a 2020 2020 5468 6973 2066 756e 6374  ".    This funct
-0000f350: 696f 6e20 7461 6b65 7320 6120 7469 6d65  ion takes a time
-0000f360: 7365 7269 6573 2061 7272 6179 2c20 7472  series array, tr
-0000f370: 616e 7366 6f72 6d73 2074 6f20 6672 6571  ansforms to freq
-0000f380: 7565 6e63 7920 646f 6d61 696e 2075 7369  uency domain usi
-0000f390: 6e67 2066 6674 2c0a 2020 2020 7768 6974  ng fft,.    whit
-0000f3a0: 656e 7320 7468 6520 616d 706c 6974 7564  ens the amplitud
-0000f3b0: 6520 6f66 2074 6865 2073 7065 6374 7275  e of the spectru
-0000f3c0: 6d20 696e 2066 7265 7175 656e 6379 2064  m in frequency d
-0000f3d0: 6f6d 6169 6e20 6265 7477 6565 6e20 2a66  omain between *f
-0000f3e0: 7265 716d 696e 2a20 616e 6420 2a66 7265  reqmin* and *fre
-0000f3f0: 716d 6178 2a0a 2020 2020 616e 6420 7265  qmax*.    and re
-0000f400: 7475 726e 7320 7468 6520 7768 6974 656e  turns the whiten
-0000f410: 6564 2066 6674 2e0a 2020 2020 5041 5241  ed fft..    PARA
-0000f420: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
-0000f430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000f440: 2d2d 0a20 2020 2064 6174 613a 206e 756d  --.    data: num
-0000f450: 7079 2e6e 6461 7272 6179 2063 6f6e 7461  py.ndarray conta
-0000f460: 696e 7320 7468 6520 3144 2074 696d 6520  ins the 1D time 
-0000f470: 7365 7269 6573 2074 6f20 7768 6974 656e  series to whiten
-0000f480: 0a20 2020 2066 6674 5f70 6172 613a 2064  .    fft_para: d
-0000f490: 6963 7420 636f 6e74 6169 6e69 6e67 2061  ict containing a
-0000f4a0: 6c6c 2066 6674 5f63 6320 7061 7261 6d65  ll fft_cc parame
-0000f4b0: 7465 7273 2073 7563 6820 6173 0a20 2020  ters such as.   
-0000f4c0: 2020 2020 2064 743a 2054 6865 2073 616d       dt: The sam
-0000f4d0: 706c 696e 6720 7370 6163 6520 6f66 2074  pling space of t
-0000f4e0: 6865 2060 6461 7461 600a 2020 2020 2020  he `data`.      
-0000f4f0: 2020 6672 6571 6d69 6e3a 2054 6865 206c    freqmin: The l
-0000f500: 6f77 6572 2066 7265 7175 656e 6379 2062  ower frequency b
-0000f510: 6f75 6e64 0a20 2020 2020 2020 2066 7265  ound.        fre
-0000f520: 716d 6178 3a20 5468 6520 7570 7065 7220  qmax: The upper 
-0000f530: 6672 6571 7565 6e63 7920 626f 756e 640a  frequency bound.
-0000f540: 2020 2020 2020 2020 736d 6f6f 7468 5f4e          smooth_N
-0000f550: 3a20 696e 7465 6765 722c 2069 7420 6465  : integer, it de
-0000f560: 6669 6e65 7320 7468 6520 6861 6c66 2077  fines the half w
-0000f570: 696e 646f 7720 6c65 6e67 7468 2074 6f20  indow length to 
-0000f580: 736d 6f6f 7468 0a20 2020 2020 2020 2066  smooth.        f
-0000f590: 7265 715f 6e6f 726d 3a20 7768 6974 656e  req_norm: whiten
-0000f5a0: 696e 6720 6d65 7468 6f64 2062 6574 7765  ing method betwe
-0000f5b0: 656e 2027 6f6e 652d 6269 7427 2061 6e64  en 'one-bit' and
-0000f5c0: 2027 524d 4127 0a20 2020 2052 4554 5552   'RMA'.    RETUR
-0000f5d0: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
-0000f5e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-0000f5f0: 2020 2046 4654 5261 7753 6967 6e3a 206e     FFTRawSign: n
-0000f600: 756d 7079 2e6e 6461 7272 6179 2063 6f6e  umpy.ndarray con
-0000f610: 7461 696e 7320 7468 6520 4646 5420 6f66  tains the FFT of
-0000f620: 2074 6865 2077 6869 7465 6e65 6420 696e   the whitened in
-0000f630: 7075 7420 7472 6163 6520 6265 7477 6565  put trace betwee
-0000f640: 6e20 7468 6520 6672 6571 7565 6e63 7920  n the frequency 
-0000f650: 626f 756e 6473 0a20 2020 2022 2222 0a0a  bounds.    """..
-0000f660: 2020 2020 2320 5370 6565 6420 7570 2046      # Speed up F
-0000f670: 4654 2062 7920 7061 6464 696e 6720 746f  FT by padding to
-0000f680: 206f 7074 696d 616c 2073 697a 6520 666f   optimal size fo
-0000f690: 7220 4646 5450 4143 4b0a 2020 2020 6966  r FFTPACK.    if
-0000f6a0: 2064 6174 612e 6e64 696d 203d 3d20 313a   data.ndim == 1:
-0000f6b0: 0a20 2020 2020 2020 2046 4654 5261 7753  .        FFTRawS
-0000f6c0: 6967 6e20 3d20 7768 6974 656e 5f31 4428  ign = whiten_1D(
-0000f6d0: 6461 7461 2c20 6666 745f 7061 7261 2c20  data, fft_para, 
-0000f6e0: 6e5f 7461 7065 7229 0a20 2020 2020 2020  n_taper).       
-0000f6f0: 2023 2041 5252 5f4f 5554 3a20 4f6e 6c79   # ARR_OUT: Only
-0000f700: 2066 6f72 2063 6f6e 7369 7374 656e 6379   for consistency
-0000f710: 2077 6974 6820 6e6f 6973 6570 7920 6170   with noisepy ap
-0000f720: 7072 6f61 6368 206f 6620 686f 6c64 696e  proach of holdin
-0000f730: 6720 7468 6520 6675 6c6c 0a20 2020 2020  g the full.     
-0000f740: 2020 2023 2073 7065 6374 7275 6d20 286e     # spectrum (n
-0000f750: 6f74 206a 7573 7420 3020 616e 6420 706f  ot just 0 and po
-0000f760: 7369 7469 7665 2066 7265 712e 2070 6172  sitive freq. par
-0000f770: 7429 0a20 2020 2020 2020 2061 7272 5f6f  t).        arr_o
-0000f780: 7574 203d 206e 702e 7a65 726f 7328 2846  ut = np.zeros((F
-0000f790: 4654 5261 7753 6967 6e2e 7368 6170 655b  FTRawSign.shape[
-0000f7a0: 305d 202d 2031 2920 2a20 3220 2b20 312c  0] - 1) * 2 + 1,
-0000f7b0: 2064 7479 7065 3d63 6f6d 706c 6578 290a   dtype=complex).
-0000f7c0: 2020 2020 2020 2020 6172 725f 6f75 745b          arr_out[
-0000f7d0: 3020 3a20 4646 5452 6177 5369 676e 2e73  0 : FFTRawSign.s
-0000f7e0: 6861 7065 5b30 5d5d 203d 2046 4654 5261  hape[0]] = FFTRa
-0000f7f0: 7753 6967 6e0a 2020 2020 2020 2020 6172  wSign.        ar
-0000f800: 725f 6f75 745b 4646 5452 6177 5369 676e  r_out[FFTRawSign
-0000f810: 2e73 6861 7065 5b30 5d20 3a5d 203d 2046  .shape[0] :] = F
-0000f820: 4654 5261 7753 6967 6e5b 313a 5d2e 636f  FTRawSign[1:].co
-0000f830: 6e6a 7567 6174 6528 295b 3a3a 2d31 5d0a  njugate()[::-1].
-0000f840: 0a20 2020 2065 6c69 6620 6461 7461 2e6e  .    elif data.n
-0000f850: 6469 6d20 3d3d 2032 3a0a 2020 2020 2020  dim == 2:.      
-0000f860: 2020 4646 5452 6177 5369 676e 203d 2077    FFTRawSign = w
-0000f870: 6869 7465 6e5f 3244 2864 6174 612c 2066  hiten_2D(data, f
-0000f880: 6674 5f70 6172 612c 206e 5f74 6170 6572  ft_para, n_taper
-0000f890: 290a 2020 2020 2020 2020 6172 725f 6f75  ).        arr_ou
-0000f8a0: 7420 3d20 6e70 2e7a 6572 6f73 2828 4646  t = np.zeros((FF
-0000f8b0: 5452 6177 5369 676e 2e73 6861 7065 5b30  TRawSign.shape[0
-0000f8c0: 5d2c 2028 4646 5452 6177 5369 676e 2e73  ], (FFTRawSign.s
-0000f8d0: 6861 7065 5b31 5d20 2d20 3129 202a 2032  hape[1] - 1) * 2
-0000f8e0: 202b 2031 292c 2064 7479 7065 3d63 6f6d   + 1), dtype=com
-0000f8f0: 706c 6578 290a 2020 2020 2020 2020 6172  plex).        ar
-0000f900: 725f 6f75 745b 3a2c 2046 4654 5261 7753  r_out[:, FFTRawS
-0000f910: 6967 6e2e 7368 6170 655b 315d 203a 5d20  ign.shape[1] :] 
-0000f920: 3d20 4646 5452 6177 5369 676e 5b3a 2c20  = FFTRawSign[:, 
-0000f930: 313a 5d2e 636f 6e6a 7567 6174 6528 295b  1:].conjugate()[
-0000f940: 3a3a 2d31 5d0a 2020 2020 7265 7475 726e  ::-1].    return
-0000f950: 2046 4654 5261 7753 6967 6e0a 0a0a 6465   FFTRawSign...de
-0000f960: 6620 6164 6170 7469 7665 5f66 696c 7465  f adaptive_filte
-0000f970: 7228 6172 722c 2067 293a 0a20 2020 2022  r(arr, g):.    "
-0000f980: 2222 0a20 2020 2074 6865 2061 6461 7074  "".    the adapt
-0000f990: 6976 6520 636f 7661 7269 616e 6365 2066  ive covariance f
-0000f9a0: 696c 7465 7220 746f 2065 6e68 616e 6365  ilter to enhance
-0000f9b0: 2063 6f68 6572 656e 7420 7369 676e 616c   coherent signal
-0000f9c0: 732e 2046 656c 6c6f 7773 2074 6865 206d  s. Fellows the m
-0000f9d0: 6574 686f 6420 6f66 0a20 2020 204e 616b  ethod of.    Nak
-0000f9e0: 6174 6120 6574 2061 6c2e 2c20 3230 3135  ata et al., 2015
-0000f9f0: 2028 4170 7065 6e64 6978 2042 290a 0a20   (Appendix B).. 
-0000fa00: 2020 2074 6865 2066 696c 7465 7265 6420     the filtered 
-0000fa10: 7369 676e 616c 205b 7831 5d20 6973 2067  signal [x1] is g
-0000fa20: 6976 656e 2062 7920 7831 203d 2069 6666  iven by x1 = iff
-0000fa30: 7428 502a 7831 2877 2929 2077 6865 7265  t(P*x1(w)) where
-0000fa40: 2078 3120 6973 2074 6865 2066 6674 6564   x1 is the ffted
-0000fa50: 2073 7065 6374 7261 0a20 2020 2061 6e64   spectra.    and
-0000fa60: 2050 2069 7320 7468 6520 6669 6c74 6572   P is the filter
-0000fa70: 2e20 5020 6973 2063 6f6e 7374 7275 6374  . P is construct
-0000fa80: 6564 2062 7920 7573 696e 6720 7468 6520  ed by using the 
-0000fa90: 7465 6d70 6f72 616c 2063 6f76 6172 6961  temporal covaria
-0000faa0: 6e63 6520 6d61 7472 6978 2e0a 0a20 2020  nce matrix...   
-0000fab0: 2050 4152 414d 4554 4552 533a 0a20 2020   PARAMETERS:.   
-0000fac0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-0000fad0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6172 723a  -------.    arr:
-0000fae0: 206e 756d 7079 2e6e 6461 7272 6179 2063   numpy.ndarray c
-0000faf0: 6f6e 7461 696e 7320 7468 6520 3244 2074  ontains the 2D t
-0000fb00: 7261 6365 7320 6f66 2064 6169 6c79 2f68  races of daily/h
-0000fb10: 6f75 726c 7920 6372 6f73 732d 636f 7272  ourly cross-corr
-0000fb20: 656c 6174 696f 6e20 6675 6e63 7469 6f6e  elation function
-0000fb30: 730a 2020 2020 673a 2061 2070 6f73 6974  s.    g: a posit
-0000fb40: 6976 6520 6e75 6d62 6572 2074 6f20 6164  ive number to ad
-0000fb50: 6a75 7374 2074 6865 2066 696c 7465 7220  just the filter 
-0000fb60: 6861 7273 686e 6573 730a 2020 2020 5245  harshness.    RE
-0000fb70: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
-0000fb80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0000fb90: 2d0a 2020 2020 6e61 7272 3a20 6e75 6d70  -.    narr: nump
-0000fba0: 7920 7665 6374 6f72 2063 6f6e 7461 696e  y vector contain
-0000fbb0: 7320 7468 6520 7374 6163 6b65 6420 6372  s the stacked cr
-0000fbc0: 6f73 7320 636f 7272 656c 6174 696f 6e20  oss correlation 
-0000fbd0: 6675 6e63 7469 6f6e 0a20 2020 2022 2222  function.    """
-0000fbe0: 0a20 2020 2069 6620 6172 722e 6e64 696d  .    if arr.ndim
-0000fbf0: 203d 3d20 313a 0a20 2020 2020 2020 2072   == 1:.        r
-0000fc00: 6574 7572 6e20 6172 720a 2020 2020 4e2c  eturn arr.    N,
-0000fc10: 204d 203d 2061 7272 2e73 6861 7065 0a20   M = arr.shape. 
-0000fc20: 2020 204e 6666 7420 3d20 6e65 7874 5f66     Nfft = next_f
-0000fc30: 6173 745f 6c65 6e28 4d29 0a0a 2020 2020  ast_len(M)..    
-0000fc40: 2320 6666 7420 7468 6520 3244 2061 7272  # fft the 2D arr
-0000fc50: 6179 0a20 2020 2073 7065 6320 3d20 7363  ay.    spec = sc
-0000fc60: 6970 792e 6666 7470 6163 6b2e 6666 7428  ipy.fftpack.fft(
-0000fc70: 6172 722c 2061 7869 733d 312c 206e 3d4e  arr, axis=1, n=N
-0000fc80: 6666 7429 5b3a 2c20 3a4d 5d0a 0a20 2020  fft)[:, :M]..   
-0000fc90: 2023 206d 616b 6520 6372 6f73 732d 7370   # make cross-sp
-0000fca0: 6563 7472 6d20 6d61 7472 6978 0a20 2020  ectrm matrix.   
-0000fcb0: 2063 7370 6563 203d 206e 702e 7a65 726f   cspec = np.zero
-0000fcc0: 7328 7368 6170 653d 284e 202a 204e 2c20  s(shape=(N * N, 
-0000fcd0: 4d29 2c20 6474 7970 653d 6e70 2e63 6f6d  M), dtype=np.com
-0000fce0: 706c 6578 3634 290a 2020 2020 666f 7220  plex64).    for 
-0000fcf0: 6969 2069 6e20 7261 6e67 6528 4e29 3a0a  ii in range(N):.
-0000fd00: 2020 2020 2020 2020 666f 7220 6a6a 2069          for jj i
-0000fd10: 6e20 7261 6e67 6528 4e29 3a0a 2020 2020  n range(N):.    
-0000fd20: 2020 2020 2020 2020 6b6b 203d 2069 6920          kk = ii 
-0000fd30: 2a20 4e20 2b20 6a6a 0a20 2020 2020 2020  * N + jj.       
-0000fd40: 2020 2020 2063 7370 6563 5b6b 6b5d 203d       cspec[kk] =
-0000fd50: 2073 7065 635b 6969 5d20 2a20 6e70 2e63   spec[ii] * np.c
-0000fd60: 6f6e 6a75 6761 7465 2873 7065 635b 6a6a  onjugate(spec[jj
-0000fd70: 5d29 0a0a 2020 2020 5331 203d 206e 702e  ])..    S1 = np.
-0000fd80: 7a65 726f 7328 4d2c 2064 7479 7065 3d6e  zeros(M, dtype=n
-0000fd90: 702e 636f 6d70 6c65 7836 3429 0a20 2020  p.complex64).   
-0000fda0: 2053 3220 3d20 6e70 2e7a 6572 6f73 284d   S2 = np.zeros(M
-0000fdb0: 2c20 6474 7970 653d 6e70 2e63 6f6d 706c  , dtype=np.compl
-0000fdc0: 6578 3634 290a 2020 2020 2320 636f 6e73  ex64).    # cons
-0000fdd0: 7472 7563 7420 7468 6520 6669 6c74 6572  truct the filter
-0000fde0: 2050 0a20 2020 2066 6f72 2069 6920 696e   P.    for ii in
-0000fdf0: 2072 616e 6765 284e 293a 0a20 2020 2020   range(N):.     
-0000fe00: 2020 206d 6d20 3d20 6969 202a 204e 202b     mm = ii * N +
-0000fe10: 2069 690a 2020 2020 2020 2020 5332 202b   ii.        S2 +
-0000fe20: 3d20 6373 7065 635b 6d6d 5d0a 2020 2020  = cspec[mm].    
-0000fe30: 2020 2020 666f 7220 6a6a 2069 6e20 7261      for jj in ra
-0000fe40: 6e67 6528 4e29 3a0a 2020 2020 2020 2020  nge(N):.        
-0000fe50: 2020 2020 6b6b 203d 2069 6920 2a20 4e20      kk = ii * N 
-0000fe60: 2b20 6a6a 0a20 2020 2020 2020 2020 2020  + jj.           
-0000fe70: 2053 3120 2b3d 2063 7370 6563 5b6b 6b5d   S1 += cspec[kk]
-0000fe80: 0a0a 2020 2020 7020 3d20 6e70 2e70 6f77  ..    p = np.pow
-0000fe90: 6572 2828 5331 202d 2053 3229 202f 2028  er((S1 - S2) / (
-0000fea0: 5332 202a 2028 4e20 2d20 3129 292c 2067  S2 * (N - 1)), g
-0000feb0: 290a 0a20 2020 2023 206d 616b 6520 6966  )..    # make if
-0000fec0: 6674 0a20 2020 206e 6172 7220 3d20 6e70  ft.    narr = np
-0000fed0: 2e72 6561 6c28 7363 6970 792e 6666 7470  .real(scipy.fftp
-0000fee0: 6163 6b2e 6966 6674 286e 702e 6d75 6c74  ack.ifft(np.mult
-0000fef0: 6970 6c79 2870 2c20 7370 6563 292c 204e  iply(p, spec), N
-0000ff00: 6666 742c 2061 7869 733d 3129 5b3a 2c20  fft, axis=1)[:, 
-0000ff10: 3a4d 5d29 0a20 2020 2072 6574 7572 6e20  :M]).    return 
-0000ff20: 6e70 2e6d 6561 6e28 6e61 7272 2c20 6178  np.mean(narr, ax
-0000ff30: 6973 3d30 290a 0a0a 6465 6620 7077 7328  is=0)...def pws(
-0000ff40: 6172 722c 2073 616d 706c 696e 675f 7261  arr, sampling_ra
-0000ff50: 7465 2c20 706f 7765 723d 322c 2070 7773  te, power=2, pws
-0000ff60: 5f74 696d 6567 6174 653d 352e 3029 3a0a  _timegate=5.0):.
-0000ff70: 2020 2020 2222 220a 2020 2020 5065 7266      """.    Perf
-0000ff80: 6f72 6d73 2070 6861 7365 2d77 6569 6768  orms phase-weigh
-0000ff90: 7465 6420 7374 6163 6b20 6f6e 2061 7272  ted stack on arr
-0000ffa0: 6179 206f 6620 7469 6d65 2073 6572 6965  ay of time serie
-0000ffb0: 732e 204d 6f64 6966 6965 6420 6f6e 2074  s. Modified on t
-0000ffc0: 6865 206e 6f69 7365 2066 756e 6374 696f  he noise functio
-0000ffd0: 6e20 6279 2054 696d 2043 6c69 6d65 6e74  n by Tim Climent
-0000ffe0: 732e 0a20 2020 2046 6f6c 6c6f 7773 206d  s..    Follows m
-0000fff0: 6574 686f 6473 206f 6620 5363 6869 6d6d  ethods of Schimm
-00010000: 656c 2061 6e64 2050 6175 6c73 7365 6e2c  el and Paulssen,
-00010010: 2031 3939 372e 0a20 2020 2049 6620 7328   1997..    If s(
-00010020: 7429 2069 7320 7469 6d65 2073 6572 6965  t) is time serie
-00010030: 7320 6461 7461 2028 7365 6973 6d6f 6772  s data (seismogr
-00010040: 616d 2c20 6f72 2063 726f 7373 2d63 6f72  am, or cross-cor
-00010050: 7265 6c61 7469 6f6e 292c 0a20 2020 2053  relation),.    S
-00010060: 2874 2920 3d20 7328 7429 202b 2069 2a48  (t) = s(t) + i*H
-00010070: 2873 2874 2929 2c20 7768 6572 6520 4828  (s(t)), where H(
-00010080: 7328 7429 2920 6973 2048 696c 6265 7274  s(t)) is Hilbert
-00010090: 2074 7261 6e73 666f 726d 206f 6620 7328   transform of s(
-000100a0: 7429 0a20 2020 2053 2874 2920 3d20 7328  t).    S(t) = s(
-000100b0: 7429 202b 2069 2a48 2873 2874 2929 203d  t) + i*H(s(t)) =
-000100c0: 2041 2874 292a 6578 7028 692a 7068 6928   A(t)*exp(i*phi(
-000100d0: 7429 292c 2077 6865 7265 0a20 2020 2041  t)), where.    A
-000100e0: 2874 2920 6973 2065 6e76 656c 6f70 6520  (t) is envelope 
-000100f0: 6f66 2073 2874 2920 616e 6420 7068 6928  of s(t) and phi(
-00010100: 7429 2069 7320 7068 6173 6520 6f66 2073  t) is phase of s
-00010110: 2874 290a 2020 2020 5068 6173 652d 7765  (t).    Phase-we
-00010120: 6967 6874 6564 2073 7461 636b 2c20 6728  ighted stack, g(
-00010130: 7429 2c20 6973 2074 6865 6e3a 0a20 2020  t), is then:.   
-00010140: 2067 2874 2920 3d20 312f 4e20 7375 6d20   g(t) = 1/N sum 
-00010150: 6a20 3d20 313a 4e20 735f 6a28 7429 202a  j = 1:N s_j(t) *
-00010160: 207c 2031 2f4e 2073 756d 206b 203d 2031   | 1/N sum k = 1
-00010170: 3a4e 2065 7870 5b69 202a 2070 6869 5f6b  :N exp[i * phi_k
-00010180: 2874 295d 7c5e 760a 2020 2020 7768 6572  (t)]|^v.    wher
-00010190: 6520 4e20 6973 206e 756d 6265 7220 6f66  e N is number of
-000101a0: 2074 7261 6365 7320 7573 6564 2c20 7620   traces used, v 
-000101b0: 6973 2073 6861 7270 6e65 7373 206f 6620  is sharpness of 
-000101c0: 7068 6173 652d 7765 6967 6874 6564 2073  phase-weighted s
-000101d0: 7461 636b 0a0a 2020 2020 5041 5241 4d45  tack..    PARAME
-000101e0: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
-000101f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00010200: 2020 2020 6172 723a 204e 206c 656e 6774      arr: N lengt
-00010210: 6820 6172 7261 7920 6f66 2074 696d 6520  h array of time 
-00010220: 7365 7269 6573 2064 6174 6120 286e 756d  series data (num
-00010230: 7079 2e6e 6461 7272 6179 290a 2020 2020  py.ndarray).    
-00010240: 7361 6d70 6c69 6e67 5f72 6174 653a 2073  sampling_rate: s
-00010250: 616d 706c 696e 6720 7261 7465 206f 6620  ampling rate of 
-00010260: 7469 6d65 2073 6572 6965 7320 6172 7220  time series arr 
-00010270: 2869 6e74 290a 2020 2020 706f 7765 723a  (int).    power:
-00010280: 2065 7870 6f6e 656e 7420 666f 7220 7068   exponent for ph
-00010290: 6173 6520 7374 6163 6b20 2869 6e74 290a  ase stack (int).
-000102a0: 2020 2020 7077 735f 7469 6d65 6761 7465      pws_timegate
-000102b0: 3a20 6e75 6d62 6572 206f 6620 7365 636f  : number of seco
-000102c0: 6e64 7320 746f 2073 6d6f 6f74 6820 7068  nds to smooth ph
-000102d0: 6173 6520 7374 6163 6b20 2866 6c6f 6174  ase stack (float
-000102e0: 290a 0a20 2020 2052 4554 5552 4e53 3a0a  )..    RETURNS:.
-000102f0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-00010300: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7765  ---------.    we
-00010310: 6967 6874 6564 3a20 5068 6173 6520 7765  ighted: Phase we
-00010320: 6967 6874 6564 2073 7461 636b 206f 6620  ighted stack of 
-00010330: 7469 6d65 2073 6572 6965 7320 6461 7461  time series data
-00010340: 2028 6e75 6d70 792e 6e64 6172 7261 7929   (numpy.ndarray)
-00010350: 0a20 2020 2022 2222 0a0a 2020 2020 6966  .    """..    if
-00010360: 2061 7272 2e6e 6469 6d20 3d3d 2031 3a0a   arr.ndim == 1:.
-00010370: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00010380: 7272 0a20 2020 204e 2c20 4d20 3d20 6172  rr.    N, M = ar
-00010390: 722e 7368 6170 650a 2020 2020 616e 616c  r.shape.    anal
-000103a0: 7974 6963 203d 2068 696c 6265 7274 2861  ytic = hilbert(a
-000103b0: 7272 2c20 6178 6973 3d31 2c20 4e3d 6e65  rr, axis=1, N=ne
-000103c0: 7874 5f66 6173 745f 6c65 6e28 4d29 295b  xt_fast_len(M))[
-000103d0: 3a2c 203a 4d5d 0a20 2020 2070 6861 7365  :, :M].    phase
-000103e0: 203d 206e 702e 616e 676c 6528 616e 616c   = np.angle(anal
-000103f0: 7974 6963 290a 2020 2020 7068 6173 655f  ytic).    phase_
-00010400: 7374 6163 6b20 3d20 6e70 2e6d 6561 6e28  stack = np.mean(
-00010410: 6e70 2e65 7870 2831 6a20 2a20 7068 6173  np.exp(1j * phas
-00010420: 6529 2c20 6178 6973 3d30 290a 2020 2020  e), axis=0).    
-00010430: 7068 6173 655f 7374 6163 6b20 3d20 6e70  phase_stack = np
-00010440: 2e61 6273 2870 6861 7365 5f73 7461 636b  .abs(phase_stack
-00010450: 2920 2a2a 2028 706f 7765 7229 0a0a 2020  ) ** (power)..  
-00010460: 2020 2320 736d 6f6f 7468 696e 670a 2020    # smoothing.  
-00010470: 2020 2320 7469 6d65 6761 7465 5f73 616d    # timegate_sam
-00010480: 706c 6573 203d 2069 6e74 2870 7773 5f74  ples = int(pws_t
-00010490: 696d 6567 6174 6520 2a20 7361 6d70 6c69  imegate * sampli
-000104a0: 6e67 5f72 6174 6529 0a20 2020 2023 2070  ng_rate).    # p
-000104b0: 6861 7365 5f73 7461 636b 203d 206d 6f76  hase_stack = mov
-000104c0: 696e 675f 6176 6528 7068 6173 655f 7374  ing_ave(phase_st
-000104d0: 6163 6b2c 7469 6d65 6761 7465 5f73 616d  ack,timegate_sam
-000104e0: 706c 6573 290a 2020 2020 7765 6967 6874  ples).    weight
-000104f0: 6564 203d 206e 702e 6d75 6c74 6970 6c79  ed = np.multiply
-00010500: 2861 7272 2c20 7068 6173 655f 7374 6163  (arr, phase_stac
-00010510: 6b29 0a20 2020 2072 6574 7572 6e20 6e70  k).    return np
-00010520: 2e6d 6561 6e28 7765 6967 6874 6564 2c20  .mean(weighted, 
-00010530: 6178 6973 3d30 290a 0a0a 6465 6620 6e72  axis=0)...def nr
-00010540: 6f6f 745f 7374 6163 6b28 6363 5f61 7272  oot_stack(cc_arr
-00010550: 6179 2c20 706f 7765 7229 3a0a 2020 2020  ay, power):.    
-00010560: 2222 220a 2020 2020 7468 6973 2069 7320  """.    this is 
-00010570: 6e74 682d 726f 6f74 2073 7461 636b 696e  nth-root stackin
-00010580: 6720 616c 676f 7269 7468 6d20 7472 616e  g algorithm tran
-00010590: 736c 6174 6564 2062 6173 6564 206f 6e20  slated based on 
-000105a0: 7468 6520 6d61 746c 6162 2066 756e 6374  the matlab funct
-000105b0: 696f 6e0a 2020 2020 6672 6f6d 2068 7474  ion.    from htt
-000105c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000105d0: 7874 7961 6e67 7073 702f 5365 6973 5374  xtyangpsp/SeisSt
-000105e0: 6163 6b20 2862 7920 5869 616f 7461 6f20  ack (by Xiaotao 
-000105f0: 5961 6e67 3b20 666f 6c6c 6f77 7320 7468  Yang; follows th
-00010600: 650a 2020 2020 7265 6665 7265 6e63 6520  e.    reference 
-00010610: 6f66 204d 696c 6c65 742c 2046 2065 7420  of Millet, F et 
-00010620: 616c 2e2c 2032 3031 3920 4a47 5229 0a0a  al., 2019 JGR)..
-00010630: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
-00010640: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
-00010650: 0a20 2020 2063 635f 6172 7261 793a 206e  .    cc_array: n
-00010660: 756d 7079 2e6e 6461 7272 6179 2063 6f6e  umpy.ndarray con
-00010670: 7461 696e 7320 7468 6520 3244 2063 726f  tains the 2D cro
-00010680: 7373 2063 6f72 7265 6c61 7469 6f6e 206d  ss correlation m
-00010690: 6174 7269 780a 2020 2020 706f 7765 723a  atrix.    power:
-000106a0: 206e 702e 696e 742c 206e 7468 2072 6f6f   np.int, nth roo
-000106b0: 7420 666f 7220 7468 6520 7374 6163 6b69  t for the stacki
-000106c0: 6e67 0a0a 2020 2020 5265 7475 726e 733a  ng..    Returns:
-000106d0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
-000106e0: 2d0a 2020 2020 6e73 7461 636b 3a20 6e70  -.    nstack: np
-000106f0: 2e6e 6461 7272 6179 2c20 6669 6e61 6c20  .ndarray, final 
-00010700: 7374 6163 6b65 6420 7761 7665 666f 726d  stacked waveform
-00010710: 730a 0a20 2020 2057 7269 7474 656e 2062  s..    Written b
-00010720: 7920 4368 656e 6778 696e 204a 6961 6e67  y Chengxin Jiang
-00010730: 2040 414e 5520 284d 6179 3230 3230 290a   @ANU (May2020).
-00010740: 2020 2020 2222 220a 2020 2020 6966 2063      """.    if c
-00010750: 635f 6172 7261 792e 6e64 696d 203d 3d20  c_array.ndim == 
-00010760: 313a 0a20 2020 2020 2020 2070 7269 6e74  1:.        print
-00010770: 2822 3244 206d 6174 7269 7820 6973 206e  ("2D matrix is n
-00010780: 6565 6465 6420 666f 7220 6e72 6f6f 745f  eeded for nroot_
-00010790: 7374 6163 6b22 290a 2020 2020 2020 2020  stack").        
-000107a0: 7265 7475 726e 2063 635f 6172 7261 790a  return cc_array.
-000107b0: 2020 2020 4e2c 204d 203d 2063 635f 6172      N, M = cc_ar
-000107c0: 7261 792e 7368 6170 650a 2020 2020 646f  ray.shape.    do
-000107d0: 7574 203d 206e 702e 7a65 726f 7328 4d2c  ut = np.zeros(M,
-000107e0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-000107f0: 3229 0a0a 2020 2020 2320 636f 6e73 7472  2)..    # constr
-00010800: 7563 7420 790a 2020 2020 666f 7220 6969  uct y.    for ii
-00010810: 2069 6e20 7261 6e67 6528 4e29 3a0a 2020   in range(N):.  
-00010820: 2020 2020 2020 6461 7420 3d20 6363 5f61        dat = cc_a
-00010830: 7272 6179 5b69 692c 203a 5d0a 2020 2020  rray[ii, :].    
-00010840: 2020 2020 646f 7574 202b 3d20 6e70 2e73      dout += np.s
-00010850: 6967 6e28 6461 7429 202a 206e 702e 6162  ign(dat) * np.ab
-00010860: 7328 6461 7429 202a 2a20 2831 202f 2070  s(dat) ** (1 / p
-00010870: 6f77 6572 290a 2020 2020 646f 7574 202f  ower).    dout /
-00010880: 3d20 4e0a 0a20 2020 2023 2074 6865 2066  = N..    # the f
-00010890: 696e 616c 2073 7461 636b 6564 2077 6176  inal stacked wav
-000108a0: 6566 6f72 6d0a 2020 2020 6e73 7461 636b  eform.    nstack
-000108b0: 203d 2064 6f75 7420 2a20 6e70 2e61 6273   = dout * np.abs
-000108c0: 2864 6f75 7429 202a 2a20 2870 6f77 6572  (dout) ** (power
-000108d0: 202d 2031 290a 0a20 2020 2072 6574 7572   - 1)..    retur
-000108e0: 6e20 6e73 7461 636b 0a0a 0a64 6566 2073  n nstack...def s
-000108f0: 656c 6563 7469 7665 5f73 7461 636b 2863  elective_stack(c
-00010900: 635f 6172 7261 792c 2065 7073 696c 6f6e  c_array, epsilon
-00010910: 2c20 6363 5f74 6829 3a20 2023 206e 6f71  , cc_th):  # noq
-00010920: 613a 2046 3831 310a 2020 2020 2222 220a  a: F811.    """.
-00010930: 2020 2020 7468 6973 2069 7320 6120 7365      this is a se
-00010940: 6c65 6374 6976 6520 7374 6163 6b69 6e67  lective stacking
-00010950: 2061 6c67 6f72 6974 686d 2064 6576 656c   algorithm devel
-00010960: 6f70 6564 2062 7920 4a61 7265 6420 4272  oped by Jared Br
-00010970: 7961 6e2f 4b75 7261 6d61 204f 6b75 626f  yan/Kurama Okubo
-00010980: 2e0a 0a20 2020 2050 4152 414d 4554 4552  ...    PARAMETER
-00010990: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-000109a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-000109b0: 2020 6363 5f61 7272 6179 3a20 6e75 6d70    cc_array: nump
-000109c0: 792e 6e64 6172 7261 7920 636f 6e74 6169  y.ndarray contai
-000109d0: 6e73 2074 6865 2032 4420 6372 6f73 7320  ns the 2D cross 
-000109e0: 636f 7272 656c 6174 696f 6e20 6d61 7472  correlation matr
-000109f0: 6978 0a20 2020 2065 7073 696c 6f6e 3a20  ix.    epsilon: 
-00010a00: 7265 7369 6475 616c 2074 6872 6568 6f6c  residual threhol
-00010a10: 6420 746f 2071 7569 7420 7468 6520 6974  d to quit the it
-00010a20: 6572 6174 696f 6e0a 2020 2020 6363 5f74  eration.    cc_t
-00010a30: 683a 206e 756d 7079 2e66 6c6f 6174 2c20  h: numpy.float, 
-00010a40: 7468 7265 7368 6f6c 6420 6f66 2063 6f72  threshold of cor
-00010a50: 7265 6c61 7469 6f6e 2063 6f65 6666 6963  relation coeffic
-00010a60: 6965 6e74 2074 6f20 6265 2073 656c 6563  ient to be selec
-00010a70: 7465 640a 0a20 2020 2052 4554 5552 4e53  ted..    RETURNS
-00010a80: 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  :.    ----------
-00010a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00010aa0: 206e 6577 7374 6163 6b3a 206e 756d 7079   newstack: numpy
-00010ab0: 2076 6563 746f 7220 636f 6e74 6169 6e73   vector contains
-00010ac0: 2074 6865 2073 7461 636b 6564 2063 726f   the stacked cro
-00010ad0: 7373 2063 6f72 7265 6c61 7469 6f6e 0a20  ss correlation. 
-00010ae0: 2020 206e 7374 6570 3a20 6e70 2e69 6e74     nstep: np.int
-00010af0: 2c20 746f 7461 6c20 6e75 6d62 6572 206f  , total number o
-00010b00: 6620 6974 6572 6174 696f 6e73 2066 6f72  f iterations for
-00010b10: 2074 6865 2073 7461 636b 696e 670a 0a20   the stacking.. 
-00010b20: 2020 204f 7269 6769 6e61 6c6c 7920 7269     Originally ri
-00010b30: 7474 656e 2062 7920 4d61 7269 6e65 2044  tten by Marine D
-00010b40: 656e 6f6c 6c65 0a20 2020 204d 6f64 6966  enolle.    Modif
-00010b50: 6965 6420 6279 2043 6865 6e67 7869 6e20  ied by Chengxin 
-00010b60: 4a69 616e 6720 4048 6172 7661 7264 2028  Jiang @Harvard (
-00010b70: 4f63 7432 3032 3029 0a20 2020 2022 2222  Oct2020).    """
-00010b80: 0a20 2020 2069 6620 6363 5f61 7272 6179  .    if cc_array
-00010b90: 2e6e 6469 6d20 3d3d 2031 3a0a 2020 2020  .ndim == 1:.    
-00010ba0: 2020 2020 7072 696e 7428 2232 4420 6d61      print("2D ma
-00010bb0: 7472 6978 2069 7320 6e65 6564 6564 2066  trix is needed f
-00010bc0: 6f72 206e 726f 6f74 5f73 7461 636b 2229  or nroot_stack")
-00010bd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010be0: 6363 5f61 7272 6179 0a20 2020 204e 2c20  cc_array.    N, 
-00010bf0: 4d20 3d20 6363 5f61 7272 6179 2e73 6861  M = cc_array.sha
-00010c00: 7065 0a0a 2020 2020 7265 7320 3d20 3965  pe..    res = 9e
-00010c10: 3920 2023 2072 6573 6964 7561 6c73 0a20  9  # residuals. 
-00010c20: 2020 2063 6f66 203d 206e 702e 7a65 726f     cof = np.zero
-00010c30: 7328 4e2c 2064 7479 7065 3d6e 702e 666c  s(N, dtype=np.fl
-00010c40: 6f61 7433 3229 0a20 2020 206e 6577 7374  oat32).    newst
-00010c50: 6163 6b20 3d20 6e70 2e6d 6561 6e28 6363  ack = np.mean(cc
-00010c60: 5f61 7272 6179 2c20 6178 6973 3d30 290a  _array, axis=0).
-00010c70: 0a20 2020 206e 7374 6570 203d 2030 0a20  .    nstep = 0. 
-00010c80: 2020 2023 2073 7461 7274 2069 7465 7261     # start itera
-00010c90: 7469 6f6e 0a20 2020 2077 6869 6c65 2072  tion.    while r
-00010ca0: 6573 203e 2065 7073 696c 6f6e 3a0a 2020  es > epsilon:.  
-00010cb0: 2020 2020 2020 666f 7220 6969 2069 6e20        for ii in 
-00010cc0: 7261 6e67 6528 4e29 3a0a 2020 2020 2020  range(N):.      
-00010cd0: 2020 2020 2020 636f 665b 6969 5d20 3d20        cof[ii] = 
-00010ce0: 6e70 2e63 6f72 7263 6f65 6628 6e65 7773  np.corrcoef(news
-00010cf0: 7461 636b 2c20 6363 5f61 7272 6179 5b69  tack, cc_array[i
-00010d00: 692c 203a 5d29 5b30 2c20 315d 0a0a 2020  i, :])[0, 1]..  
-00010d10: 2020 2020 2020 2320 6669 6e64 2067 6f6f        # find goo
-00010d20: 6420 7761 7665 666f 726d 730a 2020 2020  d waveforms.    
-00010d30: 2020 2020 696e 6478 203d 206e 702e 7768      indx = np.wh
-00010d40: 6572 6528 636f 6620 3e3d 2063 635f 7468  ere(cof >= cc_th
-00010d50: 295b 305d 0a20 2020 2020 2020 2069 6620  )[0].        if 
-00010d60: 6e6f 7420 6c65 6e28 696e 6478 293a 0a20  not len(indx):. 
-00010d70: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00010d80: 2056 616c 7565 4572 726f 7228 2263 616e   ValueError("can
-00010d90: 6e6f 7420 6669 6e64 2067 6f6f 6420 7761  not find good wa
-00010da0: 7665 666f 726d 7320 696e 7369 6465 2073  veforms inside s
-00010db0: 656c 6563 7469 7665 2073 7461 636b 696e  elective stackin
-00010dc0: 6722 290a 2020 2020 2020 2020 6f6c 6473  g").        olds
-00010dd0: 7461 636b 203d 206e 6577 7374 6163 6b0a  tack = newstack.
-00010de0: 2020 2020 2020 2020 6e65 7773 7461 636b          newstack
-00010df0: 203d 206e 702e 6d65 616e 2863 635f 6172   = np.mean(cc_ar
-00010e00: 7261 795b 696e 6478 5d2c 2061 7869 733d  ray[indx], axis=
-00010e10: 3029 0a20 2020 2020 2020 2072 6573 203d  0).        res =
-00010e20: 206e 702e 6c69 6e61 6c67 2e6e 6f72 6d28   np.linalg.norm(
-00010e30: 6e65 7773 7461 636b 202d 206f 6c64 7374  newstack - oldst
-00010e40: 6163 6b29 202f 2028 6e70 2e6c 696e 616c  ack) / (np.linal
-00010e50: 672e 6e6f 726d 286e 6577 7374 6163 6b29  g.norm(newstack)
-00010e60: 202a 204d 290a 2020 2020 2020 2020 6e73   * M).        ns
-00010e70: 7465 7020 2b3d 2031 0a0a 2020 2020 7265  tep += 1..    re
-00010e80: 7475 726e 206e 6577 7374 6163 6b2c 206e  turn newstack, n
-00010e90: 7374 6570 0a0a 0a64 6566 2067 6574 5f63  step...def get_c
-00010ea0: 6328 7331 2c20 735f 7265 6629 3a0a 2020  c(s1, s_ref):.  
-00010eb0: 2020 2320 7265 7475 726e 7320 7468 6520    # returns the 
-00010ec0: 636f 7272 656c 6174 696f 6e20 636f 6566  correlation coef
-00010ed0: 6669 6369 656e 7420 6265 7477 6565 6e20  ficient between 
-00010ee0: 7761 7665 666f 726d 7320 696e 2073 3120  waveforms in s1 
-00010ef0: 6167 6169 6e73 7420 7265 6665 7265 6e63  against referenc
-00010f00: 650a 2020 2020 2320 7761 7665 666f 726d  e.    # waveform
-00010f10: 2073 5f72 6566 2e0a 2020 2020 230a 2020   s_ref..    #.  
-00010f20: 2020 6363 203d 206e 702e 7a65 726f 7328    cc = np.zeros(
-00010f30: 7331 2e73 6861 7065 5b30 5d29 0a20 2020  s1.shape[0]).   
-00010f40: 2073 5f72 6566 5f6e 6f72 6d20 3d20 6e70   s_ref_norm = np
-00010f50: 2e6c 696e 616c 672e 6e6f 726d 2873 5f72  .linalg.norm(s_r
-00010f60: 6566 290a 2020 2020 666f 7220 6920 696e  ef).    for i in
-00010f70: 2072 616e 6765 2873 312e 7368 6170 655b   range(s1.shape[
-00010f80: 305d 293a 0a20 2020 2020 2020 2063 635b  0]):.        cc[
-00010f90: 695d 203d 206e 702e 7375 6d28 6e70 2e6d  i] = np.sum(np.m
-00010fa0: 756c 7469 706c 7928 7331 5b69 2c20 3a5d  ultiply(s1[i, :]
-00010fb0: 2c20 735f 7265 6629 2920 2f20 6e70 2e6c  , s_ref)) / np.l
-00010fc0: 696e 616c 672e 6e6f 726d 2873 315b 692c  inalg.norm(s1[i,
-00010fd0: 203a 5d29 202f 2073 5f72 6566 5f6e 6f72   :]) / s_ref_nor
-00010fe0: 6d0a 2020 2020 7265 7475 726e 2063 630a  m.    return cc.
-00010ff0: 0a0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+0000b260: 2323 2323 2323 230a 0a0a 6465 6620 6368  #######...def ch
+0000b270: 6563 6b5f 7361 6d70 6c65 5f67 6170 7328  eck_sample_gaps(
+0000b280: 7374 7265 616d 3a20 6f62 7370 792e 5374  stream: obspy.St
+0000b290: 7265 616d 2c20 7374 6172 7474 696d 653a  ream, starttime:
+0000b2a0: 206f 6273 7079 2e55 5443 4461 7465 5469   obspy.UTCDateTi
+0000b2b0: 6d65 2c20 656e 6474 696d 653a 206f 6273  me, endtime: obs
+0000b2c0: 7079 2e55 5443 4461 7465 5469 6d65 293a  py.UTCDateTime):
+0000b2d0: 0a20 2020 2022 2222 0a20 2020 2074 6869  .    """.    thi
+0000b2e0: 7320 6675 6e63 7469 6f6e 2063 6865 636b  s function check
+0000b2f0: 7320 7361 6d70 6c69 6e67 2072 6174 6520  s sampling rate 
+0000b300: 616e 6420 6669 6e64 2067 6170 7320 6f66  and find gaps of
+0000b310: 2061 6c6c 2074 7261 6365 7320 696e 2073   all traces in s
+0000b320: 7472 6561 6d2e 0a20 2020 2050 4152 414d  tream..    PARAM
+0000b330: 4554 4552 533a 0a20 2020 202d 2d2d 2d2d  ETERS:.    -----
+0000b340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+0000b350: 2073 7472 6561 6d3a 206f 6273 7079 2073   stream: obspy s
+0000b360: 7472 6561 6d20 6f62 6a65 6374 2e0a 2020  tream object..  
+0000b370: 2020 6461 7465 5f69 6e66 6f3a 2064 6963    date_info: dic
+0000b380: 7420 6f66 2073 7461 7274 696e 6720 616e  t of starting an
+0000b390: 6420 656e 6469 6e67 2074 696d 6520 6f66  d ending time of
+0000b3a0: 2074 6865 2073 7472 6561 6d0a 0a20 2020   the stream..   
+0000b3b0: 2052 4554 5552 454e 533a 0a20 2020 202d   RETURENS:.    -
+0000b3c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b3d0: 0a20 2020 2073 7472 6561 6d3a 204c 6973  .    stream: Lis
+0000b3e0: 7420 6f66 2067 6f6f 6420 7472 6163 6573  t of good traces
+0000b3f0: 2069 6e20 7468 6520 7374 7265 616d 0a20   in the stream. 
+0000b400: 2020 2022 2222 0a20 2020 2023 2072 656d     """.    # rem
+0000b410: 6f76 6520 656d 7074 792f 6269 6720 7472  ove empty/big tr
+0000b420: 6163 6573 0a20 2020 2069 6620 6c65 6e28  aces.    if len(
+0000b430: 7374 7265 616d 2920 3d3d 2030 206f 7220  stream) == 0 or 
+0000b440: 6c65 6e28 7374 7265 616d 2920 3e20 3130  len(stream) > 10
+0000b450: 303a 0a20 2020 2020 2020 2073 7472 6561  0:.        strea
+0000b460: 6d20 3d20 5b5d 0a20 2020 2020 2020 2072  m = [].        r
+0000b470: 6574 7572 6e20 7374 7265 616d 0a0a 2020  eturn stream..  
+0000b480: 2020 2320 7265 6d6f 7665 2074 7261 6365    # remove trace
+0000b490: 7320 7769 7468 2062 6967 2067 6170 730a  s with big gaps.
+0000b4a0: 2020 2020 6966 2070 6f72 7469 6f6e 5f67      if portion_g
+0000b4b0: 6170 7328 7374 7265 616d 2c20 7374 6172  aps(stream, star
+0000b4c0: 7474 696d 652c 2065 6e64 7469 6d65 2920  ttime, endtime) 
+0000b4d0: 3e20 302e 333a 0a20 2020 2020 2020 2073  > 0.3:.        s
+0000b4e0: 7472 6561 6d20 3d20 5b5d 0a20 2020 2020  tream = [].     
+0000b4f0: 2020 2072 6574 7572 6e20 7374 7265 616d     return stream
+0000b500: 0a0a 2020 2020 6672 6571 7320 3d20 5b5d  ..    freqs = []
+0000b510: 0a20 2020 2066 6f72 2074 7220 696e 2073  .    for tr in s
+0000b520: 7472 6561 6d3a 0a20 2020 2020 2020 2066  tream:.        f
+0000b530: 7265 7173 2e61 7070 656e 6428 696e 7428  reqs.append(int(
+0000b540: 7472 2e73 7461 7473 2e73 616d 706c 696e  tr.stats.samplin
+0000b550: 675f 7261 7465 2929 0a20 2020 2066 7265  g_rate)).    fre
+0000b560: 7120 3d20 6d61 7828 6672 6571 7329 0a20  q = max(freqs). 
+0000b570: 2020 2066 6f72 2074 7220 696e 2073 7472     for tr in str
+0000b580: 6561 6d3a 0a20 2020 2020 2020 2069 6620  eam:.        if 
+0000b590: 696e 7428 7472 2e73 7461 7473 2e73 616d  int(tr.stats.sam
+0000b5a0: 706c 696e 675f 7261 7465 2920 213d 2066  pling_rate) != f
+0000b5b0: 7265 713a 0a20 2020 2020 2020 2020 2020  req:.           
+0000b5c0: 2073 7472 6561 6d2e 7265 6d6f 7665 2874   stream.remove(t
+0000b5d0: 7229 0a20 2020 2020 2020 2069 6620 7472  r).        if tr
+0000b5e0: 2e73 7461 7473 2e6e 7074 7320 3c20 3130  .stats.npts < 10
+0000b5f0: 3a0a 2020 2020 2020 2020 2020 2020 7374  :.            st
+0000b600: 7265 616d 2e72 656d 6f76 6528 7472 290a  ream.remove(tr).
+0000b610: 0a20 2020 2072 6574 7572 6e20 7374 7265  .    return stre
+0000b620: 616d 0a0a 0a64 6566 2070 6f72 7469 6f6e  am...def portion
+0000b630: 5f67 6170 7328 7374 7265 616d 2c20 7374  _gaps(stream, st
+0000b640: 6172 7474 696d 653a 206f 6273 7079 2e55  arttime: obspy.U
+0000b650: 5443 4461 7465 5469 6d65 2c20 656e 6474  TCDateTime, endt
+0000b660: 696d 653a 206f 6273 7079 2e55 5443 4461  ime: obspy.UTCDa
+0000b670: 7465 5469 6d65 293a 0a20 2020 2022 2222  teTime):.    """
+0000b680: 0a20 2020 2074 6869 7320 6675 6e63 7469  .    this functi
+0000b690: 6f6e 2074 7261 636b 7320 7468 6520 6761  on tracks the ga
+0000b6a0: 7073 2028 6e70 7473 2920 6672 6f6d 2074  ps (npts) from t
+0000b6b0: 6865 2061 6363 756d 756c 6174 6564 2064  he accumulated d
+0000b6c0: 6966 6665 7265 6e63 6520 6265 7477 6565  ifference betwee
+0000b6d0: 6e20 7374 6172 7474 696d 6520 616e 6420  n starttime and 
+0000b6e0: 656e 6474 696d 650a 2020 2020 6f66 2065  endtime.    of e
+0000b6f0: 6163 6820 7374 7265 616d 2074 7261 6365  ach stream trace
+0000b700: 2e20 6974 2072 656d 6f76 6573 2074 7261  . it removes tra
+0000b710: 6365 2077 6974 6820 6761 7020 6c65 6e67  ce with gap leng
+0000b720: 7468 203e 2033 3025 206f 6620 7472 6163  th > 30% of trac
+0000b730: 6520 7369 7a65 2e0a 2020 2020 5041 5241  e size..    PARA
+0000b740: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
+0000b750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+0000b760: 2020 2020 7374 7265 616d 3a20 6f62 7370      stream: obsp
+0000b770: 7920 7374 7265 616d 206f 626a 6563 740a  y stream object.
+0000b780: 2020 2020 6461 7465 5f69 6e66 6f3a 2064      date_info: d
+0000b790: 6963 7420 6f66 2073 7461 7274 696e 6720  ict of starting 
+0000b7a0: 616e 6420 656e 6469 6e67 2074 696d 6520  and ending time 
+0000b7b0: 6f66 2074 6865 2073 7472 6561 6d0a 0a20  of the stream.. 
+0000b7c0: 2020 2052 4554 5552 4e53 3a0a 2020 2020     RETURNS:.    
+0000b7d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000b7e0: 2d0a 2020 2020 7067 6170 733a 2070 726f  -.    pgaps: pro
+0000b7f0: 706f 7274 696f 6e20 6f66 2067 6170 732f  portion of gaps/
+0000b800: 616c 6c5f 7074 7320 696e 2073 7472 6561  all_pts in strea
+0000b810: 6d0a 2020 2020 2222 220a 2020 2020 2320  m.    """.    # 
+0000b820: 6964 6561 6c20 6475 7261 7469 6f6e 206f  ideal duration o
+0000b830: 6620 6461 7461 0a20 2020 206e 7074 7320  f data.    npts 
+0000b840: 3d20 2865 6e64 7469 6d65 202d 2073 7461  = (endtime - sta
+0000b850: 7274 7469 6d65 2920 2a20 7374 7265 616d  rttime) * stream
+0000b860: 5b30 5d2e 7374 6174 732e 7361 6d70 6c69  [0].stats.sampli
+0000b870: 6e67 5f72 6174 650a 0a20 2020 2070 6761  ng_rate..    pga
+0000b880: 7073 203d 2030 0a20 2020 2023 206c 6f6f  ps = 0.    # loo
+0000b890: 7020 7468 726f 7567 6820 616c 6c20 7472  p through all tr
+0000b8a0: 6163 6520 746f 2061 6363 756d 756c 6174  ace to accumulat
+0000b8b0: 6520 6761 7073 0a20 2020 2066 6f72 2069  e gaps.    for i
+0000b8c0: 6920 696e 2072 616e 6765 286c 656e 2873  i in range(len(s
+0000b8d0: 7472 6561 6d29 202d 2031 293a 0a20 2020  tream) - 1):.   
+0000b8e0: 2020 2020 2070 6761 7073 202b 3d20 2873       pgaps += (s
+0000b8f0: 7472 6561 6d5b 6969 202b 2031 5d2e 7374  tream[ii + 1].st
+0000b900: 6174 732e 7374 6172 7474 696d 6520 2d20  ats.starttime - 
+0000b910: 7374 7265 616d 5b69 695d 2e73 7461 7473  stream[ii].stats
+0000b920: 2e65 6e64 7469 6d65 2920 2a20 7374 7265  .endtime) * stre
+0000b930: 616d 5b69 695d 2e73 7461 7473 2e73 616d  am[ii].stats.sam
+0000b940: 706c 696e 675f 7261 7465 0a20 2020 2069  pling_rate.    i
+0000b950: 6620 6e70 7473 2021 3d20 303a 0a20 2020  f npts != 0:.   
+0000b960: 2020 2020 2070 6761 7073 203d 2070 6761       pgaps = pga
+0000b970: 7073 202f 206e 7074 730a 2020 2020 6966  ps / npts.    if
+0000b980: 206e 7074 7320 3d3d 2030 3a0a 2020 2020   npts == 0:.    
+0000b990: 2020 2020 7067 6170 7320 3d20 310a 2020      pgaps = 1.  
+0000b9a0: 2020 7265 7475 726e 2070 6761 7073 0a0a    return pgaps..
+0000b9b0: 0a40 6a69 7428 2266 6c6f 6174 3332 5b3a  .@jit("float32[:
+0000b9c0: 5d28 666c 6f61 7433 325b 3a5d 2c66 6c6f  ](float32[:],flo
+0000b9d0: 6174 3332 2922 290a 6465 6620 7365 676d  at32)").def segm
+0000b9e0: 656e 745f 696e 7465 7270 6f6c 6174 6528  ent_interpolate(
+0000b9f0: 7369 6731 2c20 6e66 7269 6329 3a0a 2020  sig1, nfric):.  
+0000ba00: 2020 2222 220a 2020 2020 7468 6973 2066    """.    this f
+0000ba10: 756e 6374 696f 6e20 696e 7465 7270 6f6c  unction interpol
+0000ba20: 6174 6573 2074 6865 2064 6174 6120 746f  ates the data to
+0000ba30: 2065 6e73 7572 6520 616c 6c20 706f 696e   ensure all poin
+0000ba40: 7473 206c 6f63 6174 6564 206f 6e20 696e  ts located on in
+0000ba50: 7465 7267 6572 2074 696d 6573 206f 6620  terger times of 
+0000ba60: 7468 650a 2020 2020 7361 6d70 6c69 6e67  the.    sampling
+0000ba70: 2072 6174 6520 2865 2e67 2e2c 2073 7461   rate (e.g., sta
+0000ba80: 7274 7469 6d65 203d 2030 303a 3030 3a30  rttime = 00:00:0
+0000ba90: 302e 3031 352c 2064 656c 7461 203d 2030  0.015, delta = 0
+0000baa0: 2e30 352e 290a 2020 2020 5041 5241 4d45  .05.).    PARAME
+0000bab0: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
+0000bac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bad0: 0a20 2020 2073 6967 313a 2020 7365 6973  .    sig1:  seis
+0000bae0: 6d69 6320 7265 636f 7264 696e 6773 2069  mic recordings i
+0000baf0: 6e20 6120 3144 2061 7272 6179 0a20 2020  n a 1D array.   
+0000bb00: 206e 6672 6963 3a20 7468 6520 616d 6f75   nfric: the amou
+0000bb10: 6e74 206f 6620 7469 6d65 2064 6966 6665  nt of time diffe
+0000bb20: 7265 6e63 6520 6265 7477 6565 6e20 7468  rence between th
+0000bb30: 6520 706f 696e 7420 616e 6420 7468 6520  e point and the 
+0000bb40: 6164 6a61 6365 6e74 2061 7373 756d 6564  adjacent assumed
+0000bb50: 2073 616d 706c 6573 0a20 2020 2052 4554   samples.    RET
+0000bb60: 5552 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d  URNS:.    ------
+0000bb70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000bb80: 0a20 2020 2073 6967 323a 2020 696e 7465  .    sig2:  inte
+0000bb90: 7270 6f6c 6174 6564 2073 6569 736d 6963  rpolated seismic
+0000bba0: 2072 6563 6f72 6469 6e67 7320 6f6e 2074   recordings on t
+0000bbb0: 6865 2073 616d 706c 696e 6720 706f 696e  he sampling poin
+0000bbc0: 7473 0a20 2020 2022 2222 0a20 2020 206e  ts.    """.    n
+0000bbd0: 7074 7320 3d20 6c65 6e28 7369 6731 290a  pts = len(sig1).
+0000bbe0: 2020 2020 7369 6732 203d 206e 702e 7a65      sig2 = np.ze
+0000bbf0: 726f 7328 6e70 7473 2c20 6474 7970 653d  ros(npts, dtype=
+0000bc00: 6e70 2e66 6c6f 6174 3332 290a 0a20 2020  np.float32)..   
+0000bc10: 2023 202d 2d2d 2d69 6e73 7465 6164 206f   # ----instead o
+0000bc20: 6620 7368 6966 7469 6e67 2c20 646f 2061  f shifting, do a
+0000bc30: 2069 6e74 6572 706f 6c61 7469 6f6e 2d2d   interpolation--
+0000bc40: 2d2d 2d2d 0a20 2020 2066 6f72 2069 6920  ----.    for ii 
+0000bc50: 696e 2072 616e 6765 286e 7074 7329 3a0a  in range(npts):.
+0000bc60: 2020 2020 2020 2020 2320 2d2d 2d2d 6465          # ----de
+0000bc70: 616c 2077 6974 6820 6564 6765 732d 2d2d  al with edges---
+0000bc80: 2d2d 0a20 2020 2020 2020 2069 6620 6969  --.        if ii
+0000bc90: 203d 3d20 3020 6f72 2069 6920 3d3d 206e   == 0 or ii == n
+0000bca0: 7074 7320 2d20 313a 0a20 2020 2020 2020  pts - 1:.       
+0000bcb0: 2020 2020 2073 6967 325b 6969 5d20 3d20       sig2[ii] = 
+0000bcc0: 7369 6731 5b69 695d 0a20 2020 2020 2020  sig1[ii].       
+0000bcd0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000bce0: 2020 2023 202d 2d2d 2d2d 2d69 6e74 6572     # ------inter
+0000bcf0: 706f 6c61 7465 2075 7369 6e67 2061 2068  polate using a h
+0000bd00: 6174 2066 756e 6374 696f 6e2d 2d2d 2d2d  at function-----
+0000bd10: 2d0a 2020 2020 2020 2020 2020 2020 7369  -.            si
+0000bd20: 6732 5b69 695d 203d 2028 3120 2d20 6e66  g2[ii] = (1 - nf
+0000bd30: 7269 6329 202a 2073 6967 315b 6969 202b  ric) * sig1[ii +
+0000bd40: 2031 5d20 2b20 6e66 7269 6320 2a20 7369   1] + nfric * si
+0000bd50: 6731 5b69 695d 0a0a 2020 2020 7265 7475  g1[ii]..    retu
+0000bd60: 726e 2073 6967 320a 0a0a 6465 6620 7265  rn sig2...def re
+0000bd70: 7370 5f73 7065 6374 7275 6d28 736f 7572  sp_spectrum(sour
+0000bd80: 6365 2c20 7265 7370 5f66 696c 652c 2064  ce, resp_file, d
+0000bd90: 6f77 6e73 616d 705f 6672 6571 2c20 7072  ownsamp_freq, pr
+0000bda0: 655f 6669 6c74 3d4e 6f6e 6529 3a0a 2020  e_filt=None):.  
+0000bdb0: 2020 2222 220a 2020 2020 7468 6973 2066    """.    this f
+0000bdc0: 756e 6374 696f 6e20 7265 6d6f 7665 7320  unction removes 
+0000bdd0: 7468 6520 696e 7374 7275 6d65 6e74 2072  the instrument r
+0000bde0: 6573 706f 6e73 6520 7573 696e 6720 7265  esponse using re
+0000bdf0: 7370 6f6e 7365 2073 7065 6374 7275 6d20  sponse spectrum 
+0000be00: 6672 6f6d 2065 7661 6c72 6573 702e 0a20  from evalresp.. 
+0000be10: 2020 2074 6865 2072 6573 706f 6e73 6520     the response 
+0000be20: 7370 6563 7472 756d 2069 7320 6576 616c  spectrum is eval
+0000be30: 7561 7465 6420 6261 7365 6420 6f6e 2052  uated based on R
+0000be40: 4553 502f 505a 2066 696c 6573 2062 6566  ESP/PZ files bef
+0000be50: 6f72 6520 696e 7665 7274 6564 2075 7369  ore inverted usi
+0000be60: 6e67 2074 6865 206f 6273 7079 0a20 2020  ng the obspy.   
+0000be70: 2066 756e 6374 696f 6e20 6f66 2069 6e76   function of inv
+0000be80: 6572 745f 7370 6563 7472 756d 2e20 6120  ert_spectrum. a 
+0000be90: 6d6f 6475 6c65 206f 6620 6372 6561 7465  module of create
+0000bea0: 5f72 6573 702e 7079 2069 7320 7072 6f76  _resp.py is prov
+0000beb0: 6964 6564 2069 6e20 6469 7265 6374 6f72  ided in director
+0000bec0: 7920 6f66 2027 6164 6469 7469 6f6e 616c  y of 'additional
+0000bed0: 5f6d 6f64 756c 6573 270a 2020 2020 746f  _modules'.    to
+0000bee0: 2063 7265 6174 6520 7468 6520 7265 7370   create the resp
+0000bef0: 6f6e 7365 2073 7065 6374 7275 6d0a 2020  onse spectrum.  
+0000bf00: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
+0000bf10: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+0000bf20: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2073 6f75  --------.    sou
+0000bf30: 7263 653a 206f 6273 7079 2073 7472 6561  rce: obspy strea
+0000bf40: 6d20 6f62 6a65 6374 206f 6620 7461 7267  m object of targ
+0000bf50: 6574 6564 206e 6f69 7365 2064 6174 610a  eted noise data.
+0000bf60: 2020 2020 7265 7370 5f66 696c 653a 206e      resp_file: n
+0000bf70: 756d 7079 2064 6174 6120 6669 6c65 206f  umpy data file o
+0000bf80: 6620 7265 7370 6f6e 7365 2073 7065 6374  f response spect
+0000bf90: 7275 6d0a 2020 2020 646f 776e 7361 6d70  rum.    downsamp
+0000bfa0: 5f66 7265 713a 2073 616d 706c 696e 6720  _freq: sampling 
+0000bfb0: 7261 7465 206f 6620 7468 6520 736f 7572  rate of the sour
+0000bfc0: 6365 2064 6174 610a 2020 2020 7072 655f  ce data.    pre_
+0000bfd0: 6669 6c74 3a20 7072 652d 6465 6669 6e65  filt: pre-define
+0000bfe0: 6420 6669 6c74 6572 2070 6172 616d 6574  d filter paramet
+0000bff0: 6572 730a 2020 2020 5245 5455 524e 533a  ers.    RETURNS:
+0000c000: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+0000c010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+0000c020: 736f 7572 6365 3a20 6f62 7370 7920 7374  source: obspy st
+0000c030: 7265 616d 206f 626a 6563 7420 6f66 206e  ream object of n
+0000c040: 6f69 7365 2064 6174 6120 7769 7468 2069  oise data with i
+0000c050: 6e73 7472 756d 656e 7420 7265 7370 6f6e  nstrument respon
+0000c060: 7365 2072 656d 6f76 6564 0a20 2020 2022  se removed.    "
+0000c070: 2222 0a20 2020 2023 202d 2d2d 2d2d 2d2d  "".    # -------
+0000c080: 2d72 6573 705f 6669 6c65 2069 7320 7468  -resp_file is th
+0000c090: 6520 696e 7665 7274 6564 2073 7065 6374  e inverted spect
+0000c0a0: 7275 6d20 7265 7370 6f6e 7365 2d2d 2d2d  rum response----
+0000c0b0: 2d2d 2d2d 2d0a 2020 2020 7265 7370 7a20  -----.    respz 
+0000c0c0: 3d20 6e70 2e6c 6f61 6428 7265 7370 5f66  = np.load(resp_f
+0000c0d0: 696c 6529 0a20 2020 206e 7265 7370 7a20  ile).    nrespz 
+0000c0e0: 3d20 7265 7370 7a5b 315d 5b3a 5d0a 2020  = respz[1][:].  
+0000c0f0: 2020 7370 6563 5f66 7265 7120 3d20 6d61    spec_freq = ma
+0000c100: 7828 7265 7370 7a5b 305d 290a 0a20 2020  x(respz[0])..   
+0000c110: 2023 202d 2d2d 2d2d 2d2d 6f6e 2063 7572   # -------on cur
+0000c120: 7265 6e74 2074 7261 6365 2d2d 2d2d 2d2d  rent trace------
+0000c130: 2d2d 2d2d 0a20 2020 206e 6666 7420 3d20  ----.    nfft = 
+0000c140: 5f6e 7074 7332 6e66 6674 2873 6f75 7263  _npts2nfft(sourc
+0000c150: 655b 305d 2e73 7461 7473 2e6e 7074 7329  e[0].stats.npts)
+0000c160: 0a20 2020 2073 7073 203d 2069 6e74 2873  .    sps = int(s
+0000c170: 6f75 7263 655b 305d 2e73 7461 7473 2e73  ource[0].stats.s
+0000c180: 616d 706c 696e 675f 7261 7465 290a 0a20  ampling_rate).. 
+0000c190: 2020 2023 202d 2d2d 2d2d 2d2d 2d2d 646f     # ---------do
+0000c1a0: 2074 6865 2069 6e74 6572 706f 6c61 7469   the interpolati
+0000c1b0: 6f6e 2069 6620 6e65 6564 6564 2d2d 2d2d  on if needed----
+0000c1c0: 2d2d 2d2d 0a20 2020 2069 6620 7370 6563  ----.    if spec
+0000c1d0: 5f66 7265 7120 3c20 302e 3520 2a20 7370  _freq < 0.5 * sp
+0000c1e0: 733a 0a20 2020 2020 2020 2072 6169 7365  s:.        raise
+0000c1f0: 2056 616c 7565 4572 726f 7228 2273 7065   ValueError("spe
+0000c200: 6374 7275 6d20 6669 6c65 2068 6173 2070  ctrum file has p
+0000c210: 6561 6b20 6672 6571 2073 6d61 6c6c 6572  eak freq smaller
+0000c220: 2074 6861 6e20 7468 6520 6461 7461 2c20   than the data, 
+0000c230: 6162 6f72 7421 2229 0a20 2020 2065 6c73  abort!").    els
+0000c240: 653a 0a20 2020 2020 2020 2069 6e64 7820  e:.        indx 
+0000c250: 3d20 6e70 2e77 6865 7265 2872 6573 707a  = np.where(respz
+0000c260: 5b30 5d20 3c3d 2030 2e35 202a 2073 7073  [0] <= 0.5 * sps
+0000c270: 290a 2020 2020 2020 2020 6e66 7265 7120  ).        nfreq 
+0000c280: 3d20 6e70 2e6c 696e 7370 6163 6528 302c  = np.linspace(0,
+0000c290: 2030 2e35 202a 2073 7073 2c20 6e66 6674   0.5 * sps, nfft
+0000c2a0: 202f 2f20 3220 2b20 3129 0a20 2020 2020   // 2 + 1).     
+0000c2b0: 2020 206e 7265 7370 7a20 3d20 6e70 2e69     nrespz = np.i
+0000c2c0: 6e74 6572 7028 6e66 7265 712c 206e 702e  nterp(nfreq, np.
+0000c2d0: 7265 616c 2872 6573 707a 5b30 5d5b 696e  real(respz[0][in
+0000c2e0: 6478 5d29 2c20 7265 7370 7a5b 315d 5b69  dx]), respz[1][i
+0000c2f0: 6e64 785d 290a 0a20 2020 2023 202d 2d2d  ndx])..    # ---
+0000c300: 2d64 6f20 696e 7465 7270 6f6c 6174 696f  -do interpolatio
+0000c310: 6e20 6966 206e 6563 6573 7361 7279 2d2d  n if necessary--
+0000c320: 2d2d 2d0a 2020 2020 736f 7572 6365 5f73  ---.    source_s
+0000c330: 7065 6374 203d 206e 702e 6666 742e 7266  pect = np.fft.rf
+0000c340: 6674 2873 6f75 7263 655b 305d 2e64 6174  ft(source[0].dat
+0000c350: 612c 206e 3d6e 6666 7429 0a0a 2020 2020  a, n=nfft)..    
+0000c360: 2320 2d2d 2d2d 2d6e 7265 7370 7a20 6973  # -----nrespz is
+0000c370: 2069 6e76 6572 7365 6420 2877 6174 6572   inversed (water
+0000c380: 2d6c 6576 656c 6564 2920 7370 6563 7472  -leveled) spectr
+0000c390: 756d 2d2d 2d2d 2d0a 2020 2020 736f 7572  um-----.    sour
+0000c3a0: 6365 5f73 7065 6374 202a 3d20 6e72 6573  ce_spect *= nres
+0000c3b0: 707a 0a20 2020 2073 6f75 7263 655b 305d  pz.    source[0]
+0000c3c0: 2e64 6174 6120 3d20 6e70 2e66 6674 2e69  .data = np.fft.i
+0000c3d0: 7266 6674 2873 6f75 7263 655f 7370 6563  rfft(source_spec
+0000c3e0: 7429 5b30 203a 2073 6f75 7263 655b 305d  t)[0 : source[0]
+0000c3f0: 2e73 7461 7473 2e6e 7074 735d 0a0a 2020  .stats.npts]..  
+0000c400: 2020 6966 2070 7265 5f66 696c 7420 6973    if pre_filt is
+0000c410: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000c420: 2020 2073 6f75 7263 655b 305d 2e64 6174     source[0].dat
+0000c430: 6120 3d20 6e70 2e66 6c6f 6174 3332 280a  a = np.float32(.
+0000c440: 2020 2020 2020 2020 2020 2020 6261 6e64              band
+0000c450: 7061 7373 280a 2020 2020 2020 2020 2020  pass(.          
+0000c460: 2020 2020 2020 736f 7572 6365 5b30 5d2e        source[0].
+0000c470: 6461 7461 2c0a 2020 2020 2020 2020 2020  data,.          
+0000c480: 2020 2020 2020 7072 655f 6669 6c74 5b30        pre_filt[0
+0000c490: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+0000c4a0: 2020 2070 7265 5f66 696c 745b 2d31 5d2c     pre_filt[-1],
+0000c4b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c4c0: 2064 663d 7370 732c 0a20 2020 2020 2020   df=sps,.       
+0000c4d0: 2020 2020 2020 2020 2063 6f72 6e65 7273           corners
+0000c4e0: 3d34 2c0a 2020 2020 2020 2020 2020 2020  =4,.            
+0000c4f0: 2020 2020 7a65 726f 7068 6173 653d 5472      zerophase=Tr
+0000c500: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+0000c510: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+0000c520: 2072 6574 7572 6e20 736f 7572 6365 0a0a   return source..
+0000c530: 0a64 6566 206d 6164 2861 7272 293a 0a20  .def mad(arr):. 
+0000c540: 2020 2022 2222 0a20 2020 204d 6564 6961     """.    Media
+0000c550: 6e20 4162 736f 6c75 7465 2044 6576 6961  n Absolute Devia
+0000c560: 7469 6f6e 3a20 4d41 4420 3d20 6d65 6469  tion: MAD = medi
+0000c570: 616e 287c 5869 2d20 6d65 6469 616e 2858  an(|Xi- median(X
+0000c580: 297c 290a 2020 2020 5041 5241 4d45 5445  )|).    PARAMETE
+0000c590: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
+0000c5a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+0000c5b0: 6172 723a 206e 756d 7079 2e6e 6461 7272  arr: numpy.ndarr
+0000c5c0: 6179 2c20 7365 6973 6d69 6320 7472 6163  ay, seismic trac
+0000c5d0: 6520 6461 7461 2061 7272 6179 0a20 2020  e data array.   
+0000c5e0: 2052 4554 5552 4e53 3a0a 2020 2020 6461   RETURNS:.    da
+0000c5f0: 7461 3a20 4d65 6469 616e 2041 6273 6f6c  ta: Median Absol
+0000c600: 7574 6520 4465 7669 6174 696f 6e20 6f66  ute Deviation of
+0000c610: 2064 6174 610a 2020 2020 2222 220a 2020   data.    """.  
+0000c620: 2020 6966 206e 6f74 206e 702e 6d61 2e69    if not np.ma.i
+0000c630: 735f 6d61 736b 6564 2861 7272 293a 0a20  s_masked(arr):. 
+0000c640: 2020 2020 2020 206d 6564 203d 206e 702e         med = np.
+0000c650: 6d65 6469 616e 2861 7272 290a 2020 2020  median(arr).    
+0000c660: 2020 2020 6461 7461 203d 206e 702e 6d65      data = np.me
+0000c670: 6469 616e 286e 702e 6162 7328 6172 7220  dian(np.abs(arr 
+0000c680: 2d20 6d65 6429 290a 2020 2020 656c 7365  - med)).    else
+0000c690: 3a0a 2020 2020 2020 2020 6d65 6420 3d20  :.        med = 
+0000c6a0: 6e70 2e6d 612e 6d65 6469 616e 2861 7272  np.ma.median(arr
+0000c6b0: 290a 2020 2020 2020 2020 6461 7461 203d  ).        data =
+0000c6c0: 206e 702e 6d61 2e6d 6564 6961 6e28 6e70   np.ma.median(np
+0000c6d0: 2e6d 612e 6162 7328 6172 7220 2d20 6d65  .ma.abs(arr - me
+0000c6e0: 6429 290a 2020 2020 7265 7475 726e 2064  d)).    return d
+0000c6f0: 6174 610a 0a0a 6465 6620 6465 7472 656e  ata...def detren
+0000c700: 6428 6461 7461 293a 0a20 2020 2022 2222  d(data):.    """
+0000c710: 0a20 2020 2074 6869 7320 6675 6e63 7469  .    this functi
+0000c720: 6f6e 2072 656d 6f76 6573 2074 6865 2073  on removes the s
+0000c730: 6967 6e61 6c20 7472 656e 6420 6261 7365  ignal trend base
+0000c740: 6420 6f6e 2051 5220 6465 636f 6d70 6f73  d on QR decompos
+0000c750: 696f 6e0a 2020 2020 4e4f 5445 3a20 5152  ion.    NOTE: QR
+0000c760: 2069 7320 6120 6c6f 7420 6661 7374 6572   is a lot faster
+0000c770: 2074 6861 6e20 7468 6520 6c65 6173 7420   than the least 
+0000c780: 7371 7561 7265 2069 6e76 6572 7369 6f6e  square inversion
+0000c790: 2075 7365 6420 6279 0a20 2020 2073 6369   used by.    sci
+0000c7a0: 7079 2028 616c 736f 2069 6e20 6f62 7370  py (also in obsp
+0000c7b0: 7929 2e0a 2020 2020 5041 5241 4d45 5445  y)..    PARAMETE
+0000c7c0: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
+0000c7d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0000c7e0: 2020 6461 7461 3a20 696e 7075 7420 6461    data: input da
+0000c7f0: 7461 206d 6174 7269 780a 2020 2020 5245  ta matrix.    RE
+0000c800: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
+0000c810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000c820: 0a20 2020 2064 6174 613a 2064 6174 6120  .    data: data 
+0000c830: 6d61 7472 6978 2077 6974 6820 7472 656e  matrix with tren
+0000c840: 6420 7265 6d6f 7665 640a 2020 2020 2222  d removed.    ""
+0000c850: 220a 2020 2020 2320 6e64 6174 6120 3d20  ".    # ndata = 
+0000c860: 6e70 2e7a 6572 6f73 2873 6861 7065 3d64  np.zeros(shape=d
+0000c870: 6174 612e 7368 6170 652c 6474 7970 653d  ata.shape,dtype=
+0000c880: 6461 7461 2e64 7479 7065 290a 2020 2020  data.dtype).    
+0000c890: 6966 2064 6174 612e 6e64 696d 203d 3d20  if data.ndim == 
+0000c8a0: 313a 0a20 2020 2020 2020 206e 7074 7320  1:.        npts 
+0000c8b0: 3d20 6461 7461 2e73 6861 7065 5b30 5d0a  = data.shape[0].
+0000c8c0: 2020 2020 2020 2020 5820 3d20 6e70 2e6f          X = np.o
+0000c8d0: 6e65 7328 286e 7074 732c 2032 2929 0a20  nes((npts, 2)). 
+0000c8e0: 2020 2020 2020 2058 5b3a 2c20 305d 203d         X[:, 0] =
+0000c8f0: 206e 702e 6172 616e 6765 2830 2c20 6e70   np.arange(0, np
+0000c900: 7473 2920 2f20 6e70 7473 0a20 2020 2020  ts) / npts.     
+0000c910: 2020 2051 2c20 5220 3d20 6e70 2e6c 696e     Q, R = np.lin
+0000c920: 616c 672e 7172 2858 290a 2020 2020 2020  alg.qr(X).      
+0000c930: 2020 7271 203d 206e 702e 646f 7428 6e70    rq = np.dot(np
+0000c940: 2e6c 696e 616c 672e 696e 7628 5229 2c20  .linalg.inv(R), 
+0000c950: 512e 7472 616e 7370 6f73 6528 2929 0a20  Q.transpose()). 
+0000c960: 2020 2020 2020 2063 6f65 6666 203d 206e         coeff = n
+0000c970: 702e 646f 7428 7271 2c20 6461 7461 290a  p.dot(rq, data).
+0000c980: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
+0000c990: 6174 6120 2d20 6e70 2e64 6f74 2858 2c20  ata - np.dot(X, 
+0000c9a0: 636f 6566 6629 0a20 2020 2065 6c69 6620  coeff).    elif 
+0000c9b0: 6461 7461 2e6e 6469 6d20 3d3d 2032 3a0a  data.ndim == 2:.
+0000c9c0: 2020 2020 2020 2020 6e70 7473 203d 2064          npts = d
+0000c9d0: 6174 612e 7368 6170 655b 315d 0a20 2020  ata.shape[1].   
+0000c9e0: 2020 2020 2058 203d 206e 702e 6f6e 6573       X = np.ones
+0000c9f0: 2828 6e70 7473 2c20 3229 290a 2020 2020  ((npts, 2)).    
+0000ca00: 2020 2020 585b 3a2c 2030 5d20 3d20 6e70      X[:, 0] = np
+0000ca10: 2e61 7261 6e67 6528 302c 206e 7074 7329  .arange(0, npts)
+0000ca20: 202f 206e 7074 730a 2020 2020 2020 2020   / npts.        
+0000ca30: 512c 2052 203d 206e 702e 6c69 6e61 6c67  Q, R = np.linalg
+0000ca40: 2e71 7228 5829 0a20 2020 2020 2020 2072  .qr(X).        r
+0000ca50: 7120 3d20 6e70 2e64 6f74 286e 702e 6c69  q = np.dot(np.li
+0000ca60: 6e61 6c67 2e69 6e76 2852 292c 2051 2e74  nalg.inv(R), Q.t
+0000ca70: 7261 6e73 706f 7365 2829 290a 2020 2020  ranspose()).    
+0000ca80: 2020 2020 666f 7220 6969 2069 6e20 7261      for ii in ra
+0000ca90: 6e67 6528 6461 7461 2e73 6861 7065 5b30  nge(data.shape[0
+0000caa0: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
+0000cab0: 636f 6566 6620 3d20 6e70 2e64 6f74 2872  coeff = np.dot(r
+0000cac0: 712c 2064 6174 615b 6969 5d29 0a20 2020  q, data[ii]).   
+0000cad0: 2020 2020 2020 2020 2064 6174 615b 6969           data[ii
+0000cae0: 5d20 3d20 6461 7461 5b69 695d 202d 206e  ] = data[ii] - n
+0000caf0: 702e 646f 7428 582c 2063 6f65 6666 290a  p.dot(X, coeff).
+0000cb00: 2020 2020 7265 7475 726e 2064 6174 610a      return data.
+0000cb10: 0a0a 6465 6620 6465 6d65 616e 2864 6174  ..def demean(dat
+0000cb20: 6129 3a0a 2020 2020 2222 220a 2020 2020  a):.    """.    
+0000cb30: 7468 6973 2066 756e 6374 696f 6e20 7265  this function re
+0000cb40: 6d6f 7665 2074 6865 206d 6561 6e20 6f66  move the mean of
+0000cb50: 2074 6865 2073 6967 6e61 6c0a 2020 2020   the signal.    
+0000cb60: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
+0000cb70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000cb80: 2d2d 2d2d 2d0a 2020 2020 6461 7461 3a20  -----.    data: 
+0000cb90: 696e 7075 7420 6461 7461 206d 6174 7269  input data matri
+0000cba0: 780a 2020 2020 5245 5455 524e 533a 0a20  x.    RETURNS:. 
+0000cbb0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+0000cbc0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
+0000cbd0: 613a 2064 6174 6120 6d61 7472 6978 2077  a: data matrix w
+0000cbe0: 6974 6820 6d65 616e 2072 656d 6f76 6564  ith mean removed
+0000cbf0: 0a20 2020 2022 2222 0a20 2020 2023 206e  .    """.    # n
+0000cc00: 6461 7461 203d 206e 702e 7a65 726f 7328  data = np.zeros(
+0000cc10: 7368 6170 653d 6461 7461 2e73 6861 7065  shape=data.shape
+0000cc20: 2c64 7479 7065 3d64 6174 612e 6474 7970  ,dtype=data.dtyp
+0000cc30: 6529 0a20 2020 2069 6620 6461 7461 2e6e  e).    if data.n
+0000cc40: 6469 6d20 3d3d 2031 3a0a 2020 2020 2020  dim == 1:.      
+0000cc50: 2020 6461 7461 203d 2064 6174 6120 2d20    data = data - 
+0000cc60: 6e70 2e6d 6561 6e28 6461 7461 290a 2020  np.mean(data).  
+0000cc70: 2020 656c 6966 2064 6174 612e 6e64 696d    elif data.ndim
+0000cc80: 203d 3d20 323a 0a20 2020 2020 2020 2066   == 2:.        f
+0000cc90: 6f72 2069 6920 696e 2072 616e 6765 2864  or ii in range(d
+0000cca0: 6174 612e 7368 6170 655b 305d 293a 0a20  ata.shape[0]):. 
+0000ccb0: 2020 2020 2020 2020 2020 2064 6174 615b             data[
+0000ccc0: 6969 5d20 3d20 6461 7461 5b69 695d 202d  ii] = data[ii] -
+0000ccd0: 206e 702e 6d65 616e 2864 6174 615b 6969   np.mean(data[ii
+0000cce0: 5d29 0a20 2020 2072 6574 7572 6e20 6461  ]).    return da
+0000ccf0: 7461 0a0a 0a64 6566 2074 6170 6572 2864  ta...def taper(d
+0000cd00: 6174 6129 3a0a 2020 2020 2222 220a 2020  ata):.    """.  
+0000cd10: 2020 7468 6973 2066 756e 6374 696f 6e20    this function 
+0000cd20: 6170 706c 6965 7320 6120 636f 7369 6e65  applies a cosine
+0000cd30: 2074 6170 6572 2075 7369 6e67 206f 6273   taper using obs
+0000cd40: 7079 2066 756e 6374 696f 6e73 0a20 2020  py functions.   
+0000cd50: 2050 4152 414d 4554 4552 533a 0a20 2020   PARAMETERS:.   
+0000cd60: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000cd70: 2d2d 2d2d 2d2d 0a20 2020 2064 6174 613a  ------.    data:
+0000cd80: 2069 6e70 7574 2064 6174 6120 6d61 7472   input data matr
+0000cd90: 6978 0a20 2020 2052 4554 5552 4e53 3a0a  ix.    RETURNS:.
+0000cda0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+0000cdb0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6461  ---------.    da
+0000cdc0: 7461 3a20 6461 7461 206d 6174 7269 7820  ta: data matrix 
+0000cdd0: 7769 7468 2074 6170 6572 2061 7070 6c69  with taper appli
+0000cde0: 6564 0a20 2020 2022 2222 0a20 2020 2023  ed.    """.    #
+0000cdf0: 206e 6461 7461 203d 206e 702e 7a65 726f   ndata = np.zero
+0000ce00: 7328 7368 6170 653d 6461 7461 2e73 6861  s(shape=data.sha
+0000ce10: 7065 2c64 7479 7065 3d64 6174 612e 6474  pe,dtype=data.dt
+0000ce20: 7970 6529 0a20 2020 2069 6620 6461 7461  ype).    if data
+0000ce30: 2e6e 6469 6d20 3d3d 2031 3a0a 2020 2020  .ndim == 1:.    
+0000ce40: 2020 2020 6e70 7473 203d 2064 6174 612e      npts = data.
+0000ce50: 7368 6170 655b 305d 0a20 2020 2020 2020  shape[0].       
+0000ce60: 2023 2077 696e 646f 7720 6c65 6e67 7468   # window length
+0000ce70: 0a20 2020 2020 2020 2069 6620 6e70 7473  .        if npts
+0000ce80: 202a 2030 2e30 3520 3e20 3230 3a0a 2020   * 0.05 > 20:.  
+0000ce90: 2020 2020 2020 2020 2020 776c 656e 203d            wlen =
+0000cea0: 2032 300a 2020 2020 2020 2020 656c 7365   20.        else
+0000ceb0: 3a0a 2020 2020 2020 2020 2020 2020 776c  :.            wl
+0000cec0: 656e 203d 206e 7074 7320 2a20 302e 3035  en = npts * 0.05
+0000ced0: 0a20 2020 2020 2020 2023 2074 6170 6572  .        # taper
+0000cee0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
+0000cef0: 6675 6e63 203d 205f 6765 745f 6675 6e63  func = _get_func
+0000cf00: 7469 6f6e 5f66 726f 6d5f 656e 7472 795f  tion_from_entry_
+0000cf10: 706f 696e 7428 2274 6170 6572 222c 2022  point("taper", "
+0000cf20: 6861 6e6e 2229 0a20 2020 2020 2020 2069  hann").        i
+0000cf30: 6620 3220 2a20 776c 656e 203d 3d20 6e70  f 2 * wlen == np
+0000cf40: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+0000cf50: 7461 7065 725f 7369 6465 7320 3d20 6675  taper_sides = fu
+0000cf60: 6e63 2832 202a 2077 6c65 6e29 0a20 2020  nc(2 * wlen).   
+0000cf70: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000cf80: 2020 2020 2020 2074 6170 6572 5f73 6964         taper_sid
+0000cf90: 6573 203d 2066 756e 6328 3220 2a20 776c  es = func(2 * wl
+0000cfa0: 656e 202b 2031 290a 2020 2020 2020 2020  en + 1).        
+0000cfb0: 2320 7461 7065 7220 7769 6e64 6f77 0a20  # taper window. 
+0000cfc0: 2020 2020 2020 2077 696e 203d 206e 702e         win = np.
+0000cfd0: 6873 7461 636b 280a 2020 2020 2020 2020  hstack(.        
+0000cfe0: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+0000cff0: 2020 2020 2020 7461 7065 725f 7369 6465        taper_side
+0000d000: 735b 3a77 6c65 6e5d 2c0a 2020 2020 2020  s[:wlen],.      
+0000d010: 2020 2020 2020 2020 2020 6e70 2e6f 6e65            np.one
+0000d020: 7328 6e70 7473 202d 2032 202a 2077 6c65  s(npts - 2 * wle
+0000d030: 6e29 2c0a 2020 2020 2020 2020 2020 2020  n),.            
+0000d040: 2020 2020 7461 7065 725f 7369 6465 735b      taper_sides[
+0000d050: 6c65 6e28 7461 7065 725f 7369 6465 7329  len(taper_sides)
+0000d060: 202d 2077 6c65 6e20 3a5d 2c0a 2020 2020   - wlen :],.    
+0000d070: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000d080: 2020 290a 2020 2020 2020 2020 6461 7461    ).        data
+0000d090: 202a 3d20 7769 6e0a 2020 2020 656c 6966   *= win.    elif
+0000d0a0: 2064 6174 612e 6e64 696d 203d 3d20 323a   data.ndim == 2:
+0000d0b0: 0a20 2020 2020 2020 206e 7074 7320 3d20  .        npts = 
+0000d0c0: 6461 7461 2e73 6861 7065 5b31 5d0a 2020  data.shape[1].  
+0000d0d0: 2020 2020 2020 2320 7769 6e64 6f77 206c        # window l
+0000d0e0: 656e 6774 680a 2020 2020 2020 2020 6966  ength.        if
+0000d0f0: 206e 7074 7320 2a20 302e 3035 203e 2032   npts * 0.05 > 2
+0000d100: 303a 0a20 2020 2020 2020 2020 2020 2077  0:.            w
+0000d110: 6c65 6e20 3d20 3230 0a20 2020 2020 2020  len = 20.       
+0000d120: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d130: 2020 2077 6c65 6e20 3d20 6e70 7473 202a     wlen = npts *
+0000d140: 2030 2e30 350a 2020 2020 2020 2020 2320   0.05.        # 
+0000d150: 7461 7065 7220 7661 6c75 6573 0a20 2020  taper values.   
+0000d160: 2020 2020 2066 756e 6320 3d20 5f67 6574       func = _get
+0000d170: 5f66 756e 6374 696f 6e5f 6672 6f6d 5f65  _function_from_e
+0000d180: 6e74 7279 5f70 6f69 6e74 2822 7461 7065  ntry_point("tape
+0000d190: 7222 2c20 2268 616e 6e22 290a 2020 2020  r", "hann").    
+0000d1a0: 2020 2020 6966 2032 202a 2077 6c65 6e20      if 2 * wlen 
+0000d1b0: 3d3d 206e 7074 733a 0a20 2020 2020 2020  == npts:.       
+0000d1c0: 2020 2020 2074 6170 6572 5f73 6964 6573       taper_sides
+0000d1d0: 203d 2066 756e 6328 3220 2a20 776c 656e   = func(2 * wlen
+0000d1e0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+0000d1f0: 2020 2020 2020 2020 2020 2020 7461 7065              tape
+0000d200: 725f 7369 6465 7320 3d20 6675 6e63 2832  r_sides = func(2
+0000d210: 202a 2077 6c65 6e20 2b20 3129 0a20 2020   * wlen + 1).   
+0000d220: 2020 2020 2023 2074 6170 6572 2077 696e       # taper win
+0000d230: 646f 770a 2020 2020 2020 2020 7769 6e20  dow.        win 
+0000d240: 3d20 6e70 2e68 7374 6163 6b28 0a20 2020  = np.hstack(.   
+0000d250: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
+0000d260: 2020 2020 2020 2020 2020 2074 6170 6572             taper
+0000d270: 5f73 6964 6573 5b3a 776c 656e 5d2c 0a20  _sides[:wlen],. 
+0000d280: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000d290: 702e 6f6e 6573 286e 7074 7320 2d20 3220  p.ones(npts - 2 
+0000d2a0: 2a20 776c 656e 292c 0a20 2020 2020 2020  * wlen),.       
+0000d2b0: 2020 2020 2020 2020 2074 6170 6572 5f73           taper_s
+0000d2c0: 6964 6573 5b6c 656e 2874 6170 6572 5f73  ides[len(taper_s
+0000d2d0: 6964 6573 2920 2d20 776c 656e 203a 5d2c  ides) - wlen :],
+0000d2e0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000d2f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000d300: 2066 6f72 2069 6920 696e 2072 616e 6765   for ii in range
+0000d310: 2864 6174 612e 7368 6170 655b 305d 293a  (data.shape[0]):
+0000d320: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+0000d330: 615b 6969 5d20 2a3d 2077 696e 0a20 2020  a[ii] *= win.   
+0000d340: 2072 6574 7572 6e20 6461 7461 0a0a 0a23   return data...#
+0000d350: 2040 6a69 7428 6e6f 7079 7468 6f6e 203d   @jit(nopython =
+0000d360: 2054 7275 6529 0a0a 0a23 2063 6861 6e67   True)...# chang
+0000d370: 6520 7468 6520 6d6f 7669 6e67 2061 7665  e the moving ave
+0000d380: 7261 6765 2063 616c 6375 6c61 7469 6f6e  rage calculation
+0000d390: 2074 6f20 7461 6b65 2061 7320 696e 7075   to take as inpu
+0000d3a0: 7420 4e20 7468 6520 6675 6c6c 2077 696e  t N the full win
+0000d3b0: 646f 7720 6c65 6e67 7468 2074 6f20 736d  dow length to sm
+0000d3c0: 6f6f 7468 0a64 6566 206d 6f76 696e 675f  ooth.def moving_
+0000d3d0: 6176 6528 412c 204e 293a 0a20 2020 2022  ave(A, N):.    "
+0000d3e0: 2222 0a20 2020 2041 6c74 6572 6e61 7469  "".    Alternati
+0000d3f0: 7665 2066 756e 6374 696f 6e20 666f 7220  ve function for 
+0000d400: 6d6f 7669 6e67 2061 7665 7261 6765 2066  moving average f
+0000d410: 6f72 2061 6e20 6172 7261 792e 0a20 2020  or an array..   
+0000d420: 2050 4152 414d 4554 4552 533a 0a20 2020   PARAMETERS:.   
+0000d430: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000d440: 2d2d 2d2d 2d2d 0a20 2020 2041 3a20 312d  ------.    A: 1-
+0000d450: 4420 6172 7261 7920 6f66 2064 6174 6120  D array of data 
+0000d460: 746f 2062 6520 736d 6f6f 7468 6564 0a20  to be smoothed. 
+0000d470: 2020 204e 3a20 696e 7465 6765 722c 2069     N: integer, i
+0000d480: 7420 6465 6669 6e65 7320 7468 6520 6675  t defines the fu
+0000d490: 6c6c 2121 2077 696e 646f 7720 6c65 6e67  ll!! window leng
+0000d4a0: 7468 2074 6f20 736d 6f6f 7468 0a20 2020  th to smooth.   
+0000d4b0: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
+0000d4c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d4d0: 2d2d 2d0a 2020 2020 423a 2031 2d44 2061  ---.    B: 1-D a
+0000d4e0: 7272 6179 2077 6974 6820 736d 6f6f 7468  rray with smooth
+0000d4f0: 6564 2064 6174 610a 2020 2020 2222 220a  ed data.    """.
+0000d500: 2020 2020 2320 6465 6669 6e65 7320 616e      # defines an
+0000d510: 2061 7272 6179 2077 6974 6820 4e20 6578   array with N ex
+0000d520: 7472 6120 7361 6d70 6c65 7320 6174 2065  tra samples at e
+0000d530: 6974 6865 7220 7369 6465 0a20 2020 2074  ither side.    t
+0000d540: 656d 7020 3d20 6e70 2e7a 6572 6f73 286c  emp = np.zeros(l
+0000d550: 656e 2841 2920 2b20 3220 2a20 4e29 0a20  en(A) + 2 * N). 
+0000d560: 2020 2023 2073 6574 2074 6865 2063 656e     # set the cen
+0000d570: 7472 616c 2070 6f72 7469 6f6e 206f 6620  tral portion of 
+0000d580: 7468 6520 6172 7261 7920 746f 2041 0a20  the array to A. 
+0000d590: 2020 2074 656d 705b 4e3a 2d4e 5d20 3d20     temp[N:-N] = 
+0000d5a0: 410a 2020 2020 2320 6c65 6164 696e 6720  A.    # leading 
+0000d5b0: 7361 6d70 6c65 733a 2065 7175 616c 2074  samples: equal t
+0000d5c0: 6f20 6669 7273 7420 7361 6d70 6c65 206f  o first sample o
+0000d5d0: 6620 6163 7475 616c 2061 7272 6179 0a20  f actual array. 
+0000d5e0: 2020 2074 656d 705b 303a 4e5d 203d 2074     temp[0:N] = t
+0000d5f0: 656d 705b 4e5d 0a20 2020 2023 2074 7261  emp[N].    # tra
+0000d600: 696c 696e 6720 7361 6d70 6c65 733a 2045  iling samples: E
+0000d610: 7175 616c 2074 6f20 6c61 7374 2073 616d  qual to last sam
+0000d620: 706c 6520 6f66 2061 6374 7561 6c20 6172  ple of actual ar
+0000d630: 7261 790a 2020 2020 7465 6d70 5b2d 4e3a  ray.    temp[-N:
+0000d640: 5d20 3d20 7465 6d70 5b2d 4e20 2d20 315d  ] = temp[-N - 1]
+0000d650: 0a20 2020 2023 2063 6f6e 766f 6c76 6520  .    # convolve 
+0000d660: 7769 7468 2061 2062 6f78 6361 7220 616e  with a boxcar an
+0000d670: 6420 6e6f 726d 616c 697a 652c 2061 6e64  d normalize, and
+0000d680: 2075 7365 206f 6e6c 7920 6365 6e74 7261   use only centra
+0000d690: 6c20 706f 7274 696f 6e20 6f66 2074 6865  l portion of the
+0000d6a0: 2072 6573 756c 740a 2020 2020 2320 7769   result.    # wi
+0000d6b0: 7468 206c 656e 6774 6820 6571 7561 6c20  th length equal 
+0000d6c0: 746f 2074 6865 206f 7269 6769 6e61 6c20  to the original 
+0000d6d0: 6172 7261 792c 2064 6973 6361 7264 696e  array, discardin
+0000d6e0: 6720 7468 6520 6164 6465 6420 6c65 6164  g the added lead
+0000d6f0: 696e 6720 616e 6420 7472 6169 6c69 6e67  ing and trailing
+0000d700: 2073 616d 706c 6573 0a20 2020 2042 203d   samples.    B =
+0000d710: 206e 702e 636f 6e76 6f6c 7665 2874 656d   np.convolve(tem
+0000d720: 702c 206e 702e 6f6e 6573 284e 2920 2f20  p, np.ones(N) / 
+0000d730: 4e2c 206d 6f64 653d 2273 616d 6522 295b  N, mode="same")[
+0000d740: 4e3a 2d4e 5d0a 2020 2020 7265 7475 726e  N:-N].    return
+0000d750: 2042 0a0a 0a23 2063 6861 6e67 6520 7468   B...# change th
+0000d760: 6520 6d6f 7669 6e67 2061 7665 7261 6765  e moving average
+0000d770: 2063 616c 6375 6c61 7469 6f6e 2074 6f20   calculation to 
+0000d780: 7461 6b65 2061 7320 696e 7075 7420 4e20  take as input N 
+0000d790: 7468 6520 6675 6c6c 2077 696e 646f 7720  the full window 
+0000d7a0: 6c65 6e67 7468 2074 6f20 736d 6f6f 7468  length to smooth
+0000d7b0: 0a64 6566 206d 6f76 696e 675f 6176 655f  .def moving_ave_
+0000d7c0: 3244 2841 2c20 4e29 3a0a 2020 2020 2222  2D(A, N):.    ""
+0000d7d0: 220a 2020 2020 416c 7465 726e 6174 6976  ".    Alternativ
+0000d7e0: 6520 6675 6e63 7469 6f6e 2066 6f72 206d  e function for m
+0000d7f0: 6f76 696e 6720 6176 6572 6167 6520 666f  oving average fo
+0000d800: 7220 616e 2061 7272 6179 2e0a 2020 2020  r an array..    
+0000d810: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
+0000d820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d830: 2d2d 2d2d 2d0a 2020 2020 413a 2032 2d44  -----.    A: 2-D
+0000d840: 2061 7272 6179 206f 6620 6461 7461 2074   array of data t
+0000d850: 6f20 6265 2073 6d6f 6f74 6865 640a 2020  o be smoothed.  
+0000d860: 2020 4e3a 2069 6e74 6567 6572 2c20 6974    N: integer, it
+0000d870: 2064 6566 696e 6573 2074 6865 2066 756c   defines the ful
+0000d880: 6c21 2120 7769 6e64 6f77 206c 656e 6774  l!! window lengt
+0000d890: 6820 746f 2073 6d6f 6f74 680a 2020 2020  h to smooth.    
+0000d8a0: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
+0000d8b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000d8c0: 2d2d 0a20 2020 2042 3a20 322d 4420 6172  --.    B: 2-D ar
+0000d8d0: 7261 7920 7769 7468 2073 6d6f 6f74 6865  ray with smoothe
+0000d8e0: 6420 6461 7461 0a20 2020 2022 2222 0a20  d data.    """. 
+0000d8f0: 2020 206e 7463 2c20 6e73 7074 203d 2041     ntc, nspt = A
+0000d900: 2e73 6861 7065 0a20 2020 2023 2064 6566  .shape.    # def
+0000d910: 696e 6573 2061 6e20 6172 7261 7920 7769  ines an array wi
+0000d920: 7468 204e 2065 7874 7261 2073 616d 706c  th N extra sampl
+0000d930: 6573 2061 7420 6569 7468 6572 2073 6964  es at either sid
+0000d940: 650a 2020 2020 7465 6d70 203d 206e 702e  e.    temp = np.
+0000d950: 7a65 726f 7328 5b6e 7463 2c20 6e73 7074  zeros([ntc, nspt
+0000d960: 202b 2032 202a 204e 5d29 0a20 2020 2023   + 2 * N]).    #
+0000d970: 2073 6574 2074 6865 2063 656e 7472 616c   set the central
+0000d980: 2070 6f72 7469 6f6e 206f 6620 7468 6520   portion of the 
+0000d990: 6172 7261 7920 746f 2041 0a20 2020 2074  array to A.    t
+0000d9a0: 656d 705b 3a2c 204e 3a2d 4e5d 203d 2041  emp[:, N:-N] = A
+0000d9b0: 0a20 2020 2023 206c 6561 6469 6e67 2073  .    # leading s
+0000d9c0: 616d 706c 6573 3a20 6571 7561 6c20 746f  amples: equal to
+0000d9d0: 2066 6972 7374 2073 616d 706c 6520 6f66   first sample of
+0000d9e0: 2061 6374 7561 6c20 6172 7261 790a 2020   actual array.  
+0000d9f0: 2020 7465 6d70 5b3a 2c20 303a 4e5d 203d    temp[:, 0:N] =
+0000da00: 206e 702e 7265 7065 6174 286e 702e 6578   np.repeat(np.ex
+0000da10: 7061 6e64 5f64 696d 7328 7465 6d70 5b3a  pand_dims(temp[:
+0000da20: 2c20 4e5d 2c20 6178 6973 3d2d 3129 2c20  , N], axis=-1), 
+0000da30: 4e2c 2061 7869 733d 2d31 290a 2020 2020  N, axis=-1).    
+0000da40: 2320 7472 6169 6c69 6e67 2073 616d 706c  # trailing sampl
+0000da50: 6573 3a20 4571 7561 6c20 746f 206c 6173  es: Equal to las
+0000da60: 7420 7361 6d70 6c65 206f 6620 6163 7475  t sample of actu
+0000da70: 616c 2061 7272 6179 0a20 2020 2074 656d  al array.    tem
+0000da80: 705b 3a2c 202d 4e3a 5d20 3d20 6e70 2e72  p[:, -N:] = np.r
+0000da90: 6570 6561 7428 6e70 2e65 7870 616e 645f  epeat(np.expand_
+0000daa0: 6469 6d73 2874 656d 705b 3a2c 202d 4e20  dims(temp[:, -N 
+0000dab0: 2d20 315d 2c20 6178 6973 3d2d 3129 2c20  - 1], axis=-1), 
+0000dac0: 4e2c 2061 7869 733d 2d31 290a 2020 2020  N, axis=-1).    
+0000dad0: 2320 636f 6e76 6f6c 7665 2077 6974 6820  # convolve with 
+0000dae0: 6120 626f 7863 6172 2061 6e64 206e 6f72  a boxcar and nor
+0000daf0: 6d61 6c69 7a65 2c20 616e 6420 7573 6520  malize, and use 
+0000db00: 6f6e 6c79 2063 656e 7472 616c 2070 6f72  only central por
+0000db10: 7469 6f6e 206f 6620 7468 6520 7265 7375  tion of the resu
+0000db20: 6c74 0a20 2020 2023 2077 6974 6820 6c65  lt.    # with le
+0000db30: 6e67 7468 2065 7175 616c 2074 6f20 7468  ngth equal to th
+0000db40: 6520 6f72 6967 696e 616c 2061 7272 6179  e original array
+0000db50: 2c20 6469 7363 6172 6469 6e67 2074 6865  , discarding the
+0000db60: 2061 6464 6564 206c 6561 6469 6e67 2061   added leading a
+0000db70: 6e64 2074 7261 696c 696e 6720 7361 6d70  nd trailing samp
+0000db80: 6c65 730a 2020 2020 4220 3d20 7363 6970  les.    B = scip
+0000db90: 792e 7369 676e 616c 2e63 6f6e 766f 6c76  y.signal.convolv
+0000dba0: 6532 6428 7465 6d70 2c20 6e70 2e65 7870  e2d(temp, np.exp
+0000dbb0: 616e 645f 6469 6d73 286e 702e 6f6e 6573  and_dims(np.ones
+0000dbc0: 284e 2920 2f20 4e2c 2061 7869 733d 3029  (N) / N, axis=0)
+0000dbd0: 2c20 6d6f 6465 3d22 7361 6d65 2229 5b3a  , mode="same")[:
+0000dbe0: 2c20 4e3a 2d4e 5d0a 2020 2020 7265 7475  , N:-N].    retu
+0000dbf0: 726e 2042 0a0a 0a64 6566 2072 6f62 7573  rn B...def robus
+0000dc00: 745f 7374 6163 6b28 6363 5f61 7272 6179  t_stack(cc_array
+0000dc10: 2c20 6570 7369 6c6f 6e29 3a0a 2020 2020  , epsilon):.    
+0000dc20: 2222 220a 2020 2020 7468 6973 2069 7320  """.    this is 
+0000dc30: 6120 726f 6275 7374 2073 7461 636b 696e  a robust stackin
+0000dc40: 6720 616c 676f 7269 7468 6d20 6465 7363  g algorithm desc
+0000dc50: 7269 6265 6420 696e 2050 616c 7669 7320  ribed in Palvis 
+0000dc60: 616e 6420 5665 726e 6f6e 2032 3031 300a  and Vernon 2010.
+0000dc70: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
+0000dc80: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+0000dc90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+0000dca0: 6363 5f61 7272 6179 3a20 6e75 6d70 792e  cc_array: numpy.
+0000dcb0: 6e64 6172 7261 7920 636f 6e74 6169 6e73  ndarray contains
+0000dcc0: 2074 6865 2032 4420 6372 6f73 7320 636f   the 2D cross co
+0000dcd0: 7272 656c 6174 696f 6e20 6d61 7472 6978  rrelation matrix
+0000dce0: 0a20 2020 2065 7073 696c 6f6e 3a20 7265  .    epsilon: re
+0000dcf0: 7369 6475 616c 2074 6872 6568 6f6c 6420  sidual threhold 
+0000dd00: 746f 2071 7569 7420 7468 6520 6974 6572  to quit the iter
+0000dd10: 6174 696f 6e0a 2020 2020 5245 5455 524e  ation.    RETURN
+0000dd20: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+0000dd30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0000dd40: 2020 6e65 7773 7461 636b 3a20 6e75 6d70    newstack: nump
+0000dd50: 7920 7665 6374 6f72 2063 6f6e 7461 696e  y vector contain
+0000dd60: 7320 7468 6520 7374 6163 6b65 6420 6372  s the stacked cr
+0000dd70: 6f73 7320 636f 7272 656c 6174 696f 6e0a  oss correlation.
+0000dd80: 0a20 2020 2057 7269 7474 656e 2062 7920  .    Written by 
+0000dd90: 4d61 7269 6e65 2044 656e 6f6c 6c65 0a20  Marine Denolle. 
+0000dda0: 2020 2022 2222 0a20 2020 2072 6573 203d     """.    res =
+0000ddb0: 2039 6539 2020 2320 7265 7369 6475 616c   9e9  # residual
+0000ddc0: 730a 2020 2020 7720 3d20 6e70 2e6f 6e65  s.    w = np.one
+0000ddd0: 7328 6363 5f61 7272 6179 2e73 6861 7065  s(cc_array.shape
+0000dde0: 5b30 5d29 0a20 2020 206e 7374 6570 203d  [0]).    nstep =
+0000ddf0: 2030 0a20 2020 206e 6577 7374 6163 6b20   0.    newstack 
+0000de00: 3d20 6e70 2e6d 6564 6961 6e28 6363 5f61  = np.median(cc_a
+0000de10: 7272 6179 2c20 6178 6973 3d30 290a 2020  rray, axis=0).  
+0000de20: 2020 7768 696c 6520 7265 7320 3e20 6570    while res > ep
+0000de30: 7369 6c6f 6e3a 0a20 2020 2020 2020 2073  silon:.        s
+0000de40: 7461 636b 203d 206e 6577 7374 6163 6b0a  tack = newstack.
+0000de50: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0000de60: 2072 616e 6765 2863 635f 6172 7261 792e   range(cc_array.
+0000de70: 7368 6170 655b 305d 293a 0a20 2020 2020  shape[0]):.     
+0000de80: 2020 2020 2020 2063 7261 7020 3d20 6e70         crap = np
+0000de90: 2e6d 756c 7469 706c 7928 7374 6163 6b2c  .multiply(stack,
+0000dea0: 2063 635f 6172 7261 795b 692c 203a 5d2e   cc_array[i, :].
+0000deb0: 5429 0a20 2020 2020 2020 2020 2020 2063  T).            c
+0000dec0: 7261 705f 646f 7420 3d20 6e70 2e73 756d  rap_dot = np.sum
+0000ded0: 2863 7261 7029 0a20 2020 2020 2020 2020  (crap).         
+0000dee0: 2020 2064 695f 6e6f 726d 203d 206e 702e     di_norm = np.
+0000def0: 6c69 6e61 6c67 2e6e 6f72 6d28 6363 5f61  linalg.norm(cc_a
+0000df00: 7272 6179 5b69 2c20 3a5d 290a 2020 2020  rray[i, :]).    
+0000df10: 2020 2020 2020 2020 7269 203d 2063 635f          ri = cc_
+0000df20: 6172 7261 795b 692c 203a 5d20 2d20 6372  array[i, :] - cr
+0000df30: 6170 5f64 6f74 202a 2073 7461 636b 0a20  ap_dot * stack. 
+0000df40: 2020 2020 2020 2020 2020 2072 695f 6e6f             ri_no
+0000df50: 726d 203d 206e 702e 6c69 6e61 6c67 2e6e  rm = np.linalg.n
+0000df60: 6f72 6d28 7269 290a 2020 2020 2020 2020  orm(ri).        
+0000df70: 2020 2020 775b 695d 203d 206e 702e 6162      w[i] = np.ab
+0000df80: 7328 6372 6170 5f64 6f74 2920 2f20 6469  s(crap_dot) / di
+0000df90: 5f6e 6f72 6d20 2f20 7269 5f6e 6f72 6d20  _norm / ri_norm 
+0000dfa0: 2023 202f 6c65 6e28 6363 5f61 7272 6179   # /len(cc_array
+0000dfb0: 5b3a 2c31 5d29 0a20 2020 2020 2020 2023  [:,1]).        #
+0000dfc0: 2070 7269 6e74 2877 290a 2020 2020 2020   print(w).      
+0000dfd0: 2020 7720 3d20 7720 2f20 6e70 2e73 756d    w = w / np.sum
+0000dfe0: 2877 290a 2020 2020 2020 2020 6e65 7773  (w).        news
+0000dff0: 7461 636b 203d 206e 702e 7375 6d28 2877  tack = np.sum((w
+0000e000: 202a 2063 635f 6172 7261 792e 5429 2e54   * cc_array.T).T
+0000e010: 2c20 6178 6973 3d30 2920 2023 202f 6c65  , axis=0)  # /le
+0000e020: 6e28 6363 5f61 7272 6179 5b3a 2c31 5d29  n(cc_array[:,1])
+0000e030: 0a20 2020 2020 2020 2072 6573 203d 206e  .        res = n
+0000e040: 702e 6c69 6e61 6c67 2e6e 6f72 6d28 6e65  p.linalg.norm(ne
+0000e050: 7773 7461 636b 202d 2073 7461 636b 2c20  wstack - stack, 
+0000e060: 6f72 643d 3129 202f 206e 702e 6c69 6e61  ord=1) / np.lina
+0000e070: 6c67 2e6e 6f72 6d28 6e65 7773 7461 636b  lg.norm(newstack
+0000e080: 2920 2f20 6c65 6e28 6363 5f61 7272 6179  ) / len(cc_array
+0000e090: 5b3a 2c20 315d 290a 2020 2020 2020 2020  [:, 1]).        
+0000e0a0: 6e73 7465 7020 2b3d 2031 0a20 2020 2020  nstep += 1.     
+0000e0b0: 2020 2069 6620 6e73 7465 7020 3e20 3130     if nstep > 10
+0000e0c0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000e0d0: 7475 726e 206e 6577 7374 6163 6b2c 2077  turn newstack, w
+0000e0e0: 2c20 6e73 7465 700a 2020 2020 7265 7475  , nstep.    retu
+0000e0f0: 726e 206e 6577 7374 6163 6b2c 2077 2c20  rn newstack, w, 
+0000e100: 6e73 7465 700a 0a0a 6465 6620 7365 6c65  nstep...def sele
+0000e110: 6374 6976 655f 7374 6163 6b28 6363 5f61  ctive_stack(cc_a
+0000e120: 7272 6179 2c20 6570 7369 6c6f 6e29 3a0a  rray, epsilon):.
+0000e130: 2020 2020 2222 220a 2020 2020 7468 6973      """.    this
+0000e140: 2069 7320 6120 7365 6c65 6374 6976 6520   is a selective 
+0000e150: 7374 6163 6b69 6e67 2061 6c67 6f72 6974  stacking algorit
+0000e160: 686d 2064 6576 656c 6f70 6564 2062 7920  hm developed by 
+0000e170: 4a61 7265 6420 4272 7961 6e2e 0a0a 2020  Jared Bryan...  
+0000e180: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
+0000e190: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+0000e1a0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2063 635f  --------.    cc_
+0000e1b0: 6172 7261 793a 206e 756d 7079 2e6e 6461  array: numpy.nda
+0000e1c0: 7272 6179 2063 6f6e 7461 696e 7320 7468  rray contains th
+0000e1d0: 6520 3244 2063 726f 7373 2063 6f72 7265  e 2D cross corre
+0000e1e0: 6c61 7469 6f6e 206d 6174 7269 780a 2020  lation matrix.  
+0000e1f0: 2020 6570 7369 6c6f 6e3a 2072 6573 6964    epsilon: resid
+0000e200: 7561 6c20 7468 7265 686f 6c64 2074 6f20  ual threhold to 
+0000e210: 7175 6974 2074 6865 2069 7465 7261 7469  quit the iterati
+0000e220: 6f6e 0a20 2020 2052 4554 5552 4e53 3a0a  on.    RETURNS:.
+0000e230: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+0000e240: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e  ----------.    n
+0000e250: 6577 7374 6163 6b3a 206e 756d 7079 2076  ewstack: numpy v
+0000e260: 6563 746f 7220 636f 6e74 6169 6e73 2074  ector contains t
+0000e270: 6865 2073 7461 636b 6564 2063 726f 7373  he stacked cross
+0000e280: 2063 6f72 7265 6c61 7469 6f6e 0a0a 2020   correlation..  
+0000e290: 2020 5772 6974 7465 6e20 6279 204d 6172    Written by Mar
+0000e2a0: 696e 6520 4465 6e6f 6c6c 650a 2020 2020  ine Denolle.    
+0000e2b0: 2222 220a 2020 2020 6363 203d 206e 702e  """.    cc = np.
+0000e2c0: 6f6e 6573 2863 635f 6172 7261 792e 7368  ones(cc_array.sh
+0000e2d0: 6170 655b 305d 290a 2020 2020 6e65 7773  ape[0]).    news
+0000e2e0: 7461 636b 203d 206e 702e 6d65 616e 2863  tack = np.mean(c
+0000e2f0: 635f 6172 7261 792c 2061 7869 733d 3029  c_array, axis=0)
+0000e300: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
+0000e310: 6e67 6528 6363 5f61 7272 6179 2e73 6861  nge(cc_array.sha
+0000e320: 7065 5b30 5d29 3a0a 2020 2020 2020 2020  pe[0]):.        
+0000e330: 6363 5b69 5d20 3d20 6e70 2e73 756d 286e  cc[i] = np.sum(n
+0000e340: 702e 6d75 6c74 6970 6c79 286e 6577 7374  p.multiply(newst
+0000e350: 6163 6b2c 2063 635f 6172 7261 795b 692c  ack, cc_array[i,
+0000e360: 203a 5d2e 5429 290a 2020 2020 696b 203d   :].T)).    ik =
+0000e370: 206e 702e 7768 6572 6528 6363 203e 3d20   np.where(cc >= 
+0000e380: 6570 7369 6c6f 6e29 5b30 5d0a 2020 2020  epsilon)[0].    
+0000e390: 6e65 7773 7461 636b 203d 206e 702e 6d65  newstack = np.me
+0000e3a0: 616e 2863 635f 6172 7261 795b 696b 2c20  an(cc_array[ik, 
+0000e3b0: 3a5d 2c20 6178 6973 3d30 290a 0a20 2020  :], axis=0)..   
+0000e3c0: 2072 6574 7572 6e20 6e65 7773 7461 636b   return newstack
+0000e3d0: 2c20 6363 0a0a 0a64 6566 2077 6869 7465  , cc...def white
+0000e3e0: 6e5f 3144 2874 696d 6573 6572 6965 732c  n_1D(timeseries,
+0000e3f0: 2066 6674 5f70 6172 612c 206e 5f74 6170   fft_para, n_tap
+0000e400: 6572 293a 0a20 2020 2022 2222 0a20 2020  er):.    """.   
+0000e410: 2054 6869 7320 6675 6e63 7469 6f6e 2074   This function t
+0000e420: 616b 6573 2061 2031 2d64 696d 656e 7369  akes a 1-dimensi
+0000e430: 6f6e 616c 2074 696d 6573 6572 6965 7320  onal timeseries 
+0000e440: 6172 7261 792c 2074 7261 6e73 666f 726d  array, transform
+0000e450: 7320 746f 2066 7265 7175 656e 6379 2064  s to frequency d
+0000e460: 6f6d 6169 6e20 7573 696e 6720 6666 742c  omain using fft,
+0000e470: 0a20 2020 2077 6869 7465 6e73 2074 6865  .    whitens the
+0000e480: 2061 6d70 6c69 7475 6465 206f 6620 7468   amplitude of th
+0000e490: 6520 7370 6563 7472 756d 2069 6e20 6672  e spectrum in fr
+0000e4a0: 6571 7565 6e63 7920 646f 6d61 696e 2062  equency domain b
+0000e4b0: 6574 7765 656e 202a 6672 6571 6d69 6e2a  etween *freqmin*
+0000e4c0: 2061 6e64 202a 6672 6571 6d61 782a 0a20   and *freqmax*. 
+0000e4d0: 2020 2061 6e64 2072 6574 7572 6e73 2074     and returns t
+0000e4e0: 6865 2077 6869 7465 6e65 6420 6666 742e  he whitened fft.
+0000e4f0: 0a20 2020 2050 4152 414d 4554 4552 533a  .    PARAMETERS:
+0000e500: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+0000e510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+0000e520: 6461 7461 3a20 6e75 6d70 792e 6e64 6172  data: numpy.ndar
+0000e530: 7261 7920 636f 6e74 6169 6e73 2074 6865  ray contains the
+0000e540: 2031 4420 7469 6d65 2073 6572 6965 7320   1D time series 
+0000e550: 746f 2077 6869 7465 6e0a 2020 2020 6666  to whiten.    ff
+0000e560: 745f 7061 7261 3a20 6469 6374 2063 6f6e  t_para: dict con
+0000e570: 7461 696e 696e 6720 616c 6c20 6666 745f  taining all fft_
+0000e580: 6363 2070 6172 616d 6574 6572 7320 7375  cc parameters su
+0000e590: 6368 2061 730a 2020 2020 2020 2020 6474  ch as.        dt
+0000e5a0: 3a20 5468 6520 7361 6d70 6c69 6e67 2073  : The sampling s
+0000e5b0: 7061 6365 206f 6620 7468 6520 6064 6174  pace of the `dat
+0000e5c0: 6160 0a20 2020 2020 2020 2066 7265 716d  a`.        freqm
+0000e5d0: 696e 3a20 5468 6520 6c6f 7765 7220 6672  in: The lower fr
+0000e5e0: 6571 7565 6e63 7920 626f 756e 640a 2020  equency bound.  
+0000e5f0: 2020 2020 2020 6672 6571 6d61 783a 2054        freqmax: T
+0000e600: 6865 2075 7070 6572 2066 7265 7175 656e  he upper frequen
+0000e610: 6379 2062 6f75 6e64 0a20 2020 2020 2020  cy bound.       
+0000e620: 2073 6d6f 6f74 685f 4e3a 2069 6e74 6567   smooth_N: integ
+0000e630: 6572 2c20 6974 2064 6566 696e 6573 2074  er, it defines t
+0000e640: 6865 2068 616c 6620 7769 6e64 6f77 206c  he half window l
+0000e650: 656e 6774 6820 746f 2073 6d6f 6f74 680a  ength to smooth.
+0000e660: 2020 2020 2020 2020 6e5f 7461 7065 722c          n_taper,
+0000e670: 206f 7074 696f 6e61 6c3a 2069 6e74 6567   optional: integ
+0000e680: 6572 2c20 6465 6669 6e65 2074 6865 2077  er, define the w
+0000e690: 6964 7468 206f 6620 7468 6520 7461 7065  idth of the tape
+0000e6a0: 7220 696e 2073 616d 706c 6573 0a20 2020  r in samples.   
+0000e6b0: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
+0000e6c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000e6d0: 2d2d 2d2d 0a20 2020 2046 4654 5261 7753  ----.    FFTRawS
+0000e6e0: 6967 6e3a 206e 756d 7079 2e6e 6461 7272  ign: numpy.ndarr
+0000e6f0: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
+0000e700: 4646 5420 6f66 2074 6865 2077 6869 7465  FFT of the white
+0000e710: 6e65 6420 696e 7075 7420 7472 6163 6520  ned input trace 
+0000e720: 6265 7477 6565 6e20 7468 6520 6672 6571  between the freq
+0000e730: 7565 6e63 7920 626f 756e 6473 0a20 2020  uency bounds.   
+0000e740: 2022 2222 0a20 2020 2023 206c 6f61 6420   """.    # load 
+0000e750: 7061 7261 6d65 7465 7273 0a20 2020 2064  parameters.    d
+0000e760: 656c 7461 203d 2066 6674 5f70 6172 615b  elta = fft_para[
+0000e770: 2264 7422 5d0a 2020 2020 6672 6571 6d69  "dt"].    freqmi
+0000e780: 6e20 3d20 6666 745f 7061 7261 5b22 6672  n = fft_para["fr
+0000e790: 6571 6d69 6e22 5d0a 2020 2020 6672 6571  eqmin"].    freq
+0000e7a0: 6d61 7820 3d20 6666 745f 7061 7261 5b22  max = fft_para["
+0000e7b0: 6672 6571 6d61 7822 5d0a 2020 2020 736d  freqmax"].    sm
+0000e7c0: 6f6f 7468 5f4e 203d 2066 6674 5f70 6172  ooth_N = fft_par
+0000e7d0: 615b 2273 6d6f 6f74 685f 4e22 5d0a 0a20  a["smooth_N"].. 
+0000e7e0: 2020 206e 6666 7420 3d20 6e65 7874 5f66     nfft = next_f
+0000e7f0: 6173 745f 6c65 6e28 6c65 6e28 7469 6d65  ast_len(len(time
+0000e800: 7365 7269 6573 2929 0a20 2020 2073 7065  series)).    spe
+0000e810: 6320 3d20 6e70 2e66 6674 2e66 6674 2874  c = np.fft.fft(t
+0000e820: 696d 6573 6572 6965 732c 206e 6666 7429  imeseries, nfft)
+0000e830: 0a20 2020 2066 7265 7120 3d20 6e70 2e66  .    freq = np.f
+0000e840: 6674 2e66 6674 6672 6571 286e 6666 742c  ft.fftfreq(nfft,
+0000e850: 2064 3d64 656c 7461 290a 0a20 2020 2069   d=delta)..    i
+0000e860: 7830 203d 206e 702e 6172 676d 696e 286e  x0 = np.argmin(n
+0000e870: 702e 6162 7328 6672 6571 202d 2066 7265  p.abs(freq - fre
+0000e880: 716d 696e 2929 0a20 2020 2069 7831 203d  qmin)).    ix1 =
+0000e890: 206e 702e 6172 676d 696e 286e 702e 6162   np.argmin(np.ab
+0000e8a0: 7328 6672 6571 202d 2066 7265 716d 6178  s(freq - freqmax
+0000e8b0: 2929 0a0a 2020 2020 6966 2069 7831 202b  ))..    if ix1 +
+0000e8c0: 206e 5f74 6170 6572 203e 206e 6666 743a   n_taper > nfft:
+0000e8d0: 0a20 2020 2020 2020 2069 7831 3120 3d20  .        ix11 = 
+0000e8e0: 6e66 6674 0a20 2020 2065 6c73 653a 0a20  nfft.    else:. 
+0000e8f0: 2020 2020 2020 2069 7831 3120 3d20 6978         ix11 = ix
+0000e900: 3120 2b20 6e5f 7461 7065 720a 0a20 2020  1 + n_taper..   
+0000e910: 2069 6620 6978 3020 2d20 6e5f 7461 7065   if ix0 - n_tape
+0000e920: 7220 3c20 303a 0a20 2020 2020 2020 2069  r < 0:.        i
+0000e930: 7830 3020 3d20 300a 2020 2020 656c 7365  x00 = 0.    else
+0000e940: 3a0a 2020 2020 2020 2020 6978 3030 203d  :.        ix00 =
+0000e950: 2069 7830 202d 206e 5f74 6170 6572 0a0a   ix0 - n_taper..
+0000e960: 2020 2020 7370 6563 5f6f 7574 203d 2073      spec_out = s
+0000e970: 7065 632e 636f 7079 2829 0a20 2020 2073  pec.copy().    s
+0000e980: 7065 635f 6f75 745b 303a 6978 3030 5d20  pec_out[0:ix00] 
+0000e990: 3d20 302e 3020 2b20 302e 306a 0a20 2020  = 0.0 + 0.0j.   
+0000e9a0: 2073 7065 635f 6f75 745b 6978 3131 3a5d   spec_out[ix11:]
+0000e9b0: 203d 2030 2e30 202b 2030 2e30 6a0a 0a20   = 0.0 + 0.0j.. 
+0000e9c0: 2020 2069 6620 736d 6f6f 7468 5f4e 203c     if smooth_N <
+0000e9d0: 3d20 313a 0a20 2020 2020 2020 2073 7065  = 1:.        spe
+0000e9e0: 635f 6f75 745b 6978 3030 3a69 7831 315d  c_out[ix00:ix11]
+0000e9f0: 203d 206e 702e 6578 7028 312e 306a 202a   = np.exp(1.0j *
+0000ea00: 206e 702e 616e 676c 6528 7370 6563 5f6f   np.angle(spec_o
+0000ea10: 7574 5b69 7830 303a 6978 3131 5d29 290a  ut[ix00:ix11])).
+0000ea20: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000ea30: 2020 7370 6563 5f6f 7574 5b69 7830 303a    spec_out[ix00:
+0000ea40: 6978 3131 5d20 2f3d 206d 6f76 696e 675f  ix11] /= moving_
+0000ea50: 6176 6528 6e70 2e61 6273 2873 7065 635f  ave(np.abs(spec_
+0000ea60: 6f75 745b 6978 3030 3a69 7831 315d 292c  out[ix00:ix11]),
+0000ea70: 2073 6d6f 6f74 685f 4e29 0a0a 2020 2020   smooth_N)..    
+0000ea80: 7820 3d20 6e70 2e6c 696e 7370 6163 6528  x = np.linspace(
+0000ea90: 6e70 2e70 6920 2f20 322e 302c 206e 702e  np.pi / 2.0, np.
+0000eaa0: 7069 2c20 6978 3020 2d20 6978 3030 290a  pi, ix0 - ix00).
+0000eab0: 2020 2020 7370 6563 5f6f 7574 5b69 7830      spec_out[ix0
+0000eac0: 303a 6978 305d 202a 3d20 6e70 2e63 6f73  0:ix0] *= np.cos
+0000ead0: 2878 2920 2a2a 2032 0a0a 2020 2020 7820  (x) ** 2..    x 
+0000eae0: 3d20 6e70 2e6c 696e 7370 6163 6528 302e  = np.linspace(0.
+0000eaf0: 302c 206e 702e 7069 202f 2032 2e30 2c20  0, np.pi / 2.0, 
+0000eb00: 6978 3131 202d 2069 7831 290a 2020 2020  ix11 - ix1).    
+0000eb10: 7370 6563 5f6f 7574 5b69 7831 3a69 7831  spec_out[ix1:ix1
+0000eb20: 315d 202a 3d20 6e70 2e63 6f73 2878 2920  1] *= np.cos(x) 
+0000eb30: 2a2a 2032 0a0a 2020 2020 7265 7475 726e  ** 2..    return
+0000eb40: 2073 7065 635f 6f75 740a 0a0a 6465 6620   spec_out...def 
+0000eb50: 7768 6974 656e 5f32 4428 7469 6d65 7365  whiten_2D(timese
+0000eb60: 7269 6573 2c20 6666 745f 7061 7261 2c20  ries, fft_para, 
+0000eb70: 6e5f 7461 7065 7229 3a0a 2020 2020 2222  n_taper):.    ""
+0000eb80: 220a 2020 2020 5468 6973 2066 756e 6374  ".    This funct
+0000eb90: 696f 6e20 7461 6b65 7320 6120 322d 6469  ion takes a 2-di
+0000eba0: 6d65 6e73 696f 6e61 6c20 7469 6d65 7365  mensional timese
+0000ebb0: 7269 6573 2061 7272 6179 2c20 7472 616e  ries array, tran
+0000ebc0: 7366 6f72 6d73 2074 6f20 6672 6571 7565  sforms to freque
+0000ebd0: 6e63 7920 646f 6d61 696e 2075 7369 6e67  ncy domain using
+0000ebe0: 2066 6674 2c0a 2020 2020 7768 6974 656e   fft,.    whiten
+0000ebf0: 7320 7468 6520 616d 706c 6974 7564 6520  s the amplitude 
+0000ec00: 6f66 2074 6865 2073 7065 6374 7275 6d20  of the spectrum 
+0000ec10: 696e 2066 7265 7175 656e 6379 2064 6f6d  in frequency dom
+0000ec20: 6169 6e20 6265 7477 6565 6e20 2a66 7265  ain between *fre
+0000ec30: 716d 696e 2a20 616e 6420 2a66 7265 716d  qmin* and *freqm
+0000ec40: 6178 2a0a 2020 2020 616e 6420 7265 7475  ax*.    and retu
+0000ec50: 726e 7320 7468 6520 7768 6974 656e 6564  rns the whitened
+0000ec60: 2066 6674 2e0a 2020 2020 5041 5241 4d45   fft..    PARAME
+0000ec70: 5445 5253 3a0a 2020 2020 2d2d 2d2d 2d2d  TERS:.    ------
+0000ec80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000ec90: 0a20 2020 2064 6174 613a 206e 756d 7079  .    data: numpy
+0000eca0: 2e6e 6461 7272 6179 2063 6f6e 7461 696e  .ndarray contain
+0000ecb0: 7320 7468 6520 3144 2074 696d 6520 7365  s the 1D time se
+0000ecc0: 7269 6573 2074 6f20 7768 6974 656e 0a20  ries to whiten. 
+0000ecd0: 2020 2066 6674 5f70 6172 613a 2064 6963     fft_para: dic
+0000ece0: 7420 636f 6e74 6169 6e69 6e67 2061 6c6c  t containing all
+0000ecf0: 2066 6674 5f63 6320 7061 7261 6d65 7465   fft_cc paramete
+0000ed00: 7273 2073 7563 6820 6173 0a20 2020 2020  rs such as.     
+0000ed10: 2020 2064 743a 2054 6865 2073 616d 706c     dt: The sampl
+0000ed20: 696e 6720 7370 6163 6520 6f66 2074 6865  ing space of the
+0000ed30: 2060 6461 7461 600a 2020 2020 2020 2020   `data`.        
+0000ed40: 6672 6571 6d69 6e3a 2054 6865 206c 6f77  freqmin: The low
+0000ed50: 6572 2066 7265 7175 656e 6379 2062 6f75  er frequency bou
+0000ed60: 6e64 0a20 2020 2020 2020 2066 7265 716d  nd.        freqm
+0000ed70: 6178 3a20 5468 6520 7570 7065 7220 6672  ax: The upper fr
+0000ed80: 6571 7565 6e63 7920 626f 756e 640a 2020  equency bound.  
+0000ed90: 2020 2020 2020 736d 6f6f 7468 5f4e 3a20        smooth_N: 
+0000eda0: 696e 7465 6765 722c 2069 7420 6465 6669  integer, it defi
+0000edb0: 6e65 7320 7468 6520 6861 6c66 2077 696e  nes the half win
+0000edc0: 646f 7720 6c65 6e67 7468 2074 6f20 736d  dow length to sm
+0000edd0: 6f6f 7468 0a20 2020 2020 2020 206e 5f74  ooth.        n_t
+0000ede0: 6170 6572 2c20 6f70 7469 6f6e 616c 3a20  aper, optional: 
+0000edf0: 696e 7465 6765 722c 2064 6566 696e 6520  integer, define 
+0000ee00: 7468 6520 7769 6474 6820 6f66 2074 6865  the width of the
+0000ee10: 2074 6170 6572 2069 6e20 7361 6d70 6c65   taper in sample
+0000ee20: 730a 2020 2020 5245 5455 524e 533a 0a20  s.    RETURNS:. 
+0000ee30: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+0000ee40: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 4646  ---------.    FF
+0000ee50: 5452 6177 5369 676e 3a20 6e75 6d70 792e  TRawSign: numpy.
+0000ee60: 6e64 6172 7261 7920 636f 6e74 6169 6e73  ndarray contains
+0000ee70: 2074 6865 2046 4654 206f 6620 7468 6520   the FFT of the 
+0000ee80: 7768 6974 656e 6564 2069 6e70 7574 2074  whitened input t
+0000ee90: 7261 6365 2062 6574 7765 656e 2074 6865  race between the
+0000eea0: 2066 7265 7175 656e 6379 2062 6f75 6e64   frequency bound
+0000eeb0: 730a 2020 2020 2222 220a 2020 2020 2320  s.    """.    # 
+0000eec0: 6c6f 6164 2070 6172 616d 6574 6572 730a  load parameters.
+0000eed0: 2020 2020 6465 6c74 6120 3d20 6666 745f      delta = fft_
+0000eee0: 7061 7261 5b22 6474 225d 0a20 2020 2066  para["dt"].    f
+0000eef0: 7265 716d 696e 203d 2066 6674 5f70 6172  reqmin = fft_par
+0000ef00: 615b 2266 7265 716d 696e 225d 0a20 2020  a["freqmin"].   
+0000ef10: 2066 7265 716d 6178 203d 2066 6674 5f70   freqmax = fft_p
+0000ef20: 6172 615b 2266 7265 716d 6178 225d 0a20  ara["freqmax"]. 
+0000ef30: 2020 2073 6d6f 6f74 685f 4e20 3d20 6666     smooth_N = ff
+0000ef40: 745f 7061 7261 5b22 736d 6f6f 7468 5f4e  t_para["smooth_N
+0000ef50: 225d 0a0a 2020 2020 6e66 6674 203d 206e  "]..    nfft = n
+0000ef60: 6578 745f 6661 7374 5f6c 656e 2874 696d  ext_fast_len(tim
+0000ef70: 6573 6572 6965 732e 7368 6170 655b 315d  eseries.shape[1]
+0000ef80: 290a 2020 2020 7370 6563 203d 206e 702e  ).    spec = np.
+0000ef90: 6666 742e 6666 746e 2874 696d 6573 6572  fft.fftn(timeser
+0000efa0: 6965 732c 2073 3d5b 6e66 6674 5d29 0a20  ies, s=[nfft]). 
+0000efb0: 2020 2066 7265 7120 3d20 6e70 2e66 6674     freq = np.fft
+0000efc0: 2e66 6674 6672 6571 286e 6666 742c 2064  .fftfreq(nfft, d
+0000efd0: 3d64 656c 7461 290a 0a20 2020 2069 7830  =delta)..    ix0
+0000efe0: 203d 206e 702e 6172 676d 696e 286e 702e   = np.argmin(np.
+0000eff0: 6162 7328 6672 6571 202d 2066 7265 716d  abs(freq - freqm
+0000f000: 696e 2929 0a20 2020 2069 7831 203d 206e  in)).    ix1 = n
+0000f010: 702e 6172 676d 696e 286e 702e 6162 7328  p.argmin(np.abs(
+0000f020: 6672 6571 202d 2066 7265 716d 6178 2929  freq - freqmax))
+0000f030: 0a0a 2020 2020 6966 2069 7831 202b 206e  ..    if ix1 + n
+0000f040: 5f74 6170 6572 203e 206e 6666 743a 0a20  _taper > nfft:. 
+0000f050: 2020 2020 2020 2069 7831 3120 3d20 6e66         ix11 = nf
+0000f060: 6674 0a20 2020 2065 6c73 653a 0a20 2020  ft.    else:.   
+0000f070: 2020 2020 2069 7831 3120 3d20 6978 3120       ix11 = ix1 
+0000f080: 2b20 6e5f 7461 7065 720a 0a20 2020 2069  + n_taper..    i
+0000f090: 6620 6978 3020 2d20 6e5f 7461 7065 7220  f ix0 - n_taper 
+0000f0a0: 3c20 303a 0a20 2020 2020 2020 2069 7830  < 0:.        ix0
+0000f0b0: 3020 3d20 300a 2020 2020 656c 7365 3a0a  0 = 0.    else:.
+0000f0c0: 2020 2020 2020 2020 6978 3030 203d 2069          ix00 = i
+0000f0d0: 7830 202d 206e 5f74 6170 6572 0a0a 2020  x0 - n_taper..  
+0000f0e0: 2020 7370 6563 5f6f 7574 203d 2073 7065    spec_out = spe
+0000f0f0: 632e 636f 7079 2829 2020 2320 6d61 7920  c.copy()  # may 
+0000f100: 6265 2069 6e63 6f6e 7665 6e69 656e 7420  be inconvenient 
+0000f110: 6475 6520 746f 2068 6967 6865 7220 6d65  due to higher me
+0000f120: 6d6f 7279 2075 7361 6765 0a20 2020 2073  mory usage.    s
+0000f130: 7065 635f 6f75 745b 3a2c 2030 3a69 7830  pec_out[:, 0:ix0
+0000f140: 305d 203d 2030 2e30 202b 2030 2e30 6a0a  0] = 0.0 + 0.0j.
+0000f150: 2020 2020 7370 6563 5f6f 7574 5b3a 2c20      spec_out[:, 
+0000f160: 6978 3131 3a5d 203d 2030 2e30 202b 2030  ix11:] = 0.0 + 0
+0000f170: 2e30 6a0a 0a20 2020 2069 6620 736d 6f6f  .0j..    if smoo
+0000f180: 7468 5f4e 203c 3d20 313a 0a20 2020 2020  th_N <= 1:.     
+0000f190: 2020 2073 7065 635f 6f75 745b 3a2c 2069     spec_out[:, i
+0000f1a0: 7830 303a 6978 3131 5d20 3d20 6e70 2e65  x00:ix11] = np.e
+0000f1b0: 7870 2831 2e30 6a20 2a20 6e70 2e61 6e67  xp(1.0j * np.ang
+0000f1c0: 6c65 2873 7065 635f 6f75 745b 3a2c 2069  le(spec_out[:, i
+0000f1d0: 7830 303a 6978 3131 5d29 290a 2020 2020  x00:ix11])).    
+0000f1e0: 656c 7365 3a0a 2020 2020 2020 2020 7370  else:.        sp
+0000f1f0: 6563 5f6f 7574 5b3a 2c20 6978 3030 3a69  ec_out[:, ix00:i
+0000f200: 7831 315d 202f 3d20 6d6f 7669 6e67 5f61  x11] /= moving_a
+0000f210: 7665 5f32 4428 6e70 2e61 6273 2873 7065  ve_2D(np.abs(spe
+0000f220: 635f 6f75 745b 3a2c 2069 7830 303a 6978  c_out[:, ix00:ix
+0000f230: 3131 5d29 2c20 736d 6f6f 7468 5f4e 290a  11]), smooth_N).
+0000f240: 0a20 2020 2078 203d 206e 702e 6c69 6e73  .    x = np.lins
+0000f250: 7061 6365 286e 702e 7069 202f 2032 2e30  pace(np.pi / 2.0
+0000f260: 2c20 6e70 2e70 692c 2069 7830 202d 2069  , np.pi, ix0 - i
+0000f270: 7830 3029 0a20 2020 2073 7065 635f 6f75  x00).    spec_ou
+0000f280: 745b 3a2c 2069 7830 303a 6978 305d 202a  t[:, ix00:ix0] *
+0000f290: 3d20 6e70 2e63 6f73 2878 2920 2a2a 2032  = np.cos(x) ** 2
+0000f2a0: 0a0a 2020 2020 7820 3d20 6e70 2e6c 696e  ..    x = np.lin
+0000f2b0: 7370 6163 6528 302e 302c 206e 702e 7069  space(0.0, np.pi
+0000f2c0: 202f 2032 2e30 2c20 6978 3131 202d 2069   / 2.0, ix11 - i
+0000f2d0: 7831 290a 2020 2020 7370 6563 5f6f 7574  x1).    spec_out
+0000f2e0: 5b3a 2c20 6978 313a 6978 3131 5d20 2a3d  [:, ix1:ix11] *=
+0000f2f0: 206e 702e 636f 7328 7829 202a 2a20 320a   np.cos(x) ** 2.
+0000f300: 0a20 2020 2072 6574 7572 6e20 7370 6563  .    return spec
+0000f310: 5f6f 7574 0a0a 0a64 6566 2077 6869 7465  _out...def white
+0000f320: 6e28 6461 7461 2c20 6666 745f 7061 7261  n(data, fft_para
+0000f330: 2c20 6e5f 7461 7065 723d 3130 3029 3a0a  , n_taper=100):.
+0000f340: 2020 2020 2222 220a 2020 2020 5468 6973      """.    This
+0000f350: 2066 756e 6374 696f 6e20 7461 6b65 7320   function takes 
+0000f360: 6120 7469 6d65 7365 7269 6573 2061 7272  a timeseries arr
+0000f370: 6179 2c20 7472 616e 7366 6f72 6d73 2074  ay, transforms t
+0000f380: 6f20 6672 6571 7565 6e63 7920 646f 6d61  o frequency doma
+0000f390: 696e 2075 7369 6e67 2066 6674 2c0a 2020  in using fft,.  
+0000f3a0: 2020 7768 6974 656e 7320 7468 6520 616d    whitens the am
+0000f3b0: 706c 6974 7564 6520 6f66 2074 6865 2073  plitude of the s
+0000f3c0: 7065 6374 7275 6d20 696e 2066 7265 7175  pectrum in frequ
+0000f3d0: 656e 6379 2064 6f6d 6169 6e20 6265 7477  ency domain betw
+0000f3e0: 6565 6e20 2a66 7265 716d 696e 2a20 616e  een *freqmin* an
+0000f3f0: 6420 2a66 7265 716d 6178 2a0a 2020 2020  d *freqmax*.    
+0000f400: 616e 6420 7265 7475 726e 7320 7468 6520  and returns the 
+0000f410: 7768 6974 656e 6564 2066 6674 2e0a 2020  whitened fft..  
+0000f420: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
+0000f430: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+0000f440: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6174  --------.    dat
+0000f450: 613a 206e 756d 7079 2e6e 6461 7272 6179  a: numpy.ndarray
+0000f460: 2063 6f6e 7461 696e 7320 7468 6520 3144   contains the 1D
+0000f470: 2074 696d 6520 7365 7269 6573 2074 6f20   time series to 
+0000f480: 7768 6974 656e 0a20 2020 2066 6674 5f70  whiten.    fft_p
+0000f490: 6172 613a 2064 6963 7420 636f 6e74 6169  ara: dict contai
+0000f4a0: 6e69 6e67 2061 6c6c 2066 6674 5f63 6320  ning all fft_cc 
+0000f4b0: 7061 7261 6d65 7465 7273 2073 7563 6820  parameters such 
+0000f4c0: 6173 0a20 2020 2020 2020 2064 743a 2054  as.        dt: T
+0000f4d0: 6865 2073 616d 706c 696e 6720 7370 6163  he sampling spac
+0000f4e0: 6520 6f66 2074 6865 2060 6461 7461 600a  e of the `data`.
+0000f4f0: 2020 2020 2020 2020 6672 6571 6d69 6e3a          freqmin:
+0000f500: 2054 6865 206c 6f77 6572 2066 7265 7175   The lower frequ
+0000f510: 656e 6379 2062 6f75 6e64 0a20 2020 2020  ency bound.     
+0000f520: 2020 2066 7265 716d 6178 3a20 5468 6520     freqmax: The 
+0000f530: 7570 7065 7220 6672 6571 7565 6e63 7920  upper frequency 
+0000f540: 626f 756e 640a 2020 2020 2020 2020 736d  bound.        sm
+0000f550: 6f6f 7468 5f4e 3a20 696e 7465 6765 722c  ooth_N: integer,
+0000f560: 2069 7420 6465 6669 6e65 7320 7468 6520   it defines the 
+0000f570: 6861 6c66 2077 696e 646f 7720 6c65 6e67  half window leng
+0000f580: 7468 2074 6f20 736d 6f6f 7468 0a20 2020  th to smooth.   
+0000f590: 2020 2020 2066 7265 715f 6e6f 726d 3a20       freq_norm: 
+0000f5a0: 7768 6974 656e 696e 6720 6d65 7468 6f64  whitening method
+0000f5b0: 2062 6574 7765 656e 2027 6f6e 652d 6269   between 'one-bi
+0000f5c0: 7427 2061 6e64 2027 524d 4127 0a20 2020  t' and 'RMA'.   
+0000f5d0: 2052 4554 5552 4e53 3a0a 2020 2020 2d2d   RETURNS:.    --
+0000f5e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0000f5f0: 2d2d 2d2d 0a20 2020 2046 4654 5261 7753  ----.    FFTRawS
+0000f600: 6967 6e3a 206e 756d 7079 2e6e 6461 7272  ign: numpy.ndarr
+0000f610: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
+0000f620: 4646 5420 6f66 2074 6865 2077 6869 7465  FFT of the white
+0000f630: 6e65 6420 696e 7075 7420 7472 6163 6520  ned input trace 
+0000f640: 6265 7477 6565 6e20 7468 6520 6672 6571  between the freq
+0000f650: 7565 6e63 7920 626f 756e 6473 0a20 2020  uency bounds.   
+0000f660: 2022 2222 0a0a 2020 2020 2320 5370 6565   """..    # Spee
+0000f670: 6420 7570 2046 4654 2062 7920 7061 6464  d up FFT by padd
+0000f680: 696e 6720 746f 206f 7074 696d 616c 2073  ing to optimal s
+0000f690: 697a 6520 666f 7220 4646 5450 4143 4b0a  ize for FFTPACK.
+0000f6a0: 2020 2020 6966 2064 6174 612e 6e64 696d      if data.ndim
+0000f6b0: 203d 3d20 313a 0a20 2020 2020 2020 2046   == 1:.        F
+0000f6c0: 4654 5261 7753 6967 6e20 3d20 7768 6974  FTRawSign = whit
+0000f6d0: 656e 5f31 4428 6461 7461 2c20 6666 745f  en_1D(data, fft_
+0000f6e0: 7061 7261 2c20 6e5f 7461 7065 7229 0a20  para, n_taper). 
+0000f6f0: 2020 2020 2020 2023 2041 5252 5f4f 5554         # ARR_OUT
+0000f700: 3a20 4f6e 6c79 2066 6f72 2063 6f6e 7369  : Only for consi
+0000f710: 7374 656e 6379 2077 6974 6820 6e6f 6973  stency with nois
+0000f720: 6570 7920 6170 7072 6f61 6368 206f 6620  epy approach of 
+0000f730: 686f 6c64 696e 6720 7468 6520 6675 6c6c  holding the full
+0000f740: 0a20 2020 2020 2020 2023 2073 7065 6374  .        # spect
+0000f750: 7275 6d20 286e 6f74 206a 7573 7420 3020  rum (not just 0 
+0000f760: 616e 6420 706f 7369 7469 7665 2066 7265  and positive fre
+0000f770: 712e 2070 6172 7429 0a20 2020 2020 2020  q. part).       
+0000f780: 2061 7272 5f6f 7574 203d 206e 702e 7a65   arr_out = np.ze
+0000f790: 726f 7328 2846 4654 5261 7753 6967 6e2e  ros((FFTRawSign.
+0000f7a0: 7368 6170 655b 305d 202d 2031 2920 2a20  shape[0] - 1) * 
+0000f7b0: 3220 2b20 312c 2064 7479 7065 3d63 6f6d  2 + 1, dtype=com
+0000f7c0: 706c 6578 290a 2020 2020 2020 2020 6172  plex).        ar
+0000f7d0: 725f 6f75 745b 3020 3a20 4646 5452 6177  r_out[0 : FFTRaw
+0000f7e0: 5369 676e 2e73 6861 7065 5b30 5d5d 203d  Sign.shape[0]] =
+0000f7f0: 2046 4654 5261 7753 6967 6e0a 2020 2020   FFTRawSign.    
+0000f800: 2020 2020 6172 725f 6f75 745b 4646 5452      arr_out[FFTR
+0000f810: 6177 5369 676e 2e73 6861 7065 5b30 5d20  awSign.shape[0] 
+0000f820: 3a5d 203d 2046 4654 5261 7753 6967 6e5b  :] = FFTRawSign[
+0000f830: 313a 5d2e 636f 6e6a 7567 6174 6528 295b  1:].conjugate()[
+0000f840: 3a3a 2d31 5d0a 0a20 2020 2065 6c69 6620  ::-1]..    elif 
+0000f850: 6461 7461 2e6e 6469 6d20 3d3d 2032 3a0a  data.ndim == 2:.
+0000f860: 2020 2020 2020 2020 4646 5452 6177 5369          FFTRawSi
+0000f870: 676e 203d 2077 6869 7465 6e5f 3244 2864  gn = whiten_2D(d
+0000f880: 6174 612c 2066 6674 5f70 6172 612c 206e  ata, fft_para, n
+0000f890: 5f74 6170 6572 290a 2020 2020 2020 2020  _taper).        
+0000f8a0: 6172 725f 6f75 7420 3d20 6e70 2e7a 6572  arr_out = np.zer
+0000f8b0: 6f73 2828 4646 5452 6177 5369 676e 2e73  os((FFTRawSign.s
+0000f8c0: 6861 7065 5b30 5d2c 2028 4646 5452 6177  hape[0], (FFTRaw
+0000f8d0: 5369 676e 2e73 6861 7065 5b31 5d20 2d20  Sign.shape[1] - 
+0000f8e0: 3129 202a 2032 202b 2031 292c 2064 7479  1) * 2 + 1), dty
+0000f8f0: 7065 3d63 6f6d 706c 6578 290a 2020 2020  pe=complex).    
+0000f900: 2020 2020 6172 725f 6f75 745b 3a2c 2046      arr_out[:, F
+0000f910: 4654 5261 7753 6967 6e2e 7368 6170 655b  FTRawSign.shape[
+0000f920: 315d 203a 5d20 3d20 4646 5452 6177 5369  1] :] = FFTRawSi
+0000f930: 676e 5b3a 2c20 313a 5d2e 636f 6e6a 7567  gn[:, 1:].conjug
+0000f940: 6174 6528 295b 3a3a 2d31 5d0a 2020 2020  ate()[::-1].    
+0000f950: 7265 7475 726e 2046 4654 5261 7753 6967  return FFTRawSig
+0000f960: 6e0a 0a0a 6465 6620 6164 6170 7469 7665  n...def adaptive
+0000f970: 5f66 696c 7465 7228 6172 722c 2067 293a  _filter(arr, g):
+0000f980: 0a20 2020 2022 2222 0a20 2020 2074 6865  .    """.    the
+0000f990: 2061 6461 7074 6976 6520 636f 7661 7269   adaptive covari
+0000f9a0: 616e 6365 2066 696c 7465 7220 746f 2065  ance filter to e
+0000f9b0: 6e68 616e 6365 2063 6f68 6572 656e 7420  nhance coherent 
+0000f9c0: 7369 676e 616c 732e 2046 656c 6c6f 7773  signals. Fellows
+0000f9d0: 2074 6865 206d 6574 686f 6420 6f66 0a20   the method of. 
+0000f9e0: 2020 204e 616b 6174 6120 6574 2061 6c2e     Nakata et al.
+0000f9f0: 2c20 3230 3135 2028 4170 7065 6e64 6978  , 2015 (Appendix
+0000fa00: 2042 290a 0a20 2020 2074 6865 2066 696c   B)..    the fil
+0000fa10: 7465 7265 6420 7369 676e 616c 205b 7831  tered signal [x1
+0000fa20: 5d20 6973 2067 6976 656e 2062 7920 7831  ] is given by x1
+0000fa30: 203d 2069 6666 7428 502a 7831 2877 2929   = ifft(P*x1(w))
+0000fa40: 2077 6865 7265 2078 3120 6973 2074 6865   where x1 is the
+0000fa50: 2066 6674 6564 2073 7065 6374 7261 0a20   ffted spectra. 
+0000fa60: 2020 2061 6e64 2050 2069 7320 7468 6520     and P is the 
+0000fa70: 6669 6c74 6572 2e20 5020 6973 2063 6f6e  filter. P is con
+0000fa80: 7374 7275 6374 6564 2062 7920 7573 696e  structed by usin
+0000fa90: 6720 7468 6520 7465 6d70 6f72 616c 2063  g the temporal c
+0000faa0: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
+0000fab0: 2e0a 0a20 2020 2050 4152 414d 4554 4552  ...    PARAMETER
+0000fac0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+0000fad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
+0000fae0: 2020 6172 723a 206e 756d 7079 2e6e 6461    arr: numpy.nda
+0000faf0: 7272 6179 2063 6f6e 7461 696e 7320 7468  rray contains th
+0000fb00: 6520 3244 2074 7261 6365 7320 6f66 2064  e 2D traces of d
+0000fb10: 6169 6c79 2f68 6f75 726c 7920 6372 6f73  aily/hourly cros
+0000fb20: 732d 636f 7272 656c 6174 696f 6e20 6675  s-correlation fu
+0000fb30: 6e63 7469 6f6e 730a 2020 2020 673a 2061  nctions.    g: a
+0000fb40: 2070 6f73 6974 6976 6520 6e75 6d62 6572   positive number
+0000fb50: 2074 6f20 6164 6a75 7374 2074 6865 2066   to adjust the f
+0000fb60: 696c 7465 7220 6861 7273 686e 6573 730a  ilter harshness.
+0000fb70: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
+0000fb80: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+0000fb90: 2d2d 2d2d 2d2d 2d0a 2020 2020 6e61 7272  -------.    narr
+0000fba0: 3a20 6e75 6d70 7920 7665 6374 6f72 2063  : numpy vector c
+0000fbb0: 6f6e 7461 696e 7320 7468 6520 7374 6163  ontains the stac
+0000fbc0: 6b65 6420 6372 6f73 7320 636f 7272 656c  ked cross correl
+0000fbd0: 6174 696f 6e20 6675 6e63 7469 6f6e 0a20  ation function. 
+0000fbe0: 2020 2022 2222 0a20 2020 2069 6620 6172     """.    if ar
+0000fbf0: 722e 6e64 696d 203d 3d20 313a 0a20 2020  r.ndim == 1:.   
+0000fc00: 2020 2020 2072 6574 7572 6e20 6172 720a       return arr.
+0000fc10: 2020 2020 4e2c 204d 203d 2061 7272 2e73      N, M = arr.s
+0000fc20: 6861 7065 0a20 2020 204e 6666 7420 3d20  hape.    Nfft = 
+0000fc30: 6e65 7874 5f66 6173 745f 6c65 6e28 4d29  next_fast_len(M)
+0000fc40: 0a0a 2020 2020 2320 6666 7420 7468 6520  ..    # fft the 
+0000fc50: 3244 2061 7272 6179 0a20 2020 2073 7065  2D array.    spe
+0000fc60: 6320 3d20 7363 6970 792e 6666 7470 6163  c = scipy.fftpac
+0000fc70: 6b2e 6666 7428 6172 722c 2061 7869 733d  k.fft(arr, axis=
+0000fc80: 312c 206e 3d4e 6666 7429 5b3a 2c20 3a4d  1, n=Nfft)[:, :M
+0000fc90: 5d0a 0a20 2020 2023 206d 616b 6520 6372  ]..    # make cr
+0000fca0: 6f73 732d 7370 6563 7472 6d20 6d61 7472  oss-spectrm matr
+0000fcb0: 6978 0a20 2020 2063 7370 6563 203d 206e  ix.    cspec = n
+0000fcc0: 702e 7a65 726f 7328 7368 6170 653d 284e  p.zeros(shape=(N
+0000fcd0: 202a 204e 2c20 4d29 2c20 6474 7970 653d   * N, M), dtype=
+0000fce0: 6e70 2e63 6f6d 706c 6578 3634 290a 2020  np.complex64).  
+0000fcf0: 2020 666f 7220 6969 2069 6e20 7261 6e67    for ii in rang
+0000fd00: 6528 4e29 3a0a 2020 2020 2020 2020 666f  e(N):.        fo
+0000fd10: 7220 6a6a 2069 6e20 7261 6e67 6528 4e29  r jj in range(N)
+0000fd20: 3a0a 2020 2020 2020 2020 2020 2020 6b6b  :.            kk
+0000fd30: 203d 2069 6920 2a20 4e20 2b20 6a6a 0a20   = ii * N + jj. 
+0000fd40: 2020 2020 2020 2020 2020 2063 7370 6563             cspec
+0000fd50: 5b6b 6b5d 203d 2073 7065 635b 6969 5d20  [kk] = spec[ii] 
+0000fd60: 2a20 6e70 2e63 6f6e 6a75 6761 7465 2873  * np.conjugate(s
+0000fd70: 7065 635b 6a6a 5d29 0a0a 2020 2020 5331  pec[jj])..    S1
+0000fd80: 203d 206e 702e 7a65 726f 7328 4d2c 2064   = np.zeros(M, d
+0000fd90: 7479 7065 3d6e 702e 636f 6d70 6c65 7836  type=np.complex6
+0000fda0: 3429 0a20 2020 2053 3220 3d20 6e70 2e7a  4).    S2 = np.z
+0000fdb0: 6572 6f73 284d 2c20 6474 7970 653d 6e70  eros(M, dtype=np
+0000fdc0: 2e63 6f6d 706c 6578 3634 290a 2020 2020  .complex64).    
+0000fdd0: 2320 636f 6e73 7472 7563 7420 7468 6520  # construct the 
+0000fde0: 6669 6c74 6572 2050 0a20 2020 2066 6f72  filter P.    for
+0000fdf0: 2069 6920 696e 2072 616e 6765 284e 293a   ii in range(N):
+0000fe00: 0a20 2020 2020 2020 206d 6d20 3d20 6969  .        mm = ii
+0000fe10: 202a 204e 202b 2069 690a 2020 2020 2020   * N + ii.      
+0000fe20: 2020 5332 202b 3d20 6373 7065 635b 6d6d    S2 += cspec[mm
+0000fe30: 5d0a 2020 2020 2020 2020 666f 7220 6a6a  ].        for jj
+0000fe40: 2069 6e20 7261 6e67 6528 4e29 3a0a 2020   in range(N):.  
+0000fe50: 2020 2020 2020 2020 2020 6b6b 203d 2069            kk = i
+0000fe60: 6920 2a20 4e20 2b20 6a6a 0a20 2020 2020  i * N + jj.     
+0000fe70: 2020 2020 2020 2053 3120 2b3d 2063 7370         S1 += csp
+0000fe80: 6563 5b6b 6b5d 0a0a 2020 2020 7020 3d20  ec[kk]..    p = 
+0000fe90: 6e70 2e70 6f77 6572 2828 5331 202d 2053  np.power((S1 - S
+0000fea0: 3229 202f 2028 5332 202a 2028 4e20 2d20  2) / (S2 * (N - 
+0000feb0: 3129 292c 2067 290a 0a20 2020 2023 206d  1)), g)..    # m
+0000fec0: 616b 6520 6966 6674 0a20 2020 206e 6172  ake ifft.    nar
+0000fed0: 7220 3d20 6e70 2e72 6561 6c28 7363 6970  r = np.real(scip
+0000fee0: 792e 6666 7470 6163 6b2e 6966 6674 286e  y.fftpack.ifft(n
+0000fef0: 702e 6d75 6c74 6970 6c79 2870 2c20 7370  p.multiply(p, sp
+0000ff00: 6563 292c 204e 6666 742c 2061 7869 733d  ec), Nfft, axis=
+0000ff10: 3129 5b3a 2c20 3a4d 5d29 0a20 2020 2072  1)[:, :M]).    r
+0000ff20: 6574 7572 6e20 6e70 2e6d 6561 6e28 6e61  eturn np.mean(na
+0000ff30: 7272 2c20 6178 6973 3d30 290a 0a0a 6465  rr, axis=0)...de
+0000ff40: 6620 7077 7328 6172 722c 2073 616d 706c  f pws(arr, sampl
+0000ff50: 696e 675f 7261 7465 2c20 706f 7765 723d  ing_rate, power=
+0000ff60: 322c 2070 7773 5f74 696d 6567 6174 653d  2, pws_timegate=
+0000ff70: 352e 3029 3a0a 2020 2020 2222 220a 2020  5.0):.    """.  
+0000ff80: 2020 5065 7266 6f72 6d73 2070 6861 7365    Performs phase
+0000ff90: 2d77 6569 6768 7465 6420 7374 6163 6b20  -weighted stack 
+0000ffa0: 6f6e 2061 7272 6179 206f 6620 7469 6d65  on array of time
+0000ffb0: 2073 6572 6965 732e 204d 6f64 6966 6965   series. Modifie
+0000ffc0: 6420 6f6e 2074 6865 206e 6f69 7365 2066  d on the noise f
+0000ffd0: 756e 6374 696f 6e20 6279 2054 696d 2043  unction by Tim C
+0000ffe0: 6c69 6d65 6e74 732e 0a20 2020 2046 6f6c  liments..    Fol
+0000fff0: 6c6f 7773 206d 6574 686f 6473 206f 6620  lows methods of 
+00010000: 5363 6869 6d6d 656c 2061 6e64 2050 6175  Schimmel and Pau
+00010010: 6c73 7365 6e2c 2031 3939 372e 0a20 2020  lssen, 1997..   
+00010020: 2049 6620 7328 7429 2069 7320 7469 6d65   If s(t) is time
+00010030: 2073 6572 6965 7320 6461 7461 2028 7365   series data (se
+00010040: 6973 6d6f 6772 616d 2c20 6f72 2063 726f  ismogram, or cro
+00010050: 7373 2d63 6f72 7265 6c61 7469 6f6e 292c  ss-correlation),
+00010060: 0a20 2020 2053 2874 2920 3d20 7328 7429  .    S(t) = s(t)
+00010070: 202b 2069 2a48 2873 2874 2929 2c20 7768   + i*H(s(t)), wh
+00010080: 6572 6520 4828 7328 7429 2920 6973 2048  ere H(s(t)) is H
+00010090: 696c 6265 7274 2074 7261 6e73 666f 726d  ilbert transform
+000100a0: 206f 6620 7328 7429 0a20 2020 2053 2874   of s(t).    S(t
+000100b0: 2920 3d20 7328 7429 202b 2069 2a48 2873  ) = s(t) + i*H(s
+000100c0: 2874 2929 203d 2041 2874 292a 6578 7028  (t)) = A(t)*exp(
+000100d0: 692a 7068 6928 7429 292c 2077 6865 7265  i*phi(t)), where
+000100e0: 0a20 2020 2041 2874 2920 6973 2065 6e76  .    A(t) is env
+000100f0: 656c 6f70 6520 6f66 2073 2874 2920 616e  elope of s(t) an
+00010100: 6420 7068 6928 7429 2069 7320 7068 6173  d phi(t) is phas
+00010110: 6520 6f66 2073 2874 290a 2020 2020 5068  e of s(t).    Ph
+00010120: 6173 652d 7765 6967 6874 6564 2073 7461  ase-weighted sta
+00010130: 636b 2c20 6728 7429 2c20 6973 2074 6865  ck, g(t), is the
+00010140: 6e3a 0a20 2020 2067 2874 2920 3d20 312f  n:.    g(t) = 1/
+00010150: 4e20 7375 6d20 6a20 3d20 313a 4e20 735f  N sum j = 1:N s_
+00010160: 6a28 7429 202a 207c 2031 2f4e 2073 756d  j(t) * | 1/N sum
+00010170: 206b 203d 2031 3a4e 2065 7870 5b69 202a   k = 1:N exp[i *
+00010180: 2070 6869 5f6b 2874 295d 7c5e 760a 2020   phi_k(t)]|^v.  
+00010190: 2020 7768 6572 6520 4e20 6973 206e 756d    where N is num
+000101a0: 6265 7220 6f66 2074 7261 6365 7320 7573  ber of traces us
+000101b0: 6564 2c20 7620 6973 2073 6861 7270 6e65  ed, v is sharpne
+000101c0: 7373 206f 6620 7068 6173 652d 7765 6967  ss of phase-weig
+000101d0: 6874 6564 2073 7461 636b 0a0a 2020 2020  hted stack..    
+000101e0: 5041 5241 4d45 5445 5253 3a0a 2020 2020  PARAMETERS:.    
+000101f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00010200: 2d2d 2d2d 2d0a 2020 2020 6172 723a 204e  -----.    arr: N
+00010210: 206c 656e 6774 6820 6172 7261 7920 6f66   length array of
+00010220: 2074 696d 6520 7365 7269 6573 2064 6174   time series dat
+00010230: 6120 286e 756d 7079 2e6e 6461 7272 6179  a (numpy.ndarray
+00010240: 290a 2020 2020 7361 6d70 6c69 6e67 5f72  ).    sampling_r
+00010250: 6174 653a 2073 616d 706c 696e 6720 7261  ate: sampling ra
+00010260: 7465 206f 6620 7469 6d65 2073 6572 6965  te of time serie
+00010270: 7320 6172 7220 2869 6e74 290a 2020 2020  s arr (int).    
+00010280: 706f 7765 723a 2065 7870 6f6e 656e 7420  power: exponent 
+00010290: 666f 7220 7068 6173 6520 7374 6163 6b20  for phase stack 
+000102a0: 2869 6e74 290a 2020 2020 7077 735f 7469  (int).    pws_ti
+000102b0: 6d65 6761 7465 3a20 6e75 6d62 6572 206f  megate: number o
+000102c0: 6620 7365 636f 6e64 7320 746f 2073 6d6f  f seconds to smo
+000102d0: 6f74 6820 7068 6173 6520 7374 6163 6b20  oth phase stack 
+000102e0: 2866 6c6f 6174 290a 0a20 2020 2052 4554  (float)..    RET
+000102f0: 5552 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d  URNS:.    ------
+00010300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00010310: 2020 2020 7765 6967 6874 6564 3a20 5068      weighted: Ph
+00010320: 6173 6520 7765 6967 6874 6564 2073 7461  ase weighted sta
+00010330: 636b 206f 6620 7469 6d65 2073 6572 6965  ck of time serie
+00010340: 7320 6461 7461 2028 6e75 6d70 792e 6e64  s data (numpy.nd
+00010350: 6172 7261 7929 0a20 2020 2022 2222 0a0a  array).    """..
+00010360: 2020 2020 6966 2061 7272 2e6e 6469 6d20      if arr.ndim 
+00010370: 3d3d 2031 3a0a 2020 2020 2020 2020 7265  == 1:.        re
+00010380: 7475 726e 2061 7272 0a20 2020 204e 2c20  turn arr.    N, 
+00010390: 4d20 3d20 6172 722e 7368 6170 650a 2020  M = arr.shape.  
+000103a0: 2020 616e 616c 7974 6963 203d 2068 696c    analytic = hil
+000103b0: 6265 7274 2861 7272 2c20 6178 6973 3d31  bert(arr, axis=1
+000103c0: 2c20 4e3d 6e65 7874 5f66 6173 745f 6c65  , N=next_fast_le
+000103d0: 6e28 4d29 295b 3a2c 203a 4d5d 0a20 2020  n(M))[:, :M].   
+000103e0: 2070 6861 7365 203d 206e 702e 616e 676c   phase = np.angl
+000103f0: 6528 616e 616c 7974 6963 290a 2020 2020  e(analytic).    
+00010400: 7068 6173 655f 7374 6163 6b20 3d20 6e70  phase_stack = np
+00010410: 2e6d 6561 6e28 6e70 2e65 7870 2831 6a20  .mean(np.exp(1j 
+00010420: 2a20 7068 6173 6529 2c20 6178 6973 3d30  * phase), axis=0
+00010430: 290a 2020 2020 7068 6173 655f 7374 6163  ).    phase_stac
+00010440: 6b20 3d20 6e70 2e61 6273 2870 6861 7365  k = np.abs(phase
+00010450: 5f73 7461 636b 2920 2a2a 2028 706f 7765  _stack) ** (powe
+00010460: 7229 0a0a 2020 2020 2320 736d 6f6f 7468  r)..    # smooth
+00010470: 696e 670a 2020 2020 2320 7469 6d65 6761  ing.    # timega
+00010480: 7465 5f73 616d 706c 6573 203d 2069 6e74  te_samples = int
+00010490: 2870 7773 5f74 696d 6567 6174 6520 2a20  (pws_timegate * 
+000104a0: 7361 6d70 6c69 6e67 5f72 6174 6529 0a20  sampling_rate). 
+000104b0: 2020 2023 2070 6861 7365 5f73 7461 636b     # phase_stack
+000104c0: 203d 206d 6f76 696e 675f 6176 6528 7068   = moving_ave(ph
+000104d0: 6173 655f 7374 6163 6b2c 7469 6d65 6761  ase_stack,timega
+000104e0: 7465 5f73 616d 706c 6573 290a 2020 2020  te_samples).    
+000104f0: 7765 6967 6874 6564 203d 206e 702e 6d75  weighted = np.mu
+00010500: 6c74 6970 6c79 2861 7272 2c20 7068 6173  ltiply(arr, phas
+00010510: 655f 7374 6163 6b29 0a20 2020 2072 6574  e_stack).    ret
+00010520: 7572 6e20 6e70 2e6d 6561 6e28 7765 6967  urn np.mean(weig
+00010530: 6874 6564 2c20 6178 6973 3d30 290a 0a0a  hted, axis=0)...
+00010540: 6465 6620 6e72 6f6f 745f 7374 6163 6b28  def nroot_stack(
+00010550: 6363 5f61 7272 6179 2c20 706f 7765 7229  cc_array, power)
+00010560: 3a0a 2020 2020 2222 220a 2020 2020 7468  :.    """.    th
+00010570: 6973 2069 7320 6e74 682d 726f 6f74 2073  is is nth-root s
+00010580: 7461 636b 696e 6720 616c 676f 7269 7468  tacking algorith
+00010590: 6d20 7472 616e 736c 6174 6564 2062 6173  m translated bas
+000105a0: 6564 206f 6e20 7468 6520 6d61 746c 6162  ed on the matlab
+000105b0: 2066 756e 6374 696f 6e0a 2020 2020 6672   function.    fr
+000105c0: 6f6d 2068 7474 7073 3a2f 2f67 6974 6875  om https://githu
+000105d0: 622e 636f 6d2f 7874 7961 6e67 7073 702f  b.com/xtyangpsp/
+000105e0: 5365 6973 5374 6163 6b20 2862 7920 5869  SeisStack (by Xi
+000105f0: 616f 7461 6f20 5961 6e67 3b20 666f 6c6c  aotao Yang; foll
+00010600: 6f77 7320 7468 650a 2020 2020 7265 6665  ows the.    refe
+00010610: 7265 6e63 6520 6f66 204d 696c 6c65 742c  rence of Millet,
+00010620: 2046 2065 7420 616c 2e2c 2032 3031 3920   F et al., 2019 
+00010630: 4a47 5229 0a0a 2020 2020 5061 7261 6d65  JGR)..    Parame
+00010640: 7465 7273 3a0a 2020 2020 2d2d 2d2d 2d2d  ters:.    ------
+00010650: 2d2d 2d2d 2d2d 0a20 2020 2063 635f 6172  ------.    cc_ar
+00010660: 7261 793a 206e 756d 7079 2e6e 6461 7272  ray: numpy.ndarr
+00010670: 6179 2063 6f6e 7461 696e 7320 7468 6520  ay contains the 
+00010680: 3244 2063 726f 7373 2063 6f72 7265 6c61  2D cross correla
+00010690: 7469 6f6e 206d 6174 7269 780a 2020 2020  tion matrix.    
+000106a0: 706f 7765 723a 206e 702e 696e 742c 206e  power: np.int, n
+000106b0: 7468 2072 6f6f 7420 666f 7220 7468 6520  th root for the 
+000106c0: 7374 6163 6b69 6e67 0a0a 2020 2020 5265  stacking..    Re
+000106d0: 7475 726e 733a 0a20 2020 202d 2d2d 2d2d  turns:.    -----
+000106e0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6e73 7461  -------.    nsta
+000106f0: 636b 3a20 6e70 2e6e 6461 7272 6179 2c20  ck: np.ndarray, 
+00010700: 6669 6e61 6c20 7374 6163 6b65 6420 7761  final stacked wa
+00010710: 7665 666f 726d 730a 0a20 2020 2057 7269  veforms..    Wri
+00010720: 7474 656e 2062 7920 4368 656e 6778 696e  tten by Chengxin
+00010730: 204a 6961 6e67 2040 414e 5520 284d 6179   Jiang @ANU (May
+00010740: 3230 3230 290a 2020 2020 2222 220a 2020  2020).    """.  
+00010750: 2020 6966 2063 635f 6172 7261 792e 6e64    if cc_array.nd
+00010760: 696d 203d 3d20 313a 0a20 2020 2020 2020  im == 1:.       
+00010770: 2070 7269 6e74 2822 3244 206d 6174 7269   print("2D matri
+00010780: 7820 6973 206e 6565 6465 6420 666f 7220  x is needed for 
+00010790: 6e72 6f6f 745f 7374 6163 6b22 290a 2020  nroot_stack").  
+000107a0: 2020 2020 2020 7265 7475 726e 2063 635f        return cc_
+000107b0: 6172 7261 790a 2020 2020 4e2c 204d 203d  array.    N, M =
+000107c0: 2063 635f 6172 7261 792e 7368 6170 650a   cc_array.shape.
+000107d0: 2020 2020 646f 7574 203d 206e 702e 7a65      dout = np.ze
+000107e0: 726f 7328 4d2c 2064 7479 7065 3d6e 702e  ros(M, dtype=np.
+000107f0: 666c 6f61 7433 3229 0a0a 2020 2020 2320  float32)..    # 
+00010800: 636f 6e73 7472 7563 7420 790a 2020 2020  construct y.    
+00010810: 666f 7220 6969 2069 6e20 7261 6e67 6528  for ii in range(
+00010820: 4e29 3a0a 2020 2020 2020 2020 6461 7420  N):.        dat 
+00010830: 3d20 6363 5f61 7272 6179 5b69 692c 203a  = cc_array[ii, :
+00010840: 5d0a 2020 2020 2020 2020 646f 7574 202b  ].        dout +
+00010850: 3d20 6e70 2e73 6967 6e28 6461 7429 202a  = np.sign(dat) *
+00010860: 206e 702e 6162 7328 6461 7429 202a 2a20   np.abs(dat) ** 
+00010870: 2831 202f 2070 6f77 6572 290a 2020 2020  (1 / power).    
+00010880: 646f 7574 202f 3d20 4e0a 0a20 2020 2023  dout /= N..    #
+00010890: 2074 6865 2066 696e 616c 2073 7461 636b   the final stack
+000108a0: 6564 2077 6176 6566 6f72 6d0a 2020 2020  ed waveform.    
+000108b0: 6e73 7461 636b 203d 2064 6f75 7420 2a20  nstack = dout * 
+000108c0: 6e70 2e61 6273 2864 6f75 7429 202a 2a20  np.abs(dout) ** 
+000108d0: 2870 6f77 6572 202d 2031 290a 0a20 2020  (power - 1)..   
+000108e0: 2072 6574 7572 6e20 6e73 7461 636b 0a0a   return nstack..
+000108f0: 0a64 6566 2073 656c 6563 7469 7665 5f73  .def selective_s
+00010900: 7461 636b 2863 635f 6172 7261 792c 2065  tack(cc_array, e
+00010910: 7073 696c 6f6e 2c20 6363 5f74 6829 3a20  psilon, cc_th): 
+00010920: 2023 206e 6f71 613a 2046 3831 310a 2020   # noqa: F811.  
+00010930: 2020 2222 220a 2020 2020 7468 6973 2069    """.    this i
+00010940: 7320 6120 7365 6c65 6374 6976 6520 7374  s a selective st
+00010950: 6163 6b69 6e67 2061 6c67 6f72 6974 686d  acking algorithm
+00010960: 2064 6576 656c 6f70 6564 2062 7920 4a61   developed by Ja
+00010970: 7265 6420 4272 7961 6e2f 4b75 7261 6d61  red Bryan/Kurama
+00010980: 204f 6b75 626f 2e0a 0a20 2020 2050 4152   Okubo...    PAR
+00010990: 414d 4554 4552 533a 0a20 2020 202d 2d2d  AMETERS:.    ---
+000109a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000109b0: 2d2d 2d0a 2020 2020 6363 5f61 7272 6179  ---.    cc_array
+000109c0: 3a20 6e75 6d70 792e 6e64 6172 7261 7920  : numpy.ndarray 
+000109d0: 636f 6e74 6169 6e73 2074 6865 2032 4420  contains the 2D 
+000109e0: 6372 6f73 7320 636f 7272 656c 6174 696f  cross correlatio
+000109f0: 6e20 6d61 7472 6978 0a20 2020 2065 7073  n matrix.    eps
+00010a00: 696c 6f6e 3a20 7265 7369 6475 616c 2074  ilon: residual t
+00010a10: 6872 6568 6f6c 6420 746f 2071 7569 7420  hrehold to quit 
+00010a20: 7468 6520 6974 6572 6174 696f 6e0a 2020  the iteration.  
+00010a30: 2020 6363 5f74 683a 206e 756d 7079 2e66    cc_th: numpy.f
+00010a40: 6c6f 6174 2c20 7468 7265 7368 6f6c 6420  loat, threshold 
+00010a50: 6f66 2063 6f72 7265 6c61 7469 6f6e 2063  of correlation c
+00010a60: 6f65 6666 6963 6965 6e74 2074 6f20 6265  oefficient to be
+00010a70: 2073 656c 6563 7465 640a 0a20 2020 2052   selected..    R
+00010a80: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
+00010a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00010aa0: 2d2d 0a20 2020 206e 6577 7374 6163 6b3a  --.    newstack:
+00010ab0: 206e 756d 7079 2076 6563 746f 7220 636f   numpy vector co
+00010ac0: 6e74 6169 6e73 2074 6865 2073 7461 636b  ntains the stack
+00010ad0: 6564 2063 726f 7373 2063 6f72 7265 6c61  ed cross correla
+00010ae0: 7469 6f6e 0a20 2020 206e 7374 6570 3a20  tion.    nstep: 
+00010af0: 6e70 2e69 6e74 2c20 746f 7461 6c20 6e75  np.int, total nu
+00010b00: 6d62 6572 206f 6620 6974 6572 6174 696f  mber of iteratio
+00010b10: 6e73 2066 6f72 2074 6865 2073 7461 636b  ns for the stack
+00010b20: 696e 670a 0a20 2020 204f 7269 6769 6e61  ing..    Origina
+00010b30: 6c6c 7920 7269 7474 656e 2062 7920 4d61  lly ritten by Ma
+00010b40: 7269 6e65 2044 656e 6f6c 6c65 0a20 2020  rine Denolle.   
+00010b50: 204d 6f64 6966 6965 6420 6279 2043 6865   Modified by Che
+00010b60: 6e67 7869 6e20 4a69 616e 6720 4048 6172  ngxin Jiang @Har
+00010b70: 7661 7264 2028 4f63 7432 3032 3029 0a20  vard (Oct2020). 
+00010b80: 2020 2022 2222 0a20 2020 2069 6620 6363     """.    if cc
+00010b90: 5f61 7272 6179 2e6e 6469 6d20 3d3d 2031  _array.ndim == 1
+00010ba0: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+00010bb0: 2232 4420 6d61 7472 6978 2069 7320 6e65  "2D matrix is ne
+00010bc0: 6564 6564 2066 6f72 206e 726f 6f74 5f73  eded for nroot_s
+00010bd0: 7461 636b 2229 0a20 2020 2020 2020 2072  tack").        r
+00010be0: 6574 7572 6e20 6363 5f61 7272 6179 0a20  eturn cc_array. 
+00010bf0: 2020 204e 2c20 4d20 3d20 6363 5f61 7272     N, M = cc_arr
+00010c00: 6179 2e73 6861 7065 0a0a 2020 2020 7265  ay.shape..    re
+00010c10: 7320 3d20 3965 3920 2023 2072 6573 6964  s = 9e9  # resid
+00010c20: 7561 6c73 0a20 2020 2063 6f66 203d 206e  uals.    cof = n
+00010c30: 702e 7a65 726f 7328 4e2c 2064 7479 7065  p.zeros(N, dtype
+00010c40: 3d6e 702e 666c 6f61 7433 3229 0a20 2020  =np.float32).   
+00010c50: 206e 6577 7374 6163 6b20 3d20 6e70 2e6d   newstack = np.m
+00010c60: 6561 6e28 6363 5f61 7272 6179 2c20 6178  ean(cc_array, ax
+00010c70: 6973 3d30 290a 0a20 2020 206e 7374 6570  is=0)..    nstep
+00010c80: 203d 2030 0a20 2020 2023 2073 7461 7274   = 0.    # start
+00010c90: 2069 7465 7261 7469 6f6e 0a20 2020 2077   iteration.    w
+00010ca0: 6869 6c65 2072 6573 203e 2065 7073 696c  hile res > epsil
+00010cb0: 6f6e 3a0a 2020 2020 2020 2020 666f 7220  on:.        for 
+00010cc0: 6969 2069 6e20 7261 6e67 6528 4e29 3a0a  ii in range(N):.
+00010cd0: 2020 2020 2020 2020 2020 2020 636f 665b              cof[
+00010ce0: 6969 5d20 3d20 6e70 2e63 6f72 7263 6f65  ii] = np.corrcoe
+00010cf0: 6628 6e65 7773 7461 636b 2c20 6363 5f61  f(newstack, cc_a
+00010d00: 7272 6179 5b69 692c 203a 5d29 5b30 2c20  rray[ii, :])[0, 
+00010d10: 315d 0a0a 2020 2020 2020 2020 2320 6669  1]..        # fi
+00010d20: 6e64 2067 6f6f 6420 7761 7665 666f 726d  nd good waveform
+00010d30: 730a 2020 2020 2020 2020 696e 6478 203d  s.        indx =
+00010d40: 206e 702e 7768 6572 6528 636f 6620 3e3d   np.where(cof >=
+00010d50: 2063 635f 7468 295b 305d 0a20 2020 2020   cc_th)[0].     
+00010d60: 2020 2069 6620 6e6f 7420 6c65 6e28 696e     if not len(in
+00010d70: 6478 293a 0a20 2020 2020 2020 2020 2020  dx):.           
+00010d80: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00010d90: 7228 2263 616e 6e6f 7420 6669 6e64 2067  r("cannot find g
+00010da0: 6f6f 6420 7761 7665 666f 726d 7320 696e  ood waveforms in
+00010db0: 7369 6465 2073 656c 6563 7469 7665 2073  side selective s
+00010dc0: 7461 636b 696e 6722 290a 2020 2020 2020  tacking").      
+00010dd0: 2020 6f6c 6473 7461 636b 203d 206e 6577    oldstack = new
+00010de0: 7374 6163 6b0a 2020 2020 2020 2020 6e65  stack.        ne
+00010df0: 7773 7461 636b 203d 206e 702e 6d65 616e  wstack = np.mean
+00010e00: 2863 635f 6172 7261 795b 696e 6478 5d2c  (cc_array[indx],
+00010e10: 2061 7869 733d 3029 0a20 2020 2020 2020   axis=0).       
+00010e20: 2072 6573 203d 206e 702e 6c69 6e61 6c67   res = np.linalg
+00010e30: 2e6e 6f72 6d28 6e65 7773 7461 636b 202d  .norm(newstack -
+00010e40: 206f 6c64 7374 6163 6b29 202f 2028 6e70   oldstack) / (np
+00010e50: 2e6c 696e 616c 672e 6e6f 726d 286e 6577  .linalg.norm(new
+00010e60: 7374 6163 6b29 202a 204d 290a 2020 2020  stack) * M).    
+00010e70: 2020 2020 6e73 7465 7020 2b3d 2031 0a0a      nstep += 1..
+00010e80: 2020 2020 7265 7475 726e 206e 6577 7374      return newst
+00010e90: 6163 6b2c 206e 7374 6570 0a0a 0a64 6566  ack, nstep...def
+00010ea0: 2067 6574 5f63 6328 7331 2c20 735f 7265   get_cc(s1, s_re
+00010eb0: 6629 3a0a 2020 2020 2320 7265 7475 726e  f):.    # return
+00010ec0: 7320 7468 6520 636f 7272 656c 6174 696f  s the correlatio
+00010ed0: 6e20 636f 6566 6669 6369 656e 7420 6265  n coefficient be
+00010ee0: 7477 6565 6e20 7761 7665 666f 726d 7320  tween waveforms 
+00010ef0: 696e 2073 3120 6167 6169 6e73 7420 7265  in s1 against re
+00010f00: 6665 7265 6e63 650a 2020 2020 2320 7761  ference.    # wa
+00010f10: 7665 666f 726d 2073 5f72 6566 2e0a 2020  veform s_ref..  
+00010f20: 2020 230a 2020 2020 6363 203d 206e 702e    #.    cc = np.
+00010f30: 7a65 726f 7328 7331 2e73 6861 7065 5b30  zeros(s1.shape[0
+00010f40: 5d29 0a20 2020 2073 5f72 6566 5f6e 6f72  ]).    s_ref_nor
+00010f50: 6d20 3d20 6e70 2e6c 696e 616c 672e 6e6f  m = np.linalg.no
+00010f60: 726d 2873 5f72 6566 290a 2020 2020 666f  rm(s_ref).    fo
+00010f70: 7220 6920 696e 2072 616e 6765 2873 312e  r i in range(s1.
+00010f80: 7368 6170 655b 305d 293a 0a20 2020 2020  shape[0]):.     
+00010f90: 2020 2063 635b 695d 203d 206e 702e 7375     cc[i] = np.su
+00010fa0: 6d28 6e70 2e6d 756c 7469 706c 7928 7331  m(np.multiply(s1
+00010fb0: 5b69 2c20 3a5d 2c20 735f 7265 6629 2920  [i, :], s_ref)) 
+00010fc0: 2f20 6e70 2e6c 696e 616c 672e 6e6f 726d  / np.linalg.norm
+00010fd0: 2873 315b 692c 203a 5d29 202f 2073 5f72  (s1[i, :]) / s_r
+00010fe0: 6566 5f6e 6f72 6d0a 2020 2020 7265 7475  ef_norm.    retu
+00010ff0: 726e 2063 630a 0a0a 2323 2323 2323 2323  rn cc...########
 00011000: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00011010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00011020: 2323 2323 2323 2323 2323 0a23 2323 2323  ##########.#####
-00011030: 2323 2323 2323 2323 2323 2320 4d4f 4e49  ########### MONI
-00011040: 544f 5249 4e47 2046 554e 4354 494f 4e53  TORING FUNCTIONS
-00011050: 2023 2323 2323 2323 2323 2323 2323 2323   ###############
-00011060: 2323 230a 2323 2323 2323 2323 2323 2323  ###.############
+00011020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00011030: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
+00011040: 2320 4d4f 4e49 544f 5249 4e47 2046 554e  # MONITORING FUN
+00011050: 4354 494f 4e53 2023 2323 2323 2323 2323  CTIONS #########
+00011060: 2323 2323 2323 2323 230a 2323 2323 2323  #########.######
 00011070: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00011080: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00011090: 2323 2323 2323 2323 2323 2323 0a0a 2222  ############..""
-000110a0: 220a 6120 636f 6d70 696c 6174 696f 6e20  ".a compilation 
-000110b0: 6f66 2061 6c6c 2061 7661 696c 6162 6c65  of all available
-000110c0: 2063 6f72 6520 6675 6e63 7469 6f6e 7320   core functions 
-000110d0: 666f 7220 636f 6d70 7574 696e 6720 7068  for computing ph
-000110e0: 6173 6520 6465 6c61 7973 2062 6173 6564  ase delays based
-000110f0: 206f 6e20 616d 6269 656e 7420 6e6f 6973   on ambient nois
-00011100: 6520 696e 7465 7266 6572 6f6d 6574 7279  e interferometry
-00011110: 0a0a 7175 6963 6b20 696e 6465 7820 6f66  ..quick index of
-00011120: 2064 762f 7620 6d65 7468 6f64 733a 0a31   dv/v methods:.1
-00011130: 2920 7374 7265 7463 6869 6e67 2028 7469  ) stretching (ti
-00011140: 6d65 2073 7472 6574 6368 696e 673b 2057  me stretching; W
-00011150: 6561 7665 7220 6574 2061 6c20 2832 3031  eaver et al (201
-00011160: 3129 290a 3229 2064 7477 5f64 7676 2028  1)).2) dtw_dvv (
-00011170: 4479 6e61 6d69 6320 5469 6d65 2057 6172  Dynamic Time War
-00011180: 7069 6e67 3b20 4d69 6b65 7365 6c6c 2065  ping; Mikesell e
-00011190: 7420 616c 2e20 3230 3135 290a 3329 206d  t al. 2015).3) m
-000111a0: 7763 735f 6476 7620 284d 6f76 696e 6720  wcs_dvv (Moving 
-000111b0: 5769 6e64 6f77 2043 726f 7373 2053 7065  Window Cross Spe
-000111c0: 6374 7275 6d3b 2043 6c61 726b 2065 7420  ctrum; Clark et 
-000111d0: 616c 2e2c 2032 3031 3129 0a34 2920 6d77  al., 2011).4) mw
-000111e0: 6363 5f64 7676 2028 4d6f 7669 6e67 2057  cc_dvv (Moving W
-000111f0: 696e 646f 7720 4372 6f73 7320 436f 7272  indow Cross Corr
-00011200: 656c 6174 696f 6e3b 2053 6e69 6564 6572  elation; Snieder
-00011210: 2065 7420 616c 2e2c 2032 3031 3229 0a35   et al., 2012).5
-00011220: 2920 7774 735f 6476 7620 2857 6176 656c  ) wts_dvv (Wavel
-00011230: 6574 2053 7472 6563 6869 6e67 3b20 5975  et Streching; Yu
-00011240: 616e 2065 7420 616c 2e2c 2069 6e20 7072  an et al., in pr
-00011250: 6570 290a 3629 2077 7873 5f64 7676 2028  ep).6) wxs_dvv (
-00011260: 5761 7665 6c65 7420 5872 6f73 7320 5370  Wavelet Xross Sp
-00011270: 6563 7472 756d 3b20 4d61 6f20 6574 2061  ectrum; Mao et a
-00011280: 6c2e 2c20 3230 3139 290a 3729 2077 6477  l., 2019).7) wdw
-00011290: 5f64 7676 2028 5761 7665 6c65 7420 4479  _dvv (Wavelet Dy
-000112a0: 6e61 6d69 6320 5761 7270 696e 673b 2059  namic Warping; Y
-000112b0: 7561 6e20 6574 2061 6c2e 2c20 696e 2070  uan et al., in p
-000112c0: 7265 7029 0a22 2222 0a0a 0a64 6566 2073  rep)."""...def s
-000112d0: 7472 6574 6368 696e 6728 7265 662c 2063  tretching(ref, c
-000112e0: 7572 2c20 6476 5f72 616e 6765 2c20 6e62  ur, dv_range, nb
-000112f0: 7472 6961 6c2c 2070 6172 6129 3a0a 2020  trial, para):.  
-00011300: 2020 2222 220a 2020 2020 5468 6973 2066    """.    This f
-00011310: 756e 6374 696f 6e20 636f 6d70 6172 6573  unction compares
-00011320: 2074 6865 2052 6566 6572 656e 6365 2077   the Reference w
-00011330: 6176 6566 6f72 6d20 746f 2073 7472 6574  aveform to stret
-00011340: 6368 6564 2f63 6f6d 7072 6573 7365 6420  ched/compressed 
-00011350: 6375 7272 656e 7420 7761 7665 666f 726d  current waveform
-00011360: 7320 746f 2067 6574 2074 6865 0a20 2020  s to get the.   
-00011370: 2072 656c 6174 6976 6520 7365 6973 6d69   relative seismi
-00011380: 6320 7665 6c6f 6369 7479 2076 6172 6961  c velocity varia
-00011390: 7469 6f6e 2028 616e 6420 6173 736f 6369  tion (and associ
-000113a0: 6174 6564 2065 7272 6f72 292e 0a20 2020  ated error)..   
-000113b0: 2049 7420 616c 736f 2063 6f6d 7075 7465   It also compute
-000113c0: 7320 7468 6520 636f 7272 656c 6174 696f  s the correlatio
-000113d0: 6e20 636f 6566 6669 6369 656e 7420 6265  n coefficient be
-000113e0: 7477 6565 6e20 7468 6520 5265 6665 7265  tween the Refere
-000113f0: 6e63 6520 7761 7665 666f 726d 2061 6e64  nce waveform and
-00011400: 2074 6865 2063 7572 7265 6e74 2077 6176   the current wav
-00011410: 6566 6f72 6d2e 0a0a 2020 2020 5041 5241  eform...    PARA
-00011420: 4d45 5445 5253 3a0a 2020 2020 2d2d 2d2d  METERS:.    ----
-00011430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00011440: 2072 6566 3a20 5265 6665 7265 6e63 6520   ref: Reference 
-00011450: 7761 7665 666f 726d 2028 6e70 2e6e 6461  waveform (np.nda
-00011460: 7272 6179 2c20 7369 7a65 204e 290a 2020  rray, size N).  
-00011470: 2020 6375 723a 2043 7572 7265 6e74 2077    cur: Current w
-00011480: 6176 6566 6f72 6d20 286e 702e 6e64 6172  aveform (np.ndar
-00011490: 7261 792c 2073 697a 6520 4e29 0a20 2020  ray, size N).   
-000114a0: 2064 765f 7261 6e67 653a 2061 6273 6f6c   dv_range: absol
-000114b0: 7574 6520 626f 756e 6420 666f 7220 7468  ute bound for th
-000114c0: 6520 7665 6c6f 6369 7479 2076 6172 6961  e velocity varia
-000114d0: 7469 6f6e 3b20 6578 616d 706c 653a 2064  tion; example: d
-000114e0: 763d 302e 3033 2066 6f72 205b 2d33 2c33  v=0.03 for [-3,3
-000114f0: 5d25 0a20 2020 206f 6620 7265 6c61 7469  ]%.    of relati
-00011500: 7665 2076 656c 6f63 6974 7920 6368 616e  ve velocity chan
-00011510: 6765 2028 2766 6c6f 6174 2729 0a20 2020  ge ('float').   
-00011520: 206e 6274 7269 616c 3a20 6e75 6d62 6572   nbtrial: number
-00011530: 206f 6620 7374 7265 7463 6869 6e67 2063   of stretching c
-00011540: 6f65 6666 6963 6965 6e74 2062 6574 7765  oefficient betwe
-00011550: 656e 2064 766d 696e 2061 6e64 2064 766d  en dvmin and dvm
-00011560: 6178 2c20 6e6f 206e 6565 6420 746f 2062  ax, no need to b
-00011570: 6520 6869 6768 6572 2074 6861 6e20 3130  e higher than 10
-00011580: 3020 2028 2766 6c6f 6174 2729 0a20 2020  0  ('float').   
-00011590: 2070 6172 613a 2076 6563 746f 7220 6f66   para: vector of
-000115a0: 2074 6865 2069 6e64 6963 6573 206f 6620   the indices of 
-000115b0: 7468 6520 6375 7220 616e 6420 7265 6620  the cur and ref 
-000115c0: 7769 6e64 6f77 7320 6f6e 2077 6963 6820  windows on wich 
-000115d0: 796f 7520 7761 6e74 2074 6f20 646f 2074  you want to do t
-000115e0: 6865 206d 6561 7375 7265 6d65 6e74 730a  he measurements.
-000115f0: 2020 2020 286e 702e 6e64 6172 7261 792c      (np.ndarray,
-00011600: 2073 697a 6520 746d 696e 2a64 656c 7461   size tmin*delta
-00011610: 3a74 6d61 782a 6465 6c74 6129 0a20 2020  :tmax*delta).   
-00011620: 2046 6f72 2065 7272 6f72 2063 6f6d 7075   For error compu
-00011630: 7461 7469 6f6e 2c20 7765 206e 6565 6420  tation, we need 
-00011640: 7061 7261 6d65 7465 7273 3a0a 2020 2020  parameters:.    
-00011650: 2020 2020 666d 696e 3a20 6d69 6e69 6d75      fmin: minimu
-00011660: 6d20 6672 6571 7565 6e63 7920 6f66 2074  m frequency of t
-00011670: 6865 2064 6174 610a 2020 2020 2020 2020  he data.        
-00011680: 666d 6178 3a20 6d61 7869 6d75 6d20 6672  fmax: maximum fr
-00011690: 6571 7565 6e63 7920 6f66 2074 6865 2064  equency of the d
-000116a0: 6174 610a 2020 2020 2020 2020 746d 696e  ata.        tmin
-000116b0: 3a20 6d69 6e69 6d75 6d20 7469 6d65 2077  : minimum time w
-000116c0: 696e 646f 7720 7768 6572 6520 7468 6520  indow where the 
-000116d0: 6476 2f76 2069 7320 636f 6d70 7574 6564  dv/v is computed
-000116e0: 0a20 2020 2020 2020 2074 6d61 783a 206d  .        tmax: m
-000116f0: 6178 696d 756d 2074 696d 6520 7769 6e64  aximum time wind
-00011700: 6f77 2077 6865 7265 2074 6865 2064 762f  ow where the dv/
-00011710: 7620 6973 2063 6f6d 7075 7465 640a 2020  v is computed.  
-00011720: 2020 5245 5455 524e 533a 0a20 2020 202d    RETURNS:.    -
-00011730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
-00011740: 2020 2020 6476 3a20 5265 6c61 7469 7665      dv: Relative
-00011750: 2076 656c 6f63 6974 7920 6368 616e 6765   velocity change
-00011760: 2064 762f 7620 2869 6e20 2529 0a20 2020   dv/v (in %).   
-00011770: 2063 633a 2063 6f72 7265 6c61 7469 6f6e   cc: correlation
-00011780: 2063 6f65 6666 6963 6965 6e74 2062 6574   coefficient bet
-00011790: 7765 656e 2074 6865 2072 6566 6572 656e  ween the referen
-000117a0: 6365 2077 6176 6566 6f72 6d20 616e 6420  ce waveform and 
-000117b0: 7468 6520 6265 7374 2073 7472 6574 6368  the best stretch
-000117c0: 6564 2f63 6f6d 7072 6573 7365 6420 6375  ed/compressed cu
-000117d0: 7272 656e 7420 7761 7665 666f 726d 0a20  rrent waveform. 
-000117e0: 2020 2063 6470 3a20 636f 7272 656c 6174     cdp: correlat
-000117f0: 696f 6e20 636f 6566 6669 6369 656e 7420  ion coefficient 
-00011800: 6265 7477 6565 6e20 7468 6520 7265 6665  between the refe
-00011810: 7265 6e63 6520 7761 7665 666f 726d 2061  rence waveform a
-00011820: 6e64 2074 6865 2069 6e69 7469 616c 2063  nd the initial c
-00011830: 7572 7265 6e74 2077 6176 6566 6f72 6d0a  urrent waveform.
-00011840: 2020 2020 6572 726f 723a 2045 7272 6f72      error: Error
-00011850: 7320 696e 2074 6865 2064 762f 7620 6d65  s in the dv/v me
-00011860: 6173 7572 656d 656e 7473 2062 6173 6564  asurements based
-00011870: 206f 6e20 5765 6176 6572 2065 7420 616c   on Weaver et al
-00011880: 2028 3230 3131 292c 0a20 2020 204f 6e20   (2011),.    On 
-00011890: 7468 6520 7072 6563 6973 696f 6e20 6f66  the precision of
-000118a0: 206e 6f69 7365 2d63 6f72 7265 6c61 7469   noise-correlati
-000118b0: 6f6e 2069 6e74 6572 6665 726f 6d65 7472  on interferometr
-000118c0: 792c 2047 656f 7068 7973 2e20 4a2e 2049  y, Geophys. J. I
-000118d0: 6e74 2e2c 2031 3835 2833 290a 0a20 2020  nt., 185(3)..   
-000118e0: 204e 6f74 653a 2054 6865 2063 6f64 6520   Note: The code 
-000118f0: 6669 7273 7420 6669 6e64 7320 7468 6520  first finds the 
-00011900: 6265 7374 2063 6f72 7265 6c61 7469 6f6e  best correlation
-00011910: 2063 6f65 6666 6963 6965 6e74 2062 6574   coefficient bet
-00011920: 7765 656e 2074 6865 2052 6566 6572 656e  ween the Referen
-00011930: 6365 2077 6176 6566 6f72 6d20 616e 640a  ce waveform and.
-00011940: 2020 2020 7468 6520 7374 7265 7463 6865      the stretche
-00011950: 642f 636f 6d70 7265 7373 6564 2063 7572  d/compressed cur
-00011960: 7265 6e74 2077 6176 6566 6f72 6d20 616d  rent waveform am
-00011970: 6f6e 6720 7468 6520 226e 6274 7269 616c  ong the "nbtrial
-00011980: 2220 7661 6c75 6573 2e0a 2020 2020 4120  " values..    A 
-00011990: 7265 6669 6e65 6420 616e 616c 7973 6973  refined analysis
-000119a0: 2069 7320 7468 656e 2070 6572 666f 726d   is then perform
-000119b0: 6564 2061 726f 756e 6420 7468 6973 2076  ed around this v
-000119c0: 616c 7565 2074 6f20 6f62 7461 696e 2061  alue to obtain a
-000119d0: 206d 6f72 6520 7072 6563 6973 6520 6476   more precise dv
-000119e0: 2f76 206d 6561 7375 7265 6d65 6e74 202e  /v measurement .
-000119f0: 0a0a 2020 2020 4f72 6967 696e 616c 6c79  ..    Originally
-00011a00: 2062 7920 4c2e 2056 6965 6e73 2030 342f   by L. Viens 04/
-00011a10: 3236 2f32 3031 3820 2856 6965 6e73 2065  26/2018 (Viens e
-00011a20: 7420 616c 2e2c 2032 3031 3820 4a47 5229  t al., 2018 JGR)
-00011a30: 0a20 2020 206d 6f64 6966 6965 6420 6279  .    modified by
-00011a40: 2043 6865 6e67 7869 6e20 4a69 616e 670a   Chengxin Jiang.
-00011a50: 2020 2020 2222 220a 2020 2020 2320 6c6f      """.    # lo
-00011a60: 6164 2063 6f6d 6d6f 6e20 7661 7269 6162  ad common variab
-00011a70: 6c65 7320 6672 6f6d 2064 6963 7469 6f6e  les from diction
-00011a80: 6172 790a 2020 2020 7477 696e 203d 2070  ary.    twin = p
-00011a90: 6172 615b 2274 7769 6e22 5d0a 2020 2020  ara["twin"].    
-00011aa0: 6672 6571 203d 2070 6172 615b 2266 7265  freq = para["fre
-00011ab0: 7122 5d0a 2020 2020 6474 203d 2070 6172  q"].    dt = par
-00011ac0: 615b 2264 7422 5d0a 2020 2020 746d 696e  a["dt"].    tmin
-00011ad0: 203d 206e 702e 6d69 6e28 7477 696e 290a   = np.min(twin).
-00011ae0: 2020 2020 746d 6178 203d 206e 702e 6d61      tmax = np.ma
-00011af0: 7828 7477 696e 290a 2020 2020 666d 696e  x(twin).    fmin
-00011b00: 203d 206e 702e 6d69 6e28 6672 6571 290a   = np.min(freq).
-00011b10: 2020 2020 666d 6178 203d 206e 702e 6d61      fmax = np.ma
-00011b20: 7828 6672 6571 290a 2020 2020 7476 6563  x(freq).    tvec
-00011b30: 203d 206e 702e 6172 616e 6765 2874 6d69   = np.arange(tmi
-00011b40: 6e2c 2074 6d61 782c 2064 7429 0a0a 2020  n, tmax, dt)..  
-00011b50: 2020 2320 6d61 6b65 2075 7365 6675 6c20    # make useful 
-00011b60: 6f6e 6520 666f 7220 6d65 6173 7572 656d  one for measurem
-00011b70: 656e 7473 0a20 2020 2064 766d 696e 203d  ents.    dvmin =
-00011b80: 202d 6e70 2e61 6273 2864 765f 7261 6e67   -np.abs(dv_rang
-00011b90: 6529 0a20 2020 2064 766d 6178 203d 206e  e).    dvmax = n
-00011ba0: 702e 6162 7328 6476 5f72 616e 6765 290a  p.abs(dv_range).
-00011bb0: 2020 2020 4570 7320 3d20 3120 2b20 286e      Eps = 1 + (n
-00011bc0: 702e 6c69 6e73 7061 6365 2864 766d 696e  p.linspace(dvmin
-00011bd0: 2c20 6476 6d61 782c 206e 6274 7269 616c  , dvmax, nbtrial
-00011be0: 2929 0a20 2020 2063 6f66 203d 206e 702e  )).    cof = np.
-00011bf0: 7a65 726f 7328 4570 732e 7368 6170 652c  zeros(Eps.shape,
-00011c00: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00011c10: 3229 0a0a 2020 2020 2320 5365 7420 6f66  2)..    # Set of
-00011c20: 2073 7472 6574 6368 6564 2f63 6f6d 7072   stretched/compr
-00011c30: 6573 7365 6420 6375 7272 656e 7420 7761  essed current wa
-00011c40: 7665 666f 726d 730a 2020 2020 666f 7220  veforms.    for 
-00011c50: 6969 2069 6e20 7261 6e67 6528 6c65 6e28  ii in range(len(
-00011c60: 4570 7329 293a 0a20 2020 2020 2020 206e  Eps)):.        n
-00011c70: 7420 3d20 7476 6563 202a 2045 7073 5b69  t = tvec * Eps[i
-00011c80: 695d 0a20 2020 2020 2020 2073 203d 206e  i].        s = n
-00011c90: 702e 696e 7465 7270 2878 3d74 7665 632c  p.interp(x=tvec,
-00011ca0: 2078 703d 6e74 2c20 6670 3d63 7572 290a   xp=nt, fp=cur).
-00011cb0: 2020 2020 2020 2020 7761 7665 666f 726d          waveform
-00011cc0: 5f72 6566 203d 2072 6566 0a20 2020 2020  _ref = ref.     
-00011cd0: 2020 2077 6176 6566 6f72 6d5f 6375 7220     waveform_cur 
-00011ce0: 3d20 730a 2020 2020 2020 2020 636f 665b  = s.        cof[
-00011cf0: 6969 5d20 3d20 6e70 2e63 6f72 7263 6f65  ii] = np.corrcoe
-00011d00: 6628 7761 7665 666f 726d 5f72 6566 2c20  f(waveform_ref, 
-00011d10: 7761 7665 666f 726d 5f63 7572 295b 302c  waveform_cur)[0,
-00011d20: 2031 5d0a 0a20 2020 2063 6470 203d 206e   1]..    cdp = n
-00011d30: 702e 636f 7272 636f 6566 2863 7572 2c20  p.corrcoef(cur, 
-00011d40: 7265 6629 5b30 2c20 315d 2020 2320 636f  ref)[0, 1]  # co
-00011d50: 7272 656c 6174 696f 6e20 636f 6566 6669  rrelation coeffi
-00011d60: 6369 656e 7420 6265 7477 6565 6e20 7468  cient between th
-00011d70: 6520 7265 6665 7265 6e63 6520 616e 6420  e reference and 
-00011d80: 696e 6974 6961 6c20 6375 7272 656e 7420  initial current 
-00011d90: 7761 7665 666f 726d 730a 0a20 2020 2023  waveforms..    #
-00011da0: 2066 696e 6420 7468 6520 6d61 7869 6d75   find the maximu
-00011db0: 6d20 636f 7272 656c 6174 696f 6e20 636f  m correlation co
-00011dc0: 6566 6669 6369 656e 740a 2020 2020 696d  efficient.    im
-00011dd0: 6178 203d 206e 702e 6e61 6e61 7267 6d61  ax = np.nanargma
-00011de0: 7828 636f 6629 0a20 2020 2069 6620 696d  x(cof).    if im
-00011df0: 6178 203e 3d20 6c65 6e28 4570 7329 202d  ax >= len(Eps) -
-00011e00: 2032 3a0a 2020 2020 2020 2020 696d 6178   2:.        imax
-00011e10: 203d 2069 6d61 7820 2d20 320a 2020 2020   = imax - 2.    
-00011e20: 6966 2069 6d61 7820 3c3d 2032 3a0a 2020  if imax <= 2:.  
-00011e30: 2020 2020 2020 696d 6178 203d 2069 6d61        imax = ima
-00011e40: 7820 2b20 320a 0a20 2020 2023 2050 726f  x + 2..    # Pro
-00011e50: 6365 6564 2074 6f20 7468 6520 7365 636f  ceed to the seco
-00011e60: 6e64 2073 7465 7020 746f 2067 6574 2061  nd step to get a
-00011e70: 206d 6f72 6520 7072 6563 6973 6520 6476   more precise dv
-00011e80: 2f76 206d 6561 7375 7265 6d65 6e74 0a20  /v measurement. 
-00011e90: 2020 2064 7466 696e 6572 203d 206e 702e     dtfiner = np.
-00011ea0: 6c69 6e73 7061 6365 2845 7073 5b69 6d61  linspace(Eps[ima
-00011eb0: 7820 2d20 325d 2c20 4570 735b 696d 6178  x - 2], Eps[imax
-00011ec0: 202b 2032 5d2c 2031 3030 290a 2020 2020   + 2], 100).    
-00011ed0: 6e63 6f66 203d 206e 702e 7a65 726f 7328  ncof = np.zeros(
-00011ee0: 6474 6669 6e65 722e 7368 6170 652c 2064  dtfiner.shape, d
-00011ef0: 7479 7065 3d6e 702e 666c 6f61 7433 3229  type=np.float32)
-00011f00: 0a20 2020 2066 6f72 2069 6920 696e 2072  .    for ii in r
-00011f10: 616e 6765 286c 656e 2864 7466 696e 6572  ange(len(dtfiner
-00011f20: 2929 3a0a 2020 2020 2020 2020 6e74 203d  )):.        nt =
-00011f30: 2074 7665 6320 2a20 6474 6669 6e65 725b   tvec * dtfiner[
-00011f40: 6969 5d0a 2020 2020 2020 2020 7320 3d20  ii].        s = 
-00011f50: 6e70 2e69 6e74 6572 7028 783d 7476 6563  np.interp(x=tvec
-00011f60: 2c20 7870 3d6e 742c 2066 703d 6375 7229  , xp=nt, fp=cur)
-00011f70: 0a20 2020 2020 2020 2077 6176 6566 6f72  .        wavefor
-00011f80: 6d5f 7265 6620 3d20 7265 660a 2020 2020  m_ref = ref.    
-00011f90: 2020 2020 7761 7665 666f 726d 5f63 7572      waveform_cur
-00011fa0: 203d 2073 0a20 2020 2020 2020 206e 636f   = s.        nco
-00011fb0: 665b 6969 5d20 3d20 6e70 2e63 6f72 7263  f[ii] = np.corrc
-00011fc0: 6f65 6628 7761 7665 666f 726d 5f72 6566  oef(waveform_ref
-00011fd0: 2c20 7761 7665 666f 726d 5f63 7572 295b  , waveform_cur)[
-00011fe0: 302c 2031 5d0a 0a20 2020 2063 6320 3d20  0, 1]..    cc = 
-00011ff0: 6e70 2e6d 6178 286e 636f 6629 2020 2320  np.max(ncof)  # 
-00012000: 4669 6e64 206d 6178 696d 756d 2063 6f72  Find maximum cor
-00012010: 7265 6c61 7469 6f6e 2063 6f65 6666 6963  relation coeffic
-00012020: 6965 6e74 206f 6620 7468 6520 7265 6669  ient of the refi
-00012030: 6e65 6420 2061 6e61 6c79 7369 730a 2020  ned  analysis.  
-00012040: 2020 6476 203d 2031 3030 2e30 202a 2064    dv = 100.0 * d
-00012050: 7466 696e 6572 5b6e 702e 6172 676d 6178  tfiner[np.argmax
-00012060: 286e 636f 6629 5d20 2d20 3130 3020 2023  (ncof)] - 100  #
-00012070: 204d 756c 7469 706c 7920 6279 2031 3030   Multiply by 100
-00012080: 2074 6f20 636f 6e76 6572 7420 746f 2070   to convert to p
-00012090: 6572 6365 6e74 6167 6520 2845 7073 696c  ercentage (Epsil
-000120a0: 6f6e 203d 202d 6474 2f74 203d 2064 762f  on = -dt/t = dv/
-000120b0: 7629 0a0a 2020 2020 2320 4572 726f 7220  v)..    # Error 
-000120c0: 636f 6d70 7574 6174 696f 6e20 6261 7365  computation base
-000120d0: 6420 6f6e 2057 6561 7665 7220 6574 2061  d on Weaver et a
-000120e0: 6c20 2832 3031 3129 2c20 4f6e 2074 6865  l (2011), On the
-000120f0: 2070 7265 6369 7369 6f6e 206f 6620 6e6f   precision of no
-00012100: 6973 652d 636f 7272 656c 6174 696f 6e0a  ise-correlation.
-00012110: 2020 2020 2320 696e 7465 7266 6572 6f6d      # interferom
-00012120: 6574 7279 2c20 4765 6f70 6879 732e 204a  etry, Geophys. J
-00012130: 2e20 496e 742e 2c20 3138 3528 3329 0a20  . Int., 185(3). 
-00012140: 2020 2054 203d 2031 202f 2028 666d 6178     T = 1 / (fmax
-00012150: 202d 2066 6d69 6e29 0a20 2020 2058 203d   - fmin).    X =
-00012160: 2063 630a 2020 2020 7763 203d 206e 702e   cc.    wc = np.
-00012170: 7069 202a 2028 666d 696e 202b 2066 6d61  pi * (fmin + fma
-00012180: 7829 0a20 2020 2074 3120 3d20 6e70 2e6d  x).    t1 = np.m
-00012190: 696e 285b 746d 696e 2c20 746d 6178 5d29  in([tmin, tmax])
-000121a0: 0a20 2020 2074 3220 3d20 6e70 2e6d 6178  .    t2 = np.max
-000121b0: 285b 746d 696e 2c20 746d 6178 5d29 0a20  ([tmin, tmax]). 
-000121c0: 2020 2065 7272 6f72 203d 2031 3030 202a     error = 100 *
-000121d0: 2028 0a20 2020 2020 2020 206e 702e 7371   (.        np.sq
-000121e0: 7274 2831 202d 2058 2a2a 3229 202f 2028  rt(1 - X**2) / (
-000121f0: 3220 2a20 5829 202a 206e 702e 7371 7274  2 * X) * np.sqrt
-00012200: 2828 3620 2a20 6e70 2e73 7172 7428 6e70  ((6 * np.sqrt(np
-00012210: 2e70 6920 2f20 3229 202a 2054 2920 2f20  .pi / 2) * T) / 
-00012220: 2877 632a 2a32 202a 2028 7432 2a2a 3320  (wc**2 * (t2**3 
-00012230: 2d20 7431 2a2a 3329 2929 0a20 2020 2029  - t1**3))).    )
-00012240: 0a0a 2020 2020 7265 7475 726e 2064 762c  ..    return dv,
-00012250: 2065 7272 6f72 2c20 6363 2c20 6364 700a   error, cc, cdp.
-00012260: 0a0a 6465 6620 7374 7265 7463 6869 6e67  ..def stretching
-00012270: 5f76 6563 7428 7265 662c 2063 7572 2c20  _vect(ref, cur, 
-00012280: 6476 5f72 616e 6765 2c20 6e62 7472 6961  dv_range, nbtria
-00012290: 6c2c 2070 6172 6129 3a0a 2020 2020 2222  l, para):.    ""
-000122a0: 220a 2020 2020 5468 6973 2066 756e 6374  ".    This funct
-000122b0: 696f 6e20 636f 6d70 6172 6573 2074 6865  ion compares the
-000122c0: 2052 6566 6572 656e 6365 2077 6176 6566   Reference wavef
-000122d0: 6f72 6d20 746f 2073 7472 6574 6368 6564  orm to stretched
-000122e0: 2f63 6f6d 7072 6573 7365 6420 6375 7272  /compressed curr
-000122f0: 656e 7420 7761 7665 666f 726d 730a 2020  ent waveforms.  
-00012300: 2020 746f 2067 6574 2074 6865 2072 656c    to get the rel
-00012310: 6174 6976 6520 7365 6973 6d69 6320 7665  ative seismic ve
-00012320: 6c6f 6369 7479 2076 6172 6961 7469 6f6e  locity variation
-00012330: 2028 616e 6420 6173 736f 6369 6174 6564   (and associated
-00012340: 2065 7272 6f72 292e 0a20 2020 2049 7420   error)..    It 
-00012350: 616c 736f 2063 6f6d 7075 7465 7320 7468  also computes th
-00012360: 6520 636f 7272 656c 6174 696f 6e20 636f  e correlation co
-00012370: 6566 6669 6369 656e 7420 6265 7477 6565  efficient betwee
-00012380: 6e20 7468 6520 5265 6665 7265 6e63 6520  n the Reference 
-00012390: 7761 7665 666f 726d 2061 6e64 2074 6865  waveform and the
-000123a0: 2063 7572 7265 6e74 2077 6176 6566 6f72   current wavefor
-000123b0: 6d2e 0a0a 2020 2020 5041 5241 4d45 5445  m...    PARAMETE
-000123c0: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
-000123d0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2072 6566  --------.    ref
-000123e0: 3a20 5265 6665 7265 6e63 6520 7761 7665  : Reference wave
-000123f0: 666f 726d 2028 6e70 2e6e 6461 7272 6179  form (np.ndarray
-00012400: 2c20 7369 7a65 204e 290a 2020 2020 6375  , size N).    cu
-00012410: 723a 2043 7572 7265 6e74 2077 6176 6566  r: Current wavef
-00012420: 6f72 6d20 286e 702e 6e64 6172 7261 792c  orm (np.ndarray,
-00012430: 2073 697a 6520 4e29 0a20 2020 2064 765f   size N).    dv_
-00012440: 7261 6e67 653a 2061 6273 6f6c 7574 6520  range: absolute 
-00012450: 626f 756e 6420 666f 7220 7468 6520 7665  bound for the ve
-00012460: 6c6f 6369 7479 2076 6172 6961 7469 6f6e  locity variation
-00012470: 3b20 6578 616d 706c 653a 2064 763d 302e  ; example: dv=0.
-00012480: 3033 2066 6f72 205b 2d33 2c33 5d25 0a20  03 for [-3,3]%. 
-00012490: 2020 206f 6620 7265 6c61 7469 7665 2076     of relative v
-000124a0: 656c 6f63 6974 7920 6368 616e 6765 2028  elocity change (
-000124b0: 2766 6c6f 6174 2729 0a20 2020 206e 6274  'float').    nbt
-000124c0: 7269 616c 3a20 6e75 6d62 6572 206f 6620  rial: number of 
-000124d0: 7374 7265 7463 6869 6e67 2063 6f65 6666  stretching coeff
-000124e0: 6963 6965 6e74 2062 6574 7765 656e 2064  icient between d
-000124f0: 766d 696e 2061 6e64 2064 766d 6178 2c20  vmin and dvmax, 
-00012500: 6e6f 206e 6565 6420 746f 2062 6520 6869  no need to be hi
-00012510: 6768 6572 2074 6861 6e20 3130 3020 2028  gher than 100  (
-00012520: 2766 6c6f 6174 2729 0a20 2020 2070 6172  'float').    par
-00012530: 613a 2076 6563 746f 7220 6f66 2074 6865  a: vector of the
-00012540: 2069 6e64 6963 6573 206f 6620 7468 6520   indices of the 
-00012550: 6375 7220 616e 6420 7265 6620 7769 6e64  cur and ref wind
-00012560: 6f77 7320 6f6e 2077 6963 6820 796f 7520  ows on wich you 
-00012570: 7761 6e74 2074 6f20 646f 2074 6865 0a20  want to do the. 
-00012580: 2020 206d 6561 7375 7265 6d65 6e74 7320     measurements 
-00012590: 286e 702e 6e64 6172 7261 792c 2073 697a  (np.ndarray, siz
-000125a0: 6520 746d 696e 2a64 656c 7461 3a74 6d61  e tmin*delta:tma
-000125b0: 782a 6465 6c74 6129 0a20 2020 2046 6f72  x*delta).    For
-000125c0: 2065 7272 6f72 2063 6f6d 7075 7461 7469   error computati
-000125d0: 6f6e 2c20 7765 206e 6565 6420 7061 7261  on, we need para
-000125e0: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
-000125f0: 666d 696e 3a20 6d69 6e69 6d75 6d20 6672  fmin: minimum fr
-00012600: 6571 7565 6e63 7920 6f66 2074 6865 2064  equency of the d
-00012610: 6174 610a 2020 2020 2020 2020 666d 6178  ata.        fmax
-00012620: 3a20 6d61 7869 6d75 6d20 6672 6571 7565  : maximum freque
-00012630: 6e63 7920 6f66 2074 6865 2064 6174 610a  ncy of the data.
-00012640: 2020 2020 2020 2020 746d 696e 3a20 6d69          tmin: mi
-00012650: 6e69 6d75 6d20 7469 6d65 2077 696e 646f  nimum time windo
-00012660: 7720 7768 6572 6520 7468 6520 6476 2f76  w where the dv/v
-00012670: 2069 7320 636f 6d70 7574 6564 0a20 2020   is computed.   
-00012680: 2020 2020 2074 6d61 783a 206d 6178 696d       tmax: maxim
-00012690: 756d 2074 696d 6520 7769 6e64 6f77 2077  um time window w
-000126a0: 6865 7265 2074 6865 2064 762f 7620 6973  here the dv/v is
-000126b0: 2063 6f6d 7075 7465 640a 2020 2020 5245   computed.    RE
-000126c0: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
-000126d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-000126e0: 6476 3a20 5265 6c61 7469 7665 2076 656c  dv: Relative vel
-000126f0: 6f63 6974 7920 6368 616e 6765 2064 762f  ocity change dv/
-00012700: 7620 2869 6e20 2529 0a20 2020 2063 633a  v (in %).    cc:
-00012710: 2063 6f72 7265 6c61 7469 6f6e 2063 6f65   correlation coe
-00012720: 6666 6963 6965 6e74 2062 6574 7765 656e  fficient between
-00012730: 2074 6865 2072 6566 6572 656e 6365 2077   the reference w
-00012740: 6176 6566 6f72 6d20 616e 6420 7468 6520  aveform and the 
-00012750: 6265 7374 2073 7472 6574 6368 6564 2f63  best stretched/c
-00012760: 6f6d 7072 6573 7365 6420 6375 7272 656e  ompressed curren
-00012770: 7420 7761 7665 666f 726d 0a20 2020 2063  t waveform.    c
-00012780: 6470 3a20 636f 7272 656c 6174 696f 6e20  dp: correlation 
-00012790: 636f 6566 6669 6369 656e 7420 6265 7477  coefficient betw
-000127a0: 6565 6e20 7468 6520 7265 6665 7265 6e63  een the referenc
-000127b0: 6520 7761 7665 666f 726d 2061 6e64 2074  e waveform and t
-000127c0: 6865 2069 6e69 7469 616c 2063 7572 7265  he initial curre
-000127d0: 6e74 2077 6176 6566 6f72 6d0a 2020 2020  nt waveform.    
-000127e0: 6572 726f 723a 2045 7272 6f72 7320 696e  error: Errors in
-000127f0: 2074 6865 2064 762f 7620 6d65 6173 7572   the dv/v measur
-00012800: 656d 656e 7473 2062 6173 6564 206f 6e20  ements based on 
-00012810: 5765 6176 6572 2065 7420 616c 2028 3230  Weaver et al (20
-00012820: 3131 292c 204f 6e20 7468 6520 7072 6563  11), On the prec
-00012830: 6973 696f 6e0a 2020 2020 6f66 206e 6f69  ision.    of noi
-00012840: 7365 2d63 6f72 7265 6c61 7469 6f6e 2069  se-correlation i
-00012850: 6e74 6572 6665 726f 6d65 7472 792c 2047  nterferometry, G
-00012860: 656f 7068 7973 2e20 4a2e 2049 6e74 2e2c  eophys. J. Int.,
-00012870: 2031 3835 2833 290a 0a20 2020 204e 6f74   185(3)..    Not
-00012880: 653a 2054 6865 2063 6f64 6520 6669 7273  e: The code firs
-00012890: 7420 6669 6e64 7320 7468 6520 6265 7374  t finds the best
-000128a0: 2063 6f72 7265 6c61 7469 6f6e 2063 6f65   correlation coe
-000128b0: 6666 6963 6965 6e74 2062 6574 7765 656e  fficient between
-000128c0: 2074 6865 2052 6566 6572 656e 6365 2077   the Reference w
-000128d0: 6176 6566 6f72 6d20 616e 640a 2020 2020  aveform and.    
-000128e0: 7468 6520 7374 7265 7463 6865 642f 636f  the stretched/co
-000128f0: 6d70 7265 7373 6564 2063 7572 7265 6e74  mpressed current
-00012900: 2077 6176 6566 6f72 6d20 616d 6f6e 6720   waveform among 
-00012910: 7468 6520 226e 6274 7269 616c 2220 7661  the "nbtrial" va
-00012920: 6c75 6573 2e0a 2020 2020 4120 7265 6669  lues..    A refi
-00012930: 6e65 6420 616e 616c 7973 6973 2069 7320  ned analysis is 
-00012940: 7468 656e 2070 6572 666f 726d 6564 2061  then performed a
-00012950: 726f 756e 6420 7468 6973 2076 616c 7565  round this value
-00012960: 2074 6f20 6f62 7461 696e 2061 206d 6f72   to obtain a mor
-00012970: 6520 7072 6563 6973 6520 6476 2f76 206d  e precise dv/v m
-00012980: 6561 7375 7265 6d65 6e74 202e 0a0a 2020  easurement ...  
-00012990: 2020 4f72 6967 696e 616c 6c79 2062 7920    Originally by 
-000129a0: 4c2e 2056 6965 6e73 2030 342f 3236 2f32  L. Viens 04/26/2
-000129b0: 3031 3820 2856 6965 6e73 2065 7420 616c  018 (Viens et al
-000129c0: 2e2c 2032 3031 3820 4a47 5229 0a20 2020  ., 2018 JGR).   
-000129d0: 206d 6f64 6966 6965 6420 6279 2043 6865   modified by Che
-000129e0: 6e67 7869 6e20 4a69 616e 670a 2020 2020  ngxin Jiang.    
-000129f0: 6d6f 6469 6669 6564 2062 7920 4c61 7572  modified by Laur
-00012a00: 6120 4572 6d65 7274 3a20 7665 6374 6f72  a Ermert: vector
-00012a10: 697a 6564 2076 6572 7369 6f6e 0a20 2020  ized version.   
-00012a20: 2022 2222 0a20 2020 2023 206c 6f61 6420   """.    # load 
-00012a30: 636f 6d6d 6f6e 2076 6172 6961 626c 6573  common variables
-00012a40: 2066 726f 6d20 6469 6374 696f 6e61 7279   from dictionary
-00012a50: 0a20 2020 2074 7769 6e20 3d20 7061 7261  .    twin = para
-00012a60: 5b22 7477 696e 225d 0a20 2020 2066 7265  ["twin"].    fre
-00012a70: 7120 3d20 7061 7261 5b22 6672 6571 225d  q = para["freq"]
-00012a80: 0a20 2020 2064 7420 3d20 7061 7261 5b22  .    dt = para["
-00012a90: 6474 225d 0a20 2020 2074 6d69 6e20 3d20  dt"].    tmin = 
-00012aa0: 6e70 2e6d 696e 2874 7769 6e29 0a20 2020  np.min(twin).   
-00012ab0: 2074 6d61 7820 3d20 6e70 2e6d 6178 2874   tmax = np.max(t
-00012ac0: 7769 6e29 0a20 2020 2066 6d69 6e20 3d20  win).    fmin = 
-00012ad0: 6e70 2e6d 696e 2866 7265 7129 0a20 2020  np.min(freq).   
-00012ae0: 2066 6d61 7820 3d20 6e70 2e6d 6178 2866   fmax = np.max(f
-00012af0: 7265 7129 0a20 2020 2074 7665 6320 3d20  req).    tvec = 
-00012b00: 6e70 2e61 7261 6e67 6528 746d 696e 2c20  np.arange(tmin, 
-00012b10: 746d 6178 2c20 6474 290a 0a20 2020 2023  tmax, dt)..    #
-00012b20: 206d 616b 6520 7573 6566 756c 206f 6e65   make useful one
-00012b30: 2066 6f72 206d 6561 7375 7265 6d65 6e74   for measurement
-00012b40: 730a 2020 2020 6476 6d69 6e20 3d20 2d6e  s.    dvmin = -n
-00012b50: 702e 6162 7328 6476 5f72 616e 6765 290a  p.abs(dv_range).
-00012b60: 2020 2020 6476 6d61 7820 3d20 6e70 2e61      dvmax = np.a
-00012b70: 6273 2864 765f 7261 6e67 6529 0a20 2020  bs(dv_range).   
-00012b80: 2045 7073 203d 2031 202b 2028 6e70 2e6c   Eps = 1 + (np.l
-00012b90: 696e 7370 6163 6528 6476 6d69 6e2c 2064  inspace(dvmin, d
-00012ba0: 766d 6178 2c20 6e62 7472 6961 6c29 290a  vmax, nbtrial)).
-00012bb0: 2020 2020 6364 7020 3d20 6e70 2e63 6f72      cdp = np.cor
-00012bc0: 7263 6f65 6628 6375 722c 2072 6566 295b  rcoef(cur, ref)[
-00012bd0: 302c 2031 5d20 2023 2063 6f72 7265 6c61  0, 1]  # correla
-00012be0: 7469 6f6e 2063 6f65 6666 6963 6965 6e74  tion coefficient
-00012bf0: 2062 6574 7765 656e 2074 6865 2072 6566   between the ref
-00012c00: 6572 656e 6365 2061 6e64 2069 6e69 7469  erence and initi
-00012c10: 616c 2063 7572 7265 6e74 2077 6176 6566  al current wavef
-00012c20: 6f72 6d73 0a20 2020 2077 6176 6566 6f72  orms.    wavefor
-00012c30: 6d73 203d 206e 702e 7a65 726f 7328 286e  ms = np.zeros((n
-00012c40: 6274 7269 616c 202b 2031 2c20 6c65 6e28  btrial + 1, len(
-00012c50: 7265 6629 2929 0a20 2020 2077 6176 6566  ref))).    wavef
-00012c60: 6f72 6d73 5b30 2c20 3a5d 203d 2072 6566  orms[0, :] = ref
-00012c70: 0a0a 2020 2020 2320 5365 7420 6f66 2073  ..    # Set of s
-00012c80: 7472 6574 6368 6564 2f63 6f6d 7072 6573  tretched/compres
-00012c90: 7365 6420 6375 7272 656e 7420 7761 7665  sed current wave
-00012ca0: 666f 726d 730a 2020 2020 666f 7220 6969  forms.    for ii
-00012cb0: 2069 6e20 7261 6e67 6528 6e62 7472 6961   in range(nbtria
-00012cc0: 6c29 3a0a 2020 2020 2020 2020 6e74 203d  l):.        nt =
-00012cd0: 2074 7665 6320 2a20 4570 735b 6969 5d0a   tvec * Eps[ii].
-00012ce0: 2020 2020 2020 2020 7320 3d20 6e70 2e69          s = np.i
-00012cf0: 6e74 6572 7028 783d 7476 6563 2c20 7870  nterp(x=tvec, xp
-00012d00: 3d6e 742c 2066 703d 6375 7229 0a20 2020  =nt, fp=cur).   
-00012d10: 2020 2020 2077 6176 6566 6f72 6d73 5b69       waveforms[i
-00012d20: 6920 2b20 312c 203a 5d20 3d20 730a 2020  i + 1, :] = s.  
-00012d30: 2020 636f 6620 3d20 6e70 2e63 6f72 7263    cof = np.corrc
-00012d40: 6f65 6628 7761 7665 666f 726d 7329 5b30  oef(waveforms)[0
-00012d50: 5d5b 313a 5d0a 0a20 2020 2023 2066 696e  ][1:]..    # fin
-00012d60: 6420 7468 6520 6d61 7869 6d75 6d20 636f  d the maximum co
-00012d70: 7272 656c 6174 696f 6e20 636f 6566 6669  rrelation coeffi
-00012d80: 6369 656e 740a 2020 2020 696d 6178 203d  cient.    imax =
-00012d90: 206e 702e 6e61 6e61 7267 6d61 7828 636f   np.nanargmax(co
-00012da0: 6629 0a20 2020 2069 6620 696d 6178 203e  f).    if imax >
-00012db0: 3d20 6c65 6e28 4570 7329 202d 2032 3a0a  = len(Eps) - 2:.
-00012dc0: 2020 2020 2020 2020 696d 6178 203d 2069          imax = i
-00012dd0: 6d61 7820 2d20 320a 2020 2020 6966 2069  max - 2.    if i
-00012de0: 6d61 7820 3c20 323a 0a20 2020 2020 2020  max < 2:.       
-00012df0: 2069 6d61 7820 3d20 696d 6178 202b 2032   imax = imax + 2
-00012e00: 0a0a 2020 2020 2320 5072 6f63 6565 6420  ..    # Proceed 
-00012e10: 746f 2074 6865 2073 6563 6f6e 6420 7374  to the second st
-00012e20: 6570 2074 6f20 6765 7420 6120 6d6f 7265  ep to get a more
-00012e30: 2070 7265 6369 7365 2064 762f 7620 6d65   precise dv/v me
-00012e40: 6173 7572 656d 656e 740a 2020 2020 6474  asurement.    dt
-00012e50: 6669 6e65 7220 3d20 6e70 2e6c 696e 7370  finer = np.linsp
-00012e60: 6163 6528 4570 735b 696d 6178 202d 2032  ace(Eps[imax - 2
-00012e70: 5d2c 2045 7073 5b69 6d61 7820 2b20 325d  ], Eps[imax + 2]
-00012e80: 2c20 6e62 7472 6961 6c29 0a20 2020 2023  , nbtrial).    #
-00012e90: 206e 636f 6620 2020 203d 206e 702e 7a65   ncof    = np.ze
-00012ea0: 726f 7328 6474 6669 6e65 722e 7368 6170  ros(dtfiner.shap
-00012eb0: 652c 6474 7970 653d 6e70 2e66 6c6f 6174  e,dtype=np.float
-00012ec0: 3332 290a 2020 2020 7761 7665 666f 726d  32).    waveform
-00012ed0: 7320 3d20 6e70 2e7a 6572 6f73 2828 6e62  s = np.zeros((nb
-00012ee0: 7472 6961 6c20 2b20 312c 206c 656e 2872  trial + 1, len(r
-00012ef0: 6566 2929 290a 2020 2020 7761 7665 666f  ef))).    wavefo
-00012f00: 726d 735b 302c 203a 5d20 3d20 7265 660a  rms[0, :] = ref.
-00012f10: 2020 2020 666f 7220 6969 2069 6e20 7261      for ii in ra
-00012f20: 6e67 6528 6c65 6e28 6474 6669 6e65 7229  nge(len(dtfiner)
-00012f30: 293a 0a20 2020 2020 2020 206e 7420 3d20  ):.        nt = 
-00012f40: 7476 6563 202a 2064 7466 696e 6572 5b69  tvec * dtfiner[i
-00012f50: 695d 0a20 2020 2020 2020 2073 203d 206e  i].        s = n
-00012f60: 702e 696e 7465 7270 2878 3d74 7665 632c  p.interp(x=tvec,
-00012f70: 2078 703d 6e74 2c20 6670 3d63 7572 290a   xp=nt, fp=cur).
-00012f80: 2020 2020 2020 2020 7761 7665 666f 726d          waveform
-00012f90: 735b 6969 202b 2031 2c20 3a5d 203d 2073  s[ii + 1, :] = s
-00012fa0: 0a20 2020 206e 636f 6620 3d20 6e70 2e63  .    ncof = np.c
-00012fb0: 6f72 7263 6f65 6628 7761 7665 666f 726d  orrcoef(waveform
-00012fc0: 7329 5b30 5d5b 313a 5d0a 2020 2020 6363  s)[0][1:].    cc
-00012fd0: 203d 206e 702e 6d61 7828 6e63 6f66 2920   = np.max(ncof) 
-00012fe0: 2023 2046 696e 6420 6d61 7869 6d75 6d20   # Find maximum 
-00012ff0: 636f 7272 656c 6174 696f 6e20 636f 6566  correlation coef
-00013000: 6669 6369 656e 7420 6f66 2074 6865 2072  ficient of the r
-00013010: 6566 696e 6564 2020 616e 616c 7973 6973  efined  analysis
-00013020: 0a20 2020 2064 7620 3d20 3130 302e 3020  .    dv = 100.0 
-00013030: 2a20 6474 6669 6e65 725b 6e70 2e61 7267  * dtfiner[np.arg
-00013040: 6d61 7828 6e63 6f66 295d 202d 2031 3030  max(ncof)] - 100
-00013050: 2020 2320 4d75 6c74 6970 6c79 2062 7920    # Multiply by 
-00013060: 3130 3020 746f 2063 6f6e 7665 7274 2074  100 to convert t
-00013070: 6f20 7065 7263 656e 7461 6765 2028 4570  o percentage (Ep
-00013080: 7369 6c6f 6e20 3d20 2d64 742f 7420 3d20  silon = -dt/t = 
-00013090: 6476 2f76 290a 0a20 2020 2023 2045 7272  dv/v)..    # Err
-000130a0: 6f72 2063 6f6d 7075 7461 7469 6f6e 2062  or computation b
-000130b0: 6173 6564 206f 6e20 5765 6176 6572 2065  ased on Weaver e
-000130c0: 7420 616c 2028 3230 3131 292c 204f 6e20  t al (2011), On 
-000130d0: 7468 6520 7072 6563 6973 696f 6e20 6f66  the precision of
-000130e0: 206e 6f69 7365 2d63 6f72 7265 6c61 7469   noise-correlati
-000130f0: 6f6e 2069 6e74 6572 6665 726f 6d65 7472  on interferometr
-00013100: 792c 0a20 2020 2023 2047 656f 7068 7973  y,.    # Geophys
-00013110: 2e20 4a2e 2049 6e74 2e2c 2031 3835 2833  . J. Int., 185(3
-00013120: 290a 2020 2020 5420 3d20 3120 2f20 2866  ).    T = 1 / (f
-00013130: 6d61 7820 2d20 666d 696e 290a 2020 2020  max - fmin).    
-00013140: 5820 3d20 6363 0a20 2020 2077 6320 3d20  X = cc.    wc = 
-00013150: 6e70 2e70 6920 2a20 2866 6d69 6e20 2b20  np.pi * (fmin + 
-00013160: 666d 6178 290a 2020 2020 7431 203d 206e  fmax).    t1 = n
-00013170: 702e 6d69 6e28 5b74 6d69 6e2c 2074 6d61  p.min([tmin, tma
-00013180: 785d 290a 2020 2020 7432 203d 206e 702e  x]).    t2 = np.
-00013190: 6d61 7828 5b74 6d69 6e2c 2074 6d61 785d  max([tmin, tmax]
-000131a0: 290a 2020 2020 6572 726f 7220 3d20 3130  ).    error = 10
-000131b0: 3020 2a20 280a 2020 2020 2020 2020 6e70  0 * (.        np
-000131c0: 2e73 7172 7428 3120 2d20 582a 2a32 2920  .sqrt(1 - X**2) 
-000131d0: 2f20 2832 202a 2058 2920 2a20 6e70 2e73  / (2 * X) * np.s
-000131e0: 7172 7428 2836 202a 206e 702e 7371 7274  qrt((6 * np.sqrt
-000131f0: 286e 702e 7069 202f 2032 2920 2a20 5429  (np.pi / 2) * T)
-00013200: 202f 2028 7763 2a2a 3220 2a20 2874 322a   / (wc**2 * (t2*
-00013210: 2a33 202d 2074 312a 2a33 2929 290a 2020  *3 - t1**3))).  
-00013220: 2020 290a 0a20 2020 2072 6574 7572 6e20    )..    return 
-00013230: 6476 2c20 6572 726f 722c 2063 632c 2063  dv, error, cc, c
-00013240: 6470 0a0a 0a64 6566 2064 7477 5f64 7676  dp...def dtw_dvv
-00013250: 2872 6566 2c20 6375 722c 2070 6172 612c  (ref, cur, para,
-00013260: 206d 6178 4c61 672c 2062 2c20 6469 7265   maxLag, b, dire
-00013270: 6374 696f 6e29 3a0a 2020 2020 2222 220a  ction):.    """.
-00013280: 2020 2020 4479 6e61 6d69 6320 7469 6d65      Dynamic time
-00013290: 2077 6172 7069 6e67 2066 6f72 2064 762f   warping for dv/
-000132a0: 7620 6573 7469 6d61 7469 6f6e 2e0a 0a20  v estimation... 
-000132b0: 2020 2050 4152 414d 4554 4552 533a 0a20     PARAMETERS:. 
-000132c0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-000132d0: 2d2d 2d0a 2020 2020 7265 6620 3a20 7265  ---.    ref : re
-000132e0: 6665 7265 6e63 6520 7369 676e 616c 2028  ference signal (
-000132f0: 6e70 2e61 7272 6179 2c20 7369 7a65 204e  np.array, size N
-00013300: 290a 2020 2020 6375 7220 3a20 6375 7272  ).    cur : curr
-00013310: 656e 7420 7369 676e 616c 2028 6e70 2e61  ent signal (np.a
-00013320: 7272 6179 2c20 7369 7a65 204e 290a 2020  rray, size N).  
-00013330: 2020 7061 7261 3a20 6469 6374 2063 6f6e    para: dict con
-00013340: 7461 696e 696e 6720 7573 6566 756c 2070  taining useful p
-00013350: 6172 616d 6574 6572 7320 6162 6f75 7420  arameters about 
-00013360: 7468 6520 6461 7461 2077 696e 646f 7720  the data window 
-00013370: 616e 6420 7461 7267 6574 6564 2066 7265  and targeted fre
-00013380: 7175 656e 6379 0a20 2020 206d 6178 4c61  quency.    maxLa
-00013390: 6720 3a20 6d61 7820 6e75 6d62 6572 206f  g : max number o
-000133a0: 6620 706f 696e 7473 2074 6f20 7365 6172  f points to sear
-000133b0: 6368 2066 6f72 7761 7264 2061 6e64 2062  ch forward and b
-000133c0: 6163 6b77 6172 642e 0a20 2020 2020 2020  ackward..       
-000133d0: 2020 2020 2053 7567 6765 7374 2073 6574       Suggest set
-000133e0: 7469 6e67 2069 7420 6c61 7267 6572 2069  ting it larger i
-000133f0: 6620 7769 6e64 6f77 2069 7320 7365 7420  f window is set 
-00013400: 6c61 7267 6572 2e0a 2020 2020 6220 3a20  larger..    b : 
-00013410: 622d 7661 6c75 6520 746f 206c 696d 6974  b-value to limit
-00013420: 2073 7472 6169 6e2c 2077 6869 6368 2069   strain, which i
-00013430: 7320 746f 206c 696d 6974 2074 6865 206d  s to limit the m
-00013440: 6178 696d 756d 2076 656c 6f63 6974 7920  aximum velocity 
-00013450: 7065 7274 7572 6261 7469 6f6e 2e0a 2020  perturbation..  
-00013460: 2020 2020 2020 2020 2020 5365 6520 6571            See eq
-00013470: 7561 7469 6f6e 2031 3120 696e 2028 4d69  uation 11 in (Mi
-00013480: 6b65 7365 6c6c 2065 7420 616c 2e20 3230  kesell et al. 20
-00013490: 3135 290a 2020 2020 6469 7265 6374 696f  15).    directio
-000134a0: 6e3a 2064 6972 6563 7469 6f6e 2074 6f20  n: direction to 
-000134b0: 6163 6375 6d75 6c61 7465 2065 7272 6f72  accumulate error
-000134c0: 7320 2831 3d66 6f72 7761 7264 2c20 2d31  s (1=forward, -1
-000134d0: 3d62 6163 6b77 6172 6429 0a20 2020 2052  =backward).    R
-000134e0: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
-000134f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-00013500: 2020 202d 6d30 203a 2065 7374 696d 6174     -m0 : estimat
-00013510: 6564 2064 762f 760a 2020 2020 656d 3020  ed dv/v.    em0 
-00013520: 3a20 6572 726f 7220 6f66 2064 762f 7620  : error of dv/v 
-00013530: 6573 7469 6d61 7469 6f6e 0a0a 2020 2020  estimation..    
-00013540: 4f72 6967 696e 616c 2062 7920 4469 2059  Original by Di Y
-00013550: 616e 670a 2020 2020 4c61 7374 206d 6f64  ang.    Last mod
-00013560: 6966 6965 6420 6279 2044 796c 616e 204d  ified by Dylan M
-00013570: 696b 6573 656c 6c20 2832 3520 4665 622e  ikesell (25 Feb.
-00013580: 2032 3031 3529 0a20 2020 2054 7261 6e73   2015).    Trans
-00013590: 6c61 7465 6420 746f 2070 7974 686f 6e20  lated to python 
-000135a0: 6279 2054 696d 2043 6c65 6d65 6e74 7320  by Tim Clements 
-000135b0: 2831 3720 4175 672e 2032 3031 3829 0a20  (17 Aug. 2018). 
-000135c0: 2020 2022 2222 0a20 2020 2074 7769 6e20     """.    twin 
-000135d0: 3d20 7061 7261 5b22 7477 696e 225d 0a20  = para["twin"]. 
-000135e0: 2020 2064 7420 3d20 7061 7261 5b22 6474     dt = para["dt
-000135f0: 225d 0a20 2020 2074 6d69 6e20 3d20 6e70  "].    tmin = np
-00013600: 2e6d 696e 2874 7769 6e29 0a20 2020 2074  .min(twin).    t
-00013610: 6d61 7820 3d20 6e70 2e6d 6178 2874 7769  max = np.max(twi
-00013620: 6e29 0a20 2020 2074 7665 6374 203d 206e  n).    tvect = n
-00013630: 702e 6172 616e 6765 2874 6d69 6e2c 2074  p.arange(tmin, t
-00013640: 6d61 782c 2064 7429 0a0a 2020 2020 2320  max, dt)..    # 
-00013650: 7365 7475 7020 6f74 6865 7220 7061 7261  setup other para
-00013660: 6d65 7465 7273 0a20 2020 206e 7074 7320  meters.    npts 
-00013670: 3d20 6c65 6e28 7265 6629 2020 2320 6e75  = len(ref)  # nu
-00013680: 6d62 6572 206f 6620 7469 6d65 2073 616d  mber of time sam
-00013690: 706c 6573 0a0a 2020 2020 2320 636f 6d70  ples..    # comp
-000136a0: 7574 6520 6572 726f 7220 6675 6e63 7469  ute error functi
-000136b0: 6f6e 206f 7665 7220 6c61 6773 2c20 7768  on over lags, wh
-000136c0: 6963 6820 6973 2069 6e64 6570 656e 6465  ich is independe
-000136d0: 6e74 206f 6620 7374 7261 696e 206c 696d  nt of strain lim
-000136e0: 6974 2027 6227 2e0a 2020 2020 6572 7220  it 'b'..    err 
-000136f0: 3d20 636f 6d70 7574 6545 7272 6f72 4675  = computeErrorFu
-00013700: 6e63 7469 6f6e 2863 7572 2c20 7265 662c  nction(cur, ref,
-00013710: 206e 7074 732c 206d 6178 4c61 6729 0a0a   npts, maxLag)..
-00013720: 2020 2020 2320 6469 7265 6374 696f 6e20      # direction 
-00013730: 746f 2061 6363 756d 756c 6174 6520 6572  to accumulate er
-00013740: 726f 7273 2028 313d 666f 7277 6172 642c  rors (1=forward,
-00013750: 202d 313d 6261 636b 7761 7264 290a 2020   -1=backward).  
-00013760: 2020 6469 7374 203d 2061 6363 756d 756c    dist = accumul
-00013770: 6174 6545 7272 6f72 4675 6e63 7469 6f6e  ateErrorFunction
-00013780: 2864 6972 6563 7469 6f6e 2c20 6572 722c  (direction, err,
-00013790: 206e 7074 732c 206d 6178 4c61 672c 2062   npts, maxLag, b
-000137a0: 290a 2020 2020 7374 6261 7220 3d20 6261  ).    stbar = ba
-000137b0: 636b 7472 6163 6b44 6973 7461 6e63 6546  cktrackDistanceF
-000137c0: 756e 6374 696f 6e28 2d31 202a 2064 6972  unction(-1 * dir
-000137d0: 6563 7469 6f6e 2c20 6469 7374 2c20 6572  ection, dist, er
-000137e0: 722c 202d 6d61 784c 6167 2c20 6229 0a20  r, -maxLag, b). 
-000137f0: 2020 2073 7462 6172 5469 6d65 203d 2073     stbarTime = s
-00013800: 7462 6172 202a 2064 7420 2023 2063 6f6e  tbar * dt  # con
-00013810: 7665 7274 2066 726f 6d20 7361 6d70 6c65  vert from sample
-00013820: 7320 746f 2074 696d 650a 0a20 2020 2023  s to time..    #
-00013830: 2063 7574 2074 6865 2066 6972 7374 2061   cut the first a
-00013840: 6e64 206c 6173 7420 3525 2066 6f72 2062  nd last 5% for b
-00013850: 6574 7465 7220 7265 6772 6573 7369 6f6e  etter regression
-00013860: 0a20 2020 2069 6e64 7820 3d20 6e70 2e77  .    indx = np.w
-00013870: 6865 7265 2828 7476 6563 7420 3e3d 2030  here((tvect >= 0
-00013880: 2e30 3520 2a20 6e70 7473 202a 2064 7429  .05 * npts * dt)
-00013890: 2026 2028 7476 6563 7420 3c3d 2030 2e39   & (tvect <= 0.9
-000138a0: 3520 2a20 6e70 7473 202a 2064 7429 295b  5 * npts * dt))[
-000138b0: 305d 0a0a 2020 2020 2320 6c69 6e65 6172  0]..    # linear
-000138c0: 2072 6567 7265 7373 696f 6e20 746f 2067   regression to g
-000138d0: 6574 2064 762f 760a 2020 2020 6966 206e  et dv/v.    if n
-000138e0: 7074 7320 3e20 323a 0a20 2020 2020 2020  pts > 2:.       
-000138f0: 2023 2077 6569 6768 7473 0a20 2020 2020   # weights.     
-00013900: 2020 2077 203d 206e 702e 6f6e 6573 286e     w = np.ones(n
-00013910: 7074 7329 0a20 2020 2020 2020 2023 206d  pts).        # m
-00013920: 2c20 612c 2065 6d2c 2065 6120 3d20 6c69  , a, em, ea = li
-00013930: 6e65 6172 5f72 6567 7265 7373 696f 6e28  near_regression(
-00013940: 7469 6d65 5f61 7869 735b 696e 6478 5d2c  time_axis[indx],
-00013950: 2064 656c 7461 5f74 5b69 6e64 785d 2c20   delta_t[indx], 
-00013960: 772c 2069 6e74 6572 6365 7074 5f6f 7269  w, intercept_ori
-00013970: 6769 6e3d 4661 6c73 6529 0a20 2020 2020  gin=False).     
-00013980: 2020 206d 302c 2065 6d30 203d 206c 696e     m0, em0 = lin
-00013990: 6561 725f 7265 6772 6573 7369 6f6e 280a  ear_regression(.
-000139a0: 2020 2020 2020 2020 2020 2020 7476 6563              tvec
-000139b0: 742e 666c 6174 7465 6e28 295b 696e 6478  t.flatten()[indx
-000139c0: 5d2c 0a20 2020 2020 2020 2020 2020 2073  ],.            s
-000139d0: 7462 6172 5469 6d65 2e66 6c61 7474 656e  tbarTime.flatten
-000139e0: 2829 5b69 6e64 785d 2c0a 2020 2020 2020  ()[indx],.      
-000139f0: 2020 2020 2020 772e 666c 6174 7465 6e28        w.flatten(
-00013a00: 295b 696e 6478 5d2c 0a20 2020 2020 2020  )[indx],.       
-00013a10: 2020 2020 2069 6e74 6572 6365 7074 5f6f       intercept_o
-00013a20: 7269 6769 6e3d 5472 7565 2c0a 2020 2020  rigin=True,.    
-00013a30: 2020 2020 290a 0a20 2020 2065 6c73 653a      )..    else:
-00013a40: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
-00013a50: 6e6f 7420 656e 6f75 6768 2070 6f69 6e74  not enough point
-00013a60: 7320 746f 2065 7374 696d 6174 6520 6476  s to estimate dv
-00013a70: 2f76 2066 6f72 2064 7477 2229 0a20 2020  /v for dtw").   
-00013a80: 2020 2020 206d 3020 3d20 300a 2020 2020       m0 = 0.    
-00013a90: 2020 2020 656d 3020 3d20 300a 0a20 2020      em0 = 0..   
-00013aa0: 2072 6574 7572 6e20 6d30 202a 2031 3030   return m0 * 100
-00013ab0: 2c20 656d 3020 2a20 3130 302c 2064 6973  , em0 * 100, dis
-00013ac0: 740a 0a0a 6465 6620 6d77 6373 5f64 7676  t...def mwcs_dvv
-00013ad0: 2872 6566 2c20 6375 722c 206d 6f76 696e  (ref, cur, movin
-00013ae0: 675f 7769 6e64 6f77 5f6c 656e 6774 682c  g_window_length,
-00013af0: 2073 6c69 6465 5f73 7465 702c 2070 6172   slide_step, par
-00013b00: 612c 2073 6d6f 6f74 6869 6e67 5f68 616c  a, smoothing_hal
-00013b10: 665f 7769 6e3d 3529 3a0a 2020 2020 2222  f_win=5):.    ""
-00013b20: 220a 2020 2020 4d6f 7669 6e67 2057 696e  ".    Moving Win
-00013b30: 646f 7720 4372 6f73 7320 5370 6563 7472  dow Cross Spectr
-00013b40: 756d 206d 6574 686f 6420 746f 206d 6561  um method to mea
-00013b50: 7375 7265 2064 762f 7620 2872 656c 7969  sure dv/v (relyi
-00013b60: 6e67 206f 6e20 7068 693d 322a 7069 2a66  ng on phi=2*pi*f
-00013b70: 2a74 2069 6e20 6672 6571 2064 6f6d 6169  *t in freq domai
-00013b80: 6e29 0a0a 2020 2020 5041 5241 4d45 5445  n)..    PARAMETE
-00013b90: 5253 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  RS:.    --------
-00013ba0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2072 6566  --------.    ref
-00013bb0: 3a20 5265 6665 7265 6e63 6520 7761 7665  : Reference wave
-00013bc0: 666f 726d 2028 6e70 2e6e 6461 7272 6179  form (np.ndarray
-00013bd0: 2c20 7369 7a65 204e 290a 2020 2020 6375  , size N).    cu
-00013be0: 723a 2043 7572 7265 6e74 2077 6176 6566  r: Current wavef
-00013bf0: 6f72 6d20 286e 702e 6e64 6172 7261 792c  orm (np.ndarray,
-00013c00: 2073 697a 6520 4e29 0a20 2020 206d 6f76   size N).    mov
-00013c10: 696e 675f 7769 6e64 6f77 5f6c 656e 6774  ing_window_lengt
-00013c20: 683a 206d 6f76 696e 6720 7769 6e64 6f77  h: moving window
-00013c30: 206c 656e 6774 6820 746f 2063 616c 6375   length to calcu
-00013c40: 6c61 7465 2063 726f 7373 2d73 7065 6374  late cross-spect
-00013c50: 7275 6d20 286e 702e 666c 6f61 742c 2069  rum (np.float, i
-00013c60: 6e20 7365 6329 0a20 2020 2073 6c69 6465  n sec).    slide
-00013c70: 5f73 7465 703a 2073 7465 7073 2069 6e20  _step: steps in 
-00013c80: 7469 6d65 2074 6f20 7368 6966 7420 7468  time to shift th
-00013c90: 6520 6d6f 7669 6e67 2077 696e 646f 7720  e moving window 
-00013ca0: 286e 702e 666c 6f61 742c 2069 6e20 7365  (np.float, in se
-00013cb0: 636f 6e64 7329 0a20 2020 2070 6172 613a  conds).    para:
-00013cc0: 2061 2064 6963 7420 636f 6e74 6169 6e69   a dict containi
-00013cd0: 6e67 2070 6172 616d 6574 6572 7320 6162  ng parameters ab
-00013ce0: 6f75 7420 696e 7075 7420 6461 7461 2077  out input data w
-00013cf0: 696e 646f 7720 616e 6420 6672 6571 7565  indow and freque
-00013d00: 6e63 7920 696e 666f 2c20 696e 636c 7564  ncy info, includ
-00013d10: 696e 670a 2020 2020 2020 2020 6465 6c74  ing.        delt
-00013d20: 612d 3e54 6865 2073 616d 706c 696e 6720  a->The sampling 
-00013d30: 7261 7465 206f 6620 7468 6520 696e 7075  rate of the inpu
-00013d40: 7420 7469 6d65 7365 7269 6573 2028 696e  t timeseries (in
-00013d50: 2048 7a29 0a20 2020 2020 2020 2077 696e   Hz).        win
-00013d60: 646f 772d 3e20 5468 6520 7461 7267 6574  dow-> The target
-00013d70: 2077 696e 646f 7720 666f 7220 6d65 6173   window for meas
-00013d80: 7572 696e 6720 6474 2f74 0a20 2020 2020  uring dt/t.     
-00013d90: 2020 2066 7265 712d 3e20 5468 6520 6672     freq-> The fr
-00013da0: 6571 7565 6e63 7920 626f 756e 6420 746f  equency bound to
-00013db0: 2063 6f6d 7075 7465 2074 6865 2064 6570   compute the dep
-00013dc0: 6861 7369 6e67 2028 696e 2048 7a29 0a20  hasing (in Hz). 
-00013dd0: 2020 2020 2020 2074 6d69 6e3a 2054 6865         tmin: The
-00013de0: 206c 6566 746d 6f73 7420 7469 6d65 206c   leftmost time l
-00013df0: 6167 2028 7573 6564 2074 6f20 636f 6d70  ag (used to comp
-00013e00: 7574 6520 7468 6520 2274 696d 6520 6c61  ute the "time la
-00013e10: 6773 2061 7272 6179 2229 0a20 2020 2073  gs array").    s
-00013e20: 6d6f 6f74 6869 6e67 5f68 616c 665f 7769  moothing_half_wi
-00013e30: 6e3a 2049 6620 6469 6666 6572 656e 7420  n: If different 
-00013e40: 6672 6f6d 2030 2c20 6465 6669 6e65 7320  from 0, defines 
-00013e50: 7468 6520 6861 6c66 206c 656e 6774 6820  the half length 
-00013e60: 6f66 2074 6865 2073 6d6f 6f74 6869 6e67  of the smoothing
-00013e70: 2068 616e 6e69 6e67 2077 696e 646f 772e   hanning window.
-00013e80: 0a0a 2020 2020 5245 5455 524e 533a 0a20  ..    RETURNS:. 
-00013e90: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-00013ea0: 2d2d 2d2d 2d0a 2020 2020 7469 6d65 5f61  -----.    time_a
-00013eb0: 7869 733a 2074 6865 2063 656e 7472 616c  xis: the central
-00013ec0: 2074 696d 6573 206f 6620 7468 6520 7769   times of the wi
-00013ed0: 6e64 6f77 732e 0a20 2020 2064 656c 7461  ndows..    delta
-00013ee0: 5f74 3a20 6474 0a20 2020 2064 656c 7461  _t: dt.    delta
-00013ef0: 5f65 7272 3a65 7272 6f72 0a20 2020 2064  _err:error.    d
-00013f00: 656c 7461 5f6d 636f 683a 206d 6561 6e20  elta_mcoh: mean 
-00013f10: 636f 6865 7265 6e63 650a 0a20 2020 2043  coherence..    C
-00013f20: 6f70 6965 6420 6672 6f6d 204d 534e 6f69  opied from MSNoi
-00013f30: 7365 2028 6874 7470 733a 2f2f 6769 7468  se (https://gith
-00013f40: 7562 2e63 6f6d 2f52 4f42 656c 6769 756d  ub.com/ROBelgium
-00013f50: 2f4d 534e 6f69 7365 2f74 7265 652f 6d61  /MSNoise/tree/ma
-00013f60: 7374 6572 2f6d 736e 6f69 7365 290a 2020  ster/msnoise).  
-00013f70: 2020 4d6f 6469 6669 6564 2062 7920 4368    Modified by Ch
-00013f80: 656e 6778 696e 204a 6961 6e67 0a20 2020  engxin Jiang.   
-00013f90: 2022 2222 0a20 2020 2023 2063 6f6d 6d6f   """.    # commo
-00013fa0: 6e20 7661 7269 6162 6c65 730a 2020 2020  n variables.    
-00013fb0: 7477 696e 203d 2070 6172 615b 2274 7769  twin = para["twi
-00013fc0: 6e22 5d0a 2020 2020 6672 6571 203d 2070  n"].    freq = p
-00013fd0: 6172 615b 2266 7265 7122 5d0a 2020 2020  ara["freq"].    
-00013fe0: 6474 203d 2070 6172 615b 2264 7422 5d0a  dt = para["dt"].
-00013ff0: 2020 2020 746d 696e 203d 206e 702e 6d69      tmin = np.mi
-00014000: 6e28 7477 696e 290a 2020 2020 666d 696e  n(twin).    fmin
-00014010: 203d 206e 702e 6d69 6e28 6672 6571 290a   = np.min(freq).
-00014020: 2020 2020 666d 6178 203d 206e 702e 6d61      fmax = np.ma
-00014030: 7828 6672 6571 290a 0a20 2020 2023 2070  x(freq)..    # p
-00014040: 6172 616d 6574 6572 2069 6e69 7469 616c  arameter initial
-00014050: 697a 650a 2020 2020 6465 6c74 615f 7420  ize.    delta_t 
-00014060: 3d20 5b5d 0a20 2020 2064 656c 7461 5f65  = [].    delta_e
-00014070: 7272 203d 205b 5d0a 2020 2020 6465 6c74  rr = [].    delt
-00014080: 615f 6d63 6f68 203d 205b 5d0a 2020 2020  a_mcoh = [].    
-00014090: 7469 6d65 5f61 7869 7320 3d20 5b5d 0a0a  time_axis = []..
-000140a0: 2020 2020 2320 696e 666f 206f 6e20 7468      # info on th
-000140b0: 6520 6d6f 7669 6e67 2077 696e 646f 770a  e moving window.
-000140c0: 2020 2020 7769 6e64 6f77 5f6c 656e 6774      window_lengt
-000140d0: 685f 7361 6d70 6c65 7320 3d20 6e70 2e69  h_samples = np.i
-000140e0: 6e74 286d 6f76 696e 675f 7769 6e64 6f77  nt(moving_window
-000140f0: 5f6c 656e 6774 6820 2f20 6474 290a 2020  _length / dt).  
-00014100: 2020 7061 6464 203d 2069 6e74 2832 202a    padd = int(2 *
-00014110: 2a20 286e 6578 7470 6f77 3228 7769 6e64  * (nextpow2(wind
-00014120: 6f77 5f6c 656e 6774 685f 7361 6d70 6c65  ow_length_sample
-00014130: 7329 202b 2032 2929 0a20 2020 2063 6f75  s) + 2)).    cou
-00014140: 6e74 203d 2030 0a20 2020 2074 7020 3d20  nt = 0.    tp = 
-00014150: 636f 7369 6e65 5f74 6170 6572 2877 696e  cosine_taper(win
-00014160: 646f 775f 6c65 6e67 7468 5f73 616d 706c  dow_length_sampl
-00014170: 6573 2c20 302e 3135 290a 0a20 2020 206d  es, 0.15)..    m
-00014180: 696e 696e 6420 3d20 300a 2020 2020 6d61  inind = 0.    ma
-00014190: 7869 6e64 203d 2077 696e 646f 775f 6c65  xind = window_le
-000141a0: 6e67 7468 5f73 616d 706c 6573 0a0a 2020  ngth_samples..  
-000141b0: 2020 2320 6c6f 6f70 2074 6872 6f75 6768    # loop through
-000141c0: 2061 6c6c 2073 7562 2d77 696e 646f 7773   all sub-windows
-000141d0: 0a20 2020 2077 6869 6c65 206d 6178 696e  .    while maxin
-000141e0: 6420 3c3d 206c 656e 2872 6566 293a 0a20  d <= len(ref):. 
-000141f0: 2020 2020 2020 2063 6369 203d 2063 7572         cci = cur
-00014200: 5b6d 696e 696e 643a 6d61 7869 6e64 5d0a  [minind:maxind].
-00014210: 2020 2020 2020 2020 6363 6920 3d20 7363          cci = sc
-00014220: 6970 792e 7369 676e 616c 2e64 6574 7265  ipy.signal.detre
-00014230: 6e64 2863 6369 2c20 7479 7065 3d22 6c69  nd(cci, type="li
-00014240: 6e65 6172 2229 0a20 2020 2020 2020 2063  near").        c
-00014250: 6369 202a 3d20 7470 0a0a 2020 2020 2020  ci *= tp..      
-00014260: 2020 6372 6920 3d20 7265 665b 6d69 6e69    cri = ref[mini
-00014270: 6e64 3a6d 6178 696e 645d 0a20 2020 2020  nd:maxind].     
-00014280: 2020 2063 7269 203d 2073 6369 7079 2e73     cri = scipy.s
-00014290: 6967 6e61 6c2e 6465 7472 656e 6428 6372  ignal.detrend(cr
-000142a0: 692c 2074 7970 653d 226c 696e 6561 7222  i, type="linear"
-000142b0: 290a 2020 2020 2020 2020 6372 6920 2a3d  ).        cri *=
-000142c0: 2074 700a 0a20 2020 2020 2020 206d 696e   tp..        min
-000142d0: 696e 6420 2b3d 2069 6e74 2873 6c69 6465  ind += int(slide
-000142e0: 5f73 7465 7020 2f20 6474 290a 2020 2020  _step / dt).    
-000142f0: 2020 2020 6d61 7869 6e64 202b 3d20 696e      maxind += in
-00014300: 7428 736c 6964 655f 7374 6570 202f 2064  t(slide_step / d
-00014310: 7429 0a0a 2020 2020 2020 2020 2320 646f  t)..        # do
-00014320: 2066 6674 0a20 2020 2020 2020 2066 6375   fft.        fcu
-00014330: 7220 3d20 7363 6970 792e 6666 7470 6163  r = scipy.fftpac
-00014340: 6b2e 6666 7428 6363 692c 206e 3d70 6164  k.fft(cci, n=pad
-00014350: 6429 5b3a 2070 6164 6420 2f2f 2032 5d0a  d)[: padd // 2].
-00014360: 2020 2020 2020 2020 6672 6566 203d 2073          fref = s
-00014370: 6369 7079 2e66 6674 7061 636b 2e66 6674  cipy.fftpack.fft
-00014380: 2863 7269 2c20 6e3d 7061 6464 295b 3a20  (cri, n=padd)[: 
-00014390: 7061 6464 202f 2f20 325d 0a0a 2020 2020  padd // 2]..    
-000143a0: 2020 2020 6663 7572 3220 3d20 6e70 2e72      fcur2 = np.r
-000143b0: 6561 6c28 6663 7572 2920 2a2a 2032 202b  eal(fcur) ** 2 +
-000143c0: 206e 702e 696d 6167 2866 6375 7229 202a   np.imag(fcur) *
-000143d0: 2a20 320a 2020 2020 2020 2020 6672 6566  * 2.        fref
-000143e0: 3220 3d20 6e70 2e72 6561 6c28 6672 6566  2 = np.real(fref
-000143f0: 2920 2a2a 2032 202b 206e 702e 696d 6167  ) ** 2 + np.imag
-00014400: 2866 7265 6629 202a 2a20 320a 0a20 2020  (fref) ** 2..   
-00014410: 2020 2020 2023 2067 6574 2063 726f 7373       # get cross
-00014420: 2d73 7065 6374 7275 6d20 2620 646f 2066  -spectrum & do f
-00014430: 696c 7465 7269 6e67 0a20 2020 2020 2020  iltering.       
-00014440: 2058 203d 2066 7265 6620 2a20 2866 6375   X = fref * (fcu
-00014450: 722e 636f 6e6a 2829 290a 2020 2020 2020  r.conj()).      
-00014460: 2020 6966 2073 6d6f 6f74 6869 6e67 5f68    if smoothing_h
-00014470: 616c 665f 7769 6e20 213d 2030 3a0a 2020  alf_win != 0:.  
-00014480: 2020 2020 2020 2020 2020 6463 7572 203d            dcur =
-00014490: 206e 702e 7371 7274 2873 6d6f 6f74 6828   np.sqrt(smooth(
-000144a0: 6663 7572 322c 2077 696e 646f 773d 2268  fcur2, window="h
-000144b0: 616e 6e69 6e67 222c 2068 616c 665f 7769  anning", half_wi
-000144c0: 6e3d 736d 6f6f 7468 696e 675f 6861 6c66  n=smoothing_half
-000144d0: 5f77 696e 2929 0a20 2020 2020 2020 2020  _win)).         
-000144e0: 2020 2064 7265 6620 3d20 6e70 2e73 7172     dref = np.sqr
-000144f0: 7428 736d 6f6f 7468 2866 7265 6632 2c20  t(smooth(fref2, 
-00014500: 7769 6e64 6f77 3d22 6861 6e6e 696e 6722  window="hanning"
-00014510: 2c20 6861 6c66 5f77 696e 3d73 6d6f 6f74  , half_win=smoot
-00014520: 6869 6e67 5f68 616c 665f 7769 6e29 290a  hing_half_win)).
-00014530: 2020 2020 2020 2020 2020 2020 5820 3d20              X = 
-00014540: 736d 6f6f 7468 2858 2c20 7769 6e64 6f77  smooth(X, window
-00014550: 3d22 6861 6e6e 696e 6722 2c20 6861 6c66  ="hanning", half
-00014560: 5f77 696e 3d73 6d6f 6f74 6869 6e67 5f68  _win=smoothing_h
-00014570: 616c 665f 7769 6e29 0a20 2020 2020 2020  alf_win).       
-00014580: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00014590: 2020 2064 6375 7220 3d20 6e70 2e73 7172     dcur = np.sqr
-000145a0: 7428 6663 7572 3229 0a20 2020 2020 2020  t(fcur2).       
-000145b0: 2020 2020 2064 7265 6620 3d20 6e70 2e73       dref = np.s
-000145c0: 7172 7428 6672 6566 3229 0a0a 2020 2020  qrt(fref2)..    
-000145d0: 2020 2020 6463 7320 3d20 6e70 2e61 6273      dcs = np.abs
-000145e0: 2858 290a 0a20 2020 2020 2020 2023 2046  (X)..        # F
-000145f0: 696e 6420 7468 6520 7661 6c75 6573 2074  ind the values t
-00014600: 6865 2066 7265 7175 656e 6379 2072 616e  he frequency ran
-00014610: 6765 206f 6620 696e 7465 7265 7374 0a20  ge of interest. 
-00014620: 2020 2020 2020 2066 7265 715f 7665 6320         freq_vec 
-00014630: 3d20 7363 6970 792e 6666 7470 6163 6b2e  = scipy.fftpack.
-00014640: 6666 7466 7265 7128 6c65 6e28 5829 202a  fftfreq(len(X) *
-00014650: 2032 2c20 6474 295b 3a20 7061 6464 202f   2, dt)[: padd /
-00014660: 2f20 325d 0a20 2020 2020 2020 2069 6e64  / 2].        ind
-00014670: 6578 5f72 616e 6765 203d 206e 702e 6172  ex_range = np.ar
-00014680: 6777 6865 7265 286e 702e 6c6f 6769 6361  gwhere(np.logica
-00014690: 6c5f 616e 6428 6672 6571 5f76 6563 203e  l_and(freq_vec >
-000146a0: 3d20 666d 696e 2c20 6672 6571 5f76 6563  = fmin, freq_vec
-000146b0: 203c 3d20 666d 6178 2929 0a0a 2020 2020   <= fmax))..    
-000146c0: 2020 2020 2320 4765 7420 436f 6865 7265      # Get Cohere
-000146d0: 6e63 6520 616e 6420 6974 7320 6d65 616e  nce and its mean
-000146e0: 2076 616c 7565 0a20 2020 2020 2020 2063   value.        c
-000146f0: 6f68 203d 2067 6574 436f 6865 7265 6e63  oh = getCoherenc
-00014700: 6528 6463 732c 2064 7265 662c 2064 6375  e(dcs, dref, dcu
-00014710: 7229 0a20 2020 2020 2020 206d 636f 6820  r).        mcoh 
-00014720: 3d20 6e70 2e6d 6561 6e28 636f 685b 696e  = np.mean(coh[in
-00014730: 6465 785f 7261 6e67 655d 290a 0a20 2020  dex_range])..   
-00014740: 2020 2020 2023 2047 6574 2057 6569 6768       # Get Weigh
-00014750: 7473 0a20 2020 2020 2020 2077 203d 2031  ts.        w = 1
-00014760: 2e30 202f 2028 312e 3020 2f20 2863 6f68  .0 / (1.0 / (coh
-00014770: 5b69 6e64 6578 5f72 616e 6765 5d20 2a2a  [index_range] **
-00014780: 2032 2920 2d20 312e 3029 0a20 2020 2020   2) - 1.0).     
-00014790: 2020 2077 5b63 6f68 5b69 6e64 6578 5f72     w[coh[index_r
-000147a0: 616e 6765 5d20 3e3d 2030 2e39 395d 203d  ange] >= 0.99] =
-000147b0: 2031 2e30 202f 2028 312e 3020 2f20 302e   1.0 / (1.0 / 0.
-000147c0: 3938 3031 202d 2031 2e30 290a 2020 2020  9801 - 1.0).    
-000147d0: 2020 2020 7720 3d20 6e70 2e73 7172 7428      w = np.sqrt(
-000147e0: 7720 2a20 6e70 2e73 7172 7428 6463 735b  w * np.sqrt(dcs[
-000147f0: 696e 6465 785f 7261 6e67 655d 2929 0a20  index_range])). 
-00014800: 2020 2020 2020 2077 203d 206e 702e 7265         w = np.re
-00014810: 616c 2877 290a 0a20 2020 2020 2020 2023  al(w)..        #
-00014820: 2046 7265 7175 656e 6379 2061 7272 6179   Frequency array
-00014830: 3a0a 2020 2020 2020 2020 7620 3d20 6e70  :.        v = np
-00014840: 2e72 6561 6c28 6672 6571 5f76 6563 5b69  .real(freq_vec[i
-00014850: 6e64 6578 5f72 616e 6765 5d29 202a 2032  ndex_range]) * 2
-00014860: 202a 206e 702e 7069 0a0a 2020 2020 2020   * np.pi..      
-00014870: 2020 2320 5068 6173 653a 0a20 2020 2020    # Phase:.     
-00014880: 2020 2070 6869 203d 206e 702e 616e 676c     phi = np.angl
-00014890: 6528 5829 0a20 2020 2020 2020 2070 6869  e(X).        phi
-000148a0: 5b30 5d20 3d20 302e 300a 2020 2020 2020  [0] = 0.0.      
-000148b0: 2020 7068 6920 3d20 6e70 2e75 6e77 7261    phi = np.unwra
-000148c0: 7028 7068 6929 0a20 2020 2020 2020 2070  p(phi).        p
-000148d0: 6869 203d 2070 6869 5b69 6e64 6578 5f72  hi = phi[index_r
-000148e0: 616e 6765 5d0a 0a20 2020 2020 2020 2023  ange]..        #
-000148f0: 2043 616c 6375 6c61 7465 2074 6865 2073   Calculate the s
-00014900: 6c6f 7065 2077 6974 6820 6120 7765 6967  lope with a weig
-00014910: 6874 6564 206c 6561 7374 2073 7175 6172  hted least squar
-00014920: 6520 6c69 6e65 6172 2072 6567 7265 7373  e linear regress
-00014930: 696f 6e0a 2020 2020 2020 2020 2320 666f  ion.        # fo
-00014940: 7263 6564 2074 6872 6f75 6768 2074 6865  rced through the
-00014950: 206f 7269 6769 6e3b 2077 6569 6768 7473   origin; weights
-00014960: 2066 6f72 2074 6865 2057 4c53 206d 7573   for the WLS mus
-00014970: 7420 6265 2074 6865 2076 6172 6961 6e63  t be the varianc
-00014980: 6520 210a 2020 2020 2020 2020 6d2c 2065  e !.        m, e
-00014990: 6d20 3d20 6c69 6e65 6172 5f72 6567 7265  m = linear_regre
-000149a0: 7373 696f 6e28 762e 666c 6174 7465 6e28  ssion(v.flatten(
-000149b0: 292c 2070 6869 2e66 6c61 7474 656e 2829  ), phi.flatten()
-000149c0: 2c20 772e 666c 6174 7465 6e28 2929 0a20  , w.flatten()). 
-000149d0: 2020 2020 2020 2064 656c 7461 5f74 2e61         delta_t.a
-000149e0: 7070 656e 6428 6d29 0a0a 2020 2020 2020  ppend(m)..      
-000149f0: 2020 2320 7072 696e 7420 7068 692e 7368    # print phi.sh
-00014a00: 6170 652c 2076 2e73 6861 7065 2c20 772e  ape, v.shape, w.
-00014a10: 7368 6170 650a 2020 2020 2020 2020 6520  shape.        e 
-00014a20: 3d20 6e70 2e73 756d 2828 7068 6920 2d20  = np.sum((phi - 
-00014a30: 6d20 2a20 7629 202a 2a20 3229 202f 2028  m * v) ** 2) / (
-00014a40: 6e70 2e73 697a 6528 7629 202d 2031 290a  np.size(v) - 1).
-00014a50: 2020 2020 2020 2020 7332 7832 203d 206e          s2x2 = n
-00014a60: 702e 7375 6d28 762a 2a32 202a 2077 2a2a  p.sum(v**2 * w**
-00014a70: 3229 0a20 2020 2020 2020 2073 7832 203d  2).        sx2 =
-00014a80: 206e 702e 7375 6d28 7720 2a20 762a 2a32   np.sum(w * v**2
-00014a90: 290a 2020 2020 2020 2020 6520 3d20 6e70  ).        e = np
-00014aa0: 2e73 7172 7428 6520 2a20 7332 7832 202f  .sqrt(e * s2x2 /
-00014ab0: 2073 7832 2a2a 3229 0a0a 2020 2020 2020   sx2**2)..      
-00014ac0: 2020 6465 6c74 615f 6572 722e 6170 7065    delta_err.appe
-00014ad0: 6e64 2865 290a 2020 2020 2020 2020 6465  nd(e).        de
-00014ae0: 6c74 615f 6d63 6f68 2e61 7070 656e 6428  lta_mcoh.append(
-00014af0: 6e70 2e72 6561 6c28 6d63 6f68 2929 0a20  np.real(mcoh)). 
-00014b00: 2020 2020 2020 2074 696d 655f 6178 6973         time_axis
-00014b10: 2e61 7070 656e 6428 746d 696e 202b 206d  .append(tmin + m
-00014b20: 6f76 696e 675f 7769 6e64 6f77 5f6c 656e  oving_window_len
-00014b30: 6774 6820 2f20 322e 3020 2b20 636f 756e  gth / 2.0 + coun
-00014b40: 7420 2a20 736c 6964 655f 7374 6570 290a  t * slide_step).
-00014b50: 2020 2020 2020 2020 636f 756e 7420 2b3d          count +=
-00014b60: 2031 0a0a 2020 2020 2020 2020 6465 6c20   1..        del 
-00014b70: 6663 7572 2c20 6672 6566 0a20 2020 2020  fcur, fref.     
-00014b80: 2020 2064 656c 2058 0a20 2020 2020 2020     del X.       
-00014b90: 2064 656c 2066 7265 715f 7665 630a 2020   del freq_vec.  
-00014ba0: 2020 2020 2020 6465 6c20 696e 6465 785f        del index_
-00014bb0: 7261 6e67 650a 2020 2020 2020 2020 6465  range.        de
-00014bc0: 6c20 772c 2076 2c20 652c 2073 3278 322c  l w, v, e, s2x2,
-00014bd0: 2073 7832 2c20 6d2c 2065 6d0a 0a20 2020   sx2, m, em..   
-00014be0: 2069 6620 6d61 7869 6e64 203e 206c 656e   if maxind > len
-00014bf0: 2863 7572 2920 2b20 696e 7428 736c 6964  (cur) + int(slid
-00014c00: 655f 7374 6570 202f 2064 7429 3a0a 2020  e_step / dt):.  
-00014c10: 2020 2020 2020 7072 696e 7428 2254 6865        print("The
-00014c20: 206c 6173 7420 7769 6e64 6f77 2077 6173   last window was
-00014c30: 2074 6f6f 2073 6d61 6c6c 2c20 6275 7420   too small, but 
-00014c40: 7761 7320 636f 6d70 7574 6564 2229 0a0a  was computed")..
-00014c50: 2020 2020 2320 656e 7375 7265 2061 6c6c      # ensure all
-00014c60: 206d 6174 7269 7820 6172 6520 6e70 2061   matrix are np a
-00014c70: 7272 6179 0a20 2020 2064 656c 7461 5f74  rray.    delta_t
-00014c80: 203d 206e 702e 6172 7261 7928 6465 6c74   = np.array(delt
-00014c90: 615f 7429 0a20 2020 2064 656c 7461 5f65  a_t).    delta_e
-00014ca0: 7272 203d 206e 702e 6172 7261 7928 6465  rr = np.array(de
-00014cb0: 6c74 615f 6572 7229 0a20 2020 2064 656c  lta_err).    del
-00014cc0: 7461 5f6d 636f 6820 3d20 6e70 2e61 7272  ta_mcoh = np.arr
-00014cd0: 6179 2864 656c 7461 5f6d 636f 6829 0a20  ay(delta_mcoh). 
-00014ce0: 2020 2074 696d 655f 6178 6973 203d 206e     time_axis = n
-00014cf0: 702e 6172 7261 7928 7469 6d65 5f61 7869  p.array(time_axi
-00014d00: 7329 0a0a 2020 2020 2320 7265 6164 7920  s)..    # ready 
-00014d10: 666f 7220 6c69 6e65 6172 2072 6567 7265  for linear regre
-00014d20: 7373 696f 6e0a 2020 2020 6465 6c74 615f  ssion.    delta_
-00014d30: 6d69 6e63 686f 203d 2030 2e36 350a 2020  mincho = 0.65.  
-00014d40: 2020 6465 6c74 615f 6d61 7865 7272 203d    delta_maxerr =
-00014d50: 2030 2e31 0a20 2020 2064 656c 7461 5f6d   0.1.    delta_m
-00014d60: 6178 6474 203d 2030 2e31 0a20 2020 2069  axdt = 0.1.    i
-00014d70: 6e64 7831 203d 206e 702e 7768 6572 6528  ndx1 = np.where(
-00014d80: 6465 6c74 615f 6d63 6f68 203e 2064 656c  delta_mcoh > del
-00014d90: 7461 5f6d 696e 6368 6f29 0a20 2020 2069  ta_mincho).    i
-00014da0: 6e64 7832 203d 206e 702e 7768 6572 6528  ndx2 = np.where(
-00014db0: 6465 6c74 615f 6572 7220 3c20 6465 6c74  delta_err < delt
-00014dc0: 615f 6d61 7865 7272 290a 2020 2020 696e  a_maxerr).    in
-00014dd0: 6478 3320 3d20 6e70 2e77 6865 7265 2864  dx3 = np.where(d
-00014de0: 656c 7461 5f74 203c 2064 656c 7461 5f6d  elta_t < delta_m
-00014df0: 6178 6474 290a 0a20 2020 2023 202d 2d2d  axdt)..    # ---
-00014e00: 2d2d 6669 6e64 2067 6f6f 6420 6474 206d  --find good dt m
-00014e10: 6561 7375 7265 6d65 6e74 732d 2d2d 2d2d  easurements-----
-00014e20: 0a20 2020 2069 6e64 7820 3d20 6e70 2e69  .    indx = np.i
-00014e30: 6e74 6572 7365 6374 3164 2869 6e64 7831  ntersect1d(indx1
-00014e40: 2c20 696e 6478 3229 0a20 2020 2069 6e64  , indx2).    ind
-00014e50: 7820 3d20 6e70 2e69 6e74 6572 7365 6374  x = np.intersect
-00014e60: 3164 2869 6e64 782c 2069 6e64 7833 290a  1d(indx, indx3).
-00014e70: 0a20 2020 2069 6620 6c65 6e28 696e 6478  .    if len(indx
-00014e80: 2920 3e20 323a 0a20 2020 2020 2020 2023  ) > 2:.        #
-00014e90: 202d 2d2d 2d65 7374 696d 6174 6520 7765   ----estimate we
-00014ea0: 6967 6874 2066 6f72 2072 6567 7265 7373  ight for regress
-00014eb0: 696f 6e2d 2d2d 2d0a 2020 2020 2020 2020  ion----.        
-00014ec0: 7720 3d20 3120 2f20 6465 6c74 615f 6572  w = 1 / delta_er
-00014ed0: 725b 696e 6478 5d0a 2020 2020 2020 2020  r[indx].        
-00014ee0: 775b 7e6e 702e 6973 6669 6e69 7465 2877  w[~np.isfinite(w
-00014ef0: 295d 203d 2031 2e30 0a0a 2020 2020 2020  )] = 1.0..      
-00014f00: 2020 2320 2d2d 2d2d 2d2d 2d2d 2d64 6f20    # ---------do 
-00014f10: 6c69 6e65 6172 2072 6567 7265 7373 696f  linear regressio
-00014f20: 6e2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  n-----------.   
-00014f30: 2020 2020 2023 206d 2c20 612c 2065 6d2c       # m, a, em,
-00014f40: 2065 6120 3d20 6c69 6e65 6172 5f72 6567   ea = linear_reg
-00014f50: 7265 7373 696f 6e28 7469 6d65 5f61 7869  ression(time_axi
-00014f60: 735b 696e 6478 5d2c 2064 656c 7461 5f74  s[indx], delta_t
-00014f70: 5b69 6e64 785d 2c20 772c 2069 6e74 6572  [indx], w, inter
-00014f80: 6365 7074 5f6f 7269 6769 6e3d 4661 6c73  cept_origin=Fals
-00014f90: 6529 0a20 2020 2020 2020 206d 302c 2065  e).        m0, e
-00014fa0: 6d30 203d 206c 696e 6561 725f 7265 6772  m0 = linear_regr
-00014fb0: 6573 7369 6f6e 2874 696d 655f 6178 6973  ession(time_axis
-00014fc0: 5b69 6e64 785d 2c20 6465 6c74 615f 745b  [indx], delta_t[
-00014fd0: 696e 6478 5d2c 2077 2c20 696e 7465 7263  indx], w, interc
-00014fe0: 6570 745f 6f72 6967 696e 3d54 7275 6529  ept_origin=True)
-00014ff0: 0a0a 2020 2020 656c 7365 3a0a 2020 2020  ..    else:.    
-00015000: 2020 2020 7072 696e 7428 226e 6f74 2065      print("not e
-00015010: 6e6f 7567 6820 706f 696e 7473 2074 6f20  nough points to 
-00015020: 6573 7469 6d61 7465 2064 762f 7620 666f  estimate dv/v fo
-00015030: 7220 6d77 6373 2229 0a20 2020 2020 2020  r mwcs").       
-00015040: 206d 3020 3d20 300a 2020 2020 2020 2020   m0 = 0.        
-00015050: 656d 3020 3d20 300a 0a20 2020 2072 6574  em0 = 0..    ret
-00015060: 7572 6e20 2d6d 3020 2a20 3130 302c 2065  urn -m0 * 100, e
-00015070: 6d30 202a 2031 3030 0a0a 0a64 6566 2057  m0 * 100...def W
-00015080: 4343 5f64 7676 2872 6566 2c20 6375 722c  CC_dvv(ref, cur,
-00015090: 206d 6f76 696e 675f 7769 6e64 6f77 5f6c   moving_window_l
-000150a0: 656e 6774 682c 2073 6c69 6465 5f73 7465  ength, slide_ste
-000150b0: 702c 2070 6172 6129 3a0a 2020 2020 2222  p, para):.    ""
-000150c0: 220a 2020 2020 5769 6e64 6f77 6564 2063  ".    Windowed c
-000150d0: 726f 7373 2063 6f72 7265 6c61 7469 6f6e  ross correlation
-000150e0: 2028 5743 4329 2066 6f72 2064 7420 6f72   (WCC) for dt or
-000150f0: 2064 762f 7620 6d65 7375 7265 6d65 6e74   dv/v mesurement
-00015100: 2028 536e 6965 6465 7220 6574 2061 6c2e   (Snieder et al.
-00015110: 2032 3031 3229 0a0a 2020 2020 5061 7261   2012)..    Para
-00015120: 6d65 7465 7273 3a0a 2020 2020 2d2d 2d2d  meters:.    ----
-00015130: 2d2d 2d2d 2d2d 2d0a 2020 2020 7265 663a  -------.    ref:
-00015140: 2054 6865 2022 5265 6665 7265 6e63 6522   The "Reference"
-00015150: 2074 696d 6573 6572 6965 730a 2020 2020   timeseries.    
-00015160: 6375 723a 2054 6865 2022 4375 7272 656e  cur: The "Curren
-00015170: 7422 2074 696d 6573 6572 6965 730a 2020  t" timeseries.  
-00015180: 2020 6d6f 7669 6e67 5f77 696e 646f 775f    moving_window_
-00015190: 6c65 6e67 7468 3a20 5468 6520 6d6f 7669  length: The movi
-000151a0: 6e67 2077 696e 646f 7720 6c65 6e67 7468  ng window length
-000151b0: 2028 696e 2073 6563 6f6e 6473 290a 2020   (in seconds).  
-000151c0: 2020 736c 6964 655f 7374 6570 3a20 5468    slide_step: Th
-000151d0: 6520 7374 6570 2074 6f20 6a75 6d70 2066  e step to jump f
-000151e0: 6f72 2074 6865 206d 6f76 696e 6720 7769  or the moving wi
-000151f0: 6e64 6f77 2028 696e 2073 6563 6f6e 6473  ndow (in seconds
-00015200: 290a 2020 2020 7061 7261 3a20 6120 6469  ).    para: a di
-00015210: 6374 2063 6f6e 7461 696e 696e 6720 6672  ct containing fr
-00015220: 6571 2f74 696d 6520 696e 666f 206f 6620  eq/time info of 
-00015230: 7468 6520 6461 7461 206d 6174 7269 780a  the data matrix.
-00015240: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-00015250: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20    ------------. 
-00015260: 2020 2074 696d 655f 6178 6973 3a20 6365     time_axis: ce
-00015270: 6e74 7261 6c20 7469 6d65 7320 6f66 2074  ntral times of t
-00015280: 6865 206d 6f76 696e 6720 7769 6e64 6f77  he moving window
-00015290: 0a20 2020 2064 656c 7461 5f74 3a20 6474  .    delta_t: dt
-000152a0: 0a20 2020 2064 656c 7461 5f65 7272 3a20  .    delta_err: 
-000152b0: 6572 726f 720a 2020 2020 6465 6c74 615f  error.    delta_
-000152c0: 6d63 6f68 3a20 6d65 616e 2063 6f68 6572  mcoh: mean coher
-000152d0: 656e 6365 2066 6f72 2065 6163 6820 7769  ence for each wi
-000152e0: 6e64 6f77 0a0a 2020 2020 5772 6974 7465  ndow..    Writte
-000152f0: 6e20 6279 2043 6f6e 6763 6f6e 6720 5975  n by Congcong Yu
-00015300: 616e 2028 3120 4a75 6c79 2c20 3230 3139  an (1 July, 2019
-00015310: 290a 2020 2020 2222 220a 2020 2020 2320  ).    """.    # 
-00015320: 636f 6d6d 6f6e 2076 6172 6961 626c 6573  common variables
-00015330: 0a20 2020 2074 7769 6e20 3d20 7061 7261  .    twin = para
-00015340: 5b22 7477 696e 225d 0a20 2020 2064 7420  ["twin"].    dt 
-00015350: 3d20 7061 7261 5b22 6474 225d 0a20 2020  = para["dt"].   
-00015360: 2074 6d69 6e20 3d20 6e70 2e6d 696e 2874   tmin = np.min(t
-00015370: 7769 6e29 0a0a 2020 2020 2320 7061 7261  win)..    # para
-00015380: 6d65 7465 7220 696e 6974 6961 6c69 7a65  meter initialize
-00015390: 0a20 2020 2064 656c 7461 5f74 203d 205b  .    delta_t = [
-000153a0: 5d0a 2020 2020 6465 6c74 615f 745f 636f  ].    delta_t_co
-000153b0: 6566 203d 205b 5d0a 2020 2020 7469 6d65  ef = [].    time
-000153c0: 5f61 7869 7320 3d20 5b5d 0a0a 2020 2020  _axis = []..    
-000153d0: 2320 696e 666f 206f 6e20 7468 6520 6d6f  # info on the mo
-000153e0: 7669 6e67 2077 696e 646f 770a 2020 2020  ving window.    
-000153f0: 7769 6e64 6f77 5f6c 656e 6774 685f 7361  window_length_sa
-00015400: 6d70 6c65 7320 3d20 6e70 2e69 6e74 286d  mples = np.int(m
-00015410: 6f76 696e 675f 7769 6e64 6f77 5f6c 656e  oving_window_len
-00015420: 6774 6820 2f20 6474 290a 2020 2020 636f  gth / dt).    co
-00015430: 756e 7420 3d20 300a 2020 2020 7470 203d  unt = 0.    tp =
-00015440: 2063 6f73 696e 655f 7461 7065 7228 7769   cosine_taper(wi
-00015450: 6e64 6f77 5f6c 656e 6774 685f 7361 6d70  ndow_length_samp
-00015460: 6c65 732c 2030 2e31 3529 0a0a 2020 2020  les, 0.15)..    
-00015470: 6d69 6e69 6e64 203d 2030 0a20 2020 206d  minind = 0.    m
-00015480: 6178 696e 6420 3d20 7769 6e64 6f77 5f6c  axind = window_l
-00015490: 656e 6774 685f 7361 6d70 6c65 730a 0a20  ength_samples.. 
-000154a0: 2020 2023 206c 6f6f 7020 7468 726f 7567     # loop throug
-000154b0: 6820 616c 6c20 7375 622d 7769 6e64 6f77  h all sub-window
-000154c0: 730a 2020 2020 7768 696c 6520 6d61 7869  s.    while maxi
-000154d0: 6e64 203c 3d20 6c65 6e28 7265 6629 3a0a  nd <= len(ref):.
-000154e0: 2020 2020 2020 2020 6363 6920 3d20 6375          cci = cu
-000154f0: 725b 6d69 6e69 6e64 3a6d 6178 696e 645d  r[minind:maxind]
-00015500: 0a20 2020 2020 2020 2063 6369 203d 2073  .        cci = s
-00015510: 6369 7079 2e73 6967 6e61 6c2e 6465 7472  cipy.signal.detr
-00015520: 656e 6428 6363 692c 2074 7970 653d 226c  end(cci, type="l
-00015530: 696e 6561 7222 290a 2020 2020 2020 2020  inear").        
-00015540: 6363 6920 2a3d 2074 700a 0a20 2020 2020  cci *= tp..     
-00015550: 2020 2063 7269 203d 2072 6566 5b6d 696e     cri = ref[min
-00015560: 696e 643a 6d61 7869 6e64 5d0a 2020 2020  ind:maxind].    
-00015570: 2020 2020 6372 6920 3d20 7363 6970 792e      cri = scipy.
-00015580: 7369 676e 616c 2e64 6574 7265 6e64 2863  signal.detrend(c
-00015590: 7269 2c20 7479 7065 3d22 6c69 6e65 6172  ri, type="linear
-000155a0: 2229 0a20 2020 2020 2020 2063 7269 202a  ").        cri *
-000155b0: 3d20 7470 0a0a 2020 2020 2020 2020 6d69  = tp..        mi
-000155c0: 6e69 6e64 202b 3d20 696e 7428 736c 6964  nind += int(slid
-000155d0: 655f 7374 6570 202f 2064 7429 0a20 2020  e_step / dt).   
-000155e0: 2020 2020 206d 6178 696e 6420 2b3d 2069       maxind += i
-000155f0: 6e74 2873 6c69 6465 5f73 7465 7020 2f20  nt(slide_step / 
-00015600: 6474 290a 0a20 2020 2020 2020 2023 206e  dt)..        # n
-00015610: 6f72 6d61 6c69 7a65 2073 6967 6e61 6c73  ormalize signals
-00015620: 2062 6566 6f72 6520 6372 6f73 7320 636f   before cross co
-00015630: 7272 656c 6174 696f 6e0a 2020 2020 2020  rrelation.      
-00015640: 2020 6363 6920 3d20 2863 6369 202d 2063    cci = (cci - c
-00015650: 6369 2e6d 6561 6e28 2929 202f 2063 6369  ci.mean()) / cci
-00015660: 2e73 7464 2829 0a20 2020 2020 2020 2063  .std().        c
-00015670: 7269 203d 2028 6372 6920 2d20 6372 692e  ri = (cri - cri.
-00015680: 6d65 616e 2829 2920 2f20 6372 692e 7374  mean()) / cri.st
-00015690: 6428 290a 0a20 2020 2020 2020 2023 2067  d()..        # g
-000156a0: 6574 206d 6178 696d 756d 2063 6f72 7265  et maximum corre
-000156b0: 6c61 7469 6f6e 2063 6f65 6666 6963 6965  lation coefficie
-000156c0: 6e74 2061 6e64 2069 7473 2069 6e64 6578  nt and its index
-000156d0: 0a20 2020 2020 2020 2063 6332 203d 206e  .        cc2 = n
-000156e0: 702e 636f 7272 656c 6174 6528 6363 692c  p.correlate(cci,
-000156f0: 2063 7269 2c20 6d6f 6465 3d22 7361 6d65   cri, mode="same
-00015700: 2229 0a20 2020 2020 2020 2063 6332 203d  ").        cc2 =
-00015710: 2063 6332 202f 206e 702e 7371 7274 2828   cc2 / np.sqrt((
-00015720: 6363 692a 2a32 292e 7375 6d28 2920 2a20  cci**2).sum() * 
-00015730: 2863 7269 2a2a 3229 2e73 756d 2829 290a  (cri**2).sum()).
-00015740: 0a20 2020 2020 2020 2069 6d61 7863 6332  .        imaxcc2
-00015750: 203d 206e 702e 7768 6572 6528 6363 3220   = np.where(cc2 
-00015760: 3d3d 206e 702e 6d61 7828 6363 3229 295b  == np.max(cc2))[
-00015770: 305d 0a20 2020 2020 2020 206d 6178 6363  0].        maxcc
-00015780: 3220 3d20 6e70 2e6d 6178 2863 6332 290a  2 = np.max(cc2).
-00015790: 0a20 2020 2020 2020 2023 2067 6574 2074  .        # get t
-000157a0: 6865 2074 696d 6520 7368 6966 740a 2020  he time shift.  
-000157b0: 2020 2020 2020 6d20 3d20 2869 6d61 7863        m = (imaxc
-000157c0: 6332 202d 2028 286d 6178 696e 6420 2d20  c2 - ((maxind - 
-000157d0: 6d69 6e69 6e64 2920 2f2f 2032 2929 202a  minind) // 2)) *
-000157e0: 2064 740a 2020 2020 2020 2020 6465 6c74   dt.        delt
-000157f0: 615f 742e 6170 7065 6e64 286d 290a 2020  a_t.append(m).  
-00015800: 2020 2020 2020 6465 6c74 615f 745f 636f        delta_t_co
-00015810: 6566 2e61 7070 656e 6428 6d61 7863 6332  ef.append(maxcc2
-00015820: 290a 0a20 2020 2020 2020 2074 696d 655f  )..        time_
-00015830: 6178 6973 2e61 7070 656e 6428 746d 696e  axis.append(tmin
-00015840: 202b 206d 6f76 696e 675f 7769 6e64 6f77   + moving_window
-00015850: 5f6c 656e 6774 6820 2f20 322e 3020 2b20  _length / 2.0 + 
-00015860: 636f 756e 7420 2a20 736c 6964 655f 7374  count * slide_st
-00015870: 6570 290a 2020 2020 2020 2020 636f 756e  ep).        coun
-00015880: 7420 2b3d 2031 0a0a 2020 2020 6465 6c20  t += 1..    del 
-00015890: 6363 692c 2063 7269 2c20 6363 322c 2069  cci, cri, cc2, i
-000158a0: 6d61 7863 6332 2c20 6d61 7863 6332 0a20  maxcc2, maxcc2. 
-000158b0: 2020 2064 656c 206d 0a0a 2020 2020 6966     del m..    if
-000158c0: 206d 6178 696e 6420 3e20 6c65 6e28 6375   maxind > len(cu
-000158d0: 7229 202b 2069 6e74 2873 6c69 6465 5f73  r) + int(slide_s
-000158e0: 7465 7020 2f20 6474 293a 0a20 2020 2020  tep / dt):.     
-000158f0: 2020 2070 7269 6e74 2822 5468 6520 6c61     print("The la
-00015900: 7374 2077 696e 646f 7720 7761 7320 746f  st window was to
-00015910: 6f20 736d 616c 6c2c 2062 7574 2077 6173  o small, but was
-00015920: 2063 6f6d 7075 7465 6422 290a 0a20 2020   computed")..   
-00015930: 2064 656c 7461 5f74 203d 206e 702e 6172   delta_t = np.ar
-00015940: 7261 7928 6465 6c74 615f 7429 0a20 2020  ray(delta_t).   
-00015950: 2064 656c 7461 5f74 5f63 6f65 6620 3d20   delta_t_coef = 
-00015960: 6e70 2e61 7272 6179 2864 656c 7461 5f74  np.array(delta_t
-00015970: 5f63 6f65 6629 0a20 2020 2074 696d 655f  _coef).    time_
-00015980: 6178 6973 203d 206e 702e 6172 7261 7928  axis = np.array(
-00015990: 7469 6d65 5f61 7869 7329 0a0a 2020 2020  time_axis)..    
-000159a0: 2320 6c69 6e65 6172 2072 6567 7265 7373  # linear regress
-000159b0: 696f 6e20 746f 2067 6574 2064 762f 760a  ion to get dv/v.
-000159c0: 2020 2020 6966 2063 6f75 6e74 203e 2032      if count > 2
-000159d0: 3a0a 2020 2020 2020 2020 2320 7369 6d70  :.        # simp
-000159e0: 6c65 2077 6569 6768 740a 2020 2020 2020  le weight.      
-000159f0: 2020 7720 3d20 6e70 2e6f 6e65 7328 636f    w = np.ones(co
-00015a00: 756e 7429 0a20 2020 2020 2020 2023 206d  unt).        # m
-00015a10: 2c20 612c 2065 6d2c 2065 6120 3d20 6c69  , a, em, ea = li
-00015a20: 6e65 6172 5f72 6567 7265 7373 696f 6e28  near_regression(
-00015a30: 7469 6d65 5f61 7869 735b 696e 6478 5d2c  time_axis[indx],
-00015a40: 2064 656c 7461 5f74 5b69 6e64 785d 2c20   delta_t[indx], 
-00015a50: 772c 2069 6e74 6572 6365 7074 5f6f 7269  w, intercept_ori
-00015a60: 6769 6e3d 4661 6c73 6529 0a20 2020 2020  gin=False).     
-00015a70: 2020 206d 302c 2065 6d30 203d 206c 696e     m0, em0 = lin
-00015a80: 6561 725f 7265 6772 6573 7369 6f6e 2874  ear_regression(t
-00015a90: 696d 655f 6178 6973 2e66 6c61 7474 656e  ime_axis.flatten
-00015aa0: 2829 2c20 6465 6c74 615f 742e 666c 6174  (), delta_t.flat
-00015ab0: 7465 6e28 292c 2077 2e66 6c61 7474 656e  ten(), w.flatten
-00015ac0: 2829 2c20 696e 7465 7263 6570 745f 6f72  (), intercept_or
-00015ad0: 6967 696e 3d54 7275 6529 0a0a 2020 2020  igin=True)..    
-00015ae0: 656c 7365 3a0a 2020 2020 2020 2020 7072  else:.        pr
-00015af0: 696e 7428 226e 6f74 2065 6e6f 7567 6820  int("not enough 
-00015b00: 706f 696e 7473 2074 6f20 6573 7469 6d61  points to estima
-00015b10: 7465 2064 762f 7620 666f 7220 7763 6322  te dv/v for wcc"
-00015b20: 290a 2020 2020 2020 2020 6d30 203d 2030  ).        m0 = 0
-00015b30: 0a20 2020 2020 2020 2065 6d30 203d 2030  .        em0 = 0
-00015b40: 0a0a 2020 2020 7265 7475 726e 202d 6d30  ..    return -m0
-00015b50: 202a 2031 3030 2c20 656d 3020 2a20 3130   * 100, em0 * 10
-00015b60: 300a 0a0a 6465 6620 7778 735f 6476 7628  0...def wxs_dvv(
-00015b70: 0a20 2020 2072 6566 2c0a 2020 2020 6375  .    ref,.    cu
-00015b80: 722c 0a20 2020 2061 6c6c 6672 6571 2c0a  r,.    allfreq,.
-00015b90: 2020 2020 7061 7261 2c0a 2020 2020 646a      para,.    dj
-00015ba0: 3d31 202f 2031 322c 0a20 2020 2073 303d  =1 / 12,.    s0=
-00015bb0: 2d31 2c0a 2020 2020 4a3d 2d31 2c0a 2020  -1,.    J=-1,.  
-00015bc0: 2020 7369 673d 4661 6c73 652c 0a20 2020    sig=False,.   
-00015bd0: 2077 766e 3d22 6d6f 726c 6574 222c 0a20   wvn="morlet",. 
-00015be0: 2020 2075 6e77 7261 7066 6c61 673d 4661     unwrapflag=Fa
-00015bf0: 6c73 652c 0a29 3a0a 2020 2020 2222 220a  lse,.):.    """.
-00015c00: 2020 2020 436f 6d70 7574 6520 6474 206f      Compute dt o
-00015c10: 7220 6476 2f76 2069 6e20 7469 6d65 2061  r dv/v in time a
-00015c20: 6e64 2066 7265 7175 656e 6379 2064 6f6d  nd frequency dom
-00015c30: 6169 6e20 6672 6f6d 2077 6176 656c 6574  ain from wavelet
-00015c40: 2063 726f 7373 2073 7065 6374 7275 6d20   cross spectrum 
-00015c50: 2877 7873 292e 0a20 2020 2066 6f72 2061  (wxs)..    for a
-00015c60: 6c6c 2066 7265 7175 6563 6965 7320 696e  ll frequecies in
-00015c70: 2061 6e20 696e 7465 7265 7374 2072 616e   an interest ran
-00015c80: 6765 0a0a 2020 2020 5061 7261 6d65 7465  ge..    Paramete
-00015c90: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
-00015ca0: 2d2d 2d2d 2d0a 2020 2020 7265 663a 2054  -----.    ref: T
-00015cb0: 6865 2022 5265 6665 7265 6e63 6522 2074  he "Reference" t
-00015cc0: 696d 6573 6572 6965 7320 286e 756d 7079  imeseries (numpy
-00015cd0: 2e6e 6461 7272 6179 290a 2020 2020 6375  .ndarray).    cu
-00015ce0: 723a 2054 6865 2022 4375 7272 656e 7422  r: The "Current"
-00015cf0: 2074 696d 6573 6572 6965 7320 286e 756d   timeseries (num
-00015d00: 7079 2e6e 6461 7272 6179 290a 2020 2020  py.ndarray).    
-00015d10: 616c 6c66 7265 713a 2061 2062 6f6f 6c65  allfreq: a boole
-00015d20: 6e20 7661 7269 6162 6c65 2074 6f20 6d61  n variable to ma
-00015d30: 6b65 206d 6561 7375 7265 6d65 6e74 7320  ke measurements 
-00015d40: 6f6e 2061 6c6c 2066 7265 7175 656e 6379  on all frequency
-00015d50: 2072 616e 6765 206f 7220 6e6f 740a 2020   range or not.  
-00015d60: 2020 7061 7261 3a20 6120 6469 6374 2063    para: a dict c
-00015d70: 6f6e 7461 696e 696e 6720 6672 6571 2f74  ontaining freq/t
-00015d80: 696d 6520 696e 666f 206f 6620 7468 6520  ime info of the 
-00015d90: 6461 7461 206d 6174 7269 780a 2020 2020  data matrix.    
-00015da0: 646a 2c20 7330 2c20 4a2c 2073 6967 2c20  dj, s0, J, sig, 
-00015db0: 7776 6e3a 2063 6f6d 6d6f 6e20 7061 7261  wvn: common para
-00015dc0: 6d65 7465 7273 2075 7365 6420 696e 2027  meters used in '
-00015dd0: 7761 7665 6c65 742e 7763 7427 0a20 2020  wavelet.wct'.   
-00015de0: 2075 6e77 7261 7066 6c61 673a 2054 7275   unwrapflag: Tru
-00015df0: 6520 2d20 756e 7772 6170 2070 6861 7365  e - unwrap phase
-00015e00: 2064 656c 6179 732e 2044 6566 6175 6c74   delays. Default
-00015e10: 2069 7320 4661 6c73 650a 0a20 2020 2052   is False..    R
-00015e20: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
-00015e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-00015e40: 2020 2064 7676 2a31 3030 203a 2065 7374     dvv*100 : est
-00015e50: 696d 6174 6564 2064 762f 7620 696e 2025  imated dv/v in %
-00015e60: 0a20 2020 2065 7272 2a31 3030 203a 2065  .    err*100 : e
-00015e70: 7272 6f72 206f 6620 6476 2f76 2065 7374  rror of dv/v est
-00015e80: 696d 6174 696f 6e20 696e 2025 0a0a 2020  imation in %..  
-00015e90: 2020 4f72 6967 696e 616c 6c79 2077 7269    Originally wri
-00015ea0: 7474 656e 2062 7920 5469 6d20 436c 656d  tten by Tim Clem
-00015eb0: 656e 7473 2028 3120 4d61 7263 682c 2032  ents (1 March, 2
-00015ec0: 3031 3929 0a20 2020 204d 6f64 6966 6965  019).    Modifie
-00015ed0: 6420 6279 2043 6f6e 6763 6f6e 6720 5975  d by Congcong Yu
-00015ee0: 616e 2028 3330 204a 756e 652c 2032 3031  an (30 June, 201
-00015ef0: 3929 2062 6173 6564 206f 6e20 284d 616f  9) based on (Mao
-00015f00: 2065 7420 616c 2e20 3230 3139 292e 0a20   et al. 2019).. 
-00015f10: 2020 2055 7064 6174 6564 2062 7920 4368     Updated by Ch
-00015f20: 656e 6778 696e 204a 6961 6e67 2028 3130  engxin Jiang (10
-00015f30: 204f 6374 2c20 3230 3139 2920 746f 206d   Oct, 2019) to m
-00015f40: 6572 6765 2074 6865 2066 756e 6374 696f  erge the functio
-00015f50: 6e61 6c69 7479 2066 6f72 206d 6573 7572  nality for mesur
-00015f60: 656d 656e 7473 0a20 2020 2061 6372 6f73  ements.    acros
-00015f70: 7320 616c 6c20 6672 6571 7565 6e63 7920  s all frequency 
-00015f80: 616e 6420 6f6e 6520 6672 6571 2072 616e  and one freq ran
-00015f90: 6765 0a20 2020 2022 2222 0a20 2020 2023  ge.    """.    #
-00015fa0: 2063 6f6d 6d6f 6e20 7661 7269 6162 6c65   common variable
-00015fb0: 730a 2020 2020 7477 696e 203d 2070 6172  s.    twin = par
-00015fc0: 615b 2274 7769 6e22 5d0a 2020 2020 6672  a["twin"].    fr
-00015fd0: 6571 203d 2070 6172 615b 2266 7265 7122  eq = para["freq"
-00015fe0: 5d0a 2020 2020 6474 203d 2070 6172 615b  ].    dt = para[
-00015ff0: 2264 7422 5d0a 2020 2020 746d 696e 203d  "dt"].    tmin =
-00016000: 206e 702e 6d69 6e28 7477 696e 290a 2020   np.min(twin).  
-00016010: 2020 746d 6178 203d 206e 702e 6d61 7828    tmax = np.max(
-00016020: 7477 696e 290a 2020 2020 666d 696e 203d  twin).    fmin =
-00016030: 206e 702e 6d69 6e28 6672 6571 290a 2020   np.min(freq).  
-00016040: 2020 666d 6178 203d 206e 702e 6d61 7828    fmax = np.max(
-00016050: 6672 6571 290a 2020 2020 7476 6563 203d  freq).    tvec =
-00016060: 206e 702e 6172 616e 6765 2874 6d69 6e2c   np.arange(tmin,
-00016070: 2074 6d61 782c 2064 7429 0a20 2020 206e   tmax, dt).    n
-00016080: 7074 7320 3d20 6c65 6e28 7476 6563 290a  pts = len(tvec).
-00016090: 0a20 2020 2023 2070 6572 666f 726d 2063  .    # perform c
-000160a0: 726f 7373 2063 6f68 6572 656e 7420 616e  ross coherent an
-000160b0: 616c 7973 6973 2c20 6d6f 6469 6669 6564  alysis, modified
-000160c0: 2066 726f 6d20 6675 6e63 7469 6f6e 2027   from function '
-000160d0: 7761 7665 6c65 742e 6377 7427 0a20 2020  wavelet.cwt'.   
-000160e0: 2057 4354 2c20 6157 4354 2c20 636f 692c   WCT, aWCT, coi,
-000160f0: 2066 7265 712c 2073 6967 203d 2077 6374   freq, sig = wct
-00016100: 5f6d 6f64 6966 6965 6428 7265 662c 2063  _modified(ref, c
-00016110: 7572 2c20 6474 2c20 646a 3d64 6a2c 2073  ur, dt, dj=dj, s
-00016120: 303d 7330 2c20 4a3d 4a2c 2073 6967 3d73  0=s0, J=J, sig=s
-00016130: 6967 2c20 7761 7665 6c65 743d 7776 6e2c  ig, wavelet=wvn,
-00016140: 206e 6f72 6d61 6c69 7a65 3d54 7275 6529   normalize=True)
-00016150: 0a0a 2020 2020 6966 2075 6e77 7261 7066  ..    if unwrapf
-00016160: 6c61 673a 0a20 2020 2020 2020 2070 6861  lag:.        pha
-00016170: 7365 203d 206e 702e 756e 7772 6170 2861  se = np.unwrap(a
-00016180: 5743 542c 2061 7869 733d 2d31 2920 2023  WCT, axis=-1)  #
-00016190: 2061 7869 733d 302c 2075 7077 7261 7020   axis=0, upwrap 
-000161a0: 616c 6f6e 6720 7469 6d65 3b20 6178 6973  along time; axis
-000161b0: 3d2d 312c 2075 6e77 7261 7020 616c 6f6e  =-1, unwrap alon
-000161c0: 6720 6672 6571 7565 6e63 790a 2020 2020  g frequency.    
-000161d0: 656c 7365 3a0a 2020 2020 2020 2020 7068  else:.        ph
-000161e0: 6173 6520 3d20 6157 4354 0a0a 2020 2020  ase = aWCT..    
-000161f0: 2320 7a65 726f 206f 7574 2064 6174 6120  # zero out data 
-00016200: 6f75 7473 6964 6520 6672 6571 7565 6e63  outside frequenc
-00016210: 7920 6261 6e64 0a20 2020 2069 6620 2866  y band.    if (f
-00016220: 6d61 7820 3e20 6e70 2e6d 6178 2866 7265  max > np.max(fre
-00016230: 7129 2920 7c20 2866 6d61 7820 3c3d 2066  q)) | (fmax <= f
-00016240: 6d69 6e29 3a0a 2020 2020 2020 2020 7261  min):.        ra
-00016250: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
-00016260: 4162 6f72 743a 2069 6e70 7574 2066 7265  Abort: input fre
-00016270: 7175 656e 6379 206f 7574 206f 6620 6c69  quency out of li
-00016280: 6d69 7473 2122 290a 2020 2020 656c 7365  mits!").    else
-00016290: 3a0a 2020 2020 2020 2020 6672 6571 5f69  :.        freq_i
-000162a0: 6e64 696e 203d 206e 702e 7768 6572 6528  ndin = np.where(
-000162b0: 2866 7265 7120 3e3d 2066 6d69 6e29 2026  (freq >= fmin) &
-000162c0: 2028 6672 6571 203c 3d20 666d 6178 2929   (freq <= fmax))
-000162d0: 5b30 5d0a 0a20 2020 2023 2066 6f6c 6c6f  [0]..    # follo
-000162e0: 7720 4d57 4353 2074 6f20 646f 2074 776f  w MWCS to do two
-000162f0: 2073 7465 7073 206f 6620 6c69 6e65 6172   steps of linear
-00016300: 2072 6567 7265 7373 696f 6e0a 2020 2020   regression.    
-00016310: 6966 206e 6f74 2061 6c6c 6672 6571 3a0a  if not allfreq:.
-00016320: 2020 2020 2020 2020 6465 6c74 615f 745f          delta_t_
-00016330: 6d2c 2064 656c 7461 5f74 5f75 6e63 203d  m, delta_t_unc =
-00016340: 206e 702e 7a65 726f 7328 6e70 7473 2c20   np.zeros(npts, 
-00016350: 6474 7970 653d 6e70 2e66 6c6f 6174 3332  dtype=np.float32
-00016360: 292c 206e 702e 7a65 726f 7328 6e70 7473  ), np.zeros(npts
-00016370: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
-00016380: 3332 290a 2020 2020 2020 2020 2320 6173  32).        # as
-00016390: 7375 6d65 2074 6865 2074 7665 6320 6973  sume the tvec is
-000163a0: 2074 6865 2074 696d 6520 7769 6e64 6f77   the time window
-000163b0: 2074 6f20 6d65 6173 7572 6520 6474 0a20   to measure dt. 
-000163c0: 2020 2020 2020 2066 6f72 2069 7420 696e         for it in
-000163d0: 2072 616e 6765 286e 7074 7329 3a0a 2020   range(npts):.  
-000163e0: 2020 2020 2020 2020 2020 7720 3d20 3120            w = 1 
-000163f0: 2f20 5743 545b 6672 6571 5f69 6e64 696e  / WCT[freq_indin
-00016400: 2c20 6974 5d0a 2020 2020 2020 2020 2020  , it].          
-00016410: 2020 775b 7e6e 702e 6973 6669 6e69 7465    w[~np.isfinite
-00016420: 2877 295d 203d 2031 2e30 0a20 2020 2020  (w)] = 1.0.     
-00016430: 2020 2020 2020 2064 656c 7461 5f74 5f6d         delta_t_m
-00016440: 5b69 745d 2c20 6465 6c74 615f 745f 756e  [it], delta_t_un
-00016450: 635b 6974 5d20 3d20 6c69 6e65 6172 5f72  c[it] = linear_r
-00016460: 6567 7265 7373 696f 6e28 6672 6571 5b66  egression(freq[f
-00016470: 7265 715f 696e 6469 6e5d 202a 2032 202a  req_indin] * 2 *
-00016480: 206e 702e 7069 2c20 7068 6173 655b 6672   np.pi, phase[fr
-00016490: 6571 5f69 6e64 696e 2c20 6974 5d2c 2077  eq_indin, it], w
-000164a0: 290a 0a20 2020 2020 2020 2023 206e 6577  )..        # new
-000164b0: 2077 6569 6768 7473 2066 6f72 2072 6567   weights for reg
-000164c0: 7265 7373 696f 6e0a 2020 2020 2020 2020  ression.        
-000164d0: 7732 203d 2031 202f 206e 702e 6d65 616e  w2 = 1 / np.mean
-000164e0: 2857 4354 5b66 7265 715f 696e 6469 6e2c  (WCT[freq_indin,
-000164f0: 203a 5d2c 2061 7869 733d 3029 0a20 2020   :], axis=0).   
-00016500: 2020 2020 2077 325b 7e6e 702e 6973 6669       w2[~np.isfi
-00016510: 6e69 7465 2877 3229 5d20 3d20 312e 300a  nite(w2)] = 1.0.
-00016520: 0a20 2020 2020 2020 2023 206e 6f77 2075  .        # now u
-00016530: 7365 2064 7420 616e 6420 7420 746f 2067  se dt and t to g
-00016540: 6574 2064 762f 760a 2020 2020 2020 2020  et dv/v.        
-00016550: 6966 206c 656e 2877 3229 203e 2032 3a0a  if len(w2) > 2:.
-00016560: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00016570: 6f74 206e 702e 616e 7928 6465 6c74 615f  ot np.any(delta_
-00016580: 745f 6d29 3a0a 2020 2020 2020 2020 2020  t_m):.          
-00016590: 2020 2020 2020 6476 762c 2065 7272 203d        dvv, err =
-000165a0: 206e 702e 6e61 6e2c 206e 702e 6e61 6e0a   np.nan, np.nan.
-000165b0: 2020 2020 2020 2020 2020 2020 6d2c 2065              m, e
-000165c0: 6d20 3d20 6c69 6e65 6172 5f72 6567 7265  m = linear_regre
-000165d0: 7373 696f 6e28 7476 6563 2c20 6465 6c74  ssion(tvec, delt
-000165e0: 615f 745f 6d2c 2077 322c 2069 6e74 6572  a_t_m, w2, inter
-000165f0: 6365 7074 5f6f 7269 6769 6e3d 5472 7565  cept_origin=True
-00016600: 290a 2020 2020 2020 2020 2020 2020 6476  ).            dv
-00016610: 762c 2065 7272 203d 202d 6d2c 2065 6d0a  v, err = -m, em.
-00016620: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00016630: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00016640: 226e 6f74 2065 6e6f 7567 6820 706f 696e  "not enough poin
-00016650: 7473 2074 6f20 6573 7469 6d61 7465 2064  ts to estimate d
-00016660: 762f 7620 666f 7220 7774 7322 290a 2020  v/v for wts").  
-00016670: 2020 2020 2020 2020 2020 6476 762c 2065            dvv, e
-00016680: 7272 203d 206e 702e 6e61 6e2c 206e 702e  rr = np.nan, np.
-00016690: 6e61 6e0a 0a20 2020 2020 2020 2072 6574  nan..        ret
-000166a0: 7572 6e20 6476 7620 2a20 3130 302c 2065  urn dvv * 100, e
-000166b0: 7272 202a 2031 3030 0a0a 2020 2020 2320  rr * 100..    # 
-000166c0: 636f 6e76 6572 7420 7068 6173 6520 6469  convert phase di
-000166d0: 7265 6374 6c79 2074 6f20 6465 6c74 615f  rectly to delta_
-000166e0: 7420 666f 7220 616c 6c20 6672 6571 7565  t for all freque
-000166f0: 6e63 6965 730a 2020 2020 656c 7365 3a0a  ncies.    else:.
-00016700: 2020 2020 2020 2020 2320 636f 6e76 6572          # conver
-00016710: 7420 7068 6173 6520 6465 6c61 7920 746f  t phase delay to
-00016720: 2074 696d 6520 6465 6c61 790a 2020 2020   time delay.    
-00016730: 2020 2020 6465 6c74 615f 7420 3d20 7068      delta_t = ph
-00016740: 6173 6520 2f20 2832 202a 206e 702e 7069  ase / (2 * np.pi
-00016750: 202a 2066 7265 715b 3a2c 204e 6f6e 655d   * freq[:, None]
-00016760: 2920 2023 206e 6f72 6d61 6c69 7a65 2070  )  # normalize p
-00016770: 6861 7365 2062 7920 2832 2a70 692a 6672  hase by (2*pi*fr
-00016780: 6571 7565 6e63 7929 0a20 2020 2020 2020  equency).       
-00016790: 2064 7676 2c20 6572 7220 3d20 6e70 2e7a   dvv, err = np.z
-000167a0: 6572 6f73 2866 7265 715f 696e 6469 6e2e  eros(freq_indin.
-000167b0: 7368 6170 6529 2c20 6e70 2e7a 6572 6f73  shape), np.zeros
-000167c0: 2866 7265 715f 696e 6469 6e2e 7368 6170  (freq_indin.shap
-000167d0: 6529 0a0a 2020 2020 2020 2020 2320 6c6f  e)..        # lo
-000167e0: 6f70 2074 6872 6f75 6768 2066 7265 7120  op through freq 
-000167f0: 666f 7220 6c69 6e65 6172 2072 6567 7265  for linear regre
-00016800: 7373 696f 6e0a 2020 2020 2020 2020 666f  ssion.        fo
-00016810: 7220 6969 2c20 6966 7265 7120 696e 2065  r ii, ifreq in e
-00016820: 6e75 6d65 7261 7465 2866 7265 715f 696e  numerate(freq_in
-00016830: 6469 6e29 3a0a 2020 2020 2020 2020 2020  din):.          
-00016840: 2020 6966 206c 656e 2874 7665 6329 203e    if len(tvec) >
-00016850: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-00016860: 2020 2020 6966 206e 6f74 206e 702e 616e      if not np.an
-00016870: 7928 6465 6c74 615f 745b 6966 7265 715d  y(delta_t[ifreq]
-00016880: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00016890: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-000168a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000168b0: 2023 2068 6f77 2074 6f20 6265 7474 6572   # how to better
-000168c0: 2061 7070 726f 6163 6820 7468 6520 756e   approach the un
-000168d0: 6365 7274 6169 6e74 7920 6f66 2064 656c  certainty of del
-000168e0: 7461 5f74 0a20 2020 2020 2020 2020 2020  ta_t.           
-000168f0: 2020 2020 2077 203d 2031 202f 2057 4354       w = 1 / WCT
-00016900: 5b69 6672 6571 5d0a 2020 2020 2020 2020  [ifreq].        
-00016910: 2020 2020 2020 2020 775b 7e6e 702e 6973          w[~np.is
-00016920: 6669 6e69 7465 2877 295d 203d 2031 2e30  finite(w)] = 1.0
-00016930: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00016940: 2020 2320 6d2c 2061 2c20 656d 2c20 6561    # m, a, em, ea
-00016950: 203d 206c 696e 6561 725f 7265 6772 6573   = linear_regres
-00016960: 7369 6f6e 2874 696d 655f 6178 6973 5b69  sion(time_axis[i
-00016970: 6e64 785d 2c20 6465 6c74 615f 745b 696e  ndx], delta_t[in
-00016980: 6478 5d2c 2077 2c20 696e 7465 7263 6570  dx], w, intercep
-00016990: 745f 6f72 6967 696e 3d46 616c 7365 290a  t_origin=False).
-000169a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000169b0: 6d2c 2065 6d20 3d20 6c69 6e65 6172 5f72  m, em = linear_r
-000169c0: 6567 7265 7373 696f 6e28 7476 6563 2c20  egression(tvec, 
-000169d0: 6465 6c74 615f 745b 6966 7265 715d 2c20  delta_t[ifreq], 
-000169e0: 772c 2069 6e74 6572 6365 7074 5f6f 7269  w, intercept_ori
-000169f0: 6769 6e3d 5472 7565 290a 2020 2020 2020  gin=True).      
-00016a00: 2020 2020 2020 2020 2020 6476 765b 6969            dvv[ii
-00016a10: 5d2c 2065 7272 5b69 695d 203d 202d 6d2c  ], err[ii] = -m,
-00016a20: 2065 6d0a 2020 2020 2020 2020 2020 2020   em.            
-00016a30: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00016a40: 2020 2020 2020 7072 696e 7428 226e 6f74        print("not
-00016a50: 2065 6e6f 7567 6820 706f 696e 7473 2074   enough points t
-00016a60: 6f20 6573 7469 6d61 7465 2064 762f 7620  o estimate dv/v 
-00016a70: 666f 7220 7774 7322 290a 2020 2020 2020  for wts").      
-00016a80: 2020 2020 2020 2020 2020 6476 765b 6969            dvv[ii
-00016a90: 5d2c 2065 7272 5b69 695d 203d 206e 702e  ], err[ii] = np.
-00016aa0: 6e61 6e2c 206e 702e 6e61 6e0a 0a20 2020  nan, np.nan..   
-00016ab0: 2020 2020 2072 6574 7572 6e20 6672 6571       return freq
-00016ac0: 5b66 7265 715f 696e 6469 6e5d 2c20 6476  [freq_indin], dv
-00016ad0: 7620 2a20 3130 302c 2065 7272 202a 2031  v * 100, err * 1
-00016ae0: 3030 0a0a 0a64 6566 2077 7473 5f64 7676  00...def wts_dvv
-00016af0: 280a 2020 2020 7265 662c 0a20 2020 2063  (.    ref,.    c
-00016b00: 7572 2c0a 2020 2020 616c 6c66 7265 712c  ur,.    allfreq,
-00016b10: 0a20 2020 2070 6172 612c 0a20 2020 2064  .    para,.    d
-00016b20: 765f 7261 6e67 652c 0a20 2020 206e 6274  v_range,.    nbt
-00016b30: 7269 616c 2c0a 2020 2020 646a 3d31 202f  rial,.    dj=1 /
-00016b40: 2031 322c 0a20 2020 2073 303d 2d31 2c0a   12,.    s0=-1,.
-00016b50: 2020 2020 4a3d 2d31 2c0a 2020 2020 7776      J=-1,.    wv
-00016b60: 6e3d 226d 6f72 6c65 7422 2c0a 2020 2020  n="morlet",.    
-00016b70: 6e6f 726d 616c 697a 653d 5472 7565 2c0a  normalize=True,.
-00016b80: 293a 0a20 2020 2022 2222 0a20 2020 2041  ):.    """.    A
-00016b90: 7070 6c79 2073 7472 6574 6368 696e 6720  pply stretching 
-00016ba0: 6d65 7468 6f64 2074 6f20 636f 6e74 696e  method to contin
-00016bb0: 756f 7573 2077 6176 656c 6574 2074 7261  uous wavelet tra
-00016bc0: 6e73 666f 726d 6174 696f 6e20 2843 5754  nsformation (CWT
-00016bd0: 2920 6f66 2073 6967 6e61 6c73 0a20 2020  ) of signals.   
-00016be0: 2066 6f72 2061 6c6c 2066 7265 7175 6563   for all frequec
-00016bf0: 6965 7320 696e 2061 6e20 696e 7465 7265  ies in an intere
-00016c00: 7374 2072 616e 6765 0a0a 2020 2020 5061  st range..    Pa
-00016c10: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-00016c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-00016c30: 7265 663a 2054 6865 2022 5265 6665 7265  ref: The "Refere
-00016c40: 6e63 6522 2074 696d 6573 6572 6965 7320  nce" timeseries 
-00016c50: 286e 756d 7079 2e6e 6461 7272 6179 290a  (numpy.ndarray).
-00016c60: 2020 2020 6375 723a 2054 6865 2022 4375      cur: The "Cu
-00016c70: 7272 656e 7422 2074 696d 6573 6572 6965  rrent" timeserie
-00016c80: 7320 286e 756d 7079 2e6e 6461 7272 6179  s (numpy.ndarray
-00016c90: 290a 2020 2020 616c 6c66 7265 713a 2061  ).    allfreq: a
-00016ca0: 2062 6f6f 6c65 6e20 7661 7269 6162 6c65   boolen variable
-00016cb0: 2074 6f20 6d61 6b65 206d 6561 7375 7265   to make measure
-00016cc0: 6d65 6e74 7320 6f6e 2061 6c6c 2066 7265  ments on all fre
-00016cd0: 7175 656e 6379 2072 616e 6765 206f 7220  quency range or 
-00016ce0: 6e6f 740a 2020 2020 7061 7261 3a20 6120  not.    para: a 
-00016cf0: 6469 6374 2063 6f6e 7461 696e 696e 6720  dict containing 
-00016d00: 6672 6571 2f74 696d 6520 696e 666f 206f  freq/time info o
-00016d10: 6620 7468 6520 6461 7461 206d 6174 7269  f the data matri
-00016d20: 780a 2020 2020 6476 5f72 616e 6765 3a20  x.    dv_range: 
-00016d30: 6162 736f 6c75 7465 2062 6f75 6e64 2066  absolute bound f
-00016d40: 6f72 2074 6865 2076 656c 6f63 6974 7920  or the velocity 
-00016d50: 7661 7269 6174 696f 6e3b 2065 7861 6d70  variation; examp
-00016d60: 6c65 3a20 6476 3d30 2e30 3320 666f 7220  le: dv=0.03 for 
-00016d70: 5b2d 332c 335d 250a 2020 2020 6f66 2072  [-3,3]%.    of r
-00016d80: 656c 6174 6976 6520 7665 6c6f 6369 7479  elative velocity
-00016d90: 2063 6861 6e67 6520 2866 6c6f 6174 290a   change (float).
-00016da0: 2020 2020 6e62 7472 6961 6c3a 206e 756d      nbtrial: num
-00016db0: 6265 7220 6f66 2073 7472 6574 6368 696e  ber of stretchin
-00016dc0: 6720 636f 6566 6669 6369 656e 7420 6265  g coefficient be
-00016dd0: 7477 6565 6e20 6476 6d69 6e20 616e 6420  tween dvmin and 
-00016de0: 6476 6d61 782c 206e 6f20 6e65 6564 2074  dvmax, no need t
-00016df0: 6f20 6265 2068 6967 6865 7220 7468 616e  o be higher than
-00016e00: 2031 3030 2020 2866 6c6f 6174 290a 2020   100  (float).  
-00016e10: 2020 646a 2c20 7330 2c20 4a2c 2073 6967    dj, s0, J, sig
-00016e20: 2c20 7776 6e3a 2063 6f6d 6d6f 6e20 7061  , wvn: common pa
-00016e30: 7261 6d65 7465 7273 2075 7365 6420 696e  rameters used in
-00016e40: 2027 7761 7665 6c65 742e 7763 7427 0a20   'wavelet.wct'. 
-00016e50: 2020 206e 6f72 6d61 6c69 7a65 3a20 6e6f     normalize: no
-00016e60: 726d 616c 697a 6520 7468 6520 7761 7665  rmalize the wave
-00016e70: 6c65 7420 7370 6563 7472 756d 206f 7220  let spectrum or 
-00016e80: 6e6f 742e 2044 6566 6175 6c74 2069 7320  not. Default is 
-00016e90: 5472 7565 0a0a 2020 2020 5245 5455 524e  True..    RETURN
-00016ea0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-00016eb0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6476  ---------.    dv
-00016ec0: 763a 2065 7374 696d 6174 6564 2064 762f  v: estimated dv/
-00016ed0: 760a 2020 2020 6572 723a 2065 7272 6f72  v.    err: error
-00016ee0: 206f 6620 6476 2f76 2065 7374 696d 6174   of dv/v estimat
-00016ef0: 696f 6e0a 0a20 2020 2057 7269 7474 656e  ion..    Written
-00016f00: 2062 7920 436f 6e67 636f 6e67 2059 7561   by Congcong Yua
-00016f10: 6e20 2833 3020 4a75 6e2c 2032 3031 3929  n (30 Jun, 2019)
-00016f20: 0a20 2020 2022 2222 0a20 2020 2023 2063  .    """.    # c
-00016f30: 6f6d 6d6f 6e20 7661 7269 6162 6c65 730a  ommon variables.
-00016f40: 2020 2020 6672 6571 203d 2070 6172 615b      freq = para[
-00016f50: 2266 7265 7122 5d0a 2020 2020 6474 203d  "freq"].    dt =
-00016f60: 2070 6172 615b 2264 7422 5d0a 2020 2020   para["dt"].    
-00016f70: 666d 696e 203d 206e 702e 6d69 6e28 6672  fmin = np.min(fr
-00016f80: 6571 290a 2020 2020 666d 6178 203d 206e  eq).    fmax = n
-00016f90: 702e 6d61 7828 6672 6571 290a 0a20 2020  p.max(freq)..   
-00016fa0: 2023 2061 7070 6c79 2063 7774 206f 6e20   # apply cwt on 
-00016fb0: 7477 6f20 7472 6163 6573 0a20 2020 2063  two traces.    c
-00016fc0: 7774 312c 2073 6a2c 2066 7265 712c 2063  wt1, sj, freq, c
-00016fd0: 6f69 2c20 5f2c 205f 203d 2070 7963 7774  oi, _, _ = pycwt
-00016fe0: 2e63 7774 2863 7572 2c20 6474 2c20 646a  .cwt(cur, dt, dj
-00016ff0: 2c20 7330 2c20 4a2c 2077 766e 290a 2020  , s0, J, wvn).  
-00017000: 2020 6377 7432 2c20 736a 2c20 6672 6571    cwt2, sj, freq
-00017010: 2c20 636f 692c 205f 2c20 5f20 3d20 7079  , coi, _, _ = py
-00017020: 6377 742e 6377 7428 7265 662c 2064 742c  cwt.cwt(ref, dt,
-00017030: 2064 6a2c 2073 302c 204a 2c20 7776 6e29   dj, s0, J, wvn)
-00017040: 0a0a 2020 2020 2320 6578 7472 6163 7420  ..    # extract 
-00017050: 7265 616c 2076 616c 7565 7320 6f66 2063  real values of c
-00017060: 7774 0a20 2020 2072 6377 7431 2c20 7263  wt.    rcwt1, rc
-00017070: 7774 3220 3d20 6e70 2e72 6561 6c28 6377  wt2 = np.real(cw
-00017080: 7431 292c 206e 702e 7265 616c 2863 7774  t1), np.real(cwt
-00017090: 3229 0a0a 2020 2020 2320 7a65 726f 206f  2)..    # zero o
-000170a0: 7574 2064 6174 6120 6f75 7473 6964 6520  ut data outside 
-000170b0: 6672 6571 7565 6e63 7920 6261 6e64 0a20  frequency band. 
-000170c0: 2020 2069 6620 2866 6d61 7820 3e20 6e70     if (fmax > np
-000170d0: 2e6d 6178 2866 7265 7129 2920 7c20 2866  .max(freq)) | (f
-000170e0: 6d61 7820 3c3d 2066 6d69 6e29 3a0a 2020  max <= fmin):.  
-000170f0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00017100: 6545 7272 6f72 2822 4162 6f72 743a 2069  eError("Abort: i
-00017110: 6e70 7574 2066 7265 7175 656e 6379 206f  nput frequency o
-00017120: 7574 206f 6620 6c69 6d69 7473 2122 290a  ut of limits!").
-00017130: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00017140: 2020 6672 6571 5f69 6e64 696e 203d 206e    freq_indin = n
-00017150: 702e 7768 6572 6528 2866 7265 7120 3e3d  p.where((freq >=
-00017160: 2066 6d69 6e29 2026 2028 6672 6571 203c   fmin) & (freq <
-00017170: 3d20 666d 6178 2929 5b30 5d0a 0a20 2020  = fmax))[0]..   
-00017180: 2023 2063 6f6e 7665 7274 2077 6176 656c   # convert wavel
-00017190: 6574 2064 6f6d 6169 6e20 6261 636b 2074  et domain back t
-000171a0: 6f20 7469 6d65 2064 6f6d 6169 6e20 287e  o time domain (~
-000171b0: 6669 6c74 6572 696e 6729 0a20 2020 2069  filtering).    i
-000171c0: 6620 6e6f 7420 616c 6c66 7265 713a 0a20  f not allfreq:. 
-000171d0: 2020 2020 2020 2023 2069 6e76 6572 7365         # inverse
-000171e0: 2063 7774 2074 6f20 7469 6d65 2064 6f6d   cwt to time dom
-000171f0: 6169 6e0a 2020 2020 2020 2020 6963 7774  ain.        icwt
-00017200: 3120 3d20 7079 6377 742e 6963 7774 2863  1 = pycwt.icwt(c
-00017210: 7774 315b 6672 6571 5f69 6e64 696e 5d2c  wt1[freq_indin],
-00017220: 2073 6a5b 6672 6571 5f69 6e64 696e 5d2c   sj[freq_indin],
-00017230: 2064 742c 2064 6a2c 2077 766e 290a 2020   dt, dj, wvn).  
-00017240: 2020 2020 2020 6963 7774 3220 3d20 7079        icwt2 = py
-00017250: 6377 742e 6963 7774 2863 7774 325b 6672  cwt.icwt(cwt2[fr
-00017260: 6571 5f69 6e64 696e 5d2c 2073 6a5b 6672  eq_indin], sj[fr
-00017270: 6571 5f69 6e64 696e 5d2c 2064 742c 2064  eq_indin], dt, d
-00017280: 6a2c 2077 766e 290a 0a20 2020 2020 2020  j, wvn)..       
-00017290: 2023 2061 7373 756d 6520 616c 6c20 7469   # assume all ti
-000172a0: 6d65 2077 696e 646f 7720 6973 2075 7365  me window is use
-000172b0: 640a 2020 2020 2020 2020 7763 7774 312c  d.        wcwt1,
-000172c0: 2077 6377 7432 203d 206e 702e 7265 616c   wcwt2 = np.real
-000172d0: 2869 6377 7431 292c 206e 702e 7265 616c  (icwt1), np.real
-000172e0: 2869 6377 7432 290a 0a20 2020 2020 2020  (icwt2)..       
-000172f0: 2023 204e 6f72 6d61 6c69 7a65 7320 626f   # Normalizes bo
-00017300: 7468 2073 6967 6e61 6c73 2c20 6966 2061  th signals, if a
-00017310: 7070 726f 7072 6961 7465 2e0a 2020 2020  ppropriate..    
-00017320: 2020 2020 6966 206e 6f72 6d61 6c69 7a65      if normalize
-00017330: 3a0a 2020 2020 2020 2020 2020 2020 6e63  :.            nc
-00017340: 7774 3120 3d20 2877 6377 7431 202d 2077  wt1 = (wcwt1 - w
-00017350: 6377 7431 2e6d 6561 6e28 2929 202f 2077  cwt1.mean()) / w
-00017360: 6377 7431 2e73 7464 2829 0a20 2020 2020  cwt1.std().     
-00017370: 2020 2020 2020 206e 6377 7432 203d 2028         ncwt2 = (
-00017380: 7763 7774 3220 2d20 7763 7774 322e 6d65  wcwt2 - wcwt2.me
-00017390: 616e 2829 2920 2f20 7763 7774 322e 7374  an()) / wcwt2.st
-000173a0: 6428 290a 2020 2020 2020 2020 656c 7365  d().        else
-000173b0: 3a0a 2020 2020 2020 2020 2020 2020 6e63  :.            nc
-000173c0: 7774 3120 3d20 7763 7774 310a 2020 2020  wt1 = wcwt1.    
-000173d0: 2020 2020 2020 2020 6e63 7774 3220 3d20          ncwt2 = 
-000173e0: 7763 7774 320a 0a20 2020 2020 2020 2023  wcwt2..        #
-000173f0: 2072 756e 2073 7472 6574 6368 696e 670a   run stretching.
-00017400: 2020 2020 2020 2020 6476 762c 2065 7272          dvv, err
-00017410: 2c20 6363 2c20 6364 7020 3d20 7374 7265  , cc, cdp = stre
-00017420: 7463 6869 6e67 286e 6377 7432 2c20 6e63  tching(ncwt2, nc
-00017430: 7774 312c 2064 765f 7261 6e67 652c 206e  wt1, dv_range, n
-00017440: 6274 7269 616c 2c20 7061 7261 290a 2020  btrial, para).  
-00017450: 2020 2020 2020 7265 7475 726e 2064 7676        return dvv
-00017460: 2c20 6572 720a 0a20 2020 2023 2064 6972  , err..    # dir
-00017470: 6563 746c 7920 7461 6b65 2061 6476 616e  ectly take advan
-00017480: 7461 6765 206f 6620 7468 650a 2020 2020  tage of the.    
-00017490: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
-000174a0: 696e 6974 6961 6c69 7a65 2076 6172 6961  initialize varia
-000174b0: 626c 650a 2020 2020 2020 2020 6e66 7265  ble.        nfre
-000174c0: 7120 3d20 6c65 6e28 6672 6571 5f69 6e64  q = len(freq_ind
-000174d0: 696e 290a 2020 2020 2020 2020 6476 762c  in).        dvv,
-000174e0: 2063 632c 2063 6470 2c20 6572 7220 3d20   cc, cdp, err = 
-000174f0: 280a 2020 2020 2020 2020 2020 2020 6e70  (.            np
-00017500: 2e7a 6572 6f73 286e 6672 6571 2c20 6474  .zeros(nfreq, dt
-00017510: 7970 653d 6e70 2e66 6c6f 6174 3332 292c  ype=np.float32),
-00017520: 0a20 2020 2020 2020 2020 2020 206e 702e  .            np.
-00017530: 7a65 726f 7328 6e66 7265 712c 2064 7479  zeros(nfreq, dty
-00017540: 7065 3d6e 702e 666c 6f61 7433 3229 2c0a  pe=np.float32),.
-00017550: 2020 2020 2020 2020 2020 2020 6e70 2e7a              np.z
-00017560: 6572 6f73 286e 6672 6571 2c20 6474 7970  eros(nfreq, dtyp
-00017570: 653d 6e70 2e66 6c6f 6174 3332 292c 0a20  e=np.float32),. 
-00017580: 2020 2020 2020 2020 2020 206e 702e 7a65             np.ze
-00017590: 726f 7328 6e66 7265 712c 2064 7479 7065  ros(nfreq, dtype
-000175a0: 3d6e 702e 666c 6f61 7433 3229 2c0a 2020  =np.float32),.  
-000175b0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000175c0: 2023 206c 6f6f 7020 7468 726f 7567 6820   # loop through 
-000175d0: 6561 6368 2066 7265 710a 2020 2020 2020  each freq.      
-000175e0: 2020 666f 7220 6969 2c20 6966 7265 7120    for ii, ifreq 
-000175f0: 696e 2065 6e75 6d65 7261 7465 2866 7265  in enumerate(fre
-00017600: 715f 696e 6469 6e29 3a0a 2020 2020 2020  q_indin):.      
-00017610: 2020 2020 2020 2320 7072 6570 6172 6520        # prepare 
-00017620: 7769 6e64 6f77 6564 2064 6174 610a 2020  windowed data.  
-00017630: 2020 2020 2020 2020 2020 7763 7774 312c            wcwt1,
-00017640: 2077 6377 7432 203d 2072 6377 7431 5b69   wcwt2 = rcwt1[i
-00017650: 6672 6571 5d2c 2072 6377 7432 5b69 6672  freq], rcwt2[ifr
-00017660: 6571 5d0a 0a20 2020 2020 2020 2020 2020  eq]..           
-00017670: 2023 204e 6f72 6d61 6c69 7a65 7320 626f   # Normalizes bo
-00017680: 7468 2073 6967 6e61 6c73 2c20 6966 2061  th signals, if a
-00017690: 7070 726f 7072 6961 7465 2e0a 2020 2020  ppropriate..    
-000176a0: 2020 2020 2020 2020 6966 206e 6f72 6d61          if norma
-000176b0: 6c69 7a65 3a0a 2020 2020 2020 2020 2020  lize:.          
-000176c0: 2020 2020 2020 6e63 7774 3120 3d20 2877        ncwt1 = (w
-000176d0: 6377 7431 202d 2077 6377 7431 2e6d 6561  cwt1 - wcwt1.mea
-000176e0: 6e28 2929 202f 2077 6377 7431 2e73 7464  n()) / wcwt1.std
-000176f0: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00017700: 2020 206e 6377 7432 203d 2028 7763 7774     ncwt2 = (wcwt
-00017710: 3220 2d20 7763 7774 322e 6d65 616e 2829  2 - wcwt2.mean()
-00017720: 2920 2f20 7763 7774 322e 7374 6428 290a  ) / wcwt2.std().
-00017730: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00017740: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00017750: 2020 6e63 7774 3120 3d20 7763 7774 310a    ncwt1 = wcwt1.
-00017760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017770: 6e63 7774 3220 3d20 7763 7774 320a 0a20  ncwt2 = wcwt2.. 
-00017780: 2020 2020 2020 2020 2020 2023 2072 756e             # run
-00017790: 2073 7472 6574 6368 696e 670a 2020 2020   stretching.    
-000177a0: 2020 2020 2020 2020 6476 2c20 6572 726f          dv, erro
-000177b0: 722c 2063 312c 2063 3220 3d20 7374 7265  r, c1, c2 = stre
-000177c0: 7463 6869 6e67 286e 6377 7432 2c20 6e63  tching(ncwt2, nc
-000177d0: 7774 312c 2064 765f 7261 6e67 652c 206e  wt1, dv_range, n
-000177e0: 6274 7269 616c 2c20 7061 7261 290a 2020  btrial, para).  
-000177f0: 2020 2020 2020 2020 2020 6476 765b 6969            dvv[ii
-00017800: 5d2c 2063 635b 6969 5d2c 2063 6470 5b69  ], cc[ii], cdp[i
-00017810: 695d 2c20 6572 725b 6969 5d20 3d20 6476  i], err[ii] = dv
-00017820: 2c20 6331 2c20 6332 2c20 6572 726f 720a  , c1, c2, error.
-00017830: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00017840: 6672 6571 5b66 7265 715f 696e 6469 6e5d  freq[freq_indin]
-00017850: 2c20 6476 762c 2065 7272 0a0a 0a64 6566  , dvv, err...def
-00017860: 2077 7464 7477 5f61 6c6c 6672 6571 280a   wtdtw_allfreq(.
-00017870: 2020 2020 7265 662c 0a20 2020 2063 7572      ref,.    cur
-00017880: 2c0a 2020 2020 616c 6c66 7265 712c 0a20  ,.    allfreq,. 
-00017890: 2020 2070 6172 612c 0a20 2020 206d 6178     para,.    max
-000178a0: 4c61 672c 0a20 2020 2062 2c0a 2020 2020  Lag,.    b,.    
-000178b0: 6469 7265 6374 696f 6e2c 0a20 2020 2064  direction,.    d
-000178c0: 6a3d 3120 2f20 3132 2c0a 2020 2020 7330  j=1 / 12,.    s0
-000178d0: 3d2d 312c 0a20 2020 204a 3d2d 312c 0a20  =-1,.    J=-1,. 
-000178e0: 2020 2077 766e 3d22 6d6f 726c 6574 222c     wvn="morlet",
-000178f0: 0a20 2020 206e 6f72 6d61 6c69 7a65 3d54  .    normalize=T
-00017900: 7275 652c 0a29 3a0a 2020 2020 2222 220a  rue,.):.    """.
-00017910: 2020 2020 4170 706c 7920 6479 6e61 6d69      Apply dynami
-00017920: 6320 7469 6d65 2077 6172 7069 6e67 206d  c time warping m
-00017930: 6574 686f 6420 746f 2063 6f6e 7469 6e75  ethod to continu
-00017940: 6f75 7320 7761 7665 6c65 7420 7472 616e  ous wavelet tran
-00017950: 7366 6f72 6d61 7469 6f6e 2028 4357 5429  sformation (CWT)
-00017960: 206f 6620 7369 676e 616c 730a 2020 2020   of signals.    
-00017970: 666f 7220 616c 6c20 6672 6571 7565 6369  for all frequeci
-00017980: 6573 2069 6e20 616e 2069 6e74 6572 6573  es in an interes
-00017990: 7420 7261 6e67 650a 0a20 2020 2050 6172  t range..    Par
-000179a0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-000179b0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2072  ----------.    r
-000179c0: 6566 3a20 5468 6520 2252 6566 6572 656e  ef: The "Referen
-000179d0: 6365 2220 7469 6d65 7365 7269 6573 2028  ce" timeseries (
-000179e0: 6e75 6d70 792e 6e64 6172 7261 7929 0a20  numpy.ndarray). 
-000179f0: 2020 2063 7572 3a20 5468 6520 2243 7572     cur: The "Cur
-00017a00: 7265 6e74 2220 7469 6d65 7365 7269 6573  rent" timeseries
-00017a10: 2028 6e75 6d70 792e 6e64 6172 7261 7929   (numpy.ndarray)
-00017a20: 0a20 2020 2061 6c6c 6672 6571 3a20 6120  .    allfreq: a 
-00017a30: 626f 6f6c 656e 2076 6172 6961 626c 6520  boolen variable 
-00017a40: 746f 206d 616b 6520 6d65 6173 7572 656d  to make measurem
-00017a50: 656e 7473 206f 6e20 616c 6c20 6672 6571  ents on all freq
-00017a60: 7565 6e63 7920 7261 6e67 6520 6f72 206e  uency range or n
-00017a70: 6f74 0a20 2020 206d 6178 4c61 673a 206d  ot.    maxLag: m
-00017a80: 6178 206e 756d 6265 7220 6f66 2070 6f69  ax number of poi
-00017a90: 6e74 7320 746f 2073 6561 7263 6820 666f  nts to search fo
-00017aa0: 7277 6172 6420 616e 6420 6261 636b 7761  rward and backwa
-00017ab0: 7264 2e0a 2020 2020 623a 2062 2d76 616c  rd..    b: b-val
-00017ac0: 7565 2074 6f20 6c69 6d69 7420 7374 7261  ue to limit stra
-00017ad0: 696e 2c20 7768 6963 6820 6973 2074 6f20  in, which is to 
-00017ae0: 6c69 6d69 7420 7468 6520 6d61 7869 6d75  limit the maximu
-00017af0: 6d20 7665 6c6f 6369 7479 2070 6572 7475  m velocity pertu
-00017b00: 7262 6174 696f 6e2e 0a20 2020 2053 6565  rbation..    See
-00017b10: 2065 7175 6174 696f 6e20 3131 2069 6e20   equation 11 in 
-00017b20: 284d 696b 6573 656c 6c20 6574 2061 6c2e  (Mikesell et al.
-00017b30: 2032 3031 3529 0a20 2020 2064 6972 6563   2015).    direc
-00017b40: 7469 6f6e 3a20 6469 7265 6374 696f 6e20  tion: direction 
-00017b50: 746f 2061 6363 756d 756c 6174 6520 6572  to accumulate er
-00017b60: 726f 7273 2028 313d 666f 7277 6172 642c  rors (1=forward,
-00017b70: 202d 313d 6261 636b 7761 7264 290a 2020   -1=backward).  
-00017b80: 2020 646a 2c20 7330 2c20 4a2c 2073 6967    dj, s0, J, sig
-00017b90: 2c20 7776 6e3a 2063 6f6d 6d6f 6e20 7061  , wvn: common pa
-00017ba0: 7261 6d65 7465 7273 2075 7365 6420 696e  rameters used in
-00017bb0: 2027 7761 7665 6c65 742e 7763 7427 0a20   'wavelet.wct'. 
-00017bc0: 2020 206e 6f72 6d61 6c69 7a65 3a20 6e6f     normalize: no
-00017bd0: 726d 616c 697a 6520 7468 6520 7761 7665  rmalize the wave
-00017be0: 6c65 7420 7370 6563 7472 756d 206f 7220  let spectrum or 
-00017bf0: 6e6f 742e 2044 6566 6175 6c74 2069 7320  not. Default is 
-00017c00: 5472 7565 0a0a 2020 2020 5245 5455 524e  True..    RETURN
-00017c10: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
-00017c20: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 6476  ---------.    dv
-00017c30: 763a 2065 7374 696d 6174 6564 2064 762f  v: estimated dv/
-00017c40: 760a 2020 2020 6572 723a 2065 7272 6f72  v.    err: error
-00017c50: 206f 6620 6476 2f76 2065 7374 696d 6174   of dv/v estimat
-00017c60: 696f 6e0a 0a20 2020 2057 7269 7474 656e  ion..    Written
-00017c70: 2062 7920 436f 6e67 636f 6e67 2059 7561   by Congcong Yua
-00017c80: 6e20 2833 3020 4a75 6e2c 2032 3031 3929  n (30 Jun, 2019)
-00017c90: 0a20 2020 2022 2222 0a20 2020 2023 2063  .    """.    # c
-00017ca0: 6f6d 6d6f 6e20 7661 7269 6162 6c65 730a  ommon variables.
-00017cb0: 2020 2020 6672 6571 203d 2070 6172 615b      freq = para[
-00017cc0: 2266 7265 7122 5d0a 2020 2020 6474 203d  "freq"].    dt =
-00017cd0: 2070 6172 615b 2264 7422 5d0a 2020 2020   para["dt"].    
-00017ce0: 666d 696e 203d 206e 702e 6d69 6e28 6672  fmin = np.min(fr
-00017cf0: 6571 290a 2020 2020 666d 6178 203d 206e  eq).    fmax = n
-00017d00: 702e 6d61 7828 6672 6571 290a 0a20 2020  p.max(freq)..   
-00017d10: 2023 2061 7070 6c79 2063 7774 206f 6e20   # apply cwt on 
-00017d20: 7477 6f20 7472 6163 6573 0a20 2020 2063  two traces.    c
-00017d30: 7774 312c 2073 6a2c 2066 7265 712c 2063  wt1, sj, freq, c
-00017d40: 6f69 2c20 5f2c 205f 203d 2070 7963 7774  oi, _, _ = pycwt
-00017d50: 2e63 7774 2863 7572 2c20 6474 2c20 646a  .cwt(cur, dt, dj
-00017d60: 2c20 7330 2c20 4a2c 2077 766e 290a 2020  , s0, J, wvn).  
-00017d70: 2020 6377 7432 2c20 736a 2c20 6672 6571    cwt2, sj, freq
-00017d80: 2c20 636f 692c 205f 2c20 5f20 3d20 7079  , coi, _, _ = py
-00017d90: 6377 742e 6377 7428 7265 662c 2064 742c  cwt.cwt(ref, dt,
-00017da0: 2064 6a2c 2073 302c 204a 2c20 7776 6e29   dj, s0, J, wvn)
-00017db0: 0a0a 2020 2020 2320 6578 7472 6163 7420  ..    # extract 
-00017dc0: 7265 616c 2076 616c 7565 7320 6f66 2063  real values of c
-00017dd0: 7774 0a20 2020 2072 6377 7431 2c20 7263  wt.    rcwt1, rc
-00017de0: 7774 3220 3d20 6e70 2e72 6561 6c28 6377  wt2 = np.real(cw
-00017df0: 7431 292c 206e 702e 7265 616c 2863 7774  t1), np.real(cwt
-00017e00: 3229 0a0a 2020 2020 2320 7a65 726f 206f  2)..    # zero o
-00017e10: 7574 2063 6f6e 6520 6f66 2069 6e66 6c75  ut cone of influ
-00017e20: 656e 6365 2061 6e64 2064 6174 6120 6f75  ence and data ou
-00017e30: 7473 6964 6520 6672 6571 7565 6e63 7920  tside frequency 
-00017e40: 6261 6e64 0a20 2020 2069 6620 2866 6d61  band.    if (fma
-00017e50: 7820 3e20 6e70 2e6d 6178 2866 7265 7129  x > np.max(freq)
-00017e60: 2920 7c20 2866 6d61 7820 3c3d 2066 6d69  ) | (fmax <= fmi
-00017e70: 6e29 3a0a 2020 2020 2020 2020 7261 6973  n):.        rais
-00017e80: 6520 5661 6c75 6545 7272 6f72 2822 4162  e ValueError("Ab
-00017e90: 6f72 743a 2069 6e70 7574 2066 7265 7175  ort: input frequ
-00017ea0: 656e 6379 206f 7574 206f 6620 6c69 6d69  ency out of limi
-00017eb0: 7473 2122 290a 2020 2020 656c 7365 3a0a  ts!").    else:.
-00017ec0: 2020 2020 2020 2020 6672 6571 5f69 6e64          freq_ind
-00017ed0: 696e 203d 206e 702e 7768 6572 6528 2866  in = np.where((f
-00017ee0: 7265 7120 3e3d 2066 6d69 6e29 2026 2028  req >= fmin) & (
-00017ef0: 6672 6571 203c 3d20 666d 6178 2929 5b30  freq <= fmax))[0
-00017f00: 5d0a 0a20 2020 2020 2020 2023 2055 7365  ]..        # Use
-00017f10: 2044 5457 206d 6574 686f 6420 746f 2065   DTW method to e
-00017f20: 7874 7261 6374 2064 7676 0a20 2020 2020  xtract dvv.     
-00017f30: 2020 206e 6672 6571 203d 206c 656e 2866     nfreq = len(f
-00017f40: 7265 715f 696e 6469 6e29 0a20 2020 2020  req_indin).     
-00017f50: 2020 2064 7676 2c20 6572 7220 3d20 6e70     dvv, err = np
-00017f60: 2e7a 6572 6f73 286e 6672 6571 2c20 6474  .zeros(nfreq, dt
-00017f70: 7970 653d 6e70 2e66 6c6f 6174 3332 292c  ype=np.float32),
-00017f80: 206e 702e 7a65 726f 7328 6e66 7265 712c   np.zeros(nfreq,
-00017f90: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
-00017fa0: 3229 0a0a 2020 2020 2020 2020 666f 7220  2)..        for 
-00017fb0: 6969 2c20 6966 7265 7120 696e 2065 6e75  ii, ifreq in enu
-00017fc0: 6d65 7261 7465 2866 7265 715f 696e 6469  merate(freq_indi
-00017fd0: 6e29 3a0a 2020 2020 2020 2020 2020 2020  n):.            
-00017fe0: 2320 7072 6570 6172 6520 7769 6e64 6f77  # prepare window
-00017ff0: 6564 2064 6174 610a 2020 2020 2020 2020  ed data.        
-00018000: 2020 2020 7763 7774 312c 2077 6377 7432      wcwt1, wcwt2
-00018010: 203d 2072 6377 7431 5b69 6672 6571 5d2c   = rcwt1[ifreq],
-00018020: 2072 6377 7432 5b69 6672 6571 5d0a 2020   rcwt2[ifreq].  
-00018030: 2020 2020 2020 2020 2020 2320 4e6f 726d            # Norm
-00018040: 616c 697a 6573 2062 6f74 6820 7369 676e  alizes both sign
-00018050: 616c 732c 2069 6620 6170 7072 6f70 7269  als, if appropri
-00018060: 6174 652e 0a20 2020 2020 2020 2020 2020  ate..           
-00018070: 2069 6620 6e6f 726d 616c 697a 653a 0a20   if normalize:. 
-00018080: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00018090: 6377 7431 203d 2028 7763 7774 3120 2d20  cwt1 = (wcwt1 - 
-000180a0: 7763 7774 312e 6d65 616e 2829 2920 2f20  wcwt1.mean()) / 
-000180b0: 7763 7774 312e 7374 6428 290a 2020 2020  wcwt1.std().    
-000180c0: 2020 2020 2020 2020 2020 2020 6e63 7774              ncwt
-000180d0: 3220 3d20 2877 6377 7432 202d 2077 6377  2 = (wcwt2 - wcw
-000180e0: 7432 2e6d 6561 6e28 2929 202f 2077 6377  t2.mean()) / wcw
-000180f0: 7432 2e73 7464 2829 0a20 2020 2020 2020  t2.std().       
-00018100: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00018110: 2020 2020 2020 2020 2020 206e 6377 7431             ncwt1
-00018120: 203d 2077 6377 7431 0a20 2020 2020 2020   = wcwt1.       
-00018130: 2020 2020 2020 2020 206e 6377 7432 203d           ncwt2 =
-00018140: 2077 6377 7432 0a0a 2020 2020 2020 2020   wcwt2..        
-00018150: 2020 2020 2320 7275 6e20 6474 770a 2020      # run dtw.  
-00018160: 2020 2020 2020 2020 2020 6476 2c20 6572            dv, er
-00018170: 726f 722c 2064 6973 7420 3d20 6474 775f  ror, dist = dtw_
-00018180: 6476 7628 6e63 7774 322c 206e 6377 7431  dvv(ncwt2, ncwt1
-00018190: 2c20 7061 7261 2c20 6d61 784c 6167 2c20  , para, maxLag, 
-000181a0: 622c 2064 6972 6563 7469 6f6e 290a 2020  b, direction).  
-000181b0: 2020 2020 2020 2020 2020 6476 765b 6969            dvv[ii
-000181c0: 5d2c 2065 7272 5b69 695d 203d 2064 762c  ], err[ii] = dv,
-000181d0: 2065 7272 6f72 0a0a 2020 2020 6465 6c20   error..    del 
-000181e0: 6377 7431 2c20 6377 7432 2c20 7263 7774  cwt1, cwt2, rcwt
-000181f0: 312c 2072 6377 7432 2c20 6e63 7774 312c  1, rcwt2, ncwt1,
-00018200: 206e 6377 7432 2c20 7763 7774 312c 2077   ncwt2, wcwt1, w
-00018210: 6377 7432 2c20 636f 692c 2073 6a2c 2064  cwt2, coi, sj, d
-00018220: 6973 740a 0a20 2020 2069 6620 6e6f 7420  ist..    if not 
-00018230: 616c 6c66 7265 713a 0a20 2020 2020 2020  allfreq:.       
-00018240: 2072 6574 7572 6e20 6e70 2e6d 6561 6e28   return np.mean(
-00018250: 6476 7629 2c20 6e70 2e6d 6561 6e28 6572  dvv), np.mean(er
-00018260: 7229 0a20 2020 2065 6c73 653a 0a20 2020  r).    else:.   
-00018270: 2020 2020 2072 6574 7572 6e20 6672 6571       return freq
-00018280: 5b66 7265 715f 696e 6469 6e5d 2c20 6476  [freq_indin], dv
-00018290: 762c 2065 7272 0a0a 0a23 2323 2323 2323  v, err...#######
+00011090: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000110a0: 2323 0a0a 2222 220a 6120 636f 6d70 696c  ##..""".a compil
+000110b0: 6174 696f 6e20 6f66 2061 6c6c 2061 7661  ation of all ava
+000110c0: 696c 6162 6c65 2063 6f72 6520 6675 6e63  ilable core func
+000110d0: 7469 6f6e 7320 666f 7220 636f 6d70 7574  tions for comput
+000110e0: 696e 6720 7068 6173 6520 6465 6c61 7973  ing phase delays
+000110f0: 2062 6173 6564 206f 6e20 616d 6269 656e   based on ambien
+00011100: 7420 6e6f 6973 6520 696e 7465 7266 6572  t noise interfer
+00011110: 6f6d 6574 7279 0a0a 7175 6963 6b20 696e  ometry..quick in
+00011120: 6465 7820 6f66 2064 762f 7620 6d65 7468  dex of dv/v meth
+00011130: 6f64 733a 0a31 2920 7374 7265 7463 6869  ods:.1) stretchi
+00011140: 6e67 2028 7469 6d65 2073 7472 6574 6368  ng (time stretch
+00011150: 696e 673b 2057 6561 7665 7220 6574 2061  ing; Weaver et a
+00011160: 6c20 2832 3031 3129 290a 3229 2064 7477  l (2011)).2) dtw
+00011170: 5f64 7676 2028 4479 6e61 6d69 6320 5469  _dvv (Dynamic Ti
+00011180: 6d65 2057 6172 7069 6e67 3b20 4d69 6b65  me Warping; Mike
+00011190: 7365 6c6c 2065 7420 616c 2e20 3230 3135  sell et al. 2015
+000111a0: 290a 3329 206d 7763 735f 6476 7620 284d  ).3) mwcs_dvv (M
+000111b0: 6f76 696e 6720 5769 6e64 6f77 2043 726f  oving Window Cro
+000111c0: 7373 2053 7065 6374 7275 6d3b 2043 6c61  ss Spectrum; Cla
+000111d0: 726b 2065 7420 616c 2e2c 2032 3031 3129  rk et al., 2011)
+000111e0: 0a34 2920 6d77 6363 5f64 7676 2028 4d6f  .4) mwcc_dvv (Mo
+000111f0: 7669 6e67 2057 696e 646f 7720 4372 6f73  ving Window Cros
+00011200: 7320 436f 7272 656c 6174 696f 6e3b 2053  s Correlation; S
+00011210: 6e69 6564 6572 2065 7420 616c 2e2c 2032  nieder et al., 2
+00011220: 3031 3229 0a35 2920 7774 735f 6476 7620  012).5) wts_dvv 
+00011230: 2857 6176 656c 6574 2053 7472 6563 6869  (Wavelet Strechi
+00011240: 6e67 3b20 5975 616e 2065 7420 616c 2e2c  ng; Yuan et al.,
+00011250: 2069 6e20 7072 6570 290a 3629 2077 7873   in prep).6) wxs
+00011260: 5f64 7676 2028 5761 7665 6c65 7420 5872  _dvv (Wavelet Xr
+00011270: 6f73 7320 5370 6563 7472 756d 3b20 4d61  oss Spectrum; Ma
+00011280: 6f20 6574 2061 6c2e 2c20 3230 3139 290a  o et al., 2019).
+00011290: 3729 2077 6477 5f64 7676 2028 5761 7665  7) wdw_dvv (Wave
+000112a0: 6c65 7420 4479 6e61 6d69 6320 5761 7270  let Dynamic Warp
+000112b0: 696e 673b 2059 7561 6e20 6574 2061 6c2e  ing; Yuan et al.
+000112c0: 2c20 696e 2070 7265 7029 0a22 2222 0a0a  , in prep)."""..
+000112d0: 0a64 6566 2073 7472 6574 6368 696e 6728  .def stretching(
+000112e0: 7265 662c 2063 7572 2c20 6476 5f72 616e  ref, cur, dv_ran
+000112f0: 6765 2c20 6e62 7472 6961 6c2c 2070 6172  ge, nbtrial, par
+00011300: 6129 3a0a 2020 2020 2222 220a 2020 2020  a):.    """.    
+00011310: 5468 6973 2066 756e 6374 696f 6e20 636f  This function co
+00011320: 6d70 6172 6573 2074 6865 2052 6566 6572  mpares the Refer
+00011330: 656e 6365 2077 6176 6566 6f72 6d20 746f  ence waveform to
+00011340: 2073 7472 6574 6368 6564 2f63 6f6d 7072   stretched/compr
+00011350: 6573 7365 6420 6375 7272 656e 7420 7761  essed current wa
+00011360: 7665 666f 726d 7320 746f 2067 6574 2074  veforms to get t
+00011370: 6865 0a20 2020 2072 656c 6174 6976 6520  he.    relative 
+00011380: 7365 6973 6d69 6320 7665 6c6f 6369 7479  seismic velocity
+00011390: 2076 6172 6961 7469 6f6e 2028 616e 6420   variation (and 
+000113a0: 6173 736f 6369 6174 6564 2065 7272 6f72  associated error
+000113b0: 292e 0a20 2020 2049 7420 616c 736f 2063  )..    It also c
+000113c0: 6f6d 7075 7465 7320 7468 6520 636f 7272  omputes the corr
+000113d0: 656c 6174 696f 6e20 636f 6566 6669 6369  elation coeffici
+000113e0: 656e 7420 6265 7477 6565 6e20 7468 6520  ent between the 
+000113f0: 5265 6665 7265 6e63 6520 7761 7665 666f  Reference wavefo
+00011400: 726d 2061 6e64 2074 6865 2063 7572 7265  rm and the curre
+00011410: 6e74 2077 6176 6566 6f72 6d2e 0a0a 2020  nt waveform...  
+00011420: 2020 5041 5241 4d45 5445 5253 3a0a 2020    PARAMETERS:.  
+00011430: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00011440: 2d2d 0a20 2020 2072 6566 3a20 5265 6665  --.    ref: Refe
+00011450: 7265 6e63 6520 7761 7665 666f 726d 2028  rence waveform (
+00011460: 6e70 2e6e 6461 7272 6179 2c20 7369 7a65  np.ndarray, size
+00011470: 204e 290a 2020 2020 6375 723a 2043 7572   N).    cur: Cur
+00011480: 7265 6e74 2077 6176 6566 6f72 6d20 286e  rent waveform (n
+00011490: 702e 6e64 6172 7261 792c 2073 697a 6520  p.ndarray, size 
+000114a0: 4e29 0a20 2020 2064 765f 7261 6e67 653a  N).    dv_range:
+000114b0: 2061 6273 6f6c 7574 6520 626f 756e 6420   absolute bound 
+000114c0: 666f 7220 7468 6520 7665 6c6f 6369 7479  for the velocity
+000114d0: 2076 6172 6961 7469 6f6e 3b20 6578 616d   variation; exam
+000114e0: 706c 653a 2064 763d 302e 3033 2066 6f72  ple: dv=0.03 for
+000114f0: 205b 2d33 2c33 5d25 0a20 2020 206f 6620   [-3,3]%.    of 
+00011500: 7265 6c61 7469 7665 2076 656c 6f63 6974  relative velocit
+00011510: 7920 6368 616e 6765 2028 2766 6c6f 6174  y change ('float
+00011520: 2729 0a20 2020 206e 6274 7269 616c 3a20  ').    nbtrial: 
+00011530: 6e75 6d62 6572 206f 6620 7374 7265 7463  number of stretc
+00011540: 6869 6e67 2063 6f65 6666 6963 6965 6e74  hing coefficient
+00011550: 2062 6574 7765 656e 2064 766d 696e 2061   between dvmin a
+00011560: 6e64 2064 766d 6178 2c20 6e6f 206e 6565  nd dvmax, no nee
+00011570: 6420 746f 2062 6520 6869 6768 6572 2074  d to be higher t
+00011580: 6861 6e20 3130 3020 2028 2766 6c6f 6174  han 100  ('float
+00011590: 2729 0a20 2020 2070 6172 613a 2076 6563  ').    para: vec
+000115a0: 746f 7220 6f66 2074 6865 2069 6e64 6963  tor of the indic
+000115b0: 6573 206f 6620 7468 6520 6375 7220 616e  es of the cur an
+000115c0: 6420 7265 6620 7769 6e64 6f77 7320 6f6e  d ref windows on
+000115d0: 2077 6963 6820 796f 7520 7761 6e74 2074   wich you want t
+000115e0: 6f20 646f 2074 6865 206d 6561 7375 7265  o do the measure
+000115f0: 6d65 6e74 730a 2020 2020 286e 702e 6e64  ments.    (np.nd
+00011600: 6172 7261 792c 2073 697a 6520 746d 696e  array, size tmin
+00011610: 2a64 656c 7461 3a74 6d61 782a 6465 6c74  *delta:tmax*delt
+00011620: 6129 0a20 2020 2046 6f72 2065 7272 6f72  a).    For error
+00011630: 2063 6f6d 7075 7461 7469 6f6e 2c20 7765   computation, we
+00011640: 206e 6565 6420 7061 7261 6d65 7465 7273   need parameters
+00011650: 3a0a 2020 2020 2020 2020 666d 696e 3a20  :.        fmin: 
+00011660: 6d69 6e69 6d75 6d20 6672 6571 7565 6e63  minimum frequenc
+00011670: 7920 6f66 2074 6865 2064 6174 610a 2020  y of the data.  
+00011680: 2020 2020 2020 666d 6178 3a20 6d61 7869        fmax: maxi
+00011690: 6d75 6d20 6672 6571 7565 6e63 7920 6f66  mum frequency of
+000116a0: 2074 6865 2064 6174 610a 2020 2020 2020   the data.      
+000116b0: 2020 746d 696e 3a20 6d69 6e69 6d75 6d20    tmin: minimum 
+000116c0: 7469 6d65 2077 696e 646f 7720 7768 6572  time window wher
+000116d0: 6520 7468 6520 6476 2f76 2069 7320 636f  e the dv/v is co
+000116e0: 6d70 7574 6564 0a20 2020 2020 2020 2074  mputed.        t
+000116f0: 6d61 783a 206d 6178 696d 756d 2074 696d  max: maximum tim
+00011700: 6520 7769 6e64 6f77 2077 6865 7265 2074  e window where t
+00011710: 6865 2064 762f 7620 6973 2063 6f6d 7075  he dv/v is compu
+00011720: 7465 640a 2020 2020 5245 5455 524e 533a  ted.    RETURNS:
+00011730: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+00011740: 2d2d 2d2d 2d0a 2020 2020 6476 3a20 5265  -----.    dv: Re
+00011750: 6c61 7469 7665 2076 656c 6f63 6974 7920  lative velocity 
+00011760: 6368 616e 6765 2064 762f 7620 2869 6e20  change dv/v (in 
+00011770: 2529 0a20 2020 2063 633a 2063 6f72 7265  %).    cc: corre
+00011780: 6c61 7469 6f6e 2063 6f65 6666 6963 6965  lation coefficie
+00011790: 6e74 2062 6574 7765 656e 2074 6865 2072  nt between the r
+000117a0: 6566 6572 656e 6365 2077 6176 6566 6f72  eference wavefor
+000117b0: 6d20 616e 6420 7468 6520 6265 7374 2073  m and the best s
+000117c0: 7472 6574 6368 6564 2f63 6f6d 7072 6573  tretched/compres
+000117d0: 7365 6420 6375 7272 656e 7420 7761 7665  sed current wave
+000117e0: 666f 726d 0a20 2020 2063 6470 3a20 636f  form.    cdp: co
+000117f0: 7272 656c 6174 696f 6e20 636f 6566 6669  rrelation coeffi
+00011800: 6369 656e 7420 6265 7477 6565 6e20 7468  cient between th
+00011810: 6520 7265 6665 7265 6e63 6520 7761 7665  e reference wave
+00011820: 666f 726d 2061 6e64 2074 6865 2069 6e69  form and the ini
+00011830: 7469 616c 2063 7572 7265 6e74 2077 6176  tial current wav
+00011840: 6566 6f72 6d0a 2020 2020 6572 726f 723a  eform.    error:
+00011850: 2045 7272 6f72 7320 696e 2074 6865 2064   Errors in the d
+00011860: 762f 7620 6d65 6173 7572 656d 656e 7473  v/v measurements
+00011870: 2062 6173 6564 206f 6e20 5765 6176 6572   based on Weaver
+00011880: 2065 7420 616c 2028 3230 3131 292c 0a20   et al (2011),. 
+00011890: 2020 204f 6e20 7468 6520 7072 6563 6973     On the precis
+000118a0: 696f 6e20 6f66 206e 6f69 7365 2d63 6f72  ion of noise-cor
+000118b0: 7265 6c61 7469 6f6e 2069 6e74 6572 6665  relation interfe
+000118c0: 726f 6d65 7472 792c 2047 656f 7068 7973  rometry, Geophys
+000118d0: 2e20 4a2e 2049 6e74 2e2c 2031 3835 2833  . J. Int., 185(3
+000118e0: 290a 0a20 2020 204e 6f74 653a 2054 6865  )..    Note: The
+000118f0: 2063 6f64 6520 6669 7273 7420 6669 6e64   code first find
+00011900: 7320 7468 6520 6265 7374 2063 6f72 7265  s the best corre
+00011910: 6c61 7469 6f6e 2063 6f65 6666 6963 6965  lation coefficie
+00011920: 6e74 2062 6574 7765 656e 2074 6865 2052  nt between the R
+00011930: 6566 6572 656e 6365 2077 6176 6566 6f72  eference wavefor
+00011940: 6d20 616e 640a 2020 2020 7468 6520 7374  m and.    the st
+00011950: 7265 7463 6865 642f 636f 6d70 7265 7373  retched/compress
+00011960: 6564 2063 7572 7265 6e74 2077 6176 6566  ed current wavef
+00011970: 6f72 6d20 616d 6f6e 6720 7468 6520 226e  orm among the "n
+00011980: 6274 7269 616c 2220 7661 6c75 6573 2e0a  btrial" values..
+00011990: 2020 2020 4120 7265 6669 6e65 6420 616e      A refined an
+000119a0: 616c 7973 6973 2069 7320 7468 656e 2070  alysis is then p
+000119b0: 6572 666f 726d 6564 2061 726f 756e 6420  erformed around 
+000119c0: 7468 6973 2076 616c 7565 2074 6f20 6f62  this value to ob
+000119d0: 7461 696e 2061 206d 6f72 6520 7072 6563  tain a more prec
+000119e0: 6973 6520 6476 2f76 206d 6561 7375 7265  ise dv/v measure
+000119f0: 6d65 6e74 202e 0a0a 2020 2020 4f72 6967  ment ...    Orig
+00011a00: 696e 616c 6c79 2062 7920 4c2e 2056 6965  inally by L. Vie
+00011a10: 6e73 2030 342f 3236 2f32 3031 3820 2856  ns 04/26/2018 (V
+00011a20: 6965 6e73 2065 7420 616c 2e2c 2032 3031  iens et al., 201
+00011a30: 3820 4a47 5229 0a20 2020 206d 6f64 6966  8 JGR).    modif
+00011a40: 6965 6420 6279 2043 6865 6e67 7869 6e20  ied by Chengxin 
+00011a50: 4a69 616e 670a 2020 2020 2222 220a 2020  Jiang.    """.  
+00011a60: 2020 2320 6c6f 6164 2063 6f6d 6d6f 6e20    # load common 
+00011a70: 7661 7269 6162 6c65 7320 6672 6f6d 2064  variables from d
+00011a80: 6963 7469 6f6e 6172 790a 2020 2020 7477  ictionary.    tw
+00011a90: 696e 203d 2070 6172 615b 2274 7769 6e22  in = para["twin"
+00011aa0: 5d0a 2020 2020 6672 6571 203d 2070 6172  ].    freq = par
+00011ab0: 615b 2266 7265 7122 5d0a 2020 2020 6474  a["freq"].    dt
+00011ac0: 203d 2070 6172 615b 2264 7422 5d0a 2020   = para["dt"].  
+00011ad0: 2020 746d 696e 203d 206e 702e 6d69 6e28    tmin = np.min(
+00011ae0: 7477 696e 290a 2020 2020 746d 6178 203d  twin).    tmax =
+00011af0: 206e 702e 6d61 7828 7477 696e 290a 2020   np.max(twin).  
+00011b00: 2020 666d 696e 203d 206e 702e 6d69 6e28    fmin = np.min(
+00011b10: 6672 6571 290a 2020 2020 666d 6178 203d  freq).    fmax =
+00011b20: 206e 702e 6d61 7828 6672 6571 290a 2020   np.max(freq).  
+00011b30: 2020 7476 6563 203d 206e 702e 6172 616e    tvec = np.aran
+00011b40: 6765 2874 6d69 6e2c 2074 6d61 782c 2064  ge(tmin, tmax, d
+00011b50: 7429 0a0a 2020 2020 2320 6d61 6b65 2075  t)..    # make u
+00011b60: 7365 6675 6c20 6f6e 6520 666f 7220 6d65  seful one for me
+00011b70: 6173 7572 656d 656e 7473 0a20 2020 2064  asurements.    d
+00011b80: 766d 696e 203d 202d 6e70 2e61 6273 2864  vmin = -np.abs(d
+00011b90: 765f 7261 6e67 6529 0a20 2020 2064 766d  v_range).    dvm
+00011ba0: 6178 203d 206e 702e 6162 7328 6476 5f72  ax = np.abs(dv_r
+00011bb0: 616e 6765 290a 2020 2020 4570 7320 3d20  ange).    Eps = 
+00011bc0: 3120 2b20 286e 702e 6c69 6e73 7061 6365  1 + (np.linspace
+00011bd0: 2864 766d 696e 2c20 6476 6d61 782c 206e  (dvmin, dvmax, n
+00011be0: 6274 7269 616c 2929 0a20 2020 2063 6f66  btrial)).    cof
+00011bf0: 203d 206e 702e 7a65 726f 7328 4570 732e   = np.zeros(Eps.
+00011c00: 7368 6170 652c 2064 7479 7065 3d6e 702e  shape, dtype=np.
+00011c10: 666c 6f61 7433 3229 0a0a 2020 2020 2320  float32)..    # 
+00011c20: 5365 7420 6f66 2073 7472 6574 6368 6564  Set of stretched
+00011c30: 2f63 6f6d 7072 6573 7365 6420 6375 7272  /compressed curr
+00011c40: 656e 7420 7761 7665 666f 726d 730a 2020  ent waveforms.  
+00011c50: 2020 666f 7220 6969 2069 6e20 7261 6e67    for ii in rang
+00011c60: 6528 6c65 6e28 4570 7329 293a 0a20 2020  e(len(Eps)):.   
+00011c70: 2020 2020 206e 7420 3d20 7476 6563 202a       nt = tvec *
+00011c80: 2045 7073 5b69 695d 0a20 2020 2020 2020   Eps[ii].       
+00011c90: 2073 203d 206e 702e 696e 7465 7270 2878   s = np.interp(x
+00011ca0: 3d74 7665 632c 2078 703d 6e74 2c20 6670  =tvec, xp=nt, fp
+00011cb0: 3d63 7572 290a 2020 2020 2020 2020 7761  =cur).        wa
+00011cc0: 7665 666f 726d 5f72 6566 203d 2072 6566  veform_ref = ref
+00011cd0: 0a20 2020 2020 2020 2077 6176 6566 6f72  .        wavefor
+00011ce0: 6d5f 6375 7220 3d20 730a 2020 2020 2020  m_cur = s.      
+00011cf0: 2020 636f 665b 6969 5d20 3d20 6e70 2e63    cof[ii] = np.c
+00011d00: 6f72 7263 6f65 6628 7761 7665 666f 726d  orrcoef(waveform
+00011d10: 5f72 6566 2c20 7761 7665 666f 726d 5f63  _ref, waveform_c
+00011d20: 7572 295b 302c 2031 5d0a 0a20 2020 2063  ur)[0, 1]..    c
+00011d30: 6470 203d 206e 702e 636f 7272 636f 6566  dp = np.corrcoef
+00011d40: 2863 7572 2c20 7265 6629 5b30 2c20 315d  (cur, ref)[0, 1]
+00011d50: 2020 2320 636f 7272 656c 6174 696f 6e20    # correlation 
+00011d60: 636f 6566 6669 6369 656e 7420 6265 7477  coefficient betw
+00011d70: 6565 6e20 7468 6520 7265 6665 7265 6e63  een the referenc
+00011d80: 6520 616e 6420 696e 6974 6961 6c20 6375  e and initial cu
+00011d90: 7272 656e 7420 7761 7665 666f 726d 730a  rrent waveforms.
+00011da0: 0a20 2020 2023 2066 696e 6420 7468 6520  .    # find the 
+00011db0: 6d61 7869 6d75 6d20 636f 7272 656c 6174  maximum correlat
+00011dc0: 696f 6e20 636f 6566 6669 6369 656e 740a  ion coefficient.
+00011dd0: 2020 2020 696d 6178 203d 206e 702e 6e61      imax = np.na
+00011de0: 6e61 7267 6d61 7828 636f 6629 0a20 2020  nargmax(cof).   
+00011df0: 2069 6620 696d 6178 203e 3d20 6c65 6e28   if imax >= len(
+00011e00: 4570 7329 202d 2032 3a0a 2020 2020 2020  Eps) - 2:.      
+00011e10: 2020 696d 6178 203d 2069 6d61 7820 2d20    imax = imax - 
+00011e20: 320a 2020 2020 6966 2069 6d61 7820 3c3d  2.    if imax <=
+00011e30: 2032 3a0a 2020 2020 2020 2020 696d 6178   2:.        imax
+00011e40: 203d 2069 6d61 7820 2b20 320a 0a20 2020   = imax + 2..   
+00011e50: 2023 2050 726f 6365 6564 2074 6f20 7468   # Proceed to th
+00011e60: 6520 7365 636f 6e64 2073 7465 7020 746f  e second step to
+00011e70: 2067 6574 2061 206d 6f72 6520 7072 6563   get a more prec
+00011e80: 6973 6520 6476 2f76 206d 6561 7375 7265  ise dv/v measure
+00011e90: 6d65 6e74 0a20 2020 2064 7466 696e 6572  ment.    dtfiner
+00011ea0: 203d 206e 702e 6c69 6e73 7061 6365 2845   = np.linspace(E
+00011eb0: 7073 5b69 6d61 7820 2d20 325d 2c20 4570  ps[imax - 2], Ep
+00011ec0: 735b 696d 6178 202b 2032 5d2c 2031 3030  s[imax + 2], 100
+00011ed0: 290a 2020 2020 6e63 6f66 203d 206e 702e  ).    ncof = np.
+00011ee0: 7a65 726f 7328 6474 6669 6e65 722e 7368  zeros(dtfiner.sh
+00011ef0: 6170 652c 2064 7479 7065 3d6e 702e 666c  ape, dtype=np.fl
+00011f00: 6f61 7433 3229 0a20 2020 2066 6f72 2069  oat32).    for i
+00011f10: 6920 696e 2072 616e 6765 286c 656e 2864  i in range(len(d
+00011f20: 7466 696e 6572 2929 3a0a 2020 2020 2020  tfiner)):.      
+00011f30: 2020 6e74 203d 2074 7665 6320 2a20 6474    nt = tvec * dt
+00011f40: 6669 6e65 725b 6969 5d0a 2020 2020 2020  finer[ii].      
+00011f50: 2020 7320 3d20 6e70 2e69 6e74 6572 7028    s = np.interp(
+00011f60: 783d 7476 6563 2c20 7870 3d6e 742c 2066  x=tvec, xp=nt, f
+00011f70: 703d 6375 7229 0a20 2020 2020 2020 2077  p=cur).        w
+00011f80: 6176 6566 6f72 6d5f 7265 6620 3d20 7265  aveform_ref = re
+00011f90: 660a 2020 2020 2020 2020 7761 7665 666f  f.        wavefo
+00011fa0: 726d 5f63 7572 203d 2073 0a20 2020 2020  rm_cur = s.     
+00011fb0: 2020 206e 636f 665b 6969 5d20 3d20 6e70     ncof[ii] = np
+00011fc0: 2e63 6f72 7263 6f65 6628 7761 7665 666f  .corrcoef(wavefo
+00011fd0: 726d 5f72 6566 2c20 7761 7665 666f 726d  rm_ref, waveform
+00011fe0: 5f63 7572 295b 302c 2031 5d0a 0a20 2020  _cur)[0, 1]..   
+00011ff0: 2063 6320 3d20 6e70 2e6d 6178 286e 636f   cc = np.max(nco
+00012000: 6629 2020 2320 4669 6e64 206d 6178 696d  f)  # Find maxim
+00012010: 756d 2063 6f72 7265 6c61 7469 6f6e 2063  um correlation c
+00012020: 6f65 6666 6963 6965 6e74 206f 6620 7468  oefficient of th
+00012030: 6520 7265 6669 6e65 6420 2061 6e61 6c79  e refined  analy
+00012040: 7369 730a 2020 2020 6476 203d 2031 3030  sis.    dv = 100
+00012050: 2e30 202a 2064 7466 696e 6572 5b6e 702e  .0 * dtfiner[np.
+00012060: 6172 676d 6178 286e 636f 6629 5d20 2d20  argmax(ncof)] - 
+00012070: 3130 3020 2023 204d 756c 7469 706c 7920  100  # Multiply 
+00012080: 6279 2031 3030 2074 6f20 636f 6e76 6572  by 100 to conver
+00012090: 7420 746f 2070 6572 6365 6e74 6167 6520  t to percentage 
+000120a0: 2845 7073 696c 6f6e 203d 202d 6474 2f74  (Epsilon = -dt/t
+000120b0: 203d 2064 762f 7629 0a0a 2020 2020 2320   = dv/v)..    # 
+000120c0: 4572 726f 7220 636f 6d70 7574 6174 696f  Error computatio
+000120d0: 6e20 6261 7365 6420 6f6e 2057 6561 7665  n based on Weave
+000120e0: 7220 6574 2061 6c20 2832 3031 3129 2c20  r et al (2011), 
+000120f0: 4f6e 2074 6865 2070 7265 6369 7369 6f6e  On the precision
+00012100: 206f 6620 6e6f 6973 652d 636f 7272 656c   of noise-correl
+00012110: 6174 696f 6e0a 2020 2020 2320 696e 7465  ation.    # inte
+00012120: 7266 6572 6f6d 6574 7279 2c20 4765 6f70  rferometry, Geop
+00012130: 6879 732e 204a 2e20 496e 742e 2c20 3138  hys. J. Int., 18
+00012140: 3528 3329 0a20 2020 2054 203d 2031 202f  5(3).    T = 1 /
+00012150: 2028 666d 6178 202d 2066 6d69 6e29 0a20   (fmax - fmin). 
+00012160: 2020 2058 203d 2063 630a 2020 2020 7763     X = cc.    wc
+00012170: 203d 206e 702e 7069 202a 2028 666d 696e   = np.pi * (fmin
+00012180: 202b 2066 6d61 7829 0a20 2020 2074 3120   + fmax).    t1 
+00012190: 3d20 6e70 2e6d 696e 285b 746d 696e 2c20  = np.min([tmin, 
+000121a0: 746d 6178 5d29 0a20 2020 2074 3220 3d20  tmax]).    t2 = 
+000121b0: 6e70 2e6d 6178 285b 746d 696e 2c20 746d  np.max([tmin, tm
+000121c0: 6178 5d29 0a20 2020 2065 7272 6f72 203d  ax]).    error =
+000121d0: 2031 3030 202a 2028 0a20 2020 2020 2020   100 * (.       
+000121e0: 206e 702e 7371 7274 2831 202d 2058 2a2a   np.sqrt(1 - X**
+000121f0: 3229 202f 2028 3220 2a20 5829 202a 206e  2) / (2 * X) * n
+00012200: 702e 7371 7274 2828 3620 2a20 6e70 2e73  p.sqrt((6 * np.s
+00012210: 7172 7428 6e70 2e70 6920 2f20 3229 202a  qrt(np.pi / 2) *
+00012220: 2054 2920 2f20 2877 632a 2a32 202a 2028   T) / (wc**2 * (
+00012230: 7432 2a2a 3320 2d20 7431 2a2a 3329 2929  t2**3 - t1**3)))
+00012240: 0a20 2020 2029 0a0a 2020 2020 7265 7475  .    )..    retu
+00012250: 726e 2064 762c 2065 7272 6f72 2c20 6363  rn dv, error, cc
+00012260: 2c20 6364 700a 0a0a 6465 6620 7374 7265  , cdp...def stre
+00012270: 7463 6869 6e67 5f76 6563 7428 7265 662c  tching_vect(ref,
+00012280: 2063 7572 2c20 6476 5f72 616e 6765 2c20   cur, dv_range, 
+00012290: 6e62 7472 6961 6c2c 2070 6172 6129 3a0a  nbtrial, para):.
+000122a0: 2020 2020 2222 220a 2020 2020 5468 6973      """.    This
+000122b0: 2066 756e 6374 696f 6e20 636f 6d70 6172   function compar
+000122c0: 6573 2074 6865 2052 6566 6572 656e 6365  es the Reference
+000122d0: 2077 6176 6566 6f72 6d20 746f 2073 7472   waveform to str
+000122e0: 6574 6368 6564 2f63 6f6d 7072 6573 7365  etched/compresse
+000122f0: 6420 6375 7272 656e 7420 7761 7665 666f  d current wavefo
+00012300: 726d 730a 2020 2020 746f 2067 6574 2074  rms.    to get t
+00012310: 6865 2072 656c 6174 6976 6520 7365 6973  he relative seis
+00012320: 6d69 6320 7665 6c6f 6369 7479 2076 6172  mic velocity var
+00012330: 6961 7469 6f6e 2028 616e 6420 6173 736f  iation (and asso
+00012340: 6369 6174 6564 2065 7272 6f72 292e 0a20  ciated error).. 
+00012350: 2020 2049 7420 616c 736f 2063 6f6d 7075     It also compu
+00012360: 7465 7320 7468 6520 636f 7272 656c 6174  tes the correlat
+00012370: 696f 6e20 636f 6566 6669 6369 656e 7420  ion coefficient 
+00012380: 6265 7477 6565 6e20 7468 6520 5265 6665  between the Refe
+00012390: 7265 6e63 6520 7761 7665 666f 726d 2061  rence waveform a
+000123a0: 6e64 2074 6865 2063 7572 7265 6e74 2077  nd the current w
+000123b0: 6176 6566 6f72 6d2e 0a0a 2020 2020 5041  aveform...    PA
+000123c0: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
+000123d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+000123e0: 2020 2072 6566 3a20 5265 6665 7265 6e63     ref: Referenc
+000123f0: 6520 7761 7665 666f 726d 2028 6e70 2e6e  e waveform (np.n
+00012400: 6461 7272 6179 2c20 7369 7a65 204e 290a  darray, size N).
+00012410: 2020 2020 6375 723a 2043 7572 7265 6e74      cur: Current
+00012420: 2077 6176 6566 6f72 6d20 286e 702e 6e64   waveform (np.nd
+00012430: 6172 7261 792c 2073 697a 6520 4e29 0a20  array, size N). 
+00012440: 2020 2064 765f 7261 6e67 653a 2061 6273     dv_range: abs
+00012450: 6f6c 7574 6520 626f 756e 6420 666f 7220  olute bound for 
+00012460: 7468 6520 7665 6c6f 6369 7479 2076 6172  the velocity var
+00012470: 6961 7469 6f6e 3b20 6578 616d 706c 653a  iation; example:
+00012480: 2064 763d 302e 3033 2066 6f72 205b 2d33   dv=0.03 for [-3
+00012490: 2c33 5d25 0a20 2020 206f 6620 7265 6c61  ,3]%.    of rela
+000124a0: 7469 7665 2076 656c 6f63 6974 7920 6368  tive velocity ch
+000124b0: 616e 6765 2028 2766 6c6f 6174 2729 0a20  ange ('float'). 
+000124c0: 2020 206e 6274 7269 616c 3a20 6e75 6d62     nbtrial: numb
+000124d0: 6572 206f 6620 7374 7265 7463 6869 6e67  er of stretching
+000124e0: 2063 6f65 6666 6963 6965 6e74 2062 6574   coefficient bet
+000124f0: 7765 656e 2064 766d 696e 2061 6e64 2064  ween dvmin and d
+00012500: 766d 6178 2c20 6e6f 206e 6565 6420 746f  vmax, no need to
+00012510: 2062 6520 6869 6768 6572 2074 6861 6e20   be higher than 
+00012520: 3130 3020 2028 2766 6c6f 6174 2729 0a20  100  ('float'). 
+00012530: 2020 2070 6172 613a 2076 6563 746f 7220     para: vector 
+00012540: 6f66 2074 6865 2069 6e64 6963 6573 206f  of the indices o
+00012550: 6620 7468 6520 6375 7220 616e 6420 7265  f the cur and re
+00012560: 6620 7769 6e64 6f77 7320 6f6e 2077 6963  f windows on wic
+00012570: 6820 796f 7520 7761 6e74 2074 6f20 646f  h you want to do
+00012580: 2074 6865 0a20 2020 206d 6561 7375 7265   the.    measure
+00012590: 6d65 6e74 7320 286e 702e 6e64 6172 7261  ments (np.ndarra
+000125a0: 792c 2073 697a 6520 746d 696e 2a64 656c  y, size tmin*del
+000125b0: 7461 3a74 6d61 782a 6465 6c74 6129 0a20  ta:tmax*delta). 
+000125c0: 2020 2046 6f72 2065 7272 6f72 2063 6f6d     For error com
+000125d0: 7075 7461 7469 6f6e 2c20 7765 206e 6565  putation, we nee
+000125e0: 6420 7061 7261 6d65 7465 7273 3a0a 2020  d parameters:.  
+000125f0: 2020 2020 2020 666d 696e 3a20 6d69 6e69        fmin: mini
+00012600: 6d75 6d20 6672 6571 7565 6e63 7920 6f66  mum frequency of
+00012610: 2074 6865 2064 6174 610a 2020 2020 2020   the data.      
+00012620: 2020 666d 6178 3a20 6d61 7869 6d75 6d20    fmax: maximum 
+00012630: 6672 6571 7565 6e63 7920 6f66 2074 6865  frequency of the
+00012640: 2064 6174 610a 2020 2020 2020 2020 746d   data.        tm
+00012650: 696e 3a20 6d69 6e69 6d75 6d20 7469 6d65  in: minimum time
+00012660: 2077 696e 646f 7720 7768 6572 6520 7468   window where th
+00012670: 6520 6476 2f76 2069 7320 636f 6d70 7574  e dv/v is comput
+00012680: 6564 0a20 2020 2020 2020 2074 6d61 783a  ed.        tmax:
+00012690: 206d 6178 696d 756d 2074 696d 6520 7769   maximum time wi
+000126a0: 6e64 6f77 2077 6865 7265 2074 6865 2064  ndow where the d
+000126b0: 762f 7620 6973 2063 6f6d 7075 7465 640a  v/v is computed.
+000126c0: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
+000126d0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+000126e0: 2d0a 2020 2020 6476 3a20 5265 6c61 7469  -.    dv: Relati
+000126f0: 7665 2076 656c 6f63 6974 7920 6368 616e  ve velocity chan
+00012700: 6765 2064 762f 7620 2869 6e20 2529 0a20  ge dv/v (in %). 
+00012710: 2020 2063 633a 2063 6f72 7265 6c61 7469     cc: correlati
+00012720: 6f6e 2063 6f65 6666 6963 6965 6e74 2062  on coefficient b
+00012730: 6574 7765 656e 2074 6865 2072 6566 6572  etween the refer
+00012740: 656e 6365 2077 6176 6566 6f72 6d20 616e  ence waveform an
+00012750: 6420 7468 6520 6265 7374 2073 7472 6574  d the best stret
+00012760: 6368 6564 2f63 6f6d 7072 6573 7365 6420  ched/compressed 
+00012770: 6375 7272 656e 7420 7761 7665 666f 726d  current waveform
+00012780: 0a20 2020 2063 6470 3a20 636f 7272 656c  .    cdp: correl
+00012790: 6174 696f 6e20 636f 6566 6669 6369 656e  ation coefficien
+000127a0: 7420 6265 7477 6565 6e20 7468 6520 7265  t between the re
+000127b0: 6665 7265 6e63 6520 7761 7665 666f 726d  ference waveform
+000127c0: 2061 6e64 2074 6865 2069 6e69 7469 616c   and the initial
+000127d0: 2063 7572 7265 6e74 2077 6176 6566 6f72   current wavefor
+000127e0: 6d0a 2020 2020 6572 726f 723a 2045 7272  m.    error: Err
+000127f0: 6f72 7320 696e 2074 6865 2064 762f 7620  ors in the dv/v 
+00012800: 6d65 6173 7572 656d 656e 7473 2062 6173  measurements bas
+00012810: 6564 206f 6e20 5765 6176 6572 2065 7420  ed on Weaver et 
+00012820: 616c 2028 3230 3131 292c 204f 6e20 7468  al (2011), On th
+00012830: 6520 7072 6563 6973 696f 6e0a 2020 2020  e precision.    
+00012840: 6f66 206e 6f69 7365 2d63 6f72 7265 6c61  of noise-correla
+00012850: 7469 6f6e 2069 6e74 6572 6665 726f 6d65  tion interferome
+00012860: 7472 792c 2047 656f 7068 7973 2e20 4a2e  try, Geophys. J.
+00012870: 2049 6e74 2e2c 2031 3835 2833 290a 0a20   Int., 185(3).. 
+00012880: 2020 204e 6f74 653a 2054 6865 2063 6f64     Note: The cod
+00012890: 6520 6669 7273 7420 6669 6e64 7320 7468  e first finds th
+000128a0: 6520 6265 7374 2063 6f72 7265 6c61 7469  e best correlati
+000128b0: 6f6e 2063 6f65 6666 6963 6965 6e74 2062  on coefficient b
+000128c0: 6574 7765 656e 2074 6865 2052 6566 6572  etween the Refer
+000128d0: 656e 6365 2077 6176 6566 6f72 6d20 616e  ence waveform an
+000128e0: 640a 2020 2020 7468 6520 7374 7265 7463  d.    the stretc
+000128f0: 6865 642f 636f 6d70 7265 7373 6564 2063  hed/compressed c
+00012900: 7572 7265 6e74 2077 6176 6566 6f72 6d20  urrent waveform 
+00012910: 616d 6f6e 6720 7468 6520 226e 6274 7269  among the "nbtri
+00012920: 616c 2220 7661 6c75 6573 2e0a 2020 2020  al" values..    
+00012930: 4120 7265 6669 6e65 6420 616e 616c 7973  A refined analys
+00012940: 6973 2069 7320 7468 656e 2070 6572 666f  is is then perfo
+00012950: 726d 6564 2061 726f 756e 6420 7468 6973  rmed around this
+00012960: 2076 616c 7565 2074 6f20 6f62 7461 696e   value to obtain
+00012970: 2061 206d 6f72 6520 7072 6563 6973 6520   a more precise 
+00012980: 6476 2f76 206d 6561 7375 7265 6d65 6e74  dv/v measurement
+00012990: 202e 0a0a 2020 2020 4f72 6967 696e 616c   ...    Original
+000129a0: 6c79 2062 7920 4c2e 2056 6965 6e73 2030  ly by L. Viens 0
+000129b0: 342f 3236 2f32 3031 3820 2856 6965 6e73  4/26/2018 (Viens
+000129c0: 2065 7420 616c 2e2c 2032 3031 3820 4a47   et al., 2018 JG
+000129d0: 5229 0a20 2020 206d 6f64 6966 6965 6420  R).    modified 
+000129e0: 6279 2043 6865 6e67 7869 6e20 4a69 616e  by Chengxin Jian
+000129f0: 670a 2020 2020 6d6f 6469 6669 6564 2062  g.    modified b
+00012a00: 7920 4c61 7572 6120 4572 6d65 7274 3a20  y Laura Ermert: 
+00012a10: 7665 6374 6f72 697a 6564 2076 6572 7369  vectorized versi
+00012a20: 6f6e 0a20 2020 2022 2222 0a20 2020 2023  on.    """.    #
+00012a30: 206c 6f61 6420 636f 6d6d 6f6e 2076 6172   load common var
+00012a40: 6961 626c 6573 2066 726f 6d20 6469 6374  iables from dict
+00012a50: 696f 6e61 7279 0a20 2020 2074 7769 6e20  ionary.    twin 
+00012a60: 3d20 7061 7261 5b22 7477 696e 225d 0a20  = para["twin"]. 
+00012a70: 2020 2066 7265 7120 3d20 7061 7261 5b22     freq = para["
+00012a80: 6672 6571 225d 0a20 2020 2064 7420 3d20  freq"].    dt = 
+00012a90: 7061 7261 5b22 6474 225d 0a20 2020 2074  para["dt"].    t
+00012aa0: 6d69 6e20 3d20 6e70 2e6d 696e 2874 7769  min = np.min(twi
+00012ab0: 6e29 0a20 2020 2074 6d61 7820 3d20 6e70  n).    tmax = np
+00012ac0: 2e6d 6178 2874 7769 6e29 0a20 2020 2066  .max(twin).    f
+00012ad0: 6d69 6e20 3d20 6e70 2e6d 696e 2866 7265  min = np.min(fre
+00012ae0: 7129 0a20 2020 2066 6d61 7820 3d20 6e70  q).    fmax = np
+00012af0: 2e6d 6178 2866 7265 7129 0a20 2020 2074  .max(freq).    t
+00012b00: 7665 6320 3d20 6e70 2e61 7261 6e67 6528  vec = np.arange(
+00012b10: 746d 696e 2c20 746d 6178 2c20 6474 290a  tmin, tmax, dt).
+00012b20: 0a20 2020 2023 206d 616b 6520 7573 6566  .    # make usef
+00012b30: 756c 206f 6e65 2066 6f72 206d 6561 7375  ul one for measu
+00012b40: 7265 6d65 6e74 730a 2020 2020 6476 6d69  rements.    dvmi
+00012b50: 6e20 3d20 2d6e 702e 6162 7328 6476 5f72  n = -np.abs(dv_r
+00012b60: 616e 6765 290a 2020 2020 6476 6d61 7820  ange).    dvmax 
+00012b70: 3d20 6e70 2e61 6273 2864 765f 7261 6e67  = np.abs(dv_rang
+00012b80: 6529 0a20 2020 2045 7073 203d 2031 202b  e).    Eps = 1 +
+00012b90: 2028 6e70 2e6c 696e 7370 6163 6528 6476   (np.linspace(dv
+00012ba0: 6d69 6e2c 2064 766d 6178 2c20 6e62 7472  min, dvmax, nbtr
+00012bb0: 6961 6c29 290a 2020 2020 6364 7020 3d20  ial)).    cdp = 
+00012bc0: 6e70 2e63 6f72 7263 6f65 6628 6375 722c  np.corrcoef(cur,
+00012bd0: 2072 6566 295b 302c 2031 5d20 2023 2063   ref)[0, 1]  # c
+00012be0: 6f72 7265 6c61 7469 6f6e 2063 6f65 6666  orrelation coeff
+00012bf0: 6963 6965 6e74 2062 6574 7765 656e 2074  icient between t
+00012c00: 6865 2072 6566 6572 656e 6365 2061 6e64  he reference and
+00012c10: 2069 6e69 7469 616c 2063 7572 7265 6e74   initial current
+00012c20: 2077 6176 6566 6f72 6d73 0a20 2020 2077   waveforms.    w
+00012c30: 6176 6566 6f72 6d73 203d 206e 702e 7a65  aveforms = np.ze
+00012c40: 726f 7328 286e 6274 7269 616c 202b 2031  ros((nbtrial + 1
+00012c50: 2c20 6c65 6e28 7265 6629 2929 0a20 2020  , len(ref))).   
+00012c60: 2077 6176 6566 6f72 6d73 5b30 2c20 3a5d   waveforms[0, :]
+00012c70: 203d 2072 6566 0a0a 2020 2020 2320 5365   = ref..    # Se
+00012c80: 7420 6f66 2073 7472 6574 6368 6564 2f63  t of stretched/c
+00012c90: 6f6d 7072 6573 7365 6420 6375 7272 656e  ompressed curren
+00012ca0: 7420 7761 7665 666f 726d 730a 2020 2020  t waveforms.    
+00012cb0: 666f 7220 6969 2069 6e20 7261 6e67 6528  for ii in range(
+00012cc0: 6e62 7472 6961 6c29 3a0a 2020 2020 2020  nbtrial):.      
+00012cd0: 2020 6e74 203d 2074 7665 6320 2a20 4570    nt = tvec * Ep
+00012ce0: 735b 6969 5d0a 2020 2020 2020 2020 7320  s[ii].        s 
+00012cf0: 3d20 6e70 2e69 6e74 6572 7028 783d 7476  = np.interp(x=tv
+00012d00: 6563 2c20 7870 3d6e 742c 2066 703d 6375  ec, xp=nt, fp=cu
+00012d10: 7229 0a20 2020 2020 2020 2077 6176 6566  r).        wavef
+00012d20: 6f72 6d73 5b69 6920 2b20 312c 203a 5d20  orms[ii + 1, :] 
+00012d30: 3d20 730a 2020 2020 636f 6620 3d20 6e70  = s.    cof = np
+00012d40: 2e63 6f72 7263 6f65 6628 7761 7665 666f  .corrcoef(wavefo
+00012d50: 726d 7329 5b30 5d5b 313a 5d0a 0a20 2020  rms)[0][1:]..   
+00012d60: 2023 2066 696e 6420 7468 6520 6d61 7869   # find the maxi
+00012d70: 6d75 6d20 636f 7272 656c 6174 696f 6e20  mum correlation 
+00012d80: 636f 6566 6669 6369 656e 740a 2020 2020  coefficient.    
+00012d90: 696d 6178 203d 206e 702e 6e61 6e61 7267  imax = np.nanarg
+00012da0: 6d61 7828 636f 6629 0a20 2020 2069 6620  max(cof).    if 
+00012db0: 696d 6178 203e 3d20 6c65 6e28 4570 7329  imax >= len(Eps)
+00012dc0: 202d 2032 3a0a 2020 2020 2020 2020 696d   - 2:.        im
+00012dd0: 6178 203d 2069 6d61 7820 2d20 320a 2020  ax = imax - 2.  
+00012de0: 2020 6966 2069 6d61 7820 3c20 323a 0a20    if imax < 2:. 
+00012df0: 2020 2020 2020 2069 6d61 7820 3d20 696d         imax = im
+00012e00: 6178 202b 2032 0a0a 2020 2020 2320 5072  ax + 2..    # Pr
+00012e10: 6f63 6565 6420 746f 2074 6865 2073 6563  oceed to the sec
+00012e20: 6f6e 6420 7374 6570 2074 6f20 6765 7420  ond step to get 
+00012e30: 6120 6d6f 7265 2070 7265 6369 7365 2064  a more precise d
+00012e40: 762f 7620 6d65 6173 7572 656d 656e 740a  v/v measurement.
+00012e50: 2020 2020 6474 6669 6e65 7220 3d20 6e70      dtfiner = np
+00012e60: 2e6c 696e 7370 6163 6528 4570 735b 696d  .linspace(Eps[im
+00012e70: 6178 202d 2032 5d2c 2045 7073 5b69 6d61  ax - 2], Eps[ima
+00012e80: 7820 2b20 325d 2c20 6e62 7472 6961 6c29  x + 2], nbtrial)
+00012e90: 0a20 2020 2023 206e 636f 6620 2020 203d  .    # ncof    =
+00012ea0: 206e 702e 7a65 726f 7328 6474 6669 6e65   np.zeros(dtfine
+00012eb0: 722e 7368 6170 652c 6474 7970 653d 6e70  r.shape,dtype=np
+00012ec0: 2e66 6c6f 6174 3332 290a 2020 2020 7761  .float32).    wa
+00012ed0: 7665 666f 726d 7320 3d20 6e70 2e7a 6572  veforms = np.zer
+00012ee0: 6f73 2828 6e62 7472 6961 6c20 2b20 312c  os((nbtrial + 1,
+00012ef0: 206c 656e 2872 6566 2929 290a 2020 2020   len(ref))).    
+00012f00: 7761 7665 666f 726d 735b 302c 203a 5d20  waveforms[0, :] 
+00012f10: 3d20 7265 660a 2020 2020 666f 7220 6969  = ref.    for ii
+00012f20: 2069 6e20 7261 6e67 6528 6c65 6e28 6474   in range(len(dt
+00012f30: 6669 6e65 7229 293a 0a20 2020 2020 2020  finer)):.       
+00012f40: 206e 7420 3d20 7476 6563 202a 2064 7466   nt = tvec * dtf
+00012f50: 696e 6572 5b69 695d 0a20 2020 2020 2020  iner[ii].       
+00012f60: 2073 203d 206e 702e 696e 7465 7270 2878   s = np.interp(x
+00012f70: 3d74 7665 632c 2078 703d 6e74 2c20 6670  =tvec, xp=nt, fp
+00012f80: 3d63 7572 290a 2020 2020 2020 2020 7761  =cur).        wa
+00012f90: 7665 666f 726d 735b 6969 202b 2031 2c20  veforms[ii + 1, 
+00012fa0: 3a5d 203d 2073 0a20 2020 206e 636f 6620  :] = s.    ncof 
+00012fb0: 3d20 6e70 2e63 6f72 7263 6f65 6628 7761  = np.corrcoef(wa
+00012fc0: 7665 666f 726d 7329 5b30 5d5b 313a 5d0a  veforms)[0][1:].
+00012fd0: 2020 2020 6363 203d 206e 702e 6d61 7828      cc = np.max(
+00012fe0: 6e63 6f66 2920 2023 2046 696e 6420 6d61  ncof)  # Find ma
+00012ff0: 7869 6d75 6d20 636f 7272 656c 6174 696f  ximum correlatio
+00013000: 6e20 636f 6566 6669 6369 656e 7420 6f66  n coefficient of
+00013010: 2074 6865 2072 6566 696e 6564 2020 616e   the refined  an
+00013020: 616c 7973 6973 0a20 2020 2064 7620 3d20  alysis.    dv = 
+00013030: 3130 302e 3020 2a20 6474 6669 6e65 725b  100.0 * dtfiner[
+00013040: 6e70 2e61 7267 6d61 7828 6e63 6f66 295d  np.argmax(ncof)]
+00013050: 202d 2031 3030 2020 2320 4d75 6c74 6970   - 100  # Multip
+00013060: 6c79 2062 7920 3130 3020 746f 2063 6f6e  ly by 100 to con
+00013070: 7665 7274 2074 6f20 7065 7263 656e 7461  vert to percenta
+00013080: 6765 2028 4570 7369 6c6f 6e20 3d20 2d64  ge (Epsilon = -d
+00013090: 742f 7420 3d20 6476 2f76 290a 0a20 2020  t/t = dv/v)..   
+000130a0: 2023 2045 7272 6f72 2063 6f6d 7075 7461   # Error computa
+000130b0: 7469 6f6e 2062 6173 6564 206f 6e20 5765  tion based on We
+000130c0: 6176 6572 2065 7420 616c 2028 3230 3131  aver et al (2011
+000130d0: 292c 204f 6e20 7468 6520 7072 6563 6973  ), On the precis
+000130e0: 696f 6e20 6f66 206e 6f69 7365 2d63 6f72  ion of noise-cor
+000130f0: 7265 6c61 7469 6f6e 2069 6e74 6572 6665  relation interfe
+00013100: 726f 6d65 7472 792c 0a20 2020 2023 2047  rometry,.    # G
+00013110: 656f 7068 7973 2e20 4a2e 2049 6e74 2e2c  eophys. J. Int.,
+00013120: 2031 3835 2833 290a 2020 2020 5420 3d20   185(3).    T = 
+00013130: 3120 2f20 2866 6d61 7820 2d20 666d 696e  1 / (fmax - fmin
+00013140: 290a 2020 2020 5820 3d20 6363 0a20 2020  ).    X = cc.   
+00013150: 2077 6320 3d20 6e70 2e70 6920 2a20 2866   wc = np.pi * (f
+00013160: 6d69 6e20 2b20 666d 6178 290a 2020 2020  min + fmax).    
+00013170: 7431 203d 206e 702e 6d69 6e28 5b74 6d69  t1 = np.min([tmi
+00013180: 6e2c 2074 6d61 785d 290a 2020 2020 7432  n, tmax]).    t2
+00013190: 203d 206e 702e 6d61 7828 5b74 6d69 6e2c   = np.max([tmin,
+000131a0: 2074 6d61 785d 290a 2020 2020 6572 726f   tmax]).    erro
+000131b0: 7220 3d20 3130 3020 2a20 280a 2020 2020  r = 100 * (.    
+000131c0: 2020 2020 6e70 2e73 7172 7428 3120 2d20      np.sqrt(1 - 
+000131d0: 582a 2a32 2920 2f20 2832 202a 2058 2920  X**2) / (2 * X) 
+000131e0: 2a20 6e70 2e73 7172 7428 2836 202a 206e  * np.sqrt((6 * n
+000131f0: 702e 7371 7274 286e 702e 7069 202f 2032  p.sqrt(np.pi / 2
+00013200: 2920 2a20 5429 202f 2028 7763 2a2a 3220  ) * T) / (wc**2 
+00013210: 2a20 2874 322a 2a33 202d 2074 312a 2a33  * (t2**3 - t1**3
+00013220: 2929 290a 2020 2020 290a 0a20 2020 2072  ))).    )..    r
+00013230: 6574 7572 6e20 6476 2c20 6572 726f 722c  eturn dv, error,
+00013240: 2063 632c 2063 6470 0a0a 0a64 6566 2064   cc, cdp...def d
+00013250: 7477 5f64 7676 2872 6566 2c20 6375 722c  tw_dvv(ref, cur,
+00013260: 2070 6172 612c 206d 6178 4c61 672c 2062   para, maxLag, b
+00013270: 2c20 6469 7265 6374 696f 6e29 3a0a 2020  , direction):.  
+00013280: 2020 2222 220a 2020 2020 4479 6e61 6d69    """.    Dynami
+00013290: 6320 7469 6d65 2077 6172 7069 6e67 2066  c time warping f
+000132a0: 6f72 2064 762f 7620 6573 7469 6d61 7469  or dv/v estimati
+000132b0: 6f6e 2e0a 0a20 2020 2050 4152 414d 4554  on...    PARAMET
+000132c0: 4552 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ERS:.    -------
+000132d0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7265  ---------.    re
+000132e0: 6620 3a20 7265 6665 7265 6e63 6520 7369  f : reference si
+000132f0: 676e 616c 2028 6e70 2e61 7272 6179 2c20  gnal (np.array, 
+00013300: 7369 7a65 204e 290a 2020 2020 6375 7220  size N).    cur 
+00013310: 3a20 6375 7272 656e 7420 7369 676e 616c  : current signal
+00013320: 2028 6e70 2e61 7272 6179 2c20 7369 7a65   (np.array, size
+00013330: 204e 290a 2020 2020 7061 7261 3a20 6469   N).    para: di
+00013340: 6374 2063 6f6e 7461 696e 696e 6720 7573  ct containing us
+00013350: 6566 756c 2070 6172 616d 6574 6572 7320  eful parameters 
+00013360: 6162 6f75 7420 7468 6520 6461 7461 2077  about the data w
+00013370: 696e 646f 7720 616e 6420 7461 7267 6574  indow and target
+00013380: 6564 2066 7265 7175 656e 6379 0a20 2020  ed frequency.   
+00013390: 206d 6178 4c61 6720 3a20 6d61 7820 6e75   maxLag : max nu
+000133a0: 6d62 6572 206f 6620 706f 696e 7473 2074  mber of points t
+000133b0: 6f20 7365 6172 6368 2066 6f72 7761 7264  o search forward
+000133c0: 2061 6e64 2062 6163 6b77 6172 642e 0a20   and backward.. 
+000133d0: 2020 2020 2020 2020 2020 2053 7567 6765             Sugge
+000133e0: 7374 2073 6574 7469 6e67 2069 7420 6c61  st setting it la
+000133f0: 7267 6572 2069 6620 7769 6e64 6f77 2069  rger if window i
+00013400: 7320 7365 7420 6c61 7267 6572 2e0a 2020  s set larger..  
+00013410: 2020 6220 3a20 622d 7661 6c75 6520 746f    b : b-value to
+00013420: 206c 696d 6974 2073 7472 6169 6e2c 2077   limit strain, w
+00013430: 6869 6368 2069 7320 746f 206c 696d 6974  hich is to limit
+00013440: 2074 6865 206d 6178 696d 756d 2076 656c   the maximum vel
+00013450: 6f63 6974 7920 7065 7274 7572 6261 7469  ocity perturbati
+00013460: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+00013470: 5365 6520 6571 7561 7469 6f6e 2031 3120  See equation 11 
+00013480: 696e 2028 4d69 6b65 7365 6c6c 2065 7420  in (Mikesell et 
+00013490: 616c 2e20 3230 3135 290a 2020 2020 6469  al. 2015).    di
+000134a0: 7265 6374 696f 6e3a 2064 6972 6563 7469  rection: directi
+000134b0: 6f6e 2074 6f20 6163 6375 6d75 6c61 7465  on to accumulate
+000134c0: 2065 7272 6f72 7320 2831 3d66 6f72 7761   errors (1=forwa
+000134d0: 7264 2c20 2d31 3d62 6163 6b77 6172 6429  rd, -1=backward)
+000134e0: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
+000134f0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00013500: 2d2d 2d2d 0a20 2020 202d 6d30 203a 2065  ----.    -m0 : e
+00013510: 7374 696d 6174 6564 2064 762f 760a 2020  stimated dv/v.  
+00013520: 2020 656d 3020 3a20 6572 726f 7220 6f66    em0 : error of
+00013530: 2064 762f 7620 6573 7469 6d61 7469 6f6e   dv/v estimation
+00013540: 0a0a 2020 2020 4f72 6967 696e 616c 2062  ..    Original b
+00013550: 7920 4469 2059 616e 670a 2020 2020 4c61  y Di Yang.    La
+00013560: 7374 206d 6f64 6966 6965 6420 6279 2044  st modified by D
+00013570: 796c 616e 204d 696b 6573 656c 6c20 2832  ylan Mikesell (2
+00013580: 3520 4665 622e 2032 3031 3529 0a20 2020  5 Feb. 2015).   
+00013590: 2054 7261 6e73 6c61 7465 6420 746f 2070   Translated to p
+000135a0: 7974 686f 6e20 6279 2054 696d 2043 6c65  ython by Tim Cle
+000135b0: 6d65 6e74 7320 2831 3720 4175 672e 2032  ments (17 Aug. 2
+000135c0: 3031 3829 0a20 2020 2022 2222 0a20 2020  018).    """.   
+000135d0: 2074 7769 6e20 3d20 7061 7261 5b22 7477   twin = para["tw
+000135e0: 696e 225d 0a20 2020 2064 7420 3d20 7061  in"].    dt = pa
+000135f0: 7261 5b22 6474 225d 0a20 2020 2074 6d69  ra["dt"].    tmi
+00013600: 6e20 3d20 6e70 2e6d 696e 2874 7769 6e29  n = np.min(twin)
+00013610: 0a20 2020 2074 6d61 7820 3d20 6e70 2e6d  .    tmax = np.m
+00013620: 6178 2874 7769 6e29 0a20 2020 2074 7665  ax(twin).    tve
+00013630: 6374 203d 206e 702e 6172 616e 6765 2874  ct = np.arange(t
+00013640: 6d69 6e2c 2074 6d61 782c 2064 7429 0a0a  min, tmax, dt)..
+00013650: 2020 2020 2320 7365 7475 7020 6f74 6865      # setup othe
+00013660: 7220 7061 7261 6d65 7465 7273 0a20 2020  r parameters.   
+00013670: 206e 7074 7320 3d20 6c65 6e28 7265 6629   npts = len(ref)
+00013680: 2020 2320 6e75 6d62 6572 206f 6620 7469    # number of ti
+00013690: 6d65 2073 616d 706c 6573 0a0a 2020 2020  me samples..    
+000136a0: 2320 636f 6d70 7574 6520 6572 726f 7220  # compute error 
+000136b0: 6675 6e63 7469 6f6e 206f 7665 7220 6c61  function over la
+000136c0: 6773 2c20 7768 6963 6820 6973 2069 6e64  gs, which is ind
+000136d0: 6570 656e 6465 6e74 206f 6620 7374 7261  ependent of stra
+000136e0: 696e 206c 696d 6974 2027 6227 2e0a 2020  in limit 'b'..  
+000136f0: 2020 6572 7220 3d20 636f 6d70 7574 6545    err = computeE
+00013700: 7272 6f72 4675 6e63 7469 6f6e 2863 7572  rrorFunction(cur
+00013710: 2c20 7265 662c 206e 7074 732c 206d 6178  , ref, npts, max
+00013720: 4c61 6729 0a0a 2020 2020 2320 6469 7265  Lag)..    # dire
+00013730: 6374 696f 6e20 746f 2061 6363 756d 756c  ction to accumul
+00013740: 6174 6520 6572 726f 7273 2028 313d 666f  ate errors (1=fo
+00013750: 7277 6172 642c 202d 313d 6261 636b 7761  rward, -1=backwa
+00013760: 7264 290a 2020 2020 6469 7374 203d 2061  rd).    dist = a
+00013770: 6363 756d 756c 6174 6545 7272 6f72 4675  ccumulateErrorFu
+00013780: 6e63 7469 6f6e 2864 6972 6563 7469 6f6e  nction(direction
+00013790: 2c20 6572 722c 206e 7074 732c 206d 6178  , err, npts, max
+000137a0: 4c61 672c 2062 290a 2020 2020 7374 6261  Lag, b).    stba
+000137b0: 7220 3d20 6261 636b 7472 6163 6b44 6973  r = backtrackDis
+000137c0: 7461 6e63 6546 756e 6374 696f 6e28 2d31  tanceFunction(-1
+000137d0: 202a 2064 6972 6563 7469 6f6e 2c20 6469   * direction, di
+000137e0: 7374 2c20 6572 722c 202d 6d61 784c 6167  st, err, -maxLag
+000137f0: 2c20 6229 0a20 2020 2073 7462 6172 5469  , b).    stbarTi
+00013800: 6d65 203d 2073 7462 6172 202a 2064 7420  me = stbar * dt 
+00013810: 2023 2063 6f6e 7665 7274 2066 726f 6d20   # convert from 
+00013820: 7361 6d70 6c65 7320 746f 2074 696d 650a  samples to time.
+00013830: 0a20 2020 2023 2063 7574 2074 6865 2066  .    # cut the f
+00013840: 6972 7374 2061 6e64 206c 6173 7420 3525  irst and last 5%
+00013850: 2066 6f72 2062 6574 7465 7220 7265 6772   for better regr
+00013860: 6573 7369 6f6e 0a20 2020 2069 6e64 7820  ession.    indx 
+00013870: 3d20 6e70 2e77 6865 7265 2828 7476 6563  = np.where((tvec
+00013880: 7420 3e3d 2030 2e30 3520 2a20 6e70 7473  t >= 0.05 * npts
+00013890: 202a 2064 7429 2026 2028 7476 6563 7420   * dt) & (tvect 
+000138a0: 3c3d 2030 2e39 3520 2a20 6e70 7473 202a  <= 0.95 * npts *
+000138b0: 2064 7429 295b 305d 0a0a 2020 2020 2320   dt))[0]..    # 
+000138c0: 6c69 6e65 6172 2072 6567 7265 7373 696f  linear regressio
+000138d0: 6e20 746f 2067 6574 2064 762f 760a 2020  n to get dv/v.  
+000138e0: 2020 6966 206e 7074 7320 3e20 323a 0a20    if npts > 2:. 
+000138f0: 2020 2020 2020 2023 2077 6569 6768 7473         # weights
+00013900: 0a20 2020 2020 2020 2077 203d 206e 702e  .        w = np.
+00013910: 6f6e 6573 286e 7074 7329 0a20 2020 2020  ones(npts).     
+00013920: 2020 2023 206d 2c20 612c 2065 6d2c 2065     # m, a, em, e
+00013930: 6120 3d20 6c69 6e65 6172 5f72 6567 7265  a = linear_regre
+00013940: 7373 696f 6e28 7469 6d65 5f61 7869 735b  ssion(time_axis[
+00013950: 696e 6478 5d2c 2064 656c 7461 5f74 5b69  indx], delta_t[i
+00013960: 6e64 785d 2c20 772c 2069 6e74 6572 6365  ndx], w, interce
+00013970: 7074 5f6f 7269 6769 6e3d 4661 6c73 6529  pt_origin=False)
+00013980: 0a20 2020 2020 2020 206d 302c 2065 6d30  .        m0, em0
+00013990: 203d 206c 696e 6561 725f 7265 6772 6573   = linear_regres
+000139a0: 7369 6f6e 280a 2020 2020 2020 2020 2020  sion(.          
+000139b0: 2020 7476 6563 742e 666c 6174 7465 6e28    tvect.flatten(
+000139c0: 295b 696e 6478 5d2c 0a20 2020 2020 2020  )[indx],.       
+000139d0: 2020 2020 2073 7462 6172 5469 6d65 2e66       stbarTime.f
+000139e0: 6c61 7474 656e 2829 5b69 6e64 785d 2c0a  latten()[indx],.
+000139f0: 2020 2020 2020 2020 2020 2020 772e 666c              w.fl
+00013a00: 6174 7465 6e28 295b 696e 6478 5d2c 0a20  atten()[indx],. 
+00013a10: 2020 2020 2020 2020 2020 2069 6e74 6572             inter
+00013a20: 6365 7074 5f6f 7269 6769 6e3d 5472 7565  cept_origin=True
+00013a30: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00013a40: 2065 6c73 653a 0a20 2020 2020 2020 2070   else:.        p
+00013a50: 7269 6e74 2822 6e6f 7420 656e 6f75 6768  rint("not enough
+00013a60: 2070 6f69 6e74 7320 746f 2065 7374 696d   points to estim
+00013a70: 6174 6520 6476 2f76 2066 6f72 2064 7477  ate dv/v for dtw
+00013a80: 2229 0a20 2020 2020 2020 206d 3020 3d20  ").        m0 = 
+00013a90: 300a 2020 2020 2020 2020 656d 3020 3d20  0.        em0 = 
+00013aa0: 300a 0a20 2020 2072 6574 7572 6e20 6d30  0..    return m0
+00013ab0: 202a 2031 3030 2c20 656d 3020 2a20 3130   * 100, em0 * 10
+00013ac0: 302c 2064 6973 740a 0a0a 6465 6620 6d77  0, dist...def mw
+00013ad0: 6373 5f64 7676 2872 6566 2c20 6375 722c  cs_dvv(ref, cur,
+00013ae0: 206d 6f76 696e 675f 7769 6e64 6f77 5f6c   moving_window_l
+00013af0: 656e 6774 682c 2073 6c69 6465 5f73 7465  ength, slide_ste
+00013b00: 702c 2070 6172 612c 2073 6d6f 6f74 6869  p, para, smoothi
+00013b10: 6e67 5f68 616c 665f 7769 6e3d 3529 3a0a  ng_half_win=5):.
+00013b20: 2020 2020 2222 220a 2020 2020 4d6f 7669      """.    Movi
+00013b30: 6e67 2057 696e 646f 7720 4372 6f73 7320  ng Window Cross 
+00013b40: 5370 6563 7472 756d 206d 6574 686f 6420  Spectrum method 
+00013b50: 746f 206d 6561 7375 7265 2064 762f 7620  to measure dv/v 
+00013b60: 2872 656c 7969 6e67 206f 6e20 7068 693d  (relying on phi=
+00013b70: 322a 7069 2a66 2a74 2069 6e20 6672 6571  2*pi*f*t in freq
+00013b80: 2064 6f6d 6169 6e29 0a0a 2020 2020 5041   domain)..    PA
+00013b90: 5241 4d45 5445 5253 3a0a 2020 2020 2d2d  RAMETERS:.    --
+00013ba0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+00013bb0: 2020 2072 6566 3a20 5265 6665 7265 6e63     ref: Referenc
+00013bc0: 6520 7761 7665 666f 726d 2028 6e70 2e6e  e waveform (np.n
+00013bd0: 6461 7272 6179 2c20 7369 7a65 204e 290a  darray, size N).
+00013be0: 2020 2020 6375 723a 2043 7572 7265 6e74      cur: Current
+00013bf0: 2077 6176 6566 6f72 6d20 286e 702e 6e64   waveform (np.nd
+00013c00: 6172 7261 792c 2073 697a 6520 4e29 0a20  array, size N). 
+00013c10: 2020 206d 6f76 696e 675f 7769 6e64 6f77     moving_window
+00013c20: 5f6c 656e 6774 683a 206d 6f76 696e 6720  _length: moving 
+00013c30: 7769 6e64 6f77 206c 656e 6774 6820 746f  window length to
+00013c40: 2063 616c 6375 6c61 7465 2063 726f 7373   calculate cross
+00013c50: 2d73 7065 6374 7275 6d20 286e 702e 666c  -spectrum (np.fl
+00013c60: 6f61 742c 2069 6e20 7365 6329 0a20 2020  oat, in sec).   
+00013c70: 2073 6c69 6465 5f73 7465 703a 2073 7465   slide_step: ste
+00013c80: 7073 2069 6e20 7469 6d65 2074 6f20 7368  ps in time to sh
+00013c90: 6966 7420 7468 6520 6d6f 7669 6e67 2077  ift the moving w
+00013ca0: 696e 646f 7720 286e 702e 666c 6f61 742c  indow (np.float,
+00013cb0: 2069 6e20 7365 636f 6e64 7329 0a20 2020   in seconds).   
+00013cc0: 2070 6172 613a 2061 2064 6963 7420 636f   para: a dict co
+00013cd0: 6e74 6169 6e69 6e67 2070 6172 616d 6574  ntaining paramet
+00013ce0: 6572 7320 6162 6f75 7420 696e 7075 7420  ers about input 
+00013cf0: 6461 7461 2077 696e 646f 7720 616e 6420  data window and 
+00013d00: 6672 6571 7565 6e63 7920 696e 666f 2c20  frequency info, 
+00013d10: 696e 636c 7564 696e 670a 2020 2020 2020  including.      
+00013d20: 2020 6465 6c74 612d 3e54 6865 2073 616d    delta->The sam
+00013d30: 706c 696e 6720 7261 7465 206f 6620 7468  pling rate of th
+00013d40: 6520 696e 7075 7420 7469 6d65 7365 7269  e input timeseri
+00013d50: 6573 2028 696e 2048 7a29 0a20 2020 2020  es (in Hz).     
+00013d60: 2020 2077 696e 646f 772d 3e20 5468 6520     window-> The 
+00013d70: 7461 7267 6574 2077 696e 646f 7720 666f  target window fo
+00013d80: 7220 6d65 6173 7572 696e 6720 6474 2f74  r measuring dt/t
+00013d90: 0a20 2020 2020 2020 2066 7265 712d 3e20  .        freq-> 
+00013da0: 5468 6520 6672 6571 7565 6e63 7920 626f  The frequency bo
+00013db0: 756e 6420 746f 2063 6f6d 7075 7465 2074  und to compute t
+00013dc0: 6865 2064 6570 6861 7369 6e67 2028 696e  he dephasing (in
+00013dd0: 2048 7a29 0a20 2020 2020 2020 2074 6d69   Hz).        tmi
+00013de0: 6e3a 2054 6865 206c 6566 746d 6f73 7420  n: The leftmost 
+00013df0: 7469 6d65 206c 6167 2028 7573 6564 2074  time lag (used t
+00013e00: 6f20 636f 6d70 7574 6520 7468 6520 2274  o compute the "t
+00013e10: 696d 6520 6c61 6773 2061 7272 6179 2229  ime lags array")
+00013e20: 0a20 2020 2073 6d6f 6f74 6869 6e67 5f68  .    smoothing_h
+00013e30: 616c 665f 7769 6e3a 2049 6620 6469 6666  alf_win: If diff
+00013e40: 6572 656e 7420 6672 6f6d 2030 2c20 6465  erent from 0, de
+00013e50: 6669 6e65 7320 7468 6520 6861 6c66 206c  fines the half l
+00013e60: 656e 6774 6820 6f66 2074 6865 2073 6d6f  ength of the smo
+00013e70: 6f74 6869 6e67 2068 616e 6e69 6e67 2077  othing hanning w
+00013e80: 696e 646f 772e 0a0a 2020 2020 5245 5455  indow...    RETU
+00013e90: 524e 533a 0a20 2020 202d 2d2d 2d2d 2d2d  RNS:.    -------
+00013ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00013eb0: 7469 6d65 5f61 7869 733a 2074 6865 2063  time_axis: the c
+00013ec0: 656e 7472 616c 2074 696d 6573 206f 6620  entral times of 
+00013ed0: 7468 6520 7769 6e64 6f77 732e 0a20 2020  the windows..   
+00013ee0: 2064 656c 7461 5f74 3a20 6474 0a20 2020   delta_t: dt.   
+00013ef0: 2064 656c 7461 5f65 7272 3a65 7272 6f72   delta_err:error
+00013f00: 0a20 2020 2064 656c 7461 5f6d 636f 683a  .    delta_mcoh:
+00013f10: 206d 6561 6e20 636f 6865 7265 6e63 650a   mean coherence.
+00013f20: 0a20 2020 2043 6f70 6965 6420 6672 6f6d  .    Copied from
+00013f30: 204d 534e 6f69 7365 2028 6874 7470 733a   MSNoise (https:
+00013f40: 2f2f 6769 7468 7562 2e63 6f6d 2f52 4f42  //github.com/ROB
+00013f50: 656c 6769 756d 2f4d 534e 6f69 7365 2f74  elgium/MSNoise/t
+00013f60: 7265 652f 6d61 7374 6572 2f6d 736e 6f69  ree/master/msnoi
+00013f70: 7365 290a 2020 2020 4d6f 6469 6669 6564  se).    Modified
+00013f80: 2062 7920 4368 656e 6778 696e 204a 6961   by Chengxin Jia
+00013f90: 6e67 0a20 2020 2022 2222 0a20 2020 2023  ng.    """.    #
+00013fa0: 2063 6f6d 6d6f 6e20 7661 7269 6162 6c65   common variable
+00013fb0: 730a 2020 2020 7477 696e 203d 2070 6172  s.    twin = par
+00013fc0: 615b 2274 7769 6e22 5d0a 2020 2020 6672  a["twin"].    fr
+00013fd0: 6571 203d 2070 6172 615b 2266 7265 7122  eq = para["freq"
+00013fe0: 5d0a 2020 2020 6474 203d 2070 6172 615b  ].    dt = para[
+00013ff0: 2264 7422 5d0a 2020 2020 746d 696e 203d  "dt"].    tmin =
+00014000: 206e 702e 6d69 6e28 7477 696e 290a 2020   np.min(twin).  
+00014010: 2020 666d 696e 203d 206e 702e 6d69 6e28    fmin = np.min(
+00014020: 6672 6571 290a 2020 2020 666d 6178 203d  freq).    fmax =
+00014030: 206e 702e 6d61 7828 6672 6571 290a 0a20   np.max(freq).. 
+00014040: 2020 2023 2070 6172 616d 6574 6572 2069     # parameter i
+00014050: 6e69 7469 616c 697a 650a 2020 2020 6465  nitialize.    de
+00014060: 6c74 615f 7420 3d20 5b5d 0a20 2020 2064  lta_t = [].    d
+00014070: 656c 7461 5f65 7272 203d 205b 5d0a 2020  elta_err = [].  
+00014080: 2020 6465 6c74 615f 6d63 6f68 203d 205b    delta_mcoh = [
+00014090: 5d0a 2020 2020 7469 6d65 5f61 7869 7320  ].    time_axis 
+000140a0: 3d20 5b5d 0a0a 2020 2020 2320 696e 666f  = []..    # info
+000140b0: 206f 6e20 7468 6520 6d6f 7669 6e67 2077   on the moving w
+000140c0: 696e 646f 770a 2020 2020 7769 6e64 6f77  indow.    window
+000140d0: 5f6c 656e 6774 685f 7361 6d70 6c65 7320  _length_samples 
+000140e0: 3d20 6e70 2e69 6e74 286d 6f76 696e 675f  = np.int(moving_
+000140f0: 7769 6e64 6f77 5f6c 656e 6774 6820 2f20  window_length / 
+00014100: 6474 290a 2020 2020 7061 6464 203d 2069  dt).    padd = i
+00014110: 6e74 2832 202a 2a20 286e 6578 7470 6f77  nt(2 ** (nextpow
+00014120: 3228 7769 6e64 6f77 5f6c 656e 6774 685f  2(window_length_
+00014130: 7361 6d70 6c65 7329 202b 2032 2929 0a20  samples) + 2)). 
+00014140: 2020 2063 6f75 6e74 203d 2030 0a20 2020     count = 0.   
+00014150: 2074 7020 3d20 636f 7369 6e65 5f74 6170   tp = cosine_tap
+00014160: 6572 2877 696e 646f 775f 6c65 6e67 7468  er(window_length
+00014170: 5f73 616d 706c 6573 2c20 302e 3135 290a  _samples, 0.15).
+00014180: 0a20 2020 206d 696e 696e 6420 3d20 300a  .    minind = 0.
+00014190: 2020 2020 6d61 7869 6e64 203d 2077 696e      maxind = win
+000141a0: 646f 775f 6c65 6e67 7468 5f73 616d 706c  dow_length_sampl
+000141b0: 6573 0a0a 2020 2020 2320 6c6f 6f70 2074  es..    # loop t
+000141c0: 6872 6f75 6768 2061 6c6c 2073 7562 2d77  hrough all sub-w
+000141d0: 696e 646f 7773 0a20 2020 2077 6869 6c65  indows.    while
+000141e0: 206d 6178 696e 6420 3c3d 206c 656e 2872   maxind <= len(r
+000141f0: 6566 293a 0a20 2020 2020 2020 2063 6369  ef):.        cci
+00014200: 203d 2063 7572 5b6d 696e 696e 643a 6d61   = cur[minind:ma
+00014210: 7869 6e64 5d0a 2020 2020 2020 2020 6363  xind].        cc
+00014220: 6920 3d20 7363 6970 792e 7369 676e 616c  i = scipy.signal
+00014230: 2e64 6574 7265 6e64 2863 6369 2c20 7479  .detrend(cci, ty
+00014240: 7065 3d22 6c69 6e65 6172 2229 0a20 2020  pe="linear").   
+00014250: 2020 2020 2063 6369 202a 3d20 7470 0a0a       cci *= tp..
+00014260: 2020 2020 2020 2020 6372 6920 3d20 7265          cri = re
+00014270: 665b 6d69 6e69 6e64 3a6d 6178 696e 645d  f[minind:maxind]
+00014280: 0a20 2020 2020 2020 2063 7269 203d 2073  .        cri = s
+00014290: 6369 7079 2e73 6967 6e61 6c2e 6465 7472  cipy.signal.detr
+000142a0: 656e 6428 6372 692c 2074 7970 653d 226c  end(cri, type="l
+000142b0: 696e 6561 7222 290a 2020 2020 2020 2020  inear").        
+000142c0: 6372 6920 2a3d 2074 700a 0a20 2020 2020  cri *= tp..     
+000142d0: 2020 206d 696e 696e 6420 2b3d 2069 6e74     minind += int
+000142e0: 2873 6c69 6465 5f73 7465 7020 2f20 6474  (slide_step / dt
+000142f0: 290a 2020 2020 2020 2020 6d61 7869 6e64  ).        maxind
+00014300: 202b 3d20 696e 7428 736c 6964 655f 7374   += int(slide_st
+00014310: 6570 202f 2064 7429 0a0a 2020 2020 2020  ep / dt)..      
+00014320: 2020 2320 646f 2066 6674 0a20 2020 2020    # do fft.     
+00014330: 2020 2066 6375 7220 3d20 7363 6970 792e     fcur = scipy.
+00014340: 6666 7470 6163 6b2e 6666 7428 6363 692c  fftpack.fft(cci,
+00014350: 206e 3d70 6164 6429 5b3a 2070 6164 6420   n=padd)[: padd 
+00014360: 2f2f 2032 5d0a 2020 2020 2020 2020 6672  // 2].        fr
+00014370: 6566 203d 2073 6369 7079 2e66 6674 7061  ef = scipy.fftpa
+00014380: 636b 2e66 6674 2863 7269 2c20 6e3d 7061  ck.fft(cri, n=pa
+00014390: 6464 295b 3a20 7061 6464 202f 2f20 325d  dd)[: padd // 2]
+000143a0: 0a0a 2020 2020 2020 2020 6663 7572 3220  ..        fcur2 
+000143b0: 3d20 6e70 2e72 6561 6c28 6663 7572 2920  = np.real(fcur) 
+000143c0: 2a2a 2032 202b 206e 702e 696d 6167 2866  ** 2 + np.imag(f
+000143d0: 6375 7229 202a 2a20 320a 2020 2020 2020  cur) ** 2.      
+000143e0: 2020 6672 6566 3220 3d20 6e70 2e72 6561    fref2 = np.rea
+000143f0: 6c28 6672 6566 2920 2a2a 2032 202b 206e  l(fref) ** 2 + n
+00014400: 702e 696d 6167 2866 7265 6629 202a 2a20  p.imag(fref) ** 
+00014410: 320a 0a20 2020 2020 2020 2023 2067 6574  2..        # get
+00014420: 2063 726f 7373 2d73 7065 6374 7275 6d20   cross-spectrum 
+00014430: 2620 646f 2066 696c 7465 7269 6e67 0a20  & do filtering. 
+00014440: 2020 2020 2020 2058 203d 2066 7265 6620         X = fref 
+00014450: 2a20 2866 6375 722e 636f 6e6a 2829 290a  * (fcur.conj()).
+00014460: 2020 2020 2020 2020 6966 2073 6d6f 6f74          if smoot
+00014470: 6869 6e67 5f68 616c 665f 7769 6e20 213d  hing_half_win !=
+00014480: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00014490: 6463 7572 203d 206e 702e 7371 7274 2873  dcur = np.sqrt(s
+000144a0: 6d6f 6f74 6828 6663 7572 322c 2077 696e  mooth(fcur2, win
+000144b0: 646f 773d 2268 616e 6e69 6e67 222c 2068  dow="hanning", h
+000144c0: 616c 665f 7769 6e3d 736d 6f6f 7468 696e  alf_win=smoothin
+000144d0: 675f 6861 6c66 5f77 696e 2929 0a20 2020  g_half_win)).   
+000144e0: 2020 2020 2020 2020 2064 7265 6620 3d20           dref = 
+000144f0: 6e70 2e73 7172 7428 736d 6f6f 7468 2866  np.sqrt(smooth(f
+00014500: 7265 6632 2c20 7769 6e64 6f77 3d22 6861  ref2, window="ha
+00014510: 6e6e 696e 6722 2c20 6861 6c66 5f77 696e  nning", half_win
+00014520: 3d73 6d6f 6f74 6869 6e67 5f68 616c 665f  =smoothing_half_
+00014530: 7769 6e29 290a 2020 2020 2020 2020 2020  win)).          
+00014540: 2020 5820 3d20 736d 6f6f 7468 2858 2c20    X = smooth(X, 
+00014550: 7769 6e64 6f77 3d22 6861 6e6e 696e 6722  window="hanning"
+00014560: 2c20 6861 6c66 5f77 696e 3d73 6d6f 6f74  , half_win=smoot
+00014570: 6869 6e67 5f68 616c 665f 7769 6e29 0a20  hing_half_win). 
+00014580: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00014590: 2020 2020 2020 2020 2064 6375 7220 3d20           dcur = 
+000145a0: 6e70 2e73 7172 7428 6663 7572 3229 0a20  np.sqrt(fcur2). 
+000145b0: 2020 2020 2020 2020 2020 2064 7265 6620             dref 
+000145c0: 3d20 6e70 2e73 7172 7428 6672 6566 3229  = np.sqrt(fref2)
+000145d0: 0a0a 2020 2020 2020 2020 6463 7320 3d20  ..        dcs = 
+000145e0: 6e70 2e61 6273 2858 290a 0a20 2020 2020  np.abs(X)..     
+000145f0: 2020 2023 2046 696e 6420 7468 6520 7661     # Find the va
+00014600: 6c75 6573 2074 6865 2066 7265 7175 656e  lues the frequen
+00014610: 6379 2072 616e 6765 206f 6620 696e 7465  cy range of inte
+00014620: 7265 7374 0a20 2020 2020 2020 2066 7265  rest.        fre
+00014630: 715f 7665 6320 3d20 7363 6970 792e 6666  q_vec = scipy.ff
+00014640: 7470 6163 6b2e 6666 7466 7265 7128 6c65  tpack.fftfreq(le
+00014650: 6e28 5829 202a 2032 2c20 6474 295b 3a20  n(X) * 2, dt)[: 
+00014660: 7061 6464 202f 2f20 325d 0a20 2020 2020  padd // 2].     
+00014670: 2020 2069 6e64 6578 5f72 616e 6765 203d     index_range =
+00014680: 206e 702e 6172 6777 6865 7265 286e 702e   np.argwhere(np.
+00014690: 6c6f 6769 6361 6c5f 616e 6428 6672 6571  logical_and(freq
+000146a0: 5f76 6563 203e 3d20 666d 696e 2c20 6672  _vec >= fmin, fr
+000146b0: 6571 5f76 6563 203c 3d20 666d 6178 2929  eq_vec <= fmax))
+000146c0: 0a0a 2020 2020 2020 2020 2320 4765 7420  ..        # Get 
+000146d0: 436f 6865 7265 6e63 6520 616e 6420 6974  Coherence and it
+000146e0: 7320 6d65 616e 2076 616c 7565 0a20 2020  s mean value.   
+000146f0: 2020 2020 2063 6f68 203d 2067 6574 436f       coh = getCo
+00014700: 6865 7265 6e63 6528 6463 732c 2064 7265  herence(dcs, dre
+00014710: 662c 2064 6375 7229 0a20 2020 2020 2020  f, dcur).       
+00014720: 206d 636f 6820 3d20 6e70 2e6d 6561 6e28   mcoh = np.mean(
+00014730: 636f 685b 696e 6465 785f 7261 6e67 655d  coh[index_range]
+00014740: 290a 0a20 2020 2020 2020 2023 2047 6574  )..        # Get
+00014750: 2057 6569 6768 7473 0a20 2020 2020 2020   Weights.       
+00014760: 2077 203d 2031 2e30 202f 2028 312e 3020   w = 1.0 / (1.0 
+00014770: 2f20 2863 6f68 5b69 6e64 6578 5f72 616e  / (coh[index_ran
+00014780: 6765 5d20 2a2a 2032 2920 2d20 312e 3029  ge] ** 2) - 1.0)
+00014790: 0a20 2020 2020 2020 2077 5b63 6f68 5b69  .        w[coh[i
+000147a0: 6e64 6578 5f72 616e 6765 5d20 3e3d 2030  ndex_range] >= 0
+000147b0: 2e39 395d 203d 2031 2e30 202f 2028 312e  .99] = 1.0 / (1.
+000147c0: 3020 2f20 302e 3938 3031 202d 2031 2e30  0 / 0.9801 - 1.0
+000147d0: 290a 2020 2020 2020 2020 7720 3d20 6e70  ).        w = np
+000147e0: 2e73 7172 7428 7720 2a20 6e70 2e73 7172  .sqrt(w * np.sqr
+000147f0: 7428 6463 735b 696e 6465 785f 7261 6e67  t(dcs[index_rang
+00014800: 655d 2929 0a20 2020 2020 2020 2077 203d  e])).        w =
+00014810: 206e 702e 7265 616c 2877 290a 0a20 2020   np.real(w)..   
+00014820: 2020 2020 2023 2046 7265 7175 656e 6379       # Frequency
+00014830: 2061 7272 6179 3a0a 2020 2020 2020 2020   array:.        
+00014840: 7620 3d20 6e70 2e72 6561 6c28 6672 6571  v = np.real(freq
+00014850: 5f76 6563 5b69 6e64 6578 5f72 616e 6765  _vec[index_range
+00014860: 5d29 202a 2032 202a 206e 702e 7069 0a0a  ]) * 2 * np.pi..
+00014870: 2020 2020 2020 2020 2320 5068 6173 653a          # Phase:
+00014880: 0a20 2020 2020 2020 2070 6869 203d 206e  .        phi = n
+00014890: 702e 616e 676c 6528 5829 0a20 2020 2020  p.angle(X).     
+000148a0: 2020 2070 6869 5b30 5d20 3d20 302e 300a     phi[0] = 0.0.
+000148b0: 2020 2020 2020 2020 7068 6920 3d20 6e70          phi = np
+000148c0: 2e75 6e77 7261 7028 7068 6929 0a20 2020  .unwrap(phi).   
+000148d0: 2020 2020 2070 6869 203d 2070 6869 5b69       phi = phi[i
+000148e0: 6e64 6578 5f72 616e 6765 5d0a 0a20 2020  ndex_range]..   
+000148f0: 2020 2020 2023 2043 616c 6375 6c61 7465       # Calculate
+00014900: 2074 6865 2073 6c6f 7065 2077 6974 6820   the slope with 
+00014910: 6120 7765 6967 6874 6564 206c 6561 7374  a weighted least
+00014920: 2073 7175 6172 6520 6c69 6e65 6172 2072   square linear r
+00014930: 6567 7265 7373 696f 6e0a 2020 2020 2020  egression.      
+00014940: 2020 2320 666f 7263 6564 2074 6872 6f75    # forced throu
+00014950: 6768 2074 6865 206f 7269 6769 6e3b 2077  gh the origin; w
+00014960: 6569 6768 7473 2066 6f72 2074 6865 2057  eights for the W
+00014970: 4c53 206d 7573 7420 6265 2074 6865 2076  LS must be the v
+00014980: 6172 6961 6e63 6520 210a 2020 2020 2020  ariance !.      
+00014990: 2020 6d2c 2065 6d20 3d20 6c69 6e65 6172    m, em = linear
+000149a0: 5f72 6567 7265 7373 696f 6e28 762e 666c  _regression(v.fl
+000149b0: 6174 7465 6e28 292c 2070 6869 2e66 6c61  atten(), phi.fla
+000149c0: 7474 656e 2829 2c20 772e 666c 6174 7465  tten(), w.flatte
+000149d0: 6e28 2929 0a20 2020 2020 2020 2064 656c  n()).        del
+000149e0: 7461 5f74 2e61 7070 656e 6428 6d29 0a0a  ta_t.append(m)..
+000149f0: 2020 2020 2020 2020 2320 7072 696e 7420          # print 
+00014a00: 7068 692e 7368 6170 652c 2076 2e73 6861  phi.shape, v.sha
+00014a10: 7065 2c20 772e 7368 6170 650a 2020 2020  pe, w.shape.    
+00014a20: 2020 2020 6520 3d20 6e70 2e73 756d 2828      e = np.sum((
+00014a30: 7068 6920 2d20 6d20 2a20 7629 202a 2a20  phi - m * v) ** 
+00014a40: 3229 202f 2028 6e70 2e73 697a 6528 7629  2) / (np.size(v)
+00014a50: 202d 2031 290a 2020 2020 2020 2020 7332   - 1).        s2
+00014a60: 7832 203d 206e 702e 7375 6d28 762a 2a32  x2 = np.sum(v**2
+00014a70: 202a 2077 2a2a 3229 0a20 2020 2020 2020   * w**2).       
+00014a80: 2073 7832 203d 206e 702e 7375 6d28 7720   sx2 = np.sum(w 
+00014a90: 2a20 762a 2a32 290a 2020 2020 2020 2020  * v**2).        
+00014aa0: 6520 3d20 6e70 2e73 7172 7428 6520 2a20  e = np.sqrt(e * 
+00014ab0: 7332 7832 202f 2073 7832 2a2a 3229 0a0a  s2x2 / sx2**2)..
+00014ac0: 2020 2020 2020 2020 6465 6c74 615f 6572          delta_er
+00014ad0: 722e 6170 7065 6e64 2865 290a 2020 2020  r.append(e).    
+00014ae0: 2020 2020 6465 6c74 615f 6d63 6f68 2e61      delta_mcoh.a
+00014af0: 7070 656e 6428 6e70 2e72 6561 6c28 6d63  ppend(np.real(mc
+00014b00: 6f68 2929 0a20 2020 2020 2020 2074 696d  oh)).        tim
+00014b10: 655f 6178 6973 2e61 7070 656e 6428 746d  e_axis.append(tm
+00014b20: 696e 202b 206d 6f76 696e 675f 7769 6e64  in + moving_wind
+00014b30: 6f77 5f6c 656e 6774 6820 2f20 322e 3020  ow_length / 2.0 
+00014b40: 2b20 636f 756e 7420 2a20 736c 6964 655f  + count * slide_
+00014b50: 7374 6570 290a 2020 2020 2020 2020 636f  step).        co
+00014b60: 756e 7420 2b3d 2031 0a0a 2020 2020 2020  unt += 1..      
+00014b70: 2020 6465 6c20 6663 7572 2c20 6672 6566    del fcur, fref
+00014b80: 0a20 2020 2020 2020 2064 656c 2058 0a20  .        del X. 
+00014b90: 2020 2020 2020 2064 656c 2066 7265 715f         del freq_
+00014ba0: 7665 630a 2020 2020 2020 2020 6465 6c20  vec.        del 
+00014bb0: 696e 6465 785f 7261 6e67 650a 2020 2020  index_range.    
+00014bc0: 2020 2020 6465 6c20 772c 2076 2c20 652c      del w, v, e,
+00014bd0: 2073 3278 322c 2073 7832 2c20 6d2c 2065   s2x2, sx2, m, e
+00014be0: 6d0a 0a20 2020 2069 6620 6d61 7869 6e64  m..    if maxind
+00014bf0: 203e 206c 656e 2863 7572 2920 2b20 696e   > len(cur) + in
+00014c00: 7428 736c 6964 655f 7374 6570 202f 2064  t(slide_step / d
+00014c10: 7429 3a0a 2020 2020 2020 2020 7072 696e  t):.        prin
+00014c20: 7428 2254 6865 206c 6173 7420 7769 6e64  t("The last wind
+00014c30: 6f77 2077 6173 2074 6f6f 2073 6d61 6c6c  ow was too small
+00014c40: 2c20 6275 7420 7761 7320 636f 6d70 7574  , but was comput
+00014c50: 6564 2229 0a0a 2020 2020 2320 656e 7375  ed")..    # ensu
+00014c60: 7265 2061 6c6c 206d 6174 7269 7820 6172  re all matrix ar
+00014c70: 6520 6e70 2061 7272 6179 0a20 2020 2064  e np array.    d
+00014c80: 656c 7461 5f74 203d 206e 702e 6172 7261  elta_t = np.arra
+00014c90: 7928 6465 6c74 615f 7429 0a20 2020 2064  y(delta_t).    d
+00014ca0: 656c 7461 5f65 7272 203d 206e 702e 6172  elta_err = np.ar
+00014cb0: 7261 7928 6465 6c74 615f 6572 7229 0a20  ray(delta_err). 
+00014cc0: 2020 2064 656c 7461 5f6d 636f 6820 3d20     delta_mcoh = 
+00014cd0: 6e70 2e61 7272 6179 2864 656c 7461 5f6d  np.array(delta_m
+00014ce0: 636f 6829 0a20 2020 2074 696d 655f 6178  coh).    time_ax
+00014cf0: 6973 203d 206e 702e 6172 7261 7928 7469  is = np.array(ti
+00014d00: 6d65 5f61 7869 7329 0a0a 2020 2020 2320  me_axis)..    # 
+00014d10: 7265 6164 7920 666f 7220 6c69 6e65 6172  ready for linear
+00014d20: 2072 6567 7265 7373 696f 6e0a 2020 2020   regression.    
+00014d30: 6465 6c74 615f 6d69 6e63 686f 203d 2030  delta_mincho = 0
+00014d40: 2e36 350a 2020 2020 6465 6c74 615f 6d61  .65.    delta_ma
+00014d50: 7865 7272 203d 2030 2e31 0a20 2020 2064  xerr = 0.1.    d
+00014d60: 656c 7461 5f6d 6178 6474 203d 2030 2e31  elta_maxdt = 0.1
+00014d70: 0a20 2020 2069 6e64 7831 203d 206e 702e  .    indx1 = np.
+00014d80: 7768 6572 6528 6465 6c74 615f 6d63 6f68  where(delta_mcoh
+00014d90: 203e 2064 656c 7461 5f6d 696e 6368 6f29   > delta_mincho)
+00014da0: 0a20 2020 2069 6e64 7832 203d 206e 702e  .    indx2 = np.
+00014db0: 7768 6572 6528 6465 6c74 615f 6572 7220  where(delta_err 
+00014dc0: 3c20 6465 6c74 615f 6d61 7865 7272 290a  < delta_maxerr).
+00014dd0: 2020 2020 696e 6478 3320 3d20 6e70 2e77      indx3 = np.w
+00014de0: 6865 7265 2864 656c 7461 5f74 203c 2064  here(delta_t < d
+00014df0: 656c 7461 5f6d 6178 6474 290a 0a20 2020  elta_maxdt)..   
+00014e00: 2023 202d 2d2d 2d2d 6669 6e64 2067 6f6f   # -----find goo
+00014e10: 6420 6474 206d 6561 7375 7265 6d65 6e74  d dt measurement
+00014e20: 732d 2d2d 2d2d 0a20 2020 2069 6e64 7820  s-----.    indx 
+00014e30: 3d20 6e70 2e69 6e74 6572 7365 6374 3164  = np.intersect1d
+00014e40: 2869 6e64 7831 2c20 696e 6478 3229 0a20  (indx1, indx2). 
+00014e50: 2020 2069 6e64 7820 3d20 6e70 2e69 6e74     indx = np.int
+00014e60: 6572 7365 6374 3164 2869 6e64 782c 2069  ersect1d(indx, i
+00014e70: 6e64 7833 290a 0a20 2020 2069 6620 6c65  ndx3)..    if le
+00014e80: 6e28 696e 6478 2920 3e20 323a 0a20 2020  n(indx) > 2:.   
+00014e90: 2020 2020 2023 202d 2d2d 2d65 7374 696d       # ----estim
+00014ea0: 6174 6520 7765 6967 6874 2066 6f72 2072  ate weight for r
+00014eb0: 6567 7265 7373 696f 6e2d 2d2d 2d0a 2020  egression----.  
+00014ec0: 2020 2020 2020 7720 3d20 3120 2f20 6465        w = 1 / de
+00014ed0: 6c74 615f 6572 725b 696e 6478 5d0a 2020  lta_err[indx].  
+00014ee0: 2020 2020 2020 775b 7e6e 702e 6973 6669        w[~np.isfi
+00014ef0: 6e69 7465 2877 295d 203d 2031 2e30 0a0a  nite(w)] = 1.0..
+00014f00: 2020 2020 2020 2020 2320 2d2d 2d2d 2d2d          # ------
+00014f10: 2d2d 2d64 6f20 6c69 6e65 6172 2072 6567  ---do linear reg
+00014f20: 7265 7373 696f 6e2d 2d2d 2d2d 2d2d 2d2d  ression---------
+00014f30: 2d2d 0a20 2020 2020 2020 2023 206d 2c20  --.        # m, 
+00014f40: 612c 2065 6d2c 2065 6120 3d20 6c69 6e65  a, em, ea = line
+00014f50: 6172 5f72 6567 7265 7373 696f 6e28 7469  ar_regression(ti
+00014f60: 6d65 5f61 7869 735b 696e 6478 5d2c 2064  me_axis[indx], d
+00014f70: 656c 7461 5f74 5b69 6e64 785d 2c20 772c  elta_t[indx], w,
+00014f80: 2069 6e74 6572 6365 7074 5f6f 7269 6769   intercept_origi
+00014f90: 6e3d 4661 6c73 6529 0a20 2020 2020 2020  n=False).       
+00014fa0: 206d 302c 2065 6d30 203d 206c 696e 6561   m0, em0 = linea
+00014fb0: 725f 7265 6772 6573 7369 6f6e 2874 696d  r_regression(tim
+00014fc0: 655f 6178 6973 5b69 6e64 785d 2c20 6465  e_axis[indx], de
+00014fd0: 6c74 615f 745b 696e 6478 5d2c 2077 2c20  lta_t[indx], w, 
+00014fe0: 696e 7465 7263 6570 745f 6f72 6967 696e  intercept_origin
+00014ff0: 3d54 7275 6529 0a0a 2020 2020 656c 7365  =True)..    else
+00015000: 3a0a 2020 2020 2020 2020 7072 696e 7428  :.        print(
+00015010: 226e 6f74 2065 6e6f 7567 6820 706f 696e  "not enough poin
+00015020: 7473 2074 6f20 6573 7469 6d61 7465 2064  ts to estimate d
+00015030: 762f 7620 666f 7220 6d77 6373 2229 0a20  v/v for mwcs"). 
+00015040: 2020 2020 2020 206d 3020 3d20 300a 2020         m0 = 0.  
+00015050: 2020 2020 2020 656d 3020 3d20 300a 0a20        em0 = 0.. 
+00015060: 2020 2072 6574 7572 6e20 2d6d 3020 2a20     return -m0 * 
+00015070: 3130 302c 2065 6d30 202a 2031 3030 0a0a  100, em0 * 100..
+00015080: 0a64 6566 2057 4343 5f64 7676 2872 6566  .def WCC_dvv(ref
+00015090: 2c20 6375 722c 206d 6f76 696e 675f 7769  , cur, moving_wi
+000150a0: 6e64 6f77 5f6c 656e 6774 682c 2073 6c69  ndow_length, sli
+000150b0: 6465 5f73 7465 702c 2070 6172 6129 3a0a  de_step, para):.
+000150c0: 2020 2020 2222 220a 2020 2020 5769 6e64      """.    Wind
+000150d0: 6f77 6564 2063 726f 7373 2063 6f72 7265  owed cross corre
+000150e0: 6c61 7469 6f6e 2028 5743 4329 2066 6f72  lation (WCC) for
+000150f0: 2064 7420 6f72 2064 762f 7620 6d65 7375   dt or dv/v mesu
+00015100: 7265 6d65 6e74 2028 536e 6965 6465 7220  rement (Snieder 
+00015110: 6574 2061 6c2e 2032 3031 3229 0a0a 2020  et al. 2012)..  
+00015120: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
+00015130: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020    -----------.  
+00015140: 2020 7265 663a 2054 6865 2022 5265 6665    ref: The "Refe
+00015150: 7265 6e63 6522 2074 696d 6573 6572 6965  rence" timeserie
+00015160: 730a 2020 2020 6375 723a 2054 6865 2022  s.    cur: The "
+00015170: 4375 7272 656e 7422 2074 696d 6573 6572  Current" timeser
+00015180: 6965 730a 2020 2020 6d6f 7669 6e67 5f77  ies.    moving_w
+00015190: 696e 646f 775f 6c65 6e67 7468 3a20 5468  indow_length: Th
+000151a0: 6520 6d6f 7669 6e67 2077 696e 646f 7720  e moving window 
+000151b0: 6c65 6e67 7468 2028 696e 2073 6563 6f6e  length (in secon
+000151c0: 6473 290a 2020 2020 736c 6964 655f 7374  ds).    slide_st
+000151d0: 6570 3a20 5468 6520 7374 6570 2074 6f20  ep: The step to 
+000151e0: 6a75 6d70 2066 6f72 2074 6865 206d 6f76  jump for the mov
+000151f0: 696e 6720 7769 6e64 6f77 2028 696e 2073  ing window (in s
+00015200: 6563 6f6e 6473 290a 2020 2020 7061 7261  econds).    para
+00015210: 3a20 6120 6469 6374 2063 6f6e 7461 696e  : a dict contain
+00015220: 696e 6720 6672 6571 2f74 696d 6520 696e  ing freq/time in
+00015230: 666f 206f 6620 7468 6520 6461 7461 206d  fo of the data m
+00015240: 6174 7269 780a 0a20 2020 2052 6574 7572  atrix..    Retur
+00015250: 6e73 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  ns:.    --------
+00015260: 2d2d 2d2d 0a20 2020 2074 696d 655f 6178  ----.    time_ax
+00015270: 6973 3a20 6365 6e74 7261 6c20 7469 6d65  is: central time
+00015280: 7320 6f66 2074 6865 206d 6f76 696e 6720  s of the moving 
+00015290: 7769 6e64 6f77 0a20 2020 2064 656c 7461  window.    delta
+000152a0: 5f74 3a20 6474 0a20 2020 2064 656c 7461  _t: dt.    delta
+000152b0: 5f65 7272 3a20 6572 726f 720a 2020 2020  _err: error.    
+000152c0: 6465 6c74 615f 6d63 6f68 3a20 6d65 616e  delta_mcoh: mean
+000152d0: 2063 6f68 6572 656e 6365 2066 6f72 2065   coherence for e
+000152e0: 6163 6820 7769 6e64 6f77 0a0a 2020 2020  ach window..    
+000152f0: 5772 6974 7465 6e20 6279 2043 6f6e 6763  Written by Congc
+00015300: 6f6e 6720 5975 616e 2028 3120 4a75 6c79  ong Yuan (1 July
+00015310: 2c20 3230 3139 290a 2020 2020 2222 220a  , 2019).    """.
+00015320: 2020 2020 2320 636f 6d6d 6f6e 2076 6172      # common var
+00015330: 6961 626c 6573 0a20 2020 2074 7769 6e20  iables.    twin 
+00015340: 3d20 7061 7261 5b22 7477 696e 225d 0a20  = para["twin"]. 
+00015350: 2020 2064 7420 3d20 7061 7261 5b22 6474     dt = para["dt
+00015360: 225d 0a20 2020 2074 6d69 6e20 3d20 6e70  "].    tmin = np
+00015370: 2e6d 696e 2874 7769 6e29 0a0a 2020 2020  .min(twin)..    
+00015380: 2320 7061 7261 6d65 7465 7220 696e 6974  # parameter init
+00015390: 6961 6c69 7a65 0a20 2020 2064 656c 7461  ialize.    delta
+000153a0: 5f74 203d 205b 5d0a 2020 2020 6465 6c74  _t = [].    delt
+000153b0: 615f 745f 636f 6566 203d 205b 5d0a 2020  a_t_coef = [].  
+000153c0: 2020 7469 6d65 5f61 7869 7320 3d20 5b5d    time_axis = []
+000153d0: 0a0a 2020 2020 2320 696e 666f 206f 6e20  ..    # info on 
+000153e0: 7468 6520 6d6f 7669 6e67 2077 696e 646f  the moving windo
+000153f0: 770a 2020 2020 7769 6e64 6f77 5f6c 656e  w.    window_len
+00015400: 6774 685f 7361 6d70 6c65 7320 3d20 6e70  gth_samples = np
+00015410: 2e69 6e74 286d 6f76 696e 675f 7769 6e64  .int(moving_wind
+00015420: 6f77 5f6c 656e 6774 6820 2f20 6474 290a  ow_length / dt).
+00015430: 2020 2020 636f 756e 7420 3d20 300a 2020      count = 0.  
+00015440: 2020 7470 203d 2063 6f73 696e 655f 7461    tp = cosine_ta
+00015450: 7065 7228 7769 6e64 6f77 5f6c 656e 6774  per(window_lengt
+00015460: 685f 7361 6d70 6c65 732c 2030 2e31 3529  h_samples, 0.15)
+00015470: 0a0a 2020 2020 6d69 6e69 6e64 203d 2030  ..    minind = 0
+00015480: 0a20 2020 206d 6178 696e 6420 3d20 7769  .    maxind = wi
+00015490: 6e64 6f77 5f6c 656e 6774 685f 7361 6d70  ndow_length_samp
+000154a0: 6c65 730a 0a20 2020 2023 206c 6f6f 7020  les..    # loop 
+000154b0: 7468 726f 7567 6820 616c 6c20 7375 622d  through all sub-
+000154c0: 7769 6e64 6f77 730a 2020 2020 7768 696c  windows.    whil
+000154d0: 6520 6d61 7869 6e64 203c 3d20 6c65 6e28  e maxind <= len(
+000154e0: 7265 6629 3a0a 2020 2020 2020 2020 6363  ref):.        cc
+000154f0: 6920 3d20 6375 725b 6d69 6e69 6e64 3a6d  i = cur[minind:m
+00015500: 6178 696e 645d 0a20 2020 2020 2020 2063  axind].        c
+00015510: 6369 203d 2073 6369 7079 2e73 6967 6e61  ci = scipy.signa
+00015520: 6c2e 6465 7472 656e 6428 6363 692c 2074  l.detrend(cci, t
+00015530: 7970 653d 226c 696e 6561 7222 290a 2020  ype="linear").  
+00015540: 2020 2020 2020 6363 6920 2a3d 2074 700a        cci *= tp.
+00015550: 0a20 2020 2020 2020 2063 7269 203d 2072  .        cri = r
+00015560: 6566 5b6d 696e 696e 643a 6d61 7869 6e64  ef[minind:maxind
+00015570: 5d0a 2020 2020 2020 2020 6372 6920 3d20  ].        cri = 
+00015580: 7363 6970 792e 7369 676e 616c 2e64 6574  scipy.signal.det
+00015590: 7265 6e64 2863 7269 2c20 7479 7065 3d22  rend(cri, type="
+000155a0: 6c69 6e65 6172 2229 0a20 2020 2020 2020  linear").       
+000155b0: 2063 7269 202a 3d20 7470 0a0a 2020 2020   cri *= tp..    
+000155c0: 2020 2020 6d69 6e69 6e64 202b 3d20 696e      minind += in
+000155d0: 7428 736c 6964 655f 7374 6570 202f 2064  t(slide_step / d
+000155e0: 7429 0a20 2020 2020 2020 206d 6178 696e  t).        maxin
+000155f0: 6420 2b3d 2069 6e74 2873 6c69 6465 5f73  d += int(slide_s
+00015600: 7465 7020 2f20 6474 290a 0a20 2020 2020  tep / dt)..     
+00015610: 2020 2023 206e 6f72 6d61 6c69 7a65 2073     # normalize s
+00015620: 6967 6e61 6c73 2062 6566 6f72 6520 6372  ignals before cr
+00015630: 6f73 7320 636f 7272 656c 6174 696f 6e0a  oss correlation.
+00015640: 2020 2020 2020 2020 6363 6920 3d20 2863          cci = (c
+00015650: 6369 202d 2063 6369 2e6d 6561 6e28 2929  ci - cci.mean())
+00015660: 202f 2063 6369 2e73 7464 2829 0a20 2020   / cci.std().   
+00015670: 2020 2020 2063 7269 203d 2028 6372 6920       cri = (cri 
+00015680: 2d20 6372 692e 6d65 616e 2829 2920 2f20  - cri.mean()) / 
+00015690: 6372 692e 7374 6428 290a 0a20 2020 2020  cri.std()..     
+000156a0: 2020 2023 2067 6574 206d 6178 696d 756d     # get maximum
+000156b0: 2063 6f72 7265 6c61 7469 6f6e 2063 6f65   correlation coe
+000156c0: 6666 6963 6965 6e74 2061 6e64 2069 7473  fficient and its
+000156d0: 2069 6e64 6578 0a20 2020 2020 2020 2063   index.        c
+000156e0: 6332 203d 206e 702e 636f 7272 656c 6174  c2 = np.correlat
+000156f0: 6528 6363 692c 2063 7269 2c20 6d6f 6465  e(cci, cri, mode
+00015700: 3d22 7361 6d65 2229 0a20 2020 2020 2020  ="same").       
+00015710: 2063 6332 203d 2063 6332 202f 206e 702e   cc2 = cc2 / np.
+00015720: 7371 7274 2828 6363 692a 2a32 292e 7375  sqrt((cci**2).su
+00015730: 6d28 2920 2a20 2863 7269 2a2a 3229 2e73  m() * (cri**2).s
+00015740: 756d 2829 290a 0a20 2020 2020 2020 2069  um())..        i
+00015750: 6d61 7863 6332 203d 206e 702e 7768 6572  maxcc2 = np.wher
+00015760: 6528 6363 3220 3d3d 206e 702e 6d61 7828  e(cc2 == np.max(
+00015770: 6363 3229 295b 305d 0a20 2020 2020 2020  cc2))[0].       
+00015780: 206d 6178 6363 3220 3d20 6e70 2e6d 6178   maxcc2 = np.max
+00015790: 2863 6332 290a 0a20 2020 2020 2020 2023  (cc2)..        #
+000157a0: 2067 6574 2074 6865 2074 696d 6520 7368   get the time sh
+000157b0: 6966 740a 2020 2020 2020 2020 6d20 3d20  ift.        m = 
+000157c0: 2869 6d61 7863 6332 202d 2028 286d 6178  (imaxcc2 - ((max
+000157d0: 696e 6420 2d20 6d69 6e69 6e64 2920 2f2f  ind - minind) //
+000157e0: 2032 2929 202a 2064 740a 2020 2020 2020   2)) * dt.      
+000157f0: 2020 6465 6c74 615f 742e 6170 7065 6e64    delta_t.append
+00015800: 286d 290a 2020 2020 2020 2020 6465 6c74  (m).        delt
+00015810: 615f 745f 636f 6566 2e61 7070 656e 6428  a_t_coef.append(
+00015820: 6d61 7863 6332 290a 0a20 2020 2020 2020  maxcc2)..       
+00015830: 2074 696d 655f 6178 6973 2e61 7070 656e   time_axis.appen
+00015840: 6428 746d 696e 202b 206d 6f76 696e 675f  d(tmin + moving_
+00015850: 7769 6e64 6f77 5f6c 656e 6774 6820 2f20  window_length / 
+00015860: 322e 3020 2b20 636f 756e 7420 2a20 736c  2.0 + count * sl
+00015870: 6964 655f 7374 6570 290a 2020 2020 2020  ide_step).      
+00015880: 2020 636f 756e 7420 2b3d 2031 0a0a 2020    count += 1..  
+00015890: 2020 6465 6c20 6363 692c 2063 7269 2c20    del cci, cri, 
+000158a0: 6363 322c 2069 6d61 7863 6332 2c20 6d61  cc2, imaxcc2, ma
+000158b0: 7863 6332 0a20 2020 2064 656c 206d 0a0a  xcc2.    del m..
+000158c0: 2020 2020 6966 206d 6178 696e 6420 3e20      if maxind > 
+000158d0: 6c65 6e28 6375 7229 202b 2069 6e74 2873  len(cur) + int(s
+000158e0: 6c69 6465 5f73 7465 7020 2f20 6474 293a  lide_step / dt):
+000158f0: 0a20 2020 2020 2020 2070 7269 6e74 2822  .        print("
+00015900: 5468 6520 6c61 7374 2077 696e 646f 7720  The last window 
+00015910: 7761 7320 746f 6f20 736d 616c 6c2c 2062  was too small, b
+00015920: 7574 2077 6173 2063 6f6d 7075 7465 6422  ut was computed"
+00015930: 290a 0a20 2020 2064 656c 7461 5f74 203d  )..    delta_t =
+00015940: 206e 702e 6172 7261 7928 6465 6c74 615f   np.array(delta_
+00015950: 7429 0a20 2020 2064 656c 7461 5f74 5f63  t).    delta_t_c
+00015960: 6f65 6620 3d20 6e70 2e61 7272 6179 2864  oef = np.array(d
+00015970: 656c 7461 5f74 5f63 6f65 6629 0a20 2020  elta_t_coef).   
+00015980: 2074 696d 655f 6178 6973 203d 206e 702e   time_axis = np.
+00015990: 6172 7261 7928 7469 6d65 5f61 7869 7329  array(time_axis)
+000159a0: 0a0a 2020 2020 2320 6c69 6e65 6172 2072  ..    # linear r
+000159b0: 6567 7265 7373 696f 6e20 746f 2067 6574  egression to get
+000159c0: 2064 762f 760a 2020 2020 6966 2063 6f75   dv/v.    if cou
+000159d0: 6e74 203e 2032 3a0a 2020 2020 2020 2020  nt > 2:.        
+000159e0: 2320 7369 6d70 6c65 2077 6569 6768 740a  # simple weight.
+000159f0: 2020 2020 2020 2020 7720 3d20 6e70 2e6f          w = np.o
+00015a00: 6e65 7328 636f 756e 7429 0a20 2020 2020  nes(count).     
+00015a10: 2020 2023 206d 2c20 612c 2065 6d2c 2065     # m, a, em, e
+00015a20: 6120 3d20 6c69 6e65 6172 5f72 6567 7265  a = linear_regre
+00015a30: 7373 696f 6e28 7469 6d65 5f61 7869 735b  ssion(time_axis[
+00015a40: 696e 6478 5d2c 2064 656c 7461 5f74 5b69  indx], delta_t[i
+00015a50: 6e64 785d 2c20 772c 2069 6e74 6572 6365  ndx], w, interce
+00015a60: 7074 5f6f 7269 6769 6e3d 4661 6c73 6529  pt_origin=False)
+00015a70: 0a20 2020 2020 2020 206d 302c 2065 6d30  .        m0, em0
+00015a80: 203d 206c 696e 6561 725f 7265 6772 6573   = linear_regres
+00015a90: 7369 6f6e 2874 696d 655f 6178 6973 2e66  sion(time_axis.f
+00015aa0: 6c61 7474 656e 2829 2c20 6465 6c74 615f  latten(), delta_
+00015ab0: 742e 666c 6174 7465 6e28 292c 2077 2e66  t.flatten(), w.f
+00015ac0: 6c61 7474 656e 2829 2c20 696e 7465 7263  latten(), interc
+00015ad0: 6570 745f 6f72 6967 696e 3d54 7275 6529  ept_origin=True)
+00015ae0: 0a0a 2020 2020 656c 7365 3a0a 2020 2020  ..    else:.    
+00015af0: 2020 2020 7072 696e 7428 226e 6f74 2065      print("not e
+00015b00: 6e6f 7567 6820 706f 696e 7473 2074 6f20  nough points to 
+00015b10: 6573 7469 6d61 7465 2064 762f 7620 666f  estimate dv/v fo
+00015b20: 7220 7763 6322 290a 2020 2020 2020 2020  r wcc").        
+00015b30: 6d30 203d 2030 0a20 2020 2020 2020 2065  m0 = 0.        e
+00015b40: 6d30 203d 2030 0a0a 2020 2020 7265 7475  m0 = 0..    retu
+00015b50: 726e 202d 6d30 202a 2031 3030 2c20 656d  rn -m0 * 100, em
+00015b60: 3020 2a20 3130 300a 0a0a 6465 6620 7778  0 * 100...def wx
+00015b70: 735f 6476 7628 0a20 2020 2072 6566 2c0a  s_dvv(.    ref,.
+00015b80: 2020 2020 6375 722c 0a20 2020 2061 6c6c      cur,.    all
+00015b90: 6672 6571 2c0a 2020 2020 7061 7261 2c0a  freq,.    para,.
+00015ba0: 2020 2020 646a 3d31 202f 2031 322c 0a20      dj=1 / 12,. 
+00015bb0: 2020 2073 303d 2d31 2c0a 2020 2020 4a3d     s0=-1,.    J=
+00015bc0: 2d31 2c0a 2020 2020 7369 673d 4661 6c73  -1,.    sig=Fals
+00015bd0: 652c 0a20 2020 2077 766e 3d22 6d6f 726c  e,.    wvn="morl
+00015be0: 6574 222c 0a20 2020 2075 6e77 7261 7066  et",.    unwrapf
+00015bf0: 6c61 673d 4661 6c73 652c 0a29 3a0a 2020  lag=False,.):.  
+00015c00: 2020 2222 220a 2020 2020 436f 6d70 7574    """.    Comput
+00015c10: 6520 6474 206f 7220 6476 2f76 2069 6e20  e dt or dv/v in 
+00015c20: 7469 6d65 2061 6e64 2066 7265 7175 656e  time and frequen
+00015c30: 6379 2064 6f6d 6169 6e20 6672 6f6d 2077  cy domain from w
+00015c40: 6176 656c 6574 2063 726f 7373 2073 7065  avelet cross spe
+00015c50: 6374 7275 6d20 2877 7873 292e 0a20 2020  ctrum (wxs)..   
+00015c60: 2066 6f72 2061 6c6c 2066 7265 7175 6563   for all frequec
+00015c70: 6965 7320 696e 2061 6e20 696e 7465 7265  ies in an intere
+00015c80: 7374 2072 616e 6765 0a0a 2020 2020 5061  st range..    Pa
+00015c90: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+00015ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
+00015cb0: 7265 663a 2054 6865 2022 5265 6665 7265  ref: The "Refere
+00015cc0: 6e63 6522 2074 696d 6573 6572 6965 7320  nce" timeseries 
+00015cd0: 286e 756d 7079 2e6e 6461 7272 6179 290a  (numpy.ndarray).
+00015ce0: 2020 2020 6375 723a 2054 6865 2022 4375      cur: The "Cu
+00015cf0: 7272 656e 7422 2074 696d 6573 6572 6965  rrent" timeserie
+00015d00: 7320 286e 756d 7079 2e6e 6461 7272 6179  s (numpy.ndarray
+00015d10: 290a 2020 2020 616c 6c66 7265 713a 2061  ).    allfreq: a
+00015d20: 2062 6f6f 6c65 6e20 7661 7269 6162 6c65   boolen variable
+00015d30: 2074 6f20 6d61 6b65 206d 6561 7375 7265   to make measure
+00015d40: 6d65 6e74 7320 6f6e 2061 6c6c 2066 7265  ments on all fre
+00015d50: 7175 656e 6379 2072 616e 6765 206f 7220  quency range or 
+00015d60: 6e6f 740a 2020 2020 7061 7261 3a20 6120  not.    para: a 
+00015d70: 6469 6374 2063 6f6e 7461 696e 696e 6720  dict containing 
+00015d80: 6672 6571 2f74 696d 6520 696e 666f 206f  freq/time info o
+00015d90: 6620 7468 6520 6461 7461 206d 6174 7269  f the data matri
+00015da0: 780a 2020 2020 646a 2c20 7330 2c20 4a2c  x.    dj, s0, J,
+00015db0: 2073 6967 2c20 7776 6e3a 2063 6f6d 6d6f   sig, wvn: commo
+00015dc0: 6e20 7061 7261 6d65 7465 7273 2075 7365  n parameters use
+00015dd0: 6420 696e 2027 7761 7665 6c65 742e 7763  d in 'wavelet.wc
+00015de0: 7427 0a20 2020 2075 6e77 7261 7066 6c61  t'.    unwrapfla
+00015df0: 673a 2054 7275 6520 2d20 756e 7772 6170  g: True - unwrap
+00015e00: 2070 6861 7365 2064 656c 6179 732e 2044   phase delays. D
+00015e10: 6566 6175 6c74 2069 7320 4661 6c73 650a  efault is False.
+00015e20: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
+00015e30: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+00015e40: 2d2d 2d2d 0a20 2020 2064 7676 2a31 3030  ----.    dvv*100
+00015e50: 203a 2065 7374 696d 6174 6564 2064 762f   : estimated dv/
+00015e60: 7620 696e 2025 0a20 2020 2065 7272 2a31  v in %.    err*1
+00015e70: 3030 203a 2065 7272 6f72 206f 6620 6476  00 : error of dv
+00015e80: 2f76 2065 7374 696d 6174 696f 6e20 696e  /v estimation in
+00015e90: 2025 0a0a 2020 2020 4f72 6967 696e 616c   %..    Original
+00015ea0: 6c79 2077 7269 7474 656e 2062 7920 5469  ly written by Ti
+00015eb0: 6d20 436c 656d 656e 7473 2028 3120 4d61  m Clements (1 Ma
+00015ec0: 7263 682c 2032 3031 3929 0a20 2020 204d  rch, 2019).    M
+00015ed0: 6f64 6966 6965 6420 6279 2043 6f6e 6763  odified by Congc
+00015ee0: 6f6e 6720 5975 616e 2028 3330 204a 756e  ong Yuan (30 Jun
+00015ef0: 652c 2032 3031 3929 2062 6173 6564 206f  e, 2019) based o
+00015f00: 6e20 284d 616f 2065 7420 616c 2e20 3230  n (Mao et al. 20
+00015f10: 3139 292e 0a20 2020 2055 7064 6174 6564  19)..    Updated
+00015f20: 2062 7920 4368 656e 6778 696e 204a 6961   by Chengxin Jia
+00015f30: 6e67 2028 3130 204f 6374 2c20 3230 3139  ng (10 Oct, 2019
+00015f40: 2920 746f 206d 6572 6765 2074 6865 2066  ) to merge the f
+00015f50: 756e 6374 696f 6e61 6c69 7479 2066 6f72  unctionality for
+00015f60: 206d 6573 7572 656d 656e 7473 0a20 2020   mesurements.   
+00015f70: 2061 6372 6f73 7320 616c 6c20 6672 6571   across all freq
+00015f80: 7565 6e63 7920 616e 6420 6f6e 6520 6672  uency and one fr
+00015f90: 6571 2072 616e 6765 0a20 2020 2022 2222  eq range.    """
+00015fa0: 0a20 2020 2023 2063 6f6d 6d6f 6e20 7661  .    # common va
+00015fb0: 7269 6162 6c65 730a 2020 2020 7477 696e  riables.    twin
+00015fc0: 203d 2070 6172 615b 2274 7769 6e22 5d0a   = para["twin"].
+00015fd0: 2020 2020 6672 6571 203d 2070 6172 615b      freq = para[
+00015fe0: 2266 7265 7122 5d0a 2020 2020 6474 203d  "freq"].    dt =
+00015ff0: 2070 6172 615b 2264 7422 5d0a 2020 2020   para["dt"].    
+00016000: 746d 696e 203d 206e 702e 6d69 6e28 7477  tmin = np.min(tw
+00016010: 696e 290a 2020 2020 746d 6178 203d 206e  in).    tmax = n
+00016020: 702e 6d61 7828 7477 696e 290a 2020 2020  p.max(twin).    
+00016030: 666d 696e 203d 206e 702e 6d69 6e28 6672  fmin = np.min(fr
+00016040: 6571 290a 2020 2020 666d 6178 203d 206e  eq).    fmax = n
+00016050: 702e 6d61 7828 6672 6571 290a 2020 2020  p.max(freq).    
+00016060: 7476 6563 203d 206e 702e 6172 616e 6765  tvec = np.arange
+00016070: 2874 6d69 6e2c 2074 6d61 782c 2064 7429  (tmin, tmax, dt)
+00016080: 0a20 2020 206e 7074 7320 3d20 6c65 6e28  .    npts = len(
+00016090: 7476 6563 290a 0a20 2020 2023 2070 6572  tvec)..    # per
+000160a0: 666f 726d 2063 726f 7373 2063 6f68 6572  form cross coher
+000160b0: 656e 7420 616e 616c 7973 6973 2c20 6d6f  ent analysis, mo
+000160c0: 6469 6669 6564 2066 726f 6d20 6675 6e63  dified from func
+000160d0: 7469 6f6e 2027 7761 7665 6c65 742e 6377  tion 'wavelet.cw
+000160e0: 7427 0a20 2020 2057 4354 2c20 6157 4354  t'.    WCT, aWCT
+000160f0: 2c20 636f 692c 2066 7265 712c 2073 6967  , coi, freq, sig
+00016100: 203d 2077 6374 5f6d 6f64 6966 6965 6428   = wct_modified(
+00016110: 7265 662c 2063 7572 2c20 6474 2c20 646a  ref, cur, dt, dj
+00016120: 3d64 6a2c 2073 303d 7330 2c20 4a3d 4a2c  =dj, s0=s0, J=J,
+00016130: 2073 6967 3d73 6967 2c20 7761 7665 6c65   sig=sig, wavele
+00016140: 743d 7776 6e2c 206e 6f72 6d61 6c69 7a65  t=wvn, normalize
+00016150: 3d54 7275 6529 0a0a 2020 2020 6966 2075  =True)..    if u
+00016160: 6e77 7261 7066 6c61 673a 0a20 2020 2020  nwrapflag:.     
+00016170: 2020 2070 6861 7365 203d 206e 702e 756e     phase = np.un
+00016180: 7772 6170 2861 5743 542c 2061 7869 733d  wrap(aWCT, axis=
+00016190: 2d31 2920 2023 2061 7869 733d 302c 2075  -1)  # axis=0, u
+000161a0: 7077 7261 7020 616c 6f6e 6720 7469 6d65  pwrap along time
+000161b0: 3b20 6178 6973 3d2d 312c 2075 6e77 7261  ; axis=-1, unwra
+000161c0: 7020 616c 6f6e 6720 6672 6571 7565 6e63  p along frequenc
+000161d0: 790a 2020 2020 656c 7365 3a0a 2020 2020  y.    else:.    
+000161e0: 2020 2020 7068 6173 6520 3d20 6157 4354      phase = aWCT
+000161f0: 0a0a 2020 2020 2320 7a65 726f 206f 7574  ..    # zero out
+00016200: 2064 6174 6120 6f75 7473 6964 6520 6672   data outside fr
+00016210: 6571 7565 6e63 7920 6261 6e64 0a20 2020  equency band.   
+00016220: 2069 6620 2866 6d61 7820 3e20 6e70 2e6d   if (fmax > np.m
+00016230: 6178 2866 7265 7129 2920 7c20 2866 6d61  ax(freq)) | (fma
+00016240: 7820 3c3d 2066 6d69 6e29 3a0a 2020 2020  x <= fmin):.    
+00016250: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00016260: 7272 6f72 2822 4162 6f72 743a 2069 6e70  rror("Abort: inp
+00016270: 7574 2066 7265 7175 656e 6379 206f 7574  ut frequency out
+00016280: 206f 6620 6c69 6d69 7473 2122 290a 2020   of limits!").  
+00016290: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000162a0: 6672 6571 5f69 6e64 696e 203d 206e 702e  freq_indin = np.
+000162b0: 7768 6572 6528 2866 7265 7120 3e3d 2066  where((freq >= f
+000162c0: 6d69 6e29 2026 2028 6672 6571 203c 3d20  min) & (freq <= 
+000162d0: 666d 6178 2929 5b30 5d0a 0a20 2020 2023  fmax))[0]..    #
+000162e0: 2066 6f6c 6c6f 7720 4d57 4353 2074 6f20   follow MWCS to 
+000162f0: 646f 2074 776f 2073 7465 7073 206f 6620  do two steps of 
+00016300: 6c69 6e65 6172 2072 6567 7265 7373 696f  linear regressio
+00016310: 6e0a 2020 2020 6966 206e 6f74 2061 6c6c  n.    if not all
+00016320: 6672 6571 3a0a 2020 2020 2020 2020 6465  freq:.        de
+00016330: 6c74 615f 745f 6d2c 2064 656c 7461 5f74  lta_t_m, delta_t
+00016340: 5f75 6e63 203d 206e 702e 7a65 726f 7328  _unc = np.zeros(
+00016350: 6e70 7473 2c20 6474 7970 653d 6e70 2e66  npts, dtype=np.f
+00016360: 6c6f 6174 3332 292c 206e 702e 7a65 726f  loat32), np.zero
+00016370: 7328 6e70 7473 2c20 6474 7970 653d 6e70  s(npts, dtype=np
+00016380: 2e66 6c6f 6174 3332 290a 2020 2020 2020  .float32).      
+00016390: 2020 2320 6173 7375 6d65 2074 6865 2074    # assume the t
+000163a0: 7665 6320 6973 2074 6865 2074 696d 6520  vec is the time 
+000163b0: 7769 6e64 6f77 2074 6f20 6d65 6173 7572  window to measur
+000163c0: 6520 6474 0a20 2020 2020 2020 2066 6f72  e dt.        for
+000163d0: 2069 7420 696e 2072 616e 6765 286e 7074   it in range(npt
+000163e0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+000163f0: 7720 3d20 3120 2f20 5743 545b 6672 6571  w = 1 / WCT[freq
+00016400: 5f69 6e64 696e 2c20 6974 5d0a 2020 2020  _indin, it].    
+00016410: 2020 2020 2020 2020 775b 7e6e 702e 6973          w[~np.is
+00016420: 6669 6e69 7465 2877 295d 203d 2031 2e30  finite(w)] = 1.0
+00016430: 0a20 2020 2020 2020 2020 2020 2064 656c  .            del
+00016440: 7461 5f74 5f6d 5b69 745d 2c20 6465 6c74  ta_t_m[it], delt
+00016450: 615f 745f 756e 635b 6974 5d20 3d20 6c69  a_t_unc[it] = li
+00016460: 6e65 6172 5f72 6567 7265 7373 696f 6e28  near_regression(
+00016470: 6672 6571 5b66 7265 715f 696e 6469 6e5d  freq[freq_indin]
+00016480: 202a 2032 202a 206e 702e 7069 2c20 7068   * 2 * np.pi, ph
+00016490: 6173 655b 6672 6571 5f69 6e64 696e 2c20  ase[freq_indin, 
+000164a0: 6974 5d2c 2077 290a 0a20 2020 2020 2020  it], w)..       
+000164b0: 2023 206e 6577 2077 6569 6768 7473 2066   # new weights f
+000164c0: 6f72 2072 6567 7265 7373 696f 6e0a 2020  or regression.  
+000164d0: 2020 2020 2020 7732 203d 2031 202f 206e        w2 = 1 / n
+000164e0: 702e 6d65 616e 2857 4354 5b66 7265 715f  p.mean(WCT[freq_
+000164f0: 696e 6469 6e2c 203a 5d2c 2061 7869 733d  indin, :], axis=
+00016500: 3029 0a20 2020 2020 2020 2077 325b 7e6e  0).        w2[~n
+00016510: 702e 6973 6669 6e69 7465 2877 3229 5d20  p.isfinite(w2)] 
+00016520: 3d20 312e 300a 0a20 2020 2020 2020 2023  = 1.0..        #
+00016530: 206e 6f77 2075 7365 2064 7420 616e 6420   now use dt and 
+00016540: 7420 746f 2067 6574 2064 762f 760a 2020  t to get dv/v.  
+00016550: 2020 2020 2020 6966 206c 656e 2877 3229        if len(w2)
+00016560: 203e 2032 3a0a 2020 2020 2020 2020 2020   > 2:.          
+00016570: 2020 6966 206e 6f74 206e 702e 616e 7928    if not np.any(
+00016580: 6465 6c74 615f 745f 6d29 3a0a 2020 2020  delta_t_m):.    
+00016590: 2020 2020 2020 2020 2020 2020 6476 762c              dvv,
+000165a0: 2065 7272 203d 206e 702e 6e61 6e2c 206e   err = np.nan, n
+000165b0: 702e 6e61 6e0a 2020 2020 2020 2020 2020  p.nan.          
+000165c0: 2020 6d2c 2065 6d20 3d20 6c69 6e65 6172    m, em = linear
+000165d0: 5f72 6567 7265 7373 696f 6e28 7476 6563  _regression(tvec
+000165e0: 2c20 6465 6c74 615f 745f 6d2c 2077 322c  , delta_t_m, w2,
+000165f0: 2069 6e74 6572 6365 7074 5f6f 7269 6769   intercept_origi
+00016600: 6e3d 5472 7565 290a 2020 2020 2020 2020  n=True).        
+00016610: 2020 2020 6476 762c 2065 7272 203d 202d      dvv, err = -
+00016620: 6d2c 2065 6d0a 2020 2020 2020 2020 656c  m, em.        el
+00016630: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00016640: 7072 696e 7428 226e 6f74 2065 6e6f 7567  print("not enoug
+00016650: 6820 706f 696e 7473 2074 6f20 6573 7469  h points to esti
+00016660: 6d61 7465 2064 762f 7620 666f 7220 7774  mate dv/v for wt
+00016670: 7322 290a 2020 2020 2020 2020 2020 2020  s").            
+00016680: 6476 762c 2065 7272 203d 206e 702e 6e61  dvv, err = np.na
+00016690: 6e2c 206e 702e 6e61 6e0a 0a20 2020 2020  n, np.nan..     
+000166a0: 2020 2072 6574 7572 6e20 6476 7620 2a20     return dvv * 
+000166b0: 3130 302c 2065 7272 202a 2031 3030 0a0a  100, err * 100..
+000166c0: 2020 2020 2320 636f 6e76 6572 7420 7068      # convert ph
+000166d0: 6173 6520 6469 7265 6374 6c79 2074 6f20  ase directly to 
+000166e0: 6465 6c74 615f 7420 666f 7220 616c 6c20  delta_t for all 
+000166f0: 6672 6571 7565 6e63 6965 730a 2020 2020  frequencies.    
+00016700: 656c 7365 3a0a 2020 2020 2020 2020 2320  else:.        # 
+00016710: 636f 6e76 6572 7420 7068 6173 6520 6465  convert phase de
+00016720: 6c61 7920 746f 2074 696d 6520 6465 6c61  lay to time dela
+00016730: 790a 2020 2020 2020 2020 6465 6c74 615f  y.        delta_
+00016740: 7420 3d20 7068 6173 6520 2f20 2832 202a  t = phase / (2 *
+00016750: 206e 702e 7069 202a 2066 7265 715b 3a2c   np.pi * freq[:,
+00016760: 204e 6f6e 655d 2920 2023 206e 6f72 6d61   None])  # norma
+00016770: 6c69 7a65 2070 6861 7365 2062 7920 2832  lize phase by (2
+00016780: 2a70 692a 6672 6571 7565 6e63 7929 0a20  *pi*frequency). 
+00016790: 2020 2020 2020 2064 7676 2c20 6572 7220         dvv, err 
+000167a0: 3d20 6e70 2e7a 6572 6f73 2866 7265 715f  = np.zeros(freq_
+000167b0: 696e 6469 6e2e 7368 6170 6529 2c20 6e70  indin.shape), np
+000167c0: 2e7a 6572 6f73 2866 7265 715f 696e 6469  .zeros(freq_indi
+000167d0: 6e2e 7368 6170 6529 0a0a 2020 2020 2020  n.shape)..      
+000167e0: 2020 2320 6c6f 6f70 2074 6872 6f75 6768    # loop through
+000167f0: 2066 7265 7120 666f 7220 6c69 6e65 6172   freq for linear
+00016800: 2072 6567 7265 7373 696f 6e0a 2020 2020   regression.    
+00016810: 2020 2020 666f 7220 6969 2c20 6966 7265      for ii, ifre
+00016820: 7120 696e 2065 6e75 6d65 7261 7465 2866  q in enumerate(f
+00016830: 7265 715f 696e 6469 6e29 3a0a 2020 2020  req_indin):.    
+00016840: 2020 2020 2020 2020 6966 206c 656e 2874          if len(t
+00016850: 7665 6329 203e 2032 3a0a 2020 2020 2020  vec) > 2:.      
+00016860: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00016870: 206e 702e 616e 7928 6465 6c74 615f 745b   np.any(delta_t[
+00016880: 6966 7265 715d 293a 0a20 2020 2020 2020  ifreq]):.       
+00016890: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+000168a0: 7469 6e75 650a 0a20 2020 2020 2020 2020  tinue..         
+000168b0: 2020 2020 2020 2023 2068 6f77 2074 6f20         # how to 
+000168c0: 6265 7474 6572 2061 7070 726f 6163 6820  better approach 
+000168d0: 7468 6520 756e 6365 7274 6169 6e74 7920  the uncertainty 
+000168e0: 6f66 2064 656c 7461 5f74 0a20 2020 2020  of delta_t.     
+000168f0: 2020 2020 2020 2020 2020 2077 203d 2031             w = 1
+00016900: 202f 2057 4354 5b69 6672 6571 5d0a 2020   / WCT[ifreq].  
+00016910: 2020 2020 2020 2020 2020 2020 2020 775b                w[
+00016920: 7e6e 702e 6973 6669 6e69 7465 2877 295d  ~np.isfinite(w)]
+00016930: 203d 2031 2e30 0a0a 2020 2020 2020 2020   = 1.0..        
+00016940: 2020 2020 2020 2020 2320 6d2c 2061 2c20          # m, a, 
+00016950: 656d 2c20 6561 203d 206c 696e 6561 725f  em, ea = linear_
+00016960: 7265 6772 6573 7369 6f6e 2874 696d 655f  regression(time_
+00016970: 6178 6973 5b69 6e64 785d 2c20 6465 6c74  axis[indx], delt
+00016980: 615f 745b 696e 6478 5d2c 2077 2c20 696e  a_t[indx], w, in
+00016990: 7465 7263 6570 745f 6f72 6967 696e 3d46  tercept_origin=F
+000169a0: 616c 7365 290a 2020 2020 2020 2020 2020  alse).          
+000169b0: 2020 2020 2020 6d2c 2065 6d20 3d20 6c69        m, em = li
+000169c0: 6e65 6172 5f72 6567 7265 7373 696f 6e28  near_regression(
+000169d0: 7476 6563 2c20 6465 6c74 615f 745b 6966  tvec, delta_t[if
+000169e0: 7265 715d 2c20 772c 2069 6e74 6572 6365  req], w, interce
+000169f0: 7074 5f6f 7269 6769 6e3d 5472 7565 290a  pt_origin=True).
+00016a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a10: 6476 765b 6969 5d2c 2065 7272 5b69 695d  dvv[ii], err[ii]
+00016a20: 203d 202d 6d2c 2065 6d0a 2020 2020 2020   = -m, em.      
+00016a30: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00016a40: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00016a50: 7428 226e 6f74 2065 6e6f 7567 6820 706f  t("not enough po
+00016a60: 696e 7473 2074 6f20 6573 7469 6d61 7465  ints to estimate
+00016a70: 2064 762f 7620 666f 7220 7774 7322 290a   dv/v for wts").
+00016a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a90: 6476 765b 6969 5d2c 2065 7272 5b69 695d  dvv[ii], err[ii]
+00016aa0: 203d 206e 702e 6e61 6e2c 206e 702e 6e61   = np.nan, np.na
+00016ab0: 6e0a 0a20 2020 2020 2020 2072 6574 7572  n..        retur
+00016ac0: 6e20 6672 6571 5b66 7265 715f 696e 6469  n freq[freq_indi
+00016ad0: 6e5d 2c20 6476 7620 2a20 3130 302c 2065  n], dvv * 100, e
+00016ae0: 7272 202a 2031 3030 0a0a 0a64 6566 2077  rr * 100...def w
+00016af0: 7473 5f64 7676 280a 2020 2020 7265 662c  ts_dvv(.    ref,
+00016b00: 0a20 2020 2063 7572 2c0a 2020 2020 616c  .    cur,.    al
+00016b10: 6c66 7265 712c 0a20 2020 2070 6172 612c  lfreq,.    para,
+00016b20: 0a20 2020 2064 765f 7261 6e67 652c 0a20  .    dv_range,. 
+00016b30: 2020 206e 6274 7269 616c 2c0a 2020 2020     nbtrial,.    
+00016b40: 646a 3d31 202f 2031 322c 0a20 2020 2073  dj=1 / 12,.    s
+00016b50: 303d 2d31 2c0a 2020 2020 4a3d 2d31 2c0a  0=-1,.    J=-1,.
+00016b60: 2020 2020 7776 6e3d 226d 6f72 6c65 7422      wvn="morlet"
+00016b70: 2c0a 2020 2020 6e6f 726d 616c 697a 653d  ,.    normalize=
+00016b80: 5472 7565 2c0a 293a 0a20 2020 2022 2222  True,.):.    """
+00016b90: 0a20 2020 2041 7070 6c79 2073 7472 6574  .    Apply stret
+00016ba0: 6368 696e 6720 6d65 7468 6f64 2074 6f20  ching method to 
+00016bb0: 636f 6e74 696e 756f 7573 2077 6176 656c  continuous wavel
+00016bc0: 6574 2074 7261 6e73 666f 726d 6174 696f  et transformatio
+00016bd0: 6e20 2843 5754 2920 6f66 2073 6967 6e61  n (CWT) of signa
+00016be0: 6c73 0a20 2020 2066 6f72 2061 6c6c 2066  ls.    for all f
+00016bf0: 7265 7175 6563 6965 7320 696e 2061 6e20  requecies in an 
+00016c00: 696e 7465 7265 7374 2072 616e 6765 0a0a  interest range..
+00016c10: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00016c20: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00016c30: 2d0a 2020 2020 7265 663a 2054 6865 2022  -.    ref: The "
+00016c40: 5265 6665 7265 6e63 6522 2074 696d 6573  Reference" times
+00016c50: 6572 6965 7320 286e 756d 7079 2e6e 6461  eries (numpy.nda
+00016c60: 7272 6179 290a 2020 2020 6375 723a 2054  rray).    cur: T
+00016c70: 6865 2022 4375 7272 656e 7422 2074 696d  he "Current" tim
+00016c80: 6573 6572 6965 7320 286e 756d 7079 2e6e  eseries (numpy.n
+00016c90: 6461 7272 6179 290a 2020 2020 616c 6c66  darray).    allf
+00016ca0: 7265 713a 2061 2062 6f6f 6c65 6e20 7661  req: a boolen va
+00016cb0: 7269 6162 6c65 2074 6f20 6d61 6b65 206d  riable to make m
+00016cc0: 6561 7375 7265 6d65 6e74 7320 6f6e 2061  easurements on a
+00016cd0: 6c6c 2066 7265 7175 656e 6379 2072 616e  ll frequency ran
+00016ce0: 6765 206f 7220 6e6f 740a 2020 2020 7061  ge or not.    pa
+00016cf0: 7261 3a20 6120 6469 6374 2063 6f6e 7461  ra: a dict conta
+00016d00: 696e 696e 6720 6672 6571 2f74 696d 6520  ining freq/time 
+00016d10: 696e 666f 206f 6620 7468 6520 6461 7461  info of the data
+00016d20: 206d 6174 7269 780a 2020 2020 6476 5f72   matrix.    dv_r
+00016d30: 616e 6765 3a20 6162 736f 6c75 7465 2062  ange: absolute b
+00016d40: 6f75 6e64 2066 6f72 2074 6865 2076 656c  ound for the vel
+00016d50: 6f63 6974 7920 7661 7269 6174 696f 6e3b  ocity variation;
+00016d60: 2065 7861 6d70 6c65 3a20 6476 3d30 2e30   example: dv=0.0
+00016d70: 3320 666f 7220 5b2d 332c 335d 250a 2020  3 for [-3,3]%.  
+00016d80: 2020 6f66 2072 656c 6174 6976 6520 7665    of relative ve
+00016d90: 6c6f 6369 7479 2063 6861 6e67 6520 2866  locity change (f
+00016da0: 6c6f 6174 290a 2020 2020 6e62 7472 6961  loat).    nbtria
+00016db0: 6c3a 206e 756d 6265 7220 6f66 2073 7472  l: number of str
+00016dc0: 6574 6368 696e 6720 636f 6566 6669 6369  etching coeffici
+00016dd0: 656e 7420 6265 7477 6565 6e20 6476 6d69  ent between dvmi
+00016de0: 6e20 616e 6420 6476 6d61 782c 206e 6f20  n and dvmax, no 
+00016df0: 6e65 6564 2074 6f20 6265 2068 6967 6865  need to be highe
+00016e00: 7220 7468 616e 2031 3030 2020 2866 6c6f  r than 100  (flo
+00016e10: 6174 290a 2020 2020 646a 2c20 7330 2c20  at).    dj, s0, 
+00016e20: 4a2c 2073 6967 2c20 7776 6e3a 2063 6f6d  J, sig, wvn: com
+00016e30: 6d6f 6e20 7061 7261 6d65 7465 7273 2075  mon parameters u
+00016e40: 7365 6420 696e 2027 7761 7665 6c65 742e  sed in 'wavelet.
+00016e50: 7763 7427 0a20 2020 206e 6f72 6d61 6c69  wct'.    normali
+00016e60: 7a65 3a20 6e6f 726d 616c 697a 6520 7468  ze: normalize th
+00016e70: 6520 7761 7665 6c65 7420 7370 6563 7472  e wavelet spectr
+00016e80: 756d 206f 7220 6e6f 742e 2044 6566 6175  um or not. Defau
+00016e90: 6c74 2069 7320 5472 7565 0a0a 2020 2020  lt is True..    
+00016ea0: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
+00016eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00016ec0: 2020 2020 6476 763a 2065 7374 696d 6174      dvv: estimat
+00016ed0: 6564 2064 762f 760a 2020 2020 6572 723a  ed dv/v.    err:
+00016ee0: 2065 7272 6f72 206f 6620 6476 2f76 2065   error of dv/v e
+00016ef0: 7374 696d 6174 696f 6e0a 0a20 2020 2057  stimation..    W
+00016f00: 7269 7474 656e 2062 7920 436f 6e67 636f  ritten by Congco
+00016f10: 6e67 2059 7561 6e20 2833 3020 4a75 6e2c  ng Yuan (30 Jun,
+00016f20: 2032 3031 3929 0a20 2020 2022 2222 0a20   2019).    """. 
+00016f30: 2020 2023 2063 6f6d 6d6f 6e20 7661 7269     # common vari
+00016f40: 6162 6c65 730a 2020 2020 6672 6571 203d  ables.    freq =
+00016f50: 2070 6172 615b 2266 7265 7122 5d0a 2020   para["freq"].  
+00016f60: 2020 6474 203d 2070 6172 615b 2264 7422    dt = para["dt"
+00016f70: 5d0a 2020 2020 666d 696e 203d 206e 702e  ].    fmin = np.
+00016f80: 6d69 6e28 6672 6571 290a 2020 2020 666d  min(freq).    fm
+00016f90: 6178 203d 206e 702e 6d61 7828 6672 6571  ax = np.max(freq
+00016fa0: 290a 0a20 2020 2023 2061 7070 6c79 2063  )..    # apply c
+00016fb0: 7774 206f 6e20 7477 6f20 7472 6163 6573  wt on two traces
+00016fc0: 0a20 2020 2063 7774 312c 2073 6a2c 2066  .    cwt1, sj, f
+00016fd0: 7265 712c 2063 6f69 2c20 5f2c 205f 203d  req, coi, _, _ =
+00016fe0: 2070 7963 7774 2e63 7774 2863 7572 2c20   pycwt.cwt(cur, 
+00016ff0: 6474 2c20 646a 2c20 7330 2c20 4a2c 2077  dt, dj, s0, J, w
+00017000: 766e 290a 2020 2020 6377 7432 2c20 736a  vn).    cwt2, sj
+00017010: 2c20 6672 6571 2c20 636f 692c 205f 2c20  , freq, coi, _, 
+00017020: 5f20 3d20 7079 6377 742e 6377 7428 7265  _ = pycwt.cwt(re
+00017030: 662c 2064 742c 2064 6a2c 2073 302c 204a  f, dt, dj, s0, J
+00017040: 2c20 7776 6e29 0a0a 2020 2020 2320 6578  , wvn)..    # ex
+00017050: 7472 6163 7420 7265 616c 2076 616c 7565  tract real value
+00017060: 7320 6f66 2063 7774 0a20 2020 2072 6377  s of cwt.    rcw
+00017070: 7431 2c20 7263 7774 3220 3d20 6e70 2e72  t1, rcwt2 = np.r
+00017080: 6561 6c28 6377 7431 292c 206e 702e 7265  eal(cwt1), np.re
+00017090: 616c 2863 7774 3229 0a0a 2020 2020 2320  al(cwt2)..    # 
+000170a0: 7a65 726f 206f 7574 2064 6174 6120 6f75  zero out data ou
+000170b0: 7473 6964 6520 6672 6571 7565 6e63 7920  tside frequency 
+000170c0: 6261 6e64 0a20 2020 2069 6620 2866 6d61  band.    if (fma
+000170d0: 7820 3e20 6e70 2e6d 6178 2866 7265 7129  x > np.max(freq)
+000170e0: 2920 7c20 2866 6d61 7820 3c3d 2066 6d69  ) | (fmax <= fmi
+000170f0: 6e29 3a0a 2020 2020 2020 2020 7261 6973  n):.        rais
+00017100: 6520 5661 6c75 6545 7272 6f72 2822 4162  e ValueError("Ab
+00017110: 6f72 743a 2069 6e70 7574 2066 7265 7175  ort: input frequ
+00017120: 656e 6379 206f 7574 206f 6620 6c69 6d69  ency out of limi
+00017130: 7473 2122 290a 2020 2020 656c 7365 3a0a  ts!").    else:.
+00017140: 2020 2020 2020 2020 6672 6571 5f69 6e64          freq_ind
+00017150: 696e 203d 206e 702e 7768 6572 6528 2866  in = np.where((f
+00017160: 7265 7120 3e3d 2066 6d69 6e29 2026 2028  req >= fmin) & (
+00017170: 6672 6571 203c 3d20 666d 6178 2929 5b30  freq <= fmax))[0
+00017180: 5d0a 0a20 2020 2023 2063 6f6e 7665 7274  ]..    # convert
+00017190: 2077 6176 656c 6574 2064 6f6d 6169 6e20   wavelet domain 
+000171a0: 6261 636b 2074 6f20 7469 6d65 2064 6f6d  back to time dom
+000171b0: 6169 6e20 287e 6669 6c74 6572 696e 6729  ain (~filtering)
+000171c0: 0a20 2020 2069 6620 6e6f 7420 616c 6c66  .    if not allf
+000171d0: 7265 713a 0a20 2020 2020 2020 2023 2069  req:.        # i
+000171e0: 6e76 6572 7365 2063 7774 2074 6f20 7469  nverse cwt to ti
+000171f0: 6d65 2064 6f6d 6169 6e0a 2020 2020 2020  me domain.      
+00017200: 2020 6963 7774 3120 3d20 7079 6377 742e    icwt1 = pycwt.
+00017210: 6963 7774 2863 7774 315b 6672 6571 5f69  icwt(cwt1[freq_i
+00017220: 6e64 696e 5d2c 2073 6a5b 6672 6571 5f69  ndin], sj[freq_i
+00017230: 6e64 696e 5d2c 2064 742c 2064 6a2c 2077  ndin], dt, dj, w
+00017240: 766e 290a 2020 2020 2020 2020 6963 7774  vn).        icwt
+00017250: 3220 3d20 7079 6377 742e 6963 7774 2863  2 = pycwt.icwt(c
+00017260: 7774 325b 6672 6571 5f69 6e64 696e 5d2c  wt2[freq_indin],
+00017270: 2073 6a5b 6672 6571 5f69 6e64 696e 5d2c   sj[freq_indin],
+00017280: 2064 742c 2064 6a2c 2077 766e 290a 0a20   dt, dj, wvn).. 
+00017290: 2020 2020 2020 2023 2061 7373 756d 6520         # assume 
+000172a0: 616c 6c20 7469 6d65 2077 696e 646f 7720  all time window 
+000172b0: 6973 2075 7365 640a 2020 2020 2020 2020  is used.        
+000172c0: 7763 7774 312c 2077 6377 7432 203d 206e  wcwt1, wcwt2 = n
+000172d0: 702e 7265 616c 2869 6377 7431 292c 206e  p.real(icwt1), n
+000172e0: 702e 7265 616c 2869 6377 7432 290a 0a20  p.real(icwt2).. 
+000172f0: 2020 2020 2020 2023 204e 6f72 6d61 6c69         # Normali
+00017300: 7a65 7320 626f 7468 2073 6967 6e61 6c73  zes both signals
+00017310: 2c20 6966 2061 7070 726f 7072 6961 7465  , if appropriate
+00017320: 2e0a 2020 2020 2020 2020 6966 206e 6f72  ..        if nor
+00017330: 6d61 6c69 7a65 3a0a 2020 2020 2020 2020  malize:.        
+00017340: 2020 2020 6e63 7774 3120 3d20 2877 6377      ncwt1 = (wcw
+00017350: 7431 202d 2077 6377 7431 2e6d 6561 6e28  t1 - wcwt1.mean(
+00017360: 2929 202f 2077 6377 7431 2e73 7464 2829  )) / wcwt1.std()
+00017370: 0a20 2020 2020 2020 2020 2020 206e 6377  .            ncw
+00017380: 7432 203d 2028 7763 7774 3220 2d20 7763  t2 = (wcwt2 - wc
+00017390: 7774 322e 6d65 616e 2829 2920 2f20 7763  wt2.mean()) / wc
+000173a0: 7774 322e 7374 6428 290a 2020 2020 2020  wt2.std().      
+000173b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000173c0: 2020 2020 6e63 7774 3120 3d20 7763 7774      ncwt1 = wcwt
+000173d0: 310a 2020 2020 2020 2020 2020 2020 6e63  1.            nc
+000173e0: 7774 3220 3d20 7763 7774 320a 0a20 2020  wt2 = wcwt2..   
+000173f0: 2020 2020 2023 2072 756e 2073 7472 6574       # run stret
+00017400: 6368 696e 670a 2020 2020 2020 2020 6476  ching.        dv
+00017410: 762c 2065 7272 2c20 6363 2c20 6364 7020  v, err, cc, cdp 
+00017420: 3d20 7374 7265 7463 6869 6e67 286e 6377  = stretching(ncw
+00017430: 7432 2c20 6e63 7774 312c 2064 765f 7261  t2, ncwt1, dv_ra
+00017440: 6e67 652c 206e 6274 7269 616c 2c20 7061  nge, nbtrial, pa
+00017450: 7261 290a 2020 2020 2020 2020 7265 7475  ra).        retu
+00017460: 726e 2064 7676 2c20 6572 720a 0a20 2020  rn dvv, err..   
+00017470: 2023 2064 6972 6563 746c 7920 7461 6b65   # directly take
+00017480: 2061 6476 616e 7461 6765 206f 6620 7468   advantage of th
+00017490: 650a 2020 2020 656c 7365 3a0a 2020 2020  e.    else:.    
+000174a0: 2020 2020 2320 696e 6974 6961 6c69 7a65      # initialize
+000174b0: 2076 6172 6961 626c 650a 2020 2020 2020   variable.      
+000174c0: 2020 6e66 7265 7120 3d20 6c65 6e28 6672    nfreq = len(fr
+000174d0: 6571 5f69 6e64 696e 290a 2020 2020 2020  eq_indin).      
+000174e0: 2020 6476 762c 2063 632c 2063 6470 2c20    dvv, cc, cdp, 
+000174f0: 6572 7220 3d20 280a 2020 2020 2020 2020  err = (.        
+00017500: 2020 2020 6e70 2e7a 6572 6f73 286e 6672      np.zeros(nfr
+00017510: 6571 2c20 6474 7970 653d 6e70 2e66 6c6f  eq, dtype=np.flo
+00017520: 6174 3332 292c 0a20 2020 2020 2020 2020  at32),.         
+00017530: 2020 206e 702e 7a65 726f 7328 6e66 7265     np.zeros(nfre
+00017540: 712c 2064 7479 7065 3d6e 702e 666c 6f61  q, dtype=np.floa
+00017550: 7433 3229 2c0a 2020 2020 2020 2020 2020  t32),.          
+00017560: 2020 6e70 2e7a 6572 6f73 286e 6672 6571    np.zeros(nfreq
+00017570: 2c20 6474 7970 653d 6e70 2e66 6c6f 6174  , dtype=np.float
+00017580: 3332 292c 0a20 2020 2020 2020 2020 2020  32),.           
+00017590: 206e 702e 7a65 726f 7328 6e66 7265 712c   np.zeros(nfreq,
+000175a0: 2064 7479 7065 3d6e 702e 666c 6f61 7433   dtype=np.float3
+000175b0: 3229 2c0a 2020 2020 2020 2020 290a 0a20  2),.        ).. 
+000175c0: 2020 2020 2020 2023 206c 6f6f 7020 7468         # loop th
+000175d0: 726f 7567 6820 6561 6368 2066 7265 710a  rough each freq.
+000175e0: 2020 2020 2020 2020 666f 7220 6969 2c20          for ii, 
+000175f0: 6966 7265 7120 696e 2065 6e75 6d65 7261  ifreq in enumera
+00017600: 7465 2866 7265 715f 696e 6469 6e29 3a0a  te(freq_indin):.
+00017610: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
+00017620: 6570 6172 6520 7769 6e64 6f77 6564 2064  epare windowed d
+00017630: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
+00017640: 7763 7774 312c 2077 6377 7432 203d 2072  wcwt1, wcwt2 = r
+00017650: 6377 7431 5b69 6672 6571 5d2c 2072 6377  cwt1[ifreq], rcw
+00017660: 7432 5b69 6672 6571 5d0a 0a20 2020 2020  t2[ifreq]..     
+00017670: 2020 2020 2020 2023 204e 6f72 6d61 6c69         # Normali
+00017680: 7a65 7320 626f 7468 2073 6967 6e61 6c73  zes both signals
+00017690: 2c20 6966 2061 7070 726f 7072 6961 7465  , if appropriate
+000176a0: 2e0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000176b0: 206e 6f72 6d61 6c69 7a65 3a0a 2020 2020   normalize:.    
+000176c0: 2020 2020 2020 2020 2020 2020 6e63 7774              ncwt
+000176d0: 3120 3d20 2877 6377 7431 202d 2077 6377  1 = (wcwt1 - wcw
+000176e0: 7431 2e6d 6561 6e28 2929 202f 2077 6377  t1.mean()) / wcw
+000176f0: 7431 2e73 7464 2829 0a20 2020 2020 2020  t1.std().       
+00017700: 2020 2020 2020 2020 206e 6377 7432 203d           ncwt2 =
+00017710: 2028 7763 7774 3220 2d20 7763 7774 322e   (wcwt2 - wcwt2.
+00017720: 6d65 616e 2829 2920 2f20 7763 7774 322e  mean()) / wcwt2.
+00017730: 7374 6428 290a 2020 2020 2020 2020 2020  std().          
+00017740: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00017750: 2020 2020 2020 2020 6e63 7774 3120 3d20          ncwt1 = 
+00017760: 7763 7774 310a 2020 2020 2020 2020 2020  wcwt1.          
+00017770: 2020 2020 2020 6e63 7774 3220 3d20 7763        ncwt2 = wc
+00017780: 7774 320a 0a20 2020 2020 2020 2020 2020  wt2..           
+00017790: 2023 2072 756e 2073 7472 6574 6368 696e   # run stretchin
+000177a0: 670a 2020 2020 2020 2020 2020 2020 6476  g.            dv
+000177b0: 2c20 6572 726f 722c 2063 312c 2063 3220  , error, c1, c2 
+000177c0: 3d20 7374 7265 7463 6869 6e67 286e 6377  = stretching(ncw
+000177d0: 7432 2c20 6e63 7774 312c 2064 765f 7261  t2, ncwt1, dv_ra
+000177e0: 6e67 652c 206e 6274 7269 616c 2c20 7061  nge, nbtrial, pa
+000177f0: 7261 290a 2020 2020 2020 2020 2020 2020  ra).            
+00017800: 6476 765b 6969 5d2c 2063 635b 6969 5d2c  dvv[ii], cc[ii],
+00017810: 2063 6470 5b69 695d 2c20 6572 725b 6969   cdp[ii], err[ii
+00017820: 5d20 3d20 6476 2c20 6331 2c20 6332 2c20  ] = dv, c1, c2, 
+00017830: 6572 726f 720a 0a20 2020 2020 2020 2072  error..        r
+00017840: 6574 7572 6e20 6672 6571 5b66 7265 715f  eturn freq[freq_
+00017850: 696e 6469 6e5d 2c20 6476 762c 2065 7272  indin], dvv, err
+00017860: 0a0a 0a64 6566 2077 7464 7477 5f61 6c6c  ...def wtdtw_all
+00017870: 6672 6571 280a 2020 2020 7265 662c 0a20  freq(.    ref,. 
+00017880: 2020 2063 7572 2c0a 2020 2020 616c 6c66     cur,.    allf
+00017890: 7265 712c 0a20 2020 2070 6172 612c 0a20  req,.    para,. 
+000178a0: 2020 206d 6178 4c61 672c 0a20 2020 2062     maxLag,.    b
+000178b0: 2c0a 2020 2020 6469 7265 6374 696f 6e2c  ,.    direction,
+000178c0: 0a20 2020 2064 6a3d 3120 2f20 3132 2c0a  .    dj=1 / 12,.
+000178d0: 2020 2020 7330 3d2d 312c 0a20 2020 204a      s0=-1,.    J
+000178e0: 3d2d 312c 0a20 2020 2077 766e 3d22 6d6f  =-1,.    wvn="mo
+000178f0: 726c 6574 222c 0a20 2020 206e 6f72 6d61  rlet",.    norma
+00017900: 6c69 7a65 3d54 7275 652c 0a29 3a0a 2020  lize=True,.):.  
+00017910: 2020 2222 220a 2020 2020 4170 706c 7920    """.    Apply 
+00017920: 6479 6e61 6d69 6320 7469 6d65 2077 6172  dynamic time war
+00017930: 7069 6e67 206d 6574 686f 6420 746f 2063  ping method to c
+00017940: 6f6e 7469 6e75 6f75 7320 7761 7665 6c65  ontinuous wavele
+00017950: 7420 7472 616e 7366 6f72 6d61 7469 6f6e  t transformation
+00017960: 2028 4357 5429 206f 6620 7369 676e 616c   (CWT) of signal
+00017970: 730a 2020 2020 666f 7220 616c 6c20 6672  s.    for all fr
+00017980: 6571 7565 6369 6573 2069 6e20 616e 2069  equecies in an i
+00017990: 6e74 6572 6573 7420 7261 6e67 650a 0a20  nterest range.. 
+000179a0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+000179b0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+000179c0: 0a20 2020 2072 6566 3a20 5468 6520 2252  .    ref: The "R
+000179d0: 6566 6572 656e 6365 2220 7469 6d65 7365  eference" timese
+000179e0: 7269 6573 2028 6e75 6d70 792e 6e64 6172  ries (numpy.ndar
+000179f0: 7261 7929 0a20 2020 2063 7572 3a20 5468  ray).    cur: Th
+00017a00: 6520 2243 7572 7265 6e74 2220 7469 6d65  e "Current" time
+00017a10: 7365 7269 6573 2028 6e75 6d70 792e 6e64  series (numpy.nd
+00017a20: 6172 7261 7929 0a20 2020 2061 6c6c 6672  array).    allfr
+00017a30: 6571 3a20 6120 626f 6f6c 656e 2076 6172  eq: a boolen var
+00017a40: 6961 626c 6520 746f 206d 616b 6520 6d65  iable to make me
+00017a50: 6173 7572 656d 656e 7473 206f 6e20 616c  asurements on al
+00017a60: 6c20 6672 6571 7565 6e63 7920 7261 6e67  l frequency rang
+00017a70: 6520 6f72 206e 6f74 0a20 2020 206d 6178  e or not.    max
+00017a80: 4c61 673a 206d 6178 206e 756d 6265 7220  Lag: max number 
+00017a90: 6f66 2070 6f69 6e74 7320 746f 2073 6561  of points to sea
+00017aa0: 7263 6820 666f 7277 6172 6420 616e 6420  rch forward and 
+00017ab0: 6261 636b 7761 7264 2e0a 2020 2020 623a  backward..    b:
+00017ac0: 2062 2d76 616c 7565 2074 6f20 6c69 6d69   b-value to limi
+00017ad0: 7420 7374 7261 696e 2c20 7768 6963 6820  t strain, which 
+00017ae0: 6973 2074 6f20 6c69 6d69 7420 7468 6520  is to limit the 
+00017af0: 6d61 7869 6d75 6d20 7665 6c6f 6369 7479  maximum velocity
+00017b00: 2070 6572 7475 7262 6174 696f 6e2e 0a20   perturbation.. 
+00017b10: 2020 2053 6565 2065 7175 6174 696f 6e20     See equation 
+00017b20: 3131 2069 6e20 284d 696b 6573 656c 6c20  11 in (Mikesell 
+00017b30: 6574 2061 6c2e 2032 3031 3529 0a20 2020  et al. 2015).   
+00017b40: 2064 6972 6563 7469 6f6e 3a20 6469 7265   direction: dire
+00017b50: 6374 696f 6e20 746f 2061 6363 756d 756c  ction to accumul
+00017b60: 6174 6520 6572 726f 7273 2028 313d 666f  ate errors (1=fo
+00017b70: 7277 6172 642c 202d 313d 6261 636b 7761  rward, -1=backwa
+00017b80: 7264 290a 2020 2020 646a 2c20 7330 2c20  rd).    dj, s0, 
+00017b90: 4a2c 2073 6967 2c20 7776 6e3a 2063 6f6d  J, sig, wvn: com
+00017ba0: 6d6f 6e20 7061 7261 6d65 7465 7273 2075  mon parameters u
+00017bb0: 7365 6420 696e 2027 7761 7665 6c65 742e  sed in 'wavelet.
+00017bc0: 7763 7427 0a20 2020 206e 6f72 6d61 6c69  wct'.    normali
+00017bd0: 7a65 3a20 6e6f 726d 616c 697a 6520 7468  ze: normalize th
+00017be0: 6520 7761 7665 6c65 7420 7370 6563 7472  e wavelet spectr
+00017bf0: 756d 206f 7220 6e6f 742e 2044 6566 6175  um or not. Defau
+00017c00: 6c74 2069 7320 5472 7565 0a0a 2020 2020  lt is True..    
+00017c10: 5245 5455 524e 533a 0a20 2020 202d 2d2d  RETURNS:.    ---
+00017c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+00017c30: 2020 2020 6476 763a 2065 7374 696d 6174      dvv: estimat
+00017c40: 6564 2064 762f 760a 2020 2020 6572 723a  ed dv/v.    err:
+00017c50: 2065 7272 6f72 206f 6620 6476 2f76 2065   error of dv/v e
+00017c60: 7374 696d 6174 696f 6e0a 0a20 2020 2057  stimation..    W
+00017c70: 7269 7474 656e 2062 7920 436f 6e67 636f  ritten by Congco
+00017c80: 6e67 2059 7561 6e20 2833 3020 4a75 6e2c  ng Yuan (30 Jun,
+00017c90: 2032 3031 3929 0a20 2020 2022 2222 0a20   2019).    """. 
+00017ca0: 2020 2023 2063 6f6d 6d6f 6e20 7661 7269     # common vari
+00017cb0: 6162 6c65 730a 2020 2020 6672 6571 203d  ables.    freq =
+00017cc0: 2070 6172 615b 2266 7265 7122 5d0a 2020   para["freq"].  
+00017cd0: 2020 6474 203d 2070 6172 615b 2264 7422    dt = para["dt"
+00017ce0: 5d0a 2020 2020 666d 696e 203d 206e 702e  ].    fmin = np.
+00017cf0: 6d69 6e28 6672 6571 290a 2020 2020 666d  min(freq).    fm
+00017d00: 6178 203d 206e 702e 6d61 7828 6672 6571  ax = np.max(freq
+00017d10: 290a 0a20 2020 2023 2061 7070 6c79 2063  )..    # apply c
+00017d20: 7774 206f 6e20 7477 6f20 7472 6163 6573  wt on two traces
+00017d30: 0a20 2020 2063 7774 312c 2073 6a2c 2066  .    cwt1, sj, f
+00017d40: 7265 712c 2063 6f69 2c20 5f2c 205f 203d  req, coi, _, _ =
+00017d50: 2070 7963 7774 2e63 7774 2863 7572 2c20   pycwt.cwt(cur, 
+00017d60: 6474 2c20 646a 2c20 7330 2c20 4a2c 2077  dt, dj, s0, J, w
+00017d70: 766e 290a 2020 2020 6377 7432 2c20 736a  vn).    cwt2, sj
+00017d80: 2c20 6672 6571 2c20 636f 692c 205f 2c20  , freq, coi, _, 
+00017d90: 5f20 3d20 7079 6377 742e 6377 7428 7265  _ = pycwt.cwt(re
+00017da0: 662c 2064 742c 2064 6a2c 2073 302c 204a  f, dt, dj, s0, J
+00017db0: 2c20 7776 6e29 0a0a 2020 2020 2320 6578  , wvn)..    # ex
+00017dc0: 7472 6163 7420 7265 616c 2076 616c 7565  tract real value
+00017dd0: 7320 6f66 2063 7774 0a20 2020 2072 6377  s of cwt.    rcw
+00017de0: 7431 2c20 7263 7774 3220 3d20 6e70 2e72  t1, rcwt2 = np.r
+00017df0: 6561 6c28 6377 7431 292c 206e 702e 7265  eal(cwt1), np.re
+00017e00: 616c 2863 7774 3229 0a0a 2020 2020 2320  al(cwt2)..    # 
+00017e10: 7a65 726f 206f 7574 2063 6f6e 6520 6f66  zero out cone of
+00017e20: 2069 6e66 6c75 656e 6365 2061 6e64 2064   influence and d
+00017e30: 6174 6120 6f75 7473 6964 6520 6672 6571  ata outside freq
+00017e40: 7565 6e63 7920 6261 6e64 0a20 2020 2069  uency band.    i
+00017e50: 6620 2866 6d61 7820 3e20 6e70 2e6d 6178  f (fmax > np.max
+00017e60: 2866 7265 7129 2920 7c20 2866 6d61 7820  (freq)) | (fmax 
+00017e70: 3c3d 2066 6d69 6e29 3a0a 2020 2020 2020  <= fmin):.      
+00017e80: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00017e90: 6f72 2822 4162 6f72 743a 2069 6e70 7574  or("Abort: input
+00017ea0: 2066 7265 7175 656e 6379 206f 7574 206f   frequency out o
+00017eb0: 6620 6c69 6d69 7473 2122 290a 2020 2020  f limits!").    
+00017ec0: 656c 7365 3a0a 2020 2020 2020 2020 6672  else:.        fr
+00017ed0: 6571 5f69 6e64 696e 203d 206e 702e 7768  eq_indin = np.wh
+00017ee0: 6572 6528 2866 7265 7120 3e3d 2066 6d69  ere((freq >= fmi
+00017ef0: 6e29 2026 2028 6672 6571 203c 3d20 666d  n) & (freq <= fm
+00017f00: 6178 2929 5b30 5d0a 0a20 2020 2020 2020  ax))[0]..       
+00017f10: 2023 2055 7365 2044 5457 206d 6574 686f   # Use DTW metho
+00017f20: 6420 746f 2065 7874 7261 6374 2064 7676  d to extract dvv
+00017f30: 0a20 2020 2020 2020 206e 6672 6571 203d  .        nfreq =
+00017f40: 206c 656e 2866 7265 715f 696e 6469 6e29   len(freq_indin)
+00017f50: 0a20 2020 2020 2020 2064 7676 2c20 6572  .        dvv, er
+00017f60: 7220 3d20 6e70 2e7a 6572 6f73 286e 6672  r = np.zeros(nfr
+00017f70: 6571 2c20 6474 7970 653d 6e70 2e66 6c6f  eq, dtype=np.flo
+00017f80: 6174 3332 292c 206e 702e 7a65 726f 7328  at32), np.zeros(
+00017f90: 6e66 7265 712c 2064 7479 7065 3d6e 702e  nfreq, dtype=np.
+00017fa0: 666c 6f61 7433 3229 0a0a 2020 2020 2020  float32)..      
+00017fb0: 2020 666f 7220 6969 2c20 6966 7265 7120    for ii, ifreq 
+00017fc0: 696e 2065 6e75 6d65 7261 7465 2866 7265  in enumerate(fre
+00017fd0: 715f 696e 6469 6e29 3a0a 2020 2020 2020  q_indin):.      
+00017fe0: 2020 2020 2020 2320 7072 6570 6172 6520        # prepare 
+00017ff0: 7769 6e64 6f77 6564 2064 6174 610a 2020  windowed data.  
+00018000: 2020 2020 2020 2020 2020 7763 7774 312c            wcwt1,
+00018010: 2077 6377 7432 203d 2072 6377 7431 5b69   wcwt2 = rcwt1[i
+00018020: 6672 6571 5d2c 2072 6377 7432 5b69 6672  freq], rcwt2[ifr
+00018030: 6571 5d0a 2020 2020 2020 2020 2020 2020  eq].            
+00018040: 2320 4e6f 726d 616c 697a 6573 2062 6f74  # Normalizes bot
+00018050: 6820 7369 676e 616c 732c 2069 6620 6170  h signals, if ap
+00018060: 7072 6f70 7269 6174 652e 0a20 2020 2020  propriate..     
+00018070: 2020 2020 2020 2069 6620 6e6f 726d 616c         if normal
+00018080: 697a 653a 0a20 2020 2020 2020 2020 2020  ize:.           
+00018090: 2020 2020 206e 6377 7431 203d 2028 7763       ncwt1 = (wc
+000180a0: 7774 3120 2d20 7763 7774 312e 6d65 616e  wt1 - wcwt1.mean
+000180b0: 2829 2920 2f20 7763 7774 312e 7374 6428  ()) / wcwt1.std(
+000180c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000180d0: 2020 6e63 7774 3220 3d20 2877 6377 7432    ncwt2 = (wcwt2
+000180e0: 202d 2077 6377 7432 2e6d 6561 6e28 2929   - wcwt2.mean())
+000180f0: 202f 2077 6377 7432 2e73 7464 2829 0a20   / wcwt2.std(). 
+00018100: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00018110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018120: 206e 6377 7431 203d 2077 6377 7431 0a20   ncwt1 = wcwt1. 
+00018130: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00018140: 6377 7432 203d 2077 6377 7432 0a0a 2020  cwt2 = wcwt2..  
+00018150: 2020 2020 2020 2020 2020 2320 7275 6e20            # run 
+00018160: 6474 770a 2020 2020 2020 2020 2020 2020  dtw.            
+00018170: 6476 2c20 6572 726f 722c 2064 6973 7420  dv, error, dist 
+00018180: 3d20 6474 775f 6476 7628 6e63 7774 322c  = dtw_dvv(ncwt2,
+00018190: 206e 6377 7431 2c20 7061 7261 2c20 6d61   ncwt1, para, ma
+000181a0: 784c 6167 2c20 622c 2064 6972 6563 7469  xLag, b, directi
+000181b0: 6f6e 290a 2020 2020 2020 2020 2020 2020  on).            
+000181c0: 6476 765b 6969 5d2c 2065 7272 5b69 695d  dvv[ii], err[ii]
+000181d0: 203d 2064 762c 2065 7272 6f72 0a0a 2020   = dv, error..  
+000181e0: 2020 6465 6c20 6377 7431 2c20 6377 7432    del cwt1, cwt2
+000181f0: 2c20 7263 7774 312c 2072 6377 7432 2c20  , rcwt1, rcwt2, 
+00018200: 6e63 7774 312c 206e 6377 7432 2c20 7763  ncwt1, ncwt2, wc
+00018210: 7774 312c 2077 6377 7432 2c20 636f 692c  wt1, wcwt2, coi,
+00018220: 2073 6a2c 2064 6973 740a 0a20 2020 2069   sj, dist..    i
+00018230: 6620 6e6f 7420 616c 6c66 7265 713a 0a20  f not allfreq:. 
+00018240: 2020 2020 2020 2072 6574 7572 6e20 6e70         return np
+00018250: 2e6d 6561 6e28 6476 7629 2c20 6e70 2e6d  .mean(dvv), np.m
+00018260: 6561 6e28 6572 7229 0a20 2020 2065 6c73  ean(err).    els
+00018270: 653a 0a20 2020 2020 2020 2072 6574 7572  e:.        retur
+00018280: 6e20 6672 6571 5b66 7265 715f 696e 6469  n freq[freq_indi
+00018290: 6e5d 2c20 6476 762c 2065 7272 0a0a 0a23  n], dvv, err...#
 000182a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000182b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 000182c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000182d0: 2323 2323 2323 0a23 2323 2323 2323 2323  ######.#########
-000182e0: 2323 2323 2323 2320 4d4f 4e49 544f 5249  ####### MONITORI
-000182f0: 4e47 2055 5449 4c49 5459 2046 554e 4354  NG UTILITY FUNCT
-00018300: 494f 4e53 2023 2323 2323 2323 2323 2323  IONS ###########
-00018310: 2323 2323 0a23 2323 2323 2323 2323 2323  ####.###########
+000182d0: 2323 2323 2323 2323 2323 2323 0a23 2323  ############.###
+000182e0: 2323 2323 2323 2323 2323 2323 2320 4d4f  ############# MO
+000182f0: 4e49 544f 5249 4e47 2055 5449 4c49 5459  NITORING UTILITY
+00018300: 2046 554e 4354 494f 4e53 2023 2323 2323   FUNCTIONS #####
+00018310: 2323 2323 2323 2323 2323 0a23 2323 2323  ##########.#####
 00018320: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00018330: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00018340: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00018350: 2323 0a0a 2222 220a 6265 6c6f 7720 6172  ##..""".below ar
-00018360: 6520 6173 7365 6d62 6c79 206f 6620 7468  e assembly of th
-00018370: 6520 6d6f 6e69 746f 7269 6e67 2075 7469  e monitoring uti
-00018380: 6c69 7479 2066 756e 6374 696f 6e73 2063  lity functions c
-00018390: 616c 6c65 6420 6279 206d 6f6e 6974 6f72  alled by monitor
-000183a0: 696e 6720 6675 6e63 7469 6f6e 730a 2222  ing functions.""
-000183b0: 220a 0a0a 6465 6620 736d 6f6f 7468 2878  "...def smooth(x
-000183c0: 2c20 7769 6e64 6f77 3d22 626f 7863 6172  , window="boxcar
-000183d0: 222c 2068 616c 665f 7769 6e3d 3329 3a0a  ", half_win=3):.
-000183e0: 2020 2020 2222 220a 2020 2020 7065 7266      """.    perf
-000183f0: 6f72 6d73 2073 6d6f 6f74 6869 6e67 2069  orms smoothing i
-00018400: 6e20 696e 7465 7265 7374 6564 2074 696d  n interested tim
-00018410: 6520 7769 6e64 6f77 0a0a 2020 2020 5061  e window..    Pa
-00018420: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
-00018430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020  -----------.    
-00018440: 783a 2074 696d 6573 6572 6973 2064 6174  x: timeseris dat
-00018450: 610a 2020 2020 7769 6e64 6f77 3a20 7479  a.    window: ty
-00018460: 7065 7320 6f66 2077 696e 646f 7720 746f  pes of window to
-00018470: 2064 6f20 736d 6f6f 7468 696e 670a 2020   do smoothing.  
-00018480: 2020 6861 6c66 5f77 696e 3a20 6861 6c66    half_win: half
-00018490: 2077 696e 646f 7720 6c65 6e67 7468 0a0a   window length..
-000184a0: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
-000184b0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-000184c0: 2d2d 2d0a 2020 2020 793a 2073 6d6f 6f74  ---.    y: smoot
-000184d0: 6865 6420 7469 6d65 2077 696e 646f 770a  hed time window.
-000184e0: 2020 2020 2222 220a 2020 2020 2320 544f      """.    # TO
-000184f0: 444f 3a20 646f 6373 7469 6e67 0a20 2020  DO: docsting.   
-00018500: 2077 696e 646f 775f 6c65 6e20 3d20 3220   window_len = 2 
-00018510: 2a20 6861 6c66 5f77 696e 202b 2031 0a20  * half_win + 1. 
-00018520: 2020 2023 2065 7874 656e 6469 6e67 2074     # extending t
-00018530: 6865 2064 6174 6120 6174 2062 6567 696e  he data at begin
-00018540: 6e69 6e67 2061 6e64 2061 7420 7468 6520  ning and at the 
-00018550: 656e 640a 2020 2020 2320 746f 2061 7070  end.    # to app
-00018560: 6c79 2074 6865 2077 696e 646f 7720 6174  ly the window at
-00018570: 2074 6865 2062 6f72 6465 7273 0a20 2020   the borders.   
-00018580: 2073 203d 206e 702e 725f 5b78 5b77 696e   s = np.r_[x[win
-00018590: 646f 775f 6c65 6e20 2d20 3120 3a20 3020  dow_len - 1 : 0 
-000185a0: 3a20 2d31 5d2c 2078 2c20 785b 2d31 3a2d  : -1], x, x[-1:-
-000185b0: 7769 6e64 6f77 5f6c 656e 3a2d 315d 5d0a  window_len:-1]].
-000185c0: 2020 2020 6966 2077 696e 646f 7720 3d3d      if window ==
-000185d0: 2022 626f 7863 6172 223a 0a20 2020 2020   "boxcar":.     
-000185e0: 2020 2077 203d 2073 6369 7079 2e73 6967     w = scipy.sig
-000185f0: 6e61 6c2e 626f 7863 6172 2877 696e 646f  nal.boxcar(windo
-00018600: 775f 6c65 6e29 2e61 7374 7970 6528 2263  w_len).astype("c
-00018610: 6f6d 706c 6578 2229 0a20 2020 2065 6c73  omplex").    els
-00018620: 653a 0a20 2020 2020 2020 2077 203d 2073  e:.        w = s
-00018630: 6369 7079 2e73 6967 6e61 6c2e 6861 6e6e  cipy.signal.hann
-00018640: 696e 6728 7769 6e64 6f77 5f6c 656e 292e  ing(window_len).
-00018650: 6173 7479 7065 2822 636f 6d70 6c65 7822  astype("complex"
-00018660: 290a 2020 2020 7920 3d20 6e70 2e63 6f6e  ).    y = np.con
-00018670: 766f 6c76 6528 7720 2f20 772e 7375 6d28  volve(w / w.sum(
-00018680: 292c 2073 2c20 6d6f 6465 3d22 7661 6c69  ), s, mode="vali
-00018690: 6422 290a 2020 2020 7265 7475 726e 2079  d").    return y
-000186a0: 5b68 616c 665f 7769 6e20 3a20 6c65 6e28  [half_win : len(
-000186b0: 7929 202d 2068 616c 665f 7769 6e5d 0a0a  y) - half_win]..
-000186c0: 0a64 6566 206e 6578 7470 6f77 3228 7829  .def nextpow2(x)
-000186d0: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-000186e0: 7475 726e 7320 7468 6520 6e65 7874 2070  turns the next p
-000186f0: 6f77 6572 206f 6620 3220 6f66 2078 2e0a  ower of 2 of x..
-00018700: 2020 2020 2222 220a 2020 2020 7265 7475      """.    retu
-00018710: 726e 2069 6e74 286e 702e 6365 696c 286e  rn int(np.ceil(n
-00018720: 702e 6c6f 6732 286e 702e 6162 7328 7829  p.log2(np.abs(x)
-00018730: 2929 290a 0a0a 6465 6620 6765 7443 6f68  )))...def getCoh
-00018740: 6572 656e 6365 2864 6373 2c20 6473 312c  erence(dcs, ds1,
-00018750: 2064 7332 293a 0a20 2020 2022 2222 0a20   ds2):.    """. 
-00018760: 2020 2067 6574 2063 726f 7373 2063 6f68     get cross coh
-00018770: 6572 656e 6365 2062 6574 7765 656e 2072  erence between r
-00018780: 6566 6572 656e 6365 2061 6e64 2063 7572  eference and cur
-00018790: 7265 6e74 2077 6176 6566 6f72 6d73 2066  rent waveforms f
-000187a0: 6f6c 6c6f 7769 6e67 2065 7175 6174 696f  ollowing equatio
-000187b0: 6e20 6f66 2041 3320 696e 2043 6c61 726b  n of A3 in Clark
-000187c0: 2065 7420 616c 2e2c 2032 3031 310a 0a20   et al., 2011.. 
-000187d0: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-000187e0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-000187f0: 0a20 2020 2064 6373 3a20 616d 706c 6974  .    dcs: amplit
-00018800: 7564 6520 6f66 2074 6865 2063 726f 7373  ude of the cross
-00018810: 2073 7065 6374 7275 6d0a 2020 2020 6473   spectrum.    ds
-00018820: 313a 2061 6d70 6c69 7475 6465 206f 6620  1: amplitude of 
-00018830: 7468 6520 7370 6563 7472 756d 206f 6620  the spectrum of 
-00018840: 6375 7272 656e 7420 7761 7665 666f 726d  current waveform
-00018850: 0a20 2020 2064 7332 3a20 616d 706c 6974  .    ds2: amplit
-00018860: 7564 6520 6f66 2074 6865 2073 7065 6374  ude of the spect
-00018870: 7275 6d20 6f66 2072 6566 6572 656e 6365  rum of reference
-00018880: 2077 6176 6566 6f72 6d0a 0a20 2020 2052   waveform..    R
-00018890: 4554 5552 4e53 3a0a 2020 2020 2d2d 2d2d  ETURNS:.    ----
-000188a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
-000188b0: 2020 2063 6f68 3a20 636f 6872 6572 656e     coh: cohreren
-000188c0: 6379 206d 6174 7269 7820 7573 6564 2066  cy matrix used f
-000188d0: 6f72 2065 7374 696d 6174 6520 7468 6520  or estimate the 
-000188e0: 726f 6275 7374 6e65 7373 206f 6620 7468  robustness of th
-000188f0: 6520 6372 6f73 7320 7370 6563 7472 756d  e cross spectrum
-00018900: 0a20 2020 2022 2222 0a20 2020 206e 203d  .    """.    n =
-00018910: 206c 656e 2864 6373 290a 2020 2020 636f   len(dcs).    co
-00018920: 6820 3d20 6e70 2e7a 6572 6f73 286e 292e  h = np.zeros(n).
-00018930: 6173 7479 7065 2822 636f 6d70 6c65 7822  astype("complex"
-00018940: 290a 2020 2020 7661 6c69 6473 203d 206e  ).    valids = n
-00018950: 702e 6172 6777 6865 7265 286e 702e 6c6f  p.argwhere(np.lo
-00018960: 6769 6361 6c5f 616e 6428 6e70 2e61 6273  gical_and(np.abs
-00018970: 2864 7331 2920 3e20 302c 206e 702e 6162  (ds1) > 0, np.ab
-00018980: 7328 6473 3229 203e 2030 2929 0a20 2020  s(ds2) > 0)).   
-00018990: 2063 6f68 5b76 616c 6964 735d 203d 2064   coh[valids] = d
-000189a0: 6373 5b76 616c 6964 735d 202f 2028 6473  cs[valids] / (ds
-000189b0: 315b 7661 6c69 6473 5d20 2a20 6473 325b  1[valids] * ds2[
-000189c0: 7661 6c69 6473 5d29 0a20 2020 2063 6f68  valids]).    coh
-000189d0: 5b63 6f68 203e 2028 312e 3020 2b20 306a  [coh > (1.0 + 0j
-000189e0: 295d 203d 2031 2e30 202b 2030 6a0a 2020  )] = 1.0 + 0j.  
-000189f0: 2020 7265 7475 726e 2063 6f68 0a0a 0a64    return coh...d
-00018a00: 6566 2063 6f6d 7075 7465 4572 726f 7246  ef computeErrorF
-00018a10: 756e 6374 696f 6e28 7531 2c20 7530 2c20  unction(u1, u0, 
-00018a20: 6e53 616d 706c 652c 206c 6167 2c20 6e6f  nSample, lag, no
-00018a30: 726d 3d22 4c32 2229 3a0a 2020 2020 2222  rm="L2"):.    ""
-00018a40: 220a 2020 2020 636f 6d70 7574 6520 4572  ".    compute Er
-00018a50: 726f 7220 4675 6e63 7469 6f6e 2075 7365  ror Function use
-00018a60: 6420 696e 2044 5457 2e20 5468 6520 6572  d in DTW. The er
-00018a70: 726f 7220 6675 6e63 7469 6f6e 2069 7320  ror function is 
-00018a80: 6571 7561 7469 6f6e 2031 2069 6e20 4861  equation 1 in Ha
-00018a90: 6c65 2c20 3230 3133 2e20 596f 7520 636f  le, 2013. You co
-00018aa0: 756c 6420 756e 636f 6d6d 656e 7420 7468  uld uncomment th
-00018ab0: 650a 2020 2020 4c31 206e 6f72 6d20 616e  e.    L1 norm an
-00018ac0: 6420 636f 6d6d 656e 7420 7468 6520 4c32  d comment the L2
-00018ad0: 206e 6f72 6d20 6966 2079 6f75 2077 616e   norm if you wan
-00018ae0: 7420 6f6e 204c 696e 6520 3239 0a0a 2020  t on Line 29..  
-00018af0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00018b00: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a   --------------.
-00018b10: 2020 2020 7531 3a20 2074 7261 6365 2074      u1:  trace t
-00018b20: 6861 7420 7765 2077 616e 7420 746f 2077  hat we want to w
-00018b30: 6172 703b 2073 697a 6520 3d20 286e 7361  arp; size = (nsa
-00018b40: 6d70 2c31 290a 2020 2020 7530 3a20 2072  mp,1).    u0:  r
-00018b50: 6566 6572 656e 6365 2074 7261 6365 2074  eference trace t
-00018b60: 6f20 636f 6d70 6172 6520 7769 7468 3a20  o compare with: 
-00018b70: 7369 7a65 203d 2028 6e73 616d 702c 3129  size = (nsamp,1)
-00018b80: 0a20 2020 206e 5361 6d70 6c65 3a20 6e75  .    nSample: nu
-00018b90: 6d65 7220 6f66 2070 6f69 6e74 7320 746f  mer of points to
-00018ba0: 2063 6f6d 7061 7265 2069 6e20 7468 6520   compare in the 
-00018bb0: 7472 6163 6573 0a20 2020 206c 6167 3a20  traces.    lag: 
-00018bc0: 6d61 7869 6d75 6d20 6c61 6720 696e 2073  maximum lag in s
-00018bd0: 616d 706c 6520 6e75 6d62 6572 2074 6f20  ample number to 
-00018be0: 7365 6172 6368 0a20 2020 206e 6f72 6d3a  search.    norm:
-00018bf0: 2027 4c32 2720 6f72 2027 4c31 2720 2864   'L2' or 'L1' (d
-00018c00: 6566 6175 6c74 2069 7320 274c 3227 290a  efault is 'L2').
-00018c10: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
-00018c20: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
-00018c30: 2d2d 2d2d 0a20 2020 2065 7272 3a20 7468  ----.    err: th
-00018c40: 6520 3244 2065 7272 6f72 2066 756e 6374  e 2D error funct
-00018c50: 696f 6e3b 2073 697a 6520 3d20 286e 7361  ion; size = (nsa
-00018c60: 6d70 2c32 2a6c 6167 2b31 290a 0a20 2020  mp,2*lag+1)..   
-00018c70: 204f 7269 6769 6e61 6c20 6279 2044 6920   Original by Di 
-00018c80: 5961 6e67 0a20 2020 204c 6173 7420 6d6f  Yang.    Last mo
-00018c90: 6469 6669 6564 2062 7920 4479 6c61 6e20  dified by Dylan 
-00018ca0: 4d69 6b65 7365 6c6c 2028 3235 2046 6562  Mikesell (25 Feb
-00018cb0: 2e20 3230 3135 290a 2020 2020 5472 616e  . 2015).    Tran
-00018cc0: 736c 6174 6564 2074 6f20 7079 7468 6f6e  slated to python
-00018cd0: 2062 7920 5469 6d20 436c 656d 656e 7473   by Tim Clements
-00018ce0: 2028 3137 2041 7567 2e20 3230 3138 290a   (17 Aug. 2018).
-00018cf0: 0a20 2020 2022 2222 0a0a 2020 2020 6966  .    """..    if
-00018d00: 206c 6167 203e 3d20 6e53 616d 706c 653a   lag >= nSample:
-00018d10: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
-00018d20: 616c 7565 4572 726f 7228 2263 6f6d 7075  alueError("compu
-00018d30: 7465 4572 726f 7246 756e 6374 696f 6e3a  teErrorFunction:
-00018d40: 6c61 6750 726f 626c 656d 222c 2022 6c61  lagProblem", "la
-00018d50: 6720 6d75 7374 2062 6520 736d 616c 6c65  g must be smalle
-00018d60: 7220 7468 616e 206e 5361 6d70 6c65 2229  r than nSample")
-00018d70: 0a0a 2020 2020 2320 416c 6c6f 6361 7465  ..    # Allocate
-00018d80: 2065 7272 6f72 2066 756e 6374 696f 6e20   error function 
-00018d90: 7661 7269 6162 6c65 0a20 2020 2065 7272  variable.    err
-00018da0: 203d 206e 702e 7a65 726f 7328 5b6e 5361   = np.zeros([nSa
-00018db0: 6d70 6c65 2c20 3220 2a20 6c61 6720 2b20  mple, 2 * lag + 
-00018dc0: 315d 290a 0a20 2020 2023 2069 6e69 7469  1])..    # initi
-00018dd0: 616c 2065 7272 6f72 2063 616c 6375 6c61  al error calcula
-00018de0: 7469 6f6e 0a20 2020 2023 206c 6f6f 7020  tion.    # loop 
-00018df0: 6f76 6572 206c 6167 730a 2020 2020 666f  over lags.    fo
-00018e00: 7220 6c6c 2069 6e20 6e70 2e61 7261 6e67  r ll in np.arang
-00018e10: 6528 2d6c 6167 2c20 6c61 6720 2b20 3129  e(-lag, lag + 1)
-00018e20: 3a0a 2020 2020 2020 2020 7468 6973 4c61  :.        thisLa
-00018e30: 6720 3d20 6c6c 202b 206c 6167 0a0a 2020  g = ll + lag..  
-00018e40: 2020 2020 2020 2320 6c6f 6f70 206f 7665        # loop ove
-00018e50: 7220 7361 6d70 6c65 730a 2020 2020 2020  r samples.      
-00018e60: 2020 666f 7220 6969 2069 6e20 7261 6e67    for ii in rang
-00018e70: 6528 6e53 616d 706c 6529 3a0a 2020 2020  e(nSample):.    
-00018e80: 2020 2020 2020 2020 2320 736b 6970 2063          # skip c
-00018e90: 6f72 6e65 7273 2066 6f72 206e 6f77 2c20  orners for now, 
-00018ea0: 7765 2077 696c 6c20 636f 6d65 2062 6163  we will come bac
-00018eb0: 6b20 746f 2074 6865 7365 0a20 2020 2020  k to these.     
-00018ec0: 2020 2020 2020 2069 6620 2869 6920 2b20         if (ii + 
-00018ed0: 6c6c 203e 3d20 3029 2026 2028 6969 202b  ll >= 0) & (ii +
-00018ee0: 206c 6c20 3c20 6e53 616d 706c 6529 3a0a   ll < nSample):.
-00018ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f00: 6572 725b 6969 2c20 7468 6973 4c61 675d  err[ii, thisLag]
-00018f10: 203d 2075 315b 6969 5d20 2d20 7530 5b69   = u1[ii] - u0[i
-00018f20: 6920 2b20 6c6c 5d0a 0a20 2020 2069 6620  i + ll]..    if 
-00018f30: 6e6f 726d 203d 3d20 224c 3222 3a0a 2020  norm == "L2":.  
-00018f40: 2020 2020 2020 6572 7220 3d20 6572 722a        err = err*
-00018f50: 2a32 0a20 2020 2065 6c69 6620 6e6f 726d  *2.    elif norm
-00018f60: 203d 3d20 224c 3122 3a0a 2020 2020 2020   == "L1":.      
-00018f70: 2020 6572 7220 3d20 6e70 2e61 6273 2865    err = np.abs(e
-00018f80: 7272 290a 0a20 2020 2023 204e 6f77 2066  rr)..    # Now f
-00018f90: 6978 2063 6f72 6e65 7273 2077 6974 6820  ix corners with 
-00018fa0: 636f 6e73 7461 6e74 2065 7874 7261 706f  constant extrapo
-00018fb0: 6c61 7469 6f6e 0a20 2020 2066 6f72 206c  lation.    for l
-00018fc0: 6c20 696e 206e 702e 6172 616e 6765 282d  l in np.arange(-
-00018fd0: 6c61 672c 206c 6167 202b 2031 293a 0a20  lag, lag + 1):. 
-00018fe0: 2020 2020 2020 2074 6869 734c 6167 203d         thisLag =
-00018ff0: 206c 6c20 2b20 6c61 670a 0a20 2020 2020   ll + lag..     
-00019000: 2020 2066 6f72 2069 6920 696e 2072 616e     for ii in ran
-00019010: 6765 286e 5361 6d70 6c65 293a 0a20 2020  ge(nSample):.   
-00019020: 2020 2020 2020 2020 2069 6620 6969 202b           if ii +
-00019030: 206c 6c20 3c20 303a 0a20 2020 2020 2020   ll < 0:.       
-00019040: 2020 2020 2020 2020 2065 7272 5b69 692c           err[ii,
-00019050: 2074 6869 734c 6167 5d20 3d20 6572 725b   thisLag] = err[
-00019060: 2d6c 6c2c 2074 6869 734c 6167 5d0a 0a20  -ll, thisLag].. 
-00019070: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00019080: 6969 202b 206c 6c20 3e20 6e53 616d 706c  ii + ll > nSampl
-00019090: 6520 2d20 313a 0a20 2020 2020 2020 2020  e - 1:.         
-000190a0: 2020 2020 2020 2065 7272 5b69 692c 2074         err[ii, t
-000190b0: 6869 734c 6167 5d20 3d20 6572 725b 6e53  hisLag] = err[nS
-000190c0: 616d 706c 6520 2d20 6c6c 202d 2031 2c20  ample - ll - 1, 
-000190d0: 7468 6973 4c61 675d 0a0a 2020 2020 7265  thisLag]..    re
-000190e0: 7475 726e 2065 7272 0a0a 0a64 6566 2061  turn err...def a
-000190f0: 6363 756d 756c 6174 6545 7272 6f72 4675  ccumulateErrorFu
-00019100: 6e63 7469 6f6e 2864 6972 2c20 6572 722c  nction(dir, err,
-00019110: 206e 5361 6d70 6c65 2c20 6c61 672c 2062   nSample, lag, b
-00019120: 293a 0a20 2020 2022 2222 0a20 2020 2061  ):.    """.    a
-00019130: 6363 756d 756c 6174 696f 6e20 6f66 2074  ccumulation of t
-00019140: 6865 2065 7272 6f72 2c20 7768 6963 6820  he error, which 
-00019150: 666f 6c6c 6f77 7320 7468 6520 6571 7561  follows the equa
-00019160: 7469 6f6e 2036 2069 6e20 4861 6c65 2c20  tion 6 in Hale, 
-00019170: 3230 3133 2e0a 0a20 2020 2050 6172 616d  2013...    Param
-00019180: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00019190: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2064 6972  --------.    dir
-000191a0: 3a20 6163 6375 6d75 6c61 7469 6f6e 2064  : accumulation d
-000191b0: 6972 6563 7469 6f6e 2028 2064 6972 203e  irection ( dir >
-000191c0: 2030 203d 2066 6f72 7761 7264 2069 6e20   0 = forward in 
-000191d0: 7469 6d65 2c20 6469 7220 3c3d 2030 203d  time, dir <= 0 =
-000191e0: 2062 6163 6b77 6172 6420 696e 2074 696d   backward in tim
-000191f0: 6529 0a20 2020 2065 7272 3a20 7468 6520  e).    err: the 
-00019200: 3244 2065 7272 6f72 2066 756e 6374 696f  2D error functio
-00019210: 6e3b 2073 697a 6520 3d20 286e 7361 6d70  n; size = (nsamp
-00019220: 2c32 2a6c 6167 2b31 290a 2020 2020 6e53  ,2*lag+1).    nS
-00019230: 616d 706c 653a 206e 756d 6572 206f 6620  ample: numer of 
-00019240: 706f 696e 7473 2074 6f20 636f 6d70 6172  points to compar
-00019250: 6520 696e 2074 6865 2074 7261 6365 730a  e in the traces.
-00019260: 2020 2020 6c61 673a 206d 6178 696d 756d      lag: maximum
-00019270: 206c 6167 2069 6e20 7361 6d70 6c65 206e   lag in sample n
-00019280: 756d 6265 7220 746f 2073 6561 7263 680a  umber to search.
-00019290: 2020 2020 623a 2073 7472 6169 6e20 6c69      b: strain li
-000192a0: 6d69 7420 2869 6e74 6567 6572 2076 616c  mit (integer val
-000192b0: 7565 203e 3d20 3129 0a0a 2020 2020 5245  ue >= 1)..    RE
-000192c0: 5455 524e 533a 0a20 2020 202d 2d2d 2d2d  TURNS:.    -----
-000192d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-000192e0: 2020 643a 2074 6865 2032 4420 6469 7374    d: the 2D dist
-000192f0: 616e 6365 2066 756e 6374 696f 6e3b 2073  ance function; s
-00019300: 697a 6520 3d20 286e 7361 6d70 2c32 2a6c  ize = (nsamp,2*l
-00019310: 6167 2b31 290a 0a20 2020 204f 7269 6769  ag+1)..    Origi
-00019320: 6e61 6c20 6279 2044 6920 5961 6e67 0a20  nal by Di Yang. 
-00019330: 2020 204c 6173 7420 6d6f 6469 6669 6564     Last modified
-00019340: 2062 7920 4479 6c61 6e20 4d69 6b65 7365   by Dylan Mikese
-00019350: 6c6c 2028 3235 2046 6562 2e20 3230 3135  ll (25 Feb. 2015
-00019360: 290a 2020 2020 5472 616e 736c 6174 6564  ).    Translated
-00019370: 2074 6f20 7079 7468 6f6e 2062 7920 5469   to python by Ti
-00019380: 6d20 436c 656d 656e 7473 2028 3137 2041  m Clements (17 A
-00019390: 7567 2e20 3230 3138 290a 0a20 2020 2022  ug. 2018)..    "
-000193a0: 2222 0a0a 2020 2020 2320 6e75 6d62 6572  ""..    # number
-000193b0: 206f 6620 6c61 6773 2066 726f 6d20 5b20   of lags from [ 
-000193c0: 2d6c 6167 203a 202b 6c61 6720 5d0a 2020  -lag : +lag ].  
-000193d0: 2020 6e4c 6167 203d 2028 3220 2a20 6c61    nLag = (2 * la
-000193e0: 6729 202b 2031 0a0a 2020 2020 2320 616c  g) + 1..    # al
-000193f0: 6c6f 6361 7465 2064 6973 7461 6e63 6520  locate distance 
-00019400: 6d61 7472 6978 0a20 2020 2064 203d 206e  matrix.    d = n
-00019410: 702e 7a65 726f 7328 5b6e 5361 6d70 6c65  p.zeros([nSample
-00019420: 2c20 6e4c 6167 5d29 0a0a 2020 2020 2320  , nLag])..    # 
-00019430: 5365 7475 7020 696e 6469 6365 7320 6261  Setup indices ba
-00019440: 7365 6420 6f6e 2066 6f72 7761 7264 206f  sed on forward o
-00019450: 7220 6261 636b 7761 7264 2061 6363 756d  r backward accum
-00019460: 756c 6174 696f 6e20 6469 7265 6374 696f  ulation directio
-00019470: 6e0a 2020 2020 6966 2064 6972 203e 2030  n.    if dir > 0
-00019480: 3a20 2023 2046 4f52 5741 5244 0a20 2020  :  # FORWARD.   
-00019490: 2020 2020 2069 4265 6769 6e2c 2069 456e       iBegin, iEn
-000194a0: 642c 2069 496e 6320 3d20 302c 206e 5361  d, iInc = 0, nSa
-000194b0: 6d70 6c65 202d 2031 2c20 310a 2020 2020  mple - 1, 1.    
-000194c0: 656c 7365 3a20 2023 2042 4143 4b57 4152  else:  # BACKWAR
-000194d0: 440a 2020 2020 2020 2020 6942 6567 696e  D.        iBegin
-000194e0: 2c20 6945 6e64 2c20 6949 6e63 203d 206e  , iEnd, iInc = n
-000194f0: 5361 6d70 6c65 202d 2031 2c20 302c 202d  Sample - 1, 0, -
-00019500: 310a 0a20 2020 2023 204c 6f6f 7020 7468  1..    # Loop th
-00019510: 726f 7567 6820 616c 6c20 7469 6d65 7320  rough all times 
-00019520: 6969 2069 6e20 666f 7277 6172 6420 6f72  ii in forward or
-00019530: 2062 6163 6b77 6172 6420 6469 7265 6374   backward direct
-00019540: 696f 6e0a 2020 2020 666f 7220 6969 2069  ion.    for ii i
-00019550: 6e20 7261 6e67 6528 6942 6567 696e 2c20  n range(iBegin, 
-00019560: 6945 6e64 202b 2069 496e 632c 2069 496e  iEnd + iInc, iIn
-00019570: 6329 3a0a 2020 2020 2020 2020 2320 6d69  c):.        # mi
-00019580: 6e2f 6d61 7820 746f 2061 6363 6f75 6e74  n/max to account
-00019590: 2066 6f72 2074 6865 2065 6467 6573 2f62   for the edges/b
-000195a0: 6f75 6e64 6172 6965 730a 2020 2020 2020  oundaries.      
-000195b0: 2020 6a69 203d 206d 6178 285b 302c 206d    ji = max([0, m
-000195c0: 696e 285b 6e53 616d 706c 6520 2d20 312c  in([nSample - 1,
-000195d0: 2069 6920 2d20 6949 6e63 5d29 5d29 0a20   ii - iInc])]). 
-000195e0: 2020 2020 2020 206a 6220 3d20 6d61 7828         jb = max(
-000195f0: 5b30 2c20 6d69 6e28 5b6e 5361 6d70 6c65  [0, min([nSample
-00019600: 202d 2031 2c20 6969 202d 2069 496e 6320   - 1, ii - iInc 
-00019610: 2a20 625d 295d 290a 0a20 2020 2020 2020  * b])])..       
-00019620: 2023 206c 6f6f 7020 7468 726f 7567 6820   # loop through 
-00019630: 616c 6c20 6c61 670a 2020 2020 2020 2020  all lag.        
-00019640: 666f 7220 6c6c 2069 6e20 7261 6e67 6528  for ll in range(
-00019650: 6e4c 6167 293a 0a20 2020 2020 2020 2020  nLag):.         
-00019660: 2020 2023 2063 6865 636b 206c 696d 6974     # check limit
-00019670: 7320 6f6e 206c 6167 2069 6e64 6963 6573  s on lag indices
-00019680: 0a20 2020 2020 2020 2020 2020 206c 4d69  .            lMi
-00019690: 6e75 7331 203d 206c 6c20 2d20 310a 0a20  nus1 = ll - 1.. 
-000196a0: 2020 2020 2020 2020 2020 2023 2063 6865             # che
-000196b0: 636b 206c 6167 2069 6e64 6578 2069 7320  ck lag index is 
-000196c0: 6772 6561 7465 7220 7468 616e 2030 0a20  greater than 0. 
-000196d0: 2020 2020 2020 2020 2020 2069 6620 6c4d             if lM
-000196e0: 696e 7573 3120 3c20 303a 0a20 2020 2020  inus1 < 0:.     
-000196f0: 2020 2020 2020 2020 2020 206c 4d69 6e75             lMinu
-00019700: 7331 203d 2030 2020 2320 6d61 6b65 206c  s1 = 0  # make l
-00019710: 6167 203d 2066 6972 7374 206c 6167 0a0a  ag = first lag..
-00019720: 2020 2020 2020 2020 2020 2020 6c50 6c75              lPlu
-00019730: 7331 203d 206c 6c20 2b20 3120 2023 206c  s1 = ll + 1  # l
-00019740: 6167 2061 7420 6c2b 310a 0a20 2020 2020  ag at l+1..     
-00019750: 2020 2020 2020 2023 2063 6865 636b 206c         # check l
-00019760: 6167 2069 6e64 6578 206c 6573 7320 7468  ag index less th
-00019770: 616e 206d 6178 206c 6167 0a20 2020 2020  an max lag.     
-00019780: 2020 2020 2020 2069 6620 6c50 6c75 7331         if lPlus1
-00019790: 203e 206e 4c61 6720 2d20 313a 0a20 2020   > nLag - 1:.   
-000197a0: 2020 2020 2020 2020 2020 2020 206c 506c               lPl
-000197b0: 7573 3120 3d20 6e4c 6167 202d 2031 0a0a  us1 = nLag - 1..
-000197c0: 2020 2020 2020 2020 2020 2020 2320 6765              # ge
-000197d0: 7420 6469 7374 616e 6365 2061 7420 6c61  t distance at la
-000197e0: 6773 2028 6c6c 2d31 2c20 6c6c 2c20 6c6c  gs (ll-1, ll, ll
-000197f0: 2b31 290a 2020 2020 2020 2020 2020 2020  +1).            
-00019800: 6469 7374 4c6d 696e 7573 3120 3d20 645b  distLminus1 = d[
-00019810: 6a62 2c20 6c4d 696e 7573 315d 2020 2320  jb, lMinus1]  # 
-00019820: 6d69 6e75 733a 2020 645b 692d 622c 206a  minus:  d[i-b, j
-00019830: 2d31 5d0a 2020 2020 2020 2020 2020 2020  -1].            
-00019840: 6469 7374 4c20 3d20 645b 6a69 2c20 6c6c  distL = d[ji, ll
-00019850: 5d20 2023 2061 6374 7561 6c20 645b 692d  ]  # actual d[i-
-00019860: 312c 206a 5d0a 2020 2020 2020 2020 2020  1, j].          
-00019870: 2020 6469 7374 4c70 6c75 7331 203d 2064    distLplus1 = d
-00019880: 5b6a 622c 206c 506c 7573 315d 2020 2320  [jb, lPlus1]  # 
-00019890: 706c 7573 2064 5b69 2d62 2c20 6a2b 315d  plus d[i-b, j+1]
-000198a0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-000198b0: 206a 6920 213d 206a 623a 2020 2320 6571   ji != jb:  # eq
-000198c0: 7561 7469 6f6e 2031 3020 696e 2048 616c  uation 10 in Hal
-000198d0: 652c 2032 3031 330a 2020 2020 2020 2020  e, 2013.        
-000198e0: 2020 2020 2020 2020 666f 7220 6b62 2069          for kb i
-000198f0: 6e20 7261 6e67 6528 6a69 2c20 6a62 202b  n range(ji, jb +
-00019900: 2069 496e 6320 2d20 312c 202d 6949 6e63   iInc - 1, -iInc
-00019910: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00019920: 2020 2020 2020 2064 6973 744c 6d69 6e75         distLminu
-00019930: 7331 203d 2064 6973 744c 6d69 6e75 7331  s1 = distLminus1
-00019940: 202b 2065 7272 5b6b 622c 206c 4d69 6e75   + err[kb, lMinu
-00019950: 7331 5d0a 2020 2020 2020 2020 2020 2020  s1].            
-00019960: 2020 2020 2020 2020 6469 7374 4c70 6c75          distLplu
-00019970: 7331 203d 2064 6973 744c 706c 7573 3120  s1 = distLplus1 
-00019980: 2b20 6572 725b 6b62 2c20 6c50 6c75 7331  + err[kb, lPlus1
-00019990: 5d0a 0a20 2020 2020 2020 2020 2020 2023  ]..            #
-000199a0: 2065 7175 6174 696f 6e20 3620 2869 6620   equation 6 (if 
-000199b0: 623d 3129 206f 7220 3130 2028 6966 2062  b=1) or 10 (if b
-000199c0: 3e31 2920 696e 2048 616c 6520 2832 3031  >1) in Hale (201
-000199d0: 3329 2061 6674 6572 2074 7265 6174 696e  3) after treatin
-000199e0: 6720 626f 756e 6461 7269 6573 0a20 2020  g boundaries.   
-000199f0: 2020 2020 2020 2020 2064 5b69 692c 206c           d[ii, l
-00019a00: 6c5d 203d 2065 7272 5b69 692c 206c 6c5d  l] = err[ii, ll]
-00019a10: 202b 206d 696e 285b 6469 7374 4c6d 696e   + min([distLmin
-00019a20: 7573 312c 2064 6973 744c 2c20 6469 7374  us1, distL, dist
-00019a30: 4c70 6c75 7331 5d29 0a0a 2020 2020 7265  Lplus1])..    re
-00019a40: 7475 726e 2064 0a0a 0a64 6566 2062 6163  turn d...def bac
-00019a50: 6b74 7261 636b 4469 7374 616e 6365 4675  ktrackDistanceFu
-00019a60: 6e63 7469 6f6e 2864 6972 2c20 642c 2065  nction(dir, d, e
-00019a70: 7272 2c20 6c6d 696e 2c20 6229 3a0a 2020  rr, lmin, b):.  
-00019a80: 2020 2222 220a 2020 2020 5468 6520 6675    """.    The fu
-00019a90: 6e63 7469 6f6e 2069 7320 6571 7561 7469  nction is equati
-00019aa0: 6f6e 2032 2069 6e20 4861 6c65 2c20 3230  on 2 in Hale, 20
-00019ab0: 3133 2e0a 0a20 2020 2050 6172 616d 6574  13...    Paramet
-00019ac0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-00019ad0: 2d2d 2d2d 2d2d 0a20 2020 2064 6972 3a20  ------.    dir: 
-00019ae0: 7369 6465 2074 6f20 7374 6172 7420 6d69  side to start mi
-00019af0: 6e69 6d69 7a61 7469 6f6e 2028 2064 6972  nimization ( dir
-00019b00: 203e 2030 203d 2066 726f 6e74 2c20 6469   > 0 = front, di
-00019b10: 7220 3c3d 2030 203d 2020 6261 636b 290a  r <= 0 =  back).
-00019b20: 2020 2020 6420 3a20 7468 6520 3244 2064      d : the 2D d
-00019b30: 6973 7461 6e63 6520 6675 6e63 7469 6f6e  istance function
-00019b40: 3b20 7369 7a65 203d 2028 6e73 616d 702c  ; size = (nsamp,
-00019b50: 322a 6c61 672b 3129 0a20 2020 2065 7272  2*lag+1).    err
-00019b60: 3a20 7468 6520 3244 2065 7272 6f72 2066  : the 2D error f
-00019b70: 756e 6374 696f 6e3b 2073 697a 6520 3d20  unction; size = 
-00019b80: 286e 7361 6d70 2c32 2a6c 6167 2b31 290a  (nsamp,2*lag+1).
-00019b90: 2020 2020 6c6d 696e 3a20 6d69 6e69 6d75      lmin: minimu
-00019ba0: 6d20 6c61 6720 746f 2073 6561 7263 6820  m lag to search 
-00019bb0: 6f76 6572 0a20 2020 2062 203a 2073 7472  over.    b : str
-00019bc0: 6169 6e20 6c69 6d69 7420 2869 6e74 6567  ain limit (integ
-00019bd0: 6572 2076 616c 7565 203e 3d20 3129 0a0a  er value >= 1)..
-00019be0: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
-00019bf0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
-00019c00: 2d2d 2d0a 2020 2020 7374 6261 723a 2076  ---.    stbar: v
-00019c10: 6563 746f 7220 6f66 2069 6e74 6567 6572  ector of integer
-00019c20: 2073 6869 6674 7320 7375 626a 6563 7420   shifts subject 
-00019c30: 746f 207c 7528 6929 2d75 2869 2d31 297c  to |u(i)-u(i-1)|
-00019c40: 203c 3d20 312f 620a 0a20 2020 204f 7269   <= 1/b..    Ori
-00019c50: 6769 6e61 6c20 6279 2044 6920 5961 6e67  ginal by Di Yang
-00019c60: 0a20 2020 204c 6173 7420 6d6f 6469 6669  .    Last modifi
-00019c70: 6564 2062 7920 4479 6c61 6e20 4d69 6b65  ed by Dylan Mike
-00019c80: 7365 6c6c 2028 3139 2044 6563 2e20 3230  sell (19 Dec. 20
-00019c90: 3134 290a 0a20 2020 2054 7261 6e73 6c61  14)..    Transla
-00019ca0: 7465 6420 746f 2070 7974 686f 6e20 6279  ted to python by
-00019cb0: 2054 696d 2043 6c65 6d65 6e74 7320 2831   Tim Clements (1
-00019cc0: 3720 4175 672e 2032 3031 3829 0a0a 2020  7 Aug. 2018)..  
-00019cd0: 2020 2222 220a 0a20 2020 206e 5361 6d70    """..    nSamp
-00019ce0: 6c65 2c20 6e4c 6167 203d 2064 2e73 6861  le, nLag = d.sha
-00019cf0: 7065 0a20 2020 2073 7462 6172 203d 206e  pe.    stbar = n
-00019d00: 702e 7a65 726f 7328 6e53 616d 706c 6529  p.zeros(nSample)
-00019d10: 0a0a 2020 2020 2320 5365 7475 7020 696e  ..    # Setup in
-00019d20: 6469 6365 7320 6261 7365 6420 6f6e 2066  dices based on f
-00019d30: 6f72 7761 7264 206f 7220 6261 636b 7761  orward or backwa
-00019d40: 7264 2061 6363 756d 756c 6174 696f 6e20  rd accumulation 
-00019d50: 6469 7265 6374 696f 6e0a 2020 2020 6966  direction.    if
-00019d60: 2064 6972 203e 2030 3a20 2023 2046 4f52   dir > 0:  # FOR
-00019d70: 5741 5244 0a20 2020 2020 2020 2069 4265  WARD.        iBe
-00019d80: 6769 6e2c 2069 456e 642c 2069 496e 6320  gin, iEnd, iInc 
-00019d90: 3d20 302c 206e 5361 6d70 6c65 202d 2031  = 0, nSample - 1
-00019da0: 2c20 310a 2020 2020 656c 7365 3a20 2023  , 1.    else:  #
-00019db0: 2042 4143 4b57 4152 440a 2020 2020 2020   BACKWARD.      
-00019dc0: 2020 6942 6567 696e 2c20 6945 6e64 2c20    iBegin, iEnd, 
-00019dd0: 6949 6e63 203d 206e 5361 6d70 6c65 202d  iInc = nSample -
-00019de0: 2031 2c20 302c 202d 310a 0a20 2020 2023   1, 0, -1..    #
-00019df0: 2073 7461 7274 2066 726f 6d20 7468 6520   start from the 
-00019e00: 656e 6420 2866 726f 6e74 206f 7220 6261  end (front or ba
-00019e10: 636b 290a 2020 2020 6c6c 203d 206e 702e  ck).    ll = np.
-00019e20: 6172 676d 696e 2864 5b69 4265 6769 6e2c  argmin(d[iBegin,
-00019e30: 203a 5d29 2020 2320 6669 6e64 206d 696e   :])  # find min
-00019e40: 696d 756d 2061 6363 756d 756c 6174 6564  imum accumulated
-00019e50: 2064 6973 7461 6e63 6520 6174 2066 726f   distance at fro
-00019e60: 6e74 206f 7220 6261 636b 2064 6570 656e  nt or back depen
-00019e70: 6469 6e67 206f 6e20 2764 6972 270a 2020  ding on 'dir'.  
-00019e80: 2020 7374 6261 725b 6942 6567 696e 5d20    stbar[iBegin] 
-00019e90: 3d20 6c6c 202b 206c 6d69 6e20 2023 2061  = ll + lmin  # a
-00019ea0: 6273 6f6c 7574 6520 7661 6c75 6520 6f66  bsolute value of
-00019eb0: 2069 6e74 6567 6572 2073 6869 6674 0a0a   integer shift..
-00019ec0: 2020 2020 2320 6d6f 7665 2074 6872 6f75      # move throu
-00019ed0: 6768 2061 6c6c 2074 696d 6520 7361 6d70  gh all time samp
-00019ee0: 6c65 7320 696e 2066 6f72 7761 7264 206f  les in forward o
-00019ef0: 7220 6261 636b 7761 7264 2064 6972 6563  r backward direc
-00019f00: 7469 6f6e 0a20 2020 2069 6920 3d20 6942  tion.    ii = iB
-00019f10: 6567 696e 0a0a 2020 2020 7768 696c 6520  egin..    while 
-00019f20: 6969 2021 3d20 6945 6e64 3a0a 2020 2020  ii != iEnd:.    
-00019f30: 2020 2020 2320 6d69 6e2f 6d61 7820 666f      # min/max fo
-00019f40: 7220 6564 6765 732f 626f 756e 6461 7269  r edges/boundari
-00019f50: 6573 0a20 2020 2020 2020 206a 6920 3d20  es.        ji = 
-00019f60: 6e70 2e6d 6178 285b 302c 206e 702e 6d69  np.max([0, np.mi
-00019f70: 6e28 5b6e 5361 6d70 6c65 202d 2031 2c20  n([nSample - 1, 
-00019f80: 6969 202b 2069 496e 635d 295d 290a 2020  ii + iInc])]).  
-00019f90: 2020 2020 2020 6a62 203d 206e 702e 6d61        jb = np.ma
-00019fa0: 7828 5b30 2c20 6e70 2e6d 696e 285b 6e53  x([0, np.min([nS
-00019fb0: 616d 706c 6520 2d20 312c 2069 6920 2b20  ample - 1, ii + 
-00019fc0: 6949 6e63 202a 2062 5d29 5d29 0a0a 2020  iInc * b])])..  
-00019fd0: 2020 2020 2020 2320 6368 6563 6b20 6c69        # check li
-00019fe0: 6d69 7473 206f 6e20 6c61 6720 696e 6469  mits on lag indi
-00019ff0: 6365 730a 2020 2020 2020 2020 6c4d 696e  ces.        lMin
-0001a000: 7573 3120 3d20 6c6c 202d 2031 0a0a 2020  us1 = ll - 1..  
-0001a010: 2020 2020 2020 6966 206c 4d69 6e75 7331        if lMinus1
-0001a020: 203c 2030 3a20 2023 2063 6865 636b 206c   < 0:  # check l
-0001a030: 6167 2069 6e64 6578 2069 7320 6772 6561  ag index is grea
-0001a040: 7465 7220 7468 616e 2031 0a20 2020 2020  ter than 1.     
-0001a050: 2020 2020 2020 206c 4d69 6e75 7331 203d         lMinus1 =
-0001a060: 2030 2020 2320 6d61 6b65 206c 6167 203d   0  # make lag =
-0001a070: 2066 6972 7374 206c 6167 0a0a 2020 2020   first lag..    
-0001a080: 2020 2020 6c50 6c75 7331 203d 206c 6c20      lPlus1 = ll 
-0001a090: 2b20 310a 0a20 2020 2020 2020 2069 6620  + 1..        if 
-0001a0a0: 6c50 6c75 7331 203e 206e 4c61 6720 2d20  lPlus1 > nLag - 
-0001a0b0: 313a 2020 2320 6368 6563 6b20 6c61 6720  1:  # check lag 
-0001a0c0: 696e 6465 7820 6c65 7373 2074 6861 6e20  index less than 
-0001a0d0: 6d61 7820 6c61 670a 2020 2020 2020 2020  max lag.        
-0001a0e0: 2020 2020 6c50 6c75 7331 203d 206e 4c61      lPlus1 = nLa
-0001a0f0: 6720 2d20 310a 0a20 2020 2020 2020 2023  g - 1..        #
-0001a100: 2067 6574 2064 6973 7461 6e63 6520 6174   get distance at
-0001a110: 206c 6167 7320 286c 6c2d 312c 206c 6c2c   lags (ll-1, ll,
-0001a120: 206c 6c2b 3129 0a20 2020 2020 2020 2064   ll+1).        d
-0001a130: 6973 744c 6d69 6e75 7331 203d 2064 5b6a  istLminus1 = d[j
-0001a140: 622c 206c 4d69 6e75 7331 5d20 2023 206d  b, lMinus1]  # m
-0001a150: 696e 7573 3a20 2064 5b69 2d62 2c20 6a2d  inus:  d[i-b, j-
-0001a160: 315d 0a20 2020 2020 2020 2064 6973 744c  1].        distL
-0001a170: 203d 2064 5b6a 692c 206c 6c5d 2020 2320   = d[ji, ll]  # 
-0001a180: 6163 7475 616c 2064 5b69 2d31 2c20 6a5d  actual d[i-1, j]
-0001a190: 0a20 2020 2020 2020 2064 6973 744c 706c  .        distLpl
-0001a1a0: 7573 3120 3d20 645b 6a62 2c20 6c50 6c75  us1 = d[jb, lPlu
-0001a1b0: 7331 5d20 2023 2070 6c75 7320 645b 692d  s1]  # plus d[i-
-0001a1c0: 622c 206a 2b31 5d0a 0a20 2020 2020 2020  b, j+1]..       
-0001a1d0: 2023 2065 7175 6174 696f 6e20 3130 2069   # equation 10 i
-0001a1e0: 6e20 4861 6c65 2028 3230 3133 290a 2020  n Hale (2013).  
-0001a1f0: 2020 2020 2020 2320 7375 6d20 6572 726f        # sum erro
-0001a200: 7273 206f 7665 7220 692d 313a 692d 622b  rs over i-1:i-b+
-0001a210: 310a 2020 2020 2020 2020 6966 206a 6920  1.        if ji 
-0001a220: 213d 206a 623a 0a20 2020 2020 2020 2020  != jb:.         
-0001a230: 2020 2066 6f72 206b 6220 696e 2072 616e     for kb in ran
-0001a240: 6765 286a 692c 206a 6220 2d20 6949 6e63  ge(ji, jb - iInc
-0001a250: 202d 2031 2c20 6949 6e63 293a 0a20 2020   - 1, iInc):.   
-0001a260: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-0001a270: 744c 6d69 6e75 7331 203d 2064 6973 744c  tLminus1 = distL
-0001a280: 6d69 6e75 7331 202b 2065 7272 5b6b 622c  minus1 + err[kb,
-0001a290: 206c 4d69 6e75 7331 5d0a 2020 2020 2020   lMinus1].      
-0001a2a0: 2020 2020 2020 2020 2020 6469 7374 4c70            distLp
-0001a2b0: 6c75 7331 203d 2064 6973 744c 706c 7573  lus1 = distLplus
-0001a2c0: 3120 2b20 6572 725b 6b62 2c20 6c50 6c75  1 + err[kb, lPlu
-0001a2d0: 7331 5d0a 0a20 2020 2020 2020 2023 2075  s1]..        # u
-0001a2e0: 7064 6174 6520 6d69 6e69 6d75 6d20 6469  pdate minimum di
-0001a2f0: 7374 616e 6365 2074 6f20 7072 6576 696f  stance to previo
-0001a300: 7573 2073 616d 706c 650a 2020 2020 2020  us sample.      
-0001a310: 2020 646c 203d 206e 702e 6d69 6e28 5b64    dl = np.min([d
-0001a320: 6973 744c 6d69 6e75 7331 2c20 6469 7374  istLminus1, dist
-0001a330: 4c2c 2064 6973 744c 706c 7573 315d 290a  L, distLplus1]).
-0001a340: 0a20 2020 2020 2020 2069 6620 646c 2021  .        if dl !
-0001a350: 3d20 6469 7374 4c3a 2020 2320 7468 656e  = distL:  # then
-0001a360: 206c 6c20 7e3d 206c 6c20 616e 6420 7765   ll ~= ll and we
-0001a370: 2063 6865 636b 2066 6f72 7761 7264 2061   check forward a
-0001a380: 6e64 2062 6163 6b77 6172 640a 2020 2020  nd backward.    
-0001a390: 2020 2020 2020 2020 6966 2064 6c20 3d3d          if dl ==
-0001a3a0: 2064 6973 744c 6d69 6e75 7331 3a0a 2020   distLminus1:.  
-0001a3b0: 2020 2020 2020 2020 2020 2020 2020 6c6c                ll
-0001a3c0: 203d 206c 4d69 6e75 7331 0a20 2020 2020   = lMinus1.     
-0001a3d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0001a3e0: 2020 2020 2020 2020 2020 2020 206c 6c20               ll 
-0001a3f0: 3d20 6c50 6c75 7331 0a0a 2020 2020 2020  = lPlus1..      
-0001a400: 2020 2320 6173 7375 6d65 2069 6920 3d20    # assume ii = 
-0001a410: 6969 202d 2031 0a20 2020 2020 2020 2069  ii - 1.        i
-0001a420: 6920 2b3d 2069 496e 630a 0a20 2020 2020  i += iInc..     
-0001a430: 2020 2023 2061 6273 6f6c 7574 6520 696e     # absolute in
-0001a440: 7465 6765 7220 6f66 206c 6167 0a20 2020  teger of lag.   
-0001a450: 2020 2020 2073 7462 6172 5b69 695d 203d       stbar[ii] =
-0001a460: 206c 6c20 2b20 6c6d 696e 0a0a 2020 2020   ll + lmin..    
-0001a470: 2020 2020 2320 6e6f 7720 6d6f 7665 2074      # now move t
-0001a480: 6f20 636f 7272 6563 7420 7469 6d65 2069  o correct time i
-0001a490: 6e64 6578 2c20 6966 2073 6d6f 6f74 6869  ndex, if smoothi
-0001a4a0: 6e67 2064 6966 6665 7265 6e63 6520 6f76  ng difference ov
-0001a4b0: 6572 206d 616e 790a 2020 2020 2020 2020  er many.        
-0001a4c0: 2320 7469 6d65 2073 616d 706c 6573 2075  # time samples u
-0001a4d0: 7369 6e67 2027 6227 0a20 2020 2020 2020  sing 'b'.       
-0001a4e0: 2069 6620 286c 6c20 3d3d 206c 4d69 6e75   if (ll == lMinu
-0001a4f0: 7331 2920 7c20 286c 6c20 3d3d 206c 506c  s1) | (ll == lPl
-0001a500: 7573 3129 3a20 2023 2063 6865 636b 2065  us1):  # check e
-0001a510: 6467 6573 2074 6f20 7365 6520 6162 6f75  dges to see abou
-0001a520: 7420 6220 7661 6c75 6573 0a20 2020 2020  t b values.     
-0001a530: 2020 2020 2020 2069 6620 6a69 2021 3d20         if ji != 
-0001a540: 6a62 3a20 2023 2069 6620 623e 3120 7468  jb:  # if b>1 th
-0001a550: 656e 206e 6565 6420 746f 206d 6f76 6520  en need to move 
-0001a560: 6d6f 7265 2073 7465 7073 0a20 2020 2020  more steps.     
-0001a570: 2020 2020 2020 2020 2020 2066 6f72 206b             for k
-0001a580: 6220 696e 2072 616e 6765 286a 692c 206a  b in range(ji, j
-0001a590: 6220 2d20 6949 6e63 202d 2031 2c20 6949  b - iInc - 1, iI
-0001a5a0: 6e63 293a 0a20 2020 2020 2020 2020 2020  nc):.           
-0001a5b0: 2020 2020 2020 2020 2069 6920 3d20 6969           ii = ii
-0001a5c0: 202b 2069 496e 6320 2023 206d 6f76 6520   + iInc  # move 
-0001a5d0: 6672 6f6d 2069 2d31 3a69 2d62 2d31 0a20  from i-1:i-b-1. 
-0001a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5f0: 2020 2073 7462 6172 5b69 695d 203d 206c     stbar[ii] = l
-0001a600: 6c20 2b20 6c6d 696e 2020 2320 636f 6e73  l + lmin  # cons
-0001a610: 7461 6e74 206c 6167 206f 7665 7220 7468  tant lag over th
-0001a620: 6174 2074 696d 650a 0a20 2020 2072 6574  at time..    ret
-0001a630: 7572 6e20 7374 6261 720a 0a0a 6465 6620  urn stbar...def 
-0001a640: 7763 745f 6d6f 6469 6669 6564 280a 2020  wct_modified(.  
-0001a650: 2020 7931 2c20 7932 2c20 6474 2c20 646a    y1, y2, dt, dj
-0001a660: 3d31 202f 2031 322c 2073 303d 2d31 2c20  =1 / 12, s0=-1, 
-0001a670: 4a3d 2d31 2c20 7369 673d 5472 7565 2c20  J=-1, sig=True, 
-0001a680: 7369 676e 6966 6963 616e 6365 5f6c 6576  significance_lev
-0001a690: 656c 3d30 2e39 352c 2077 6176 656c 6574  el=0.95, wavelet
-0001a6a0: 3d22 6d6f 726c 6574 222c 206e 6f72 6d61  ="morlet", norma
-0001a6b0: 6c69 7a65 3d54 7275 652c 202a 2a6b 7761  lize=True, **kwa
-0001a6c0: 7267 730a 293a 0a20 2020 2022 2222 0a20  rgs.):.    """. 
-0001a6d0: 2020 2020 2020 2057 6176 656c 6574 2063         Wavelet c
-0001a6e0: 6f68 6572 656e 6365 2074 7261 6e73 666f  oherence transfo
-0001a6f0: 726d 2028 5743 5429 2e0a 2020 2020 e280  rm (WCT)..    ..
-0001a700: 8b0a 2020 2020 2020 2020 5468 6520 5743  ..        The WC
-0001a710: 5420 6669 6e64 7320 7265 6769 6f6e 7320  T finds regions 
-0001a720: 696e 2074 696d 6520 6672 6571 7565 6e63  in time frequenc
-0001a730: 7920 7370 6163 6520 7768 6572 6520 7468  y space where th
-0001a740: 6520 7477 6f20 7469 6d65 0a20 2020 2020  e two time.     
-0001a750: 2020 2073 6572 6965 7320 636f 2d76 6172     series co-var
-0001a760: 792c 2062 7574 2064 6f20 6e6f 7420 6e65  y, but do not ne
-0001a770: 6365 7373 6172 696c 7920 6861 7665 2068  cessarily have h
-0001a780: 6967 6820 706f 7765 722e 0a20 2020 20e2  igh power..    .
-0001a790: 808b 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0001a7a0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-0001a7b0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-0001a7c0: 2079 312c 2079 3220 3a20 6e75 6d70 792e   y1, y2 : numpy.
-0001a7d0: 6e64 6172 7261 792c 206c 6973 740a 2020  ndarray, list.  
-0001a7e0: 2020 2020 2020 2020 2020 496e 7075 7420            Input 
-0001a7f0: 7369 676e 616c 732e 0a20 2020 2020 2020  signals..       
-0001a800: 2064 7420 3a20 666c 6f61 740a 2020 2020   dt : float.    
-0001a810: 2020 2020 2020 2020 5361 6d70 6c65 2073          Sample s
-0001a820: 7061 6369 6e67 2e0a 2020 2020 2020 2020  pacing..        
-0001a830: 646a 203a 2066 6c6f 6174 2c20 6f70 7469  dj : float, opti
-0001a840: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
-0001a850: 2053 7061 6369 6e67 2062 6574 7765 656e   Spacing between
-0001a860: 2064 6973 6372 6574 6520 7363 616c 6573   discrete scales
-0001a870: 2e20 4465 6661 756c 7420 7661 6c75 6520  . Default value 
-0001a880: 6973 2031 2f31 322e 0a20 2020 2020 2020  is 1/12..       
-0001a890: 2020 2020 2053 6d61 6c6c 6572 2076 616c       Smaller val
-0001a8a0: 7565 7320 7769 6c6c 2072 6573 756c 7420  ues will result 
-0001a8b0: 696e 2062 6574 7465 7220 7363 616c 6520  in better scale 
-0001a8c0: 7265 736f 6c75 7469 6f6e 2c20 6275 740a  resolution, but.
-0001a8d0: 2020 2020 2020 2020 2020 2020 736c 6f77              slow
-0001a8e0: 6572 2063 616c 6375 6c61 7469 6f6e 2061  er calculation a
-0001a8f0: 6e64 2070 6c6f 742e 0a20 2020 2020 2020  nd plot..       
-0001a900: 2073 3020 3a20 666c 6f61 742c 206f 7074   s0 : float, opt
-0001a910: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-0001a920: 2020 536d 616c 6c65 7374 2073 6361 6c65    Smallest scale
-0001a930: 206f 6620 7468 6520 7761 7665 6c65 742e   of the wavelet.
-0001a940: 2044 6566 6175 6c74 2076 616c 7565 2069   Default value i
-0001a950: 7320 322a 6474 2e0a 2020 2020 2020 2020  s 2*dt..        
-0001a960: 4a20 3a20 666c 6f61 742c 206f 7074 696f  J : float, optio
-0001a970: 6e61 6c0a 2020 2020 2020 2020 2020 2020  nal.            
-0001a980: 4e75 6d62 6572 206f 6620 7363 616c 6573  Number of scales
-0001a990: 206c 6573 7320 6f6e 652e 2053 6361 6c65   less one. Scale
-0001a9a0: 7320 7261 6e67 6520 6672 6f6d 2073 3020  s range from s0 
-0001a9b0: 7570 2074 6f0a 2020 2020 2020 2020 2020  up to.          
-0001a9c0: 2020 7330 202a 2032 2a2a 284a 202a 2064    s0 * 2**(J * d
-0001a9d0: 6a29 2c20 7768 6963 6820 6769 7665 7320  j), which gives 
-0001a9e0: 6120 746f 7461 6c20 6f66 2028 4a20 2b20  a total of (J + 
-0001a9f0: 3129 2073 6361 6c65 732e 0a20 2020 2020  1) scales..     
-0001aa00: 2020 2020 2020 2044 6566 6175 6c74 2069         Default i
-0001aa10: 7320 4a20 3d20 286c 6f67 3228 4e2a 6474  s J = (log2(N*dt
-0001aa20: 2f73 6f29 292f 646a 2e0a 2020 2020 2020  /so))/dj..      
-0001aa30: 2020 7369 676e 6966 6963 616e 6365 5f6c    significance_l
-0001aa40: 6576 656c 2028 666c 6f61 742c 206f 7074  evel (float, opt
-0001aa50: 696f 6e61 6c29 203a 0a20 2020 2020 2020  ional) :.       
-0001aa60: 2020 2020 2053 6967 6e69 6669 6361 6e63       Significanc
-0001aa70: 6520 6c65 7665 6c20 746f 2075 7365 2e20  e level to use. 
-0001aa80: 4465 6661 756c 7420 6973 2030 2e39 352e  Default is 0.95.
-0001aa90: 0a20 2020 2020 2020 206e 6f72 6d61 6c69  .        normali
-0001aaa0: 7a65 2028 626f 6f6c 6561 6e2c 206f 7074  ze (boolean, opt
-0001aab0: 696f 6e61 6c29 203a 0a20 2020 2020 2020  ional) :.       
-0001aac0: 2020 2020 2049 6620 7365 7420 746f 2074       If set to t
-0001aad0: 7275 652c 206e 6f72 6d61 6c69 7a65 7320  rue, normalizes 
-0001aae0: 4357 5420 6279 2074 6865 2073 7461 6e64  CWT by the stand
-0001aaf0: 6172 6420 6465 7669 6174 696f 6e20 6f66  ard deviation of
-0001ab00: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-0001ab10: 2073 6967 6e61 6c73 2e0a 2020 2020 e280   signals..    ..
-0001ab20: 8b0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0001ab30: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-0001ab40: 2d0a 2020 2020 2020 2020 544f 444f 3a20  -.        TODO: 
-0001ab50: 536f 6d65 7468 696e 6720 5442 4120 616e  Something TBA an
-0001ab60: 6420 5442 430a 2020 2020 e280 8b0a 2020  d TBC.    ....  
-0001ab70: 2020 2020 2020 5365 6520 616c 736f 0a20        See also. 
-0001ab80: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0a         --------.
-0001ab90: 2020 2020 2020 2020 6377 742c 2078 7774          cwt, xwt
-0001aba0: 0a20 2020 20e2 808b 0a20 2020 2022 2222  .    ....    """
-0001abb0: 0a0a 2020 2020 7761 7665 6c65 7420 3d20  ..    wavelet = 
-0001abc0: 7079 6377 742e 7761 7665 6c65 742e 5f63  pycwt.wavelet._c
-0001abd0: 6865 636b 5f70 6172 616d 6574 6572 5f77  heck_parameter_w
-0001abe0: 6176 656c 6574 2877 6176 656c 6574 290a  avelet(wavelet).
-0001abf0: 2020 2020 2320 4368 6563 6b69 6e67 2073      # Checking s
-0001ac00: 6f6d 6520 696e 7075 7420 7061 7261 6d65  ome input parame
-0001ac10: 7465 7273 0a20 2020 2069 6620 7330 203d  ters.    if s0 =
-0001ac20: 3d20 2d31 3a0a 2020 2020 2020 2020 2320  = -1:.        # 
-0001ac30: 4e75 6d62 6572 206f 6620 7363 616c 6573  Number of scales
-0001ac40: 0a20 2020 2020 2020 2073 3020 3d20 3220  .        s0 = 2 
-0001ac50: 2a20 6474 202f 2077 6176 656c 6574 2e66  * dt / wavelet.f
-0001ac60: 6c61 6d62 6461 2829 0a20 2020 2069 6620  lambda().    if 
-0001ac70: 4a20 3d3d 202d 313a 0a20 2020 2020 2020  J == -1:.       
-0001ac80: 2023 204e 756d 6265 7220 6f66 2073 6361   # Number of sca
-0001ac90: 6c65 730a 2020 2020 2020 2020 4a20 3d20  les.        J = 
-0001aca0: 6e70 2e69 6e74 286e 702e 726f 756e 6428  np.int(np.round(
-0001acb0: 6e70 2e6c 6f67 3228 7931 2e73 697a 6520  np.log2(y1.size 
-0001acc0: 2a20 6474 202f 2073 3029 202f 2064 6a29  * dt / s0) / dj)
-0001acd0: 290a 0a20 2020 2023 204d 616b 6573 2073  )..    # Makes s
-0001ace0: 7572 6520 696e 7075 7420 7369 676e 616c  ure input signal
-0001acf0: 7320 6172 6520 6e75 6d70 7920 6172 7261  s are numpy arra
-0001ad00: 7973 2e0a 2020 2020 7931 203d 206e 702e  ys..    y1 = np.
-0001ad10: 6173 6172 7261 7928 7931 290a 2020 2020  asarray(y1).    
-0001ad20: 7932 203d 206e 702e 6173 6172 7261 7928  y2 = np.asarray(
-0001ad30: 7932 290a 2020 2020 2320 4361 6c63 756c  y2).    # Calcul
-0001ad40: 6174 6573 2074 6865 2073 7461 6e64 6172  ates the standar
-0001ad50: 6420 6465 7669 6174 696f 6e20 6f66 2062  d deviation of b
-0001ad60: 6f74 6820 696e 7075 7420 7369 676e 616c  oth input signal
-0001ad70: 732e 0a20 2020 2073 7464 3120 3d20 7931  s..    std1 = y1
-0001ad80: 2e73 7464 2829 0a20 2020 2073 7464 3220  .std().    std2 
-0001ad90: 3d20 7932 2e73 7464 2829 0a20 2020 2023  = y2.std().    #
-0001ada0: 204e 6f72 6d61 6c69 7a65 7320 626f 7468   Normalizes both
-0001adb0: 2073 6967 6e61 6c73 2c20 6966 2061 7070   signals, if app
-0001adc0: 726f 7072 6961 7465 2e0a 2020 2020 6966  ropriate..    if
-0001add0: 206e 6f72 6d61 6c69 7a65 3a0a 2020 2020   normalize:.    
-0001ade0: 2020 2020 7931 5f6e 6f72 6d61 6c20 3d20      y1_normal = 
-0001adf0: 2879 3120 2d20 7931 2e6d 6561 6e28 2929  (y1 - y1.mean())
-0001ae00: 202f 2073 7464 310a 2020 2020 2020 2020   / std1.        
-0001ae10: 7932 5f6e 6f72 6d61 6c20 3d20 2879 3220  y2_normal = (y2 
-0001ae20: 2d20 7932 2e6d 6561 6e28 2929 202f 2073  - y2.mean()) / s
-0001ae30: 7464 320a 2020 2020 656c 7365 3a0a 2020  td2.    else:.  
-0001ae40: 2020 2020 2020 7931 5f6e 6f72 6d61 6c20        y1_normal 
-0001ae50: 3d20 7931 0a20 2020 2020 2020 2079 325f  = y1.        y2_
-0001ae60: 6e6f 726d 616c 203d 2079 320a 0a20 2020  normal = y2..   
-0001ae70: 2023 2043 616c 6375 6c61 7465 7320 7468   # Calculates th
-0001ae80: 6520 4357 5420 6f66 2074 6865 2074 696d  e CWT of the tim
-0001ae90: 652d 7365 7269 6573 206d 616b 696e 6720  e-series making 
-0001aea0: 7375 7265 2074 6865 2073 616d 6520 7061  sure the same pa
-0001aeb0: 7261 6d65 7465 7273 0a20 2020 2023 2061  rameters.    # a
-0001aec0: 7265 2075 7365 6420 696e 2062 6f74 6820  re used in both 
-0001aed0: 6361 6c63 756c 6174 696f 6e73 2e0a 2020  calculations..  
-0001aee0: 2020 5f6b 7761 7267 7320 3d20 6469 6374    _kwargs = dict
-0001aef0: 2864 6a3d 646a 2c20 7330 3d73 302c 204a  (dj=dj, s0=s0, J
-0001af00: 3d4a 2c20 7761 7665 6c65 743d 7761 7665  =J, wavelet=wave
-0001af10: 6c65 7429 0a20 2020 2057 312c 2073 6a2c  let).    W1, sj,
-0001af20: 2066 7265 712c 2063 6f69 2c20 5f2c 205f   freq, coi, _, _
-0001af30: 203d 2070 7963 7774 2e63 7774 2879 315f   = pycwt.cwt(y1_
-0001af40: 6e6f 726d 616c 2c20 6474 2c20 2a2a 5f6b  normal, dt, **_k
-0001af50: 7761 7267 7329 0a20 2020 2057 322c 2073  wargs).    W2, s
-0001af60: 6a2c 2066 7265 712c 2063 6f69 2c20 5f2c  j, freq, coi, _,
-0001af70: 205f 203d 2070 7963 7774 2e63 7774 2879   _ = pycwt.cwt(y
-0001af80: 325f 6e6f 726d 616c 2c20 6474 2c20 2a2a  2_normal, dt, **
-0001af90: 5f6b 7761 7267 7329 0a0a 2020 2020 7363  _kwargs)..    sc
-0001afa0: 616c 6573 3120 3d20 6e70 2e6f 6e65 7328  ales1 = np.ones(
-0001afb0: 5b31 2c20 7931 2e73 697a 655d 2920 2a20  [1, y1.size]) * 
-0001afc0: 736a 5b3a 2c20 4e6f 6e65 5d0a 2020 2020  sj[:, None].    
-0001afd0: 7363 616c 6573 3220 3d20 6e70 2e6f 6e65  scales2 = np.one
-0001afe0: 7328 5b31 2c20 7932 2e73 697a 655d 2920  s([1, y2.size]) 
-0001aff0: 2a20 736a 5b3a 2c20 4e6f 6e65 5d0a 0a20  * sj[:, None].. 
-0001b000: 2020 2023 2053 6d6f 6f74 6820 7468 6520     # Smooth the 
-0001b010: 7761 7665 6c65 7420 7370 6563 7472 6120  wavelet spectra 
-0001b020: 6265 666f 7265 2074 7275 6e63 6174 696e  before truncatin
-0001b030: 672e 0a20 2020 2053 3120 3d20 7761 7665  g..    S1 = wave
-0001b040: 6c65 742e 736d 6f6f 7468 286e 702e 6162  let.smooth(np.ab
-0001b050: 7328 5731 2920 2a2a 2032 202f 2073 6361  s(W1) ** 2 / sca
-0001b060: 6c65 7331 2c20 6474 2c20 646a 2c20 736a  les1, dt, dj, sj
-0001b070: 290a 2020 2020 5332 203d 2077 6176 656c  ).    S2 = wavel
-0001b080: 6574 2e73 6d6f 6f74 6828 6e70 2e61 6273  et.smooth(np.abs
-0001b090: 2857 3229 202a 2a20 3220 2f20 7363 616c  (W2) ** 2 / scal
-0001b0a0: 6573 322c 2064 742c 2064 6a2c 2073 6a29  es2, dt, dj, sj)
-0001b0b0: 0a0a 2020 2020 2320 4e6f 7720 7468 6520  ..    # Now the 
-0001b0c0: 7761 7665 6c65 7420 7472 616e 7366 6f72  wavelet transfor
-0001b0d0: 6d20 636f 6865 7265 6e63 650a 2020 2020  m coherence.    
-0001b0e0: 5731 3220 3d20 5731 202a 2057 322e 636f  W12 = W1 * W2.co
-0001b0f0: 6e6a 2829 0a20 2020 2073 6361 6c65 7320  nj().    scales 
-0001b100: 3d20 6e70 2e6f 6e65 7328 5b31 2c20 7931  = np.ones([1, y1
-0001b110: 2e73 697a 655d 2920 2a20 736a 5b3a 2c20  .size]) * sj[:, 
-0001b120: 4e6f 6e65 5d0a 2020 2020 5331 3220 3d20  None].    S12 = 
-0001b130: 7761 7665 6c65 742e 736d 6f6f 7468 2857  wavelet.smooth(W
-0001b140: 3132 202f 2073 6361 6c65 732c 2064 742c  12 / scales, dt,
-0001b150: 2064 6a2c 2073 6a29 0a20 2020 2057 4354   dj, sj).    WCT
-0001b160: 203d 206e 702e 6162 7328 5331 3229 202a   = np.abs(S12) *
-0001b170: 2a20 3220 2f20 2853 3120 2a20 5332 290a  * 2 / (S1 * S2).
-0001b180: 2020 2020 6157 4354 203d 206e 702e 616e      aWCT = np.an
-0001b190: 676c 6528 5731 3229 0a0a 2020 2020 2320  gle(W12)..    # 
-0001b1a0: 4361 6c63 756c 6174 6573 2074 6865 2073  Calculates the s
-0001b1b0: 6967 6e69 6669 6361 6e63 6520 7573 696e  ignificance usin
-0001b1c0: 6720 4d6f 6e74 6520 4361 726c 6f20 7369  g Monte Carlo si
-0001b1d0: 6d75 6c61 7469 6f6e 7320 7769 7468 2039  mulations with 9
-0001b1e0: 3525 0a20 2020 2023 2063 6f6e 6669 6465  5%.    # confide
-0001b1f0: 6e63 6520 6173 2061 2066 756e 6374 696f  nce as a functio
-0001b200: 6e20 6f66 2073 6361 6c65 2e0a 0a20 2020  n of scale...   
-0001b210: 2069 6620 7369 673a 0a20 2020 2020 2020   if sig:.       
-0001b220: 2061 312c 2062 312c 2063 3120 3d20 7079   a1, b1, c1 = py
-0001b230: 6377 742e 6172 3128 7931 290a 2020 2020  cwt.ar1(y1).    
-0001b240: 2020 2020 6132 2c20 6232 2c20 6332 203d      a2, b2, c2 =
-0001b250: 2070 7963 7774 2e61 7231 2879 3229 0a20   pycwt.ar1(y2). 
-0001b260: 2020 2020 2020 2073 6967 203d 2070 7963         sig = pyc
-0001b270: 7774 2e77 6374 5f73 6967 6e69 6669 6361  wt.wct_significa
-0001b280: 6e63 6528 0a20 2020 2020 2020 2020 2020  nce(.           
-0001b290: 2061 312c 2061 322c 2064 743d 6474 2c20   a1, a2, dt=dt, 
-0001b2a0: 646a 3d64 6a2c 2073 303d 7330 2c20 4a3d  dj=dj, s0=s0, J=
-0001b2b0: 4a2c 2073 6967 6e69 6669 6361 6e63 655f  J, significance_
-0001b2c0: 6c65 7665 6c3d 7369 676e 6966 6963 616e  level=significan
-0001b2d0: 6365 5f6c 6576 656c 2c20 7761 7665 6c65  ce_level, wavele
-0001b2e0: 743d 7761 7665 6c65 742c 202a 2a6b 7761  t=wavelet, **kwa
-0001b2f0: 7267 730a 2020 2020 2020 2020 290a 2020  rgs.        ).  
-0001b300: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0001b310: 7369 6720 3d20 6e70 2e61 7361 7272 6179  sig = np.asarray
-0001b320: 285b 305d 290a 0a20 2020 2072 6574 7572  ([0])..    retur
-0001b330: 6e20 5743 542c 2061 5743 542c 2063 6f69  n WCT, aWCT, coi
-0001b340: 2c20 6672 6571 2c20 7369 670a 0a0a 2323  , freq, sig...##
-0001b350: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00018350: 2323 2323 2323 2323 0a0a 2222 220a 6265  ########..""".be
+00018360: 6c6f 7720 6172 6520 6173 7365 6d62 6c79  low are assembly
+00018370: 206f 6620 7468 6520 6d6f 6e69 746f 7269   of the monitori
+00018380: 6e67 2075 7469 6c69 7479 2066 756e 6374  ng utility funct
+00018390: 696f 6e73 2063 616c 6c65 6420 6279 206d  ions called by m
+000183a0: 6f6e 6974 6f72 696e 6720 6675 6e63 7469  onitoring functi
+000183b0: 6f6e 730a 2222 220a 0a0a 6465 6620 736d  ons."""...def sm
+000183c0: 6f6f 7468 2878 2c20 7769 6e64 6f77 3d22  ooth(x, window="
+000183d0: 626f 7863 6172 222c 2068 616c 665f 7769  boxcar", half_wi
+000183e0: 6e3d 3329 3a0a 2020 2020 2222 220a 2020  n=3):.    """.  
+000183f0: 2020 7065 7266 6f72 6d73 2073 6d6f 6f74    performs smoot
+00018400: 6869 6e67 2069 6e20 696e 7465 7265 7374  hing in interest
+00018410: 6564 2074 696d 6520 7769 6e64 6f77 0a0a  ed time window..
+00018420: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00018430: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
+00018440: 2d0a 2020 2020 783a 2074 696d 6573 6572  -.    x: timeser
+00018450: 6973 2064 6174 610a 2020 2020 7769 6e64  is data.    wind
+00018460: 6f77 3a20 7479 7065 7320 6f66 2077 696e  ow: types of win
+00018470: 646f 7720 746f 2064 6f20 736d 6f6f 7468  dow to do smooth
+00018480: 696e 670a 2020 2020 6861 6c66 5f77 696e  ing.    half_win
+00018490: 3a20 6861 6c66 2077 696e 646f 7720 6c65  : half window le
+000184a0: 6e67 7468 0a0a 2020 2020 5245 5455 524e  ngth..    RETURN
+000184b0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+000184c0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 793a  ---------.    y:
+000184d0: 2073 6d6f 6f74 6865 6420 7469 6d65 2077   smoothed time w
+000184e0: 696e 646f 770a 2020 2020 2222 220a 2020  indow.    """.  
+000184f0: 2020 2320 544f 444f 3a20 646f 6373 7469    # TODO: docsti
+00018500: 6e67 0a20 2020 2077 696e 646f 775f 6c65  ng.    window_le
+00018510: 6e20 3d20 3220 2a20 6861 6c66 5f77 696e  n = 2 * half_win
+00018520: 202b 2031 0a20 2020 2023 2065 7874 656e   + 1.    # exten
+00018530: 6469 6e67 2074 6865 2064 6174 6120 6174  ding the data at
+00018540: 2062 6567 696e 6e69 6e67 2061 6e64 2061   beginning and a
+00018550: 7420 7468 6520 656e 640a 2020 2020 2320  t the end.    # 
+00018560: 746f 2061 7070 6c79 2074 6865 2077 696e  to apply the win
+00018570: 646f 7720 6174 2074 6865 2062 6f72 6465  dow at the borde
+00018580: 7273 0a20 2020 2073 203d 206e 702e 725f  rs.    s = np.r_
+00018590: 5b78 5b77 696e 646f 775f 6c65 6e20 2d20  [x[window_len - 
+000185a0: 3120 3a20 3020 3a20 2d31 5d2c 2078 2c20  1 : 0 : -1], x, 
+000185b0: 785b 2d31 3a2d 7769 6e64 6f77 5f6c 656e  x[-1:-window_len
+000185c0: 3a2d 315d 5d0a 2020 2020 6966 2077 696e  :-1]].    if win
+000185d0: 646f 7720 3d3d 2022 626f 7863 6172 223a  dow == "boxcar":
+000185e0: 0a20 2020 2020 2020 2077 203d 2073 6369  .        w = sci
+000185f0: 7079 2e73 6967 6e61 6c2e 626f 7863 6172  py.signal.boxcar
+00018600: 2877 696e 646f 775f 6c65 6e29 2e61 7374  (window_len).ast
+00018610: 7970 6528 2263 6f6d 706c 6578 2229 0a20  ype("complex"). 
+00018620: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00018630: 2077 203d 2073 6369 7079 2e73 6967 6e61   w = scipy.signa
+00018640: 6c2e 6861 6e6e 696e 6728 7769 6e64 6f77  l.hanning(window
+00018650: 5f6c 656e 292e 6173 7479 7065 2822 636f  _len).astype("co
+00018660: 6d70 6c65 7822 290a 2020 2020 7920 3d20  mplex").    y = 
+00018670: 6e70 2e63 6f6e 766f 6c76 6528 7720 2f20  np.convolve(w / 
+00018680: 772e 7375 6d28 292c 2073 2c20 6d6f 6465  w.sum(), s, mode
+00018690: 3d22 7661 6c69 6422 290a 2020 2020 7265  ="valid").    re
+000186a0: 7475 726e 2079 5b68 616c 665f 7769 6e20  turn y[half_win 
+000186b0: 3a20 6c65 6e28 7929 202d 2068 616c 665f  : len(y) - half_
+000186c0: 7769 6e5d 0a0a 0a64 6566 206e 6578 7470  win]...def nextp
+000186d0: 6f77 3228 7829 3a0a 2020 2020 2222 220a  ow2(x):.    """.
+000186e0: 2020 2020 5265 7475 726e 7320 7468 6520      Returns the 
+000186f0: 6e65 7874 2070 6f77 6572 206f 6620 3220  next power of 2 
+00018700: 6f66 2078 2e0a 2020 2020 2222 220a 2020  of x..    """.  
+00018710: 2020 7265 7475 726e 2069 6e74 286e 702e    return int(np.
+00018720: 6365 696c 286e 702e 6c6f 6732 286e 702e  ceil(np.log2(np.
+00018730: 6162 7328 7829 2929 290a 0a0a 6465 6620  abs(x))))...def 
+00018740: 6765 7443 6f68 6572 656e 6365 2864 6373  getCoherence(dcs
+00018750: 2c20 6473 312c 2064 7332 293a 0a20 2020  , ds1, ds2):.   
+00018760: 2022 2222 0a20 2020 2067 6574 2063 726f   """.    get cro
+00018770: 7373 2063 6f68 6572 656e 6365 2062 6574  ss coherence bet
+00018780: 7765 656e 2072 6566 6572 656e 6365 2061  ween reference a
+00018790: 6e64 2063 7572 7265 6e74 2077 6176 6566  nd current wavef
+000187a0: 6f72 6d73 2066 6f6c 6c6f 7769 6e67 2065  orms following e
+000187b0: 7175 6174 696f 6e20 6f66 2041 3320 696e  quation of A3 in
+000187c0: 2043 6c61 726b 2065 7420 616c 2e2c 2032   Clark et al., 2
+000187d0: 3031 310a 0a20 2020 2050 6172 616d 6574  011..    Paramet
+000187e0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+000187f0: 2d2d 2d2d 2d2d 0a20 2020 2064 6373 3a20  ------.    dcs: 
+00018800: 616d 706c 6974 7564 6520 6f66 2074 6865  amplitude of the
+00018810: 2063 726f 7373 2073 7065 6374 7275 6d0a   cross spectrum.
+00018820: 2020 2020 6473 313a 2061 6d70 6c69 7475      ds1: amplitu
+00018830: 6465 206f 6620 7468 6520 7370 6563 7472  de of the spectr
+00018840: 756d 206f 6620 6375 7272 656e 7420 7761  um of current wa
+00018850: 7665 666f 726d 0a20 2020 2064 7332 3a20  veform.    ds2: 
+00018860: 616d 706c 6974 7564 6520 6f66 2074 6865  amplitude of the
+00018870: 2073 7065 6374 7275 6d20 6f66 2072 6566   spectrum of ref
+00018880: 6572 656e 6365 2077 6176 6566 6f72 6d0a  erence waveform.
+00018890: 0a20 2020 2052 4554 5552 4e53 3a0a 2020  .    RETURNS:.  
+000188a0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d    --------------
+000188b0: 2d2d 2d2d 0a20 2020 2063 6f68 3a20 636f  ----.    coh: co
+000188c0: 6872 6572 656e 6379 206d 6174 7269 7820  hrerency matrix 
+000188d0: 7573 6564 2066 6f72 2065 7374 696d 6174  used for estimat
+000188e0: 6520 7468 6520 726f 6275 7374 6e65 7373  e the robustness
+000188f0: 206f 6620 7468 6520 6372 6f73 7320 7370   of the cross sp
+00018900: 6563 7472 756d 0a20 2020 2022 2222 0a20  ectrum.    """. 
+00018910: 2020 206e 203d 206c 656e 2864 6373 290a     n = len(dcs).
+00018920: 2020 2020 636f 6820 3d20 6e70 2e7a 6572      coh = np.zer
+00018930: 6f73 286e 292e 6173 7479 7065 2822 636f  os(n).astype("co
+00018940: 6d70 6c65 7822 290a 2020 2020 7661 6c69  mplex").    vali
+00018950: 6473 203d 206e 702e 6172 6777 6865 7265  ds = np.argwhere
+00018960: 286e 702e 6c6f 6769 6361 6c5f 616e 6428  (np.logical_and(
+00018970: 6e70 2e61 6273 2864 7331 2920 3e20 302c  np.abs(ds1) > 0,
+00018980: 206e 702e 6162 7328 6473 3229 203e 2030   np.abs(ds2) > 0
+00018990: 2929 0a20 2020 2063 6f68 5b76 616c 6964  )).    coh[valid
+000189a0: 735d 203d 2064 6373 5b76 616c 6964 735d  s] = dcs[valids]
+000189b0: 202f 2028 6473 315b 7661 6c69 6473 5d20   / (ds1[valids] 
+000189c0: 2a20 6473 325b 7661 6c69 6473 5d29 0a20  * ds2[valids]). 
+000189d0: 2020 2063 6f68 5b63 6f68 203e 2028 312e     coh[coh > (1.
+000189e0: 3020 2b20 306a 295d 203d 2031 2e30 202b  0 + 0j)] = 1.0 +
+000189f0: 2030 6a0a 2020 2020 7265 7475 726e 2063   0j.    return c
+00018a00: 6f68 0a0a 0a64 6566 2063 6f6d 7075 7465  oh...def compute
+00018a10: 4572 726f 7246 756e 6374 696f 6e28 7531  ErrorFunction(u1
+00018a20: 2c20 7530 2c20 6e53 616d 706c 652c 206c  , u0, nSample, l
+00018a30: 6167 2c20 6e6f 726d 3d22 4c32 2229 3a0a  ag, norm="L2"):.
+00018a40: 2020 2020 2222 220a 2020 2020 636f 6d70      """.    comp
+00018a50: 7574 6520 4572 726f 7220 4675 6e63 7469  ute Error Functi
+00018a60: 6f6e 2075 7365 6420 696e 2044 5457 2e20  on used in DTW. 
+00018a70: 5468 6520 6572 726f 7220 6675 6e63 7469  The error functi
+00018a80: 6f6e 2069 7320 6571 7561 7469 6f6e 2031  on is equation 1
+00018a90: 2069 6e20 4861 6c65 2c20 3230 3133 2e20   in Hale, 2013. 
+00018aa0: 596f 7520 636f 756c 6420 756e 636f 6d6d  You could uncomm
+00018ab0: 656e 7420 7468 650a 2020 2020 4c31 206e  ent the.    L1 n
+00018ac0: 6f72 6d20 616e 6420 636f 6d6d 656e 7420  orm and comment 
+00018ad0: 7468 6520 4c32 206e 6f72 6d20 6966 2079  the L2 norm if y
+00018ae0: 6f75 2077 616e 7420 6f6e 204c 696e 6520  ou want on Line 
+00018af0: 3239 0a0a 2020 2020 5061 7261 6d65 7465  29..    Paramete
+00018b00: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+00018b10: 2d2d 2d2d 2d0a 2020 2020 7531 3a20 2074  -----.    u1:  t
+00018b20: 7261 6365 2074 6861 7420 7765 2077 616e  race that we wan
+00018b30: 7420 746f 2077 6172 703b 2073 697a 6520  t to warp; size 
+00018b40: 3d20 286e 7361 6d70 2c31 290a 2020 2020  = (nsamp,1).    
+00018b50: 7530 3a20 2072 6566 6572 656e 6365 2074  u0:  reference t
+00018b60: 7261 6365 2074 6f20 636f 6d70 6172 6520  race to compare 
+00018b70: 7769 7468 3a20 7369 7a65 203d 2028 6e73  with: size = (ns
+00018b80: 616d 702c 3129 0a20 2020 206e 5361 6d70  amp,1).    nSamp
+00018b90: 6c65 3a20 6e75 6d65 7220 6f66 2070 6f69  le: numer of poi
+00018ba0: 6e74 7320 746f 2063 6f6d 7061 7265 2069  nts to compare i
+00018bb0: 6e20 7468 6520 7472 6163 6573 0a20 2020  n the traces.   
+00018bc0: 206c 6167 3a20 6d61 7869 6d75 6d20 6c61   lag: maximum la
+00018bd0: 6720 696e 2073 616d 706c 6520 6e75 6d62  g in sample numb
+00018be0: 6572 2074 6f20 7365 6172 6368 0a20 2020  er to search.   
+00018bf0: 206e 6f72 6d3a 2027 4c32 2720 6f72 2027   norm: 'L2' or '
+00018c00: 4c31 2720 2864 6566 6175 6c74 2069 7320  L1' (default is 
+00018c10: 274c 3227 290a 0a20 2020 2052 4554 5552  'L2')..    RETUR
+00018c20: 4e53 3a0a 2020 2020 2d2d 2d2d 2d2d 2d2d  NS:.    --------
+00018c30: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2065  ----------.    e
+00018c40: 7272 3a20 7468 6520 3244 2065 7272 6f72  rr: the 2D error
+00018c50: 2066 756e 6374 696f 6e3b 2073 697a 6520   function; size 
+00018c60: 3d20 286e 7361 6d70 2c32 2a6c 6167 2b31  = (nsamp,2*lag+1
+00018c70: 290a 0a20 2020 204f 7269 6769 6e61 6c20  )..    Original 
+00018c80: 6279 2044 6920 5961 6e67 0a20 2020 204c  by Di Yang.    L
+00018c90: 6173 7420 6d6f 6469 6669 6564 2062 7920  ast modified by 
+00018ca0: 4479 6c61 6e20 4d69 6b65 7365 6c6c 2028  Dylan Mikesell (
+00018cb0: 3235 2046 6562 2e20 3230 3135 290a 2020  25 Feb. 2015).  
+00018cc0: 2020 5472 616e 736c 6174 6564 2074 6f20    Translated to 
+00018cd0: 7079 7468 6f6e 2062 7920 5469 6d20 436c  python by Tim Cl
+00018ce0: 656d 656e 7473 2028 3137 2041 7567 2e20  ements (17 Aug. 
+00018cf0: 3230 3138 290a 0a20 2020 2022 2222 0a0a  2018)..    """..
+00018d00: 2020 2020 6966 206c 6167 203e 3d20 6e53      if lag >= nS
+00018d10: 616d 706c 653a 0a20 2020 2020 2020 2072  ample:.        r
+00018d20: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00018d30: 2263 6f6d 7075 7465 4572 726f 7246 756e  "computeErrorFun
+00018d40: 6374 696f 6e3a 6c61 6750 726f 626c 656d  ction:lagProblem
+00018d50: 222c 2022 6c61 6720 6d75 7374 2062 6520  ", "lag must be 
+00018d60: 736d 616c 6c65 7220 7468 616e 206e 5361  smaller than nSa
+00018d70: 6d70 6c65 2229 0a0a 2020 2020 2320 416c  mple")..    # Al
+00018d80: 6c6f 6361 7465 2065 7272 6f72 2066 756e  locate error fun
+00018d90: 6374 696f 6e20 7661 7269 6162 6c65 0a20  ction variable. 
+00018da0: 2020 2065 7272 203d 206e 702e 7a65 726f     err = np.zero
+00018db0: 7328 5b6e 5361 6d70 6c65 2c20 3220 2a20  s([nSample, 2 * 
+00018dc0: 6c61 6720 2b20 315d 290a 0a20 2020 2023  lag + 1])..    #
+00018dd0: 2069 6e69 7469 616c 2065 7272 6f72 2063   initial error c
+00018de0: 616c 6375 6c61 7469 6f6e 0a20 2020 2023  alculation.    #
+00018df0: 206c 6f6f 7020 6f76 6572 206c 6167 730a   loop over lags.
+00018e00: 2020 2020 666f 7220 6c6c 2069 6e20 6e70      for ll in np
+00018e10: 2e61 7261 6e67 6528 2d6c 6167 2c20 6c61  .arange(-lag, la
+00018e20: 6720 2b20 3129 3a0a 2020 2020 2020 2020  g + 1):.        
+00018e30: 7468 6973 4c61 6720 3d20 6c6c 202b 206c  thisLag = ll + l
+00018e40: 6167 0a0a 2020 2020 2020 2020 2320 6c6f  ag..        # lo
+00018e50: 6f70 206f 7665 7220 7361 6d70 6c65 730a  op over samples.
+00018e60: 2020 2020 2020 2020 666f 7220 6969 2069          for ii i
+00018e70: 6e20 7261 6e67 6528 6e53 616d 706c 6529  n range(nSample)
+00018e80: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00018e90: 736b 6970 2063 6f72 6e65 7273 2066 6f72  skip corners for
+00018ea0: 206e 6f77 2c20 7765 2077 696c 6c20 636f   now, we will co
+00018eb0: 6d65 2062 6163 6b20 746f 2074 6865 7365  me back to these
+00018ec0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00018ed0: 2869 6920 2b20 6c6c 203e 3d20 3029 2026  (ii + ll >= 0) &
+00018ee0: 2028 6969 202b 206c 6c20 3c20 6e53 616d   (ii + ll < nSam
+00018ef0: 706c 6529 3a0a 2020 2020 2020 2020 2020  ple):.          
+00018f00: 2020 2020 2020 6572 725b 6969 2c20 7468        err[ii, th
+00018f10: 6973 4c61 675d 203d 2075 315b 6969 5d20  isLag] = u1[ii] 
+00018f20: 2d20 7530 5b69 6920 2b20 6c6c 5d0a 0a20  - u0[ii + ll].. 
+00018f30: 2020 2069 6620 6e6f 726d 203d 3d20 224c     if norm == "L
+00018f40: 3222 3a0a 2020 2020 2020 2020 6572 7220  2":.        err 
+00018f50: 3d20 6572 722a 2a32 0a20 2020 2065 6c69  = err**2.    eli
+00018f60: 6620 6e6f 726d 203d 3d20 224c 3122 3a0a  f norm == "L1":.
+00018f70: 2020 2020 2020 2020 6572 7220 3d20 6e70          err = np
+00018f80: 2e61 6273 2865 7272 290a 0a20 2020 2023  .abs(err)..    #
+00018f90: 204e 6f77 2066 6978 2063 6f72 6e65 7273   Now fix corners
+00018fa0: 2077 6974 6820 636f 6e73 7461 6e74 2065   with constant e
+00018fb0: 7874 7261 706f 6c61 7469 6f6e 0a20 2020  xtrapolation.   
+00018fc0: 2066 6f72 206c 6c20 696e 206e 702e 6172   for ll in np.ar
+00018fd0: 616e 6765 282d 6c61 672c 206c 6167 202b  ange(-lag, lag +
+00018fe0: 2031 293a 0a20 2020 2020 2020 2074 6869   1):.        thi
+00018ff0: 734c 6167 203d 206c 6c20 2b20 6c61 670a  sLag = ll + lag.
+00019000: 0a20 2020 2020 2020 2066 6f72 2069 6920  .        for ii 
+00019010: 696e 2072 616e 6765 286e 5361 6d70 6c65  in range(nSample
+00019020: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00019030: 6620 6969 202b 206c 6c20 3c20 303a 0a20  f ii + ll < 0:. 
+00019040: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00019050: 7272 5b69 692c 2074 6869 734c 6167 5d20  rr[ii, thisLag] 
+00019060: 3d20 6572 725b 2d6c 6c2c 2074 6869 734c  = err[-ll, thisL
+00019070: 6167 5d0a 0a20 2020 2020 2020 2020 2020  ag]..           
+00019080: 2065 6c69 6620 6969 202b 206c 6c20 3e20   elif ii + ll > 
+00019090: 6e53 616d 706c 6520 2d20 313a 0a20 2020  nSample - 1:.   
+000190a0: 2020 2020 2020 2020 2020 2020 2065 7272               err
+000190b0: 5b69 692c 2074 6869 734c 6167 5d20 3d20  [ii, thisLag] = 
+000190c0: 6572 725b 6e53 616d 706c 6520 2d20 6c6c  err[nSample - ll
+000190d0: 202d 2031 2c20 7468 6973 4c61 675d 0a0a   - 1, thisLag]..
+000190e0: 2020 2020 7265 7475 726e 2065 7272 0a0a      return err..
+000190f0: 0a64 6566 2061 6363 756d 756c 6174 6545  .def accumulateE
+00019100: 7272 6f72 4675 6e63 7469 6f6e 2864 6972  rrorFunction(dir
+00019110: 2c20 6572 722c 206e 5361 6d70 6c65 2c20  , err, nSample, 
+00019120: 6c61 672c 2062 293a 0a20 2020 2022 2222  lag, b):.    """
+00019130: 0a20 2020 2061 6363 756d 756c 6174 696f  .    accumulatio
+00019140: 6e20 6f66 2074 6865 2065 7272 6f72 2c20  n of the error, 
+00019150: 7768 6963 6820 666f 6c6c 6f77 7320 7468  which follows th
+00019160: 6520 6571 7561 7469 6f6e 2036 2069 6e20  e equation 6 in 
+00019170: 4861 6c65 2c20 3230 3133 2e0a 0a20 2020  Hale, 2013...   
+00019180: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+00019190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  --------------. 
+000191a0: 2020 2064 6972 3a20 6163 6375 6d75 6c61     dir: accumula
+000191b0: 7469 6f6e 2064 6972 6563 7469 6f6e 2028  tion direction (
+000191c0: 2064 6972 203e 2030 203d 2066 6f72 7761   dir > 0 = forwa
+000191d0: 7264 2069 6e20 7469 6d65 2c20 6469 7220  rd in time, dir 
+000191e0: 3c3d 2030 203d 2062 6163 6b77 6172 6420  <= 0 = backward 
+000191f0: 696e 2074 696d 6529 0a20 2020 2065 7272  in time).    err
+00019200: 3a20 7468 6520 3244 2065 7272 6f72 2066  : the 2D error f
+00019210: 756e 6374 696f 6e3b 2073 697a 6520 3d20  unction; size = 
+00019220: 286e 7361 6d70 2c32 2a6c 6167 2b31 290a  (nsamp,2*lag+1).
+00019230: 2020 2020 6e53 616d 706c 653a 206e 756d      nSample: num
+00019240: 6572 206f 6620 706f 696e 7473 2074 6f20  er of points to 
+00019250: 636f 6d70 6172 6520 696e 2074 6865 2074  compare in the t
+00019260: 7261 6365 730a 2020 2020 6c61 673a 206d  races.    lag: m
+00019270: 6178 696d 756d 206c 6167 2069 6e20 7361  aximum lag in sa
+00019280: 6d70 6c65 206e 756d 6265 7220 746f 2073  mple number to s
+00019290: 6561 7263 680a 2020 2020 623a 2073 7472  earch.    b: str
+000192a0: 6169 6e20 6c69 6d69 7420 2869 6e74 6567  ain limit (integ
+000192b0: 6572 2076 616c 7565 203e 3d20 3129 0a0a  er value >= 1)..
+000192c0: 2020 2020 5245 5455 524e 533a 0a20 2020      RETURNS:.   
+000192d0: 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   ---------------
+000192e0: 2d2d 2d0a 2020 2020 643a 2074 6865 2032  ---.    d: the 2
+000192f0: 4420 6469 7374 616e 6365 2066 756e 6374  D distance funct
+00019300: 696f 6e3b 2073 697a 6520 3d20 286e 7361  ion; size = (nsa
+00019310: 6d70 2c32 2a6c 6167 2b31 290a 0a20 2020  mp,2*lag+1)..   
+00019320: 204f 7269 6769 6e61 6c20 6279 2044 6920   Original by Di 
+00019330: 5961 6e67 0a20 2020 204c 6173 7420 6d6f  Yang.    Last mo
+00019340: 6469 6669 6564 2062 7920 4479 6c61 6e20  dified by Dylan 
+00019350: 4d69 6b65 7365 6c6c 2028 3235 2046 6562  Mikesell (25 Feb
+00019360: 2e20 3230 3135 290a 2020 2020 5472 616e  . 2015).    Tran
+00019370: 736c 6174 6564 2074 6f20 7079 7468 6f6e  slated to python
+00019380: 2062 7920 5469 6d20 436c 656d 656e 7473   by Tim Clements
+00019390: 2028 3137 2041 7567 2e20 3230 3138 290a   (17 Aug. 2018).
+000193a0: 0a20 2020 2022 2222 0a0a 2020 2020 2320  .    """..    # 
+000193b0: 6e75 6d62 6572 206f 6620 6c61 6773 2066  number of lags f
+000193c0: 726f 6d20 5b20 2d6c 6167 203a 202b 6c61  rom [ -lag : +la
+000193d0: 6720 5d0a 2020 2020 6e4c 6167 203d 2028  g ].    nLag = (
+000193e0: 3220 2a20 6c61 6729 202b 2031 0a0a 2020  2 * lag) + 1..  
+000193f0: 2020 2320 616c 6c6f 6361 7465 2064 6973    # allocate dis
+00019400: 7461 6e63 6520 6d61 7472 6978 0a20 2020  tance matrix.   
+00019410: 2064 203d 206e 702e 7a65 726f 7328 5b6e   d = np.zeros([n
+00019420: 5361 6d70 6c65 2c20 6e4c 6167 5d29 0a0a  Sample, nLag])..
+00019430: 2020 2020 2320 5365 7475 7020 696e 6469      # Setup indi
+00019440: 6365 7320 6261 7365 6420 6f6e 2066 6f72  ces based on for
+00019450: 7761 7264 206f 7220 6261 636b 7761 7264  ward or backward
+00019460: 2061 6363 756d 756c 6174 696f 6e20 6469   accumulation di
+00019470: 7265 6374 696f 6e0a 2020 2020 6966 2064  rection.    if d
+00019480: 6972 203e 2030 3a20 2023 2046 4f52 5741  ir > 0:  # FORWA
+00019490: 5244 0a20 2020 2020 2020 2069 4265 6769  RD.        iBegi
+000194a0: 6e2c 2069 456e 642c 2069 496e 6320 3d20  n, iEnd, iInc = 
+000194b0: 302c 206e 5361 6d70 6c65 202d 2031 2c20  0, nSample - 1, 
+000194c0: 310a 2020 2020 656c 7365 3a20 2023 2042  1.    else:  # B
+000194d0: 4143 4b57 4152 440a 2020 2020 2020 2020  ACKWARD.        
+000194e0: 6942 6567 696e 2c20 6945 6e64 2c20 6949  iBegin, iEnd, iI
+000194f0: 6e63 203d 206e 5361 6d70 6c65 202d 2031  nc = nSample - 1
+00019500: 2c20 302c 202d 310a 0a20 2020 2023 204c  , 0, -1..    # L
+00019510: 6f6f 7020 7468 726f 7567 6820 616c 6c20  oop through all 
+00019520: 7469 6d65 7320 6969 2069 6e20 666f 7277  times ii in forw
+00019530: 6172 6420 6f72 2062 6163 6b77 6172 6420  ard or backward 
+00019540: 6469 7265 6374 696f 6e0a 2020 2020 666f  direction.    fo
+00019550: 7220 6969 2069 6e20 7261 6e67 6528 6942  r ii in range(iB
+00019560: 6567 696e 2c20 6945 6e64 202b 2069 496e  egin, iEnd + iIn
+00019570: 632c 2069 496e 6329 3a0a 2020 2020 2020  c, iInc):.      
+00019580: 2020 2320 6d69 6e2f 6d61 7820 746f 2061    # min/max to a
+00019590: 6363 6f75 6e74 2066 6f72 2074 6865 2065  ccount for the e
+000195a0: 6467 6573 2f62 6f75 6e64 6172 6965 730a  dges/boundaries.
+000195b0: 2020 2020 2020 2020 6a69 203d 206d 6178          ji = max
+000195c0: 285b 302c 206d 696e 285b 6e53 616d 706c  ([0, min([nSampl
+000195d0: 6520 2d20 312c 2069 6920 2d20 6949 6e63  e - 1, ii - iInc
+000195e0: 5d29 5d29 0a20 2020 2020 2020 206a 6220  ])]).        jb 
+000195f0: 3d20 6d61 7828 5b30 2c20 6d69 6e28 5b6e  = max([0, min([n
+00019600: 5361 6d70 6c65 202d 2031 2c20 6969 202d  Sample - 1, ii -
+00019610: 2069 496e 6320 2a20 625d 295d 290a 0a20   iInc * b])]).. 
+00019620: 2020 2020 2020 2023 206c 6f6f 7020 7468         # loop th
+00019630: 726f 7567 6820 616c 6c20 6c61 670a 2020  rough all lag.  
+00019640: 2020 2020 2020 666f 7220 6c6c 2069 6e20        for ll in 
+00019650: 7261 6e67 6528 6e4c 6167 293a 0a20 2020  range(nLag):.   
+00019660: 2020 2020 2020 2020 2023 2063 6865 636b           # check
+00019670: 206c 696d 6974 7320 6f6e 206c 6167 2069   limits on lag i
+00019680: 6e64 6963 6573 0a20 2020 2020 2020 2020  ndices.         
+00019690: 2020 206c 4d69 6e75 7331 203d 206c 6c20     lMinus1 = ll 
+000196a0: 2d20 310a 0a20 2020 2020 2020 2020 2020  - 1..           
+000196b0: 2023 2063 6865 636b 206c 6167 2069 6e64   # check lag ind
+000196c0: 6578 2069 7320 6772 6561 7465 7220 7468  ex is greater th
+000196d0: 616e 2030 0a20 2020 2020 2020 2020 2020  an 0.           
+000196e0: 2069 6620 6c4d 696e 7573 3120 3c20 303a   if lMinus1 < 0:
+000196f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019700: 206c 4d69 6e75 7331 203d 2030 2020 2320   lMinus1 = 0  # 
+00019710: 6d61 6b65 206c 6167 203d 2066 6972 7374  make lag = first
+00019720: 206c 6167 0a0a 2020 2020 2020 2020 2020   lag..          
+00019730: 2020 6c50 6c75 7331 203d 206c 6c20 2b20    lPlus1 = ll + 
+00019740: 3120 2023 206c 6167 2061 7420 6c2b 310a  1  # lag at l+1.
+00019750: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00019760: 6865 636b 206c 6167 2069 6e64 6578 206c  heck lag index l
+00019770: 6573 7320 7468 616e 206d 6178 206c 6167  ess than max lag
+00019780: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00019790: 6c50 6c75 7331 203e 206e 4c61 6720 2d20  lPlus1 > nLag - 
+000197a0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+000197b0: 2020 206c 506c 7573 3120 3d20 6e4c 6167     lPlus1 = nLag
+000197c0: 202d 2031 0a0a 2020 2020 2020 2020 2020   - 1..          
+000197d0: 2020 2320 6765 7420 6469 7374 616e 6365    # get distance
+000197e0: 2061 7420 6c61 6773 2028 6c6c 2d31 2c20   at lags (ll-1, 
+000197f0: 6c6c 2c20 6c6c 2b31 290a 2020 2020 2020  ll, ll+1).      
+00019800: 2020 2020 2020 6469 7374 4c6d 696e 7573        distLminus
+00019810: 3120 3d20 645b 6a62 2c20 6c4d 696e 7573  1 = d[jb, lMinus
+00019820: 315d 2020 2320 6d69 6e75 733a 2020 645b  1]  # minus:  d[
+00019830: 692d 622c 206a 2d31 5d0a 2020 2020 2020  i-b, j-1].      
+00019840: 2020 2020 2020 6469 7374 4c20 3d20 645b        distL = d[
+00019850: 6a69 2c20 6c6c 5d20 2023 2061 6374 7561  ji, ll]  # actua
+00019860: 6c20 645b 692d 312c 206a 5d0a 2020 2020  l d[i-1, j].    
+00019870: 2020 2020 2020 2020 6469 7374 4c70 6c75          distLplu
+00019880: 7331 203d 2064 5b6a 622c 206c 506c 7573  s1 = d[jb, lPlus
+00019890: 315d 2020 2320 706c 7573 2064 5b69 2d62  1]  # plus d[i-b
+000198a0: 2c20 6a2b 315d 0a0a 2020 2020 2020 2020  , j+1]..        
+000198b0: 2020 2020 6966 206a 6920 213d 206a 623a      if ji != jb:
+000198c0: 2020 2320 6571 7561 7469 6f6e 2031 3020    # equation 10 
+000198d0: 696e 2048 616c 652c 2032 3031 330a 2020  in Hale, 2013.  
+000198e0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000198f0: 7220 6b62 2069 6e20 7261 6e67 6528 6a69  r kb in range(ji
+00019900: 2c20 6a62 202b 2069 496e 6320 2d20 312c  , jb + iInc - 1,
+00019910: 202d 6949 6e63 293a 0a20 2020 2020 2020   -iInc):.       
+00019920: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00019930: 744c 6d69 6e75 7331 203d 2064 6973 744c  tLminus1 = distL
+00019940: 6d69 6e75 7331 202b 2065 7272 5b6b 622c  minus1 + err[kb,
+00019950: 206c 4d69 6e75 7331 5d0a 2020 2020 2020   lMinus1].      
+00019960: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00019970: 7374 4c70 6c75 7331 203d 2064 6973 744c  stLplus1 = distL
+00019980: 706c 7573 3120 2b20 6572 725b 6b62 2c20  plus1 + err[kb, 
+00019990: 6c50 6c75 7331 5d0a 0a20 2020 2020 2020  lPlus1]..       
+000199a0: 2020 2020 2023 2065 7175 6174 696f 6e20       # equation 
+000199b0: 3620 2869 6620 623d 3129 206f 7220 3130  6 (if b=1) or 10
+000199c0: 2028 6966 2062 3e31 2920 696e 2048 616c   (if b>1) in Hal
+000199d0: 6520 2832 3031 3329 2061 6674 6572 2074  e (2013) after t
+000199e0: 7265 6174 696e 6720 626f 756e 6461 7269  reating boundari
+000199f0: 6573 0a20 2020 2020 2020 2020 2020 2064  es.            d
+00019a00: 5b69 692c 206c 6c5d 203d 2065 7272 5b69  [ii, ll] = err[i
+00019a10: 692c 206c 6c5d 202b 206d 696e 285b 6469  i, ll] + min([di
+00019a20: 7374 4c6d 696e 7573 312c 2064 6973 744c  stLminus1, distL
+00019a30: 2c20 6469 7374 4c70 6c75 7331 5d29 0a0a  , distLplus1])..
+00019a40: 2020 2020 7265 7475 726e 2064 0a0a 0a64      return d...d
+00019a50: 6566 2062 6163 6b74 7261 636b 4469 7374  ef backtrackDist
+00019a60: 616e 6365 4675 6e63 7469 6f6e 2864 6972  anceFunction(dir
+00019a70: 2c20 642c 2065 7272 2c20 6c6d 696e 2c20  , d, err, lmin, 
+00019a80: 6229 3a0a 2020 2020 2222 220a 2020 2020  b):.    """.    
+00019a90: 5468 6520 6675 6e63 7469 6f6e 2069 7320  The function is 
+00019aa0: 6571 7561 7469 6f6e 2032 2069 6e20 4861  equation 2 in Ha
+00019ab0: 6c65 2c20 3230 3133 2e0a 0a20 2020 2050  le, 2013...    P
+00019ac0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00019ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
+00019ae0: 2064 6972 3a20 7369 6465 2074 6f20 7374   dir: side to st
+00019af0: 6172 7420 6d69 6e69 6d69 7a61 7469 6f6e  art minimization
+00019b00: 2028 2064 6972 203e 2030 203d 2066 726f   ( dir > 0 = fro
+00019b10: 6e74 2c20 6469 7220 3c3d 2030 203d 2020  nt, dir <= 0 =  
+00019b20: 6261 636b 290a 2020 2020 6420 3a20 7468  back).    d : th
+00019b30: 6520 3244 2064 6973 7461 6e63 6520 6675  e 2D distance fu
+00019b40: 6e63 7469 6f6e 3b20 7369 7a65 203d 2028  nction; size = (
+00019b50: 6e73 616d 702c 322a 6c61 672b 3129 0a20  nsamp,2*lag+1). 
+00019b60: 2020 2065 7272 3a20 7468 6520 3244 2065     err: the 2D e
+00019b70: 7272 6f72 2066 756e 6374 696f 6e3b 2073  rror function; s
+00019b80: 697a 6520 3d20 286e 7361 6d70 2c32 2a6c  ize = (nsamp,2*l
+00019b90: 6167 2b31 290a 2020 2020 6c6d 696e 3a20  ag+1).    lmin: 
+00019ba0: 6d69 6e69 6d75 6d20 6c61 6720 746f 2073  minimum lag to s
+00019bb0: 6561 7263 6820 6f76 6572 0a20 2020 2062  earch over.    b
+00019bc0: 203a 2073 7472 6169 6e20 6c69 6d69 7420   : strain limit 
+00019bd0: 2869 6e74 6567 6572 2076 616c 7565 203e  (integer value >
+00019be0: 3d20 3129 0a0a 2020 2020 5245 5455 524e  = 1)..    RETURN
+00019bf0: 533a 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  S:.    ---------
+00019c00: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7374  ---------.    st
+00019c10: 6261 723a 2076 6563 746f 7220 6f66 2069  bar: vector of i
+00019c20: 6e74 6567 6572 2073 6869 6674 7320 7375  nteger shifts su
+00019c30: 626a 6563 7420 746f 207c 7528 6929 2d75  bject to |u(i)-u
+00019c40: 2869 2d31 297c 203c 3d20 312f 620a 0a20  (i-1)| <= 1/b.. 
+00019c50: 2020 204f 7269 6769 6e61 6c20 6279 2044     Original by D
+00019c60: 6920 5961 6e67 0a20 2020 204c 6173 7420  i Yang.    Last 
+00019c70: 6d6f 6469 6669 6564 2062 7920 4479 6c61  modified by Dyla
+00019c80: 6e20 4d69 6b65 7365 6c6c 2028 3139 2044  n Mikesell (19 D
+00019c90: 6563 2e20 3230 3134 290a 0a20 2020 2054  ec. 2014)..    T
+00019ca0: 7261 6e73 6c61 7465 6420 746f 2070 7974  ranslated to pyt
+00019cb0: 686f 6e20 6279 2054 696d 2043 6c65 6d65  hon by Tim Cleme
+00019cc0: 6e74 7320 2831 3720 4175 672e 2032 3031  nts (17 Aug. 201
+00019cd0: 3829 0a0a 2020 2020 2222 220a 0a20 2020  8)..    """..   
+00019ce0: 206e 5361 6d70 6c65 2c20 6e4c 6167 203d   nSample, nLag =
+00019cf0: 2064 2e73 6861 7065 0a20 2020 2073 7462   d.shape.    stb
+00019d00: 6172 203d 206e 702e 7a65 726f 7328 6e53  ar = np.zeros(nS
+00019d10: 616d 706c 6529 0a0a 2020 2020 2320 5365  ample)..    # Se
+00019d20: 7475 7020 696e 6469 6365 7320 6261 7365  tup indices base
+00019d30: 6420 6f6e 2066 6f72 7761 7264 206f 7220  d on forward or 
+00019d40: 6261 636b 7761 7264 2061 6363 756d 756c  backward accumul
+00019d50: 6174 696f 6e20 6469 7265 6374 696f 6e0a  ation direction.
+00019d60: 2020 2020 6966 2064 6972 203e 2030 3a20      if dir > 0: 
+00019d70: 2023 2046 4f52 5741 5244 0a20 2020 2020   # FORWARD.     
+00019d80: 2020 2069 4265 6769 6e2c 2069 456e 642c     iBegin, iEnd,
+00019d90: 2069 496e 6320 3d20 302c 206e 5361 6d70   iInc = 0, nSamp
+00019da0: 6c65 202d 2031 2c20 310a 2020 2020 656c  le - 1, 1.    el
+00019db0: 7365 3a20 2023 2042 4143 4b57 4152 440a  se:  # BACKWARD.
+00019dc0: 2020 2020 2020 2020 6942 6567 696e 2c20          iBegin, 
+00019dd0: 6945 6e64 2c20 6949 6e63 203d 206e 5361  iEnd, iInc = nSa
+00019de0: 6d70 6c65 202d 2031 2c20 302c 202d 310a  mple - 1, 0, -1.
+00019df0: 0a20 2020 2023 2073 7461 7274 2066 726f  .    # start fro
+00019e00: 6d20 7468 6520 656e 6420 2866 726f 6e74  m the end (front
+00019e10: 206f 7220 6261 636b 290a 2020 2020 6c6c   or back).    ll
+00019e20: 203d 206e 702e 6172 676d 696e 2864 5b69   = np.argmin(d[i
+00019e30: 4265 6769 6e2c 203a 5d29 2020 2320 6669  Begin, :])  # fi
+00019e40: 6e64 206d 696e 696d 756d 2061 6363 756d  nd minimum accum
+00019e50: 756c 6174 6564 2064 6973 7461 6e63 6520  ulated distance 
+00019e60: 6174 2066 726f 6e74 206f 7220 6261 636b  at front or back
+00019e70: 2064 6570 656e 6469 6e67 206f 6e20 2764   depending on 'd
+00019e80: 6972 270a 2020 2020 7374 6261 725b 6942  ir'.    stbar[iB
+00019e90: 6567 696e 5d20 3d20 6c6c 202b 206c 6d69  egin] = ll + lmi
+00019ea0: 6e20 2023 2061 6273 6f6c 7574 6520 7661  n  # absolute va
+00019eb0: 6c75 6520 6f66 2069 6e74 6567 6572 2073  lue of integer s
+00019ec0: 6869 6674 0a0a 2020 2020 2320 6d6f 7665  hift..    # move
+00019ed0: 2074 6872 6f75 6768 2061 6c6c 2074 696d   through all tim
+00019ee0: 6520 7361 6d70 6c65 7320 696e 2066 6f72  e samples in for
+00019ef0: 7761 7264 206f 7220 6261 636b 7761 7264  ward or backward
+00019f00: 2064 6972 6563 7469 6f6e 0a20 2020 2069   direction.    i
+00019f10: 6920 3d20 6942 6567 696e 0a0a 2020 2020  i = iBegin..    
+00019f20: 7768 696c 6520 6969 2021 3d20 6945 6e64  while ii != iEnd
+00019f30: 3a0a 2020 2020 2020 2020 2320 6d69 6e2f  :.        # min/
+00019f40: 6d61 7820 666f 7220 6564 6765 732f 626f  max for edges/bo
+00019f50: 756e 6461 7269 6573 0a20 2020 2020 2020  undaries.       
+00019f60: 206a 6920 3d20 6e70 2e6d 6178 285b 302c   ji = np.max([0,
+00019f70: 206e 702e 6d69 6e28 5b6e 5361 6d70 6c65   np.min([nSample
+00019f80: 202d 2031 2c20 6969 202b 2069 496e 635d   - 1, ii + iInc]
+00019f90: 295d 290a 2020 2020 2020 2020 6a62 203d  )]).        jb =
+00019fa0: 206e 702e 6d61 7828 5b30 2c20 6e70 2e6d   np.max([0, np.m
+00019fb0: 696e 285b 6e53 616d 706c 6520 2d20 312c  in([nSample - 1,
+00019fc0: 2069 6920 2b20 6949 6e63 202a 2062 5d29   ii + iInc * b])
+00019fd0: 5d29 0a0a 2020 2020 2020 2020 2320 6368  ])..        # ch
+00019fe0: 6563 6b20 6c69 6d69 7473 206f 6e20 6c61  eck limits on la
+00019ff0: 6720 696e 6469 6365 730a 2020 2020 2020  g indices.      
+0001a000: 2020 6c4d 696e 7573 3120 3d20 6c6c 202d    lMinus1 = ll -
+0001a010: 2031 0a0a 2020 2020 2020 2020 6966 206c   1..        if l
+0001a020: 4d69 6e75 7331 203c 2030 3a20 2023 2063  Minus1 < 0:  # c
+0001a030: 6865 636b 206c 6167 2069 6e64 6578 2069  heck lag index i
+0001a040: 7320 6772 6561 7465 7220 7468 616e 2031  s greater than 1
+0001a050: 0a20 2020 2020 2020 2020 2020 206c 4d69  .            lMi
+0001a060: 6e75 7331 203d 2030 2020 2320 6d61 6b65  nus1 = 0  # make
+0001a070: 206c 6167 203d 2066 6972 7374 206c 6167   lag = first lag
+0001a080: 0a0a 2020 2020 2020 2020 6c50 6c75 7331  ..        lPlus1
+0001a090: 203d 206c 6c20 2b20 310a 0a20 2020 2020   = ll + 1..     
+0001a0a0: 2020 2069 6620 6c50 6c75 7331 203e 206e     if lPlus1 > n
+0001a0b0: 4c61 6720 2d20 313a 2020 2320 6368 6563  Lag - 1:  # chec
+0001a0c0: 6b20 6c61 6720 696e 6465 7820 6c65 7373  k lag index less
+0001a0d0: 2074 6861 6e20 6d61 7820 6c61 670a 2020   than max lag.  
+0001a0e0: 2020 2020 2020 2020 2020 6c50 6c75 7331            lPlus1
+0001a0f0: 203d 206e 4c61 6720 2d20 310a 0a20 2020   = nLag - 1..   
+0001a100: 2020 2020 2023 2067 6574 2064 6973 7461       # get dista
+0001a110: 6e63 6520 6174 206c 6167 7320 286c 6c2d  nce at lags (ll-
+0001a120: 312c 206c 6c2c 206c 6c2b 3129 0a20 2020  1, ll, ll+1).   
+0001a130: 2020 2020 2064 6973 744c 6d69 6e75 7331       distLminus1
+0001a140: 203d 2064 5b6a 622c 206c 4d69 6e75 7331   = d[jb, lMinus1
+0001a150: 5d20 2023 206d 696e 7573 3a20 2064 5b69  ]  # minus:  d[i
+0001a160: 2d62 2c20 6a2d 315d 0a20 2020 2020 2020  -b, j-1].       
+0001a170: 2064 6973 744c 203d 2064 5b6a 692c 206c   distL = d[ji, l
+0001a180: 6c5d 2020 2320 6163 7475 616c 2064 5b69  l]  # actual d[i
+0001a190: 2d31 2c20 6a5d 0a20 2020 2020 2020 2064  -1, j].        d
+0001a1a0: 6973 744c 706c 7573 3120 3d20 645b 6a62  istLplus1 = d[jb
+0001a1b0: 2c20 6c50 6c75 7331 5d20 2023 2070 6c75  , lPlus1]  # plu
+0001a1c0: 7320 645b 692d 622c 206a 2b31 5d0a 0a20  s d[i-b, j+1].. 
+0001a1d0: 2020 2020 2020 2023 2065 7175 6174 696f         # equatio
+0001a1e0: 6e20 3130 2069 6e20 4861 6c65 2028 3230  n 10 in Hale (20
+0001a1f0: 3133 290a 2020 2020 2020 2020 2320 7375  13).        # su
+0001a200: 6d20 6572 726f 7273 206f 7665 7220 692d  m errors over i-
+0001a210: 313a 692d 622b 310a 2020 2020 2020 2020  1:i-b+1.        
+0001a220: 6966 206a 6920 213d 206a 623a 0a20 2020  if ji != jb:.   
+0001a230: 2020 2020 2020 2020 2066 6f72 206b 6220           for kb 
+0001a240: 696e 2072 616e 6765 286a 692c 206a 6220  in range(ji, jb 
+0001a250: 2d20 6949 6e63 202d 2031 2c20 6949 6e63  - iInc - 1, iInc
+0001a260: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0001a270: 2020 2064 6973 744c 6d69 6e75 7331 203d     distLminus1 =
+0001a280: 2064 6973 744c 6d69 6e75 7331 202b 2065   distLminus1 + e
+0001a290: 7272 5b6b 622c 206c 4d69 6e75 7331 5d0a  rr[kb, lMinus1].
+0001a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a2b0: 6469 7374 4c70 6c75 7331 203d 2064 6973  distLplus1 = dis
+0001a2c0: 744c 706c 7573 3120 2b20 6572 725b 6b62  tLplus1 + err[kb
+0001a2d0: 2c20 6c50 6c75 7331 5d0a 0a20 2020 2020  , lPlus1]..     
+0001a2e0: 2020 2023 2075 7064 6174 6520 6d69 6e69     # update mini
+0001a2f0: 6d75 6d20 6469 7374 616e 6365 2074 6f20  mum distance to 
+0001a300: 7072 6576 696f 7573 2073 616d 706c 650a  previous sample.
+0001a310: 2020 2020 2020 2020 646c 203d 206e 702e          dl = np.
+0001a320: 6d69 6e28 5b64 6973 744c 6d69 6e75 7331  min([distLminus1
+0001a330: 2c20 6469 7374 4c2c 2064 6973 744c 706c  , distL, distLpl
+0001a340: 7573 315d 290a 0a20 2020 2020 2020 2069  us1])..        i
+0001a350: 6620 646c 2021 3d20 6469 7374 4c3a 2020  f dl != distL:  
+0001a360: 2320 7468 656e 206c 6c20 7e3d 206c 6c20  # then ll ~= ll 
+0001a370: 616e 6420 7765 2063 6865 636b 2066 6f72  and we check for
+0001a380: 7761 7264 2061 6e64 2062 6163 6b77 6172  ward and backwar
+0001a390: 640a 2020 2020 2020 2020 2020 2020 6966  d.            if
+0001a3a0: 2064 6c20 3d3d 2064 6973 744c 6d69 6e75   dl == distLminu
+0001a3b0: 7331 3a0a 2020 2020 2020 2020 2020 2020  s1:.            
+0001a3c0: 2020 2020 6c6c 203d 206c 4d69 6e75 7331      ll = lMinus1
+0001a3d0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0001a3e0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001a3f0: 2020 206c 6c20 3d20 6c50 6c75 7331 0a0a     ll = lPlus1..
+0001a400: 2020 2020 2020 2020 2320 6173 7375 6d65          # assume
+0001a410: 2069 6920 3d20 6969 202d 2031 0a20 2020   ii = ii - 1.   
+0001a420: 2020 2020 2069 6920 2b3d 2069 496e 630a       ii += iInc.
+0001a430: 0a20 2020 2020 2020 2023 2061 6273 6f6c  .        # absol
+0001a440: 7574 6520 696e 7465 6765 7220 6f66 206c  ute integer of l
+0001a450: 6167 0a20 2020 2020 2020 2073 7462 6172  ag.        stbar
+0001a460: 5b69 695d 203d 206c 6c20 2b20 6c6d 696e  [ii] = ll + lmin
+0001a470: 0a0a 2020 2020 2020 2020 2320 6e6f 7720  ..        # now 
+0001a480: 6d6f 7665 2074 6f20 636f 7272 6563 7420  move to correct 
+0001a490: 7469 6d65 2069 6e64 6578 2c20 6966 2073  time index, if s
+0001a4a0: 6d6f 6f74 6869 6e67 2064 6966 6665 7265  moothing differe
+0001a4b0: 6e63 6520 6f76 6572 206d 616e 790a 2020  nce over many.  
+0001a4c0: 2020 2020 2020 2320 7469 6d65 2073 616d        # time sam
+0001a4d0: 706c 6573 2075 7369 6e67 2027 6227 0a20  ples using 'b'. 
+0001a4e0: 2020 2020 2020 2069 6620 286c 6c20 3d3d         if (ll ==
+0001a4f0: 206c 4d69 6e75 7331 2920 7c20 286c 6c20   lMinus1) | (ll 
+0001a500: 3d3d 206c 506c 7573 3129 3a20 2023 2063  == lPlus1):  # c
+0001a510: 6865 636b 2065 6467 6573 2074 6f20 7365  heck edges to se
+0001a520: 6520 6162 6f75 7420 6220 7661 6c75 6573  e about b values
+0001a530: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001a540: 6a69 2021 3d20 6a62 3a20 2023 2069 6620  ji != jb:  # if 
+0001a550: 623e 3120 7468 656e 206e 6565 6420 746f  b>1 then need to
+0001a560: 206d 6f76 6520 6d6f 7265 2073 7465 7073   move more steps
+0001a570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a580: 2066 6f72 206b 6220 696e 2072 616e 6765   for kb in range
+0001a590: 286a 692c 206a 6220 2d20 6949 6e63 202d  (ji, jb - iInc -
+0001a5a0: 2031 2c20 6949 6e63 293a 0a20 2020 2020   1, iInc):.     
+0001a5b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001a5c0: 6920 3d20 6969 202b 2069 496e 6320 2023  i = ii + iInc  #
+0001a5d0: 206d 6f76 6520 6672 6f6d 2069 2d31 3a69   move from i-1:i
+0001a5e0: 2d62 2d31 0a20 2020 2020 2020 2020 2020  -b-1.           
+0001a5f0: 2020 2020 2020 2020 2073 7462 6172 5b69           stbar[i
+0001a600: 695d 203d 206c 6c20 2b20 6c6d 696e 2020  i] = ll + lmin  
+0001a610: 2320 636f 6e73 7461 6e74 206c 6167 206f  # constant lag o
+0001a620: 7665 7220 7468 6174 2074 696d 650a 0a20  ver that time.. 
+0001a630: 2020 2072 6574 7572 6e20 7374 6261 720a     return stbar.
+0001a640: 0a0a 6465 6620 7763 745f 6d6f 6469 6669  ..def wct_modifi
+0001a650: 6564 280a 2020 2020 7931 2c20 7932 2c20  ed(.    y1, y2, 
+0001a660: 6474 2c20 646a 3d31 202f 2031 322c 2073  dt, dj=1 / 12, s
+0001a670: 303d 2d31 2c20 4a3d 2d31 2c20 7369 673d  0=-1, J=-1, sig=
+0001a680: 5472 7565 2c20 7369 676e 6966 6963 616e  True, significan
+0001a690: 6365 5f6c 6576 656c 3d30 2e39 352c 2077  ce_level=0.95, w
+0001a6a0: 6176 656c 6574 3d22 6d6f 726c 6574 222c  avelet="morlet",
+0001a6b0: 206e 6f72 6d61 6c69 7a65 3d54 7275 652c   normalize=True,
+0001a6c0: 202a 2a6b 7761 7267 730a 293a 0a20 2020   **kwargs.):.   
+0001a6d0: 2022 2222 0a20 2020 2020 2020 2057 6176   """.        Wav
+0001a6e0: 656c 6574 2063 6f68 6572 656e 6365 2074  elet coherence t
+0001a6f0: 7261 6e73 666f 726d 2028 5743 5429 2e0a  ransform (WCT)..
+0001a700: 2020 2020 e280 8b0a 2020 2020 2020 2020      ....        
+0001a710: 5468 6520 5743 5420 6669 6e64 7320 7265  The WCT finds re
+0001a720: 6769 6f6e 7320 696e 2074 696d 6520 6672  gions in time fr
+0001a730: 6571 7565 6e63 7920 7370 6163 6520 7768  equency space wh
+0001a740: 6572 6520 7468 6520 7477 6f20 7469 6d65  ere the two time
+0001a750: 0a20 2020 2020 2020 2073 6572 6965 7320  .        series 
+0001a760: 636f 2d76 6172 792c 2062 7574 2064 6f20  co-vary, but do 
+0001a770: 6e6f 7420 6e65 6365 7373 6172 696c 7920  not necessarily 
+0001a780: 6861 7665 2068 6967 6820 706f 7765 722e  have high power.
+0001a790: 0a20 2020 20e2 808b 0a20 2020 2020 2020  .    ....       
+0001a7a0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+0001a7b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0001a7c0: 2020 2020 2020 2079 312c 2079 3220 3a20         y1, y2 : 
+0001a7d0: 6e75 6d70 792e 6e64 6172 7261 792c 206c  numpy.ndarray, l
+0001a7e0: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
+0001a7f0: 496e 7075 7420 7369 676e 616c 732e 0a20  Input signals.. 
+0001a800: 2020 2020 2020 2064 7420 3a20 666c 6f61         dt : floa
+0001a810: 740a 2020 2020 2020 2020 2020 2020 5361  t.            Sa
+0001a820: 6d70 6c65 2073 7061 6369 6e67 2e0a 2020  mple spacing..  
+0001a830: 2020 2020 2020 646a 203a 2066 6c6f 6174        dj : float
+0001a840: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0001a850: 2020 2020 2020 2053 7061 6369 6e67 2062         Spacing b
+0001a860: 6574 7765 656e 2064 6973 6372 6574 6520  etween discrete 
+0001a870: 7363 616c 6573 2e20 4465 6661 756c 7420  scales. Default 
+0001a880: 7661 6c75 6520 6973 2031 2f31 322e 0a20  value is 1/12.. 
+0001a890: 2020 2020 2020 2020 2020 2053 6d61 6c6c             Small
+0001a8a0: 6572 2076 616c 7565 7320 7769 6c6c 2072  er values will r
+0001a8b0: 6573 756c 7420 696e 2062 6574 7465 7220  esult in better 
+0001a8c0: 7363 616c 6520 7265 736f 6c75 7469 6f6e  scale resolution
+0001a8d0: 2c20 6275 740a 2020 2020 2020 2020 2020  , but.          
+0001a8e0: 2020 736c 6f77 6572 2063 616c 6375 6c61    slower calcula
+0001a8f0: 7469 6f6e 2061 6e64 2070 6c6f 742e 0a20  tion and plot.. 
+0001a900: 2020 2020 2020 2073 3020 3a20 666c 6f61         s0 : floa
+0001a910: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+0001a920: 2020 2020 2020 2020 536d 616c 6c65 7374          Smallest
+0001a930: 2073 6361 6c65 206f 6620 7468 6520 7761   scale of the wa
+0001a940: 7665 6c65 742e 2044 6566 6175 6c74 2076  velet. Default v
+0001a950: 616c 7565 2069 7320 322a 6474 2e0a 2020  alue is 2*dt..  
+0001a960: 2020 2020 2020 4a20 3a20 666c 6f61 742c        J : float,
+0001a970: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0001a980: 2020 2020 2020 4e75 6d62 6572 206f 6620        Number of 
+0001a990: 7363 616c 6573 206c 6573 7320 6f6e 652e  scales less one.
+0001a9a0: 2053 6361 6c65 7320 7261 6e67 6520 6672   Scales range fr
+0001a9b0: 6f6d 2073 3020 7570 2074 6f0a 2020 2020  om s0 up to.    
+0001a9c0: 2020 2020 2020 2020 7330 202a 2032 2a2a          s0 * 2**
+0001a9d0: 284a 202a 2064 6a29 2c20 7768 6963 6820  (J * dj), which 
+0001a9e0: 6769 7665 7320 6120 746f 7461 6c20 6f66  gives a total of
+0001a9f0: 2028 4a20 2b20 3129 2073 6361 6c65 732e   (J + 1) scales.
+0001aa00: 0a20 2020 2020 2020 2020 2020 2044 6566  .            Def
+0001aa10: 6175 6c74 2069 7320 4a20 3d20 286c 6f67  ault is J = (log
+0001aa20: 3228 4e2a 6474 2f73 6f29 292f 646a 2e0a  2(N*dt/so))/dj..
+0001aa30: 2020 2020 2020 2020 7369 676e 6966 6963          signific
+0001aa40: 616e 6365 5f6c 6576 656c 2028 666c 6f61  ance_level (floa
+0001aa50: 742c 206f 7074 696f 6e61 6c29 203a 0a20  t, optional) :. 
+0001aa60: 2020 2020 2020 2020 2020 2053 6967 6e69             Signi
+0001aa70: 6669 6361 6e63 6520 6c65 7665 6c20 746f  ficance level to
+0001aa80: 2075 7365 2e20 4465 6661 756c 7420 6973   use. Default is
+0001aa90: 2030 2e39 352e 0a20 2020 2020 2020 206e   0.95..        n
+0001aaa0: 6f72 6d61 6c69 7a65 2028 626f 6f6c 6561  ormalize (boolea
+0001aab0: 6e2c 206f 7074 696f 6e61 6c29 203a 0a20  n, optional) :. 
+0001aac0: 2020 2020 2020 2020 2020 2049 6620 7365             If se
+0001aad0: 7420 746f 2074 7275 652c 206e 6f72 6d61  t to true, norma
+0001aae0: 6c69 7a65 7320 4357 5420 6279 2074 6865  lizes CWT by the
+0001aaf0: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
+0001ab00: 696f 6e20 6f66 0a20 2020 2020 2020 2020  ion of.         
+0001ab10: 2020 2074 6865 2073 6967 6e61 6c73 2e0a     the signals..
+0001ab20: 2020 2020 e280 8b0a 2020 2020 2020 2020      ....        
+0001ab30: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+0001ab40: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+0001ab50: 544f 444f 3a20 536f 6d65 7468 696e 6720  TODO: Something 
+0001ab60: 5442 4120 616e 6420 5442 430a 2020 2020  TBA and TBC.    
+0001ab70: e280 8b0a 2020 2020 2020 2020 5365 6520  ....        See 
+0001ab80: 616c 736f 0a20 2020 2020 2020 202d 2d2d  also.        ---
+0001ab90: 2d2d 2d2d 2d0a 2020 2020 2020 2020 6377  -----.        cw
+0001aba0: 742c 2078 7774 0a20 2020 20e2 808b 0a20  t, xwt.    .... 
+0001abb0: 2020 2022 2222 0a0a 2020 2020 7761 7665     """..    wave
+0001abc0: 6c65 7420 3d20 7079 6377 742e 7761 7665  let = pycwt.wave
+0001abd0: 6c65 742e 5f63 6865 636b 5f70 6172 616d  let._check_param
+0001abe0: 6574 6572 5f77 6176 656c 6574 2877 6176  eter_wavelet(wav
+0001abf0: 656c 6574 290a 2020 2020 2320 4368 6563  elet).    # Chec
+0001ac00: 6b69 6e67 2073 6f6d 6520 696e 7075 7420  king some input 
+0001ac10: 7061 7261 6d65 7465 7273 0a20 2020 2069  parameters.    i
+0001ac20: 6620 7330 203d 3d20 2d31 3a0a 2020 2020  f s0 == -1:.    
+0001ac30: 2020 2020 2320 4e75 6d62 6572 206f 6620      # Number of 
+0001ac40: 7363 616c 6573 0a20 2020 2020 2020 2073  scales.        s
+0001ac50: 3020 3d20 3220 2a20 6474 202f 2077 6176  0 = 2 * dt / wav
+0001ac60: 656c 6574 2e66 6c61 6d62 6461 2829 0a20  elet.flambda(). 
+0001ac70: 2020 2069 6620 4a20 3d3d 202d 313a 0a20     if J == -1:. 
+0001ac80: 2020 2020 2020 2023 204e 756d 6265 7220         # Number 
+0001ac90: 6f66 2073 6361 6c65 730a 2020 2020 2020  of scales.      
+0001aca0: 2020 4a20 3d20 6e70 2e69 6e74 286e 702e    J = np.int(np.
+0001acb0: 726f 756e 6428 6e70 2e6c 6f67 3228 7931  round(np.log2(y1
+0001acc0: 2e73 697a 6520 2a20 6474 202f 2073 3029  .size * dt / s0)
+0001acd0: 202f 2064 6a29 290a 0a20 2020 2023 204d   / dj))..    # M
+0001ace0: 616b 6573 2073 7572 6520 696e 7075 7420  akes sure input 
+0001acf0: 7369 676e 616c 7320 6172 6520 6e75 6d70  signals are nump
+0001ad00: 7920 6172 7261 7973 2e0a 2020 2020 7931  y arrays..    y1
+0001ad10: 203d 206e 702e 6173 6172 7261 7928 7931   = np.asarray(y1
+0001ad20: 290a 2020 2020 7932 203d 206e 702e 6173  ).    y2 = np.as
+0001ad30: 6172 7261 7928 7932 290a 2020 2020 2320  array(y2).    # 
+0001ad40: 4361 6c63 756c 6174 6573 2074 6865 2073  Calculates the s
+0001ad50: 7461 6e64 6172 6420 6465 7669 6174 696f  tandard deviatio
+0001ad60: 6e20 6f66 2062 6f74 6820 696e 7075 7420  n of both input 
+0001ad70: 7369 676e 616c 732e 0a20 2020 2073 7464  signals..    std
+0001ad80: 3120 3d20 7931 2e73 7464 2829 0a20 2020  1 = y1.std().   
+0001ad90: 2073 7464 3220 3d20 7932 2e73 7464 2829   std2 = y2.std()
+0001ada0: 0a20 2020 2023 204e 6f72 6d61 6c69 7a65  .    # Normalize
+0001adb0: 7320 626f 7468 2073 6967 6e61 6c73 2c20  s both signals, 
+0001adc0: 6966 2061 7070 726f 7072 6961 7465 2e0a  if appropriate..
+0001add0: 2020 2020 6966 206e 6f72 6d61 6c69 7a65      if normalize
+0001ade0: 3a0a 2020 2020 2020 2020 7931 5f6e 6f72  :.        y1_nor
+0001adf0: 6d61 6c20 3d20 2879 3120 2d20 7931 2e6d  mal = (y1 - y1.m
+0001ae00: 6561 6e28 2929 202f 2073 7464 310a 2020  ean()) / std1.  
+0001ae10: 2020 2020 2020 7932 5f6e 6f72 6d61 6c20        y2_normal 
+0001ae20: 3d20 2879 3220 2d20 7932 2e6d 6561 6e28  = (y2 - y2.mean(
+0001ae30: 2929 202f 2073 7464 320a 2020 2020 656c  )) / std2.    el
+0001ae40: 7365 3a0a 2020 2020 2020 2020 7931 5f6e  se:.        y1_n
+0001ae50: 6f72 6d61 6c20 3d20 7931 0a20 2020 2020  ormal = y1.     
+0001ae60: 2020 2079 325f 6e6f 726d 616c 203d 2079     y2_normal = y
+0001ae70: 320a 0a20 2020 2023 2043 616c 6375 6c61  2..    # Calcula
+0001ae80: 7465 7320 7468 6520 4357 5420 6f66 2074  tes the CWT of t
+0001ae90: 6865 2074 696d 652d 7365 7269 6573 206d  he time-series m
+0001aea0: 616b 696e 6720 7375 7265 2074 6865 2073  aking sure the s
+0001aeb0: 616d 6520 7061 7261 6d65 7465 7273 0a20  ame parameters. 
+0001aec0: 2020 2023 2061 7265 2075 7365 6420 696e     # are used in
+0001aed0: 2062 6f74 6820 6361 6c63 756c 6174 696f   both calculatio
+0001aee0: 6e73 2e0a 2020 2020 5f6b 7761 7267 7320  ns..    _kwargs 
+0001aef0: 3d20 6469 6374 2864 6a3d 646a 2c20 7330  = dict(dj=dj, s0
+0001af00: 3d73 302c 204a 3d4a 2c20 7761 7665 6c65  =s0, J=J, wavele
+0001af10: 743d 7761 7665 6c65 7429 0a20 2020 2057  t=wavelet).    W
+0001af20: 312c 2073 6a2c 2066 7265 712c 2063 6f69  1, sj, freq, coi
+0001af30: 2c20 5f2c 205f 203d 2070 7963 7774 2e63  , _, _ = pycwt.c
+0001af40: 7774 2879 315f 6e6f 726d 616c 2c20 6474  wt(y1_normal, dt
+0001af50: 2c20 2a2a 5f6b 7761 7267 7329 0a20 2020  , **_kwargs).   
+0001af60: 2057 322c 2073 6a2c 2066 7265 712c 2063   W2, sj, freq, c
+0001af70: 6f69 2c20 5f2c 205f 203d 2070 7963 7774  oi, _, _ = pycwt
+0001af80: 2e63 7774 2879 325f 6e6f 726d 616c 2c20  .cwt(y2_normal, 
+0001af90: 6474 2c20 2a2a 5f6b 7761 7267 7329 0a0a  dt, **_kwargs)..
+0001afa0: 2020 2020 7363 616c 6573 3120 3d20 6e70      scales1 = np
+0001afb0: 2e6f 6e65 7328 5b31 2c20 7931 2e73 697a  .ones([1, y1.siz
+0001afc0: 655d 2920 2a20 736a 5b3a 2c20 4e6f 6e65  e]) * sj[:, None
+0001afd0: 5d0a 2020 2020 7363 616c 6573 3220 3d20  ].    scales2 = 
+0001afe0: 6e70 2e6f 6e65 7328 5b31 2c20 7932 2e73  np.ones([1, y2.s
+0001aff0: 697a 655d 2920 2a20 736a 5b3a 2c20 4e6f  ize]) * sj[:, No
+0001b000: 6e65 5d0a 0a20 2020 2023 2053 6d6f 6f74  ne]..    # Smoot
+0001b010: 6820 7468 6520 7761 7665 6c65 7420 7370  h the wavelet sp
+0001b020: 6563 7472 6120 6265 666f 7265 2074 7275  ectra before tru
+0001b030: 6e63 6174 696e 672e 0a20 2020 2053 3120  ncating..    S1 
+0001b040: 3d20 7761 7665 6c65 742e 736d 6f6f 7468  = wavelet.smooth
+0001b050: 286e 702e 6162 7328 5731 2920 2a2a 2032  (np.abs(W1) ** 2
+0001b060: 202f 2073 6361 6c65 7331 2c20 6474 2c20   / scales1, dt, 
+0001b070: 646a 2c20 736a 290a 2020 2020 5332 203d  dj, sj).    S2 =
+0001b080: 2077 6176 656c 6574 2e73 6d6f 6f74 6828   wavelet.smooth(
+0001b090: 6e70 2e61 6273 2857 3229 202a 2a20 3220  np.abs(W2) ** 2 
+0001b0a0: 2f20 7363 616c 6573 322c 2064 742c 2064  / scales2, dt, d
+0001b0b0: 6a2c 2073 6a29 0a0a 2020 2020 2320 4e6f  j, sj)..    # No
+0001b0c0: 7720 7468 6520 7761 7665 6c65 7420 7472  w the wavelet tr
+0001b0d0: 616e 7366 6f72 6d20 636f 6865 7265 6e63  ansform coherenc
+0001b0e0: 650a 2020 2020 5731 3220 3d20 5731 202a  e.    W12 = W1 *
+0001b0f0: 2057 322e 636f 6e6a 2829 0a20 2020 2073   W2.conj().    s
+0001b100: 6361 6c65 7320 3d20 6e70 2e6f 6e65 7328  cales = np.ones(
+0001b110: 5b31 2c20 7931 2e73 697a 655d 2920 2a20  [1, y1.size]) * 
+0001b120: 736a 5b3a 2c20 4e6f 6e65 5d0a 2020 2020  sj[:, None].    
+0001b130: 5331 3220 3d20 7761 7665 6c65 742e 736d  S12 = wavelet.sm
+0001b140: 6f6f 7468 2857 3132 202f 2073 6361 6c65  ooth(W12 / scale
+0001b150: 732c 2064 742c 2064 6a2c 2073 6a29 0a20  s, dt, dj, sj). 
+0001b160: 2020 2057 4354 203d 206e 702e 6162 7328     WCT = np.abs(
+0001b170: 5331 3229 202a 2a20 3220 2f20 2853 3120  S12) ** 2 / (S1 
+0001b180: 2a20 5332 290a 2020 2020 6157 4354 203d  * S2).    aWCT =
+0001b190: 206e 702e 616e 676c 6528 5731 3229 0a0a   np.angle(W12)..
+0001b1a0: 2020 2020 2320 4361 6c63 756c 6174 6573      # Calculates
+0001b1b0: 2074 6865 2073 6967 6e69 6669 6361 6e63   the significanc
+0001b1c0: 6520 7573 696e 6720 4d6f 6e74 6520 4361  e using Monte Ca
+0001b1d0: 726c 6f20 7369 6d75 6c61 7469 6f6e 7320  rlo simulations 
+0001b1e0: 7769 7468 2039 3525 0a20 2020 2023 2063  with 95%.    # c
+0001b1f0: 6f6e 6669 6465 6e63 6520 6173 2061 2066  onfidence as a f
+0001b200: 756e 6374 696f 6e20 6f66 2073 6361 6c65  unction of scale
+0001b210: 2e0a 0a20 2020 2069 6620 7369 673a 0a20  ...    if sig:. 
+0001b220: 2020 2020 2020 2061 312c 2062 312c 2063         a1, b1, c
+0001b230: 3120 3d20 7079 6377 742e 6172 3128 7931  1 = pycwt.ar1(y1
+0001b240: 290a 2020 2020 2020 2020 6132 2c20 6232  ).        a2, b2
+0001b250: 2c20 6332 203d 2070 7963 7774 2e61 7231  , c2 = pycwt.ar1
+0001b260: 2879 3229 0a20 2020 2020 2020 2073 6967  (y2).        sig
+0001b270: 203d 2070 7963 7774 2e77 6374 5f73 6967   = pycwt.wct_sig
+0001b280: 6e69 6669 6361 6e63 6528 0a20 2020 2020  nificance(.     
+0001b290: 2020 2020 2020 2061 312c 2061 322c 2064         a1, a2, d
+0001b2a0: 743d 6474 2c20 646a 3d64 6a2c 2073 303d  t=dt, dj=dj, s0=
+0001b2b0: 7330 2c20 4a3d 4a2c 2073 6967 6e69 6669  s0, J=J, signifi
+0001b2c0: 6361 6e63 655f 6c65 7665 6c3d 7369 676e  cance_level=sign
+0001b2d0: 6966 6963 616e 6365 5f6c 6576 656c 2c20  ificance_level, 
+0001b2e0: 7761 7665 6c65 743d 7761 7665 6c65 742c  wavelet=wavelet,
+0001b2f0: 202a 2a6b 7761 7267 730a 2020 2020 2020   **kwargs.      
+0001b300: 2020 290a 2020 2020 656c 7365 3a0a 2020    ).    else:.  
+0001b310: 2020 2020 2020 7369 6720 3d20 6e70 2e61        sig = np.a
+0001b320: 7361 7272 6179 285b 305d 290a 0a20 2020  sarray([0])..   
+0001b330: 2072 6574 7572 6e20 5743 542c 2061 5743   return WCT, aWC
+0001b340: 542c 2063 6f69 2c20 6672 6571 2c20 7369  T, coi, freq, si
+0001b350: 670a 0a0a 2323 2323 2323 2323 2323 2323  g...############
 0001b360: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001b370: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b380: 2323 2323 2323 2323 2323 2323 2323 0a23  ##############.#
-0001b390: 2323 2323 2323 2323 2323 2323 2323 2320  ############### 
-0001b3a0: 4449 5350 4552 5349 4f4e 2045 5854 5241  DISPERSION EXTRA
-0001b3b0: 4354 494f 4e20 4655 4e43 5449 4f4e 5320  CTION FUNCTIONS 
-0001b3c0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
-0001b3d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0001b390: 2323 2323 0a23 2323 2323 2323 2323 2323  ####.###########
+0001b3a0: 2323 2323 2320 4449 5350 4552 5349 4f4e  ##### DISPERSION
+0001b3b0: 2045 5854 5241 4354 494f 4e20 4655 4e43   EXTRACTION FUNC
+0001b3c0: 5449 4f4e 5320 2323 2323 2323 2323 2323  TIONS ##########
+0001b3d0: 2323 2323 230a 2323 2323 2323 2323 2323  #####.##########
 0001b3e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001b3f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 0001b400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0001b410: 0a0a 0a23 2066 756e 6374 696f 6e20 746f  ...# function to
-0001b420: 2065 7874 7261 6374 2074 6865 2064 6973   extract the dis
-0001b430: 7065 7273 696f 6e20 6672 6f6d 2074 6865  persion from the
-0001b440: 2069 6d61 6765 0a64 6566 2065 7874 7261   image.def extra
-0001b450: 6374 5f64 6973 7065 7273 696f 6e28 616d  ct_dispersion(am
-0001b460: 702c 2070 6572 2c20 7665 6c29 3a0a 2020  p, per, vel):.  
-0001b470: 2020 2222 220a 2020 2020 7468 6973 2066    """.    this f
-0001b480: 756e 6374 696f 6e20 7461 6b65 7320 7468  unction takes th
-0001b490: 6520 6469 7370 6572 7369 6f6e 2069 6d61  e dispersion ima
-0001b4a0: 6765 2066 726f 6d20 4357 5420 6173 2069  ge from CWT as i
-0001b4b0: 6e70 7574 2c20 7472 6163 6b73 2074 6865  nput, tracks the
-0001b4c0: 2067 6c6f 6261 6c20 6d61 7869 6e75 6d20   global maxinum 
-0001b4d0: 6f6e 0a20 2020 2074 6865 2077 6176 656c  on.    the wavel
-0001b4e0: 6574 2073 7065 6374 7275 6d20 616d 706c  et spectrum ampl
-0001b4f0: 6974 7564 6520 616e 6420 6578 7472 6163  itude and extrac
-0001b500: 7420 7468 6520 7365 6374 696f 6e73 2077  t the sections w
-0001b510: 6974 6820 636f 6e74 696e 6f75 7320 616e  ith continous an
-0001b520: 6420 6869 6768 2071 7561 6c69 7479 2064  d high quality d
-0001b530: 6174 610a 0a20 2020 2050 4152 414d 4554  ata..    PARAMET
-0001b540: 4552 533a 0a20 2020 202d 2d2d 2d2d 2d2d  ERS:.    -------
-0001b550: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 616d  ---------.    am
-0001b560: 703a 2032 4420 616d 706c 6974 7564 6520  p: 2D amplitude 
-0001b570: 6d61 7472 6978 206f 6620 7468 6520 7761  matrix of the wa
-0001b580: 7665 6c65 7420 7370 6563 7472 756d 0a20  velet spectrum. 
-0001b590: 2020 2070 6861 7365 3a20 3244 2070 6861     phase: 2D pha
-0001b5a0: 7365 206d 6174 7269 7820 6f66 2074 6865  se matrix of the
-0001b5b0: 2077 6176 656c 6574 2073 7065 6374 7275   wavelet spectru
-0001b5c0: 6d0a 2020 2020 7065 723a 2020 7065 7269  m.    per:  peri
-0001b5d0: 6f64 2076 6563 746f 7220 666f 7220 7468  od vector for th
-0001b5e0: 6520 3244 206d 6174 7269 780a 2020 2020  e 2D matrix.    
-0001b5f0: 7665 6c3a 2020 7665 6c20 7665 6374 6f72  vel:  vel vector
-0001b600: 206f 6620 7468 6520 3244 206d 6174 7269   of the 2D matri
-0001b610: 780a 2020 2020 5245 5455 524e 533a 0a20  x.    RETURNS:. 
-0001b620: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d     -------------
-0001b630: 2d2d 2d0a 2020 2020 7065 723a 2020 6365  ---.    per:  ce
-0001b640: 6e74 7261 6c20 6672 6571 7565 6e63 7920  ntral frequency 
-0001b650: 6f66 2065 6163 6820 7761 7665 6c65 7420  of each wavelet 
-0001b660: 7363 616c 6520 7769 7468 2067 6f6f 6420  scale with good 
-0001b670: 6461 7461 0a20 2020 2067 763a 2020 2067  data.    gv:   g
-0001b680: 726f 7570 2076 656c 6f63 6974 7920 7665  roup velocity ve
-0001b690: 6374 6f72 2061 7420 6561 6368 2066 7265  ctor at each fre
-0001b6a0: 7175 656e 6379 0a20 2020 2022 2222 0a20  quency.    """. 
-0001b6b0: 2020 206d 6178 6761 7020 3d20 350a 2020     maxgap = 5.  
-0001b6c0: 2020 6e70 6572 203d 2061 6d70 2e73 6861    nper = amp.sha
-0001b6d0: 7065 5b30 5d0a 2020 2020 6776 203d 206e  pe[0].    gv = n
-0001b6e0: 702e 7a65 726f 7328 6e70 6572 2c20 6474  p.zeros(nper, dt
-0001b6f0: 7970 653d 6e70 2e66 6c6f 6174 3332 290a  ype=np.float32).
-0001b700: 2020 2020 6476 656c 203d 2076 656c 5b31      dvel = vel[1
-0001b710: 5d20 2d20 7665 6c5b 305d 0a0a 2020 2020  ] - vel[0]..    
-0001b720: 2320 6669 6e64 2067 6c6f 6261 6c20 6d61  # find global ma
-0001b730: 7869 6d75 6d0a 2020 2020 666f 7220 6969  ximum.    for ii
-0001b740: 2069 6e20 7261 6e67 6528 6e70 6572 293a   in range(nper):
-0001b750: 0a20 2020 2020 2020 206d 6178 7661 6c75  .        maxvalu
-0001b760: 6520 3d20 6e70 2e6d 6178 2861 6d70 5b69  e = np.max(amp[i
-0001b770: 695d 2c20 6178 6973 3d30 290a 2020 2020  i], axis=0).    
-0001b780: 2020 2020 696e 6478 203d 206c 6973 7428      indx = list(
-0001b790: 616d 705b 6969 5d29 2e69 6e64 6578 286d  amp[ii]).index(m
-0001b7a0: 6178 7661 6c75 6529 0a20 2020 2020 2020  axvalue).       
-0001b7b0: 2067 765b 6969 5d20 3d20 7665 6c5b 696e   gv[ii] = vel[in
-0001b7c0: 6478 5d0a 0a20 2020 2023 2063 6865 636b  dx]..    # check
-0001b7d0: 2074 6865 2063 6f6e 7469 6e75 6f75 7320   the continuous 
-0001b7e0: 6f66 2074 6865 2064 6973 7065 7273 696f  of the dispersio
-0001b7f0: 6e0a 2020 2020 666f 7220 6969 2069 6e20  n.    for ii in 
-0001b800: 7261 6e67 6528 312c 206e 7065 7220 2d20  range(1, nper - 
-0001b810: 3135 293a 0a20 2020 2020 2020 2023 2031  15):.        # 1
-0001b820: 3520 6973 2074 6865 206d 696e 756d 756d  5 is the minumum
-0001b830: 206c 656e 6774 6820 6e65 6564 6564 2066   length needed f
-0001b840: 6f72 206f 7574 7075 740a 2020 2020 2020  or output.      
-0001b850: 2020 666f 7220 6a6a 2069 6e20 7261 6e67    for jj in rang
-0001b860: 6528 3135 293a 0a20 2020 2020 2020 2020  e(15):.         
-0001b870: 2020 2069 6620 6e70 2e61 6273 2867 765b     if np.abs(gv[
-0001b880: 6969 202b 206a 6a5d 202d 2067 765b 6969  ii + jj] - gv[ii
-0001b890: 202b 2031 202b 206a 6a5d 2920 3e20 6d61   + 1 + jj]) > ma
-0001b8a0: 7867 6170 202a 2064 7665 6c3a 0a20 2020  xgap * dvel:.   
-0001b8b0: 2020 2020 2020 2020 2020 2020 2067 765b               gv[
-0001b8c0: 6969 5d20 3d20 300a 2020 2020 2020 2020  ii] = 0.        
-0001b8d0: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
-0001b8e0: 2020 2023 2072 656d 6f76 6520 7468 6520     # remove the 
-0001b8f0: 6261 6420 6f6e 6573 0a20 2020 2069 6e64  bad ones.    ind
-0001b900: 7820 3d20 6e70 2e77 6865 7265 2867 7620  x = np.where(gv 
-0001b910: 3e20 3029 5b30 5d0a 0a20 2020 2072 6574  > 0)[0]..    ret
-0001b920: 7572 6e20 7065 725b 696e 6478 5d2c 2067  urn per[indx], g
-0001b930: 765b 696e 6478 5d0a                      v[indx].
+0001b410: 2323 2323 2323 0a0a 0a23 2066 756e 6374  ######...# funct
+0001b420: 696f 6e20 746f 2065 7874 7261 6374 2074  ion to extract t
+0001b430: 6865 2064 6973 7065 7273 696f 6e20 6672  he dispersion fr
+0001b440: 6f6d 2074 6865 2069 6d61 6765 0a64 6566  om the image.def
+0001b450: 2065 7874 7261 6374 5f64 6973 7065 7273   extract_dispers
+0001b460: 696f 6e28 616d 702c 2070 6572 2c20 7665  ion(amp, per, ve
+0001b470: 6c29 3a0a 2020 2020 2222 220a 2020 2020  l):.    """.    
+0001b480: 7468 6973 2066 756e 6374 696f 6e20 7461  this function ta
+0001b490: 6b65 7320 7468 6520 6469 7370 6572 7369  kes the dispersi
+0001b4a0: 6f6e 2069 6d61 6765 2066 726f 6d20 4357  on image from CW
+0001b4b0: 5420 6173 2069 6e70 7574 2c20 7472 6163  T as input, trac
+0001b4c0: 6b73 2074 6865 2067 6c6f 6261 6c20 6d61  ks the global ma
+0001b4d0: 7869 6e75 6d20 6f6e 0a20 2020 2074 6865  xinum on.    the
+0001b4e0: 2077 6176 656c 6574 2073 7065 6374 7275   wavelet spectru
+0001b4f0: 6d20 616d 706c 6974 7564 6520 616e 6420  m amplitude and 
+0001b500: 6578 7472 6163 7420 7468 6520 7365 6374  extract the sect
+0001b510: 696f 6e73 2077 6974 6820 636f 6e74 696e  ions with contin
+0001b520: 6f75 7320 616e 6420 6869 6768 2071 7561  ous and high qua
+0001b530: 6c69 7479 2064 6174 610a 0a20 2020 2050  lity data..    P
+0001b540: 4152 414d 4554 4552 533a 0a20 2020 202d  ARAMETERS:.    -
+0001b550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a  ---------------.
+0001b560: 2020 2020 616d 703a 2032 4420 616d 706c      amp: 2D ampl
+0001b570: 6974 7564 6520 6d61 7472 6978 206f 6620  itude matrix of 
+0001b580: 7468 6520 7761 7665 6c65 7420 7370 6563  the wavelet spec
+0001b590: 7472 756d 0a20 2020 2070 6861 7365 3a20  trum.    phase: 
+0001b5a0: 3244 2070 6861 7365 206d 6174 7269 7820  2D phase matrix 
+0001b5b0: 6f66 2074 6865 2077 6176 656c 6574 2073  of the wavelet s
+0001b5c0: 7065 6374 7275 6d0a 2020 2020 7065 723a  pectrum.    per:
+0001b5d0: 2020 7065 7269 6f64 2076 6563 746f 7220    period vector 
+0001b5e0: 666f 7220 7468 6520 3244 206d 6174 7269  for the 2D matri
+0001b5f0: 780a 2020 2020 7665 6c3a 2020 7665 6c20  x.    vel:  vel 
+0001b600: 7665 6374 6f72 206f 6620 7468 6520 3244  vector of the 2D
+0001b610: 206d 6174 7269 780a 2020 2020 5245 5455   matrix.    RETU
+0001b620: 524e 533a 0a20 2020 202d 2d2d 2d2d 2d2d  RNS:.    -------
+0001b630: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7065  ---------.    pe
+0001b640: 723a 2020 6365 6e74 7261 6c20 6672 6571  r:  central freq
+0001b650: 7565 6e63 7920 6f66 2065 6163 6820 7761  uency of each wa
+0001b660: 7665 6c65 7420 7363 616c 6520 7769 7468  velet scale with
+0001b670: 2067 6f6f 6420 6461 7461 0a20 2020 2067   good data.    g
+0001b680: 763a 2020 2067 726f 7570 2076 656c 6f63  v:   group veloc
+0001b690: 6974 7920 7665 6374 6f72 2061 7420 6561  ity vector at ea
+0001b6a0: 6368 2066 7265 7175 656e 6379 0a20 2020  ch frequency.   
+0001b6b0: 2022 2222 0a20 2020 206d 6178 6761 7020   """.    maxgap 
+0001b6c0: 3d20 350a 2020 2020 6e70 6572 203d 2061  = 5.    nper = a
+0001b6d0: 6d70 2e73 6861 7065 5b30 5d0a 2020 2020  mp.shape[0].    
+0001b6e0: 6776 203d 206e 702e 7a65 726f 7328 6e70  gv = np.zeros(np
+0001b6f0: 6572 2c20 6474 7970 653d 6e70 2e66 6c6f  er, dtype=np.flo
+0001b700: 6174 3332 290a 2020 2020 6476 656c 203d  at32).    dvel =
+0001b710: 2076 656c 5b31 5d20 2d20 7665 6c5b 305d   vel[1] - vel[0]
+0001b720: 0a0a 2020 2020 2320 6669 6e64 2067 6c6f  ..    # find glo
+0001b730: 6261 6c20 6d61 7869 6d75 6d0a 2020 2020  bal maximum.    
+0001b740: 666f 7220 6969 2069 6e20 7261 6e67 6528  for ii in range(
+0001b750: 6e70 6572 293a 0a20 2020 2020 2020 206d  nper):.        m
+0001b760: 6178 7661 6c75 6520 3d20 6e70 2e6d 6178  axvalue = np.max
+0001b770: 2861 6d70 5b69 695d 2c20 6178 6973 3d30  (amp[ii], axis=0
+0001b780: 290a 2020 2020 2020 2020 696e 6478 203d  ).        indx =
+0001b790: 206c 6973 7428 616d 705b 6969 5d29 2e69   list(amp[ii]).i
+0001b7a0: 6e64 6578 286d 6178 7661 6c75 6529 0a20  ndex(maxvalue). 
+0001b7b0: 2020 2020 2020 2067 765b 6969 5d20 3d20         gv[ii] = 
+0001b7c0: 7665 6c5b 696e 6478 5d0a 0a20 2020 2023  vel[indx]..    #
+0001b7d0: 2063 6865 636b 2074 6865 2063 6f6e 7469   check the conti
+0001b7e0: 6e75 6f75 7320 6f66 2074 6865 2064 6973  nuous of the dis
+0001b7f0: 7065 7273 696f 6e0a 2020 2020 666f 7220  persion.    for 
+0001b800: 6969 2069 6e20 7261 6e67 6528 312c 206e  ii in range(1, n
+0001b810: 7065 7220 2d20 3135 293a 0a20 2020 2020  per - 15):.     
+0001b820: 2020 2023 2031 3520 6973 2074 6865 206d     # 15 is the m
+0001b830: 696e 756d 756d 206c 656e 6774 6820 6e65  inumum length ne
+0001b840: 6564 6564 2066 6f72 206f 7574 7075 740a  eded for output.
+0001b850: 2020 2020 2020 2020 666f 7220 6a6a 2069          for jj i
+0001b860: 6e20 7261 6e67 6528 3135 293a 0a20 2020  n range(15):.   
+0001b870: 2020 2020 2020 2020 2069 6620 6e70 2e61           if np.a
+0001b880: 6273 2867 765b 6969 202b 206a 6a5d 202d  bs(gv[ii + jj] -
+0001b890: 2067 765b 6969 202b 2031 202b 206a 6a5d   gv[ii + 1 + jj]
+0001b8a0: 2920 3e20 6d61 7867 6170 202a 2064 7665  ) > maxgap * dve
+0001b8b0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+0001b8c0: 2020 2067 765b 6969 5d20 3d20 300a 2020     gv[ii] = 0.  
+0001b8d0: 2020 2020 2020 2020 2020 2020 2020 6272                br
+0001b8e0: 6561 6b0a 0a20 2020 2023 2072 656d 6f76  eak..    # remov
+0001b8f0: 6520 7468 6520 6261 6420 6f6e 6573 0a20  e the bad ones. 
+0001b900: 2020 2069 6e64 7820 3d20 6e70 2e77 6865     indx = np.whe
+0001b910: 7265 2867 7620 3e20 3029 5b30 5d0a 0a20  re(gv > 0)[0].. 
+0001b920: 2020 2072 6574 7572 6e20 7065 725b 696e     return per[in
+0001b930: 6478 5d2c 2067 765b 696e 6478 5d0a       dx], gv[indx].
```

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.8.1/src/noisepy/seis/plotting_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,45 +203,38 @@
                 tmarks.append(obspy.UTCDateTime(ttime[ii]).strftime("%H:%M:%S"))
 
             # plotting
             if nwin > 10:
                 tick_inc = int(nwin / 5)
             else:
                 tick_inc = 2
-            fig = plt.figure(figsize=(10, 6))
-            ax = fig.add_subplot(211)
-            ax.matshow(
+            fig, (
+                ax1,
+                ax2,
+            ) = plt.subplots(2, 1, gridspec_kw={"height_ratios": [1, 3]}, figsize=(10, 6))
+            ax1.matshow(
                 data,
                 cmap="seismic",
                 extent=[-disp_lag, disp_lag, nwin, 0],
                 aspect="auto",
             )
-            ax.set_title("%s.%s.%s  %s.%s.%s  dist:%5.2fkm" % (net1, sta1, chan1, net2, sta2, chan2, dist))
-            ax.set_xlabel("time [s]")
-            ax.set_xticks(t)
-            ax.set_yticks(np.arange(0, nwin, step=tick_inc))
-            ax.set_yticklabels(timestamp[0::tick_inc])
-            ax.xaxis.set_ticks_position("bottom")
-            ax1 = fig.add_subplot(413)
-            ax1.set_title("stacked and filtered at %4.2f-%4.2f Hz" % (freqmin, freqmax))
-            ax1.plot(
-                np.arange(-disp_lag, disp_lag + dt, dt),
-                np.mean(data, axis=0),
-                "k-",
-                linewidth=1,
-            )
+            ax1.set_title("%s.%s.%s  %s.%s.%s  dist:%5.2fkm" % (net1, sta1, chan1, net2, sta2, chan2, dist))
+            ax1.set_xlabel("time [s]")
             ax1.set_xticks(t)
-            ax2 = fig.add_subplot(414)
+            ax1.set_yticks(np.arange(0, nwin, step=tick_inc))
+            ax1.set_yticklabels(timestamp[0::tick_inc])
+            ax1.xaxis.set_ticks_position("bottom")
+
             ax2.plot(amax / min(amax), "r-")
             ax2.plot(ngood, "b-")
             ax2.set_xlabel("waveform number")
             ax2.set_xticks(np.arange(0, nwin, step=tick_inc))
             ax2.set_xticklabels(tmarks[0:nwin:tick_inc])
-            # for tick in ax[2].get_xticklabels():
-            #    tick.set_rotation(30)
+            for tick in ax2.get_xticklabels():
+                tick.set_rotation(30)
             ax2.legend(["relative amp", "ngood"], loc="upper right")
             fig.tight_layout()
 
             # save figure or just show
             if savefig:
                 if sdir is None:
                     sdir = sfile.split(".")[0]
```

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/scedc_s3store.py` & `noisepy_seis-0.8.1/src/noisepy/seis/scedc_s3store.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,27 @@
 
 from .datatypes import Channel, ChannelData, ChannelType, Station
 from .utils import fs_join, get_filesystem
 
 logger = logging.getLogger(__name__)
 
 
+def channel_filter(stations: List[str], ch_prefix: str) -> Callable[[Channel], bool]:
+    """
+    Helper function for creating a channel filter to be used in the constructor of the store.
+    This filter uses a list of allowed station name along with a channel filter prefix.
+    """
+    sta_set = set(stations)
+
+    def filter(ch: Channel) -> bool:
+        return ch.station.name in sta_set and ch.type.name.lower().startswith(ch_prefix.lower())
+
+    return filter
+
+
 class SCEDCS3DataStore(RawDataStore):
     """
     A data store implementation to read from a directory of miniSEED (.ms) files from the SCEDC S3 bucket.
     Every directory is a a day and each .ms file contains the data for a channel.
     """
 
     # TODO: Support reading directly from the S3 bucket
```

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/stores.py` & `noisepy_seis-0.8.1/src/noisepy/seis/stores.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,14 +27,23 @@
     def get_channels(self, timespan: DateTimeRange) -> List[Channel]:
         pass
 
     @abstractmethod
     def get_timespans(self) -> List[DateTimeRange]:
         pass
 
+    # TODO: Temporary method to get a list of stations to pass to the
+    # stack() function. It can be removed once the stacking uses
+    # the DataStores instead of direct file access
+    def get_station_list(self) -> List[str]:
+        ts = self.get_timespans()
+        chs = self.get_channels(ts[0])
+        stations = sorted(set(map(lambda c: str(c.station), chs)))
+        return stations
+
 
 class RawDataStore(DataStore):
     """
     A class for reading the raw data for a given channel.
     TODO: write support?
     """
```

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/utils.py` & `noisepy_seis-0.8.1/src/noisepy/seis/utils.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.8.1/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.8.1/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 this application script of NoisePy is to measure group velocity on the resulted cross-correlation
 functions from S2. It uses the wavelet transform to trace the wave energy on multiple frequencies.
 Based on our tests, it generates very similar results to those from Frequency-Time Analysis (FTAN).
 
 Authors: Chengxin Jiang (chengxin_jiang@fas.harvard.edu)
 
 NOTE:
-    According to Bensen et al., (2007), the centrel frequncy of
-    each narrowband filters (equvalent to wavelet tranformed signal
+    According to Bensen et al., (2007), the central frequency of
+    each narrowband filters (equivalent to wavelet tranformed signal
     at each scale) would be different from the instaneous frequency calculated
     using instaneous phase due to spectral linkage. We do not
     correct this effect in this script. Phase velocity is not calculated here,
     but could be expaneded using the phase info of wavelet transformed signal.
 """
 
 ############################################
```

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.8.1/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.0/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.8.1/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.0/.gitignore` & `noisepy_seis-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.0/LICENSE` & `noisepy_seis-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.0/README.md` & `noisepy_seis-0.8.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,77 +8,93 @@
 [![Documentation Status](https://readthedocs.org/projects/noisepy/badge/?version=latest)](https://noisepy.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://travis-ci.com/chengxinjiang/NoisePy.svg?branch=master)](https://travis-ci.com/github/chengxinjiang/NoisePy)
 [![Codecov](https://codecov.io/gh/chengxinjiang/NoisePy/branch/master/graph/badge.svg)](https://codecov.io/gh/chengxinjiang/NoisePy)
 
 <img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/logo.png" width="800" height="400">
 
 ## Major updates coming
-NoisePy is going through a major refactoring to make this package easier to use and contribute.
+NoisePy is going through a major refactoring to make this package easier to develop and deploy. Submit an issue, fork the repository and create pull requests to contribute.
 
 # Installation
-The nature of NoisePy being composed of python scripts allows flexible package installation, which is essentially to build dependent libraries the scripts and related functions live upon. We recommend using [conda](https://docs.conda.io/en/latest/) or [pip](https://pypi.org/project/pip/) to install the library due to their convenience. Below are command lines we have tested to create a python environment to run NoisePy. Note that the test is performed on `macOS Big Sur (11.7)`, so it could be slightly different for other OS.
-
+The nature of NoisePy being composed of python scripts allows flexible package installation, which is essentially to build dependent libraries the scripts and related functions live upon. We recommend using [conda](https://docs.conda.io/en/latest/) or [pip](https://pypi.org/project/pip/) to install.
 
 ### Note the order of the command lines below matters ###
 
-# With Conda:
+## With Conda and pip:
 ```bash
 conda create -n noisepy python=3.8 pip
 conda activate noisepy
 conda install -c conda-forge openmpi
 pip install noisepy-seis
 ```
 
-# With virtual environment:
+## With virtual environment:
 An MPI installation is required. E.g. for macOS using [brew](https://brew.sh/) :
 ```bash
 brew install open-mpi
 ```
 
 ```bash
 python -m venv noisepy
 source noisepy/bin/activate
 pip install noisepy-seis
 ```
-To run the code on a single core, open the terminal and activate the noisepy environment before run following command. To run on institutional clusters, see installation notes for individual packages on the module list of the cluster. Examples of installation on Frontera are below.
 
 
-# Deploy using Docker
+# Functionality
+Here is a list of features of the package:
+* download continous noise data based:
+   + on webservices using obspy's core functions of [get_station](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html) and [get_waveforms](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_waveforms.html)
+   + on AWS S3 bucket calls, with a test on the SCEDC AWS Open Dataset.
+* save seismic data in [ASDF](https://asdf-definition.readthedocs.io/en/latest/) format, which convinently assembles meta, wavefrom and auxililary data into one single file ([Tutorials](https://github.com/SeismicData/pyasdf/blob/master/doc/tutorial.rst) on reading/writing ASDF files)
+* offers scripts to precondition data sets before cross correlations. This involves working with gappy data from various formats (SAC/miniSEED) and storing it on local in ASDF.
+
+* performs fast and easy cross-correlation with functionality to run in parallel through [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface)
+* **Applications module**:
+   + *Ambient noise monitoring*: measure dv/v using a wide variety of techniques in time, fourier, and wavelet domain (Yuan et al., 2021)
+   + *Surface wave dispersion*: construct dispersion images using conventional techniques.
+
+
+
+# Usage
+
+To run the code on a single core, open the terminal and activate the noisepy environment before run following commands. To run on institutional clusters, see installation notes for individual packages on the module list of the cluster.
+
+## Deploy using Docker
 We use I/O on disk, so users need root access to the file system. To install rootless docker, see instructions [here](https://docs.docker.com/engine/security/rootless/#install).
 ```bash
 docker pull  ghcr.io/mdenolle/noisepy:latest
 docker run -v ~/tmp:/tmp cross_correlate --path /tmp
 ```
 
-# Functionality
-Here is a list of features of the package:
-* download continous noise data based on obspy's core functions of [get_station](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html) and [get_waveforms](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_waveforms.html)
-* save seismic data in [ASDF](https://asdf-definition.readthedocs.io/en/latest/) format, which convinently assembles meta, wavefrom and auxililary data into one single file ([Tutorials](https://github.com/SeismicData/pyasdf/blob/master/doc/tutorial.rst) on reading/writing ASDF files)
-* offers high flexibility to handle messy SAC/miniSEED data stored on your local machine and convert them into ASDF format data that could easily be pluged into NoisePy
-* performs fast and easy cross-correlation with functionality to run in parallel through [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface)
-* includes a series of monitoring functions to measure dv/v on the resulted cross-correlation functions using some recently developed new methods (see our papers for more details<sup>**</sup>)
-
-# Short tutorial
-A short tutorial on how to use NoisePy-seis can be is available as a [Jupyter notebook](https://github.com/mdenolle/NoisePy/blob/master/Jupyter_notebook/tutorial.ipynb) and can be
-[run directly in Colab](https://colab.research.google.com/github/mdenolle/NoisePy/blob/master/Jupyter_notebook/tutorial.ipynb).
+# Tutorials
+A short tutorial on how to use NoisePy-seis can be is available as a [Jupyter notebook](https://github.com/mdenolle/NoisePy/blob/master/tutorials/get_started.ipynb) and can be
+[run directly in Colab](https://colab.research.google.com/github/mdenolle/NoisePy/blob/master/tutorials/get_started.ipynb).
 
 
 This tutorial presents one simple example of how NoisePy might work! We strongly encourage you to download the NoisePy package and play it on your own! If you have any  comments and/or suggestions during running the codes, please do not hesitate to contact us through email or open an issue in this github page!
 
 Chengxin Jiang (chengxinjiang@gmail.com)
 Marine Denolle (mdenolle@uw.edu).
 
-#### Peer-Reviewed Publications Referenced
-Seats, K. J., Jesse F. L., and German A. P. "Improved ambient noise correlation functions using Welch′ s method." _Geophysical Journal International_ 188, no. 2 (2012): 513-523.
-*Jiang, C. and Denolle, M. "NoisePy: a new high-performance python tool for seismic ambient noise seismology." _Seismological Research Letter_ 91, no. 3 (2020): 1853–1866..
-** Yuan, C., Bryan, J. T., and Denolle, M. "Numerical comparison of time-, frequency- and wavelet-domain methods for coda wave interferometry." _Geophysical Journal International_ 226, no. 2 (2021): 828-846.
+## Use this reference when publishing on your work with noisepy
+
+Main code:
+* Jiang, C. and Denolle, M. [NoisePy: a new high-performance python tool for seismic ambient noise seismology.](https://doi.org/10.1785/0220190364) _Seismological Research Letter_ 91, no. 3 (2020): 1853–1866. https://doi.org/10.1785/0220190364
+
+Algorithms used:
+* (data pre-processing) Seats, K. J., Jesse F. L., and German A. P. [Improved ambient noise correlation functions using Welch′ s method.](https://doi.org/10.1111/j.1365-246X.2011.05263.x) _Geophysical Journal International_ 188, no. 2 (2012): 513-523. https://doi.org/10.1111/j.1365-246X.2011.05263.x
 
+* (dv/v in wavelet domain) Yuan, C., Bryan, J. T., and Denolle, M. [Numerical comparison of time-, frequency- and wavelet-domain methods for coda wave interferometry.](https://doi.org/10.1093/gji/ggab140) _Geophysical Journal International_ 226, no. 2 (2021): 828-846. https://doi.org/10.1093/gji/ggab140
+
+* (optimal stacking) Yang X, Bryan J, Okubo K, Jiang C, Clements T, Denolle MA. [Optimal stacking of noise cross-correlation functions/](https://doi.org/10.1093/gji/ggac410) _Geophysical Journal International_. 2023 Mar;232(3):1600-18. https://doi.org/10.1093/gji/ggac410
 
 ### Some taxonomy of the NoisePy variables.
 
+
 * ``station`` refers to the site that has the seismic instruments that records ground shaking.
 * `` channel`` refers to the direction of ground motion investigated for 3 component seismometers. For DAS project, it may refers to the single channel sensors.
 * ``ista`` is the index name for looping over stations
 
 * ``cc_len`` correlation length, basic window length in seconds
 * ``step`` is the window that get skipped when sliding windows in seconds
 * ``smooth_N`` number of points for smoothing the  time or frequency domain discrete arrays.
```

### Comparing `noisepy_seis-0.8.0/pyproject.toml` & `noisepy_seis-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.0/PKG-INFO` & `noisepy_seis-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.8.0
+Version: 0.8.1
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -60,77 +60,93 @@
 [![Documentation Status](https://readthedocs.org/projects/noisepy/badge/?version=latest)](https://noisepy.readthedocs.io/en/latest/?badge=latest)
 [![Build Status](https://travis-ci.com/chengxinjiang/NoisePy.svg?branch=master)](https://travis-ci.com/github/chengxinjiang/NoisePy)
 [![Codecov](https://codecov.io/gh/chengxinjiang/NoisePy/branch/master/graph/badge.svg)](https://codecov.io/gh/chengxinjiang/NoisePy)
 
 <img src="https://raw.githubusercontent.com/mdenolle/NoisePy/master/docs/figures/logo.png" width="800" height="400">
 
 ## Major updates coming
-NoisePy is going through a major refactoring to make this package easier to use and contribute.
+NoisePy is going through a major refactoring to make this package easier to develop and deploy. Submit an issue, fork the repository and create pull requests to contribute.
 
 # Installation
-The nature of NoisePy being composed of python scripts allows flexible package installation, which is essentially to build dependent libraries the scripts and related functions live upon. We recommend using [conda](https://docs.conda.io/en/latest/) or [pip](https://pypi.org/project/pip/) to install the library due to their convenience. Below are command lines we have tested to create a python environment to run NoisePy. Note that the test is performed on `macOS Big Sur (11.7)`, so it could be slightly different for other OS.
-
+The nature of NoisePy being composed of python scripts allows flexible package installation, which is essentially to build dependent libraries the scripts and related functions live upon. We recommend using [conda](https://docs.conda.io/en/latest/) or [pip](https://pypi.org/project/pip/) to install.
 
 ### Note the order of the command lines below matters ###
 
-# With Conda:
+## With Conda and pip:
 ```bash
 conda create -n noisepy python=3.8 pip
 conda activate noisepy
 conda install -c conda-forge openmpi
 pip install noisepy-seis
 ```
 
-# With virtual environment:
+## With virtual environment:
 An MPI installation is required. E.g. for macOS using [brew](https://brew.sh/) :
 ```bash
 brew install open-mpi
 ```
 
 ```bash
 python -m venv noisepy
 source noisepy/bin/activate
 pip install noisepy-seis
 ```
-To run the code on a single core, open the terminal and activate the noisepy environment before run following command. To run on institutional clusters, see installation notes for individual packages on the module list of the cluster. Examples of installation on Frontera are below.
 
 
-# Deploy using Docker
+# Functionality
+Here is a list of features of the package:
+* download continous noise data based:
+   + on webservices using obspy's core functions of [get_station](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html) and [get_waveforms](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_waveforms.html)
+   + on AWS S3 bucket calls, with a test on the SCEDC AWS Open Dataset.
+* save seismic data in [ASDF](https://asdf-definition.readthedocs.io/en/latest/) format, which convinently assembles meta, wavefrom and auxililary data into one single file ([Tutorials](https://github.com/SeismicData/pyasdf/blob/master/doc/tutorial.rst) on reading/writing ASDF files)
+* offers scripts to precondition data sets before cross correlations. This involves working with gappy data from various formats (SAC/miniSEED) and storing it on local in ASDF.
+
+* performs fast and easy cross-correlation with functionality to run in parallel through [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface)
+* **Applications module**:
+   + *Ambient noise monitoring*: measure dv/v using a wide variety of techniques in time, fourier, and wavelet domain (Yuan et al., 2021)
+   + *Surface wave dispersion*: construct dispersion images using conventional techniques.
+
+
+
+# Usage
+
+To run the code on a single core, open the terminal and activate the noisepy environment before run following commands. To run on institutional clusters, see installation notes for individual packages on the module list of the cluster.
+
+## Deploy using Docker
 We use I/O on disk, so users need root access to the file system. To install rootless docker, see instructions [here](https://docs.docker.com/engine/security/rootless/#install).
 ```bash
 docker pull  ghcr.io/mdenolle/noisepy:latest
 docker run -v ~/tmp:/tmp cross_correlate --path /tmp
 ```
 
-# Functionality
-Here is a list of features of the package:
-* download continous noise data based on obspy's core functions of [get_station](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_stations.html) and [get_waveforms](https://docs.obspy.org/packages/autogen/obspy.clients.fdsn.client.Client.get_waveforms.html)
-* save seismic data in [ASDF](https://asdf-definition.readthedocs.io/en/latest/) format, which convinently assembles meta, wavefrom and auxililary data into one single file ([Tutorials](https://github.com/SeismicData/pyasdf/blob/master/doc/tutorial.rst) on reading/writing ASDF files)
-* offers high flexibility to handle messy SAC/miniSEED data stored on your local machine and convert them into ASDF format data that could easily be pluged into NoisePy
-* performs fast and easy cross-correlation with functionality to run in parallel through [MPI](https://en.wikipedia.org/wiki/Message_Passing_Interface)
-* includes a series of monitoring functions to measure dv/v on the resulted cross-correlation functions using some recently developed new methods (see our papers for more details<sup>**</sup>)
-
-# Short tutorial
-A short tutorial on how to use NoisePy-seis can be is available as a [Jupyter notebook](https://github.com/mdenolle/NoisePy/blob/master/Jupyter_notebook/tutorial.ipynb) and can be
-[run directly in Colab](https://colab.research.google.com/github/mdenolle/NoisePy/blob/master/Jupyter_notebook/tutorial.ipynb).
+# Tutorials
+A short tutorial on how to use NoisePy-seis can be is available as a [Jupyter notebook](https://github.com/mdenolle/NoisePy/blob/master/tutorials/get_started.ipynb) and can be
+[run directly in Colab](https://colab.research.google.com/github/mdenolle/NoisePy/blob/master/tutorials/get_started.ipynb).
 
 
 This tutorial presents one simple example of how NoisePy might work! We strongly encourage you to download the NoisePy package and play it on your own! If you have any  comments and/or suggestions during running the codes, please do not hesitate to contact us through email or open an issue in this github page!
 
 Chengxin Jiang (chengxinjiang@gmail.com)
 Marine Denolle (mdenolle@uw.edu).
 
-#### Peer-Reviewed Publications Referenced
-Seats, K. J., Jesse F. L., and German A. P. "Improved ambient noise correlation functions using Welch′ s method." _Geophysical Journal International_ 188, no. 2 (2012): 513-523.
-*Jiang, C. and Denolle, M. "NoisePy: a new high-performance python tool for seismic ambient noise seismology." _Seismological Research Letter_ 91, no. 3 (2020): 1853–1866..
-** Yuan, C., Bryan, J. T., and Denolle, M. "Numerical comparison of time-, frequency- and wavelet-domain methods for coda wave interferometry." _Geophysical Journal International_ 226, no. 2 (2021): 828-846.
+## Use this reference when publishing on your work with noisepy
+
+Main code:
+* Jiang, C. and Denolle, M. [NoisePy: a new high-performance python tool for seismic ambient noise seismology.](https://doi.org/10.1785/0220190364) _Seismological Research Letter_ 91, no. 3 (2020): 1853–1866. https://doi.org/10.1785/0220190364
+
+Algorithms used:
+* (data pre-processing) Seats, K. J., Jesse F. L., and German A. P. [Improved ambient noise correlation functions using Welch′ s method.](https://doi.org/10.1111/j.1365-246X.2011.05263.x) _Geophysical Journal International_ 188, no. 2 (2012): 513-523. https://doi.org/10.1111/j.1365-246X.2011.05263.x
 
+* (dv/v in wavelet domain) Yuan, C., Bryan, J. T., and Denolle, M. [Numerical comparison of time-, frequency- and wavelet-domain methods for coda wave interferometry.](https://doi.org/10.1093/gji/ggab140) _Geophysical Journal International_ 226, no. 2 (2021): 828-846. https://doi.org/10.1093/gji/ggab140
+
+* (optimal stacking) Yang X, Bryan J, Okubo K, Jiang C, Clements T, Denolle MA. [Optimal stacking of noise cross-correlation functions/](https://doi.org/10.1093/gji/ggac410) _Geophysical Journal International_. 2023 Mar;232(3):1600-18. https://doi.org/10.1093/gji/ggac410
 
 ### Some taxonomy of the NoisePy variables.
 
+
 * ``station`` refers to the site that has the seismic instruments that records ground shaking.
 * `` channel`` refers to the direction of ground motion investigated for 3 component seismometers. For DAS project, it may refers to the single channel sensors.
 * ``ista`` is the index name for looping over stations
 
 * ``cc_len`` correlation length, basic window length in seconds
 * ``step`` is the window that get skipped when sliding windows in seconds
 * ``smooth_N`` number of points for smoothing the  time or frequency domain discrete arrays.
```

