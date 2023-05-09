# Comparing `tmp/omniplate-0.9.6.tar.gz` & `tmp/omniplate-0.9.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniplate-0.9.6.tar", max compression
+gzip compressed data, was "omniplate-0.9.82.tar", max compression
```

## Comparing `omniplate-0.9.6.tar` & `omniplate-0.9.82.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0      244 2022-05-26 16:08:15.000000 omniplate-0.9.6/README.md
--rw-r--r--   0        0        0     1789 2023-01-30 16:21:37.937132 omniplate-0.9.6/om_code/admin.py
--rw-r--r--   0        0        0     2575 2023-01-30 16:21:37.980446 omniplate-0.9.6/om_code/analyseOldTecan.py
--rw-r--r--   0        0        0     1771 2023-01-30 16:21:37.981212 omniplate-0.9.6/om_code/analyseSunrise.py
--rw-r--r--   0        0        0     2607 2023-01-30 16:21:37.981924 omniplate-0.9.6/om_code/analyseTecan.py
--rw-r--r--   0        0        0     1287 2023-01-30 16:21:38.018312 omniplate-0.9.6/om_code/clogger.py
--rw-r--r--   0        0        0    20290 2023-01-30 16:21:38.049651 omniplate-0.9.6/om_code/corrections.py
--rw-r--r--   0        0        0     1380 2023-01-30 16:21:38.087062 omniplate-0.9.6/om_code/dilution_data_lucia.tsv
--rw-r--r--   0        0        0     1893 2023-01-30 16:21:38.122549 omniplate-0.9.6/om_code/dilution_data_xiao.tsv
--rw-r--r--   0        0        0     6953 2023-01-30 16:21:38.129184 omniplate-0.9.6/om_code/getfitnesspenalty.py
--rw-r--r--   0        0        0     3666 2023-01-30 16:21:38.140112 omniplate-0.9.6/om_code/loadplatedata.py
--rw-r--r--   0        0        0      435 2022-05-26 16:08:15.000000 omniplate-0.9.6/om_code/omerrors.py
--rw-r--r--   0        0        0    17217 2023-01-30 16:21:38.326614 omniplate-0.9.6/om_code/omfitderiv.py
--rw-r--r--   0        0        0     3804 2023-01-30 16:21:38.347839 omniplate-0.9.6/om_code/omgenutils.py
--rw-r--r--   0        0        0    11315 2023-01-30 16:21:38.472683 omniplate-0.9.6/om_code/omplot.py
--rw-r--r--   0        0        0     6478 2023-01-30 16:21:38.473950 omniplate-0.9.6/om_code/omstats.py
--rw-r--r--   0        0        0     6425 2022-05-26 16:08:16.000000 omniplate-0.9.6/om_code/sunder.py
--rw-r--r--   0        0        0    89911 2023-01-30 16:21:38.529923 omniplate-0.9.6/omniplate/Omniplate.py
--rw-r--r--   0        0        0       44 2022-05-26 16:08:15.000000 omniplate-0.9.6/omniplate/__init__.py
--rw-r--r--   0        0        0    90000 2023-01-12 19:04:22.000000 omniplate-0.9.6/omniplate/temp.py
--rw-r--r--   0        0        0     1065 2023-01-30 16:23:42.005207 omniplate-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 omniplate-0.9.6/setup.py
--rw-r--r--   0        0        0     1465 1970-01-01 00:00:00.000000 omniplate-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0      244 2022-05-26 16:08:15.786293 omniplate-0.9.82/README.md
+-rw-r--r--   0        0        0     2972 2023-05-09 11:28:17.764069 omniplate-0.9.82/om_code/admin.py
+-rw-r--r--   0        0        0     2577 2023-04-24 14:56:03.000000 omniplate-0.9.82/om_code/analyseOldTecan.py
+-rw-r--r--   0        0        0     1771 2023-01-30 16:21:37.000000 omniplate-0.9.82/om_code/analyseSunrise.py
+-rw-r--r--   0        0        0     2609 2023-04-24 14:56:03.000000 omniplate-0.9.82/om_code/analyseTecan.py
+-rw-r--r--   0        0        0     1289 2023-04-24 14:56:03.000000 omniplate-0.9.82/om_code/clogger.py
+-rw-r--r--   0        0        0    24158 2023-05-09 11:28:17.764548 omniplate-0.9.82/om_code/corrections.py
+-rw-r--r--   0        0        0     1380 2023-01-30 16:21:38.000000 omniplate-0.9.82/om_code/dilution_data_lucia.tsv
+-rw-r--r--   0        0        0     1893 2023-01-30 16:21:38.000000 omniplate-0.9.82/om_code/dilution_data_xiao.tsv
+-rw-r--r--   0        0        0     6965 2023-04-24 14:56:03.000000 omniplate-0.9.82/om_code/getfitnesspenalty.py
+-rw-r--r--   0        0        0     3666 2023-01-30 16:21:38.000000 omniplate-0.9.82/om_code/loadplatedata.py
+-rw-r--r--   0        0        0     3905 2023-05-09 11:28:17.764767 omniplate-0.9.82/om_code/midlog.py
+-rw-r--r--   0        0        0      435 2022-05-26 16:08:15.904220 omniplate-0.9.82/om_code/omerrors.py
+-rw-r--r--   0        0        0    17184 2023-05-09 11:28:17.765933 omniplate-0.9.82/om_code/omfitderiv.py
+-rw-r--r--   0        0        0     4179 2023-05-09 11:28:17.774527 omniplate-0.9.82/om_code/omgenutils.py
+-rw-r--r--   0        0        0    11514 2023-05-09 11:28:17.775566 omniplate-0.9.82/om_code/omplot.py
+-rw-r--r--   0        0        0     6473 2023-05-09 11:28:17.776522 omniplate-0.9.82/om_code/omstats.py
+-rw-r--r--   0        0        0     6472 2023-05-09 11:28:17.820114 omniplate-0.9.82/om_code/sunder.py
+-rw-r--r--   0        0        0    95311 2023-05-09 11:28:17.820960 omniplate-0.9.82/omniplate/Omniplate.py
+-rw-r--r--   0        0        0       44 2022-05-26 16:08:15.902667 omniplate-0.9.82/omniplate/__init__.py
+-rw-r--r--   0        0        0     1116 2023-05-09 11:28:17.821366 omniplate-0.9.82/pyproject.toml
+-rw-r--r--   0        0        0     1532 1970-01-01 00:00:00.000000 omniplate-0.9.82/PKG-INFO
```

### Comparing `omniplate-0.9.6/om_code/analyseOldTecan.py` & `omniplate-0.9.82/om_code/analyseOldTecan.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         .to_numpy()[0]
         .split(": ")[1]
     ]
     # extract times of measurements
     t = (
         dfd.loc[
             dfd[dfd.columns[0]].str.startswith("Time [s]", na=False),
-            dfd.columns[1]:,
+            dfd.columns[1] :,
         ]
         .dropna(axis="columns")
         .mean()
         .to_numpy()
         .astype("float")
         / 3600.0
     )
@@ -57,15 +57,15 @@
     # add to dataframe
     df.index = df[cols[0]]
     rdict = []
     for x in np.arange(1, 13):
         for y in "ABCDEFGH":
             well = y + str(x)
             if well in df.index:
-                data = df.loc[well, cols[1]:].to_numpy(dtype="float")
+                data = df.loc[well, cols[1] :].to_numpy(dtype="float")
                 if data.ndim == 1:
                     data = data[None, :]
                 if (
                     rcontents[well][0] is not None
                     and rcontents[well][1] is not None
                 ):
                     for j in range(len(t)):
```

### Comparing `omniplate-0.9.6/om_code/analyseSunrise.py` & `omniplate-0.9.82/om_code/analyseSunrise.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.6/om_code/analyseTecan.py` & `omniplate-0.9.82/om_code/analyseTecan.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # if only OD data measured
     if not isinstance(datatypes[0], str):
         datatypes = ["OD"]
     # extract times of measurements
     t = (
         dfd.loc[
             dfd[dfd.columns[0]].str.startswith("Time [s]", na=False),
-            dfd.columns[1]:,
+            dfd.columns[1] :,
         ]
         .dropna(axis="columns")
         .mean()
         .to_numpy()
         .astype("float")
         / 3600.0
     )
@@ -58,15 +58,15 @@
     # add to dataframe
     df.index = df[cols[0]]
     rdict = []
     for x in np.arange(1, 13):
         for y in "ABCDEFGH":
             well = y + str(x)
             if well in df.index:
-                data = df.loc[well, cols[1]:].to_numpy(dtype="float")
+                data = df.loc[well, cols[1] :].to_numpy(dtype="float")
                 if data.ndim == 1:
                     data = data[None, :]
                 if (
                     rcontents[well][0] is not None
                     and rcontents[well][1] is not None
                 ):
                     for j in range(len(t)):
```

### Comparing `omniplate-0.9.6/om_code/clogger.py` & `omniplate-0.9.82/om_code/clogger.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     return logger, logstream
 
     ###
 
 
 def log(func):
     """To decorate functions whose output should be logged."""
+
     @functools.wraps(func)
     def wrapper(self, *args, **kwargs):
         res = func(self, *args, **kwargs)
         # store call to function in logstring
         methodname = func.__name__
         logstring = methodname + "("
         if any(args):
@@ -38,8 +39,9 @@
         if any(kwargs):
             kwargslist = [f"{k}={v!r}" for k, v in kwargs.items()]
         else:
             kwargslist = []
         logstring += ", ".join(argslist + kwargslist) + ")\n"
         self.logger.info(logstring)
         return res
+
     return wrapper
```

### Comparing `omniplate-0.9.6/om_code/corrections.py` & `omniplate-0.9.82/om_code/corrections.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,129 @@
-# functions for correcting for non-linearities in the OD, for
+# functions for correcting for non-linearity in the OD, for
 # the fluorescence of the media, and for autofluorescence
-import numpy as np
+import importlib.resources as import_files
+import re
+
+import gaussianprocessderivatives as gp
 import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+from nunchaku import Nunchaku
 from scipy.interpolate import interp1d
-import gaussianprocessderivatives as gp
-from statsmodels.nonparametric.smoothers_lowess import lowess
 from scipy.optimize import minimize_scalar
-import pandas as pd
-import re
-import importlib.resources as import_files
-import om_code.sunder as sunder
+from statsmodels.nonparametric.smoothers_lowess import lowess
+
 import om_code.omerrors as errors
 import om_code.omgenutils as gu
+import om_code.sunder as sunder
+from om_code.omfitderiv import fitderiv
 
 
 def _read_dilution_data(fname):
     d = import_files.read_text("om_code", fname)
     res = np.array(re.split(r"\n|\t", d)[:-1]).astype(float)
-    od, dilfac = res[::2], res[1::2]
+    if fname == "dilution_data_xiao.tsv":
+        od, dilfac = res[::2], res[1::2]
+        # missing replicate - use mean of existing ones
+        dilfac = np.insert(dilfac, 0, dilfac[0])
+        dilfac = dilfac.reshape(int(dilfac.size / 3), 3)
+        od = np.insert(od, 0, np.mean(od[:2]))
+        od = od.reshape(int(od.size / 3), 3)
+    else:
+        raise SystemExit("Dilution data unrecognised.")
     return od, dilfac
 
 
-def findODcorrection(wdirpath, ODfname, figs, odmatch, bd, gp_results):
+def findODcorrection(wdirpath, ODfname, figs, bd, gp_results):
     """
     Determine a function to correct OD.
 
     Use a Gaussian process to fit serial dilution data to correct for
     non-linearities in the relationship between OD and cell density.
 
     The data are either loaded from file ODfname or the default
     data for haploid yeast growing in glucose are used.
     """
-    print("Fitting dilution data for OD correction for non-linearities")
+    print("Fitting dilution data for OD correction for non-linearities.")
     if ODfname is not None:
         try:
             od_df = pd.read_csv(
                 str(wdirpath / ODfname), sep=None, engine="python", header=None
             )
-            print("Using", ODfname)
+            print(f"Using {ODfname}.")
             od_data = od_df.to_numpy()
             od, dilfac = od_data[:, 0], od_data[:, 1]
         except (FileNotFoundError, OSError):
             raise errors.FileNotFound(str(wdirpath / ODfname))
     else:
-        print("Using default data")
+        print("Using default data.")
         fname = "dilution_data_xiao.tsv"
         od, dilfac = _read_dilution_data(fname)
+    # run nunchaku
+    X = np.mean(dilfac, 1)
+    nc = Nunchaku(X, od.T, estimate_err=True, prior=[-5, 5])
+    num_regions, _ = nc.get_number(4)
+    bds, _ = nc.get_iboundaries(num_regions)
+    # linear region starts from origin
+    odmatch = np.mean(od, 1)[bds[0]]
+    dilfacmatch = X[bds[0]]
     # process data
-    dilfac = dilfac[np.argsort(od)]
-    od = np.sort(od)
-    if odmatch is not None:
-        # rescale so that OD and dilfac match at a particular OD
-        # compares better with Warringer & Blomberg, Yeast 2003,
-        # and rescaled OD is larger
-        dilfacmatch = interp1d(od, dilfac)(odmatch)
-        y = dilfac / dilfacmatch * odmatch
-    else:
-        y = dilfac
+    dilfac = dilfac.flatten()[np.argsort(od.flatten())]
+    od = np.sort(od.flatten())
+    # rescale so that OD and dilfac match
+    y = dilfac / dilfacmatch * odmatch
     # set up Gaussian process
     bds = {0: (-4, 4), 1: (-4, 4), 2: (-3, 1)}
     # find bounds
     if bd is not None:
         bds = gu.mergedicts(original=bds, update=bd)
     gc = gp.maternGP(bds, od, y)
     # run Gaussian process
     gc.findhyperparameters(noruns=5, exitearly=True, quiet=True)
     if gp_results:
         gc.results()
     gc.predict(od)
     if figs:
         plt.figure()
         gc.sketch(".")
+        plt.plot(odmatch, odmatch, "bs")
         plt.grid(True)
         plt.xlabel("OD")
         plt.ylabel("corrected OD (relative cell numbers)")
         if ODfname:
             plt.title("Fitting " + ODfname)
         else:
             plt.title("for haploid budding yeast in glucose")
-        plt.show()
-    return gc
-
-
-###
+        plt.show(block=False)
+    return gc, odmatch
 
 
-def performmediacorrection(r_df, dtype, exp, condition, figs, commonmedia, frac):
+def performmediacorrection(
+    r_df, dtype, exp, condition, figs, commonmedia, frac
+):
     """
     Correct data of type dtype for any signal from the media.
 
     Use lowess to smooth over time the media data from the Null
     wells and subtract the smoothed values from the data.
     """
     # find data for correction with condition equal to commonmedia
     df = r_df.query(
-        "experiment == @exp and condition == @commonmedia" " and strain == 'Null'"
+        "experiment == @exp and condition == @commonmedia"
+        " and strain == 'Null'"
     )
     if df.empty:
         # no data
         print(
-            ' No well annotated "Null" was found for',
-            commonmedia,
-            "in experiment",
-            exp,
+            f' No well annotated "Null" was found for {commonmedia}'
+            f"in experiment {exp}."
+        )
+        print(
+            f"-> Correcting for media for {dtype} in {commonmedia} abandoned!"
         )
