# Comparing `tmp/raphtory-0.2.0-cp39-none-win_amd64.whl.zip` & `tmp/raphtory-0.2.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2849769 bytes, number of entries: 7
--rw-r--r--  4.6 unx     9133 b- defN 23-May-05 17:42 raphtory-0.2.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-May-05 17:42 raphtory-0.2.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     2052 b- defN 23-May-05 17:42 raphtory/nullmodels.py
--rw-r--r--  4.6 unx     7531 b- defN 23-May-05 17:42 raphtory/vis.py
--rw-r--r--  4.6 unx      537 b- defN 23-May-05 17:42 raphtory/__init__.py
--rwxr-xr-x  4.6 unx  8158208 b- defN 23-May-05 17:42 raphtory/raphtory.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      532 b- defN 23-May-05 17:42 raphtory-0.2.0.dist-info/RECORD
-7 files, 8178089 bytes uncompressed, 2848841 bytes compressed:  65.2%
+Zip file size: 2846821 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     9743 b- defN 23-May-09 16:35 raphtory-0.2.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-May-09 16:35 raphtory-0.2.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     2052 b- defN 23-May-09 16:35 raphtory/nullmodels.py
+-rw-r--r--  4.6 unx     7531 b- defN 23-May-09 16:35 raphtory/vis.py
+-rw-r--r--  4.6 unx      537 b- defN 23-May-09 16:35 raphtory/__init__.py
+-rwxr-xr-x  4.6 unx  8145920 b- defN 23-May-09 16:35 raphtory/raphtory.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      532 b- defN 23-May-09 16:35 raphtory-0.2.1.dist-info/RECORD
+7 files, 8166410 bytes uncompressed, 2845893 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: raphtory-0.2.0.dist-info/METADATA
+Filename: raphtory-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: raphtory-0.2.0.dist-info/WHEEL
+Filename: raphtory-0.2.1.dist-info/WHEEL
 Comment: 
 
 Filename: raphtory/nullmodels.py
 Comment: 
 
 Filename: raphtory/vis.py
 Comment: 
 
 Filename: raphtory/__init__.py
 Comment: 
 
 Filename: raphtory/raphtory.cp39-win_amd64.pyd
 Comment: 
 
-Filename: raphtory-0.2.0.dist-info/RECORD
+Filename: raphtory-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `raphtory-0.2.0.dist-info/METADATA` & `raphtory-0.2.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: raphtory
-Version: 0.2.0
+Version: 0.2.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: pandas >= 1.3.3
-Requires-Dist: pyvis >= 0.3.2; extra == 'vis'
-Requires-Dist: networkx >= 2.6.3; extra == 'vis'
-Requires-Dist: matplotlib >= 3.4.3; extra == 'vis'
-Requires-Dist: seaborn >= 0.11.2; extra == 'vis'
+Requires-Dist: pandas >=1.3.3
+Requires-Dist: pyvis >=0.3.2 ; extra == 'vis'
+Requires-Dist: networkx >=2.6.3 ; extra == 'vis'
+Requires-Dist: matplotlib >=3.4.3 ; extra == 'vis'
+Requires-Dist: seaborn >=0.11.2 ; extra == 'vis'
 Provides-Extra: vis
 Summary: Python package for raphtory, a temporal graph library
 Keywords: graph,temporal-graph,temporal
 Home-Page: https://github.com/Raphtory/raphtory/
 Author: Pometry
 License: AGPL-3.0-only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: homepage, https://github.com/pometry/raphtory
 Project-URL: documentation, https://docs.raphtory.com/
-Project-URL: repository, https://github.com/raphtory/raphtory
+Project-URL: repository, https://github.com/pometry/raphtory
 Project-URL: twitter, https://twitter.com/raphtory/
-Project-URL: youtube, https://www.youtube.com/@pometry8546/videos
 Project-URL: slack, https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA
-Project-URL: homepage, https://github.com/raphtory/raphtory
+Project-URL: youtube, https://www.youtube.com/@pometry8546/videos
 
 <br>
 <p align="center">
   <img src="https://user-images.githubusercontent.com/6665739/130641943-fa7fcdb8-a0e7-4aa4-863f-3df61b5de775.png" alt="Raphtory" height="100"/>
 </p>
 <p align="center">
 </p>
@@ -161,15 +161,30 @@
 
 #### Developing an end-to-end application
 
 | Type | Description                                                                                                                                                   |
 | ------------- |---------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | Notebook | [Use our powerful time APIs to find pump and dump scams in popular NFTs](https://github.com/Raphtory/Raphtory/blob/master/examples/py/nft/nft_analysis.ipynb) |
 
-## Community  
+
+# Benchmarks
+
+We host a page which triggers and saves the result of two benchmarks upon every push to the master branch. 
+
+View this here [https://pometry.github.io/Raphtory/dev/bench/](https://pometry.github.io/Raphtory/dev/bench/)
+
+# Bounty board
+
+Raphtory is currently offering rewards for contributions, such as new features or algorithms. Contributors will receive swag and prizes! 
+
+To get started, check out our list of desired algorithms at https://github.com/Raphtory/Raphtory/discussions/categories/bounty-board which include some low hanging fruit (🍇) that are easy to implement. 
+
+
+# Community  
+
 Join the growing community of open-source enthusiasts using Raphtory to power their graph analysis projects!
 
 - Follow [![Slack](https://img.shields.io/twitter/follow/raphtory?label=@raphtory)](https://twitter.com/raphtory) for the latest Raphtory news and development
 
 - Join our [![Slack](https://img.shields.io/badge/community-Slack-red)](https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA) to chat with us and get answers to your questions!
```

### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: raphtory Version: 0.2.0 Classifier: Programming
+Metadata-Version: 2.1 Name: raphtory Version: 0.2.1 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Dist: pandas >= 1.3.3 Requires-Dist: pyvis >= 0.3.2; extra == 'vis'
-Requires-Dist: networkx >= 2.6.3; extra == 'vis' Requires-Dist: matplotlib >=
-3.4.3; extra == 'vis' Requires-Dist: seaborn >= 0.11.2; extra == 'vis'
+Requires-Dist: pandas >=1.3.3 Requires-Dist: pyvis >=0.3.2 ; extra == 'vis'
+Requires-Dist: networkx >=2.6.3 ; extra == 'vis' Requires-Dist: matplotlib
+>=3.4.3 ; extra == 'vis' Requires-Dist: seaborn >=0.11.2 ; extra == 'vis'
 Provides-Extra: vis Summary: Python package for raphtory, a temporal graph
 library Keywords: graph,temporal-graph,temporal Home-Page: https://github.com/
 Raphtory/raphtory/ Author: Pometry License: AGPL-3.0-only Requires-Python:
 >=3.7 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: documentation, https://docs.raphtory.com/ Project-URL: repository,
-https://github.com/raphtory/raphtory Project-URL: twitter, https://twitter.com/
-raphtory/ Project-URL: youtube, https://www.youtube.com/@pometry8546/videos
+Project-URL: homepage, https://github.com/pometry/raphtory Project-URL:
+documentation, https://docs.raphtory.com/ Project-URL: repository, https://
+github.com/pometry/raphtory Project-URL: twitter, https://twitter.com/raphtory/
 Project-URL: slack, https://join.slack.com/t/raphtory/shared_invite/zt-
-xbebws9j-VgPIFRleJFJBwmpf81tvxA Project-URL: homepage, https://github.com/
-raphtory/raphtory
+xbebws9j-VgPIFRleJFJBwmpf81tvxA Project-URL: youtube, https://www.youtube.com/
+@pometry8546/videos
                                   [Raphtory]
 [Test_and_Build] [Latest_Release] [Issues] [Crates.io] [PyPI] [Launch_Notebook]
 ð_Website   ð_Documentation   [https://user-images.githubusercontent.com/
      6665739/202438989-2859f8b8-30fb-4402-820a-563049e1fdb3.png]_Pometry  
            ð§ð»â_Tutorial   ð_Report_a_Bug   [https://user-
     images.githubusercontent.com/6665739/154071628-a55fb5f9-6994-4dcf-be03-
                          401afc7d9ee0.png]_Join_Slack
