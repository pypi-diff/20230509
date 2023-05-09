# Comparing `tmp/unpast-0.1.1.tar.gz` & `tmp/unpast-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unpast-0.1.1.tar", max compression
+gzip compressed data, was "unpast-0.1.2.tar", max compression
```

## Comparing `unpast-0.1.1.tar` & `unpast-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-05-08 14:23:44.608899 unpast-0.1.1/LICENSE
--rw-r--r--   0        0        0     4217 2023-05-09 13:15:04.367747 unpast-0.1.1/README.md
--rw-r--r--   0        0        0      666 2023-05-09 13:16:05.364315 unpast-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-08 14:23:44.608899 unpast-0.1.1/unpast/__init__.py
--rw-r--r--   0        0        0      770 2023-05-09 09:50:39.120334 unpast-0.1.1/unpast/install_r_dependencies.py
--rw-r--r--   0        0        0    36567 2023-05-08 14:23:44.716900 unpast-0.1.1/unpast/method.py
--rwxr-xr-x   0        0        0    12107 2023-05-09 12:58:02.266229 unpast-0.1.1/unpast/run_unpast.py
--rw-r--r--   0        0        0        0 2023-05-08 15:54:16.915484 unpast-0.1.1/unpast/utils/.Rhistory
--rw-r--r--   0        0        0        0 2023-05-08 14:23:44.768901 unpast-0.1.1/unpast/utils/__init__.py
--rw-r--r--   0        0        0      163 2023-05-09 10:32:43.215838 unpast-0.1.1/unpast/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      163 2023-05-08 15:31:35.482806 unpast-0.1.1/unpast/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    33597 2023-05-09 10:32:43.219838 unpast-0.1.1/unpast/utils/__pycache__/method.cpython-38.pyc
--rw-r--r--   0        0        0    33532 2023-05-08 15:31:35.490806 unpast-0.1.1/unpast/utils/__pycache__/method.cpython-39.pyc
--rw-r--r--   0        0        0    25724 2023-05-08 14:23:44.768901 unpast-0.1.1/unpast/utils/eval.py
--rw-r--r--   0        0        0    57918 2023-05-08 14:23:44.768901 unpast-0.1.1/unpast/utils/method.py
--rw-r--r--   0        0        0    19957 2023-05-08 14:23:44.768901 unpast-0.1.1/unpast/utils/pgm.py
--rw-r--r--   0        0        0     1757 2023-05-08 14:23:44.768901 unpast-0.1.1/unpast/utils/run_WGCNA.R
--rw-r--r--   0        0        0     5300 1970-01-01 00:00:00.000000 unpast-0.1.1/setup.py
--rw-r--r--   0        0        0     4985 1970-01-01 00:00:00.000000 unpast-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-08 14:23:44.608899 unpast-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4626 2023-05-09 15:53:28.200244 unpast-0.1.2/README.md
+-rw-r--r--   0        0        0      666 2023-05-09 15:55:48.957555 unpast-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-08 14:23:44.608899 unpast-0.1.2/unpast/__init__.py
+-rw-r--r--   0        0        0      815 2023-05-09 13:58:10.515828 unpast-0.1.2/unpast/install_r_dependencies.py
+-rw-r--r--   0        0        0    36567 2023-05-08 14:23:44.716900 unpast-0.1.2/unpast/method.py
+-rw-r--r--   0        0        0   336886 2023-05-08 14:23:44.716900 unpast-0.1.2/unpast/poster/DESMOND2.pdf
+-rw-r--r--   0        0        0  1125210 2023-05-08 14:23:44.724900 unpast-0.1.2/unpast/poster/DESMOND2.png
+-rw-r--r--   0        0        0  8345012 2023-05-08 14:23:44.764901 unpast-0.1.2/unpast/poster/DESMOND2_poster_v5.png
+-rw-r--r--   0        0        0   325387 2023-05-08 14:23:44.764901 unpast-0.1.2/unpast/poster/DESMOND2_steps2.png
+-rwxr-xr-x   0        0        0    12107 2023-05-09 12:58:02.266229 unpast-0.1.2/unpast/run_unpast.py
+-rw-r--r--   0        0        0        0 2023-05-08 15:54:16.915484 unpast-0.1.2/unpast/utils/.Rhistory
+-rw-r--r--   0        0        0        0 2023-05-08 14:23:44.768901 unpast-0.1.2/unpast/utils/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-09 10:32:43.215838 unpast-0.1.2/unpast/utils/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      163 2023-05-08 15:31:35.482806 unpast-0.1.2/unpast/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    33597 2023-05-09 10:32:43.219838 unpast-0.1.2/unpast/utils/__pycache__/method.cpython-38.pyc
+-rw-r--r--   0        0        0    33532 2023-05-08 15:31:35.490806 unpast-0.1.2/unpast/utils/__pycache__/method.cpython-39.pyc
+-rw-r--r--   0        0        0    25724 2023-05-08 14:23:44.768901 unpast-0.1.2/unpast/utils/eval.py
+-rw-r--r--   0        0        0    57918 2023-05-08 14:23:44.768901 unpast-0.1.2/unpast/utils/method.py
+-rw-r--r--   0        0        0    19957 2023-05-08 14:23:44.768901 unpast-0.1.2/unpast/utils/pgm.py
+-rw-r--r--   0        0        0     1757 2023-05-08 14:23:44.768901 unpast-0.1.2/unpast/utils/run_WGCNA.R
+-rw-r--r--   0        0        0     5730 1970-01-01 00:00:00.000000 unpast-0.1.2/setup.py
+-rw-r--r--   0        0        0     5394 1970-01-01 00:00:00.000000 unpast-0.1.2/PKG-INFO
```

### Comparing `unpast-0.1.1/LICENSE` & `unpast-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unpast-0.1.1/README.md` & `unpast-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,64 +25,57 @@
 
 R:
     WGCNA==1.70-3
 </pre>
 
 ## Installation
 This UnPaSt can be installed using `pip`, `poetry`, run using `Docker`, or a script (see examples section). Follow the appropriate instructions below for your preferred method.