-        print(" Correcting for media for", dtype, "in", commonmedia, "abandoned!")
         return False, None
     else:
         # there is data - change r dataframe
         rtest = (r_df.experiment == exp) & (r_df.condition == condition)
         t, data = df["time"].to_numpy(), df[dtype].to_numpy()
         # find correction
         res = lowess(data, t, frac=frac)
@@ -118,62 +133,81 @@
             fill_value=(res[0, 1], res[-1, 1]),
             bounds_error=False,
         )
         if figs:
             plt.figure()
             plt.plot(t, data, "ro", res[:, 0], res[:, 1], "b-")
             plt.xlabel("time (hours)")
-            plt.title(exp + ": media correction for " + dtype + " in " + condition)
-            plt.show()
+            plt.title(
+                exp + ": media correction for " + dtype + " in " + condition
+            )
+            plt.show(block=False)
         # perform correction
-        r_df.loc[rtest, dtype] = r_df[rtest][dtype] - correctionfn(r_df[rtest]["time"])
+        r_df.loc[rtest, dtype] = r_df[rtest][dtype] - correctionfn(
+            r_df[rtest]["time"]
+        )
         # check for any negative values
         negvalues = ""
         for s in np.unique(r_df[rtest]["strain"][r_df[rtest][dtype] < 0]):
             if s != "Null":
-                wstr = "\t" + dtype + ": " + s + " in " + condition + " for wells "
+                wstr = (
+                    "\t"
+                    + dtype
+                    + ": "
+                    + s
+                    + " in "
+                    + condition
+                    + " for wells "
+                )
                 for well in np.unique(
-                    r_df[rtest][r_df[rtest].strain == s]["well"][r_df[rtest][dtype] < 0]
+                    r_df[rtest][r_df[rtest].strain == s]["well"][
+                        r_df[rtest][dtype] < 0
+                    ]
                 ):
                     wstr += well + " "
                 wstr += "\n"
                 negvalues += wstr
         return True, negvalues
 
 
-###
-
-
 def correctauto1(
     self,
     f,
     refstrain,
     figs,
+    useGPs,
+    flcvfn,
+    bd,
+    nosamples,
     experiments,
     experimentincludes,
     experimentexcludes,
     conditions,
     conditionincludes,
     conditionexcludes,
     strains,
     strainincludes,
     strainexcludes,
+    **kwargs,
 ):
     """
     Correct autofluorescence for measurements with emissions at one wavelength.
 
     Corrects for autofluorescence for data with emissions measured at one
     wavelength using the fluorescence of the reference strain
     interpolated to the OD of the tagged strain.
 
     This method in principle corrects too for the fluorescence of the medium,
     although running correctmedia is still recommended.
     """
-    print("Correcting autofluorescence using", f[0])
-    for e in sunder.getexps(self, experiments, experimentincludes, experimentexcludes):
+    print("Using one fluorescence wavelength.")
+    print(f"Correcting autofluorescence using {f[0]}.")
+    for e in sunder.getexps(
+        self, experiments, experimentincludes, experimentexcludes
+    ):
         for c in sunder.getcons(
             self,
             conditions,
             conditionincludes,
             conditionexcludes,
             nomedia=True,
         ):
@@ -183,93 +217,86 @@
             for s in sunder.getstrs(
                 self, strains, strainincludes, strainexcludes, nonull=True
             ):
                 if not self.sc[
                     (self.sc.experiment == e)
                     & (self.sc.condition == c)
                     & (self.sc.strain == s)
-                ][f[0] + " corrected for autofluorescence"].any():
+                ][f[0] + "_corrected_for_autofluorescence"].any():
                     od, rawfl = sunder.extractwells(
                         self.r, self.s, e, c, s, ["OD", f[0]]
                     )
                     # no data
                     if od.size == 0 or rawfl.size == 0:
+                        print(f"\n-> No data found for {e}: {s} in {c}.\n")
                         continue
                     # correct autofluorescence for each replicate
                     fl = np.transpose(
-                        [rawfl[:, i] - refstrfn(od[:, i]) for i in range(od.shape[1])]
-                    )
-                    flperod = np.transpose(
                         [
-                            (rawfl[:, i] - refstrfn(od[:, i])) / od[:, i]
+                            rawfl[:, i] - refstrfn(od[:, i])
                             for i in range(od.shape[1])
                         ]
                     )
-                    # replace negative values with NaNs
                     fl[fl < 0] = np.nan
-                    flperod[flperod < 0] = np.nan
-                    nonans = np.count_nonzero(np.isnan(fl))
-                    if np.any(nonans):
-                        print(
-                            "Warning -",
-                            e + ":",
-                            s,
-                            "in",
+                    if useGPs:
+                        # get time
+                        t = self.s.query(
+                            "experiment == @e and condition == @c and strain == @s"
+                        )["time"].to_numpy()
+                        flperod = samplewithGPs(
+                            self,
+                            t,
+                            fl,
+                            od,
+                            flcvfn,
+                            bd,
+                            nosamples,
+                            e,
                             c,
-                            "\n",
-                            nonans,
-                            "corrected data points are"
-                            " NaN because the corrected fluorescence"
-                            " was negative",
+                            s,
+                            figs,
+                            **kwargs,
                         )
+                    else:
+                        # use only the replicates
+                        flperod = np.transpose(
+                            [fl[:, i] / od[:, i] for i in range(od.shape[1])]
+                        )
+                        flperod[flperod < 0] = np.nan
+                    # check number of NaN
+                    nonans = np.count_nonzero(np.isnan(fl))
+                    if np.any(nonans):
                         if nonans == fl.size:
                             print(
-                                "Warning -",
-                                e + ":",
-                                s,
-                                "in",
-                                c,
-                                "\n",
-                                "Corrected fluorescence is all NaN",
+                                f"\n-> Corrected fluorescence is all NaN for {e}: {s} in {c}.\n"
+                            )
+                        else:
+                            print(
+                                f"Warning - {e}: {s} in {c}\n"
+                                f"{nonans} corrected data points are"
+                                " NaN because the corrected fluorescence"
+                                " was negative.",
                             )
                     # store results
                     bname = "c-" + f[0]
                     autofdict = {
                         "experiment": e,
                         "condition": c,
                         "strain": s,
                         "time": self.s.query(
-                            "experiment == @e and condition == @c " "and strain == @s"
+                            "experiment == @e and condition == @c "
+                            "and strain == @s"
                         )["time"].to_numpy(),
                         bname: np.nanmean(fl, 1),
-                        bname + " err": nanstdzeros2nan(fl, 1),
+                        bname + "_err": nanstdzeros2nan(fl, 1),
                         bname + "perOD": np.nanmean(flperod, 1),
-                        bname + "perOD err": nanstdzeros2nan(flperod, 1),
+                        bname + "perOD_err": nanstdzeros2nan(flperod, 1),
                     }
-                    autofdf = pd.DataFrame(autofdict)
-                    if bname not in self.s.columns:
-                        # extend dataframe
-                        self.s = pd.merge(self.s, autofdf, how="outer")
-                    else:
-                        # update dataframe
-                        self.s = gu.absorbdf(
-                            self.s,
-                            autofdf,
-                            ["experiment", "condition", "strain", "time"],
-                        )
-                    # record that correction has occurred
-                    self.sc.loc[
-                        (self.sc.experiment == e)
-                        & (self.sc.condition == c)
-                        & (self.sc.strain == s),
-                        f[0] + " corrected for autofluorescence",
-                    ] = True
-
-
-###
+                    addtodataframes(self, autofdict, bname)
+                    addrecord(self, f[0], e, c, s)
 
 
 def processref1(self, f, refstrain, figs, experiment, condition):
     """
     Process reference strain for data with one fluorescence measurement.
 
     Use lowess to smooth the fluorescence of the reference
@@ -290,25 +317,18 @@
 
     Returns
     -------
     refstrfn: function
         The reference strain's fluorescence as a function of OD.
     """
     e, c = experiment, condition
-    print(
-        e + ": Processing reference strain",
-        refstrain,
-        "for",
-        f[0],
-        "in",
-        c,
-    )
+    print(f"{e}: Processing reference strain {refstrain} for {f[0]} in {c}.")
     od, fl = sunder.extractwells(self.r, self.s, e, c, refstrain, ["OD", f[0]])
     if od.size == 0 or fl.size == 0:
-        raise errors.CorrectAuto(e + ": " + refstrain + " not found in " + c)
+        raise errors.CorrectAuto(f"{e}: {refstrain} not found in {c}.")
     else:
         odf = od.flatten("F")
         flf = fl.flatten("F")
         # smooth fluorescence as a function of OD using lowess to minimize
         # refstrain's autofluorescence
 
         def choosefrac(frac):
@@ -336,35 +356,37 @@
             # plot fit
             plt.figure()
             plt.plot(odf, flf, ".", alpha=0.5)
             plt.plot(res[:, 0], res[:, 1])
             plt.xlabel("OD")
             plt.ylabel(f[0])
             plt.title(e + ": " + refstrain + " for " + c)
-            plt.show()
+            plt.show(block=False)
         return refstrfn
 
 
-###
-
-
 def correctauto2(
     self,
     f,
     refstrain,
     figs,
+    useGPs,
+    flcvfn,
+    bd,
+    nosamples,
     experiments,
     experimentincludes,
     experimentexcludes,
     conditions,
     conditionincludes,
     conditionexcludes,
     strains,
     strainincludes,
     strainexcludes,
+    **kwargs,
 ):
     """
     Correct autofluorescence for measurements with two emission wavelengths.
 
     Corrects for autofluorescence using spectral unmixing for data with
     measured emissions at two wavelengths.
 
@@ -372,16 +394,19 @@
     ----------
     CA Lichten, R White, IB Clark, PS Swain (2014). Unmixing of fluorescence
     spectra to resolve quantitative time-series measurements of gene
     expression in plate readers.
     BMC Biotech, 14, 1-11.
     """
     # correct for autofluorescence
-    print("Correcting autofluorescence using", f[0], "and", f[1])
-    for e in sunder.getexps(self, experiments, experimentincludes, experimentexcludes):
+    print("Using two fluorescence wavelengths.")
+    print(f"Correcting autofluorescence using {f[0]} and {f[1]}.")
+    for e in sunder.getexps(
+        self, experiments, experimentincludes, experimentexcludes
+    ):
         for c in sunder.getcons(
             self,
             conditions,
             conditionincludes,
             conditionexcludes,
             nomedia=True,
         ):
@@ -392,64 +417,75 @@
                 self, strains, strainincludes, strainexcludes, nonull=True
             ):
                 if s != refstrain and not (
                     self.sc[
                         (self.sc.experiment == e)
                         & (self.sc.condition == c)
                         & (self.sc.strain == s)
-                    ][f[0] + " corrected for autofluorescence"].any()
+                    ][f[0] + "_corrected_for_autofluorescence"].any()
                 ):
-                    f0, f1 = sunder.extractwells(self.r, self.s, e, c, s, f)
+                    f0, f1, od = sunder.extractwells(
+                        self.r, self.s, e, c, s, f.copy() + ["OD"]
+                    )
                     if f0.size == 0 or f1.size == 0:
+                        print(f"Warning: No data found for {e}: {s} in {c} !!")
                         continue
                     nodata, nr = f0.shape
                     # set negative values to NaNs
                     f0[f0 < 0] = np.nan
                     f1[f1 < 0] = np.nan
                     # use mean OD for correction
                     odmean = self.s.query(
                         "experiment == @e and condition == @c and strain == @s"
-                    )["OD mean"].to_numpy()
-                    # remove autofluorescence
+                    )["OD_mean"].to_numpy()
+                    # correct autofluorescence
                     ra = refqrfn(odmean)
                     fl = applyautoflcorrection(self, ra, f0, f1)
-                    od = sunder.extractwells(self.r, self.s, e, c, s, "OD")
-                    flperod = fl / od
-                    # set negative values to NaNs
                     fl[fl < 0] = np.nan
-                    flperod[flperod < 0] = np.nan
+                    # get time
+                    t = self.s.query(
+                        "experiment == @e and condition == @c and strain == @s"
+                    )["time"].to_numpy()
                     # store corrected fluorescence
                     bname = "c-" + f[0]
                     autofdict = {
                         "experiment": e,
                         "condition": c,
                         "strain": s,
-                        "time": self.s.query(
-                            "experiment == @e and condition == @c" " and strain == @s"
-                        )["time"].to_numpy(),
+                        "time": t,
                         bname: np.nanmean(fl, 1),
                         bname + " err": nanstdzeros2nan(fl, 1),
-                        bname + "perOD": np.nanmean(flperod, 1),
-                        bname + "perOD err": nanstdzeros2nan(flperod, 1),
                     }
