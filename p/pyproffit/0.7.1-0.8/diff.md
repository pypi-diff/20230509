# Comparing `tmp/pyproffit-0.7.1.tar.gz` & `tmp/pyproffit-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproffit-0.7.1.tar", last modified: Tue Aug  9 13:23:02 2022, max compression
+gzip compressed data, was "pyproffit-0.8.tar", last modified: Tue May  9 15:52:54 2023, max compression
```

## Comparing `pyproffit-0.7.1.tar` & `pyproffit-0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 deckert    (501) staff       (20)        0 2022-08-09 13:23:02.604544 pyproffit-0.7.1/
--rwxr-xr-x   0 deckert    (501) staff       (20)    35149 2022-01-11 19:50:42.000000 pyproffit-0.7.1/LICENSE
--rw-r--r--   0 deckert    (501) staff       (20)      271 2022-08-09 13:23:02.604377 pyproffit-0.7.1/PKG-INFO
--rwxr-xr-x   0 deckert    (501) staff       (20)     1173 2022-01-11 19:50:42.000000 pyproffit-0.7.1/README.md
-drwxr-xr-x   0 deckert    (501) staff       (20)        0 2022-08-09 13:23:02.603525 pyproffit-0.7.1/pyproffit/
--rwxr-xr-x   0 deckert    (501) staff       (20)      306 2022-01-11 19:50:42.000000 pyproffit-0.7.1/pyproffit/__init__.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    11332 2022-01-11 19:50:42.000000 pyproffit-0.7.1/pyproffit/data.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    74985 2022-01-26 09:20:45.000000 pyproffit-0.7.1/pyproffit/deproject.py
--rwxr-xr-x   0 deckert    (501) staff       (20)     3876 2022-01-11 19:50:42.000000 pyproffit-0.7.1/pyproffit/emissivity.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    15558 2022-01-11 19:50:42.000000 pyproffit-0.7.1/pyproffit/fitting.py
--rwxr-xr-x   0 deckert    (501) staff       (20)     9978 2022-01-11 19:50:42.000000 pyproffit-0.7.1/pyproffit/hmc.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    19742 2022-08-09 09:32:40.000000 pyproffit-0.7.1/pyproffit/miscellaneous.py
--rwxr-xr-x   0 deckert    (501) staff       (20)     8264 2022-01-11 19:50:42.000000 pyproffit-0.7.1/pyproffit/models.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    25724 2022-01-11 19:50:42.000000 pyproffit-0.7.1/pyproffit/power_spectrum.py
--rwxr-xr-x   0 deckert    (501) staff       (20)    54718 2022-06-09 19:15:31.000000 pyproffit-0.7.1/pyproffit/profextract.py
--rwxr-xr-x   0 deckert    (501) staff       (20)     3234 2022-01-11 19:50:42.000000 pyproffit-0.7.1/pyproffit/reload.py
-drwxr-xr-x   0 deckert    (501) staff       (20)        0 2022-08-09 13:23:02.604187 pyproffit-0.7.1/pyproffit.egg-info/
--rwxr-xr-x   0 deckert    (501) staff       (20)      271 2022-08-09 13:23:02.000000 pyproffit-0.7.1/pyproffit.egg-info/PKG-INFO
--rwxr-xr-x   0 deckert    (501) staff       (20)      435 2022-08-09 13:23:02.000000 pyproffit-0.7.1/pyproffit.egg-info/SOURCES.txt
--rwxr-xr-x   0 deckert    (501) staff       (20)        1 2022-08-09 13:23:02.000000 pyproffit-0.7.1/pyproffit.egg-info/dependency_links.txt
--rwxr-xr-x   0 deckert    (501) staff       (20)       45 2022-08-09 13:23:02.000000 pyproffit-0.7.1/pyproffit.egg-info/requires.txt
--rwxr-xr-x   0 deckert    (501) staff       (20)       10 2022-08-09 13:23:02.000000 pyproffit-0.7.1/pyproffit.egg-info/top_level.txt
--rw-r--r--   0 deckert    (501) staff       (20)       38 2022-08-09 13:23:02.604597 pyproffit-0.7.1/setup.cfg
--rwxr-xr-x   0 deckert    (501) staff       (20)      446 2022-08-09 13:22:35.000000 pyproffit-0.7.1/setup.py
+drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-09 15:52:54.075299 pyproffit-0.8/
+-rwxr-xr-x   0 deckert    (501) staff       (20)    35149 2022-01-11 19:50:42.000000 pyproffit-0.8/LICENSE
+-rw-r--r--   0 deckert    (501) staff       (20)      224 2023-05-09 15:52:54.075124 pyproffit-0.8/PKG-INFO
+-rwxr-xr-x   0 deckert    (501) staff       (20)     1173 2022-01-11 19:50:42.000000 pyproffit-0.8/README.md
+drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-09 15:52:54.074205 pyproffit-0.8/pyproffit/
+-rwxr-xr-x   0 deckert    (501) staff       (20)      306 2022-01-11 19:50:42.000000 pyproffit-0.8/pyproffit/__init__.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    11332 2022-01-11 19:50:42.000000 pyproffit-0.8/pyproffit/data.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    79342 2023-05-09 15:06:02.000000 pyproffit-0.8/pyproffit/deproject.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)     3876 2022-01-11 19:50:42.000000 pyproffit-0.8/pyproffit/emissivity.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    15558 2022-01-11 19:50:42.000000 pyproffit-0.8/pyproffit/fitting.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)     9977 2023-05-02 11:54:25.000000 pyproffit-0.8/pyproffit/hmc.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    20778 2023-05-09 15:07:28.000000 pyproffit-0.8/pyproffit/miscellaneous.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)     8263 2023-05-02 11:54:25.000000 pyproffit-0.8/pyproffit/models.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    25724 2022-01-11 19:50:42.000000 pyproffit-0.8/pyproffit/power_spectrum.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)    55271 2023-05-09 15:42:44.000000 pyproffit-0.8/pyproffit/profextract.py
+-rwxr-xr-x   0 deckert    (501) staff       (20)     3234 2022-01-11 19:50:42.000000 pyproffit-0.8/pyproffit/reload.py
+drwxr-xr-x   0 deckert    (501) staff       (20)        0 2023-05-09 15:52:54.074935 pyproffit-0.8/pyproffit.egg-info/
+-rwxr-xr-x   0 deckert    (501) staff       (20)      224 2023-05-09 15:52:54.000000 pyproffit-0.8/pyproffit.egg-info/PKG-INFO
+-rwxr-xr-x   0 deckert    (501) staff       (20)      435 2023-05-09 15:52:54.000000 pyproffit-0.8/pyproffit.egg-info/SOURCES.txt
+-rwxr-xr-x   0 deckert    (501) staff       (20)        1 2023-05-09 15:52:54.000000 pyproffit-0.8/pyproffit.egg-info/dependency_links.txt
+-rwxr-xr-x   0 deckert    (501) staff       (20)       44 2023-05-09 15:52:54.000000 pyproffit-0.8/pyproffit.egg-info/requires.txt
+-rwxr-xr-x   0 deckert    (501) staff       (20)       10 2023-05-09 15:52:54.000000 pyproffit-0.8/pyproffit.egg-info/top_level.txt
+-rw-r--r--   0 deckert    (501) staff       (20)       38 2023-05-09 15:52:54.075343 pyproffit-0.8/setup.cfg
+-rwxr-xr-x   0 deckert    (501) staff       (20)      443 2023-05-09 15:07:57.000000 pyproffit-0.8/setup.py
```

### Comparing `pyproffit-0.7.1/LICENSE` & `pyproffit-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproffit-0.7.1/README.md` & `pyproffit-0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyproffit-0.7.1/pyproffit/data.py` & `pyproffit-0.8/pyproffit/data.py`

 * *Files identical despite different names*

### Comparing `pyproffit-0.7.1/pyproffit/deproject.py` & `pyproffit-0.8/pyproffit/deproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-import pymc3 as pm
+import pymc as pm
 import time
 from scipy.special import gamma
 import matplotlib.pyplot as plt
 #plt.switch_backend('Agg')
 from scipy.interpolate import interp1d
 import os
 from astropy.io import fits