+You need to have R and Python 3.8 installed.
 
-1. Using pip:
-
-To install the project using `pip`, first make sure you have `pip` installed on your system. If you haven't installed it already, you can find the installation instructions [here](https://pip.pypa.io/en/stable/installation/).
-
+1. Using pip: \
+To install the project using `pip`, first make sure you have `pip` installed on your system. If you haven't installed it already, you can find the installation instructions [here](https://pip.pypa.io/en/stable/installation/). \
 Once `pip` is installed, you can install the project by running the following command:
 ```bash
 pip install unpast
 ```
-
 Run it:
 ```bash
 run_unpast -h
 ```
-
-2. Installation using Poetry
-To install the package using Poetry, first make sure you have Poetry installed, and then run:
-
+**Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:
+```bash
+python -m unpast.install_r_dependencies
+```
+2. Installation using Poetry: \
+To install the package using Poetry, first make sure you have Poetry installed, clone the repo and then run:
 ```bash
 poetry add unpast
 ```
 Run it:
 ```bash
 poetry run run_unpast -h
 ```
-
-3. Running with Docker
-You can also run the package using Docker. First, pull the Docker image:
-
+**Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:
 ```bash
-docker pull my_docker_hub_user/unpast:latest
+poetry run python -m unpast.install_r_dependencies
 ```
-Next, run the container:
-
+3. Running with Docker: \
+You can also run the package using Docker. First, pull the Docker image:
 ```bash
-docker run -it --rm -v you/data/path/:/user_data/ freddsle/unpast:latest run_unpast -h
+docker pull freddsle/unpast:version0.1
 ```