-                    # add to dataframe
-                    self.s = gu.absorbdf(
-                        self.s,
-                        pd.DataFrame(autofdict),
-                        ["experiment", "condition", "strain", "time"],
+                    if useGPs:
+                        flperod = samplewithGPs(
+                            self,
+                            t,
+                            fl,
+                            od,
+                            flcvfn,
+                            bd,
+                            nosamples,
+                            e,
+                            c,
+                            s,
+                            figs,
+                            **kwargs,
+                        )
+                    else:
+                        # use only the replicates
+                        flperod = fl / od
+                        flperod[flperod < 0] = np.nan
+                    # update dict
+                    autofdict[bname + "perOD_err"] = naniqrzeros2nan(
+                        flperod, 1
                     )
-                    self.sc.loc[
-                        (self.sc.experiment == e)
-                        & (self.sc.condition == c)
-                        & (self.sc.strain == s),
-                        f[0] + " corrected for autofluorescence",
-                    ] = True
-
-
-###
+                    autofdict[bname + "perOD"] = np.nanmean(flperod, 1)
+                    # add to data frames
+                    addtodataframes(self, autofdict, bname)
+                    addrecord(self, f[0], e, c, s)
 
 
 def processref2(self, f, refstrain, figs, experiment, condition):
     """
     Process reference strain for spectral unmixing.
 
     Requires data with two fluorescence measurements.
@@ -470,41 +506,36 @@
         The experiment to be corrected.
     condition: string
         The condition to be corrected.
 
     Returns
     -------
     qrfn: function
-        The ratio of the two fluorescences for the reference strain as a
-        function of OD.
+        The ratio of the two fluorescence values for the reference strain
+        as a function of OD.
     """
     e, c = experiment, condition
-    print(
-        e + ": Processing reference strain",
-        refstrain,
-        "for",
-        f[0],
-        "in",
-        c,
-    )
+    print(f"{e}: Processing reference strain {refstrain} for {f[0]} in {c}.")
     # refstrain data
-    f0, f1, od = sunder.extractwells(self.r, self.s, e, c, refstrain, f + ["OD"])
+    f0, f1, od = sunder.extractwells(
+        self.r, self.s, e, c, refstrain, f + ["OD"]
+    )
     if f0.size == 0 or f1.size == 0 or od.size == 0:
-        raise errors.CorrectAuto(e + ": " + refstrain + " not found in " + c)
+        raise errors.CorrectAuto(f"{e}: {refstrain} not found in {c}.")
     else:
         f0[f0 < 0] = np.nan
         f1[f1 < 0] = np.nan
         odf = od.flatten("F")
         odrefmean = np.mean(od, 1)
         qrf = (f1 / f0).flatten("F")
         if np.all(np.isnan(qrf)):
             raise errors.CorrectAuto(
-                e + ": " + refstrain + " in " + c + " has too many NaNs"
+                f"{e}: {refstrain} in {c} has too many NaNs."
             )
-        # smooth to minimize autofluorescence in refstrain
+        # smooth to minimise autofluorescence in refstrain
 
         def choosefrac(frac):
             res = lowess(qrf, odf, frac)
             qrfn = interp1d(
                 res[:, 0],
                 res[:, 1],
                 fill_value=(res[0, 1], res[-1, 1]),
@@ -526,15 +557,15 @@
         if figs:
             plt.figure()
             plt.plot(odf, qrf, ".", alpha=0.5)
             plt.plot(res[:, 0], res[:, 1])
             plt.xlabel("OD")
             plt.ylabel(f[1] + "/" + f[0])
             plt.title(e + ": " + refstrain + " in " + c)
-            plt.show()
+            plt.show(block=False)
         # check autofluorescence correction for reference strain
         flref = applyautoflcorrection(self, qrfn(odrefmean), f0, f1)
         flrefperod = flref / od
         # set negative values to NaNs
         flref[flref < 0] = np.nan
         flrefperod[flrefperod < 0] = np.nan
         # store results
@@ -544,39 +575,132 @@
             "condition": c,
             "strain": refstrain,
             "time": self.s.query(
                 "experiment == @e and condition == @c and strain == @refstrain"
             )["time"].to_numpy(),
             bname: np.nanmean(flref, 1),
             bname + "perOD": np.nanmean(flrefperod, 1),
-            bname + " err": nanstdzeros2nan(flref, 1),
-            bname + "perOD err": nanstdzeros2nan(flrefperod, 1),
+            bname + "_err": nanstdzeros2nan(flref, 1),
+            bname + "perOD_err": nanstdzeros2nan(flrefperod, 1),
         }
-        if bname not in self.s.columns:
-            self.s = pd.merge(self.s, pd.DataFrame(autofdict), how="outer")
-        else:
-            self.s = gu.absorbdf(
-                self.s,
-                pd.DataFrame(autofdict),
-                ["experiment", "condition", "strain", "time"],
-            )
+        addtodataframes(self, autofdict, bname)
         return qrfn
 
 
-###
-
-
 def applyautoflcorrection(self, ra, f0data, f1data):
     """Correct for autofluorescence returning an array of replicates."""
     nr = f0data.shape[1]
     raa = np.reshape(np.tile(ra, nr), (np.size(ra), nr), order="F")
-    return (raa * f0data - f1data) / (raa - self._gamma * np.ones(np.shape(raa)))
+    return (raa * f0data - f1data) / (
+        raa - self._gamma * np.ones(np.shape(raa))
+    )
 
 
-###
+def addtodataframes(self, autofdict, bname):
+    """Added dict of autofluorescence corrections to data frames."""
+    autofdf = pd.DataFrame(autofdict)
+    if bname not in self.s.columns:
+        # extend dataframe
+        self.s = pd.merge(self.s, autofdf, how="outer")
+    else:
+        # update dataframe
+        self.s = gu.absorbdf(
+            self.s,
+            autofdf,
+            ["experiment", "condition", "strain", "time"],
+        )
+
+
+def addrecord(self, fname, e, c, s):
+    """Record correction."""
+    self.sc.loc[
+        (self.sc.experiment == e)
+        & (self.sc.condition == c)
+        & (self.sc.strain == s),
+        fname + "_corrected_for_autofluorescence",
+    ] = True
 
 
 def nanstdzeros2nan(a, axis=None):
     """Like nanstd but setting zeros to nan."""
     err = np.nanstd(a, axis)
     err[err == 0] = np.nan
     return err
+
+
+def naniqrzeros2nan(a, axis=None):
+    """Interquartile range but setting zeros to nan."""
+    iqr = np.nanquantile(a, 0.75, axis) - np.nanquantile(a, 0.25, axis)
+    iqr[iqr == 0] = np.nan
+    return iqr
+
+
+def gethypers(self, exp, con, s, dtype="gr"):
+    """Find parameters for GP from sc data frame."""
+    sdf = self.sc[
+        (self.sc.experiment == exp)
+        & (self.sc.condition == con)
+        & (self.sc.strain == s)
+    ]
+    try:
+        cvfn = sdf["gp_for_gr"].values[0]
+        hypers = [
+            sdf[col].values[0] for col in sorted(sdf.columns) if "hyper" in col
+        ]
+        if np.any(np.isnan(hypers)):
+            return None, None
+        else:
+            return hypers, cvfn
+    except KeyError:
+        return None, None
+
+
+def samplewithGPs(
+    self, t, fl, od, flcvfn, bd, nosamples, e, c, s, figs, **kwargs
+):
+    """Generate extra samples of flperod using Gaussian processes."""
+    hypers, cvfn = gethypers(self, e, c, s)
+    if hypers is None or cvfn is None:
+        raise SystemExit(
+            f"\nYou first must run getstats for {s} in {c} for {e}."
+        )
+    # initialise GP for log ODs
+    t1 = np.tile(t, od.shape[1])
+    od1 = np.reshape(od, od.size, order="F")
+    od1 = od1[np.argsort(t1)]
+    t1 = np.sort(t1)
+    # bounds are irrelevant because parameters are optimal
+    go = getattr(gp, cvfn + "GP")(
+        {0: (-5, 5), 1: (-4, 4), 2: (-5, 2)},
+        t1,
+        np.log(od1),
+    )
+    go.lth_opt = hypers
+    go.predict(t)
+    # run GP for log fluorescence
+    print(f"Fitting fluorescence for {e}: {s} in {c}")
+    ff = fitderiv(
+        t,
+        fl,
+        cvfn=flcvfn,
+        bd=bd,
+        logs=True,
+        stats=False,
+        **kwargs,
+    )
+    if ff.success:
+        print()
+        if figs:
+            plt.figure()
+            ff.plotfit(
+                ylabel="log fluorescence",
+                figtitle=f"{e}: {s} in {c}",
+            )
+            plt.show(block=False)
+    else:
+        print(f"\n-> Fitting fluorescence failed for {e}: {s} in {c}.\n")
+        return np.nan * np.ones(fl.shape)
+    # sample
+    lod_samples = go.sample(nosamples)
+    lfl_samples = ff.fitderivsample(nosamples)[0]
+    flperod = np.exp(lfl_samples - lod_samples)
+    return flperod
```

### Comparing `omniplate-0.9.6/om_code/dilution_data_lucia.tsv` & `omniplate-0.9.82/om_code/dilution_data_lucia.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.6/om_code/dilution_data_xiao.tsv` & `omniplate-0.9.82/om_code/dilution_data_xiao.tsv`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.6/om_code/getfitnesspenalty.py` & `omniplate-0.9.82/om_code/getfitnesspenalty.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 from scipy import integrate
 from scipy.interpolate import interp1d
 import matplotlib.pylab as plt
 import om_code.omerrors as errors
 from om_code.stats import statserr
 
+
 def getfitnesspenalty(
     self, ref, com, y="gr", abs=False, figs=True, nosamples=100, norm=False
 ):
     """
     Estimate the difference in fitness between two strains.
 
     Calculate the area between typically two growth rate versus OD
@@ -174,15 +175,15 @@
                 [
                     ref[0] + ": " + ref[2] + " in " + ref[1],
                     com[0] + ": " + com[2] + " in " + com[1],
                 ],
                 loc="upper left",
                 bbox_to_anchor=(-0.05, 1.15),
             )
-            plt.show()
+            plt.show(block=False)
     if norm:
         return (
             np.median(fps),
             statserr(fps),
             np.median(nrm),
             statserr(nrm),
         )
```

### Comparing `omniplate-0.9.6/om_code/loadplatedata.py` & `omniplate-0.9.82/om_code/loadplatedata.py`

 * *Files identical despite different names*

### Comparing `omniplate-0.9.6/om_code/omfitderiv.py` & `omniplate-0.9.82/om_code/omfitderiv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
 import warnings
 import matplotlib.pylab as plt
 from scipy.interpolate import interp1d
 import copy
 import gaussianprocessderivatives as gp
 import om_code.omgenutils as gu
+import om_code.omstats as omstats
 
 
 class fitderiv:
     """
     Smooth and estimate the time derivative of the data via Gaussian processes.
 
     Summary statistics - the maximal time derivative, the time at which the
@@ -68,15 +69,15 @@
     Nat Commun 7 (2016) 13766
     """
 
     def __init__(
         self,
         t,
         d,
-        cvfn="sqexp",
+        cvfn="matern",
         logs=True,
         noruns=5,
         noinits=100,
         exitearly=False,
         bd=False,
         empirical_errors=False,
         optmethod="L-BFGS-B",
@@ -85,21 +86,19 @@
         statnames=False,
         showstaterrors=True,
         warn=False,
         linalgmax=3,
         iskip=False,
     ):
         """
-        Smooth data and estimate its time derivatives.
-
-        The Gaussian process used performs both tasks.
+        Smooth data and estimate time derivatives with a Gaussian process.
 
         Parameters
         ----------
-        t: array
+        t: 1D array
             The time points.
         d: array
             The data corresponding to the time points with any replicates given
              as columns.
         cvfn: string
             The type of kernel function for the Gaussian process either 'sqexp'
             (squared exponential) or 'matern' (Matern with nu= 5/2) or 'nn'
@@ -112,15 +111,15 @@
             The number of attempts to be made at optimising the kernel's
             hyperparmeters.
         noinits: integer, optional
             The number of random attempts made to find good initial choices for
             the hyperparameters before running their optimisation.
         exitearly: boolean, optional
             If True, stop at the first successful attempt at optimising the
-            hyperparameters otherwwise take the best choice from all successful
+            hyperparameters otherwise take the best choice from all successful
             optimisations.
         bd: dictionary, optional
             Specifies the limits on the hyperparameters for the Gaussian process.
             For example, bd= {0: [-1, 4], 2: [2, 6]})
             sets confines the first hyperparameter to be between 1e-1 and 1e^4
             and confines the third hyperparmater between 1e2 and 1e6.
         empirical_errors: boolean, optional
@@ -132,15 +131,15 @@
         optmethod: string, optional
             The algorithm used to optimise the hyperparameters, either
             'l_bfgs_b' or 'tnc'.
         nosamples: integer, optional
             The number of bootstrap samples taken to estimate errors in
             statistics.
         stats: boolean, optional
-            If True, calcuate summary statistics for both the smoothed data and
+            If True, calculate summary statistics for both the smoothed data and
             the inferred time- derivative.
         statnames: list of strings
             To customise the names of the statistics.
             The default names are:
             'max df' for the maximal time derivative;
             'time of max df' for the time at which the maximal time
             derivative occurs;
@@ -186,60 +185,49 @@
             d = self.d
         # default bounds for hyperparameters
         bddict = {
             "nn": {0: (-1, 5), 1: (-7, -2), 2: (-6, 2)},
             "sqexp": {0: (-5, 5), 1: (-6, 2), 2: (-5, 2)},
             "matern": {0: (-5, 5), 1: (-4, 4), 2: (-5, 2)},
         }
-        # display details of covariance function
-        try:
-            # find bounds
-            if bd:
-                bds = gu.mergedicts(original=bddict[cvfn], update=bd)
-            else:
-                bds = bddict[cvfn]
-            gt = getattr(gp, cvfn + "GP")(bds, t, d)
-            print("Using a " + gt.description + ".")
-            gt.info
-        except NameError:
-            raise (SystemExit("Gaussian process not recognised"))
-        self.bds = bds
+        # find bounds
+        if bd:
+            self.bds = gu.mergedicts(original=bddict[cvfn], update=bd)
+        else:
+            self.bds = bddict[cvfn]
         # log data
         self.logs = logs
         if logs:
-            print("Taking natural logarithm of the data")
+            print("Taking natural logarithm of the data.")
             if np.any(np.nonzero(d < 0)):
-                print(
-                    "Negative data found, but all data must be positive "
-                    "if taking logs"
-                )
-                self.success = False
-            else:
-                # replace zeros by machine error so that logs can be applied
-                d[d == 0] = np.finfo(float).eps
-                # take log of data
-                d = np.log(np.asarray(d))
+                print("Warning: Negative data is being set to NaN.")
+            # replace zeros and negs so that logs can be applied
+            d[np.nonzero(d <= 0)] = np.nan
+            # take log of data
+            d = np.log(np.asarray(d))
         # run checks and define measurement errors
         if empirical_errors:
             # errors must be empirically estimated
             if noreps > 1:
-                lod = [np.count_nonzero(np.isnan(d[:, i])) for i in range(noreps)]
+                lod = [
+                    np.count_nonzero(np.isnan(d[:, i])) for i in range(noreps)
+                ]
                 if np.sum(np.diff(lod)) != 0:
                     print(
                         "The replicates have different number of data "
                         "points, but equal numbers of data points are "
-                        "needed for empirically estimating errors"
+                        "needed for empirically estimating errors."
                     )
                     merrors = None
                 else:
                     # estimate errors empirically
-                    print("Estimating measurement errors empirically")
+                    print("Estimating measurement errors empirically.")
                     merrors = gu.findsmoothvariance(d)
             else:
-                print("Not enough replicates to estimate errors empirically")
+                print("Not enough replicates to estimate errors empirically.")
                 merrors = None
         else:
             merrors = None
         self.merrors = merrors
         # combine data into one array
         tb = np.tile(t, noreps)
         db = np.reshape(d, np.size(d), order="F")
@@ -252,20 +240,20 @@
         else:
             keep = np.nonzero(~np.isnan(db))[0]
         # remove any NaNs
         da = db[keep]
         ta = tb[keep]
         # check data remains after removing NaNs
         if not np.any(da):
-            print("Warning: fitderiv failed - too many NaNs")
+            print("Warning: omfitderiv failed - too many NaNs.")
             self.success = False
         elif np.any(merrors):
             ma = mb[keep]
             if not np.any(ma):
-                print("Warning: fitderiv failed - too many NaNs")
+                print("Warning: omfitderiv failed - too many NaNs.")
                 self.success = False
         else:
             ma = None
         if self.success:
             self.run(
                 cvfn,
                 ta,
@@ -293,16 +281,21 @@
         optmethod,
         stats,
         nosamples,
         statnames,
         showstaterrors,
     ):
         """Instantiate and run a Gaussian process."""
-        # instantiate Gaussian process
-        g = getattr(gp, cvfn + "GP")(self.bds, ta, da, merrors=ma)
+        try:
+            # instantiate GP
+            g = getattr(gp, cvfn + "GP")(self.bds, ta, da, merrors=ma)
+            print("Using a " + g.description + ".")
+            g.info
+        except NameError:
+            raise Exception("Gaussian process not recognised.")
         # optimise parameters
         g.findhyperparameters(
             noruns,
             noinits=noinits,
             exitearly=exitearly,
             optmethod=optmethod,
             linalgmax=self.linalgmax,
@@ -334,14 +327,17 @@
     def fitderivsample(self, nosamples, newt=None):
         """
         Generate samples from the latent function.
 
         Both values for the latent function and its first two
         derivatives are returned, as a tuple.
 
+        All derivatives must be sampled because by default all are asked
+        to be predicted by the underlying Gaussian process.
+
         Parameters
         ----------
         nosamples: integer
             The number of samples.
         newt: array, optional
             Time points for which the samples should be made.
             If None, the orginal time points are used.
@@ -376,45 +372,47 @@
         nosamples: integer
             The number of bootstrap samples used to estimate errors.
         statnames: list of strings, optional
             A list of alternative names for the statistics.
         showerrors: boolean, optional
             If True, display the estimated errors.
         """
-        print("\nCalculating statistics with " + str(nosamples) + " samples")
+        print(f"\nCalculating statistics with {nosamples} samples.")
         if showerrors:
             print("\t(displaying median +/- half interquartile range)\n")
         if statnames:
             self.stats = statnames
         else:
             self.stats = [
-                "max df",
-                "time of max df",
-                "doubling time from max df",
-                "lag time",
+                "max_df",
+                "time_of_max_df",
+                "doubling_time_from_max_df",
+                "lag_time",
             ]
         t = self.t
         fs, gs, hs = self.fitderivsample(nosamples)
         # calculate stats
         im = np.argmax(gs, 0)
         # max df
         mgr = gs[im, np.arange(nosamples)]
         # time of max df
         tmgr = np.array([t[i] for i in im])
         # inverse max df
         dt = np.log(2) / mgr
         # lag time
         lagtime = (
-            tmgr + (fs[0, np.arange(nosamples)] - fs[im, np.arange(nosamples)]) / mgr
+            tmgr
+            + (fs[0, np.arange(nosamples)] - fs[im, np.arange(nosamples)])
+            / mgr
         )
         # store stats
         ds = {}
         for stname, st in zip(self.stats, [mgr, tmgr, dt, lagtime]):
             ds[stname] = np.median(st)
-            ds[stname + " err"] = gu.findiqr(st) / 2
+            ds[stname + "_err"] = omstats.statserr(st) / 2
         self.ds = ds
         self.nosamples = nosamples
         self.printstats(showerrors=showerrors)
 
     def printstats(self, showerrors=True, performprint=True):
         """
         Create and print a dictionary of statistics.
@@ -435,23 +433,26 @@
             The statistics and their errors.
         """
         ds = self.ds
         statd = {}
         lenstr = np.max([len(s) for s in self.stats])
         for s in self.stats:
             statd[s] = ds[s]
-            statd[s + " err"] = ds[s + " err"]
+            statd[s + "_err"] = ds[s + "_err"]
             if performprint:
                 stname = s.rjust(lenstr + 1)
                 if showerrors:
                     print(
-                        "{:s}= {:6e} +/- {:6e}".format(stname, statd[s], ds[s + " err"])
+                        "{:s}= {:6e} +/- {:6e}".format(
+                            stname, statd[s], ds[s + "_err"]
+                        )
                     )
                 else:
                     print("{:s}= {:6e}".format(stname, statd[s]))
+        print()
         return statd
 
     def plotfit(
         self, char="f", errorfac=1, xlabel="time", ylabel=False, figtitle=False
     ):
         """
         Plot the results of the fitting.
```

### Comparing `omniplate-0.9.6/om_code/omgenutils.py` & `omniplate-0.9.82/om_code/omgenutils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,23 @@
 # general functions for a variety of purposes
 import numpy as np
 
 
+@property
+def cols_to_underscore(self):
+    """Replace spaces in column names of all dataframes with underscores."""
+    for df in [self.r, self.s, self.sc]:
+        df.columns = df.columns.str.replace(" ", "_")
+
+
+def rm_under(str):
+    """Replace underscore in a string with a space."""
+    return str.replace("_", " ")
+
+
 def mergedicts(original, update):
     """
     Merge two dicts into one.
 
     Parameters
     --
     x: first dict
@@ -121,23 +133,24 @@
     ell: list
     """
     if isinstance(ell, list):  # Is a list
         return all(map(islistempty, ell))
     return False  # Not a list
 
 
-def findiqr(d):
-    """
-    Find the interquartile range of data in an array.
-
-    Parameters
-    --
-    d: a one-dimensional array of data
-    """
-    return np.subtract(*np.percentile(d, [75, 25]))
+# to be deleted - use scipy instead
+# def findiqr(d):
+#     """
+#     Find the interquartile range of data in an array.
+
+#     Parameters
+#     --
+#     d: a one-dimensional array of data
+#     """
+#     return np.subtract(*np.percentile(d, [75, 25]))
 
 
 def makelist(c):
     """
     Ensure that a variable is a list.
 
     Parameters
```

### Comparing `omniplate-0.9.6/om_code/omplot.py` & `omniplate-0.9.82/om_code/omplot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # functions to plot from the data frames
 import matplotlib.pyplot as plt
-import seaborn as sns
 import numpy as np
 import pandas as pd
-import om_code.omgenutils as gu
+import seaborn as sns
+
 import om_code.omerrors as errors
+import om_code.omgenutils as gu
 
 
 def plotplate(basedf, exps, dtype):
     """
     Plot the data for each well following the layout of a 96-well plate.
 
     Parameters
@@ -43,15 +44,15 @@
             coll = int(pl[1:])
             sindex = coll + 12 * rowl
             wd = basedf.query("experiment == @e and well == @pl")
             ax[sindex - 1].plot(
                 wd["time"].to_numpy(), wd[dtype].to_numpy(), "-"
             )
         plt.suptitle(e + ": " + dtype)
-        plt.show()
+        plt.show(block=False)
 
 
 def plot_wells(
     x,
     y,
     basedf,
     exps,
@@ -63,15 +64,15 @@
     col=None,
     row=None,
     xlim=None,
     ylim=None,
     title=None,
     figsize=None,
     messages=False,
-    **kwargs
+    **kwargs,
 ):
     """
     Plot data from the individual wells.
 
     Data for each experiment, condition, and strain are plotted in
     a separate figure unless row and col are specified.
     """
@@ -99,15 +100,15 @@
                 plt.xlim(xlim)
             if ylim is not None:
                 plt.ylim(ylim)
             if figsize and len(figsize) == 2:
                 sfig.fig.set_figwidth(figsize[0])
                 sfig.fig.set_figheight(figsize[1])
             plt.tight_layout()
-            plt.show()
+            plt.show(block=False)
         else:
             # create one plot for each strain and condition
             for c in cons:
                 for s in strs:
                     df = basedf.query(
                         "experiment == @e and condition == @c and strain == @s"
                     )
@@ -130,15 +131,15 @@
                         else:
                             sfig.fig.suptitle(e + ": " + s + " in " + c)
                         if xlim is not None:
                             plt.xlim(xlim)
                         if ylim is not None:
                             plt.ylim(ylim)
                         plt.tight_layout()
-                        plt.show()
+                        plt.show(block=False)
 
 
 def plot_rs(
     x,
     y,
     basedf,
     exps,
@@ -154,15 +155,15 @@
     aspect=1,
     xlim=None,
     ylim=None,
     title=None,
     figsize=None,
     sortby=False,
     returnfacetgrid=False,
-    **kwargs
+    **kwargs,
 ):
     """Plot time-series data from the .r or .s dataframes."""
     # plot time series
     df = basedf.query(
         "experiment == @exps and condition == @cons and strain == @strs"
     )
     if df.empty:
@@ -207,24 +208,26 @@
             size=size,
             col=col,
             row=row,
             aspect=aspect,
             height=height,
             **kwargs,
         )
