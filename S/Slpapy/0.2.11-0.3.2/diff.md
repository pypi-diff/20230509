# Comparing `tmp/Slpapy-0.2.11.tar.gz` & `tmp/Slpapy-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.2.11.tar", last modified: Sat May  6 07:41:12 2023, max compression
+gzip compressed data, was "Slpapy-0.3.2.tar", last modified: Tue May  9 06:54:02 2023, max compression
```

## Comparing `Slpapy-0.2.11.tar` & `Slpapy-0.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 07:41:12.469996 Slpapy-0.2.11/
--rw-rw-rw-   0        0        0      160 2023-05-06 07:41:12.468999 Slpapy-0.2.11/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-06 07:41:12.440076 Slpapy-0.2.11/Slpapy/
--rw-rw-rw-   0        0        0     3178 2023-05-06 07:40:45.000000 Slpapy-0.2.11/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.2.11/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:41:12.467004 Slpapy-0.2.11/Slpapy/Spatial_map/
--rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.2.11/Slpapy/Spatial_map/Spatial_map.py
--rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.2.11/Slpapy/Spatial_map/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.2.11/Slpapy/Spatial_map/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.2.11/Slpapy/Spatial_map/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.2.11/Slpapy/Spatial_map/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.2.11/Slpapy/Spatial_map/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.2.11/Slpapy/Spatial_map/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.2.11/Slpapy/Spatial_map/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.2.11/Slpapy/Spatial_map/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.2.11/Slpapy/Spatial_map/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.2.11/Slpapy/Spatial_map/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.2.11/Slpapy/Spatial_map/readwrite.py
--rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.2.11/Slpapy/Spatial_map/scatterplots.py
--rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.2.11/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5266 2023-05-06 04:33:53.000000 Slpapy-0.2.11/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-06 07:41:12.447057 Slpapy-0.2.11/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      160 2023-05-06 07:41:12.000000 Slpapy-0.2.11/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-05-06 07:41:12.000000 Slpapy-0.2.11/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 07:41:12.000000 Slpapy-0.2.11/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-05-06 07:41:12.000000 Slpapy-0.2.11/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-06 07:41:12.000000 Slpapy-0.2.11/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 07:41:12.469996 Slpapy-0.2.11/setup.cfg
--rw-rw-rw-   0        0        0      485 2023-05-06 07:40:58.000000 Slpapy-0.2.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:54:02.973240 Slpapy-0.3.2/
+-rw-rw-rw-   0        0        0      159 2023-05-09 06:54:02.973240 Slpapy-0.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 06:54:02.931424 Slpapy-0.3.2/Slpapy/
+-rw-rw-rw-   0        0        0     3178 2023-05-06 07:40:45.000000 Slpapy-0.3.2/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.3.2/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:54:02.970248 Slpapy-0.3.2/Slpapy/Spatial_map/
+-rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.3.2/Slpapy/Spatial_map/Spatial_map.py
+-rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.3.2/Slpapy/Spatial_map/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.3.2/Slpapy/Spatial_map/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.3.2/Slpapy/Spatial_map/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.3.2/Slpapy/Spatial_map/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.3.2/Slpapy/Spatial_map/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.3.2/Slpapy/Spatial_map/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.3.2/Slpapy/Spatial_map/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.3.2/Slpapy/Spatial_map/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.3.2/Slpapy/Spatial_map/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.3.2/Slpapy/Spatial_map/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.3.2/Slpapy/Spatial_map/readwrite.py
+-rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.3.2/Slpapy/Spatial_map/scatterplots.py
+-rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.3.2/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5812 2023-05-09 06:48:17.000000 Slpapy-0.3.2/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-09 06:54:02.941398 Slpapy-0.3.2/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-05-09 06:54:02.000000 Slpapy-0.3.2/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-05-09 06:54:02.000000 Slpapy-0.3.2/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 06:54:02.000000 Slpapy-0.3.2/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-05-09 06:54:02.000000 Slpapy-0.3.2/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-09 06:54:02.000000 Slpapy-0.3.2/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-09 06:54:02.974237 Slpapy-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      484 2023-05-09 06:53:57.000000 Slpapy-0.3.2/setup.py
```

### Comparing `Slpapy-0.2.11/Slpapy/Data_reconstruction.py` & `Slpapy-0.3.2/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/MZ_ppm_match.py` & `Slpapy-0.3.2/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/Spatial_map/_compat.py` & `Slpapy-0.3.2/Slpapy/Spatial_map/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/Spatial_map/_docs.py` & `Slpapy-0.3.2/Slpapy/Spatial_map/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/Spatial_map/_rcmod.py` & `Slpapy-0.3.2/Slpapy/Spatial_map/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/Spatial_map/_settings.py` & `Slpapy-0.3.2/Slpapy/Spatial_map/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/Spatial_map/_utils.py` & `Slpapy-0.3.2/Slpapy/Spatial_map/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/Spatial_map/beats.py` & `Slpapy-0.3.2/Slpapy/Spatial_map/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/Spatial_map/is_constant.py` & `Slpapy-0.3.2/Slpapy/Spatial_map/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/Spatial_map/logging.py` & `Slpapy-0.3.2/Slpapy/Spatial_map/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/Spatial_map/palettes.py` & `Slpapy-0.3.2/Slpapy/Spatial_map/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/Spatial_map/readwrite.py` & `Slpapy-0.3.2/Slpapy/Spatial_map/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/Spatial_map/scatterplots.py` & `Slpapy-0.3.2/Slpapy/Spatial_map/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.11/Slpapy/processing_analyze.py` & `Slpapy-0.3.2/Slpapy/processing_analyze.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from typing import Optional
+
 import anndata as ad
