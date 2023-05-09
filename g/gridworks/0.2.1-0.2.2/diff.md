# Comparing `tmp/gridworks-0.2.1.tar.gz` & `tmp/gridworks-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks-0.2.1.tar", max compression
+gzip compressed data, was "gridworks-0.2.2.tar", max compression
```

## Comparing `gridworks-0.2.1.tar` & `gridworks-0.2.2.tar`

### file list

```diff
@@ -1,57 +1,54 @@
--rw-r--r--   0        0        0     1065 2023-03-30 15:14:04.806334 gridworks-0.2.1/LICENSE
--rw-r--r--   0        0        0     5796 2023-03-30 15:14:04.806334 gridworks-0.2.1/README.md
--rw-r--r--   0        0        0     2358 2023-03-30 15:14:18.359117 gridworks-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      208 2023-03-30 15:14:04.866337 gridworks-0.2.1/src/gridworks/__init__.py
--rw-r--r--   0        0        0      208 2023-03-30 15:14:04.866337 gridworks-0.2.1/src/gridworks/__main__.py
--rw-r--r--   0        0        0    48236 2023-03-30 15:14:04.866337 gridworks-0.2.1/src/gridworks/actor_base.py
--rw-r--r--   0        0        0    18028 2023-03-30 15:14:04.866337 gridworks-0.2.1/src/gridworks/algo_utils.py
--rw-r--r--   0        0        0    12872 2023-03-30 15:14:04.866337 gridworks-0.2.1/src/gridworks/api_utils.py
--rw-r--r--   0        0        0     2871 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/base_api_types.py
--rw-r--r--   0        0        0      251 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/conversion_factors.py
--rw-r--r--   0        0        0        0 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/data_classes/__init__.py
--rw-r--r--   0        0        0     6761 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/data_classes/g_node.py
--rw-r--r--   0        0        0     6440 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/data_classes/g_node_instance.py
--rw-r--r--   0        0        0      723 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/data_classes/gps_point.py
--rw-r--r--   0        0        0     2498 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/data_classes/market_type.py
--rw-r--r--   0        0        0     1254 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/data_classes/supervisor_container.py
--rw-r--r--   0        0        0      131 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/dev_utils/__init__.py
--rw-r--r--   0        0        0     3391 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/dev_utils/algo_setup.py
--rw-r--r--   0        0        0     1238 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/__init__.py
--rw-r--r--   0        0        0      673 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/algo_cert_type.py
--rw-r--r--   0        0        0      990 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/core_g_node_role.py
--rw-r--r--   0        0        0     2246 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/g_node_role.py
--rw-r--r--   0        0        0      992 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/g_node_status.py
--rw-r--r--   0        0        0      933 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/gni_status.py
--rw-r--r--   0        0        0      563 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/market_price_unit.py
--rw-r--r--   0        0        0      590 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/market_quantity_unit.py
--rw-r--r--   0        0        0     1394 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/market_type_name.py
--rw-r--r--   0        0        0     1326 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/message_category.py
--rw-r--r--   0        0        0     1189 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/message_category_symbol.py
--rw-r--r--   0        0        0      626 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/recognized_currency_unit.py
--rw-r--r--   0        0        0     1331 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/strategy_name.py
--rw-r--r--   0        0        0     1081 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/supervisor_container_status.py
--rw-r--r--   0        0        0      795 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/enums/universe_type.py
--rw-r--r--   0        0        0      336 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/errors.py
--rw-r--r--   0        0        0     4187 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/gw_config.py
--rw-r--r--   0        0        0     2813 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/message.py
--rw-r--r--   0        0        0    16163 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/property_format.py
--rw-r--r--   0        0        0        0 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/py.typed
--rw-r--r--   0        0        0     9199 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/rest_api.py
--rw-r--r--   0        0        0     2523 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/__init__.py
--rw-r--r--   0        0        0    24525 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/g_node_gt.py
--rw-r--r--   0        0        0    15787 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/g_node_instance_gt.py
--rw-r--r--   0        0        0     6719 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/gw_cert_id.py
--rw-r--r--   0        0        0     3502 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/heartbeat_a.py
--rw-r--r--   0        0        0     6064 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/initial_tadeed_algo_create.py
--rw-r--r--   0        0        0     7517 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/initial_tadeed_algo_optin.py
--rw-r--r--   0        0        0     8839 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/initial_tadeed_algo_transfer.py
--rw-r--r--   0        0        0        0 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/old_versions/__init__.py
--rw-r--r--   0        0        0     1838 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/old_versions/heartbeat_a_001.py
--rw-r--r--   0        0        0     5581 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/ready.py
--rw-r--r--   0        0        0     8098 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/sim_timestep.py
--rw-r--r--   0        0        0     6096 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/super_starter.py
--rw-r--r--   0        0        0    12069 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/supervisor_container_gt.py
--rw-r--r--   0        0        0     8984 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/tavalidatorcert_algo_create.py
--rw-r--r--   0        0        0     6279 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/types/tavalidatorcert_algo_transfer.py
--rw-r--r--   0        0        0     5788 2023-03-30 15:14:04.870338 gridworks-0.2.1/src/gridworks/utils.py
--rw-r--r--   0        0        0     7322 1970-01-01 00:00:00.000000 gridworks-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-09 19:35:56.464290 gridworks-0.2.2/LICENSE
+-rw-r--r--   0        0        0     5778 2023-05-09 19:36:13.624409 gridworks-0.2.2/README.md
+-rw-r--r--   0        0        0     2358 2023-05-09 19:36:13.624409 gridworks-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/__init__.py
+-rw-r--r--   0        0        0      208 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/__main__.py
+-rw-r--r--   0        0        0    47777 2023-05-09 19:36:13.628409 gridworks-0.2.2/src/gridworks/actor_base.py
+-rw-r--r--   0        0        0    18028 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/algo_utils.py
+-rw-r--r--   0        0        0    12872 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/api_utils.py
+-rw-r--r--   0        0        0     2016 2023-05-09 19:36:13.628409 gridworks-0.2.2/src/gridworks/base_api_types.py
+-rw-r--r--   0        0        0      251 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/conversion_factors.py
+-rw-r--r--   0        0        0        0 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/data_classes/__init__.py
+-rw-r--r--   0        0        0    23522 2023-05-09 19:36:13.628409 gridworks-0.2.2/src/gridworks/data_classes/base_g_node.py
+-rw-r--r--   0        0        0     6761 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/data_classes/g_node.py
+-rw-r--r--   0        0        0     6440 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/data_classes/g_node_instance.py
+-rw-r--r--   0        0        0      723 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/data_classes/gps_point.py
+-rw-r--r--   0        0        0     2498 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/data_classes/market_type.py
+-rw-r--r--   0        0        0     1254 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/data_classes/supervisor_container.py
+-rw-r--r--   0        0        0      131 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/dev_utils/__init__.py
+-rw-r--r--   0        0        0     3391 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/dev_utils/algo_setup.py
+-rw-r--r--   0        0        0     1238 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/algo_cert_type.py
+-rw-r--r--   0        0        0      990 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/core_g_node_role.py
+-rw-r--r--   0        0        0     2246 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/g_node_role.py
+-rw-r--r--   0        0        0      992 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/g_node_status.py
+-rw-r--r--   0        0        0      933 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/gni_status.py
+-rw-r--r--   0        0        0      563 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/market_price_unit.py
+-rw-r--r--   0        0        0      590 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/market_quantity_unit.py
+-rw-r--r--   0        0        0     1394 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/market_type_name.py
+-rw-r--r--   0        0        0     1326 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/message_category.py
+-rw-r--r--   0        0        0     1189 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/message_category_symbol.py
+-rw-r--r--   0        0        0      626 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/recognized_currency_unit.py
+-rw-r--r--   0        0        0     1331 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/strategy_name.py
+-rw-r--r--   0        0        0     1081 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/supervisor_container_status.py
+-rw-r--r--   0        0        0      795 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/enums/universe_type.py
+-rw-r--r--   0        0        0      336 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/errors.py
+-rw-r--r--   0        0        0     4187 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/gw_config.py
+-rw-r--r--   0        0        0     2813 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/message.py
+-rw-r--r--   0        0        0    17029 2023-05-09 19:36:13.628409 gridworks-0.2.2/src/gridworks/property_format.py
+-rw-r--r--   0        0        0        0 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/py.typed
+-rw-r--r--   0        0        0     9199 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/rest_api.py
+-rw-r--r--   0        0        0     1476 2023-05-09 19:36:13.628409 gridworks-0.2.2/src/gridworks/types/__init__.py
+-rw-r--r--   0        0        0    20321 2023-05-09 19:36:13.628409 gridworks-0.2.2/src/gridworks/types/base_g_node_gt.py
+-rw-r--r--   0        0        0    24525 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/types/g_node_gt.py
+-rw-r--r--   0        0        0    15787 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/types/g_node_instance_gt.py
+-rw-r--r--   0        0        0     6719 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/types/gw_cert_id.py
+-rw-r--r--   0        0        0     3502 2023-05-09 19:35:56.544290 gridworks-0.2.2/src/gridworks/types/heartbeat_a.py
+-rw-r--r--   0        0        0        0 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/types/old_versions/__init__.py
+-rw-r--r--   0        0        0     1838 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/types/old_versions/heartbeat_a_001.py
+-rw-r--r--   0        0        0     5581 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/types/ready.py
+-rw-r--r--   0        0        0     8098 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/types/sim_timestep.py
+-rw-r--r--   0        0        0     6096 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/types/super_starter.py
+-rw-r--r--   0        0        0    12069 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/types/supervisor_container_gt.py
+-rw-r--r--   0        0        0     5788 2023-05-09 19:35:56.548290 gridworks-0.2.2/src/gridworks/utils.py
+-rw-r--r--   0        0        0     7304 1970-01-01 00:00:00.000000 gridworks-0.2.2/PKG-INFO
```

### Comparing `gridworks-0.2.1/LICENSE` & `gridworks-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/README.md` & `gridworks-0.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,50 +17,48 @@
 [python version]: https://pypi.org/project/gridworks
 [read the docs]: https://gridworks.readthedocs.io/
 [tests]: https://github.com/thegridelectric/gridworks/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/thegridelectric/gridworks
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
-GridWorks uses distributed actors to balance the electric grid. What does this mean?  In today's world, more
+GridWorks uses distributed actors to balance the electric grid. What does this mean? In today's world, more
 power comes from highly variable power sources such as wind and solar. And yet, the number