+        sfig.set_xlabels(gu.rm_under(x))
+        sfig.set_ylabels(gu.rm_under(y))
         if title:
             sfig.fig.suptitle(title)
         if xlim is not None:
             sfig.set(xlim=xlim)
         if ylim is not None:
             sfig.set(ylim=ylim)
         if figsize and len(figsize) == 2:
             sfig.fig.set_figwidth(figsize[0])
             sfig.fig.set_figheight(figsize[1])
-        plt.show()
+        plt.show(block=False)
         if returnfacetgrid:
             return sfig
         else:
             return None
 
 
 def plot_sc(
@@ -243,15 +246,15 @@
     height=5,
     aspect=1,
     xlim=None,
     ylim=None,
     figsize=None,
     title=None,
     sortby=False,
-    **kwargs
+    **kwargs,
 ):
     """Plot summary statistics from the .sc dataframe."""
     # plot summary stats
     df = basedf.query(
         "experiment == @exps and condition == @cons and strain == @strs"
     )
     xcols = df.columns[df.columns.str.startswith(x)]
@@ -276,39 +279,41 @@
             size=size,
             col=col,
             row=row,
             aspect=aspect,
             height=height,
             **kwargs,
         )
+        sfig.set_xlabels(gu.rm_under(x))
+        sfig.set_ylabels(gu.rm_under(y))
         if xlim is not None:
             sfig.set(xlim=xlim)
         if ylim is not None:
             sfig.set(ylim=ylim)
         if row is None and col is None:
             # add error bars
             # find coordinates of points in relplot
             xc, yc = [], []
             for point_pair in sfig.ax.collections:
                 for xp, yp in point_pair.get_offsets():
                     xc.append(xp)
                     yc.append(yp)
             # add error bars
-            xerr = df[x + " err"] if x + " err" in df.columns else None
-            yerr = df[y + " err"] if y + " err" in df.columns else None
+            xerr = df[x + "_err"] if x + "_err" in df.columns else None
+            yerr = df[y + "_err"] if y + "_err" in df.columns else None
             sfig.ax.errorbar(
                 xc,
                 yc,
                 xerr=xerr,
                 yerr=yerr,
                 fmt=" ",
                 ecolor="dimgray",
                 alpha=0.5,
             )
-        plt.show()
+        plt.show(block=False)
 
 
 def plotfinddf(self, x, y):
     """
     Find the correct dataframe for plotting y versus x.
 
     Parameters
@@ -337,18 +342,16 @@
         dfname = "s"
     elif x in self.sc.columns and y in self.sc.columns:
         # summary stats
         basedf = self.sc
         dfname = "sc"
     else:
         raise errors.PlotError(
-            "The variables x= "
-            + x
-            + " and y= "
-            + y
+            f"The variables x= {x}"
+            + f" and y= {y}"
             + " cannot be plotted against each other because they are not in "
             + " the same dataframe"
         )
     return basedf, dfname
 
 
 def augmentdf(df, datatype):
@@ -359,18 +362,18 @@
     errors in relplot, otherwise returns original dataframe.
 
     Note we call seaborn with errorbar = "sd" and so use sqrt(3/2) * error
     because seaborn calculates the standard deviation from the augmented data
     (the mean, the mean + std, and the mean - std) and so gets
     std/sqrt(3/2) otherwise because there are three data points.
     """
-    if datatype + " err" in df:
-        derr = datatype + " err"
-    elif "mean" in datatype and datatype.split(" mean")[0] + " err" in df:
-        derr = datatype.split(" mean")[0] + " err"
+    if datatype + "_err" in df:
+        derr = datatype + "_err"
+    elif "mean" in datatype and datatype.split("_mean")[0] + "_err" in df:
+        derr = datatype.split("_mean")[0] + "_err"
     else:
         derr = False
         # returned if df is df_r
         return df
     if derr:
         df.insert(0, "augtype", "mean")
         mn = df[datatype].to_numpy()
```

### Comparing `omniplate-0.9.6/om_code/omstats.py` & `omniplate-0.9.82/om_code/omstats.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # functions to calculate the statistics
-import pandas as pd
 import numpy as np
-from scipy.signal import find_peaks
+import pandas as pd
 from scipy import integrate
 from scipy.interpolate import interp1d
-import om_code.omgenutils as gu
+from scipy.signal import find_peaks
+from scipy.stats import iqr
 
 
-def statserr(d):
+def statserr(d, **kwargs):
     """
     Use the half the interquartile range as an error.
 
     For errors in statistics calculated from samples from a
     Gaussian process to be consistent with fitderiv.
     """