@@ -537,15 +537,15 @@
     deproj.sb_hi = pmch
     deproj.bkg = bfit
     
     
     
 def Deproject_Multiscale_PyMC3(deproj,bkglim=None,nmcmc=1000,tune=500,back=None,samplefile=None,nrc=None,nbetas=6,min_beta=0.6):
     """
-    Run the multiscale deprojection optimization using the PyMC3 backend
+    Run the multiscale deprojection optimization using the PyMC backend
 
     :param deproj: Object of type :class:`pyproffit.deproject.Deproject` containing the data and parameters
     :type deproj: class:`pyproffit.deproject.Deproject`
     :param bkglim: Limit beyond which it is assumed that the background dominates, i.e. the source is set to 0. If bkglim=None (default), the entire radial range is used
     :type bkglim: float
     :param nmcmc: Number of HMC points in the output sample
     :type nmcmc: int
@@ -606,39 +606,65 @@
     if np.isnan(back) or back == 0:
         testbkg = -10.
     else:
         testbkg = np.log(back)
 
     with basic_model:
         # Priors for unknown model parameters
-        coefs = pm.Normal('coefs', mu=testval, sd=20, shape=npt)
-        bkgd = pm.Normal('bkg', mu=testbkg, sd=0.05, shape=1)
+        coefs = pm.Normal('coefs', mu=testval, sigma=20, shape=npt)
+        bkgd = pm.Normal('bkg', mu=testbkg, sigma=0.05, shape=1)
         ctot = pm.math.concatenate((coefs, bkgd), axis=0)
 
         # Expected value of outcome
         al = pm.math.exp(ctot)
         pred = pm.math.dot(K, al) + bkgcounts
 
         # Likelihood (sampling distribution) of observations
         Y_obs = pm.Poisson('counts', mu=pred, observed=counts)
 
     tinit = time.time()
+
+    isjax = False
+
+    try:
+        import pymc.sampling.jax as pmjax
+
+    except ImportError:
+        print('JAX not found, using default sampler')
+
+    else:
+        isjax = True
+        import pymc.sampling.jax as pmjax
+
     print('Running MCMC...')
     with basic_model:
         tm = pm.find_MAP()
-        trace = pm.sample(nmcmc, tune=tune, start=tm)
-        #trace = pm.sample(nmcmc)
+
+        if not isjax:
+
+            trace = pm.sample(nmcmc, initvals=tm, tune=tune)
+
+        else:
+
+            trace = pmjax.sample_numpyro_nuts(nmcmc, initvals=tm, tune=tune)
+
     print('Done.')
     tend = time.time()
     print(' Total computing time is: ', (tend - tinit) / 60., ' minutes')
 
     # Get chains and save them to file
-    sampc = trace.get_values('coefs')
-    sampb = trace.get_values('bkg')
-    samples = np.append(sampc, sampb, axis=1)
+    chain_coefs = trace.posterior['coefs'].to_numpy()
+    sc_coefs = chain_coefs.shape
+    sampc = chain_coefs.reshape(sc_coefs[0] * sc_coefs[1], sc_coefs[2])
+
+    sampb = trace.posterior['bkg'].to_numpy().flatten()
+
+    spb = np.array([sampb]).T
+
+    samples = np.append(sampc, spb, axis=1)
     if samplefile is not None:
         np.savetxt(samplefile, samples)
         np.savetxt(samplefile+'.par',np.array([pars.shape[0]/nbetas,nbetas,min_beta,nmcmc]),header='pymc3')
 
     # Compute output deconvolved brightness profile
     Ksb = calc_sb_operator(rad, sourcereg, pars)
     allsb = np.dot(Ksb, np.exp(samples.T))
@@ -1408,14 +1434,15 @@
         :param kwargs: Options to be passed to :class:`matplotplib.pyplot.hist`
         :return: Median :math:`M_{gas}`, 16th and 84th percentiles
         :rtype: float
         """
         if self.samples is None or self.z is None or self.cf is None:
             print('Error: no gas density profile found')
             return