+import numpy as np
+import pandas as pd
 import scanpy as sc
 from scipy.sparse import csr_matrix
 from sklearn import preprocessing
 from sklearn.cluster import KMeans
-import numpy as np
-from typing import Optional
+
 from .Spatial_map import Spatial_map
+
 sc.settings.verbosity = 3  # 设置日志等级: errors (0), warnings (1), info (2), hints (3)
 sc.logging.print_header()
 sc.settings.set_figure_params(dpi=720, facecolor='white')
 
 
-
-
 def XYadata(adata):
     df = preprocessing.normalize(np.c_[np.array(adata.obs['X']), np.array(adata.obs['Y'])])
     counts = csr_matrix(df, dtype=np.float32)
     XYmatrix = ad.AnnData(counts)
     # 为x和y轴提供索引
     XYmatrix.obs_names = adata.obs_names
     XYmatrix.var_names = ['X', 'Y']
@@ -24,15 +26,15 @@
     adata = ad.concat([adata, XYmatrix], axis=1)
     adata.obs = t
     adata.obsm['X_spacial'] = np.array(adata.obs.loc[:, 'X':'Y'])
     print('Space integration complete')
     return adata
 
 
-def pp_analyze(adata,onlyhighly):
+def pp_analyze(adata, onlyhighly):
     # 显示在所有细胞中在每个单细胞中产生最高计数分数的脂质
     # sc.pl.highest_expr_genes(adata, n_top=20, save='_highest_expr_protein.png')
     # 小提琴图：表达基因的数量，每个细胞包含的表达量，线粒体基因表达量的百分比。
     adata.var['mt'] = adata.var_names.str.startswith('MT-')  # 将线粒体基因标记为 mt
     sc.pp.calculate_qc_metrics(adata, qc_vars=['mt'], percent_top=None,
                                log1p=False, inplace=True)
     sc.pl.violin(adata, 'total_counts', jitter=0.4, multi_panel=True,
@@ -40,88 +42,92 @@
     adata = adata[adata.obs['total_counts'] != 0, :]
     # 归一化，使得不同细胞样本间可比
     sc.pp.normalize_total(adata, target_sum=1e4)
     sc.pp.log1p(adata)
     # 存储数据
     adata.raw = adata
     # 选择高变异基因
-    if onlyhighly==True:
+    if onlyhighly == True:
         sc.pp.highly_variable_genes(adata, min_mean=0.0125, max_mean=3, min_disp=0.5)
         sc.pl.highly_variable_genes(adata, save='_highly_variable_lipid.png')
         adata = adata[:, adata.var.highly_variable]
     adata.obsm['X_spacial'] = np.array(adata.obs.loc[:, 'X':'Y'])
     # 回归每个细胞的总计数和表达的线粒体基因的百分比的影响。
     sc.pp.regress_out(adata, ['total_counts', 'pct_counts_mt'])
-    #保存mz值
+    # 保存mz值
     mz = adata.var
     mz.to_csv('./mz.csv')
     adata.write('./pp_done.h5ad')
     return adata
 
 
-def se_analyze(adata, n_neighbors, n_pcs,resolution):
+def se_analyze(adata, n_neighbors, n_pcs, resolution):
     # 将每个脂质缩放到单位方差。阈值超过标准偏差 10。，如非高斯分布，则不建议使用
-    #sc.pp.scale(adata, max_value=10)
+    # sc.pp.scale(adata, max_value=10)
     # 绘制 PCA 图降维
     sc.tl.pca(adata, svd_solver='arpack')  #
     # Neighborhood graph使用数据矩阵的 PCA 表示来计算细胞的邻域图
     sc.pp.neighbors(adata, n_neighbors=n_neighbors, n_pcs=n_pcs, )
     sc.tl.umap(adata, min_dist=0.01, alpha=1, spread=2)  #
     # Leiden 图聚类
     # 计算
     sc.tl.leiden(adata, resolution=resolution)
     return adata
 
 
-
+def third_analyze(adata):
+    sc.pl.pca_variance_ratio(adata, log=True, save='_spacial.png')
+    sc.pl.umap(adata, color=['leiden'], save='_spacial.png')
+    sc.tl.rank_genes_groups(adata, 'leiden', method='wilcoxon')
+    result = adata.uns['rank_genes_groups']
+    groups = result['names'].dtype.names
+    res = pd.DataFrame({group + '_' + key: result[key][group] for group in groups for key in
+                        ['names', 'pvals', 'logfoldchanges', 'pvals_adj', 'scores']})
+    res.to_csv("dif.csv")
+    sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_Wilcoxon.png')
+    sc.pl.rank_genes_groups_violin(adata, n_genes=25, sharey=False, dendrogram=True, save='_violin_Wilcoxon.png')
+    return adata
 
 
 def Basic_processing_flow(
         adata: ad.AnnData,
         *,
         use_spacial: bool = False,
         orgknn: bool = False,
         onlyhighly: bool = False,
-        n_neighbors: int =20,
-        n_pcs: int =30,
-        resolution: int =0.8
+        n_neighbors: int = 20,
+        n_pcs: int = 30,
+        resolution: int = 0.8
 
 ) -> Optional[ad.AnnData]:
-    adata = pp_analyze(adata,onlyhighly)
+    adata = pp_analyze(adata, onlyhighly)
     if use_spacial == True:
         adata = XYadata(adata)
         adata = se_analyze(adata, n_neighbors, n_pcs, resolution)
-        sc.pl.pca_variance_ratio(adata, log=True, save='_spacial.png')
-        sc.pl.umap(adata, color=['leiden'], save='_spacial.png')
-        sc.tl.rank_genes_groups(adata, 'leiden', method='wilcoxon')
-        sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_spacial_Wilcoxon.png')
+        adata = third_analyze(adata)
         adata.obs['leidenXY'] = adata.obs['leiden']
         Spatial_map(adata, 'leidenXY')
     else:
         adata = se_analyze(adata, n_neighbors, n_pcs, resolution)
-        sc.pl.pca_variance_ratio(adata, log=True, save='_general.png')
-        sc.pl.umap(adata, color=['leiden'], save='_general.png')
-        sc.tl.rank_genes_groups(adata, 'leiden', method='wilcoxon')
-        sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_Wilcoxon.png')
+        adata = third_analyze(adata)
         Spatial_map(adata, 'leiden')
 
     if orgknn == True:
         adata = se_analyze(adata, n_neighbors, n_pcs, resolution)
         estimator = KMeans(n_clusters=adata.obs['leiden'].values.codes.max() + 1)  # 构造聚类器
         estimator.fit(
             np.c_[adata.X, preprocessing.normalize(np.c_[np.array(adata.obs['X']), np.array(adata.obs['Y'])])])
         label_pred = estimator.labels_  # 获取聚类标签
         adata.obs['KNNlableXY'] = label_pred.T
         adata.obs['KNNlableXY'] = adata.obs['KNNlableXY'].astype('category')
         sc.tl.rank_genes_groups(adata, 'KNNlableXY', method='wilcoxon')
         sc.pl.rank_genes_groups(adata, n_genes=25, sharey=False, save='_KXY_Wilcoxon.png')
+        result = adata.uns['rank_genes_groups']
+        groups = result['names'].dtype.names
+        res = pd.DataFrame({group + '_' + key: result[key][group] for group in groups for key in
+                            ['names', 'pvals', 'logfoldchanges', 'pvals_adj', 'scores']})
+        res.to_csv("dif.csv")
         sc.pl.pca_variance_ratio(adata, log=True, save='_KXY.png')
         sc.pl.umap(adata, color=['KNNlableXY'], save='_KXY.png')
         Spatial_map(adata, 'KNNlableXY')
     adata.write('./analyze_done.h5ad')
     return adata
-
-
-
-
-
-
```

### Comparing `Slpapy-0.2.11/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.3.2/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