-    return gu.findiqr(d) / 2
+    return iqr(d)
 
 
 def cleansc(self):
     """Ensure that NaNs do not change numeric variables from being floats."""
     floatvars = [
-        "log2 OD ratio",
-        "log2 OD ratio err",
-        "local max gr",
-        "local max gr err",
-        "time of local max gr",
-        "time of local max gr err",
-        "area under gr vs OD",
-        "area under gr vs OD err",
-        "normalized area under gr vs OD",
-        "normalized area under gr vs OD err",
-        "area under OD",
-        "area under OD err",
-        "normalized area under OD",
-        "normalized area under OD err",
-        "OD logmaxlike",
-        "max gr",
-        "max gr err",
-        "time of max gr",
-        "time of max gr err",
-        "doubling time",
-        "doubling time err",
-        "max OD",
-        "max OD err",
-        "lag time",
-        "lag time err",
+        "log2_OD_ratio",
+        "log2_OD_ratio_err",
+        "local_max_gr",
+        "local_max_gr_err",
+        "time_of_local_max_gr",
+        "time_of_local_max_gr_err",
+        "area_under_gr_vs_OD",
+        "area_under_gr_vs_OD_err",
+        "normalised_area_under_gr_vs_OD",
+        "normalised_area_under_gr_vs_OD_err",
+        "area_under_OD",
+        "area_under_OD_err",
+        "normalised_area_under_OD",
+        "normalised_area_under_OD_err",
+        "OD_logmaxlike",
+        "max_gr",
+        "max_gr_err",
+        "time_of_max_gr",
+        "time_of_max_gr_err",
+        "doubling_time",
+        "doubling_time_err",
+        "max_OD",
+        "max_OD_err",
+        "lag_time",
+        "lag_time_err",
     ]
     for var in floatvars:
         if var in self.sc.columns:
             self.sc[var] = self.sc[var].astype(float)
 
 
 def findsummarystats(
@@ -74,19 +74,19 @@
     outdf = pd.DataFrame(
         {
             "experiment": e,
             "condition": c,
             "strain": s,
             "time": t,
             "f" + odtype: f.f,
-            "f" + odtype + " err": np.sqrt(f.fvar),
+            "f" + odtype + "_err": np.sqrt(f.fvar),
             derivname: f.df,
-            derivname + " err": np.sqrt(f.dfvar),
-            "d/dt " + derivname: f.ddf,
-            "d/dt " + derivname + " err": np.sqrt(f.ddfvar),
+            derivname + "_err": np.sqrt(f.dfvar),
+            "d/dt_" + derivname: f.ddf,
+            "d/dt_" + derivname + "_err": np.sqrt(f.ddfvar),
         }
     )
     # check derivative has been sensibly defined
     if (
         np.max(np.abs(f.df)) < 1.0e-20
         and np.max(np.abs(np.diff(f.dfvar))) < 1.0e-20
     ):
@@ -110,33 +110,33 @@
     else:
         adff, andff, aft, anft = np.nan, np.nan, np.nan, np.nan
     # store results
     statsdict = {
         "experiment": e,
         "condition": c,
         "strain": s,
-        "local max " + derivname: np.median(da),
-        "local max " + derivname + " err": statserr(da),
-        "time of local max " + derivname: np.median(dt),
-        "time of local max " + derivname + " err": statserr(dt),
-        "area under " + derivname + " vs " + dtype: np.median(adff),
-        "area under " + derivname + " vs " + dtype + " err": statserr(adff),
-        "normalized area under "
+        "local_max_" + derivname: np.median(da),
+        "local_max_" + derivname + "_err": statserr(da),
+        "time_of_local_max_" + derivname: np.median(dt),
+        "time_of_local_max_" + derivname + "_err": statserr(dt),
+        "area_under_" + derivname + "_vs_" + dtype: np.median(adff),
+        "area_under_" + derivname + "_vs_" + dtype + "_err": statserr(adff),
+        "normalised_area_under_"
         + derivname
-        + " vs "
+        + "_vs_"
         + dtype: np.median(andff),
-        "normalized area under "
+        "normalised_area_under_"
         + derivname
-        + " vs "
+        + "_vs_"
         + dtype
-        + " err": statserr(andff),
-        "area under " + dtype: np.median(aft),
-        "area under " + dtype + " err": statserr(aft),
-        "normalized area under " + dtype: np.median(anft),
-        "normalized area under " + dtype + " err": statserr(anft),
+        + "_err": statserr(andff),
+        "area_under_" + dtype: np.median(aft),
+        "area_under_" + dtype + "_err": statserr(aft),
+        "normalised_area_under_" + dtype: np.median(anft),
+        "normalised_area_under_" + dtype + "_err": statserr(anft),
     }
     return outdf, statsdict, warning
 
 
 def findlocalmaxderiv(
     f, gs, axgr, figs, plotlocalmax, showpeakproperties, **kwargs
 ):
```

### Comparing `omniplate-0.9.6/om_code/sunder.py` & `omniplate-0.9.82/om_code/sunder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # functions for taking subsets of the data
 import numpy as np
-import om_code.omgenutils as gu
+
 import om_code.omerrors as errors
+import om_code.omgenutils as gu
 
 
 def getsubset(
-    inst,
+    self,
     type,
     set="all",
     includes=False,
     excludes=False,
     nonull=False,
     nomedia=False,
 ):
     """
-    Returns a subset of either the conditions or strains.
+    Return a subset of either the conditions or strains.
 
     Parameters
     --
-    inst: instance of platereader
+    self: instance of platereader
     type: string
         Either 'c' (conditions) or 's' (strains).
     set: list of strings
         List of items to include (default is 'all').
     includes: string
         Select only items with this string in their name.
     excludes: string
@@ -38,35 +39,35 @@
     """
     if set == "all" or includes or excludes:
         if type == "c":
             sset = list(
                 np.unique(
                     [
                         con
-                        for e in inst.allconditions
-                        for con in inst.allconditions[e]
+                        for e in self.allconditions
+                        for con in self.allconditions[e]
                     ]
                 )
             )
             if nomedia and "media" in sset:
                 sset.pop(sset.index("media"))
         elif type == "s":
             sset = list(
                 np.unique(
                     [
                         str
-                        for e in inst.allstrains
-                        for str in inst.allstrains[e]
+                        for e in self.allstrains
+                        for str in self.allstrains[e]
                     ]
                 )
             )
             if nonull and "Null" in sset:
                 sset.pop(sset.index("Null"))
         else:
-            sset = inst.allexperiments
+            sset = self.allexperiments
         # find those items containing keywords given in 'includes'
         if includes:
             includes = gu.makelist(includes)
             newset = []
             for s in sset:
                 gotone = 0
                 for item in includes:
@@ -96,148 +97,130 @@
             raise errors.getsubset(
                 "Nothing found for " + " and ".join(includes)
             )
         else:
             raise errors.getsubset("Nothing found")
 
 
-###
-
-
-def getexps(inst, experiments, experimentincludes, experimentexcludes):
-    """
-    Returns list of experiments
-    """
+def getexps(self, experiments, experimentincludes, experimentexcludes):
+    """Return list of experiments."""
     if experimentincludes or experimentexcludes:
         exps = getsubset(
-            inst,
+            self,
             "e",
             includes=experimentincludes,
             excludes=experimentexcludes,
         )
     elif experiments == "all":
-        exps = inst.allexperiments
+        exps = self.allexperiments
     else:
         exps = gu.makelist(experiments)
     return exps
 
 
-###
-
-
-def getcons(inst, conditions, conditionincludes, conditionexcludes, nomedia):
-    """
-    Returns list of conditions
-    """
+def getcons(self, conditions, conditionincludes, conditionexcludes, nomedia):
+    """Return list of conditions."""
     if conditionincludes or conditionexcludes:
         cons = getsubset(
-            inst,
+            self,
             "c",
             includes=conditionincludes,
             excludes=conditionexcludes,
             nomedia=nomedia,
         )
     elif conditions == "all":
         cons = list(
             np.unique(
                 [
                     con
-                    for e in inst.allconditions
-                    for con in inst.allconditions[e]
+                    for e in self.allconditions
+                    for con in self.allconditions[e]
                 ]
             )
         )
         if nomedia and "media" in cons:
             cons.pop(cons.index("media"))
     else:
         cons = gu.makelist(conditions)
     return sorted(cons, key=gu.natural_keys)
 
 
-###
-
-
-def getstrs(inst, strains, strainincludes, strainexcludes, nonull):
-    """
-    Returns list of strains
-    """
+def getstrs(self, strains, strainincludes, strainexcludes, nonull):
+    """Return list of strains."""
     if strainincludes or strainexcludes:
         strs = getsubset(
-            inst,
+            self,
             "s",
             includes=strainincludes,
             excludes=strainexcludes,
             nonull=nonull,
         )
     elif strains == "all":
         strs = list(
             np.unique(
-                [str for e in inst.allstrains for str in inst.allstrains[e]]
+                [str for e in self.allstrains for str in self.allstrains[e]]
             )
         )
         if nonull and "Null" in strs:
             strs.pop(strs.index("Null"))
     else:
         strs = gu.makelist(strains)
     if nonull and "Null" in strs:
         strs.pop(strs.index("Null"))
     return sorted(strs, key=gu.natural_keys)
 
 
-###
-
-
 def getall(
-    inst,
+    self,
     experiments,
     experimentincludes,
     experimentexcludes,
     conditions,
     conditionincludes,
     conditionexcludes,
     strains,
     strainincludes,
     strainexcludes,
     nonull=True,
     nomedia=True,
 ):
-    """
-    Returns experiments, conditions, and strains
-    """
-    exps = getexps(inst, experiments, experimentincludes, experimentexcludes)
+    """Return experiments, conditions, and strains."""
+    exps = getexps(self, experiments, experimentincludes, experimentexcludes)
     cons = getcons(
-        inst, conditions, conditionincludes, conditionexcludes, nomedia
+        self, conditions, conditionincludes, conditionexcludes, nomedia
     )
-    strs = getstrs(inst, strains, strainincludes, strainexcludes, nonull)
+    strs = getstrs(self, strains, strainincludes, strainexcludes, nonull)
     return exps, cons, strs
 
 
-###
-
-
 def extractwells(r_df, s_df, experiment, condition, strain, datatypes):
     """
-    Extracts a list of matrices for each dtype in
-    datatypes for the given experiment, condition, and strain with each
-    column in each matrix having the data for one well
+    Extract a list of data matrices from the r dataframe.
+
+    Each column in each matrix contains the data
+    from one well.
+
+    Data is returned for each dtype in datatypes, which may include "time", for
+    the given experiment, condition, and strain.
     """
     datatypes = gu.makelist(datatypes)
     # restrict time if necessary
     lrdf = r_df[
         (r_df.time >= s_df.time.min()) & (r_df.time <= s_df.time.max())
     ]
     # extract data
     df = lrdf.query(
         "experiment == @experiment and condition == @condition "
         "and strain == @strain"
     )
     matrices = []
     for dtype in datatypes:
         df2 = df[[dtype, "well"]]
-        df2well = df2.groupby("well")[dtype].apply(list)
-        matrices.append(np.transpose([df2well[w] for w in df2well.index]))
+        df2well = df2.groupby("well", group_keys=True)[dtype].apply(list)
+        data = np.transpose([df2well[w] for w in df2well.index])
+        matrices.append(data)
     if len(datatypes) == 1:
         # return array
         return matrices[0]
     else:
         # return list of arrays
         return matrices
```

### Comparing `omniplate-0.9.6/omniplate/Omniplate.py` & `omniplate-0.9.82/omniplate/Omniplate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # !/usr/bin/env python
-import numpy as np
-import matplotlib.pyplot as plt
-import seaborn as sns
-import pandas as pd
-import warnings
+import pprint
 import re
+import warnings
 from pathlib import Path
+
 import gaussianprocessderivatives as gp
-import om_code.omgenutils as gu
-from om_code.omfitderiv import fitderiv
-import om_code.omplot as omplot
+import matplotlib.pyplot as plt
+import numpy as np
+import om_code.admin as admin
+import om_code.clogger as clogger
+import om_code.corrections as corrections
 import om_code.loadplatedata as loadplatedata
 import om_code.omerrors as errors
-import om_code.corrections as corrections
-import om_code.sunder as sunder
+import om_code.omgenutils as gu
+import om_code.omplot as omplot
 import om_code.omstats as omstats
-import om_code.admin as admin
-import om_code.clogger as clogger
+import om_code.sunder as sunder
+import om_code.midlog as midlog
+import pandas as pd
+import seaborn as sns
+from om_code.omfitderiv import fitderiv
 
-version = "0.9.6"
+version = "0.9.82"
 
 plt.rcParams["figure.max_open_warning"] = 0
 sns.set()
 
 
 class platereader:
     """
@@ -94,15 +97,14 @@
 
     >>> p.webhelp()
     """
 
     # ratio of fluorescence emission at 585nm to emiisions at 525nm for eGFP
     _gamma = 0.114
 
-    ###
     def __init__(
         self,
         dnames=False,
         anames=False,
         wdir=".",
         platereadertype="Tecan",
         dsheetnumbers=False,
@@ -136,15 +138,14 @@
         info: boolean
             If True (default), display summary information on the data once
             loaded.
         ls: boolean
             If True (default), display contents of working directory.
         """
         self.__version__ = version
-        print("\nomniplate version=", self.__version__)
         # absolute path
         self.wdirpath = Path(wdir)
 
         # enable logging
         self.logger, self.logstream = clogger.initlog(version)
 
         if True:
@@ -157,14 +158,15 @@
             "ignoredwells": {},
             "negativevalues": {},
         }
         self.allexperiments = []
         self.allconditions = {}
         self.allstrains = {}
         self.datatypes = {}
+        self._find_available_data
 
         if dnames is False:
             # list all files in current directory
             if ls:
                 self.ls
         else:
             # immediately load data
@@ -173,56 +175,75 @@
                 anames,
                 platereadertype,
                 dsheetnumbers,
                 asheetnumbers,
                 info,
             )
 
-    ###
-
     def __repr__(self):
-        """Represent as a string."""
-        repstr = "{} v{}: ".format(self.__class__.__name__, self.__version__)
-        for e in self.allexperiments:
-            repstr += e + " ; "
-        if repstr[-2:] == "; ":
-            repstr = repstr[:-3]
+        """Standard representation."""
+        repstr = f"omniplate.{self.__class__.__name__}: "
+        if self.allexperiments:
+            for e in self.allexperiments:
+                repstr += e + " ; "
+            if repstr[-2:] == "; ":
+                repstr = repstr[:-3]
+        else:
+            repstr += "no experiments"
         return repstr
 
-    ###
     @property
-    def ls(self):
-        """
-        List all files in the working directory.
-
-        A dictionary of available datasets is created as a shortcut.
-
-        Example
-        -------
-        >>> p.ls
-        >>> p.files
-        >>> p.load(p.files[0], p.files[1])
-        """
-        print("Working directory is", str(self.wdirpath.resolve()))
-        print("Files available are:", "\n---")
+    def _find_available_data(self):
+        """Create files and data sets as attributes."""
         files = []
+        datasets = []
         for f in self.wdirpath.glob("*.*"):
             if f.is_file() and (
                 f.suffix == ".xlsx"
                 or f.suffix == ".json"
                 or f.suffix == ".tsv"
                 or f.suffix == ".csv"
                 or f.suffix == ".xls"
             ):
-                print(f.stem + f.suffix)
                 files.append(f.stem + f.suffix)
-        print()
+                if (
+                    f.suffix == ".tsv"
+                    or f.suffix == ".json"
+                    or f.suffix == ".csv"
+                ):
+                    froot = "_".join(f.stem.split("_")[:-1])
+                    if froot not in datasets:
+                        datasets.append(froot)
         self.files = {i: f for i, f in enumerate(sorted(files))}
+        self.datasets = sorted(datasets)
+
+    @property
+    def ls(self):
+        """
+        List all files in the working directory.
+
+        A dictionary of available files to load and a list of available
+        data sets to import are created as a shortcuts.
+
+        Parameter
+        --------
+        output: boolean
+            If True, list available files.
 
-    ###
+        Examples
+        --------
+        >>> p.ls
+        >>> p.files
+        >>> p.load(p.files[0], p.files[1])
+        >>> p.importdf(p.datasets)
+        """
+        print(f"Working directory is {str(self.wdirpath.resolve())}.")
+        print("Files available are:", "\n---")
+        pprint.pprint(self.files)
+        print()
 
     def changewdir(self, wdir):
         """
         Change working directory.
 
         Parameters
         ----------
@@ -232,16 +253,14 @@
         Example
         -------
         >>> p.changewdir('newdata/')
         """
         self.wdirpath = Path(wdir)
         self.ls
 
-    ###
-
     @clogger.log
     def load(
         self,
         dnames,
         anames=False,
         platereadertype="Tecan",
         dsheetnumbers=False,
@@ -277,15 +296,17 @@
         Examples
         -------
         >>> p.load('Data.xlsx', 'DataContents.xlsx')
         >>> p.load('Data.xlsx', 'DataContents.xlsx', info= False)
         """
         dnames = gu.makelist(dnames)
         if not anames:
-            anames = [dname.split(".")[0] + "Contents.xlsx" for dname in dnames]
+            anames = [
+                dname.split(".")[0] + "Contents.xlsx" for dname in dnames
+            ]
         else:
             anames = gu.makelist(anames)
         if not dsheetnumbers:
             dsheetnumbers = [0 for dname in dnames]
         if not asheetnumbers:
             asheetnumbers = [0 for dname in dnames]
 
@@ -308,15 +329,19 @@
                 asheetnumbers[i],
             )
             self.allexperiments.append(experiment)
             self.allconditions[experiment] = allconditionssingle
             self.allstrains[experiment] = allstrainssingle
             self.datatypes[experiment] = datatypes
             alldata.update(alldatasingle)
-            self.r = pd.merge(self.r, rdf, how="outer") if hasattr(self, "r") else rdf
+            self.r = (
+                pd.merge(self.r, rdf, how="outer")
+                if hasattr(self, "r")
+                else rdf
+            )
             # update progress dictionary
             admin.initialiseprogress(self, experiment)
 
         # dataframe for summary stats and corrections
         alldfs = []
         # for exp in self.allexperiments:
         for exp in alldata:
@@ -324,22 +349,25 @@
             for cs in alldata[exp]:
                 strs.append(cs.split(" in ")[0])
                 cons.append(cs.split(" in ")[1])
             corrdict = {
                 "experiment": exp,
                 "strain": strs,
                 "condition": cons,
-                "OD corrected": False,
+                "OD_corrected": False,
             }
             corrdict.update(
-                {dtype + " corrected for media": False for dtype in self.datatypes[exp]}
+                {
+                    dtype + "_corrected_for_media": False
+                    for dtype in self.datatypes[exp]
+                }
             )
             corrdict.update(
                 {
-                    dtype + " corrected for autofluorescence": False
+                    dtype + "_corrected_for_autofluorescence": False
                     for dtype in self.datatypes[exp]
                     if dtype not in ["AutoFL", "OD"]
                 }
             )
             alldfs.append(pd.DataFrame(corrdict))
         self.sc = pd.concat(alldfs)
 
@@ -354,21 +382,18 @@
         if info:
             self.info
         print(
             '\nWarning: wells with no strains have been changed to "Null"'
             "\nto avoid confusion with pandas.\n"
         )
 
-    ###
-    # Routines to display information on data and state of data processing
-    ###
     @property
     def info(self):
         """
-        Display conditions, strains, and datatypes.
+        Display conditions, strains, and data types.
 
         Example
         -------
         >>> p.info
         """
         for exp in self.allexperiments:
             print("\nExperiment:", exp, "\n---")
@@ -386,16 +411,14 @@
                 if self.progress["ignoredwells"][exp]:
                     for d in self.progress["ignoredwells"][exp]:
                         print("\t", d)
                 else:
                     print("\t", "None")
         print()
 
-    ###
-
     def webhelp(self, browser=None):
         """
         Open detailed examples of how to use in omniplate in a web browser.
 
         Parameters
         ----------
         browser: string, optional
@@ -407,15 +430,14 @@
         >>> p.webhelp()
         """
         import webbrowser
 
         url = "https://swainlab.bio.ed.ac.uk/software/omniplate/index.html"
         webbrowser.get(browser).open_new(url)
 
-    ###
     @property
     def attributes(self):
         """
         Print the attributes of the current instance.
 
         Example
         -------
@@ -430,19 +452,21 @@
             "ODfname",
             "overflow",
             "nooutchannels",
             "nodata",
             "__doc__",
         ]
         for a in self.__dict__:
-            if "corrected" not in a and "processed" not in a and a not in ignore:
+            if (
+                "corrected" not in a
+                and "processed" not in a
+                and a not in ignore
+            ):
                 print(a)
 
-    ###
-
     @clogger.log
     def rename(self, translatedict, regex=True, **kwargs):
         """
         Rename strains or conditions.
 
         Uses a dictionary to replace all occurrences of a strain or a condition
         with an alternative.
@@ -458,26 +482,50 @@
         kwargs: keyword arguments
             Passed to panda's replace.
 
         Example
         -------
         >>> p.rename({'77.WT' : 'WT', '409.Hxt4' : 'Hxt4'})
         """
-        # replace in dataframes
-        for df in [self.r, self.s, self.sc]:
-            df.replace(translatedict, inplace=True, regex=regex, **kwargs)
+        # check for duplicates
+        if (
+            len(translatedict.values())
+            != np.unique(list(translatedict.values())).size
+        ):
+            print("Warning: new names are not unique.")
+            print("Any processed data may be corrupted.\n")
+            # replace in dataframes
+            for df in [self.r, self.sc]:
+                exps = df.experiment.copy()
+                df.replace(translatedict, inplace=True, regex=regex, **kwargs)
+                # do not change names of experiments
+                df["experiment"] = exps
+            # remake s so that strains with the same name are combined
+            self.s = admin.make_s(self)
+        else:
+            # replace in dataframes
+            for df in [self.r, self.s, self.sc]:
+                exps = df.experiment.copy()
+                df.replace(translatedict, inplace=True, regex=regex, **kwargs)
+                df["experiment"] = exps
+        self.wellsdf = admin.makewellsdf(self.r)
         # replace in attributes - allstrains and allconditions
         for e in self.allexperiments:
             for listattr in [self.allconditions[e], self.allstrains[e]]:
                 for i, listitem in enumerate(listattr):
                     for key in translatedict:
                         if key in listitem:
-                            listattr[i] = listitem.replace(key, translatedict[key])
-
-    ###
+                            listattr[i] = listitem.replace(
+                                key, translatedict[key]
+                            )
+            # unique values in case two strains have been renamed to one
+            self.allconditions[e] = sorted(
+                list(np.unique(self.allconditions[e]))
+            )
+            self.allstrains[e] = sorted(list(np.unique(self.allstrains[e])))
 
     def corrections(
         self,
         experiments="all",
         conditions="all",
         strains="all",
         experimentincludes=False,
@@ -545,16 +593,14 @@
         df = df[
             ["experiment", "strain", "condition"]
             + [col for col in df.columns if "correct" in col]
         ]
         df = df.T
         return df
 
-    ###
-
     @clogger.log
     def addcolumn(self, newcolumnname, oldcolumn, newcolumnvalues):
         """
         Add a new column to all dataframes by parsing an existing column.
 
         All possible entries for the new column are specified as strings and
         the entry in the new column will be whichever of these strings is
@@ -576,23 +622,23 @@
 
         will parse each entry in 'condition' to create a new column called
         'medium' that has either a value 'Raffinose' if 'Raffinose' is in the
         entry from 'condition' or a value 'Geneticin' if 'Geneticin' is in the
         entry from 'condition'.
         """
         for df in [self.r, self.s, self.sc]:
-            newcol = np.array(("",) * len(df[oldcolumn].to_numpy()), dtype="object")
+            newcol = np.array(
+                ("",) * len(df[oldcolumn].to_numpy()), dtype="object"
+            )
             for i, oldcolvalue in enumerate(df[oldcolumn].to_numpy()):
                 for newcolvalue in newcolumnvalues:
                     if newcolvalue in oldcolvalue:
                         newcol[i] = newcolvalue
             df[newcolumnname] = newcol
 
-    ###
-
     @clogger.log
     def addnumericcolumn(
         self,
         newcolumnname,
         oldcolumn,
         picknumber=0,
         leftsplitstr=None,
@@ -648,18 +694,22 @@
             locno = -1 if leftsplitstr else 1
         else:
             splitstr = False
         # change each dataframe
         for df in [self.r, self.s, self.sc]:
             if asstr:
                 # new column of strings
-                newcol = np.full_like(df[oldcolumn].to_numpy(), "", dtype="object")
+                newcol = np.full_like(
+                    df[oldcolumn].to_numpy(), "", dtype="object"
+                )
             else:
                 # new column of floats
-                newcol = np.full_like(df[oldcolumn].to_numpy(), np.nan, dtype="float")
+                newcol = np.full_like(
+                    df[oldcolumn].to_numpy(), np.nan, dtype="float"
+                )
             # parse old column
             for i, oldcolvalue in enumerate(df[oldcolumn].to_numpy()):
                 if oldcolvalue:
                     # split string first on spaces and then find substring
                     # adjacent to specified splitstring
                     if splitstr:
                         if splitstr in oldcolvalue:
@@ -687,16 +737,14 @@
                                 newcol[i] = ci if asstr else no
                                 break
                             nocount += 1
                         except ValueError:
                             pass
             df[newcolumnname] = newcol
 
-    ###
-
     @clogger.log
     def add_to_sc(
         self,
         newcolumn=None,
         s_column=None,
         func=None,
         experiments="all",
@@ -722,17 +770,17 @@
             The name of the column in s dataframe from which the
             data is to be processed
         func:   function
             The function to be applied to the data in the s dataframe.
 
         Examples
         --------
-        >>> p.add_to_sc(newcolumn= "max GFP", s_column= "GFP mean",
+        >>> p.add_to_sc(newcolumn= "max_GFP", s_column= "GFP_mean",
         ...             func= np.nanmax)
-        >>> p.add_to_sc(newcolumn= "GFP lower quartile", s_column= "GFP mean",
+        >>> p.add_to_sc(newcolumn= "GFP_lower_quartile", s_column= "GFP_mean",
         ...             func= lambda x: np.nanquantile(x, 0.25))
         """
         # extract data
         exps, cons, strs = sunder.getall(
             self,
             experiments,
             experimentincludes,
@@ -756,19 +804,17 @@
                         self.sc.loc[
                             (self.sc.experiment == e)
                             & (self.sc.condition == c)
                             & (self.sc.strain == s),
                             newcolumn,
                         ] = func(d)
                     else:
-                        print("func must return a single value")
+                        print("func must return a single value.")
                         return False
 
-    ###
-
     @clogger.log
     def addcommonvar(
         self,
         var="time",
         dvar=None,
         varmin=None,
         varmax=None,
@@ -869,23 +915,25 @@
             conditionincludes,
             conditionexcludes,
             strains,
             strainincludes,
             strainexcludes,
             nonull=True,
         )
-        print("Finding common" + var)
+        print(f"Finding common {var}.")
         for df in [self.r, self.s]:
             if var in df:
                 loc = (
                     df.experiment.isin(exps)
                     & df.condition.isin(cons)
                     & df.strain.isin(strs)
                 )
-                print("r dataframe") if df.equals(self.r) else print("s dataframe")
+                print("r dataframe") if df.equals(self.r) else print(
+                    "s dataframe"
+                )
                 if dvar is None:
                     # calculated for tidy printing
                     elen = np.max([len(e) for e in exps]) + 5
                     # find median increment in var
                     for e in exps:
                         evar = df[loc][var].to_numpy()
                         print(
@@ -897,49 +945,46 @@
                                 var,
                                 np.median(np.diff(evar)),
                             )
                         )
                     ldvar = np.median(np.diff(df[loc][var].to_numpy()))
                 else:
                     ldvar = dvar
-                print(" Using d{}= {:.2e}".format(var, ldvar))
+                print(f" Using d{var}= {ldvar:.2e}")
                 lvarmin = df[loc][var].min() if varmin is None else varmin
-                print(" Using {}_min= {:.2e}\n".format(var, lvarmin))
+                print(f" Using {var}_min= {lvarmin:.2e}\n")
                 lvarmax = df[loc][var].max() if varmax is None else varmax
                 # define common var
                 cvar = np.arange(lvarmin, lvarmax, ldvar)
                 df.loc[loc, "common" + var] = df[loc][var].apply(
                     lambda x: cvar[np.argmin((x - cvar) ** 2)]
                 )
                 if figs:
                     plt.figure()
-                    sl = np.linspace(df[loc][var].min(), 1.05 * df[loc][var].max(), 100)
+                    sl = np.linspace(
+                        df[loc][var].min(), 1.05 * df[loc][var].max(), 100
+                    )
                     plt.plot(sl, sl, alpha=0.4)
                     plt.plot(
                         df[loc][var].to_numpy(),
                         df[loc]["common" + var].to_numpy(),
                         ".",
                     )
                     plt.xlabel(var)
                     plt.ylabel("common" + var)
-                    title = "r dataframe" if df.equals(self.r) else "s dataframe"
+                    title = (
+                        "r dataframe" if df.equals(self.r) else "s dataframe"
+                    )
                     plt.title(title)
                     plt.suptitle(
-                        "comparing "
-                        + var
-                        + " with common"
-                        + var
-                        + " – the line y= x is expected"
+                        f"comparing {var} with common {var} – "
+                        "the line y= x is expected."
                     )
                     plt.tight_layout()
-                    plt.show()
-
-    ###
-    # Routines to examine and ignore individual wells
-    ###
+                    plt.show(block=False)
 
     def contentsofwells(self, wlist):
         """
         Display contents of wells.
 
         Parameters
         ----------
@@ -955,16 +1000,14 @@
             print("\n" + w + "\n--")
             print(
                 self.wellsdf.query("well == @w")
                 .drop(["well"], axis=1)
                 .to_string(index=False)
             )
 
-    ###
-
     def showwells(
         self,
         concise=False,
         sortby=False,
         experiments="all",
         conditions="all",
         strains="all",
@@ -1041,16 +1084,14 @@
                     .query("experiment == @e")
                     .to_string(index=False)
                 )
             else:
                 print(df.query("experiment == @e").to_string(index=False))
             print()
 
-    ###
-
     @clogger.log
     def ignorewells(
         self,
         exclude=[],
         experiments="all",
         experimentincludes=False,
         experimentexcludes=False,
@@ -1080,15 +1121,17 @@
         Example
         -------
         >>> p.ignorewells(['A1', 'C2'])
         """
         if clearall:
             # forget any previously ignoredwells
             self.r = self.origr.copy()
-            self.progress["ignoredwells"] = {exp: [] for exp in self.allexperiments}
+            self.progress["ignoredwells"] = {
+                exp: [] for exp in self.allexperiments
+            }
             admin.update_s(self)
             print(
                 "Warning: all corrections and analysis to raw data have been"
                 " lost. No wells have been ignored."
             )
         else:
             if gu.islistempty(exclude):
@@ -1114,43 +1157,47 @@
                         "Either a list of wells to exclude for a particular\n"
                         "experiment or a list of experiments must be given."
                     )
                 else:
                     # drop wells
                     for ex, exp in zip(exclude, exps):
                         # wells cannot be ignored twice
