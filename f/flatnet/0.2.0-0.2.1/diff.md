# Comparing `tmp/flatnet-0.2.0.tar.gz` & `tmp/flatnet-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatnet-0.2.0.tar", last modified: Mon May  8 10:12:02 2023, max compression
+gzip compressed data, was "flatnet-0.2.1.tar", last modified: Mon May  8 21:54:23 2023, max compression
```

## Comparing `flatnet-0.2.0.tar` & `flatnet-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-08 20:34:24.043226 flatnet-0.2.0/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     5804 2023-05-08 20:34:24.043226 flatnet-0.2.0/PKG-INFO
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3562 2023-05-06 15:23:53.000000 flatnet-0.2.0/README.md
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-08 20:34:23.543223 flatnet-0.2.0/flatnet/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       24 2023-05-06 03:00:44.000000 flatnet-0.2.0/flatnet/__init__.py
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-08 20:34:23.965098 flatnet-0.2.0/flatnet/modules/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-04-06 05:54:15.000000 flatnet-0.2.0/flatnet/modules/__init__.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3564 2023-05-05 20:51:08.000000 flatnet-0.2.0/flatnet/modules/flatnet_nn.py
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    16415 2023-05-08 04:24:36.000000 flatnet-0.2.0/flatnet/train.py
-drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-08 20:34:23.824508 flatnet-0.2.0/flatnet.egg-info/
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     5804 2023-05-08 20:34:22.000000 flatnet-0.2.0/flatnet.egg-info/PKG-INFO
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      267 2023-05-08 20:34:23.000000 flatnet-0.2.0/flatnet.egg-info/SOURCES.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        1 2023-05-08 20:34:22.000000 flatnet-0.2.0/flatnet.egg-info/dependency_links.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      572 2023-05-08 20:34:22.000000 flatnet-0.2.0/flatnet.egg-info/requires.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        8 2023-05-08 20:34:22.000000 flatnet-0.2.0/flatnet.egg-info/top_level.txt
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       38 2023-05-08 20:34:24.043226 flatnet-0.2.0/setup.cfg
--rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     2213 2023-05-08 04:12:54.000000 flatnet-0.2.0/setup.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-09 16:16:08.238248 flatnet-0.2.1/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     5953 2023-05-09 16:16:08.222622 flatnet-0.2.1/PKG-INFO
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3567 2023-05-09 16:13:24.000000 flatnet-0.2.1/README.md
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-09 16:16:07.675748 flatnet-0.2.1/flatnet/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       24 2023-05-06 03:00:44.000000 flatnet-0.2.1/flatnet/__init__.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-09 16:16:08.144498 flatnet-0.2.1/flatnet/modules/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2022-04-06 05:54:15.000000 flatnet-0.2.1/flatnet/modules/__init__.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     3564 2023-05-05 20:51:08.000000 flatnet-0.2.1/flatnet/modules/flatnet_nn.py
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)    17534 2023-05-09 14:16:47.000000 flatnet-0.2.1/flatnet/train.py
+drwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        0 2023-05-09 16:16:07.988246 flatnet-0.2.1/flatnet.egg-info/
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     5953 2023-05-09 16:16:07.000000 flatnet-0.2.1/flatnet.egg-info/PKG-INFO
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      267 2023-05-09 16:16:07.000000 flatnet-0.2.1/flatnet.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        1 2023-05-09 16:16:07.000000 flatnet-0.2.1/flatnet.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)      572 2023-05-09 16:16:07.000000 flatnet-0.2.1/flatnet.egg-info/requires.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)        8 2023-05-09 16:16:07.000000 flatnet-0.2.1/flatnet.egg-info/top_level.txt
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)       38 2023-05-09 16:16:08.238248 flatnet-0.2.1/setup.cfg
+-rwxrwxrwx   0 mpsenka   (1000) mpsenka   (1000)     2213 2023-05-09 16:14:42.000000 flatnet-0.2.1/setup.py
```

### Comparing `flatnet-0.2.0/PKG-INFO` & `flatnet-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 Metadata-Version: 2.1
 Name: flatnet