+
         prof = self.profile
         cosmo = prof.cosmo
 
         kpcp = cosmo.kpc_proper_per_arcmin(self.z).value
         rkpc = prof.bins * kpcp
         erkpc = prof.ebins * kpcp
         nhconv =  mh * self.mu_e * self.nhc * kpc ** 3 / msun  # Msun/kpc^3
@@ -1471,15 +1498,15 @@
 
             mgasdist = np.empty(len(self.samples))
 
             for i in range(len(self.samples)):
 
                 mgasdist[i] = np.interp(radii[i], rkpc, mgas[:, i])
 
-                rho = np.corrcoef(radii, mgasdist)[0,1]
+            rho = np.corrcoef(radii, mgasdist)[0,1]
 
         else:
 
             f = interp1d(rkpc, mgas, axis=0)
 
             mgasdist = f(radius)
 
@@ -1501,15 +1528,130 @@
             plt.ylabel('Frequency', fontsize=fontsize)
             if outfile is not None:
                 plt.savefig(outfile)
                 plt.close()
             else:
                 plt.show(block=False)
 
-        return mg,mgl,mgh
+        return mg,mgl,mgh,rho
+
+    def Cov_Mgas_Lx(self, radius, radius_err=None, rad_scale='normal'):
+
+        if self.samples is None or self.z is None or self.cf is None:
+            print('Error: no gas density profile found')
+            return
+        prof = self.profile
+        cosmo = prof.cosmo
+
+        kpcp = cosmo.kpc_proper_per_arcmin(self.z).value
+        rkpc = prof.bins * kpcp
+        erkpc = prof.ebins * kpcp
+        nhconv =  mh * self.mu_e * self.nhc * kpc ** 3 / msun  # Msun/kpc^3
+
+        rad = prof.bins
+        sourcereg = np.where(rad < self.bkglim)
+
+        transf = 4. * (1. + self.z) ** 2 * (180. * 60.) ** 2 / np.pi / 1e-14 / self.nhc / Mpc * 1e3
+        pardens = list_params_density(rad, sourcereg, self.z, cosmo, self.nrc, self.nbetas, self.min_beta)
+        Kdens = calc_density_operator(rad, pardens, self.z, cosmo)
+
+        # All gas density profiles
+        alldens = np.sqrt(np.dot(Kdens, np.exp(self.samples.T)) / self.cf * transf)  # [0:nptfit, :]
+
+        # Matrix containing integration volumes
+        volmat = np.repeat(4. * np.pi * rkpc ** 2 * 2. * erkpc, alldens.shape[1]).reshape(len(prof.bins),alldens.shape[1])
+
+        # Compute Mgas profile as cumulative sum over the volume
+        mgas = np.cumsum(alldens * nhconv * volmat, axis=0)
+
+        # Interpolate at the radius of interest
+        # Avoid diverging profiles in the center by cutting to the innermost points, if necessary
+        a = prof.bins[0]/2.
+
+        # Set vector with list of parameters
+        pars = list_params(rad, sourcereg, self.nrc, self.nbetas, self.min_beta)
+
+        # Set randomization of the radius if radius_err is not None
+        rho = None
+
+        if radius_err is not None:
+
+            nsim = len(self.samples)
+
+            if rad_scale == 'normal':
+
+                radii = radius_err * np.random.randn(nsim) + radius
+
+            elif rad_scale == 'lognormal':
+
+                rad_log = np.log(radius)
+
+                err_rad_log = radius_err / radius
+
+                radii = np.exp(err_rad_log * np.random.randn(nsim) + rad_log)
+
+            else:
+
+                print('Unknown value rad_scale=%s , reverting to normal' % (rad_scale))
+
+                radii = radius_err * np.random.randn(nsim) + radius
+
+            if np.any(radii < 0.0):
+
+                isneg = np.where(radii < 0.0)
+
+                radii[isneg] = 0.0
+
+            mgasdist = np.empty(len(self.samples))
+            allint = np.empty(len(self.samples))
+
+            b = radii / kpcp
+
+            for i in range(len(self.samples)):
+
+                mgasdist[i] = np.interp(radii[i], rkpc, mgas[:, i])
+
+                # Compute linear combination of basis functions in the source region
+                Kint = calc_int_operator(a, b[i], pars)
+                tal = np.dot(Kint, np.exp(self.samples.T)) * self.lumfact
+                allint[i] = tal[1, i] - tal[0, i]
+
+        else:
+
+            f = interp1d(rkpc, mgas, axis=0)
+
+            Kint = calc_int_operator(a, radius/kpcp, pars)
+
+            tal = np.dot(Kint, np.exp(self.samples.T)) * self.lumfact
+            allint = tal[1, :] - tal[0, :]
+
+            mgasdist = f(radius)
+
+        rho_lxmg = np.corrcoef(allint, mgasdist)[0,1]
+
+        mg, mgl, mgh = np.percentile(mgasdist,[50.,50.-68.3/2.,50.+68.3/2.])
+        medint, intlo, inthi = np.percentile(allint, [50.,50.-68.3/2.,50.+68.3/2.])
+
+        outdict = {'MGAS': mg,
+                   'MGAS_LO': mgl,
+                   'MGAS_HI': mgh,
+                   'LX': medint,
+                   'LX_LO': intlo,
+                   'LX_HI': inthi,
+                   'RHO_LXMG': rho_lxmg
+                   }
+        if radius_err is not None:
+            rho_rlx =  np.corrcoef(radii, allint)[0,1]
+            rho_rmg =  np.corrcoef(radii, mgasdist)[0,1]
+
+            outdict['RHO_RLX'] = rho_rlx
+            outdict['RHO_RMG'] = rho_rmg
+
+        return outdict
+
 
     def PlotMgas(self,rout=None,outfile=None,xunit="kpc", figsize=(13, 10), color='C0', lw=2, fontsize=40, xscale='log', yscale='log'):
         """
         Plot the cumulative gas mass profile from the output of a reconstruction
 
         :param rout: Radial binning of the gas mass profile. If rout=None, the original binning of the surface brightness profile is used
         :type rout: numpy.ndarray
```

### Comparing `pyproffit-0.7.1/pyproffit/emissivity.py` & `pyproffit-0.8/pyproffit/emissivity.py`

 * *Files identical despite different names*

### Comparing `pyproffit-0.7.1/pyproffit/fitting.py` & `pyproffit-0.8/pyproffit/fitting.py`

 * *Files identical despite different names*

### Comparing `pyproffit-0.7.1/pyproffit/hmc.py` & `pyproffit-0.8/pyproffit/hmc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pymc3 as pm
+import pymc as pm
 import numpy as np
 import time
 from .models import IntFunc
 
 def BetaModelPM(x, beta, rc, norm, bkg):
     """
     """
```

### Comparing `pyproffit-0.7.1/pyproffit/miscellaneous.py` & `pyproffit-0.8/pyproffit/miscellaneous.py`

 * *Files 7% similar despite different names*

```diff
@@ -368,26 +368,27 @@
             all_mod[i] = np.dot(psfmat, tmod)
 
     mod_med, mod_lo, mod_hi = np.percentile(all_mod, [50., 50. - 68.3 / 2., 50. + 68.3 / 2.], axis=0)
 
     return mod_med, mod_lo, mod_hi
 
 
-def Rebin(prof, minc=None, snr=None, fitter=None):
+import copy
+
+
+def Rebin(prof, minc=None, snr=None):
     '''
     Rebin an existing surface brightness profile to reach a given target number of counts per bin (minc) or a minimum S/N (snr).
 
     :param prof: A :class:`pyproffit.profextract.Profile` object including the current profile to be rebinned
     :type prof: :class:`pyproffit.profextract.Profile`
     :param minc: Minimum number of counts per bin for the output profile. If None, a minimum S/N is used. Defaults to None.
     :type minc: int
     :param snr: Minimum signal-to-noise ratio of the output profile. If None, a minimum number of counts is used. Defaults to None.
     :type snr: float
-    :param fitter: Object of type :class:`pyproffit.fitting.Fitter` containing a model and optimization results to subtract the sky background. If None, no sky background subtraction is performed. Defaults to None.
-    :type fitter: :class:`pyproffit.fitting.Fitter`
     :return: A new :class:`pyproffit.profextract.Profile` object with the rebinned surface brightness profile.
     :rtype: :class:`pyproffit.profextract.Profile`
     '''
 
     is_minc = True
     if minc is None and snr is None:
         print('No target number of counts or S/N provided, aborting')
@@ -409,17 +410,17 @@
 
     back_new, area_new, exp_new, bkgcounts_new = np.array([]), np.array([]), np.array([]), np.array([])
 
     nbin = prof.nbin
 
     skybkg, eskybkg = 0., 0.
 
-    if fitter is not None:
-        skybkg = np.power(10., fitter.minuit.values['bkg'])
-        eskybkg = skybkg * np.log(10.) * fitter.minuit.errors['bkg']
+    if prof.bkgval is not None:
+        skybkg = prof.bkgval
+        eskybkg = prof.bkgerr
 
     i = 0
     while i < nbin:
         if is_minc:
             if prof.counts[i] >= minc:
                 prof_new = np.append(prof_new, prof.profile[i])
                 bins_new = np.append(bins_new, prof.bins[i])
@@ -462,14 +463,27 @@
                     prof_new = np.append(prof_new, sb_new)
                     bnew = tbkgc / tarea / ten
                     back_new = np.append(back_new, bnew)
                     epnew = np.sqrt(tcounts / (ten * tarea) ** 2 + eskybkg ** 2)
                     eprof_new = np.append(eprof_new, epnew)
 
                     i = i + l
+                if i == nbin - 1:
+                    prof_new = np.append(prof_new, prof.profile[i])
+                    bins_new = np.append(bins_new, prof.bins[i])
+                    ebins_new = np.append(ebins_new, prof.ebins[i])
+                    eprof_new = np.append(eprof_new, prof.eprof[i])
+                    back_new = np.append(back_new, prof.bkgprof[i])
+                    area_new = np.append(area_new, prof.area[i])
+                    exp_new = np.append(exp_new, prof.effexp[i])
+                    bkgcounts_new = np.append(bkgcounts_new, prof.bkgcounts[i])
+                    counts_new = np.append(counts_new, prof.counts[i])
+                    i = i + 1
+
+
 
         else:
             if prof.profile[i] / prof.eprof[i] >= snr:
                 prof_new = np.append(prof_new, prof.profile[i])
                 bins_new = np.append(bins_new, prof.bins[i])
                 ebins_new = np.append(ebins_new, prof.ebins[i])
                 eprof_new = np.append(eprof_new, prof.eprof[i])
@@ -515,14 +529,26 @@
                     bnew = tbkgc / tarea / ten
                     back_new = np.append(back_new, bnew)
                     epnew = np.sqrt(tcounts / (ten * tarea) ** 2 + eskybkg ** 2)
                     eprof_new = np.append(eprof_new, epnew)
 
                     i = i + l
 
+                if i == nbin - 1:
+                    prof_new = np.append(prof_new, prof.profile[i])
+                    bins_new = np.append(bins_new, prof.bins[i])
+                    ebins_new = np.append(ebins_new, prof.ebins[i])
+                    eprof_new = np.append(eprof_new, prof.eprof[i])
+                    back_new = np.append(back_new, prof.bkgprof[i])
+                    area_new = np.append(area_new, prof.area[i])
+                    exp_new = np.append(exp_new, prof.effexp[i])
+                    bkgcounts_new = np.append(bkgcounts_new, prof.bkgcounts[i])
+                    counts_new = np.append(counts_new, prof.counts[i])
+                    i = i + 1
+
     prof_out = copy.copy(prof)
     prof_out.nbin = len(prof_new)
     prof_out.profile = prof_new
     prof_out.bins = bins_new
     prof_out.ebins = ebins_new
     prof_out.eprof = eprof_new
     prof_out.area = area_new
```

### Comparing `pyproffit-0.7.1/pyproffit/models.py` & `pyproffit-0.8/pyproffit/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-import pymc3 as pm
+import pymc as pm
 
 def BetaModel(x, beta, rc, norm, bkg):
     """
     Single Beta model
 
     .. math::
