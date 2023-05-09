# Comparing `tmp/chromoformer-1.1.0.tar.gz` & `tmp/chromoformer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromoformer-1.1.0.tar", last modified: Fri Apr 14 05:26:22 2023, max compression
+gzip compressed data, was "chromoformer-1.1.1.tar", last modified: Tue May  9 05:54:16 2023, max compression
```

## Comparing `chromoformer-1.1.0.tar` & `chromoformer-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:26:22.248506 chromoformer-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 05:26:08.000000 chromoformer-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-14 05:26:22.248506 chromoformer-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-04-14 05:26:08.000000 chromoformer-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:26:22.248506 chromoformer-1.1.0/chromoformer/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 05:26:08.000000 chromoformer-1.1.0/chromoformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-14 05:26:08.000000 chromoformer-1.1.0/chromoformer/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-04-14 05:26:08.000000 chromoformer-1.1.0/chromoformer/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-04-14 05:26:08.000000 chromoformer-1.1.0/chromoformer/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-14 05:26:08.000000 chromoformer-1.1.0/chromoformer/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-14 05:26:08.000000 chromoformer-1.1.0/chromoformer/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 05:26:22.248506 chromoformer-1.1.0/chromoformer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-14 05:26:22.000000 chromoformer-1.1.0/chromoformer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-14 05:26:22.000000 chromoformer-1.1.0/chromoformer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 05:26:22.000000 chromoformer-1.1.0/chromoformer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-14 05:26:22.000000 chromoformer-1.1.0/chromoformer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-14 05:26:22.000000 chromoformer-1.1.0/chromoformer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 05:26:22.248506 chromoformer-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-04-14 05:26:09.000000 chromoformer-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:54:16.289229 chromoformer-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-09 05:54:00.000000 chromoformer-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-09 05:54:16.289229 chromoformer-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-09 05:54:00.000000 chromoformer-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:54:16.285229 chromoformer-1.1.1/chromoformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-09 05:54:00.000000 chromoformer-1.1.1/chromoformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-05-09 05:54:00.000000 chromoformer-1.1.1/chromoformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-05-09 05:54:00.000000 chromoformer-1.1.1/chromoformer/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-05-09 05:54:00.000000 chromoformer-1.1.1/chromoformer/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-05-09 05:54:00.000000 chromoformer-1.1.1/chromoformer/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-09 05:54:00.000000 chromoformer-1.1.1/chromoformer/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 05:54:16.289229 chromoformer-1.1.1/chromoformer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-09 05:54:16.000000 chromoformer-1.1.1/chromoformer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-09 05:54:16.000000 chromoformer-1.1.1/chromoformer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 05:54:16.000000 chromoformer-1.1.1/chromoformer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 05:54:16.000000 chromoformer-1.1.1/chromoformer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-09 05:54:16.000000 chromoformer-1.1.1/chromoformer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 05:54:16.289229 chromoformer-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-09 05:54:01.000000 chromoformer-1.1.1/setup.py
```

### Comparing `chromoformer-1.1.0/LICENSE` & `chromoformer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chromoformer-1.1.0/PKG-INFO` & `chromoformer-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromoformer
-Version: 1.1.0
+Version: 1.1.1
 Summary: Chromoformer - Pytorch
 Home-page: https://github.com/dohlee/chromoformer
 Author: Dohoon Lee
 Author-email: dohlee.bioinfo@gmail.com
 License: MIT
 Keywords: artificial intelligence,epigenomics,gene expression prediction
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chromoformer-1.1.0/README.md` & `chromoformer-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Chromoformer
 
 ![banner](img/chromoformer_banner_small.png)
 
 [![DOI](https://zenodo.org/badge/432363545.svg)](https://zenodo.org/badge/latestdoi/432363545)
+[![PyPI version](https://badge.fury.io/py/chromoformer.svg)](https://badge.fury.io/py/chromoformer)
 
 This repository provides the official code implementations for Chromoformer.
 
 We also provide our pipelines for preprocessing input data and training Chromoformer model to help researchers reproduce the results and extend the study with their own data.
 The repository includes two directories: `preprocessing` and `chromoformer`.
 
 Refer to the directory named [`preprocessing`](preprocessing) to explore how we preprocessed the ChIP-seq signals and gene expression data for 11 cell lines from [Roadmap Epigenomics Project](http://www.roadmapepigenomics.org). We provide the whole preprocessing workflow from raw ChIP-seq reads to processed read depth signals for training as a one-shot `snakemake` pipeline. One can easily extend the pipeline for other cell types or other histone marks by slightly tweaking the parameters.
@@ -98,19 +99,17 @@
 |strand|Direction of transcription. '+' for forward and '-' for reverse.|*+*|
 |split|Group label for cross-validation. Note that we must use chromosomal split to avoid information leak during performance evaulation (i.e., no two genes in train/val set are on the same chromosome).|*0*|
 |neighbors|A list of genomic regions interacting with the promoter. Should be joined by ';'|*chr1:14589068-14595292;chr1:13973835-13979555*|
 |scores|Normalized interaction frequencies for each neghbor in `neighbors` columns. Should be joined by ';'|*1.5494*|
 
 ## Pretrained weights
 
-*NOTE: Due to the recent update, the names of pretrained weights at the moment may not match with the paramters of ChromoformerClassifier and ChromoformerRegressor model, so you cannot directly use them. We will fix this issue soon.*
+[![pretrained_weights_doi](https://img.shields.io/badge/doi-10.6084%2Fm9.figshare.19424807.v4-blue)](https://doi.org/10.6084/m9.figshare.19424807.v4)
 
-![pretrained_weights_doi](https://img.shields.io/badge/doi-10.6084%2Fm9.figshare.19424807.v1-blue)
-
-Pretrained weights for Chromoformer models are available at https://doi.org/10.6084/m9.figshare.19424807.v1.
+Pretrained weights for Chromoformer models (for Chromoformer-clf and Chromoformer-reg) are available at https://doi.org/10.6084/m9.figshare.19424807.v4.
 Models were individually trained for 11 cell types from Roadmap Epigenomics Project. For each cell type, 18955 protein coding genes were divided into four non-overlapping cross-validation (CV) sets, and trained weights for each cross-validation fold is provided in this dataset.
 
 The directory is organized firstly by Roadmap Epigenomics cell type (using corresponding EID), and four `pytorch` checkpoint files (a `.pt` file for each CV-fold) are placed in each directory.
 
 `*.pt` files are basically dictionaries containing pretrained weights as well as some training details associated with the following keys:
 
 - `net` : Pretrained weights.
```

### Comparing `chromoformer-1.1.0/chromoformer/data.py` & `chromoformer-1.1.1/chromoformer/data.py`

 * *Files identical despite different names*

### Comparing `chromoformer-1.1.0/chromoformer/modules.py` & `chromoformer-1.1.1/chromoformer/modules.py`

 * *Files identical despite different names*

### Comparing `chromoformer-1.1.0/chromoformer/net.py` & `chromoformer-1.1.1/chromoformer/net.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,7 +547,13 @@
     print(out_classifier.sum())
     print(out_classifier.shape)
     # -3.1917, [8, 2]
 
     print(out_regressor.sum())
     print(out_regressor.shape)
     # -0.1900, [8, 1]
+
+    # ckpt = torch.load("test.pt")
+    # model_classifier.load_state_dict(ckpt["net"])
+
+    ckpt = torch.load('converted/E003/chromoformer-reg-reproduction-E003-conf1-fold1.pt')
+    model_regressor.load_state_dict(ckpt["net"])
```

### Comparing `chromoformer-1.1.0/chromoformer/train.py` & `chromoformer-1.1.1/chromoformer/train.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import torch.nn as nn
 import os
 import pandas as pd
 import wandb
 import yaml
 
 from tqdm import tqdm
+from scipy import stats
 from sklearn import metrics
 
 from .data import ChromoformerDataset
 from .net import ChromoformerClassifier, ChromoformerRegressor
 from .util import seed_everything
 
 
@@ -142,22 +143,21 @@
     regulation_kws,
     binsizes=args.binsizes,
     seed=42,
 )
 
 model.cuda()
 
-criterion = nn.CrossEntropyLoss()
+criterion = nn.MSELoss() if args.regression else nn.CrossEntropyLoss()
 optimizer = torch.optim.AdamW(model.parameters(), lr=float(config["lr"]))
 scheduler = torch.optim.lr_scheduler.StepLR(optimizer, step_size=1, gamma=gamma)
 
 optimizer.zero_grad()
 optimizer.step()
 
-best_val_auc = 0
 for epoch in range(1, num_epoch):
     # Prepare train.
     bar = tqdm(enumerate(train_loader, 1), total=len(train_loader))
     running_loss = 0.0
     train_out, train_label = [], []
 
     # Train.
@@ -192,37 +192,56 @@
         train_out.append(out.detach().cpu())
         train_label.append(d["label"].cpu())
 
         if batch % 10 == 0:
             batch_loss = running_loss / 10.0
 
             train_out, train_label = map(torch.cat, (train_out, train_label))
-            train_score = train_out.softmax(axis=1)[:, 1]
-            train_pred = train_out.argmax(axis=1)
 
-            batch_acc = metrics.accuracy_score(train_label, train_pred) * 100
-            batch_auc = metrics.roc_auc_score(train_label, train_score) * 100
-            batch_ap = metrics.average_precision_score(train_label, train_score) * 100
+            if args.regression:
+                train_pred = train_out.flatten()
 
-            bar.set_description(
-                f"E{epoch} {batch_loss:.4f}, lr={get_lr(optimizer)}, acc={batch_acc:.4f}, auc={batch_auc:.4f}, ap={batch_ap:.4f}"
-            )
+                batch_r2 = metrics.r2_score(train_label, train_pred) * 100
+                batch_r = stats.pearsonr(train_label, train_pred)[0] * 100
+
+                bar.set_description(
+                    f"E{epoch} {batch_loss:.4f}, lr={get_lr(optimizer)}, r2={batch_r2:.4f}, r={batch_r:.4f}"
+                )
+
+                wandb.log(
+                    {
+                        "train/loss": batch_loss,
+                        "train/r2": batch_r2,
+                        "train/r": batch_r,
+                    }
+                )
+            else:
+                train_score = train_out.softmax(axis=1)[:, 1]
+                train_pred = train_out.argmax(axis=1)
+
+                batch_acc = metrics.accuracy_score(train_label, train_pred) * 100
+                batch_auc = metrics.roc_auc_score(train_label, train_score) * 100
+                batch_ap = metrics.average_precision_score(train_label, train_score) * 100
+
+                bar.set_description(
+                    f"E{epoch} {batch_loss:.4f}, lr={get_lr(optimizer)}, acc={batch_acc:.4f}, auc={batch_auc:.4f}, ap={batch_ap:.4f}"
+                )
+
+                wandb.log(
+                    {
+                        "train/loss": batch_loss,
+                        "train/acc": batch_acc,
+                        "train/auc": batch_auc,
+                        "train/ap": batch_ap,
+                    }
+                )
 
             running_loss = 0.0
             train_out, train_label = [], []
 
-            wandb.log(
-                {
-                    "train/loss": batch_loss,
-                    "train/acc": batch_acc,
-                    "train/auc": batch_auc,
-                    "train/ap": batch_ap,
-                }
-            )
-
     # Prepare validation.
     bar = tqdm(enumerate(val_loader, 1), total=len(val_loader))
     val_out, val_label = [], []
 
     # Validation.
     model.eval()
     with torch.no_grad():
@@ -249,44 +268,80 @@
     val_out = torch.cat(val_out)
     val_label = torch.cat(val_label)
 
     val_loss = criterion(val_out, val_label)
 
     # Metrics.
     val_label = val_label.numpy()
-    val_score = val_out.softmax(axis=1)[:, 1].numpy()
-    val_pred = val_out.argmax(axis=1).numpy()
+    if args.regression:
+        val_score = val_out.flatten().numpy()
 
-    val_acc = metrics.accuracy_score(val_label, val_pred) * 100
-    val_auc = metrics.roc_auc_score(val_label, val_score) * 100
-    val_ap = metrics.average_precision_score(val_label, val_score) * 100
+        val_r2 = metrics.r2_score(val_label, val_score) * 100
+        val_r = stats.pearsonr(val_label, val_score)[0] * 100
 
-    print(f"Validation loss={val_loss:.4f}, acc={val_acc:.4f}, auc={val_auc:.4f}, ap={val_ap:.4f}")
+        print(f"Validation loss={val_loss:.4f}, r2={val_r2:.4f}, r={val_r:.4f}")
+        wandb.log(
+            {
+                "val/loss": val_loss,
+                "val/r2": val_r2,
+                "val/r": val_r,
+            }
+        )
+    else:
+        val_score = val_out.softmax(axis=1)[:, 1].numpy()
+        val_pred = val_out.argmax(axis=1).numpy()
+
+        val_acc = metrics.accuracy_score(val_label, val_pred) * 100
+        val_auc = metrics.roc_auc_score(val_label, val_score) * 100
+        val_ap = metrics.average_precision_score(val_label, val_score) * 100
 
-    wandb.log(
-        {
-            "val/loss": val_loss,
-            "val/acc": val_acc,
-            "val/auc": val_auc,
-            "val/ap": val_ap,
-            "val/epoch": epoch,
-        }
-    )
+        print(
+            f"Validation loss={val_loss:.4f}, acc={val_acc:.4f}, auc={val_auc:.4f}, ap={val_ap:.4f}"
+        )
+        wandb.log(
+            {
+                "val/loss": val_loss,
+                "val/acc": val_acc,
+                "val/auc": val_auc,
+                "val/ap": val_ap,
+                "val/epoch": epoch,
+            }
+        )
 
-    ckpt = {
-        "net": model.state_dict(),
-        "optimizer": optimizer.state_dict(),
-        "epoch": epoch,
-        "last_val_loss": val_loss,
-        "last_val_auc": val_auc,
-        "val_score": val_score,
-        "val_label": val_label,
-    }
-    torch.save(ckpt, args.output)
+    if args.regression:
+        ckpt = {
+            "net": model.state_dict(),
+            "optimizer": optimizer.state_dict(),
+            "epoch": epoch,
+            "last_val_loss": val_loss,
+            "last_val_r2": val_r2,
+            "val_score": val_score,
+            "val_label": val_label,
+        }
+        torch.save(ckpt, args.output)
+    else:
+        ckpt = {
+            "net": model.state_dict(),
+            "optimizer": optimizer.state_dict(),
+            "epoch": epoch,
+            "last_val_loss": val_loss,
+            "last_val_auc": val_auc,
+            "val_score": val_score,
+            "val_label": val_label,
+        }
+        torch.save(ckpt, args.output)
     scheduler.step()
 
-wandb.summary.update(
-    {
-        "last_val_loss": val_loss,
-        "last_val_auc": val_auc,
-    }
-)
+if args.regression:
+    wandb.summary.update(
+        {
+            "last_val_loss": val_loss,
+            "last_val_r2": val_r2,
+        }
+    )
+else:
+    wandb.summary.update(
+        {
+            "last_val_loss": val_loss,
+            "last_val_auc": val_auc,
+        }
+    )
```

### Comparing `chromoformer-1.1.0/chromoformer.egg-info/PKG-INFO` & `chromoformer-1.1.1/chromoformer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromoformer
-Version: 1.1.0
+Version: 1.1.1
 Summary: Chromoformer - Pytorch
 Home-page: https://github.com/dohlee/chromoformer
 Author: Dohoon Lee
 Author-email: dohlee.bioinfo@gmail.com
 License: MIT
 Keywords: artificial intelligence,epigenomics,gene expression prediction
 Classifier: Development Status :: 4 - Beta
```

### Comparing `chromoformer-1.1.0/setup.py` & `chromoformer-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name="chromoformer",
     packages=find_packages(exclude=[]),
     include_package_data=True,
-    version="1.1.0",
+    version="1.1.1",
     license="MIT",
     description="Chromoformer - Pytorch",
     author="Dohoon Lee",
     author_email="dohlee.bioinfo@gmail.com",
     long_description_content_type="text/markdown",
     url="https://github.com/dohlee/chromoformer",
     keywords=[
```