-of electrons going into the grid must match the number coming out.  This is where GridWorks comes in.
+of electrons going into the grid must match the number coming out. This is where GridWorks comes in.
 GridWorks technology enables electrical devices with some embedded storage or with flexibility to provide grid
 balancing. Furthermore, GridWorks allows these appliances to be more thrifty, using electricity when
 it is cheap and green.
 
 To learn how using and contributing to GridWorks can support a cost-effective and rapid transition to a sustainable future:
 
 - Try some simple [Hello World](https://gridworks.readthedocs.io/en/latest/hello-gridworks.html) examples;
 - Read the [Millinocket Story](https://gridworks.readthedocs.io/en/latest/millinocket-demo.html) to learn how to exploit the synergy between wind power and space heating;
 - Go through the partner [Millinocket Tutorial](https://gridworks.readthedocs.io/en/latest/millinocket-tutorial.html).
 
 ## Blockchain Mechanics
 
-
 Gridworks runs markets between distributed actors acting as avatars for physical devices on the grid. It needs a
 foundation of trustless, secure, scalable validation and authentication. It heavily uses the Algorand blockchain. If
 you want to undestand more about how and why this is, go [here](blockchain.html).
 
 ## GridWorks SDKs
 
- - **gridworks**: [package](https://pypi.org/project/gridworks/) provides basic shared mechanics for  communication and GNode structure. It is used as a package in all of our other repos.
+- **gridworks**: [package](https://pypi.org/project/gridworks/) provides basic shared mechanics for communication and GNode structure. It is used as a package in all of our other repos.
 
- - **gridworks-atn**:  [package](https://pypi.org/project/gridworks-atn/) and associated [documentation](https://gridworks-atn.readthedocs.io/en/latest/) for the GridWorks Python [AtomicTNodes](https://gridworks.readthedocs.io/en/latest/atomic-t-node.html)  SDK. AtomicTNodes  are the GridWorks actors that make electrical devices *transactive*. This SDK is a great place to learn about blockchain mechanics, as it introduces some of the simpler structures (NFTs, stateless contracts, and then some simple stateful smart contracts constructed using  [beaker](https://github.com/algorand-devrel/beaker) ) required for establishing the link between physical reality on the electric grid and the actors that play their avatars in GridWorks.  
+- **gridworks-atn**: [package](https://pypi.org/project/gridworks-atn/) and associated [documentation](https://gridworks-atn.readthedocs.io/en/latest/) for the GridWorks Python [AtomicTNodes](https://gridworks.readthedocs.io/en/latest/atomic-t-node.html) SDK. AtomicTNodes are the GridWorks actors that make electrical devices _transactive_. This SDK is a great place to learn about blockchain mechanics, as it introduces some of the simpler structures (NFTs, stateless contracts, and then some simple stateful smart contracts constructed using [beaker](https://github.com/algorand-devrel/beaker) ) required for establishing the link between physical reality on the electric grid and the actors that play their avatars in GridWorks.
 
- - **gridworks-marketmaker**: [package](https://pypi.org/project/gridworks-marketmaker/) and associated [documentation](https://gridworks-marketmaker.readthedocs.io/en/latest/)  for our Python [MarketMaker](https://gridworks.readthedocs.io/en/latest/market-maker.html) SDK.  GridWorks uses distributed actors to balance the electric grid, and MarketMakers are the actors brokering this grid balancing via the markets they run for energy and balancing services.
+- **gridworks-marketmaker**: [package](https://pypi.org/project/gridworks-marketmaker/) and associated [documentation](https://gridworks-marketmaker.readthedocs.io/en/latest/) for our Python [MarketMaker](https://gridworks.readthedocs.io/en/latest/market-maker.html) SDK. GridWorks uses distributed actors to balance the electric grid, and MarketMakers are the actors brokering this grid balancing via the markets they run for energy and balancing services.
 
 There are several other open source GridWorks repos to explore on [our github page](https://github.com/thegridelectric),
 including the code running on the [SCADA systems](https://github.com/thegridelectric/gw-scada-spaceheat-python)
 that Efficiency Maine is deploying in Millinocket this winter.
-The  [GNodeFactory](https://github.com/thegridelectric/g-node-factory) currently hosts the demo,
-and  does most of the heavy lifting in terms of identity management and authentication in GridWorks. Finally, since the demo
+The [GNodeFactory](https://github.com/thegridelectric/g-node-factory) currently hosts the demo,
+and does most of the heavy lifting in terms of identity management and authentication in GridWorks. Finally, since the demo
 is a distributed simulation, it needs a method of handling time. That's done by a [TimeCoordinator](https://github.com/thegridelectric/gridworks-timecoordinator) GNode.
 
-
 ## Usage
 
 `pip install gridworks` to install the foundational package.
 
 ## Contributing
 
 Contributions are very welcome.
```

### Comparing `gridworks-0.2.1/pyproject.toml` & `gridworks-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks"
-version = "0.2.1"
+version = "0.2.2"
 description = "Gridworks"
 authors = ["GridWorks <gridworks@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks"
 repository = "https://github.com/thegridelectric/gridworks"
 documentation = "https://gridworks.readthedocs.io"
```

### Comparing `gridworks-0.2.1/src/gridworks/actor_base.py` & `gridworks-0.2.2/src/gridworks/actor_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -803,19 +803,14 @@
            routing_key (str): This is the basic_deliver.routing_key string
            in a rabbit message
 
         Returns:
            MessageCategory: the MessageCategory, as enum
         """
         routing_key_words = routing_key.split(".")
-        if len(routing_key_words) < 4:
-            self._latest_on_message_diagnostic = (
-                OnReceiveMessageDiagnostic.UNKNOWN_ROUTING_KEY_TYPE
-            )
-            raise SchemaError(f"Routing key {routing_key} must have at least 3 words!")
         msg_category_symbol_value = routing_key_words[0]
 
         try:
             msg_category_symbol = MessageCategorySymbol(msg_category_symbol_value)
         except ValueError:
             self._latest_on_message_diagnostic = (
                 OnReceiveMessageDiagnostic.UNKNOWN_MESSAGE_CATEGORY_SYMBOL
@@ -955,47 +950,42 @@
             return OnSendMessageDiagnostic.STOPPED_SO_NOT_SENDING
 
         if "MessageId" in payload.as_dict():
             correlation_id = payload.MessageId
         else:
             correlation_id = str(uuid.uuid4())
 
+        properties = pika.BasicProperties(
+            reply_to=self.queue_name,
+            app_id=self.alias,
+            type=message_category,
+            correlation_id=correlation_id,
+        )
+        publish_exchange = self._publish_exchange
         if message_category is MessageCategory.RabbitJsonDirect:
             if not isinstance(to_role, GNodeRole):
                 raise Exception("Must include to_role for a direct message")
             if not property_format.is_left_right_dot(to_g_node_alias):
                 raise Exception(
                     f"to_g_node_alias must have LrdAliasFormat. Got {to_g_node_alias}"
                 )
             routing_key = self.direct_routing_key(
                 to_role=to_role,
                 payload=payload,
                 to_g_node_alias=to_g_node_alias,
             )
-
-            properties = pika.BasicProperties(
-                reply_to=self.queue_name,
-                app_id=self.alias,
-                type=message_category.RabbitJsonDirect,
-                correlation_id=correlation_id,
-            )
         elif message_category is MessageCategory.RabbitJsonBroadcast:
             routing_key = self.broadcast_routing_key(
                 payload=payload, radio_channel=radio_channel
             )
-            properties = pika.BasicProperties(
-                reply_to=self.queue_name,
-                app_id=self.alias,
-                type=message_category.RabbitJsonBroadcast,
-                correlation_id=correlation_id,
-            )
         elif message_category is MessageCategory.MqttJsonBroadcast:
             routing_key = self.scada_routing_key(
                 payload=payload, to_g_node_alias=to_g_node_alias
             )
+            publish_exchange = "amq.topic"
         else:
             raise Exception(f"Does not handle MessageCategory {message_category}")
 
         # if self._publish_channel is None:
         #     LOGGER.error(f"No publish channel so not sending {routing_key}")
         #     return OnSendMessageDiagnostic.CHANNEL_NOT_OPEN
         # if not self._publish_channel.is_open:
@@ -1007,15 +997,15 @@
             return OnSendMessageDiagnostic.CHANNEL_NOT_OPEN
         if not self._consume_channel.is_open:
             LOGGER.error(f"Channel not open so not sending {routing_key}")
             return OnSendMessageDiagnostic.CHANNEL_NOT_OPEN
 
         try:
             self._consume_channel.basic_publish(
-                exchange=self._publish_exchange,
+                exchange=publish_exchange,
                 routing_key=routing_key,
                 body=payload.as_type(),
                 properties=properties,
             )
             # self._publish_channel.basic_publish(
             #     exchange=self._publish_exchange,
             #     routing_key=routing_key,
```

### Comparing `gridworks-0.2.1/src/gridworks/algo_utils.py` & `gridworks-0.2.2/src/gridworks/algo_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/api_utils.py` & `gridworks-0.2.2/src/gridworks/api_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/base_api_types.py` & `gridworks-0.2.2/src/gridworks/base_api_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,78 @@
 """ List of all the types used"""
 from typing import Dict
 from typing import List
 from typing import no_type_check
 
+from gridworks.types import BaseGNodeGt_Maker
 from gridworks.types import GNodeGt_Maker
 from gridworks.types import GNodeInstanceGt_Maker
 from gridworks.types import GwCertId_Maker
 from gridworks.types import HeartbeatA_Maker
-from gridworks.types import InitialTadeedAlgoCreate_Maker
-from gridworks.types import InitialTadeedAlgoOptin_Maker
-from gridworks.types import InitialTadeedAlgoTransfer_Maker
 from gridworks.types import Ready_Maker
 from gridworks.types import SimTimestep_Maker
 from gridworks.types import SuperStarter_Maker
 from gridworks.types import SupervisorContainerGt_Maker
-from gridworks.types import TavalidatorcertAlgoCreate_Maker
-from gridworks.types import TavalidatorcertAlgoTransfer_Maker
 
 
 TypeMakerByName: Dict[str, HeartbeatA_Maker] = {}
 
 
 @no_type_check
 def type_makers() -> List[HeartbeatA_Maker]:
     return [
+        BaseGNodeGt_Maker,
         GNodeGt_Maker,
         GNodeInstanceGt_Maker,
         GwCertId_Maker,
         HeartbeatA_Maker,
-        InitialTadeedAlgoCreate_Maker,
-        InitialTadeedAlgoOptin_Maker,
-        InitialTadeedAlgoTransfer_Maker,
         Ready_Maker,
         SimTimestep_Maker,
         SuperStarter_Maker,
         SupervisorContainerGt_Maker,
-        TavalidatorcertAlgoCreate_Maker,
-        TavalidatorcertAlgoTransfer_Maker,
     ]
 
 
 for maker in type_makers():
     TypeMakerByName[maker.type_name] = maker
 
 
 def version_by_type_name() -> Dict[str, str]:
     """
     Returns:
         Dict[str, str]: Keys are TypeNames, values are versions
     """
 
     v: Dict[str, str] = {
+        "base.g.node.gt": "002",
         "g.node.gt": "002",
         "g.node.instance.gt": "000",
         "gw.cert.id": "000",
         "heartbeat.a": "100",
-        "initial.tadeed.algo.create": "000",
-        "initial.tadeed.algo.optin": "002",
-        "initial.tadeed.algo.transfer": "000",
         "ready": "001",
         "sim.timestep": "000",
         "super.starter": "000",
         "supervisor.container.gt": "000",
-        "tavalidatorcert.algo.create": "000",
-        "tavalidatorcert.algo.transfer": "000",
     }
 
     return v
 
 
 def status_by_versioned_type_name() -> Dict[str, str]:
     """
     Returns:
         Dict[str, str]: Keys are versioned TypeNames, values are type status
     """
 
     v: Dict[str, str] = {
-        "g.node.gt.002": "Pending",
-        "g.node.instance.gt.000": "Pending",
+        "base.g.node.gt.002": "Active",
+        "g.node.gt.002": "Active",
+        "g.node.instance.gt.000": "Active",
         "gw.cert.id.000": "Active",
-        "heartbeat.a.100": "Pending",
-        "initial.tadeed.algo.create.000": "Active",
-        "initial.tadeed.algo.optin.002": "Active",
-        "initial.tadeed.algo.transfer.000": "Active",
-        "ready.001": "Pending",
-        "sim.timestep.000": "Pending",
-        "super.starter.000": "Pending",
-        "supervisor.container.gt.000": "Pending",
-        "tavalidatorcert.algo.create.000": "Active",
-        "tavalidatorcert.algo.transfer.000": "Active",
+        "heartbeat.a.100": "Active",
+        "ready.001": "Active",
+        "sim.timestep.000": "Active",
+        "super.starter.000": "Active",
+        "supervisor.container.gt.000": "Active",
     }
 
     return v
```

### Comparing `gridworks-0.2.1/src/gridworks/data_classes/g_node.py` & `gridworks-0.2.2/src/gridworks/data_classes/g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/data_classes/g_node_instance.py` & `gridworks-0.2.2/src/gridworks/data_classes/g_node_instance.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/data_classes/gps_point.py` & `gridworks-0.2.2/src/gridworks/data_classes/gps_point.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/data_classes/market_type.py` & `gridworks-0.2.2/src/gridworks/data_classes/market_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/data_classes/supervisor_container.py` & `gridworks-0.2.2/src/gridworks/data_classes/supervisor_container.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/dev_utils/algo_setup.py` & `gridworks-0.2.2/src/gridworks/dev_utils/algo_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/__init__.py` & `gridworks-0.2.2/src/gridworks/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/algo_cert_type.py` & `gridworks-0.2.2/src/gridworks/enums/algo_cert_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/core_g_node_role.py` & `gridworks-0.2.2/src/gridworks/enums/core_g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/g_node_role.py` & `gridworks-0.2.2/src/gridworks/enums/g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/g_node_status.py` & `gridworks-0.2.2/src/gridworks/enums/g_node_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/gni_status.py` & `gridworks-0.2.2/src/gridworks/enums/gni_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/market_price_unit.py` & `gridworks-0.2.2/src/gridworks/enums/market_price_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/market_quantity_unit.py` & `gridworks-0.2.2/src/gridworks/enums/market_quantity_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/market_type_name.py` & `gridworks-0.2.2/src/gridworks/enums/market_type_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/message_category.py` & `gridworks-0.2.2/src/gridworks/enums/message_category.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/message_category_symbol.py` & `gridworks-0.2.2/src/gridworks/enums/message_category_symbol.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/recognized_currency_unit.py` & `gridworks-0.2.2/src/gridworks/enums/recognized_currency_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/strategy_name.py` & `gridworks-0.2.2/src/gridworks/enums/strategy_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/supervisor_container_status.py` & `gridworks-0.2.2/src/gridworks/enums/supervisor_container_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/enums/universe_type.py` & `gridworks-0.2.2/src/gridworks/enums/universe_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/gw_config.py` & `gridworks-0.2.2/src/gridworks/gw_config.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/message.py` & `gridworks-0.2.2/src/gridworks/message.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/property_format.py` & `gridworks-0.2.2/src/gridworks/property_format.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,60 @@
 import pydantic
 
 from gridworks.data_classes.market_type import MarketType
 from gridworks.enums import MarketTypeName
 
 
 def predicate_validator(
-    field_name: str, predicate: Callable[[Any], bool], error_format: str = ""
+    field_name: str, predicate: Callable[[Any], bool], error_format: str = "", **kwargs
 ) -> classmethod:  # type: ignore
+    """
+    Produce a pydantic validator from a function returning a bool.
+
+    Example:
+
+        from typing import Any
+        from pydantic import BaseModel, ValidationError
+        from gwproto.property_format import predicate_validator
+
+        def is_truthy(v: Any) -> bool:
+            return bool(v)
+
+        class Foo(BaseModel):
+            an_int: int
+
+            _validate_an_int = predicate_validator("an_int", is_truthy)
+
+        print(Foo(an_int=1))
+
+        try:
+            print(Foo(an_int=0))
+        except ValidationError as e:
+            print(e)
+
+    Args:
+        field_name: the name of the field to validate.
+        predicate: the validation function. A truthy return value indicates success.
+        error_format: Optional format string for use in exception raised by validation failure. Takes one parameter, 'v'.
+        **kwargs: Passed to pydantic.validator()
+
+    Returns:
+        The passed in object v.
+    """
+
     def _validator(v: Any) -> Any:
         if not predicate(v):
             if error_format:
                 err_str = error_format.format(value=v)
             else:
-                err_str = f"{field_name}: {predicate} fails for [{v}]"
+                err_str = f"Failure of predicate on [{v}] with predicate {predicate}"
             raise ValueError(err_str)
         return v
 
-    return pydantic.validator(field_name, allow_reuse=True)(_validator)
+    return pydantic.validator(field_name, allow_reuse=True, **kwargs)(_validator)
 
 
 def is_hex_char(v: str) -> bool:
     """HexChar format: single-char string in '0123456789abcdefABCDEF'
 
     Returns:
         bool: True if HexChar, false else
@@ -476,15 +510,15 @@
     except:
         return False
     if len(root_g_node_alias_words) > 1:
         return False
     return True
 
 
-def check_is_market_type_name_lrd_format(v: str) -> None:
+def check_is_market_name(v: str) -> None:
     try:
         x = v.split(".")
     except AttributeError:
         raise ValueError(f"{v} failed to split on '.'")
     if not x[0] in MarketTypeName.values():
         raise ValueError(f"{v} not recognized MarketType")
     g_node_alias = ".".join(x[1:])
@@ -507,27 +541,25 @@
 
     """
     try:
         x = v.split(".")
     except AttributeError:
         raise ValueError(f"{v} failed to split on '.'")
     slot_start = x[-1]
-    if len(slot_start) != 10:
-        raise ValueError(f"slot start {slot_start} not of length 10")
     try:
         slot_start = int(slot_start)
     except ValueError:
         raise ValueError(f"slot start {slot_start} not an int")
+    check_is_reasonable_unix_time_s(slot_start)
     if slot_start % 300 != 0:
         raise ValueError(f"slot start {slot_start} not a multiple of 300")
 
-    market_type_name_lrd = ".".join(x[:-1])
+    market_name = ".".join(x[:-1])
     try:
-        check_is_market_type_name_lrd_format(market_type_name_lrd)
+        check_is_market_name(market_name)
     except ValueError as e:
         raise ValueError(f"e")
-
-    market_type = MarketType.by_id[market_type_name_lrd.split(".")[0]]
+    market_type = MarketType.by_id[MarketTypeName(x[0])]
     if not slot_start % (market_type.duration_minutes * 60) == 0:
         raise ValueError(
             f"market_slot_start_s mod {(market_type.duration_minutes * 60)} must be 0"
         )
```

### Comparing `gridworks-0.2.1/src/gridworks/rest_api.py` & `gridworks-0.2.2/src/gridworks/rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/types/g_node_gt.py` & `gridworks-0.2.2/src/gridworks/types/g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/types/g_node_instance_gt.py` & `gridworks-0.2.2/src/gridworks/types/g_node_instance_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/types/gw_cert_id.py` & `gridworks-0.2.2/src/gridworks/types/gw_cert_id.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/types/heartbeat_a.py` & `gridworks-0.2.2/src/gridworks/types/heartbeat_a.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/types/old_versions/heartbeat_a_001.py` & `gridworks-0.2.2/src/gridworks/types/old_versions/heartbeat_a_001.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/types/ready.py` & `gridworks-0.2.2/src/gridworks/types/ready.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/types/sim_timestep.py` & `gridworks-0.2.2/src/gridworks/types/sim_timestep.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/types/super_starter.py` & `gridworks-0.2.2/src/gridworks/types/super_starter.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/types/supervisor_container_gt.py` & `gridworks-0.2.2/src/gridworks/types/supervisor_container_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/src/gridworks/utils.py` & `gridworks-0.2.2/src/gridworks/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.1/PKG-INFO` & `gridworks-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks
-Version: 0.2.1
+Version: 0.2.2
 Summary: Gridworks
 Home-page: https://github.com/thegridelectric/gridworks
 License: MIT
 Author: GridWorks
 Author-email: gridworks@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -54,50 +54,48 @@
 [python version]: https://pypi.org/project/gridworks
 [read the docs]: https://gridworks.readthedocs.io/
 [tests]: https://github.com/thegridelectric/gridworks/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/thegridelectric/gridworks
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
-GridWorks uses distributed actors to balance the electric grid. What does this mean?  In today's world, more
+GridWorks uses distributed actors to balance the electric grid. What does this mean? In today's world, more
 power comes from highly variable power sources such as wind and solar. And yet, the number
-of electrons going into the grid must match the number coming out.  This is where GridWorks comes in.
+of electrons going into the grid must match the number coming out. This is where GridWorks comes in.
 GridWorks technology enables electrical devices with some embedded storage or with flexibility to provide grid
 balancing. Furthermore, GridWorks allows these appliances to be more thrifty, using electricity when
 it is cheap and green.
 
 To learn how using and contributing to GridWorks can support a cost-effective and rapid transition to a sustainable future:
 
 - Try some simple [Hello World](https://gridworks.readthedocs.io/en/latest/hello-gridworks.html) examples;
 - Read the [Millinocket Story](https://gridworks.readthedocs.io/en/latest/millinocket-demo.html) to learn how to exploit the synergy between wind power and space heating;
 - Go through the partner [Millinocket Tutorial](https://gridworks.readthedocs.io/en/latest/millinocket-tutorial.html).
 
 ## Blockchain Mechanics
 
-
 Gridworks runs markets between distributed actors acting as avatars for physical devices on the grid. It needs a
 foundation of trustless, secure, scalable validation and authentication. It heavily uses the Algorand blockchain. If
 you want to undestand more about how and why this is, go [here](blockchain.html).
 
 ## GridWorks SDKs
 
- - **gridworks**: [package](https://pypi.org/project/gridworks/) provides basic shared mechanics for  communication and GNode structure. It is used as a package in all of our other repos.
+- **gridworks**: [package](https://pypi.org/project/gridworks/) provides basic shared mechanics for communication and GNode structure. It is used as a package in all of our other repos.
 
- - **gridworks-atn**:  [package](https://pypi.org/project/gridworks-atn/) and associated [documentation](https://gridworks-atn.readthedocs.io/en/latest/) for the GridWorks Python [AtomicTNodes](https://gridworks.readthedocs.io/en/latest/atomic-t-node.html)  SDK. AtomicTNodes  are the GridWorks actors that make electrical devices *transactive*. This SDK is a great place to learn about blockchain mechanics, as it introduces some of the simpler structures (NFTs, stateless contracts, and then some simple stateful smart contracts constructed using  [beaker](https://github.com/algorand-devrel/beaker) ) required for establishing the link between physical reality on the electric grid and the actors that play their avatars in GridWorks.  
+- **gridworks-atn**: [package](https://pypi.org/project/gridworks-atn/) and associated [documentation](https://gridworks-atn.readthedocs.io/en/latest/) for the GridWorks Python [AtomicTNodes](https://gridworks.readthedocs.io/en/latest/atomic-t-node.html) SDK. AtomicTNodes are the GridWorks actors that make electrical devices _transactive_. This SDK is a great place to learn about blockchain mechanics, as it introduces some of the simpler structures (NFTs, stateless contracts, and then some simple stateful smart contracts constructed using [beaker](https://github.com/algorand-devrel/beaker) ) required for establishing the link between physical reality on the electric grid and the actors that play their avatars in GridWorks.
 
- - **gridworks-marketmaker**: [package](https://pypi.org/project/gridworks-marketmaker/) and associated [documentation](https://gridworks-marketmaker.readthedocs.io/en/latest/)  for our Python [MarketMaker](https://gridworks.readthedocs.io/en/latest/market-maker.html) SDK.  GridWorks uses distributed actors to balance the electric grid, and MarketMakers are the actors brokering this grid balancing via the markets they run for energy and balancing services.
+- **gridworks-marketmaker**: [package](https://pypi.org/project/gridworks-marketmaker/) and associated [documentation](https://gridworks-marketmaker.readthedocs.io/en/latest/) for our Python [MarketMaker](https://gridworks.readthedocs.io/en/latest/market-maker.html) SDK. GridWorks uses distributed actors to balance the electric grid, and MarketMakers are the actors brokering this grid balancing via the markets they run for energy and balancing services.
 
 There are several other open source GridWorks repos to explore on [our github page](https://github.com/thegridelectric),
 including the code running on the [SCADA systems](https://github.com/thegridelectric/gw-scada-spaceheat-python)
 that Efficiency Maine is deploying in Millinocket this winter.
-The  [GNodeFactory](https://github.com/thegridelectric/g-node-factory) currently hosts the demo,
-and  does most of the heavy lifting in terms of identity management and authentication in GridWorks. Finally, since the demo
+The [GNodeFactory](https://github.com/thegridelectric/g-node-factory) currently hosts the demo,
+and does most of the heavy lifting in terms of identity management and authentication in GridWorks. Finally, since the demo
 is a distributed simulation, it needs a method of handling time. That's done by a [TimeCoordinator](https://github.com/thegridelectric/gridworks-timecoordinator) GNode.
 
-
 ## Usage
 
 `pip install gridworks` to install the foundational package.
 
 ## Contributing
 
 Contributions are very welcome.
```