```

### Comparing `pyproffit-0.7.1/pyproffit/power_spectrum.py` & `pyproffit-0.8/pyproffit/power_spectrum.py`

 * *Files identical despite different names*

### Comparing `pyproffit-0.7.1/pyproffit/profextract.py` & `pyproffit-0.8/pyproffit/profextract.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,14 +345,19 @@
         :type box: bool
         :param width: In case box=True, set the full width of the box (in arcmin)
         :type width: float
         """
         data = self.data
         img = data.img
         voronoi = self.voronoi
+
+        rmsmap = False
+        if data.rmsmap is not None:
+            rmsmap = True
+
         if not voronoi:
             exposure = np.copy(data.exposure)
 
             maxexp = np.max(exposure)
 
             lowexp = np.where(exposure <= minexp * maxexp)
 
@@ -449,16 +454,19 @@
                                            exposure > 0.0), np.fabs(xtil) <= width/2.))
                     else:
                         id = np.where(np.logical_and(np.logical_and(np.logical_and(ytil + self.maxrad/2. >= np.round(self.bins[i] - self.ebins[i], 5) + tol,
                                                     ytil + self.maxrad/2. < np.round(self.bins[i] + self.ebins[i], 5) + tol), exposure > 0.0), np.fabs(xtil) <= width/2.))
 
             #            id=np.where(np.logical_and(np.logical_and(rads>=self.bins[i]-self.ebins[i],rads<self.bins[i]+self.ebins[i]),exposure>0.0)) #left-inclusive
             nv = len(img[id])
-            if voronoi:
-                errmap = data.errmap
+            if voronoi or rmsmap:
+                if voronoi:
+                    errmap = data.errmap
+                else:
+                    errmap = data.rmsmap
                 profile[i] = np.sum(img[id]) / nv
                 eprof[i] = np.sqrt(np.sum(errmap[id] ** 2)) / nv
                 area[i] = nv * pixsize ** 2
                 effexp[i] = 1. # Dummy, but to be consistent with PSF calculation
             else:
                 if nv > 0:
                     bkgprof[i] = np.sum(bkg[id] / exposure[id]) / nv / pixsize ** 2
@@ -476,14 +484,16 @@
                     bkgcounts[i] = 0.
                     area[i] = 0.
                     effexp[i] = 0.
         self.profile = profile
         self.eprof = eprof
         self.area = area
         self.effexp = effexp
+        self.bkgval = None
+        self.bkgerr = None
 
         if not voronoi:
             self.counts = counts
             self.bkgprof = bkgprof
             self.bkgcounts = bkgcounts
 
 
@@ -503,17 +513,21 @@
         :type fitter: class:`pyproffit.fitter.Fitter`
         :param thin: Number of blocks into which the calculation of the bootstrap will be divided. Increasing thin reduces memory usage drastically, at the cost of a modest increase in computation time.
         :type thin: int
         """
         data = self.data
         img = data.img
         errmap = data.errmap