-                        wex = list(set(ex) - set(self.progress["ignoredwells"][exp]))
+                        wex = list(
+                            set(ex) - set(self.progress["ignoredwells"][exp])
+                        )
                         # drop data from ignored wells
                         df = self.r
                         filt = (df["experiment"] == exp) & df["well"].isin(wex)
                         df = df.loc[~filt]
                         df = df.reset_index(drop=True)
                         self.r = df
                         # store ignoredwells
                         self.progress["ignoredwells"][exp] += ex
                         # remove any duplicates
                         self.progress["ignoredwells"][exp] = list(
                             set(self.progress["ignoredwells"][exp])
                         )
                     anycorrections = np.count_nonzero(
                         self.sc[
-                            [col for col in self.sc.columns if "correct" in col]
+                            [
+                                col
+                                for col in self.sc.columns
+                                if "correct" in col
+                            ]
                         ].values
                     )
                     if np.any(anycorrections):
                         print(
                             "Warning: you have ignored wells after correcting\n"
                             "the data. It is best to ignorewells first, before\n"
                             "running any analysis."
                         )
                 # remake summary data
                 admin.update_s(self)
 
-    ###
-
     @clogger.log
     def restricttime(self, tmin=None, tmax=None):
         """
         Restrict the processed data to a range of time.
 
         Points outside this time range are ignored.
 
@@ -1171,19 +1218,16 @@
         if tmin is None:
             tmin = self.r.time.min()
         if tmax is None:
             tmax = self.r.time.max()
         if tmax > tmin:
             self.s = self.s[(self.s.time >= tmin) & (self.s.time <= tmax)]
         else:
-            print("tmax or tmin is not properly defined")
+            print("tmax or tmin is not properly defined.")
 
-    ###
-    # Routines for plotting
-    ###
     @clogger.log
     def plot(
         self,
         x="time",
         y="OD",
         hue="strain",
         style="condition",
@@ -1405,16 +1449,14 @@
                 title,
                 sortby,
                 **kwargs,
             )
         else:
             raise errors.PlotError("No data found")
 
-    ###
-
     def savefigs(self, fname=None, onefile=True):
         """
         Save all current figures to PDF.
 
         Either all figures save to one file or each to a separate one.
 
         Parameters