@@ -75,19 +75,27 @@
 -------------------------------------| | Tutorial | [Building your first graph]
 (https://docs.raphtory.com/en/master/Introduction/ingestion.html) | ####
 Developing an end-to-end application | Type | Description | | ------------- |--
 -------------------------------------------------------------------------------
 ------------------------------------------------------------------------------
 | | Notebook | [Use our powerful time APIs to find pump and dump scams in
 popular NFTs](https://github.com/Raphtory/Raphtory/blob/master/examples/py/nft/
-nft_analysis.ipynb) | ## Community Join the growing community of open-source
-enthusiasts using Raphtory to power their graph analysis projects! - Follow [!
-[Slack](https://img.shields.io/twitter/follow/raphtory?label=@raphtory)](https:
-//twitter.com/raphtory) for the latest Raphtory news and development - Join our
-[![Slack](https://img.shields.io/badge/community-Slack-red)](https://
-join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA) to
-chat with us and get answers to your questions! ## Contributors [https://
-contrib.rocks/image?repo=raphtory/raphtory] Want to get involved? Please join
-the Raphtory [Slack](https://join.slack.com/t/raphtory/shared_invite/zt-
-xbebws9j-VgPIFRleJFJBwmpf81tvxA) group and speak with us on how you could pitch
-in! ## License Raphtory is licensed under the terms of the GNU General Public
-License v3.0 (check out our LICENSE file).
+nft_analysis.ipynb) | # Benchmarks We host a page which triggers and saves the
+result of two benchmarks upon every push to the master branch. View this here
+[https://pometry.github.io/Raphtory/dev/bench/](https://pometry.github.io/
+Raphtory/dev/bench/) # Bounty board Raphtory is currently offering rewards for
+contributions, such as new features or algorithms. Contributors will receive
+swag and prizes! To get started, check out our list of desired algorithms at
+https://github.com/Raphtory/Raphtory/discussions/categories/bounty-board which
+include some low hanging fruit (ð) that are easy to implement. # Community
+Join the growing community of open-source enthusiasts using Raphtory to power
+their graph analysis projects! - Follow [![Slack](https://img.shields.io/
+twitter/follow/raphtory?label=@raphtory)](https://twitter.com/raphtory) for the
+latest Raphtory news and development - Join our [![Slack](https://
+img.shields.io/badge/community-Slack-red)](https://join.slack.com/t/raphtory/
+shared_invite/zt-xbebws9j-VgPIFRleJFJBwmpf81tvxA) to chat with us and get
+answers to your questions! ## Contributors [https://contrib.rocks/
+image?repo=raphtory/raphtory] Want to get involved? Please join the Raphtory
+[Slack](https://join.slack.com/t/raphtory/shared_invite/zt-xbebws9j-
+VgPIFRleJFJBwmpf81tvxA) group and speak with us on how you could pitch in! ##
+License Raphtory is licensed under the terms of the GNU General Public License
+v3.0 (check out our LICENSE file).
```

## Comparing `raphtory-0.2.0.dist-info/RECORD` & `raphtory-0.2.1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-raphtory-0.2.0.dist-info/METADATA,sha256=Vg_A1pobaghYxlu2F_m19gJkAwAwPLxDbJEuo-whsN0,9133
-raphtory-0.2.0.dist-info/WHEEL,sha256=HfbNN9yA0Gn_6VCTRBzbKHMHpOwMN7MCpAKvpT7Uqyk,96
+raphtory-0.2.1.dist-info/METADATA,sha256=xXX5KvUxnSf63XND1EPBONdyhPSxP8vKufFGJyE2qcA,9743
+raphtory-0.2.1.dist-info/WHEEL,sha256=g59ZRREgF6O89Tupb3WRh6JI_H6_P0yVbxR5mPccBf0,95
 raphtory/nullmodels.py,sha256=5nfd-RxH-6K4AauFJloQnJpNxuzZcrmm8RdC1uocT0c,2052
 raphtory/vis.py,sha256=lkhkOg98fpCA1x-GLCpBwVRCcYPf2zjHrhrMhJuBGDk,7531
 raphtory/__init__.py,sha256=cz9aVhEsCG64qaR7RGfMYVlPK_rH826ES4G2RxPW15A,537
-raphtory/raphtory.cp39-win_amd64.pyd,sha256=yPn4lOALVAv-E8_ArNa2y_rqgebFG6XDZb3rKcLOSmA,8158208
-raphtory-0.2.0.dist-info/RECORD,,
+raphtory/raphtory.cp39-win_amd64.pyd,sha256=WfteHDTZ51MCVns5l3Ra-c88npIUDgJVhLONpx_LH_U,8145920
+raphtory-0.2.1.dist-info/RECORD,,
```