+
+        if data.rmsmap is not None:
+            errmap = data.rmsmap
+
         expo = data.exposure
         if errmap is None:
-            print('Error: No Voronoi map has been loaded')
+            print('Error: No Voronoi or RMS map has been loaded')
             return
         pixsize = data.pixsize
         if not self.custom:
             if (self.islogbin):
                 self.bins, self.ebins = logbinning(self.binsize, self.maxrad)
                 nbin = len(self.bins)
                 self.nbin = nbin
@@ -745,15 +759,15 @@
                 tbhdu = fits.BinTableHDU.from_columns(cols, name='MODEL')
                 hdul.append(tbhdu)
             if self.psfmat is not None:
                 psfhdu = fits.ImageHDU(self.psfmat, name='PSF')
                 hdul.append(psfhdu)
             hdul.writeto(outfile, overwrite=True)
 
-    def PSF(self, psffunc=None, psffile=None, psfimage=None, psfpixsize=None, sourcemodel=None, psfmin = 1e-7):
+    def PSF(self, psffunc=None, psffile=None, psfimage=None, psfpixsize=None, sourcemodel=None, psfmin = 0):
         """
         Function to calculate a PSF convolution matrix given an input PSF image or function.
         To compute the PSF mixing matrix, images of each annuli are convolved with the PSF image using FFT and determine the fraction of photons leaking into neighbouring annuli. FFT-convolved images are then used to determine a mixing matrix. See Eckert et al. 2020 for more details.
 
         :param psffunc: Function describing the radial shape of the PSF, with the radius in arcmin
         :type psffunc: function
         :param psffile: Path to file containing an image of the PSF. The pixel size must be equal to the pixel size of the image.
@@ -885,15 +899,15 @@
         gsexp = gaussian_filter(self.data.exposure, smoothing_scale)
         bkgsmoothed = np.nan_to_num(np.divide(gsb, gsexp)) * self.data.exposure
  #       bkgsmoothed = bkg_smooth(self.data,smoothing_scale)
         hdu = fits.PrimaryHDU(modimg+bkgsmoothed)
         hdu.header = head
         hdu.writeto(outfile, overwrite=True)
 
-    def Plot(self, model=None, samples=None, outfile=None, axes=None, scatter=False, figsize=(13, 10),
+    def Plot(self, model=None, samples=None, outfile=None, axes=None, scatter=False, offset=None, figsize=(13, 10),
              fontsize=40., xscale='log', yscale='log', fmt='o', markersize=7, lw=2,
              data_color='black', bkg_color='green', model_color='blue', **kwargs):
         """
         Plot the loaded surface brightness profile
 
         :param model: If model is not None, plot the provided model of type :class:`pyproffit.models.Model` together with the data. Defaults to None
         :type model: class:`pyproffit.models.Model` , optional