-
-**Dependencies**
-
-To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:
-
+Next, run the container:
 ```bash
-python3 -m unpast.install_r_dependencies
+docker run -v /your/data/path/:/user_data/ freddsle/unpast:version0.1 --exprs /user_data/exprs.tsv --out_dir /user_data/out_dir/
 ```
 
 ## Examples
 * UnPaSt requires a tab-separated file with standardized expressions of genes (or transcripts) in rows, and samples in columns. Gene and sample names must be unique. 
 * A subset of 200 randomly chosen samples from TCGA-BRCA and UnPaSt output:
-[test data](https://drive.google.com/file/d/1GXR_1ErIPtQkEOxE66at0uqQN76qNG7a/view?usp=sharing)
+[test data](https://unpast-backend.zbh.uni-hamburg.de/download_example)
 
 <pre>
 # running UnPaSt with default parameters and example data
 python ./unpast/run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename TCGA_200_results
 
 # with different binarization and clustering methods
 python ./unpast/run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename results --binarization ward --clustering WGCNA
```

### Comparing `unpast-0.1.1/pyproject.toml` & `unpast-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unpast"
-version = "0.1.1"
+version = "0.1.2"
 description = "A novel method for unsupervised patient stratification."
 authors = []
 readme = "README.md"
 license = "GPL-3.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.9"
```

### Comparing `unpast-0.1.1/unpast/install_r_dependencies.py` & `unpast-0.1.2/unpast/install_r_dependencies.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
         subprocess.run(["R", "--version"], check=True, capture_output=True)
         return True
     except FileNotFoundError:
         print("R is not installed on this system. Skipping R library installation.")
         return False
 
 def install_r_library():
+    print("Installing R library 'WGCNA'...")
     if check_r_installation():
         try:
             subprocess.run(["R", "-e", "install.packages('BiocManager'); BiocManager::install('WGCNA')"], check=True)
             print("R library 'WGCNA' has been installed successfully.")
         except subprocess.CalledProcessError:
             print("An error occurred while installing the R library 'WGCNA'.")
             sys.exit(1)
```

### Comparing `unpast-0.1.1/unpast/method.py` & `unpast-0.1.2/unpast/method.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.1/unpast/run_unpast.py` & `unpast-0.1.2/unpast/run_unpast.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.1/unpast/utils/__pycache__/method.cpython-38.pyc` & `unpast-0.1.2/unpast/utils/__pycache__/method.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `unpast-0.1.1/unpast/utils/__pycache__/method.cpython-39.pyc` & `unpast-0.1.2/unpast/utils/__pycache__/method.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `unpast-0.1.1/unpast/utils/eval.py` & `unpast-0.1.2/unpast/utils/eval.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.1/unpast/utils/method.py` & `unpast-0.1.2/unpast/utils/method.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.1/unpast/utils/pgm.py` & `unpast-0.1.2/unpast/utils/pgm.py`

 * *Files identical despite different names*

### Comparing `unpast-0.1.1/unpast/utils/run_WGCNA.R` & `unpast-0.1.2/unpast/utils/run_WGCNA.R`

 * *Files identical despite different names*

### Comparing `unpast-0.1.1/setup.py` & `unpast-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['unpast', 'unpast.utils']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'unpast': ['poster/*']}
 
 install_requires = \
 ['fisher==0.1.9',
  'jenkspy==0.2.0',
  'matplotlib-venn==0.11.6',
  'numba>=0.51.2',
  'numpy==1.22.3',
@@ -21,17 +21,17 @@
  'statsmodels==0.13.2']
 
 entry_points = \
 {'console_scripts': ['run_unpast = unpast.run_unpast:main']}
 
 setup_kwargs = {
     'name': 'unpast',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'A novel method for unsupervised patient stratification.',
-    'long_description': '# UnPaSt\n\nUnPaSt is a novel method for identification of differentially expressed biclusters in gene expression matrix. It searches for gene sets up- or down-regulated in subsets of samples:\n\n![alt text](./poster/DESMOND2_steps2.png)\n\n\nWebserver: https://unpast.zbh.uni-hamburg.de/\n\n\n## Requirements:\n<pre>\nPython 3.8 and:\n    fisher==0.1.9\n    jenkspy==0.2.0\n    pandas==1.4.2\n    python-louvain==0.15\n    matplotlib-venn==0.11.6\n    numba==0.51.2\n    numpy==1.22.3\n    scikit-learn==0.23.1\n    scikit-network==0.24.0\n    scipy==1.7.1\n    statsmodels==0.13.2\n\nR:\n    WGCNA==1.70-3\n</pre>\n\n## Installation\nThis UnPaSt can be installed using `pip`, `poetry`, run using `Docker`, or a script (see examples section). Follow the appropriate instructions below for your preferred method.\n\n1. Using pip:\n\nTo install the project using `pip`, first make sure you have `pip` installed on your system. If you haven\'t installed it already, you can find the installation instructions [here](https://pip.pypa.io/en/stable/installation/).\n\nOnce `pip` is installed, you can install the project by running the following command:\n```bash\npip install unpast\n```\n\nRun it:\n```bash\nrun_unpast -h\n```\n\n2. Installation using Poetry\nTo install the package using Poetry, first make sure you have Poetry installed, and then run:\n\n```bash\npoetry add unpast\n```\nRun it:\n```bash\npoetry run run_unpast -h\n```\n\n3. Running with Docker\nYou can also run the package using Docker. First, pull the Docker image:\n\n```bash\ndocker pull my_docker_hub_user/unpast:latest\n```\nNext, run the container:\n\n```bash\ndocker run -it --rm -v you/data/path/:/user_data/ freddsle/unpast:latest run_unpast -h\n```\n\n**Dependencies**\n\nTo use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:\n\n```bash\npython3 -m unpast.install_r_dependencies\n```\n\n## Examples\n* UnPaSt requires a tab-separated file with standardized expressions of genes (or transcripts) in rows, and samples in columns. Gene and sample names must be unique. \n* A subset of 200 randomly chosen samples from TCGA-BRCA and UnPaSt output:\n[test data](https://drive.google.com/file/d/1GXR_1ErIPtQkEOxE66at0uqQN76qNG7a/view?usp=sharing)\n\n<pre>\n# running UnPaSt with default parameters and example data\npython ./unpast/run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename TCGA_200_results\n\n# with different binarization and clustering methods\npython ./unpast/run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename results --binarization ward --clustering WGCNA\n\n# help\npython ./unpast/run_unpast.py -h\n</pre>\n\n## Outputs\n* \\<basename\\>.bin=[GMM|Jenks],clust=[Louvain|WGCNA|DESMOND].biclusters.tsv - a .tsv table with found biclsuters, where \n    - avgSNR is average SNR over all genes in the biclusters\n    - columns "n_genes" and "n_samples" provide the numbers of genes and samples, respectively \n    - "gene","sample" contain gene and sample names respectively\n    - "gene_indexes" and  "sample_indexes" - 0-based gene and sample indexes in the input matrix.\n* binarized expressions, background distributions of SNR for each bicluster size and binarization statistics [if clustering is WGCNA,  or  \'--save_binary\' flag is added]\n* modules found by WGCNA [if clustering is WGCNA]\n\n## About \nUnPaSt is an unconstrained version of DESMOND method ([repository](https://github.com/ozolotareva/DESMOND), [publication](https://academic.oup.com/bioinformatics/article/37/12/1691/6039116?login=true))\n\nMajor modifications:\n * it does not require the network of gene interactions \n * UnPaSt clusters individual genes instead of gene pairs\n * uses Gaussian mixture models or Jenks method for binarization of individual gene expressions\n * SNR threshold is authomatically determined; it depends on bicluster size in samples and user-defined p-value cutoff\n \n## License\nFree for non-for-profit use. For commercial use please contact the developers. \n\n### Poster CDCS workshop\'22\n![./poster/DESMOND2_poster_v5.png](./poster/DESMOND2_poster_v5.png)\n### Poster ISMB and MCCMB\'21\n![./poster/DESMOND2.pdf](./poster/DESMOND2.png)\n',
+    'long_description': '# UnPaSt\n\nUnPaSt is a novel method for identification of differentially expressed biclusters in gene expression matrix. It searches for gene sets up- or down-regulated in subsets of samples:\n\n![alt text](./poster/DESMOND2_steps2.png)\n\n\nWebserver: https://unpast.zbh.uni-hamburg.de/\n\n\n## Requirements:\n<pre>\nPython 3.8 and:\n    fisher==0.1.9\n    jenkspy==0.2.0\n    pandas==1.4.2\n    python-louvain==0.15\n    matplotlib-venn==0.11.6\n    numba==0.51.2\n    numpy==1.22.3\n    scikit-learn==0.23.1\n    scikit-network==0.24.0\n    scipy==1.7.1\n    statsmodels==0.13.2\n\nR:\n    WGCNA==1.70-3\n</pre>\n\n## Installation\nThis UnPaSt can be installed using `pip`, `poetry`, run using `Docker`, or a script (see examples section). Follow the appropriate instructions below for your preferred method.\nYou need to have R and Python 3.8 installed.\n\n1. Using pip: \\\nTo install the project using `pip`, first make sure you have `pip` installed on your system. If you haven\'t installed it already, you can find the installation instructions [here](https://pip.pypa.io/en/stable/installation/). \\\nOnce `pip` is installed, you can install the project by running the following command:\n```bash\npip install unpast\n```\nRun it:\n```bash\nrun_unpast -h\n```\n**Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:\n```bash\npython -m unpast.install_r_dependencies\n```\n2. Installation using Poetry: \\\nTo install the package using Poetry, first make sure you have Poetry installed, clone the repo and then run:\n```bash\npoetry add unpast\n```\nRun it:\n```bash\npoetry run run_unpast -h\n```\n**Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:\n```bash\npoetry run python -m unpast.install_r_dependencies\n```\n3. Running with Docker: \\\nYou can also run the package using Docker. First, pull the Docker image:\n```bash\ndocker pull freddsle/unpast:version0.1\n```\nNext, run the container:\n```bash\ndocker run -v /your/data/path/:/user_data/ freddsle/unpast:version0.1 --exprs /user_data/exprs.tsv --out_dir /user_data/out_dir/\n```\n\n## Examples\n* UnPaSt requires a tab-separated file with standardized expressions of genes (or transcripts) in rows, and samples in columns. Gene and sample names must be unique. \n* A subset of 200 randomly chosen samples from TCGA-BRCA and UnPaSt output:\n[test data](https://unpast-backend.zbh.uni-hamburg.de/download_example)\n\n<pre>\n# running UnPaSt with default parameters and example data\npython ./unpast/run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename TCGA_200_results\n\n# with different binarization and clustering methods\npython ./unpast/run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename results --binarization ward --clustering WGCNA\n\n# help\npython ./unpast/run_unpast.py -h\n</pre>\n\n## Outputs\n* \\<basename\\>.bin=[GMM|Jenks],clust=[Louvain|WGCNA|DESMOND].biclusters.tsv - a .tsv table with found biclsuters, where \n    - avgSNR is average SNR over all genes in the biclusters\n    - columns "n_genes" and "n_samples" provide the numbers of genes and samples, respectively \n    - "gene","sample" contain gene and sample names respectively\n    - "gene_indexes" and  "sample_indexes" - 0-based gene and sample indexes in the input matrix.\n* binarized expressions, background distributions of SNR for each bicluster size and binarization statistics [if clustering is WGCNA,  or  \'--save_binary\' flag is added]\n* modules found by WGCNA [if clustering is WGCNA]\n\n## About \nUnPaSt is an unconstrained version of DESMOND method ([repository](https://github.com/ozolotareva/DESMOND), [publication](https://academic.oup.com/bioinformatics/article/37/12/1691/6039116?login=true))\n\nMajor modifications:\n * it does not require the network of gene interactions \n * UnPaSt clusters individual genes instead of gene pairs\n * uses Gaussian mixture models or Jenks method for binarization of individual gene expressions\n * SNR threshold is authomatically determined; it depends on bicluster size in samples and user-defined p-value cutoff\n \n## License\nFree for non-for-profit use. For commercial use please contact the developers. \n\n### Poster CDCS workshop\'22\n![./poster/DESMOND2_poster_v5.png](./poster/DESMOND2_poster_v5.png)\n### Poster ISMB and MCCMB\'21\n![./poster/DESMOND2.pdf](./poster/DESMOND2.png)\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `unpast-0.1.1/PKG-INFO` & `unpast-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unpast
-Version: 0.1.1
+Version: 0.1.2
 Summary: A novel method for unsupervised patient stratification.
 License: GPL-3.0
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: fisher (==0.1.9)
@@ -47,64 +47,57 @@
 
 R:
     WGCNA==1.70-3
 </pre>
 
 ## Installation
 This UnPaSt can be installed using `pip`, `poetry`, run using `Docker`, or a script (see examples section). Follow the appropriate instructions below for your preferred method.
+You need to have R and Python 3.8 installed.
 
-1. Using pip:
-
-To install the project using `pip`, first make sure you have `pip` installed on your system. If you haven't installed it already, you can find the installation instructions [here](https://pip.pypa.io/en/stable/installation/).
-
+1. Using pip: \
+To install the project using `pip`, first make sure you have `pip` installed on your system. If you haven't installed it already, you can find the installation instructions [here](https://pip.pypa.io/en/stable/installation/). \
 Once `pip` is installed, you can install the project by running the following command:
 ```bash
 pip install unpast
 ```
-
 Run it:
 ```bash
 run_unpast -h
 ```
-
-2. Installation using Poetry
-To install the package using Poetry, first make sure you have Poetry installed, and then run:
-
+**Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:
+```bash
+python -m unpast.install_r_dependencies
+```
+2. Installation using Poetry: \
+To install the package using Poetry, first make sure you have Poetry installed, clone the repo and then run:
 ```bash
 poetry add unpast
 ```
 Run it:
 ```bash
 poetry run run_unpast -h
 ```
-
-3. Running with Docker
-You can also run the package using Docker. First, pull the Docker image:
-
+**Dependencies**. To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:
 ```bash
-docker pull my_docker_hub_user/unpast:latest
+poetry run python -m unpast.install_r_dependencies
 ```
-Next, run the container:
-
+3. Running with Docker: \
+You can also run the package using Docker. First, pull the Docker image:
 ```bash
-docker run -it --rm -v you/data/path/:/user_data/ freddsle/unpast:latest run_unpast -h
+docker pull freddsle/unpast:version0.1
 ```
-
-**Dependencies**
-
-To use this package, you will need to have R and the [WGCNA library](https://horvath.genetics.ucla.edu/html/CoexpressionNetwork/Rpackages/WGCNA/) installed. You can easily install these dependencies by running the following command after installing unpast:
-
+Next, run the container:
 ```bash
-python3 -m unpast.install_r_dependencies
+docker run -v /your/data/path/:/user_data/ freddsle/unpast:version0.1 --exprs /user_data/exprs.tsv --out_dir /user_data/out_dir/
 ```
 
 ## Examples
 * UnPaSt requires a tab-separated file with standardized expressions of genes (or transcripts) in rows, and samples in columns. Gene and sample names must be unique. 
 * A subset of 200 randomly chosen samples from TCGA-BRCA and UnPaSt output:
-[test data](https://drive.google.com/file/d/1GXR_1ErIPtQkEOxE66at0uqQN76qNG7a/view?usp=sharing)
+[test data](https://unpast-backend.zbh.uni-hamburg.de/download_example)
 
 <pre>
 # running UnPaSt with default parameters and example data
 python ./unpast/run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename TCGA_200_results
 
 # with different binarization and clustering methods
 python ./unpast/run_unpast.py --exprs TCGA_200.exprs_z.tsv --basename results --binarization ward --clustering WGCNA
```