@@ -1430,41 +1472,42 @@
         >>> p.savefigs('figures.pdf')
         """
         if fname:
             if ".pdf" not in fname:
                 fname += ".pdf"
             fname = str(self.wdirpath / fname)
         else:
-            fname = str(self.wdirpath / ("".join(self.allexperiments) + ".pdf"))
+            fname = str(
+                self.wdirpath / ("".join(self.allexperiments) + ".pdf")
+            )
         if onefile:
             gu.figs2pdf(fname)
         else:
             for i in plt.get_fignums():
                 plt.figure(i)
-                savename = str(plt.getp(plt.gcf(), "axes")[0].title).split("'")[1]
+                savename = str(plt.getp(plt.gcf(), "axes")[0].title).split(
+                    "'"
+                )[1]
                 savename = savename.replace(" ", "_")
                 if savename == "":
                     savename = "Whole_plate_Figure_" + str(i)
                 print("Saving", savename)
                 plt.savefig(str(self.wdirpath / (savename + ".pdf")))
 
-    ###
     @property
     def close(self):
         """
         Close all figures.
 
         Example
         -------
         >>> p.close
         """
         plt.close("all")
 
-    ###
-
     @clogger.log
     def getdataframe(
         self,
         dfname="s",
         experiments="all",
         conditions="all",
         strains="all",
@@ -1533,58 +1576,54 @@
             strainincludes,
             strainexcludes,
             nonull,
         )
         if hasattr(self, dfname):
             df = getattr(self, dfname)
             ndf = df.query(
-                "experiment == @exps and condition == @cons " "and strain == @strs"
+                "experiment == @exps and condition == @cons "
+                "and strain == @strs"
             )
             if ndf.empty:
-                print("No data found")
+                print("No data found.")
             else:
                 return ndf.copy()
         else:
-            raise errors.UnknownDataFrame("Dataframe " + dfname + " is not recognised")
+            raise errors.UnknownDataFrame(
+                "Dataframe " + dfname + " is not recognised."
+            )
 
-    ###
-    # OD correction
-    ###
     @clogger.log
     def correctOD(
         self,
         figs=True,
-        odmatch=0.3,
         bd=None,
         gp_results=False,
         ODfname=None,
         experiments="all",
         experimentincludes=False,
         experimentexcludes=False,
         conditions="all",
         conditionincludes=False,
         conditionexcludes=False,
     ):
         """
         Correct for the non-linear relationship between OD and cell number.
 
         Requires a set of dilution data set, with the default being haploid
-        yeast growing in glucose (collected by L Bandiera).
+        yeast growing in glucose.
+
         An alternative can be loaded from a file - a txt file of two columns
         with OD specified in the first column and the dilution factor specified
         in descending order in the second.
 
         Parameters
         ---------
         figs: boolean, optional
             If True, a plot of the fit to the dilution data is produced.
-        odmatch: float, optional
-            If not None, then the corrected OD is rescaled to equal the
-            measured OD at this value. Only large ODs typically need to be
-            corrected.
         bd: dictionary, optional
             Specifies the limits on the hyperparameters for the Gaussian
             process.
             For example, bd= {0: [-1, 4], 2: [2, 6]})
             sets confines the first hyperparameter to be between 1e-1 and 1e^4
             and confines the third hyperparmater between 1e2 and 1e6.
         gp_results: boolean, optional
@@ -1610,64 +1649,61 @@
             Ignores conditions that include the specified string in their name.
 
         Examples
         -------
         >>> p.correctOD()
         >>> p.correctOD(figs= False)
         """
-        exps = sunder.getexps(self, experiments, experimentincludes, experimentexcludes)
+        exps = sunder.getexps(
+            self, experiments, experimentincludes, experimentexcludes
+        )
         cons = sunder.getcons(
             self,
             conditions,
             conditionincludes,
             conditionexcludes,
             nomedia=False,
         )
         # fit dilution data
-        gc = corrections.findODcorrection(
+        gc, odmatch = corrections.findODcorrection(
             self.wdirpath,
             ODfname,
             figs=figs,
-            odmatch=odmatch,
             bd=bd,
             gp_results=gp_results,
         )
         # correct ODs
         for exp in exps:
             for c in cons:
-                if self.sc[(self.sc.experiment == exp) & (self.sc.condition == c)][
-                    "OD corrected"
-                ].any():
-                    print(exp, ": OD is already corrected for", c)
+                if self.sc[
+                    (self.sc.experiment == exp) & (self.sc.condition == c)
+                ]["OD_corrected"].any():
+                    print(f"{exp}: OD is already corrected for {c}.")
                 else:
                     # correct all wells
-                    r_data = self.r.query("experiment == @exp and condition == @c")[
-                        "OD"
-                    ].to_numpy()
+                    r_data = self.r.query(
+                        "experiment == @exp and condition == @c"
+                    )["OD"].to_numpy()
                     gc.batchpredict(r_data)
                     # leave small ODs unchanged
                     new_r = gc.f
-                    if odmatch is not None:
-                        new_r[r_data < odmatch] = r_data[r_data < odmatch]
+                    new_r[r_data < odmatch] = r_data[r_data < odmatch]
                     # update r data frame
                     self.r.loc[
                         (self.r.experiment == exp) & (self.r.condition == c),
                         "OD",
                     ] = new_r
                     # flag corrections in summary stats dataframe
                     self.sc.loc[
                         (self.sc.experiment == exp) & (self.sc.condition == c),
-                        "OD corrected",
+                        "OD_corrected",
                     ] = True
         # update s dataframe
         admin.update_s(self)
 
-    ###
-    # Media correction
-    ###
     @clogger.log
     def correctmedia(
         self,
         datatypes="all",
         commonmedia=False,
         experiments="all",
         experimentincludes=False,
@@ -1717,69 +1753,75 @@
 
         Examples
         --------
         >>> p.correctmedia()
         >>> p.correctmedia('OD')
         >>> p.correctmedia(commonmedia= '1% Glu')
         """
-        exps = sunder.getexps(self, experiments, experimentincludes, experimentexcludes)
+        exps = sunder.getexps(
+            self, experiments, experimentincludes, experimentexcludes
+        )
         cons = sunder.getcons(
             self,
             conditions,
             conditionincludes,
             conditionexcludes,
             nomedia=False,
         )
         for exp in exps:
             # data types
             expdatatypes = (
-                self.datatypes[exp] if datatypes == "all" else gu.makelist(datatypes)
+                self.datatypes[exp]
+                if datatypes == "all"
+                else gu.makelist(datatypes)
             )
             # correct for media
             for dtype in expdatatypes:
                 for c in cons:
-                    if self.sc[(self.sc.experiment == exp) & (self.sc.condition == c)][
-                        dtype + " corrected for media"
-                    ].any():
+                    if self.sc[
+                        (self.sc.experiment == exp) & (self.sc.condition == c)
+                    ][dtype + "_corrected_for_media"].any():
                         print(
-                            exp + ":",
-                            dtype,
-                            "is already corrected for media in",
-                            c,
+                            f"{exp}: {dtype} is already corrected for media"
+                            " in {c}."
                         )
                     else:
-                        print(exp + ": Correcting", dtype, "for media in", c)
+                        print(f"{exp}: Correcting {dtype} for media in {c}.")
                         cm = commonmedia if commonmedia else c
                         # update r dataframe