@@ -949,15 +963,18 @@
                 item.set_fontsize(0)
             else:
                 item.set_fontsize(18)
 
         if not self.box:
             rads = self.bins
         else:
-            rads = self.bins - self.maxrad/2.
+            if offset is None:
+                rads = self.bins - self.maxrad/2.
+
+            else: rads = self.bins - offset
 
         mod_med, mod_lo, mod_hi = None, None, None
         if samples is not None and model is not None:
 
             mod_med, mod_lo, mod_hi = model_from_samples(rads, model, samples, self.psfmat)
 
         if model is None:
@@ -1057,17 +1074,20 @@
         if self.profile is None:
             print('Error: no surface brightness profile found')
             return
         val=np.power(10.,fitter.minuit.values['bkg'])
         eval=val*np.log(10.)*fitter.minuit.errors['bkg']
         self.profile = self.profile - val
         self.eprof = np.sqrt(self.eprof**2 + eval**2)
+        self.bkgval = val
+        self.bkgerr = eval
 
 
-    def Emissivity(self, z=None, nh=None, kt=6.0, rmf=None, Z=0.3, elow=0.5, ehigh=2.0, arf=None, type='cr', lum_elow=0.5, lum_ehigh=2.0):
+    def Emissivity(self, z=None, nh=None, kt=6.0, rmf=None, Z=0.3, elow=0.5, ehigh=2.0, arf=None, type='cr',
+                   lum_elow=0.5, lum_ehigh=2.0, abund='angr'):
         """
         Use XSPEC to compute the conversion from count rate to emissivity using the pyproffit.calc_emissivity routine (see its description)
 
         :param z: Source redshift
         :type z: float
         :param nh: Source NH in units of 1e22 cm**(-2)
         :type nh: float
@@ -1099,10 +1119,11 @@
                                         rmf=rmf,
                                         Z=Z,
                                         elow=elow,
                                         ehigh=ehigh,
                                         arf=arf,
                                         type=type,
                                         lum_elow=lum_elow,
-                                        lum_ehigh=lum_ehigh)
+                                        lum_ehigh=lum_ehigh,
+                                        abund=abund)
 
         return self.ccf
```

### Comparing `pyproffit-0.7.1/pyproffit/reload.py` & `pyproffit-0.8/pyproffit/reload.py`

 * *Files identical despite different names*