-Version: 0.2.0
+Version: 0.2.1
 Summary: FlatNet implementation in PyTorch, from the paper "Representation Learning via Manifold Flattening and Reconstruction"
 Home-page: UNKNOWN
 Author: Michael Psenka
 Author-email: psenka@eecs.berkeley.edu
 Maintainer: ['Druv Pai <druvpai@berkeley.edu>', 'Vishal Raman <vraman@berkeley.edu>']
 License: UNKNOWN
 Description: This is a minimal pip package to allow easy deployment of FlatNets, a geometry-based neural autoencoder architecture that automatically builds its layers based on geometric properties of the dataset. See our paper, [Representation Learning via Manifold Flattening and Reconstruction](https://arxiv.org/abs/2305.01777), for more details, and [the Github repo](https://github.com/michael-psenka/manifold-linearization) for the code and example scripts & notebooks.
         
         Changelog
         =========
+        0.2.1 (2023-05-09)
+        ------------------
+        Features:
+        - Added support for 3D data for gif saving.
+        
         0.2.0 (2023-05-07)
         ------------------
         Features:
         - Added easy gif saving! If your data is 2D, you can now visualize how your data evolves with the manifold flow.
         
         0.1.4 (2023-05-06)
         ------------------
         Bug Fixes:
         - Remembered why I did not add normalization into main training file, now removed
         
         0.1.3 (2023-05-06)
         ------------------
         
         Bug Fixes:
-        - Added normalization of the input data
+        - Minor performance improvements on simple cases
         
         0.1.1 (2023-05-06)
         ------------------
         
         Features:
         - Added normalization of the input data
         
         0.1.0 (2022-12-31)
         ------------------
         
-        Initial release of flatnet!
+        - Initial release of flatnet!
         
         # Manifold Linearization for Representation Learning
         
         This is a research project focused on the automatic generation of autoencoders with minimal feature size, when the data is supported near an embedded submanifold. Using the geometric structure of the manifold, we can equivalently treat this problem as a manifold flattening problem when the manifold is flattenable[^1]. See our paper, [Representation Learning via Manifold Flattening and Reconstruction](https://arxiv.org/abs/2305.01777), for more details.
         
         [^1]: Geometric note: while flattenability is not general, there are some heuristic reasons we can motivate this assumption for real world data. For example, if a dataset permits a VAE-like autoencoder, where samples from the data distribution can be generated via a standard Gaussian in the latent space, then the samples lie close in probability to a flattenable manifold, as this VAE has constructed a single-chart atlas.
         
@@ -82,15 +87,15 @@
         
         Z = f(X).detach().numpy()
         
         plt.scatter(Z[:,0], Z[:,1])
         plt.show()
         ```
         
-        The script `flatnet.py` includes many example experiments to run FlatNet constructions on. To see an example experiment, simply run `python flatnet_test.py` in the main directory to see the flattening and reconstruction of a simple sine wave. Further experiments and options can be specified through command line arguments, managed through [tyro](https://github.com/brentyi/tyro); to see the full list of arguments, run `python flatnet_test.py --help`.
+        The script `flatnet_test.py` includes many example experiments to run FlatNet constructions on. To see an example experiment, simply run `python flatnet_test.py` in the main directory to see the flattening and reconstruction of a simple sine wave. Further experiments and options can be specified through command line arguments, managed through [tyro](https://github.com/brentyi/tyro); to see the full list of arguments, run `python flatnet_test.py --help`.
         
         
         ## Directory Structure
         
         - `flatnet_test.py`: main test script, as described in above section.
         - `flatnet/train.py`: contains the main FlatNet construction (training) code.
         - `flatnet/modules`: contains code for the neural network modules used in FlatNet.
```

### Comparing `flatnet-0.2.0/README.md` & `flatnet-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 Z = f(X).detach().numpy()
 
 plt.scatter(Z[:,0], Z[:,1])
 plt.show()
 ```
 
-The script `flatnet.py` includes many example experiments to run FlatNet constructions on. To see an example experiment, simply run `python flatnet_test.py` in the main directory to see the flattening and reconstruction of a simple sine wave. Further experiments and options can be specified through command line arguments, managed through [tyro](https://github.com/brentyi/tyro); to see the full list of arguments, run `python flatnet_test.py --help`.
+The script `flatnet_test.py` includes many example experiments to run FlatNet constructions on. To see an example experiment, simply run `python flatnet_test.py` in the main directory to see the flattening and reconstruction of a simple sine wave. Further experiments and options can be specified through command line arguments, managed through [tyro](https://github.com/brentyi/tyro); to see the full list of arguments, run `python flatnet_test.py --help`.
 
 
 ## Directory Structure
 
 - `flatnet_test.py`: main test script, as described in above section.
 - `flatnet/train.py`: contains the main FlatNet construction (training) code.
 - `flatnet/modules`: contains code for the neural network modules used in FlatNet.
```

### Comparing `flatnet-0.2.0/flatnet/modules/flatnet_nn.py` & `flatnet-0.2.1/flatnet/modules/flatnet_nn.py`

 * *Files identical despite different names*

### Comparing `flatnet-0.2.0/flatnet/train.py` & `flatnet-0.2.1/flatnet/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,31 +9,40 @@
 
 from .modules import flatnet_nn
 
 from tqdm import trange
 
 # for saving gifs
 import matplotlib.pyplot as plt
+from mpl_toolkits.mplot3d import Axes3D
 import imageio
 import os
+import atexit
+
+# delete temporary files if we exit too early
+def exit_handler():
+    if os.path.exists('flatnet_gif_frames'):
+        for file_name in os.listdir('flatnet_gif_frames'):
+            os.remove(os.path.join('flatnet_gif_frames', file_name))
+        os.rmdir('flatnet_gif_frames')
 
 # ****************************i*************************************************
 # This is the primary script for the curvature compression algorithm.
 # Input: data matrix X of shape (n,D), where D is the embedding dimension and
 # n is the number of data points;
 # d_desired is the desired dimension to flatten X onto
 
 # Output: a neural network f: R^D -> R^d, where d is the intrinsic dimension of
 # the data manifold X is drawn from.
 
 # gamma_0 is the starting value of the "inverse neighborhood size"
 # --- (the smaller gamma_0 is, the larger the neighborhood size is)
 
 def train(X,
-       n_stop_to_converge=5,  # how many times of no progress do we call convergence?
+       n_stop_to_converge=10,  # how many times of no progress do we call convergence?
        n_iter=500,  # number of flattening steps to perform
        n_iter_inner=1000,  # how many max steps for inner optimization of U, V
        thres_recon=1e-4,  # threshold for reconstruction loss being good enough
        alpha_max=0.5,  # global parameter for kernel
        r_dimcheck_coeff=0.15,  # # radius for checking dimension.
        max_error_dimcheck_ratio=0.3,  # max l0 error with respect to r_dimcheck to stop dimension search
        r_min_coeff=0.15,  # minimum allowed radius for each flattening
@@ -43,16 +52,16 @@
        save_gif = False, # whether to save gif of flattening process. currently only works for 2D data
        ):
     N, D = X.shape
     # needed for dist-to-gamma conversion
     log2 = float(np.log(2))
 
     # if save gif is set to true but data is not 2D, throw warning but continue running with save_gif = False
-    if save_gif and D != 2:
-        print("Warning: save_gif is set to True but data is not 2D. Setting save_gif to False")
+    if save_gif and not (D == 2 or D == 3):
+        print("Warning: save_gif is set to True but data is not 2D or 3D. Setting save_gif to False")
         save_gif = False
     #######	## HYPERPARAMETERS ####
     ##############################
 
     converge_counter = 0
 
     # used to define hyperparameters
@@ -85,21 +94,26 @@
     # decoder network
     g = flatnet_nn.FlatteningNetwork()
     Z = X.clone()
 
     ################### ANIMATION SAVING #################
 
     if save_gif:
+        # print out to user that we are creating a folder to save frames temporarily
+        print("NOTE: creating 'flatnet_gif_frames' directory to save frames temporarily. This directory will be deleted after the flattening process is complete and the gif is rendered.")
         # Ensure the 'flatnet_gif_frames' directory does not already exist
         if os.path.exists('flatnet_gif_frames'):
             raise Exception("The 'flatnet_gif_frames' directory already exists; to ensure this script does not damage your local files, please eiehter delete flatnet_gif_frames or move this script to a new directory and try again.")
 
         # Create the 'flatnet_gif_frames' directory
         os.makedirs('flatnet_gif_frames')
 
+        # now if we exit, we need to delete the temp files
+        atexit.register(exit_handler)
+
         # create array to store frames
         frames = []
 
     # ################ MAIN LOOP #########################
     with trange(n_iter, unit="iters") as pbar:
         for j in pbar:
             # if j % 20 == 0:
@@ -194,19 +208,26 @@
                 g.add_operation(g_layer)
                 d_prev = U.shape[1]
                 # only update representation if we add the layer
                 Z = Z_new.clone()
 
                 # save gif frame
                 if save_gif:
-                    fig, ax = plt.subplots()
-                    ax.scatter(Z[:, 0].detach().numpy(), Z[:, 1].detach().numpy())
-                    ax.axis('off')
-                    for spine in ax.spines.values():
-                        spine.set_visible(False)
+                    if D == 2:
+                        fig, ax = plt.subplots()
+                        ax.scatter(Z[:, 0].detach().numpy(), Z[:, 1].detach().numpy())
+                        ax.axis('off')
+                        for spine in ax.spines.values():
+                            spine.set_visible(False)
+                    elif D == 3:
+                        fig = plt.figure()
+                        ax = fig.add_subplot(111, projection='3d')
+                        ax.axis('off')
+                        ax.scatter(Z[:, 0].detach().numpy(), Z[:, 1].detach().numpy(), Z[:, 2].detach().numpy())
+                        
                     plt.savefig(f"flatnet_gif_frames/frame_{j}.png")
                     plt.close()
                     # save frame
                     frames.append(imageio.imread(f"flatnet_gif_frames/frame_{j}.png"))
 
             # with torch.no_grad():
             # 	recon_loss = 0.5*(g(Z) - X).pow(2).mean()
```

### Comparing `flatnet-0.2.0/flatnet.egg-info/PKG-INFO` & `flatnet-0.2.1/flatnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 Metadata-Version: 2.1
 Name: flatnet
-Version: 0.2.0
+Version: 0.2.1
 Summary: FlatNet implementation in PyTorch, from the paper "Representation Learning via Manifold Flattening and Reconstruction"
 Home-page: UNKNOWN
 Author: Michael Psenka
 Author-email: psenka@eecs.berkeley.edu
 Maintainer: ['Druv Pai <druvpai@berkeley.edu>', 'Vishal Raman <vraman@berkeley.edu>']
 License: UNKNOWN
 Description: This is a minimal pip package to allow easy deployment of FlatNets, a geometry-based neural autoencoder architecture that automatically builds its layers based on geometric properties of the dataset. See our paper, [Representation Learning via Manifold Flattening and Reconstruction](https://arxiv.org/abs/2305.01777), for more details, and [the Github repo](https://github.com/michael-psenka/manifold-linearization) for the code and example scripts & notebooks.
         
         Changelog
         =========
+        0.2.1 (2023-05-09)
+        ------------------
+        Features:
+        - Added support for 3D data for gif saving.
+        
         0.2.0 (2023-05-07)
         ------------------
         Features:
         - Added easy gif saving! If your data is 2D, you can now visualize how your data evolves with the manifold flow.
         
         0.1.4 (2023-05-06)
         ------------------
         Bug Fixes:
         - Remembered why I did not add normalization into main training file, now removed
         
         0.1.3 (2023-05-06)
         ------------------
         
         Bug Fixes:
-        - Added normalization of the input data
+        - Minor performance improvements on simple cases
         
         0.1.1 (2023-05-06)
         ------------------
         
         Features:
         - Added normalization of the input data
         
         0.1.0 (2022-12-31)
         ------------------
         
-        Initial release of flatnet!
+        - Initial release of flatnet!
         
         # Manifold Linearization for Representation Learning
         
         This is a research project focused on the automatic generation of autoencoders with minimal feature size, when the data is supported near an embedded submanifold. Using the geometric structure of the manifold, we can equivalently treat this problem as a manifold flattening problem when the manifold is flattenable[^1]. See our paper, [Representation Learning via Manifold Flattening and Reconstruction](https://arxiv.org/abs/2305.01777), for more details.
         
         [^1]: Geometric note: while flattenability is not general, there are some heuristic reasons we can motivate this assumption for real world data. For example, if a dataset permits a VAE-like autoencoder, where samples from the data distribution can be generated via a standard Gaussian in the latent space, then the samples lie close in probability to a flattenable manifold, as this VAE has constructed a single-chart atlas.
         
@@ -82,15 +87,15 @@
         
         Z = f(X).detach().numpy()
         
         plt.scatter(Z[:,0], Z[:,1])
         plt.show()
         ```
         
-        The script `flatnet.py` includes many example experiments to run FlatNet constructions on. To see an example experiment, simply run `python flatnet_test.py` in the main directory to see the flattening and reconstruction of a simple sine wave. Further experiments and options can be specified through command line arguments, managed through [tyro](https://github.com/brentyi/tyro); to see the full list of arguments, run `python flatnet_test.py --help`.
+        The script `flatnet_test.py` includes many example experiments to run FlatNet constructions on. To see an example experiment, simply run `python flatnet_test.py` in the main directory to see the flattening and reconstruction of a simple sine wave. Further experiments and options can be specified through command line arguments, managed through [tyro](https://github.com/brentyi/tyro); to see the full list of arguments, run `python flatnet_test.py --help`.
         
         
         ## Directory Structure
         
         - `flatnet_test.py`: main test script, as described in above section.
         - `flatnet/train.py`: contains the main FlatNet construction (training) code.
         - `flatnet/modules`: contains code for the neural network modules used in FlatNet.
```

### Comparing `flatnet-0.2.0/flatnet.egg-info/requires.txt` & `flatnet-0.2.1/flatnet.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flatnet-0.2.0/setup.py` & `flatnet-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 long_desc_init = 'This is a minimal pip package to allow easy deployment of FlatNets, a geometry-based neural autoencoder architecture that automatically builds its layers based on geometric properties of the dataset. See our paper, [Representation Learning via Manifold Flattening and Reconstruction](https://arxiv.org/abs/2305.01777), for more details, and [the Github repo](https://github.com/michael-psenka/manifold-linearization) for the code and example scripts & notebooks.'
 
 long_description = long_desc_init + "\n\n" + changelog + "\n\n" + long_description
 
 setup(
     name='flatnet',
-    version='0.2.0',
+    version='0.2.1',
     description='FlatNet implementation in PyTorch, from the paper \"Representation Learning via Manifold Flattening and Reconstruction\"',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Michael Psenka',
     author_email='psenka@eecs.berkeley.edu',
     maintainer=['Druv Pai <druvpai@berkeley.edu>', 'Vishal Raman <vraman@berkeley.edu>'],
     packages=find_packages(),
```