-                        (success, negvalues,) = corrections.performmediacorrection(
+                        (
+                            success,
+                            negvalues,
+                        ) = corrections.performmediacorrection(
                             self.r, dtype, exp, c, figs, cm, frac
                         )
                         if success:
                             self.sc.loc[
-                                (self.sc.experiment == exp) & (self.sc.condition == c),
-                                dtype + " corrected for media",
+                                (self.sc.experiment == exp)
+                                & (self.sc.condition == c),
+                                dtype + "_corrected_for_media",
                             ] = True
                             if negvalues:
                                 if not self.progress["negativevalues"][exp]:
-                                    self.progress["negativevalues"][exp] = negvalues
+                                    self.progress["negativevalues"][
+                                        exp
+                                    ] = negvalues
                                 else:
-                                    self.progress["negativevalues"][exp] += negvalues
+                                    self.progress["negativevalues"][
+                                        exp
+                                    ] += negvalues
             if self.progress["negativevalues"][exp]:
                 print(
-                    "\nWarning: correcting media has created negative " "values in",
-                    exp,
-                    "for",
+                    "\nWarning: correcting media has created negative "
+                    f"values in {exp} for"
                 )
                 print(self.progress["negativevalues"][exp])
         # update s dataframe
         admin.update_s(self)
 
-    ###
-    # Statistical analysis
-    ###
     @clogger.log
     def getstats(
         self,
         dtype="OD",
         bd=False,
         cvfn="matern",
         empirical_errors=False,
@@ -1917,26 +1959,26 @@
         growth rates using Gaussian processes. Nat Commun, 7, 1-8.
         """
         linalgmax = 5
         warnings = ""
         if dtype == "OD" and logs:
             derivname = "gr"
         else:
-            derivname = "d/dt " + dtype
+            derivname = "d/dt_" + dtype
         snames = [
-            "max " + derivname,
-            "time of max " + derivname,
+            "max_" + derivname,
+            "time_of_max_" + derivname,
         ]
         if dtype == "OD" and logs:
             # special names with estimating specific growth rate
-            snames += ["doubling time", "lag time"]
+            snames += ["doubling_time", "lag_time"]
         else:
             snames += [
-                "doubling time from " + derivname,
-                "lag time from " + derivname,
+                "doubling_time_from-" + derivname,
+                "lag_time_from_" + derivname,
             ]
         if logs:
             ylabels = ["log(" + dtype + ")", derivname]
         else:
             ylabels = [dtype, derivname]
         # extract data
         exps, cons, strs = sunder.getall(
@@ -1956,42 +1998,50 @@
             for c in cons:
                 for s in strs:
                     figtitle = e + ": " + s + " in " + c
                     if dtype in self.r.columns:
                         # raw data
                         d = sunder.extractwells(self.r, self.s, e, c, s, dtype)
                         t = self.s.query(
-                            "experiment == @e and condition == @c and " "strain == @s"
+                            "experiment == @e and condition == @c and "
+                            "strain == @s"
                         )["time"].to_numpy()
                     elif dtype in self.s.columns:
                         # processed data
                         df = self.s.query(
-                            "experiment == @e and condition == @c and " "strain == @s"
+                            "experiment == @e and condition == @c and "
+                            "strain == @s"
                         )
                         # add columns plus and minus err
-                        df = omplot.augmentdf(df, dtype)[[dtype, "augtype", "time"]]
-                        piv_df = df.pivot(index="time", columns="augtype", values=dtype)
+                        df = omplot.augmentdf(df, dtype)[
+                            [dtype, "augtype", "time"]
+                        ]
+                        piv_df = df.pivot(
+                            index="time", columns="augtype", values=dtype
+                        )
                         # convert to array for fitderiv
                         d = piv_df.values
                         t = piv_df.index.to_numpy()
                         numberofnans = np.count_nonzero(np.isnan(d))
                         if np.any(numberofnans):
                             print(f"\nWarning: {numberofnans} NaNs in data")
                     else:
-                        print(dtype, "not recognised for", figtitle)
+                        print(f"\n-> {dtype} not recognised for {figtitle}.\n")
                         return
                     # checks
                     if d.size == 0:
                         # no data
-                        print("No data found for", dtype, "for", figtitle)
-                        break
+                        print(
+                            f"\n-> No data found for {dtype} for {figtitle}.\m"
+                        )
+                        continue
                     if logs:
-                        print("\nFitting log(" + dtype + ") for", figtitle)
+                        print(f"\nFitting log({dtype}) for {figtitle}.")
                     else:
-                        print("\nFitting", dtype, "for", figtitle)
+                        print(f"\nFitting {dtype} for {figtitle}.")
                     # call fitderiv
                     f = fitderiv(
                         t,
                         d,
                         cvfn=cvfn,
                         logs=logs,
                         bd=bd,
@@ -2004,18 +2054,22 @@
                         nosamples=nosamples,
                         iskip=iskip,
                     )
                     if f.success:
                         if figs:
                             plt.figure()
                             plt.subplot(2, 1, 1)
-                            f.plotfit("f", ylabel=ylabels[0], figtitle=figtitle)
+                            f.plotfit(
+                                "f", ylabel=ylabels[0], figtitle=figtitle
+                            )
                             axgr = plt.subplot(2, 1, 2)
                             f.plotfit("df", ylabel=ylabels[1])
                             plt.tight_layout()
+                        else:
+                            axgr = None
                         # find summary statistics
                         outdf, statsdict, warning = omstats.findsummarystats(
                             dtype,
                             derivname,
                             logs,
                             nosamples,
                             f,
@@ -2028,62 +2082,48 @@
                             plotlocalmax,
                             axgr,
                             showpeakproperties,
                             **kwargs,
                         )
                         if warning:
                             warnings += warning
-                        # store results in instance's dataframes
-                        statsdict["logmaxlikehood for " + derivname] = f.logmaxlike
-                        statsdict["gp for " + derivname] = cvfn
+                        # store results in the dataframes
+                        statsdict[
+                            "logmaxlikehood_for_" + derivname
+                        ] = f.logmaxlike
+                        statsdict["gp_for_" + derivname] = cvfn
+                        for j, val in enumerate(f.lth):
+                            statsdict[
+                                "log_hyperparameter_"
+                                + str(j)
+                                + "_for_"
+                                + derivname
+                            ] = val
+                        # add time series to s dataframe
+                        admin.add_to_s(self, derivname, outdf)
                         if stats:
                             for sname in f.ds.keys():
                                 statsdict[sname] = f.ds[sname]
-                        # add growth rates, etc., to dataframe of summary data
-                        if derivname not in self.s.columns:
-                            # add new columns to dataframe
-                            self.s = pd.merge(self.s, outdf, how="outer")
-                        else:
-                            # update dataframe
-                            self.s = gu.absorbdf(
-                                self.s,
-                                outdf,
-                                ["experiment", "condition", "strain", "time"],
-                            )
-                        # create or add summary stats to stats dataframe
-                        statsdf = pd.DataFrame(statsdict, index=pd.RangeIndex(0, 1, 1))
-                        newstats = np.count_nonzero(
-                            [
-                                True if stat not in self.sc.columns else False
-                                for stat in statsdict
-                            ]
+                        # create or add summary stats to sc dataframe
+                        statsdf = pd.DataFrame(
+                            statsdict, index=pd.RangeIndex(0, 1, 1)
                         )
-                        if newstats:
-                            # add new columns to dataframe
-                            self.sc = pd.merge(self.sc, statsdf, how="outer")
-                        else:
-                            # update dataframe
-                            self.sc = gu.absorbdf(
-                                self.sc,
-                                statsdf,
-                                ["experiment", "condition", "strain"],
-                            )
+                        admin.add_to_sc(self, statsdf)
                         if figs:
-                            plt.show()
+                            plt.show(block=False)
         omstats.cleansc(self)
         if warnings:
             print(warnings)
 
-    ###
     @clogger.log
     def averageoverexpts(
         self,
         condition,
         strain,
-        tvr="OD mean",
+        tvr="OD_mean",
         bd=False,
         addnoise=True,
         plot=False,
     ):
         """
         Average a time-dependent variable over all experiments.
 
@@ -2095,15 +2135,15 @@
         ----------
         condition: string
             The condition of interest.
         strain: string
             The strain of interest.
         tvr: float
             The time-dependent variable to be averaged.
-            For example, 'c-GFPperOD' or 'OD mean'.
+            For example, 'c-GFPperOD' or 'OD_mean'.
         bd: dictionary, optional
             The limits on the hyperparameters for the Matern Gaussian process.
             For example, {0: (-5,5), 1: (-4,4), 2: (-5,2)}
             where the first element controls amplitude, setting the bounds to
             1e-5 and 1e5, the second controls flexibility, and the third
             determines the magnitude of the measurement error.
         addnoise: boolean
@@ -2135,74 +2175,87 @@
         ndf = df.query("condition == @condition and strain == @strain")
         # use GP to average over experiments
         x = ndf["time"].to_numpy()
         y = ndf[tvr].to_numpy()
         ys = y[np.argsort(x)]
         xs = np.sort(x)
         g = gp.maternGP(bds, xs, ys)
-        print("averaging over", tvr, "experiments for", strain, "in", condition)
+        print(f"Averaging over {tvr} experiments for {strain} in {condition}.")
         g.findhyperparameters(noruns=2, noinits=1000)
         g.results()
         g.predict(xs, addnoise=addnoise)
         if plot:
             plt.figure()
             g.sketch(".")
             plt.title("averaging " + strain + " in " + condition)
             plt.xlabel("time")
             plt.ylabel(tvr)
-            plt.show()
+            plt.show(block=False)
         # return results as a dictionary
         res = {"t": xs, tvr: ys, "mn": g.f, "sd": np.sqrt(g.fvar)}
         return res
 
-    ###
-    # Fluorescence corrections
-    ###
     @clogger.log
     def correctauto(
         self,
         f=["GFP", "AutoFL"],
         refstrain="WT",
         figs=True,
+        useGPs=True,
+        flcvfn="matern",
+        bd=None,
+        nosamples=500,
         experiments="all",
         experimentincludes=False,
         experimentexcludes=False,
         conditions="all",
         conditionincludes=False,
         conditionexcludes=False,
         strains="all",
         strainincludes=False,
         strainexcludes=False,
+        **kwargs,
     ):
         """
         Correct fluorescence for autofluorescence.
 
         The correction is made using the fluorescence of an untagged
         reference strain.
 
-        The reference strain is used to estimate the autofluoresence via either
-        the method of Licthen et al., 2014, where measurements of fluoescence
-        at two wavelengths is required, or by using the fluorescence of the
-        reference strain interpolated to the OD of the strain of interest
-        (Berthoumieux et al., 2013).
+        The reference strain is used to estimate the autofluorescence via
+        either the method of Lichten et al., 2014, where measurements of
+        fluorescence at two wavelengths is required, or by using the
+        fluorescence of the reference strain interpolated to the OD of the
+        strain of interest (Berthoumieux et al., 2013).
 
         Using two measurements of fluorescence is thought to be more accurate,
         particularly for low fluorescence measurements (Mihalcescu et al.,
         2015).
 
         Arguments
         --
         f: string or list of strings
             The fluorescence measurements, typically either ['mCherry'] or
             ['GFP', 'AutoFL'].
         refstrain: string
             The reference strain.
         figs: boolean
             If True, display plots showing the fits to the reference strain's
-            fluorescnce.
+            fluorescence.
+        useGPs: boolean
+            If True, use Gaussian processes to generate extra samples from
+            the replicates. Recommended, particularly if there are only a few
+            replicates, but slower.
+        flcvfn: str, optional
+            The covariance function to use for the Gaussian process applied
+            to the logarithm of the fluorescence.
+        bd: dict, optional
+            Specifies the bounds on the hyperparameters for the Gaussian
+            process applied to the logarithm of the fluorescence,
+            e.g. {2: (-2, 0)}.
         experiments: string or list of strings
             The experiments to include.
         conditions: string or list of strings
             The conditions to include.
         strains: string or list of strings
             The strains to include.
         experimentincludes: string, optional
@@ -2217,14 +2270,15 @@
         conditionexcludes: string, optional
             Ignores conditions that include the specified string in their name.
         strainincludes: string, optional
             Selects only strains that include the specified string in their
             name.
         strainexcludes: string, optional
             Ignores strains that include the specified string in their name.
+        **kwargs: passed to fitderiv when fitting the fluorescence.
 
         Notes
         -----
         In principle
 
         >>> p.correctmedia()
 
@@ -2284,15 +2338,15 @@
         I Mihalcescu, MVM Gateau, B Chelli, C Pinel, JL Ravanat (2015).
         Green autofluorescence, a double edged monitoring tool for bacterial
         growth and activity in micro-plates.
         Phys Biol, 12, 066016.
 
         """
         f = gu.makelist(f)
-        exps, cons, strs = sunder.getall(
+        exps, cons, _ = sunder.getall(
             self,
             experiments,
             experimentincludes,
             experimentexcludes,
             conditions,
             conditionincludes,
             conditionexcludes,
@@ -2306,74 +2360,76 @@
                 if self.progress["negativevalues"][e]:
                     for datatype in f:
                         if (
                             datatype in self.progress["negativevalues"][e]
                             and c in self.progress["negativevalues"][e]
                         ):
                             print(
-                                e + ": The negative values for",
-                                datatype,
-                                "in",
-                                c,
-                                "will generate NaNs",
+                                f"{e}: The negative values for {datatype}"
+                                f" in {c} will generate NaNs."
                             )
         # going ahead
-        print("Using", refstrain, "as the reference")
+        print(f"Using {refstrain} as the reference.")
         # correct for autofluorescence
         if len(f) == 2:
             corrections.correctauto2(
                 self,
                 f,
                 refstrain,
                 figs,
+                useGPs,
+                flcvfn,
+                bd,
+                nosamples,
                 experiments,
                 experimentincludes,
                 experimentexcludes,
                 conditions,
                 conditionincludes,
                 conditionexcludes,
                 strains,
                 strainincludes,
                 strainexcludes,
+                **kwargs,
             )
         elif len(f) == 1:
             corrections.correctauto1(
                 self,
                 f,
                 refstrain,
                 figs,
+                useGPs,
+                flcvfn,
+                bd,
+                nosamples,
                 experiments,
                 experimentincludes,
                 experimentexcludes,
                 conditions,
                 conditionincludes,
                 conditionexcludes,
                 strains,
                 strainincludes,
                 strainexcludes,
+                **kwargs,
             )
         else:
-            print("f must be a list of length 1 or 2")
+            print(f"f = {f} must be a list of length 1 or 2.")
 
-    ###
-    # Logging
-    ###
     @property
     def log(self):
         """
         Print a log of all methods called and their arguments.
 
         Example
         -------
         >>> p.log
         """
         print(self.logstream.getvalue())
 
-    ###
-
     def savelog(self, fname=None):
         """
         Save log to file.
 
         Parameters
         --
         fname: string, optional
@@ -2386,19 +2442,16 @@
         # export log
         if fname:
             fnamepath = self.wdirpath / (fname + ".log")
         else:
             fnamepath = self.wdirpath / ("".join(self.allexperiments) + ".log")
         with fnamepath.open("w") as f:
             f.write(self.logstream.getvalue())
-        print("Exported to", str(fnamepath))
+        print("Exported successfully.")
 
-    ###
-    # Exporting and importing
-    ###
     @clogger.log
     def exportdf(self, commonname=False, type="tsv"):
         """
         Export the dataframes.
 
         The exported data may either be tab-delimited or csv or json files.
         Dataframes for the (processed) raw data, for summary data, and for
@@ -2427,19 +2480,20 @@
             self.r.to_json(fullcommonname + "_r.json", orient="split")
             self.s.to_json(fullcommonname + "_s.json", orient="split")
             self.sc.to_json(fullcommonname + "_sc.json", orient="split")
         else:
             sep = "\t" if type == "tsv" else ","
             self.r.to_csv(fullcommonname + "_r." + type, sep=sep, index=False)
             self.s.to_csv(fullcommonname + "_s." + type, sep=sep, index=False)
-            self.sc.to_csv(fullcommonname + "_sc." + type, sep=sep, index=False)
+            self.sc.to_csv(
+                fullcommonname + "_sc." + type, sep=sep, index=False
+            )
         # export log to file
         self.savelog(commonname)
 
-    ###
     @clogger.log
     def importdf(self, commonnames, info=True, sep="\t"):
         """
         Import dataframes saved as either json or csv or tsv files.
 
         Parameters
         ----------
@@ -2478,16 +2532,16 @@
                             exec(
                                 "impdf= pd.read_csv(commonname + '_' + df "
                                 "+ '.tsv', sep= '\t')"
                             )
                             print("Imported", commonname + "_" + df + ".tsv")
                         except FileNotFoundError:
                             print(
-                                "No file called",
-                                commonname + "_" + df + ".json or .csv or .tsv found",
+                                f"No file called {commonname}_{df}.json "
+                                "or .csv or .tsv found"
                             )
                             return
                 # ensure all are imported as strings
                 for var in ["experiment", "condition", "strain"]:
                     exec("impdf[var]= impdf[var].astype(str)")
                 # merge dataframes
                 if hasattr(self, df):
@@ -2521,15 +2575,15 @@
         dtypdict = {}
         for e in self.allexperiments:
             # drop columns of NaNs - these are created by merge if a datatype
             # is in one experiment but not in another
             tdf = self.s[self.s.experiment == e].dropna(axis=1, how="all")
             dtypdict[e] = list(tdf.columns[tdf.columns.str.contains("mean")])
         self.datatypes.update(
-            {e: [dt.split(" mean")[0] for dt in dtypdict[e]] for e in dtypdict}
+            {e: [dt.split("_mean")[0] for dt in dtypdict[e]] for e in dtypdict}
         )
         # initialise progress
         for e in self.allexperiments:
             admin.initialiseprogress(self, e)
         # display info on import
         if info:
             self.info
@@ -2537,11 +2591,92 @@
         # display warning if duplicates created
         if len(self.allexperiments) != np.unique(self.allexperiments).size:
             print(
                 "\nLikely ERROR: data with the same experiment, condition, "
                 "strain, and time now appears twice!!"
             )
 
+    @clogger.log
+    def getmidlog(
+        self,
+        stat="mean",
+        min_duration=1,
+        figs=True,
+        experiments="all",
+        experimentincludes=False,
+        experimentexcludes=False,
+        conditions="all",
+        conditionincludes=False,
+        conditionexcludes=False,
+        strains="all",
+        strainincludes=False,
+        strainexcludes=False,
+        **kwargs,
+    ):
+        """
+        Calculate mid-log statistics.
+
+        Find the region of mid-log growth using nunchakue and calculate a
+        statistic for each variable in the s dataframe in this region only.
+
+        The results are added to the sc dataframe.
+
+        Parameters
+        ----------
+        stat: str
+            The name of the statistic to be calculated (using pandas).
+        min_duration: float
+            The expected minimal duration of the midlog phase in units of time.
+        figs: boolean
+            If True, show nunchaku's results with the mid-log region marked by black squares.
+        experiments: string or list of strings
+            The experiments to include.
+        conditions: string or list of strings
+            The conditions to include.
+        strains: string or list of strings
+            The strains to include.
+        experimentincludes: string, optional
+            Selects only experiments that include the specified string in
+            their name.
+        experimentexcludes: string, optional
+            Ignores experiments that include the specified string in their
+            name.
+        conditionincludes: string, optional
+            Selects only conditions that include the specified string in their
+            name.
+        conditionexcludes: string, optional
+            Ignores conditions that include the specified string in their name.
+        strainincludes: string, optional
+            Selects only strains that include the specified string in their
+            name.
+        strainexcludes: string, optional
+            Ignores strains that include the specified string in their name.
+        kwargs: passed to Nunchaku
+        """
+        exps, cons, strs = sunder.getall(
+            self,
+            experiments,
+            experimentincludes,
+            experimentexcludes,
+            conditions,
+            conditionincludes,
+            conditionexcludes,
+            strains,
+            strainincludes,
+            strainexcludes,
+            nonull=True,
+            nomedia=True,
+        )
+        # run Nunchaku to find midlog and take the mean of summary stats
+        midlog.find_midlog_stats(
+            self, stat, min_duration, figs, exps, cons, strs
+        )
+
+    @property
+    def cols_to_underscore(self):
+        """Replace spaces in column names of all dataframes with underscores."""
+        for df in [self.r, self.s, self.sc]:
+            df.columns = df.columns.str.replace(" ", "_")
+
 
-###
 if __name__ == "__main__":
     print(platereader.__doc__)
```

### Comparing `omniplate-0.9.6/pyproject.toml` & `omniplate-0.9.82/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omniplate"
-version = "0.9.6"
+version = "0.9.82"
 description = "For analysing and meta-analysing plate-reader data"
 authors = ["Peter Swain <peter.swain@ed.ac.uk>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://swainlab.bio.ed.ac.uk/software/omniplate"
 repository = "https://git.ecdf.ed.ac.uk/pswain/omniplate"
@@ -19,22 +19,25 @@
     { include = "omniplate" },
     { include = "om_code" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 pandas = ">=1.5.1"
-numpy = ">=1.21.4"
-scipy = ">=1.7.3"
-matplotlib = ">=3.5.3"
+numpy = "^1.24.3"
+scipy = "^1.10.1"
+matplotlib = "^3.7.1"
 seaborn = ">=0.11.2"
 statsmodels = ">=0.13.1"
 openpyxl = ">=3.0.9"
-gaussianprocessderivatives = ">=0.1.2"
+gaussianprocessderivatives = ">=0.1.64"
+nunchaku = "^0.11.0"
 
+[tool.black]
+line-length = 79
 
 [tool.poetry.dev-dependencies]
 
 
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `omniplate-0.9.6/PKG-INFO` & `omniplate-0.9.82/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniplate
-Version: 0.9.6
+Version: 0.9.82
 Summary: For analysing and meta-analysing plate-reader data
 Home-page: https://swainlab.bio.ed.ac.uk/software/omniplate
 License: MIT
 Keywords: omniplate,systems biology,bioinformatics,plate readers
 Author: Peter Swain
 Author-email: peter.swain@ed.ac.uk
 Requires-Python: >=3.8,<3.11
@@ -12,20 +12,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Dist: gaussianprocessderivatives (>=0.1.2)
-Requires-Dist: matplotlib (>=3.5.3)
-Requires-Dist: numpy (>=1.21.4)
+Requires-Dist: gaussianprocessderivatives (>=0.1.64)
+Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
+Requires-Dist: nunchaku (>=0.11.0,<0.12.0)
 Requires-Dist: openpyxl (>=3.0.9)
 Requires-Dist: pandas (>=1.5.1)
-Requires-Dist: scipy (>=1.7.3)
+Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn (>=0.11.2)
 Requires-Dist: statsmodels (>=0.13.1)
 Project-URL: Documentation, https://swainlab.bio.ed.ac.uk/software/omniplate
 Project-URL: Repository, https://git.ecdf.ed.ac.uk/pswain/omniplate
 Description-Content-Type: text/markdown
 
 A Python package for analysing data from plate-reader studies of growing biological cells. Users can correct for autofluorescence, determine growth rates and the amount of fluorescence per cell, and simultaneously analyse multiple experiments.
```

