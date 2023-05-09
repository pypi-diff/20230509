# Comparing `tmp/gridworks_protocol-0.4.5.tar.gz` & `tmp/gridworks_protocol-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_protocol-0.4.5.tar", max compression
+gzip compressed data, was "gridworks_protocol-0.5.0.tar", max compression
```

## Comparing `gridworks_protocol-0.4.5.tar` & `gridworks_protocol-0.5.0.tar`

### file list

```diff
@@ -1,85 +1,84 @@
--rw-r--r--   0        0        0     1070 2023-04-10 13:49:57.918573 gridworks_protocol-0.4.5/LICENSE
--rw-r--r--   0        0        0     2552 2023-04-10 13:49:57.918573 gridworks_protocol-0.4.5/README.md
--rw-r--r--   0        0        0     2287 2023-04-10 13:50:09.642840 gridworks_protocol-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1443 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/__init__.py
--rw-r--r--   0        0        0     6610 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/api_types.py
--rw-r--r--   0        0        0     1339 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/electric_meter_cac.py
--rw-r--r--   0        0        0     1488 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
--rw-r--r--   0        0        0      995 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
--rw-r--r--   0        0        0     1112 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/relay_cac.py
--rw-r--r--   0        0        0     1118 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/resistive_heater_cac.py
--rw-r--r--   0        0        0     1580 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
--rw-r--r--   0        0        0     1388 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/component.py
--rw-r--r--   0        0        0     1094 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/component_attribute_class.py
--rw-r--r--   0        0        0     1659 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/components/electric_meter_component.py
--rw-r--r--   0        0        0     1479 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/components/multipurpose_sensor_component.py
--rw-r--r--   0        0        0     1357 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
--rw-r--r--   0        0        0     1267 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/components/relay_component.py
--rw-r--r--   0        0        0     1465 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/components/resistive_heater_component.py
--rw-r--r--   0        0        0     1308 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/components/simple_temp_sensor_component.py
--rw-r--r--   0        0        0      165 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/errors.py
--rw-r--r--   0        0        0    14718 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/hardware_layout.py
--rw-r--r--   0        0        0      273 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/mixin.py
--rw-r--r--   0        0        0     1957 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/sh_node.py
--rw-r--r--   0        0        0      362 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/data_classes/telemetry_tuple.py
--rw-r--r--   0        0        0    12051 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/decoders.py
--rw-r--r--   0        0        0      451 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/enums/__init__.py
--rw-r--r--   0        0        0     3486 2023-04-10 13:50:09.642840 gridworks_protocol-0.4.5/src/gwproto/enums/actor_class.py
--rw-r--r--   0        0        0     1119 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/enums/local_comm_interface.py
--rw-r--r--   0        0        0     2657 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/enums/make_model.py
--rw-r--r--   0        0        0     3480 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/enums/role.py
--rw-r--r--   0        0        0     1823 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/enums/telemetry_name.py
--rw-r--r--   0        0        0     1148 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/enums/unit.py
--rw-r--r--   0        0        0       89 2023-04-10 13:49:57.922573 gridworks_protocol-0.4.5/src/gwproto/errors.py
--rw-r--r--   0        0        0      249 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/__init__.py
--rw-r--r--   0        0        0      464 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/gs_dispatch.py
--rw-r--r--   0        0        0      800 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/gs_dispatch_base.py
--rw-r--r--   0        0        0      678 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/gs_dispatch_maker.py
--rw-r--r--   0        0        0      446 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/gs_pwr.py
--rw-r--r--   0        0        0      851 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/gs_pwr_base.py
--rw-r--r--   0        0        0      609 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/gs/gs_pwr_maker.py
--rw-r--r--   0        0        0     3168 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/message.py
--rw-r--r--   0        0        0     1474 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/messages/__init__.py
--rw-r--r--   0        0        0     3058 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/messages/event.py
--rw-r--r--   0        0        0      669 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/messages/misc.py
--rw-r--r--   0        0        0     4045 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/property_format.py
--rw-r--r--   0        0        0        0 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/py.typed
--rw-r--r--   0        0        0     2892 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/topic.py
--rw-r--r--   0        0        0     6632 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/__init__.py
--rw-r--r--   0        0        0     5474 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/component_attribute_class_gt.py
--rw-r--r--   0        0        0     6119 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/component_gt.py
--rw-r--r--   0        0        0    10192 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/data_channel.py
--rw-r--r--   0        0        0     3892 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/egauge_io.py
--rw-r--r--   0        0        0     3603 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/egauge_register_config.py
--rw-r--r--   0        0        0    21265 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/electric_meter_cac_gt.py
--rw-r--r--   0        0        0    13413 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/electric_meter_component_gt.py
--rw-r--r--   0        0        0     7187 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_boolean_actuator_component.py
--rw-r--r--   0        0        0     8451 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0     5798 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_dispatch_boolean_local.py
--rw-r--r--   0        0        0     4973 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_driver_booleanactuator_cmd.py
--rw-r--r--   0        0        0     5584 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
--rw-r--r--   0        0        0     5327 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_cli_atn_cmd.py
--rw-r--r--   0        0        0    12792 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
--rw-r--r--   0        0        0    11884 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_simple_telemetry_status.py
--rw-r--r--   0        0        0    13663 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_status.py
--rw-r--r--   0        0        0    12350 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
--rw-r--r--   0        0        0     8389 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/gt_telemetry.py
--rw-r--r--   0        0        0     9471 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/heartbeat_b.py
--rw-r--r--   0        0        0    21597 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/multipurpose_sensor_cac_gt.py
--rw-r--r--   0        0        0     9935 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/multipurpose_sensor_component_gt.py
--rw-r--r--   0        0        0    11300 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/pipe_flow_sensor_cac_gt.py
--rw-r--r--   0        0        0     7622 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/pipe_flow_sensor_component_gt.py
--rw-r--r--   0        0        0     2761 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/power_watts.py
--rw-r--r--   0        0        0    11124 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/relay_cac_gt.py
--rw-r--r--   0        0        0     7616 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/relay_component_gt.py
--rw-r--r--   0        0        0    11736 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/resistive_heater_cac_gt.py
--rw-r--r--   0        0        0     8096 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/resistive_heater_component_gt.py
--rw-r--r--   0        0        0    20796 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/simple_temp_sensor_cac_gt.py
--rw-r--r--   0        0        0     7280 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/simple_temp_sensor_component_gt.py
--rw-r--r--   0        0        0     6007 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/snapshot_spaceheat.py
--rw-r--r--   0        0        0    18219 2023-04-10 13:50:09.642840 gridworks_protocol-0.4.5/src/gwproto/types/spaceheat_node_gt.py
--rw-r--r--   0        0        0    14059 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/telemetry_reporting_config.py
--rw-r--r--   0        0        0    12227 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/types/telemetry_snapshot_spaceheat.py
--rw-r--r--   0        0        0     2556 2023-04-10 13:49:57.926573 gridworks_protocol-0.4.5/src/gwproto/utils.py
--rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.5/setup.py
--rw-r--r--   0        0        0     3475 1970-01-01 00:00:00.000000 gridworks_protocol-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-09 20:27:48.290001 gridworks_protocol-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2552 2023-05-09 20:27:48.290001 gridworks_protocol-0.5.0/README.md
+-rw-r--r--   0        0        0     2307 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1439 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/__init__.py
+-rw-r--r--   0        0        0     1339 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/cacs/electric_meter_cac.py
+-rw-r--r--   0        0        0     1488 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py
+-rw-r--r--   0        0        0      995 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py
+-rw-r--r--   0        0        0     1112 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/cacs/relay_cac.py
+-rw-r--r--   0        0        0     1118 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/cacs/resistive_heater_cac.py
+-rw-r--r--   0        0        0     1580 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py
+-rw-r--r--   0        0        0     1388 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/component.py
+-rw-r--r--   0        0        0     1094 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/component_attribute_class.py
+-rw-r--r--   0        0        0     1659 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/components/electric_meter_component.py
+-rw-r--r--   0        0        0     1479 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/components/multipurpose_sensor_component.py
+-rw-r--r--   0        0        0     1357 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/components/pipe_flow_sensor_component.py
+-rw-r--r--   0        0        0     1267 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/components/relay_component.py
+-rw-r--r--   0        0        0     1465 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/components/resistive_heater_component.py
+-rw-r--r--   0        0        0     1308 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/components/simple_temp_sensor_component.py
+-rw-r--r--   0        0        0      165 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/errors.py
+-rw-r--r--   0        0        0    14718 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/hardware_layout.py
+-rw-r--r--   0        0        0      273 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/mixin.py
+-rw-r--r--   0        0        0     1957 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/sh_node.py
+-rw-r--r--   0        0        0      362 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/data_classes/telemetry_tuple.py
+-rw-r--r--   0        0        0    12051 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/decoders.py
+-rw-r--r--   0        0        0      451 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/enums/__init__.py
+-rw-r--r--   0        0        0     3486 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/enums/actor_class.py
+-rw-r--r--   0        0        0     1119 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/enums/local_comm_interface.py
+-rw-r--r--   0        0        0     2657 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/enums/make_model.py
+-rw-r--r--   0        0        0     3480 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/enums/role.py
+-rw-r--r--   0        0        0     1823 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/enums/telemetry_name.py
+-rw-r--r--   0        0        0     1148 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/enums/unit.py
+-rw-r--r--   0        0        0      160 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/errors.py
+-rw-r--r--   0        0        0      249 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/gs/__init__.py
+-rw-r--r--   0        0        0      460 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/gs/gs_dispatch.py
+-rw-r--r--   0        0        0      800 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/gs/gs_dispatch_base.py
+-rw-r--r--   0        0        0      678 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/gs/gs_dispatch_maker.py
+-rw-r--r--   0        0        0      442 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/gs/gs_pwr.py
+-rw-r--r--   0        0        0      851 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/gs/gs_pwr_base.py
+-rw-r--r--   0        0        0      609 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/gs/gs_pwr_maker.py
+-rw-r--r--   0        0        0     3168 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/message.py
+-rw-r--r--   0        0        0     1474 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/messages/__init__.py
+-rw-r--r--   0        0        0     3058 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/messages/event.py
+-rw-r--r--   0        0        0      669 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/messages/misc.py
+-rw-r--r--   0        0        0       40 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/property_format.py
+-rw-r--r--   0        0        0        0 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/py.typed
+-rw-r--r--   0        0        0     2892 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/topic.py
+-rw-r--r--   0        0        0     6632 2023-05-09 20:27:48.298002 gridworks_protocol-0.5.0/src/gwproto/types/__init__.py
+-rw-r--r--   0        0        0     5464 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/types/component_attribute_class_gt.py
+-rw-r--r--   0        0        0     6107 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/types/component_gt.py
+-rw-r--r--   0        0        0    10172 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/types/data_channel.py
+-rw-r--r--   0        0        0     3876 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/types/egauge_io.py
+-rw-r--r--   0        0        0     3583 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/types/egauge_register_config.py
+-rw-r--r--   0        0        0    21173 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/types/electric_meter_cac_gt.py
+-rw-r--r--   0        0        0    13387 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/types/electric_meter_component_gt.py
+-rw-r--r--   0        0        0     7175 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/types/gt_boolean_actuator_component.py
+-rw-r--r--   0        0        0     8431 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0     5782 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/types/gt_dispatch_boolean_local.py
+-rw-r--r--   0        0        0     4959 2023-05-09 20:28:04.658072 gridworks_protocol-0.5.0/src/gwproto/types/gt_driver_booleanactuator_cmd.py
+-rw-r--r--   0        0        0     5570 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py
+-rw-r--r--   0        0        0     5313 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/gt_sh_cli_atn_cmd.py
+-rw-r--r--   0        0        0    12770 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py
+-rw-r--r--   0        0        0    11864 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/gt_sh_simple_telemetry_status.py
+-rw-r--r--   0        0        0    13625 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/gt_sh_status.py
+-rw-r--r--   0        0        0    12328 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py
+-rw-r--r--   0        0        0     8369 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/gt_telemetry.py
+-rw-r--r--   0        0        0     9449 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/heartbeat_b.py
+-rw-r--r--   0        0        0    21533 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/multipurpose_sensor_cac_gt.py
+-rw-r--r--   0        0        0     9915 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/multipurpose_sensor_component_gt.py
+-rw-r--r--   0        0        0    11254 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/pipe_flow_sensor_cac_gt.py
+-rw-r--r--   0        0        0     7606 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/pipe_flow_sensor_component_gt.py
+-rw-r--r--   0        0        0     2751 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/power_watts.py
+-rw-r--r--   0        0        0    11076 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/relay_cac_gt.py
+-rw-r--r--   0        0        0     7602 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/relay_component_gt.py
+-rw-r--r--   0        0        0    11686 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/resistive_heater_cac_gt.py
+-rw-r--r--   0        0        0     8084 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/resistive_heater_component_gt.py
+-rw-r--r--   0        0        0    20734 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/simple_temp_sensor_cac_gt.py
+-rw-r--r--   0        0        0     7268 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/simple_temp_sensor_component_gt.py
+-rw-r--r--   0        0        0     5991 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/snapshot_spaceheat.py
+-rw-r--r--   0        0        0    18195 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/spaceheat_node_gt.py
+-rw-r--r--   0        0        0    14031 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/telemetry_reporting_config.py
+-rw-r--r--   0        0        0    12205 2023-05-09 20:28:04.662072 gridworks_protocol-0.5.0/src/gwproto/types/telemetry_snapshot_spaceheat.py
+-rw-r--r--   0        0        0     2556 2023-05-09 20:27:48.302002 gridworks_protocol-0.5.0/src/gwproto/utils.py
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 gridworks_protocol-0.5.0/setup.py
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 gridworks_protocol-0.5.0/PKG-INFO
```

### Comparing `gridworks_protocol-0.4.5/LICENSE` & `gridworks_protocol-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/README.md` & `gridworks_protocol-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/pyproject.toml` & `gridworks_protocol-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-protocol"
-version = "0.4.5"
+version = "0.5.0"
 description = "Gridworks Protocol"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-protocol"
 repository = "https://github.com/thegridelectric/gridworks-protocol"
 documentation = "https://gridworks-protocol.readthedocs.io"
@@ -19,14 +19,15 @@
 Changelog = "https://github.com/thegridelectric/gridworks-protocol/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <4.0"
 pydantic = "^1.10.2"
 pendulum = "^2.1.2"
 fastapi-utils = "^0.2.1"
+gridworks = "0.2.2"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/__init__.py` & `gridworks_protocol-0.5.0/src/gwproto/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from gwproto.decoders import MessageDiscriminator
 from gwproto.decoders import MQTTCodec
 from gwproto.decoders import OneDecoderExtractor
 from gwproto.decoders import PydanticDecoder
 from gwproto.decoders import create_message_payload_discriminator
 from gwproto.decoders import get_pydantic_literal_type_name
 from gwproto.decoders import pydantic_named_types
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import Header
 from gwproto.message import Message
 from gwproto.message import as_enum
 from gwproto.topic import DecodedMQTTTopic
 from gwproto.topic import MQTTTopic
 
 
@@ -34,15 +34,15 @@
     "get_pydantic_literal_type_name",
     "Header",
     "MakerDecoder",
     "MakerExtractor",
     "Message",
     "messages",
     "MessageDiscriminator",
-    "MpSchemaError",
+    "SchemaError",
     "MQTTCodec",
     "MQTTTopic",
     "OneDecoderExtractor",
     "property_format",
     "PydanticDecoder",
     "pydantic_named_types",
 ]
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/electric_meter_cac.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/cacs/electric_meter_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/cacs/multipurpose_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/cacs/pipe_flow_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/relay_cac.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/cacs/relay_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/resistive_heater_cac.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/cacs/resistive_heater_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/cacs/simple_temp_sensor_cac.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/component.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/component_attribute_class.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/component_attribute_class.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/components/electric_meter_component.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/components/electric_meter_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/components/multipurpose_sensor_component.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/components/multipurpose_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/components/pipe_flow_sensor_component.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/components/pipe_flow_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/components/relay_component.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/components/relay_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/components/resistive_heater_component.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/components/resistive_heater_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/components/simple_temp_sensor_component.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/components/simple_temp_sensor_component.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/hardware_layout.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/hardware_layout.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/data_classes/sh_node.py` & `gridworks_protocol-0.5.0/src/gwproto/data_classes/sh_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/decoders.py` & `gridworks_protocol-0.5.0/src/gwproto/decoders.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/enums/actor_class.py` & `gridworks_protocol-0.5.0/src/gwproto/enums/actor_class.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/enums/local_comm_interface.py` & `gridworks_protocol-0.5.0/src/gwproto/enums/local_comm_interface.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/enums/make_model.py` & `gridworks_protocol-0.5.0/src/gwproto/enums/make_model.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/enums/role.py` & `gridworks_protocol-0.5.0/src/gwproto/enums/role.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/enums/telemetry_name.py` & `gridworks_protocol-0.5.0/src/gwproto/enums/telemetry_name.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/enums/unit.py` & `gridworks_protocol-0.5.0/src/gwproto/enums/unit.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/gs/gs_dispatch_base.py` & `gridworks_protocol-0.5.0/src/gwproto/gs/gs_dispatch_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/gs/gs_dispatch_maker.py` & `gridworks_protocol-0.5.0/src/gwproto/gs/gs_dispatch_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/gs/gs_pwr_base.py` & `gridworks_protocol-0.5.0/src/gwproto/gs/gs_pwr_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/gs/gs_pwr_maker.py` & `gridworks_protocol-0.5.0/src/gwproto/gs/gs_pwr_maker.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/message.py` & `gridworks_protocol-0.5.0/src/gwproto/message.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/messages/__init__.py` & `gridworks_protocol-0.5.0/src/gwproto/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/messages/event.py` & `gridworks_protocol-0.5.0/src/gwproto/messages/event.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/messages/misc.py` & `gridworks_protocol-0.5.0/src/gwproto/messages/misc.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/topic.py` & `gridworks_protocol-0.5.0/src/gwproto/topic.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/__init__.py` & `gridworks_protocol-0.5.0/src/gwproto/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/component_attribute_class_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/component_attribute_class_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.component_attribute_class import ComponentAttributeClass
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
@@ -107,28 +107,28 @@
     def type_to_tuple(cls, t: str) -> ComponentAttributeClassGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> ComponentAttributeClassGt:
         d2 = dict(d)
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return ComponentAttributeClassGt(
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             DisplayName=d2["DisplayName"],
             TypeName=d2["TypeName"],
             Version="000",
         )
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/component_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/component_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.component import Component
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
@@ -133,32 +133,32 @@
     def type_to_tuple(cls, t: str) -> ComponentGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> ComponentGt:
         d2 = dict(d)
         if "ComponentId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentId")
+            raise SchemaError(f"dict {d2} missing ComponentId")
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "HwUid" not in d2.keys():
             d2["HwUid"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return ComponentGt(
             ComponentId=d2["ComponentId"],
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             DisplayName=d2["DisplayName"],
             HwUid=d2["HwUid"],
             TypeName=d2["TypeName"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/data_channel.py` & `gridworks_protocol-0.5.0/src/gwproto/types/data_channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from fastapi_utils.enums import StrEnum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.enums import TelemetryName as EnumTelemetryName
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatTelemetryName000SchemaEnum:
     enum_name: str = "spaceheat.telemetry.name.000"
     symbols: List[str] = [
         "00000000",
@@ -66,24 +66,24 @@
         return [elt.value for elt in cls]
 
 
 class TelemetryNameMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumTelemetryName:
         if not SpaceheatTelemetryName000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"{symbol} must belong to SpaceheatTelemetryName000 symbols"
             )
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumTelemetryName, EnumTelemetryName.default())
 
     @classmethod
     def local_to_type(cls, telemetry_name: EnumTelemetryName) -> str:
         if not isinstance(telemetry_name, EnumTelemetryName):
-            raise MpSchemaError(f"{telemetry_name} must be of type {EnumTelemetryName}")
+            raise SchemaError(f"{telemetry_name} must be of type {EnumTelemetryName}")
         versioned_enum = as_enum(
             telemetry_name,
             SpaceheatTelemetryName000,
             SpaceheatTelemetryName000.default(),
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
@@ -252,45 +252,45 @@
     def type_to_tuple(cls, t: str) -> DataChannel:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> DataChannel:
         d2 = dict(d)
         if "DisplayName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing DisplayName")
+            raise SchemaError(f"dict {d2} missing DisplayName")
         if "AboutName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing AboutName")
+            raise SchemaError(f"dict {d2} missing AboutName")
         if "FromName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing FromName")
+            raise SchemaError(f"dict {d2} missing FromName")
         if "TelemetryNameGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TelemetryNameGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing TelemetryNameGtEnumSymbol")
         if (
             d2["TelemetryNameGtEnumSymbol"]
             in SpaceheatTelemetryName000SchemaEnum.symbols
         ):
             d2["TelemetryName"] = TelemetryNameMap.type_to_local(
                 d2["TelemetryNameGtEnumSymbol"]
             )
         else:
             d2["TelemetryName"] = EnumTelemetryName.default()
         if "ExpectedMaxValue" not in d2.keys():
             d2["ExpectedMaxValue"] = None
         if "ExpectedMinValue" not in d2.keys():
             d2["ExpectedMinValue"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return DataChannel(
             DisplayName=d2["DisplayName"],
             AboutName=d2["AboutName"],
             FromName=d2["FromName"],
             TelemetryName=d2["TelemetryName"],
             ExpectedMaxValue=d2["ExpectedMaxValue"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/egauge_io.py` & `gridworks_protocol-0.5.0/src/gwproto/types/egauge_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.types.egauge_register_config import EgaugeRegisterConfig
 from gwproto.types.egauge_register_config import EgaugeRegisterConfig_Maker
 from gwproto.types.telemetry_reporting_config import TelemetryReportingConfig
 from gwproto.types.telemetry_reporting_config import TelemetryReportingConfig_Maker
 
 
 class EgaugeIo(BaseModel):
@@ -72,40 +72,40 @@
     def type_to_tuple(cls, t: str) -> EgaugeIo:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> EgaugeIo:
         d2 = dict(d)
         if "InputConfig" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing InputConfig")
+            raise SchemaError(f"dict {d2} missing InputConfig")
         if not isinstance(d2["InputConfig"], dict):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"d['InputConfig'] {d2['InputConfig']} must be a EgaugeRegisterConfig!"
             )
         input_config = EgaugeRegisterConfig_Maker.dict_to_tuple(d2["InputConfig"])
         d2["InputConfig"] = input_config
         if "OutputConfig" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing OutputConfig")
+            raise SchemaError(f"dict {d2} missing OutputConfig")
         if not isinstance(d2["OutputConfig"], dict):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"d['OutputConfig'] {d2['OutputConfig']} must be a TelemetryReportingConfig!"
             )
         output_config = TelemetryReportingConfig_Maker.dict_to_tuple(d2["OutputConfig"])
         d2["OutputConfig"] = output_config
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return EgaugeIo(
             InputConfig=d2["InputConfig"],
             OutputConfig=d2["OutputConfig"],
             TypeName=d2["TypeName"],
             Version="000",
         )
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/egauge_register_config.py` & `gridworks_protocol-0.5.0/src/gwproto/types/egauge_register_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 class EgaugeRegisterConfig(BaseModel):
     """
     Used to translate eGauge's Modbus Map
 
     This type captures the information provided by eGauge in its modbus csv map,
@@ -86,36 +86,36 @@
     def type_to_tuple(cls, t: str) -> EgaugeRegisterConfig:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> EgaugeRegisterConfig:
         d2 = dict(d)
         if "Address" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Address")
+            raise SchemaError(f"dict {d2} missing Address")
         if "Name" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Name")
+            raise SchemaError(f"dict {d2} missing Name")
         if "Description" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Description")
+            raise SchemaError(f"dict {d2} missing Description")
         if "Type" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Type")
+            raise SchemaError(f"dict {d2} missing Type")
         if "Denominator" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Denominator")
+            raise SchemaError(f"dict {d2} missing Denominator")
         if "Unit" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Unit")
+            raise SchemaError(f"dict {d2} missing Unit")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return EgaugeRegisterConfig(
             Address=d2["Address"],
             Name=d2["Name"],
             Description=d2["Description"],
             Type=d2["Type"],
             Denominator=d2["Denominator"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/electric_meter_cac_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/electric_meter_cac_gt.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.cacs.electric_meter_cac import ElectricMeterCac
 from gwproto.enums import LocalCommInterface
 from gwproto.enums import MakeModel as EnumMakeModel
 from gwproto.enums import TelemetryName
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatTelemetryName000SchemaEnum:
     enum_name: str = "spaceheat.telemetry.name.000"
     symbols: List[str] = [
         "00000000",
@@ -69,24 +69,24 @@
         return [elt.value for elt in cls]
 
 
 class TelemetryNameMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> TelemetryName:
         if not SpaceheatTelemetryName000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"{symbol} must belong to SpaceheatTelemetryName000 symbols"
             )
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, TelemetryName, TelemetryName.default())
 
     @classmethod
     def local_to_type(cls, telemetry_name: TelemetryName) -> str:
         if not isinstance(telemetry_name, TelemetryName):
-            raise MpSchemaError(f"{telemetry_name} must be of type {TelemetryName}")
+            raise SchemaError(f"{telemetry_name} must be of type {TelemetryName}")
         versioned_enum = as_enum(
             telemetry_name,
             SpaceheatTelemetryName000,
             SpaceheatTelemetryName000.default(),
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
@@ -164,24 +164,22 @@
         return [elt.value for elt in cls]
 
 
 class LocalCommInterfaceMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> LocalCommInterface:
         if not LocalCommInterface000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
-                f"{symbol} must belong to LocalCommInterface000 symbols"
-            )
+            raise SchemaError(f"{symbol} must belong to LocalCommInterface000 symbols")
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, LocalCommInterface, LocalCommInterface.default())
 
     @classmethod
     def local_to_type(cls, local_comm_interface: LocalCommInterface) -> str:
         if not isinstance(local_comm_interface, LocalCommInterface):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"{local_comm_interface} must be of type {LocalCommInterface}"
             )
         versioned_enum = as_enum(
             local_comm_interface, LocalCommInterface000, LocalCommInterface000.default()
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
@@ -261,24 +259,22 @@
         return [elt.value for elt in cls]
 
 
 class MakeModelMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumMakeModel:
         if not SpaceheatMakeModel000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
-                f"{symbol} must belong to SpaceheatMakeModel000 symbols"
-            )
+            raise SchemaError(f"{symbol} must belong to SpaceheatMakeModel000 symbols")
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumMakeModel, EnumMakeModel.default())
 
     @classmethod
     def local_to_type(cls, make_model: EnumMakeModel) -> str:
         if not isinstance(make_model, EnumMakeModel):
-            raise MpSchemaError(f"{make_model} must be of type {EnumMakeModel}")
+            raise SchemaError(f"{make_model} must be of type {EnumMakeModel}")
         versioned_enum = as_enum(
             make_model, SpaceheatMakeModel000, SpaceheatMakeModel000.default()
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
     type_to_versioned_enum_dict: Dict[str, SpaceheatMakeModel000] = {
         "00000000": SpaceheatMakeModel000.UNKNOWNMAKE__UNKNOWNMODEL,
@@ -478,59 +474,59 @@
     def type_to_tuple(cls, t: str) -> ElectricMeterCacGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> ElectricMeterCacGt:
         d2 = dict(d)
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "MakeModelGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
         if d2["MakeModelGtEnumSymbol"] in SpaceheatMakeModel000SchemaEnum.symbols:
             d2["MakeModel"] = MakeModelMap.type_to_local(d2["MakeModelGtEnumSymbol"])
         else:
             d2["MakeModel"] = EnumMakeModel.default()
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "TelemetryNameList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TelemetryNameList")
+            raise SchemaError(f"dict {d2} missing TelemetryNameList")
         telemetry_name_list = []
         if not isinstance(d2["TelemetryNameList"], List):
-            raise MpSchemaError("TelemetryNameList must be a List!")
+            raise SchemaError("TelemetryNameList must be a List!")
         for elt in d2["TelemetryNameList"]:
             if elt in SpaceheatTelemetryName000SchemaEnum.symbols:
                 v = TelemetryNameMap.type_to_local(elt)
             else:
                 v = SpaceheatTelemetryName000.Unknown  #
 
             telemetry_name_list.append(v)
         d2["TelemetryNameList"] = telemetry_name_list
         if "PollPeriodMs" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing PollPeriodMs")
+            raise SchemaError(f"dict {d2} missing PollPeriodMs")
         if "InterfaceGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing InterfaceGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing InterfaceGtEnumSymbol")
         if d2["InterfaceGtEnumSymbol"] in LocalCommInterface000SchemaEnum.symbols:
             d2["Interface"] = LocalCommInterfaceMap.type_to_local(
                 d2["InterfaceGtEnumSymbol"]
             )
         else:
             d2["Interface"] = LocalCommInterface.default()
         if "DefaultBaud" not in d2.keys():
             d2["DefaultBaud"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return ElectricMeterCacGt(
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             MakeModel=d2["MakeModel"],
             DisplayName=d2["DisplayName"],
             TelemetryNameList=d2["TelemetryNameList"],
             PollPeriodMs=d2["PollPeriodMs"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/electric_meter_component_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/electric_meter_component_gt.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pydantic import Field
 from pydantic import root_validator
 from pydantic import validator
 
 from gwproto.data_classes.components.electric_meter_component import (
     ElectricMeterComponent,
 )
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.types.egauge_io import EgaugeIo
 from gwproto.types.egauge_io import EgaugeIo_Maker
 from gwproto.types.telemetry_reporting_config import TelemetryReportingConfig
 from gwproto.types.telemetry_reporting_config import TelemetryReportingConfig_Maker
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
@@ -249,64 +249,64 @@
     def type_to_tuple(cls, t: str) -> ElectricMeterComponentGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> ElectricMeterComponentGt:
         d2 = dict(d)
         if "ComponentId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentId")
+            raise SchemaError(f"dict {d2} missing ComponentId")
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "ConfigList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ConfigList")
+            raise SchemaError(f"dict {d2} missing ConfigList")
         config_list = []
         if not isinstance(d2["ConfigList"], List):
-            raise MpSchemaError("ConfigList must be a List!")
+            raise SchemaError("ConfigList must be a List!")
         for elt in d2["ConfigList"]:
             if not isinstance(elt, dict):
-                raise MpSchemaError(
+                raise SchemaError(
                     f"elt {elt} of ConfigList must be "
                     "TelemetryReportingConfig but not even a dict!"
                 )
             config_list.append(TelemetryReportingConfig_Maker.dict_to_tuple(elt))
         d2["ConfigList"] = config_list
         if "HwUid" not in d2.keys():
             d2["HwUid"] = None
         if "ModbusHost" not in d2.keys():
             d2["ModbusHost"] = None
         if "ModbusPort" not in d2.keys():
             d2["ModbusPort"] = None
         if "EgaugeIoList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing EgaugeIoList")
+            raise SchemaError(f"dict {d2} missing EgaugeIoList")
         if "EgaugeIoList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing EgaugeIoList")
+            raise SchemaError(f"dict {d2} missing EgaugeIoList")
         egauge_io_list = []
         if not isinstance(d2["EgaugeIoList"], List):
-            raise MpSchemaError("EgaugeIoList must be a List!")
+            raise SchemaError("EgaugeIoList must be a List!")
         for elt in d2["EgaugeIoList"]:
             if not isinstance(elt, dict):
-                raise MpSchemaError(
+                raise SchemaError(
                     f"elt {elt} of EgaugeIoList must be "
                     "EgaugeIo but not even a dict!"
                 )
             egauge_io_list.append(EgaugeIo_Maker.dict_to_tuple(elt))
         d2["EgaugeIoList"] = egauge_io_list
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return ElectricMeterComponentGt(
             ComponentId=d2["ComponentId"],
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             DisplayName=d2["DisplayName"],
             ConfigList=d2["ConfigList"],
             HwUid=d2["HwUid"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/gt_boolean_actuator_component.py` & `gridworks_protocol-0.5.0/src/gwproto/types/gt_boolean_actuator_component.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.components.boolean_actuator_component import (
     BooleanActuatorComponent,
 )
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
@@ -150,34 +150,34 @@
     def type_to_tuple(cls, t: str) -> GtBooleanActuatorComponent:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> GtBooleanActuatorComponent:
         d2 = dict(d)
         if "ComponentId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentId")
+            raise SchemaError(f"dict {d2} missing ComponentId")
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "Gpio" not in d2.keys():
             d2["Gpio"] = None
         if "HwUid" not in d2.keys():
             d2["HwUid"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return GtBooleanActuatorComponent(
             ComponentId=d2["ComponentId"],
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             DisplayName=d2["DisplayName"],
             Gpio=d2["Gpio"],
             HwUid=d2["HwUid"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/gt_dispatch_boolean.py` & `gridworks_protocol-0.5.0/src/gwproto/types/gt_dispatch_boolean.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
@@ -216,36 +216,36 @@
     def type_to_tuple(cls, t: str) -> GtDispatchBoolean:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> GtDispatchBoolean:
         d2 = dict(d)
         if "AboutNodeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing AboutNodeName")
+            raise SchemaError(f"dict {d2} missing AboutNodeName")
         if "ToGNodeAlias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ToGNodeAlias")
+            raise SchemaError(f"dict {d2} missing ToGNodeAlias")
         if "FromGNodeAlias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing FromGNodeAlias")
+            raise SchemaError(f"dict {d2} missing FromGNodeAlias")
         if "FromGNodeInstanceId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing FromGNodeInstanceId")
+            raise SchemaError(f"dict {d2} missing FromGNodeInstanceId")
         if "RelayState" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing RelayState")
+            raise SchemaError(f"dict {d2} missing RelayState")
         if "SendTimeUnixMs" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing SendTimeUnixMs")
+            raise SchemaError(f"dict {d2} missing SendTimeUnixMs")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return GtDispatchBoolean(
             AboutNodeName=d2["AboutNodeName"],
             ToGNodeAlias=d2["ToGNodeAlias"],
             FromGNodeAlias=d2["FromGNodeAlias"],
             FromGNodeInstanceId=d2["FromGNodeInstanceId"],
             RelayState=d2["RelayState"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/gt_dispatch_boolean_local.py` & `gridworks_protocol-0.5.0/src/gwproto/types/gt_dispatch_boolean_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_left_right_dot(v: str) -> None:
     """Checks LeftRightDot Format
 
     LeftRightDot format: Lowercase alphanumeric words separated by periods,
     most significant word (on the left) starting with an alphabet character.
@@ -149,32 +149,32 @@
     def type_to_tuple(cls, t: str) -> GtDispatchBooleanLocal:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> GtDispatchBooleanLocal:
         d2 = dict(d)
         if "RelayState" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing RelayState")
+            raise SchemaError(f"dict {d2} missing RelayState")
         if "AboutNodeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing AboutNodeName")
+            raise SchemaError(f"dict {d2} missing AboutNodeName")
         if "FromNodeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing FromNodeName")
+            raise SchemaError(f"dict {d2} missing FromNodeName")
         if "SendTimeUnixMs" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing SendTimeUnixMs")
+            raise SchemaError(f"dict {d2} missing SendTimeUnixMs")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return GtDispatchBooleanLocal(
             RelayState=d2["RelayState"],
             AboutNodeName=d2["AboutNodeName"],
             FromNodeName=d2["FromNodeName"],
             SendTimeUnixMs=d2["SendTimeUnixMs"],
             TypeName=d2["TypeName"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/gt_driver_booleanactuator_cmd.py` & `gridworks_protocol-0.5.0/src/gwproto/types/gt_driver_booleanactuator_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_left_right_dot(v: str) -> None:
     """Checks LeftRightDot Format
 
     LeftRightDot format: Lowercase alphanumeric words separated by periods,
     most significant word (on the left) starting with an alphabet character.
@@ -126,30 +126,30 @@
     def type_to_tuple(cls, t: str) -> GtDriverBooleanactuatorCmd:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> GtDriverBooleanactuatorCmd:
         d2 = dict(d)
         if "RelayState" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing RelayState")
+            raise SchemaError(f"dict {d2} missing RelayState")
         if "ShNodeAlias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ShNodeAlias")
+            raise SchemaError(f"dict {d2} missing ShNodeAlias")
         if "CommandTimeUnixMs" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing CommandTimeUnixMs")
+            raise SchemaError(f"dict {d2} missing CommandTimeUnixMs")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return GtDriverBooleanactuatorCmd(
             RelayState=d2["RelayState"],
             ShNodeAlias=d2["ShNodeAlias"],
             CommandTimeUnixMs=d2["CommandTimeUnixMs"],
             TypeName=d2["TypeName"],
             Version="100",
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py` & `gridworks_protocol-0.5.0/src/gwproto/types/gt_sh_booleanactuator_cmd_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List
 from typing import Literal
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_left_right_dot(v: str) -> None:
     """Checks LeftRightDot Format
 
     LeftRightDot format: Lowercase alphanumeric words separated by periods,
     most significant word (on the left) starting with an alphabet character.
@@ -136,30 +136,30 @@
     def type_to_tuple(cls, t: str) -> GtShBooleanactuatorCmdStatus:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> GtShBooleanactuatorCmdStatus:
         d2 = dict(d)
         if "ShNodeAlias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ShNodeAlias")
+            raise SchemaError(f"dict {d2} missing ShNodeAlias")
         if "RelayStateCommandList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing RelayStateCommandList")
+            raise SchemaError(f"dict {d2} missing RelayStateCommandList")
         if "CommandTimeUnixMsList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing CommandTimeUnixMsList")
+            raise SchemaError(f"dict {d2} missing CommandTimeUnixMsList")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return GtShBooleanactuatorCmdStatus(
             ShNodeAlias=d2["ShNodeAlias"],
             RelayStateCommandList=d2["RelayStateCommandList"],
             CommandTimeUnixMsList=d2["CommandTimeUnixMsList"],
             TypeName=d2["TypeName"],
             Version="100",
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_cli_atn_cmd.py` & `gridworks_protocol-0.5.0/src/gwproto/types/gt_sh_cli_atn_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
@@ -146,30 +146,30 @@
     def type_to_tuple(cls, t: str) -> GtShCliAtnCmd:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> GtShCliAtnCmd:
         d2 = dict(d)
         if "FromGNodeAlias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing FromGNodeAlias")
+            raise SchemaError(f"dict {d2} missing FromGNodeAlias")
         if "SendSnapshot" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing SendSnapshot")
+            raise SchemaError(f"dict {d2} missing SendSnapshot")
         if "FromGNodeId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing FromGNodeId")
+            raise SchemaError(f"dict {d2} missing FromGNodeId")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return GtShCliAtnCmd(
             FromGNodeAlias=d2["FromGNodeAlias"],
             SendSnapshot=d2["SendSnapshot"],
             FromGNodeId=d2["FromGNodeId"],
             TypeName=d2["TypeName"],
             Version="110",
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py` & `gridworks_protocol-0.5.0/src/gwproto/types/gt_sh_multipurpose_telemetry_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from fastapi_utils.enums import StrEnum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import root_validator
 from pydantic import validator
 
 from gwproto.enums import TelemetryName as EnumTelemetryName
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatTelemetryName000SchemaEnum:
     enum_name: str = "spaceheat.telemetry.name.000"
     symbols: List[str] = [
         "00000000",
@@ -66,24 +66,24 @@
         return [elt.value for elt in cls]
 
 
 class TelemetryNameMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumTelemetryName:
         if not SpaceheatTelemetryName000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"{symbol} must belong to SpaceheatTelemetryName000 symbols"
             )
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumTelemetryName, EnumTelemetryName.default())
 
     @classmethod
     def local_to_type(cls, telemetry_name: EnumTelemetryName) -> str:
         if not isinstance(telemetry_name, EnumTelemetryName):
-            raise MpSchemaError(f"{telemetry_name} must be of type {EnumTelemetryName}")
+            raise SchemaError(f"{telemetry_name} must be of type {EnumTelemetryName}")
         versioned_enum = as_enum(
             telemetry_name,
             SpaceheatTelemetryName000,
             SpaceheatTelemetryName000.default(),
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
@@ -290,43 +290,43 @@
     def type_to_tuple(cls, t: str) -> GtShMultipurposeTelemetryStatus:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> GtShMultipurposeTelemetryStatus:
         d2 = dict(d)
         if "AboutNodeAlias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing AboutNodeAlias")
+            raise SchemaError(f"dict {d2} missing AboutNodeAlias")
         if "TelemetryNameGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TelemetryNameGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing TelemetryNameGtEnumSymbol")
         if (
             d2["TelemetryNameGtEnumSymbol"]
             in SpaceheatTelemetryName000SchemaEnum.symbols
         ):
             d2["TelemetryName"] = TelemetryNameMap.type_to_local(
                 d2["TelemetryNameGtEnumSymbol"]
             )
         else:
             d2["TelemetryName"] = EnumTelemetryName.default()
         if "ValueList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ValueList")
+            raise SchemaError(f"dict {d2} missing ValueList")
         if "ReadTimeUnixMsList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ReadTimeUnixMsList")
+            raise SchemaError(f"dict {d2} missing ReadTimeUnixMsList")
         if "SensorNodeAlias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing SensorNodeAlias")
+            raise SchemaError(f"dict {d2} missing SensorNodeAlias")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return GtShMultipurposeTelemetryStatus(
             AboutNodeAlias=d2["AboutNodeAlias"],
             TelemetryName=d2["TelemetryName"],
             ValueList=d2["ValueList"],
             ReadTimeUnixMsList=d2["ReadTimeUnixMsList"],
             SensorNodeAlias=d2["SensorNodeAlias"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_simple_telemetry_status.py` & `gridworks_protocol-0.5.0/src/gwproto/types/gt_sh_simple_telemetry_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from fastapi_utils.enums import StrEnum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import root_validator
 from pydantic import validator
 
 from gwproto.enums import TelemetryName as EnumTelemetryName
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatTelemetryName000SchemaEnum:
     enum_name: str = "spaceheat.telemetry.name.000"
     symbols: List[str] = [
         "00000000",
@@ -66,24 +66,24 @@
         return [elt.value for elt in cls]
 
 
 class TelemetryNameMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumTelemetryName:
         if not SpaceheatTelemetryName000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"{symbol} must belong to SpaceheatTelemetryName000 symbols"
             )
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumTelemetryName, EnumTelemetryName.default())
 
     @classmethod
     def local_to_type(cls, telemetry_name: EnumTelemetryName) -> str:
         if not isinstance(telemetry_name, EnumTelemetryName):
-            raise MpSchemaError(f"{telemetry_name} must be of type {EnumTelemetryName}")
+            raise SchemaError(f"{telemetry_name} must be of type {EnumTelemetryName}")
         versioned_enum = as_enum(
             telemetry_name,
             SpaceheatTelemetryName000,
             SpaceheatTelemetryName000.default(),
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
@@ -280,41 +280,41 @@
     def type_to_tuple(cls, t: str) -> GtShSimpleTelemetryStatus:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> GtShSimpleTelemetryStatus:
         d2 = dict(d)
         if "ValueList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ValueList")
+            raise SchemaError(f"dict {d2} missing ValueList")
         if "ReadTimeUnixMsList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ReadTimeUnixMsList")
+            raise SchemaError(f"dict {d2} missing ReadTimeUnixMsList")
         if "TelemetryNameGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TelemetryNameGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing TelemetryNameGtEnumSymbol")
         if (
             d2["TelemetryNameGtEnumSymbol"]
             in SpaceheatTelemetryName000SchemaEnum.symbols
         ):
             d2["TelemetryName"] = TelemetryNameMap.type_to_local(
                 d2["TelemetryNameGtEnumSymbol"]
             )
         else:
             d2["TelemetryName"] = EnumTelemetryName.default()
         if "ShNodeAlias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ShNodeAlias")
+            raise SchemaError(f"dict {d2} missing ShNodeAlias")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return GtShSimpleTelemetryStatus(
             ValueList=d2["ValueList"],
             ReadTimeUnixMsList=d2["ReadTimeUnixMsList"],
             TelemetryName=d2["TelemetryName"],
             ShNodeAlias=d2["ShNodeAlias"],
             TypeName=d2["TypeName"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_status.py` & `gridworks_protocol-0.5.0/src/gwproto/types/gt_sh_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List
 from typing import Literal
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.types.gt_sh_booleanactuator_cmd_status import GtShBooleanactuatorCmdStatus
 from gwproto.types.gt_sh_booleanactuator_cmd_status import (
     GtShBooleanactuatorCmdStatus_Maker,
 )
 from gwproto.types.gt_sh_multipurpose_telemetry_status import (
     GtShMultipurposeTelemetryStatus,
 )
@@ -289,81 +289,81 @@
     def type_to_tuple(cls, t: str) -> GtShStatus:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> GtShStatus:
         d2 = dict(d)
         if "FromGNodeAlias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing FromGNodeAlias")
+            raise SchemaError(f"dict {d2} missing FromGNodeAlias")
         if "FromGNodeId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing FromGNodeId")
+            raise SchemaError(f"dict {d2} missing FromGNodeId")
         if "AboutGNodeAlias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing AboutGNodeAlias")
+            raise SchemaError(f"dict {d2} missing AboutGNodeAlias")
         if "SlotStartUnixS" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing SlotStartUnixS")
+            raise SchemaError(f"dict {d2} missing SlotStartUnixS")
         if "ReportingPeriodS" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ReportingPeriodS")
+            raise SchemaError(f"dict {d2} missing ReportingPeriodS")
         if "SimpleTelemetryList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing SimpleTelemetryList")
+            raise SchemaError(f"dict {d2} missing SimpleTelemetryList")
         simple_telemetry_list = []
         if not isinstance(d2["SimpleTelemetryList"], List):
-            raise MpSchemaError("SimpleTelemetryList must be a List!")
+            raise SchemaError("SimpleTelemetryList must be a List!")
         for elt in d2["SimpleTelemetryList"]:
             if not isinstance(elt, dict):
-                raise MpSchemaError(
+                raise SchemaError(
                     f"elt {elt} of SimpleTelemetryList must be "
                     "GtShSimpleTelemetryStatus but not even a dict!"
                 )
             simple_telemetry_list.append(
                 GtShSimpleTelemetryStatus_Maker.dict_to_tuple(elt)
             )
         d2["SimpleTelemetryList"] = simple_telemetry_list
         if "MultipurposeTelemetryList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing MultipurposeTelemetryList")
+            raise SchemaError(f"dict {d2} missing MultipurposeTelemetryList")
         multipurpose_telemetry_list = []
         if not isinstance(d2["MultipurposeTelemetryList"], List):
-            raise MpSchemaError("MultipurposeTelemetryList must be a List!")
+            raise SchemaError("MultipurposeTelemetryList must be a List!")
         for elt in d2["MultipurposeTelemetryList"]:
             if not isinstance(elt, dict):
-                raise MpSchemaError(
+                raise SchemaError(
                     f"elt {elt} of MultipurposeTelemetryList must be "
                     "GtShMultipurposeTelemetryStatus but not even a dict!"
                 )
             multipurpose_telemetry_list.append(
                 GtShMultipurposeTelemetryStatus_Maker.dict_to_tuple(elt)
             )
         d2["MultipurposeTelemetryList"] = multipurpose_telemetry_list
         if "BooleanactuatorCmdList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing BooleanactuatorCmdList")
+            raise SchemaError(f"dict {d2} missing BooleanactuatorCmdList")
         booleanactuator_cmd_list = []
         if not isinstance(d2["BooleanactuatorCmdList"], List):
-            raise MpSchemaError("BooleanactuatorCmdList must be a List!")
+            raise SchemaError("BooleanactuatorCmdList must be a List!")
         for elt in d2["BooleanactuatorCmdList"]:
             if not isinstance(elt, dict):
-                raise MpSchemaError(
+                raise SchemaError(
                     f"elt {elt} of BooleanactuatorCmdList must be "
                     "GtShBooleanactuatorCmdStatus but not even a dict!"
                 )
             booleanactuator_cmd_list.append(
                 GtShBooleanactuatorCmdStatus_Maker.dict_to_tuple(elt)
             )
         d2["BooleanactuatorCmdList"] = booleanactuator_cmd_list
         if "StatusUid" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing StatusUid")
+            raise SchemaError(f"dict {d2} missing StatusUid")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return GtShStatus(
             FromGNodeAlias=d2["FromGNodeAlias"],
             FromGNodeId=d2["FromGNodeId"],
             AboutGNodeAlias=d2["AboutGNodeAlias"],
             SlotStartUnixS=d2["SlotStartUnixS"],
             ReportingPeriodS=d2["ReportingPeriodS"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py` & `gridworks_protocol-0.5.0/src/gwproto/types/gt_sh_telemetry_from_multipurpose_sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from fastapi_utils.enums import StrEnum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import root_validator
 from pydantic import validator
 
 from gwproto.enums import TelemetryName
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatTelemetryName000SchemaEnum:
     enum_name: str = "spaceheat.telemetry.name.000"
     symbols: List[str] = [
         "00000000",
@@ -66,24 +66,24 @@
         return [elt.value for elt in cls]
 
 
 class TelemetryNameMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> TelemetryName:
         if not SpaceheatTelemetryName000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"{symbol} must belong to SpaceheatTelemetryName000 symbols"
             )
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, TelemetryName, TelemetryName.default())
 
     @classmethod
     def local_to_type(cls, telemetry_name: TelemetryName) -> str:
         if not isinstance(telemetry_name, TelemetryName):
-            raise MpSchemaError(f"{telemetry_name} must be of type {TelemetryName}")
+            raise SchemaError(f"{telemetry_name} must be of type {TelemetryName}")
         versioned_enum = as_enum(
             telemetry_name,
             SpaceheatTelemetryName000,
             SpaceheatTelemetryName000.default(),
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
@@ -290,43 +290,43 @@
     def type_to_tuple(cls, t: str) -> GtShTelemetryFromMultipurposeSensor:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> GtShTelemetryFromMultipurposeSensor:
         d2 = dict(d)
         if "AboutNodeAliasList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing AboutNodeAliasList")
+            raise SchemaError(f"dict {d2} missing AboutNodeAliasList")
         if "ValueList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ValueList")
+            raise SchemaError(f"dict {d2} missing ValueList")
         if "ScadaReadTimeUnixMs" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ScadaReadTimeUnixMs")
+            raise SchemaError(f"dict {d2} missing ScadaReadTimeUnixMs")
         if "TelemetryNameList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TelemetryNameList")
+            raise SchemaError(f"dict {d2} missing TelemetryNameList")
         telemetry_name_list = []
         if not isinstance(d2["TelemetryNameList"], List):
-            raise MpSchemaError("TelemetryNameList must be a List!")
+            raise SchemaError("TelemetryNameList must be a List!")
         for elt in d2["TelemetryNameList"]:
             if elt in SpaceheatTelemetryName000SchemaEnum.symbols:
                 v = TelemetryNameMap.type_to_local(elt)
             else:
                 v = SpaceheatTelemetryName000.Unknown  #
 
             telemetry_name_list.append(v)
         d2["TelemetryNameList"] = telemetry_name_list
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return GtShTelemetryFromMultipurposeSensor(
             AboutNodeAliasList=d2["AboutNodeAliasList"],
             ValueList=d2["ValueList"],
             ScadaReadTimeUnixMs=d2["ScadaReadTimeUnixMs"],
             TelemetryNameList=d2["TelemetryNameList"],
             TypeName=d2["TypeName"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/gt_telemetry.py` & `gridworks_protocol-0.5.0/src/gwproto/types/gt_telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from fastapi_utils.enums import StrEnum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.enums import TelemetryName
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatTelemetryName000SchemaEnum:
     enum_name: str = "spaceheat.telemetry.name.000"
     symbols: List[str] = [
         "00000000",
@@ -65,24 +65,24 @@
         return [elt.value for elt in cls]
 
 
 class TelemetryNameMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> TelemetryName:
         if not SpaceheatTelemetryName000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"{symbol} must belong to SpaceheatTelemetryName000 symbols"
             )
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, TelemetryName, TelemetryName.default())
 
     @classmethod
     def local_to_type(cls, telemetry_name: TelemetryName) -> str:
         if not isinstance(telemetry_name, TelemetryName):
-            raise MpSchemaError(f"{telemetry_name} must be of type {TelemetryName}")
+            raise SchemaError(f"{telemetry_name} must be of type {TelemetryName}")
         versioned_enum = as_enum(
             telemetry_name,
             SpaceheatTelemetryName000,
             SpaceheatTelemetryName000.default(),
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
@@ -214,36 +214,36 @@
     def type_to_tuple(cls, t: str) -> GtTelemetry:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> GtTelemetry:
         d2 = dict(d)
         if "ScadaReadTimeUnixMs" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ScadaReadTimeUnixMs")
+            raise SchemaError(f"dict {d2} missing ScadaReadTimeUnixMs")
         if "Value" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Value")
+            raise SchemaError(f"dict {d2} missing Value")
         if "NameGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing NameGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing NameGtEnumSymbol")
         if d2["NameGtEnumSymbol"] in SpaceheatTelemetryName000SchemaEnum.symbols:
             d2["Name"] = TelemetryNameMap.type_to_local(d2["NameGtEnumSymbol"])
         else:
             d2["Name"] = TelemetryName.default()
         if "Exponent" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Exponent")
+            raise SchemaError(f"dict {d2} missing Exponent")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return GtTelemetry(
             ScadaReadTimeUnixMs=d2["ScadaReadTimeUnixMs"],
             Value=d2["Value"],
             Name=d2["Name"],
             Exponent=d2["Exponent"],
             TypeName=d2["TypeName"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/heartbeat_b.py` & `gridworks_protocol-0.5.0/src/gwproto/types/heartbeat_b.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
@@ -248,38 +248,38 @@
     def type_to_tuple(cls, t: str) -> HeartbeatB:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> HeartbeatB:
         d2 = dict(d)
         if "FromGNodeAlias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing FromGNodeAlias")
+            raise SchemaError(f"dict {d2} missing FromGNodeAlias")
         if "FromGNodeInstanceId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing FromGNodeInstanceId")
+            raise SchemaError(f"dict {d2} missing FromGNodeInstanceId")
         if "MyHex" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing MyHex")
+            raise SchemaError(f"dict {d2} missing MyHex")
         if "YourLastHex" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing YourLastHex")
+            raise SchemaError(f"dict {d2} missing YourLastHex")
         if "LastReceivedTimeUnixMs" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing LastReceivedTimeUnixMs")
+            raise SchemaError(f"dict {d2} missing LastReceivedTimeUnixMs")
         if "SendTimeUnixMs" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing SendTimeUnixMs")
+            raise SchemaError(f"dict {d2} missing SendTimeUnixMs")
         if "StartingOver" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing StartingOver")
+            raise SchemaError(f"dict {d2} missing StartingOver")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return HeartbeatB(
             FromGNodeAlias=d2["FromGNodeAlias"],
             FromGNodeInstanceId=d2["FromGNodeInstanceId"],
             MyHex=d2["MyHex"],
             YourLastHex=d2["YourLastHex"],
             LastReceivedTimeUnixMs=d2["LastReceivedTimeUnixMs"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/multipurpose_sensor_cac_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/multipurpose_sensor_cac_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.cacs.multipurpose_sensor_cac import MultipurposeSensorCac
 from gwproto.enums import MakeModel as EnumMakeModel
 from gwproto.enums import TelemetryName
 from gwproto.enums import Unit
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatTelemetryName000SchemaEnum:
     enum_name: str = "spaceheat.telemetry.name.000"
     symbols: List[str] = [
         "00000000",
@@ -69,24 +69,24 @@
         return [elt.value for elt in cls]
 
 
 class TelemetryNameMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> TelemetryName:
         if not SpaceheatTelemetryName000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"{symbol} must belong to SpaceheatTelemetryName000 symbols"
             )
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, TelemetryName, TelemetryName.default())
 
     @classmethod
     def local_to_type(cls, telemetry_name: TelemetryName) -> str:
         if not isinstance(telemetry_name, TelemetryName):
-            raise MpSchemaError(f"{telemetry_name} must be of type {TelemetryName}")
+            raise SchemaError(f"{telemetry_name} must be of type {TelemetryName}")
         versioned_enum = as_enum(
             telemetry_name,
             SpaceheatTelemetryName000,
             SpaceheatTelemetryName000.default(),
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
@@ -174,24 +174,22 @@
         return [elt.value for elt in cls]
 
 
 class MakeModelMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumMakeModel:
         if not SpaceheatMakeModel000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
-                f"{symbol} must belong to SpaceheatMakeModel000 symbols"
-            )
+            raise SchemaError(f"{symbol} must belong to SpaceheatMakeModel000 symbols")
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumMakeModel, EnumMakeModel.default())
 
     @classmethod
     def local_to_type(cls, make_model: EnumMakeModel) -> str:
         if not isinstance(make_model, EnumMakeModel):
-            raise MpSchemaError(f"{make_model} must be of type {EnumMakeModel}")
+            raise SchemaError(f"{make_model} must be of type {EnumMakeModel}")
         versioned_enum = as_enum(
             make_model, SpaceheatMakeModel000, SpaceheatMakeModel000.default()
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
     type_to_versioned_enum_dict: Dict[str, SpaceheatMakeModel000] = {
         "00000000": SpaceheatMakeModel000.UNKNOWNMAKE__UNKNOWNMODEL,
@@ -271,22 +269,22 @@
         return [elt.value for elt in cls]
 
 
 class UnitMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> Unit:
         if not SpaceheatUnit000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(f"{symbol} must belong to SpaceheatUnit000 symbols")
+            raise SchemaError(f"{symbol} must belong to SpaceheatUnit000 symbols")
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, Unit, Unit.default())
 
     @classmethod
     def local_to_type(cls, unit: Unit) -> str:
         if not isinstance(unit, Unit):
-            raise MpSchemaError(f"{unit} must be of type {Unit}")
+            raise SchemaError(f"{unit} must be of type {Unit}")
         versioned_enum = as_enum(unit, SpaceheatUnit000, SpaceheatUnit000.default())
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
     type_to_versioned_enum_dict: Dict[str, SpaceheatUnit000] = {
         "00000000": SpaceheatUnit000.Unknown,
         "ec972387": SpaceheatUnit000.Unitless,
         "f459a9c3": SpaceheatUnit000.W,
@@ -488,45 +486,45 @@
     def type_to_tuple(cls, t: str) -> MultipurposeSensorCacGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> MultipurposeSensorCacGt:
         d2 = dict(d)
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "MakeModelGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
         if d2["MakeModelGtEnumSymbol"] in SpaceheatMakeModel000SchemaEnum.symbols:
             d2["MakeModel"] = MakeModelMap.type_to_local(d2["MakeModelGtEnumSymbol"])
         else:
             d2["MakeModel"] = EnumMakeModel.default()
         if "PollPeriodMs" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing PollPeriodMs")
+            raise SchemaError(f"dict {d2} missing PollPeriodMs")
         if "Exponent" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Exponent")
+            raise SchemaError(f"dict {d2} missing Exponent")
         if "TempUnitGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TempUnitGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing TempUnitGtEnumSymbol")
         if d2["TempUnitGtEnumSymbol"] in SpaceheatUnit000SchemaEnum.symbols:
             d2["TempUnit"] = UnitMap.type_to_local(d2["TempUnitGtEnumSymbol"])
         else:
             d2["TempUnit"] = Unit.default()
         if "TelemetryNameList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TelemetryNameList")
+            raise SchemaError(f"dict {d2} missing TelemetryNameList")
         telemetry_name_list = []
         if not isinstance(d2["TelemetryNameList"], List):
-            raise MpSchemaError("TelemetryNameList must be a List!")
+            raise SchemaError("TelemetryNameList must be a List!")
         for elt in d2["TelemetryNameList"]:
             if elt in SpaceheatTelemetryName000SchemaEnum.symbols:
                 v = TelemetryNameMap.type_to_local(elt)
             else:
                 v = SpaceheatTelemetryName000.Unknown  #
 
             telemetry_name_list.append(v)
@@ -534,15 +532,15 @@
         if "MaxThermistors" not in d2.keys():
             d2["MaxThermistors"] = None
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "CommsMethod" not in d2.keys():
             d2["CommsMethod"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return MultipurposeSensorCacGt(
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             MakeModel=d2["MakeModel"],
             PollPeriodMs=d2["PollPeriodMs"],
             Exponent=d2["Exponent"],
             TempUnit=d2["TempUnit"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/multipurpose_sensor_component_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/multipurpose_sensor_component_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.components.multipurpose_sensor_component import (
     MultipurposeSensorComponent,
 )
 from gwproto.enums import TelemetryName
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.types.telemetry_reporting_config import TelemetryReportingConfig
 from gwproto.types.telemetry_reporting_config import TelemetryReportingConfig_Maker
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
@@ -201,47 +201,47 @@
     def type_to_tuple(cls, t: str) -> MultipurposeSensorComponentGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> MultipurposeSensorComponentGt:
         d2 = dict(d)
         if "ComponentId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentId")
+            raise SchemaError(f"dict {d2} missing ComponentId")
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "ChannelList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ChannelList")
+            raise SchemaError(f"dict {d2} missing ChannelList")
         if "ConfigList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ConfigList")
+            raise SchemaError(f"dict {d2} missing ConfigList")
         config_list = []
         if not isinstance(d2["ConfigList"], List):
-            raise MpSchemaError("ConfigList must be a List!")
+            raise SchemaError("ConfigList must be a List!")
         for elt in d2["ConfigList"]:
             if not isinstance(elt, dict):
-                raise MpSchemaError(
+                raise SchemaError(
                     f"elt {elt} of ConfigList must be "
                     "TelemetryReportingConfig but not even a dict!"
                 )
             config_list.append(TelemetryReportingConfig_Maker.dict_to_tuple(elt))
         d2["ConfigList"] = config_list
         if "HwUid" not in d2.keys():
             d2["HwUid"] = None
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return MultipurposeSensorComponentGt(
             ComponentId=d2["ComponentId"],
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             ChannelList=d2["ChannelList"],
             ConfigList=d2["ConfigList"],
             HwUid=d2["HwUid"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/pipe_flow_sensor_cac_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/pipe_flow_sensor_cac_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from fastapi_utils.enums import StrEnum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.cacs.pipe_flow_sensor_cac import PipeFlowSensorCac
 from gwproto.enums import MakeModel as EnumMakeModel
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatMakeModel000SchemaEnum:
     enum_name: str = "spaceheat.make.model.000"
     symbols: List[str] = [
         "00000000",
@@ -69,24 +69,22 @@
         return [elt.value for elt in cls]
 
 
 class MakeModelMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumMakeModel:
         if not SpaceheatMakeModel000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
-                f"{symbol} must belong to SpaceheatMakeModel000 symbols"
-            )
+            raise SchemaError(f"{symbol} must belong to SpaceheatMakeModel000 symbols")
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumMakeModel, EnumMakeModel.default())
 
     @classmethod
     def local_to_type(cls, make_model: EnumMakeModel) -> str:
         if not isinstance(make_model, EnumMakeModel):
-            raise MpSchemaError(f"{make_model} must be of type {EnumMakeModel}")
+            raise SchemaError(f"{make_model} must be of type {EnumMakeModel}")
         versioned_enum = as_enum(
             make_model, SpaceheatMakeModel000, SpaceheatMakeModel000.default()
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
     type_to_versioned_enum_dict: Dict[str, SpaceheatMakeModel000] = {
         "00000000": SpaceheatMakeModel000.UNKNOWNMAKE__UNKNOWNMODEL,
@@ -244,36 +242,36 @@
     def type_to_tuple(cls, t: str) -> PipeFlowSensorCacGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> PipeFlowSensorCacGt:
         d2 = dict(d)
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "MakeModelGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
         if d2["MakeModelGtEnumSymbol"] in SpaceheatMakeModel000SchemaEnum.symbols:
             d2["MakeModel"] = MakeModelMap.type_to_local(d2["MakeModelGtEnumSymbol"])
         else:
             d2["MakeModel"] = EnumMakeModel.default()
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "CommsMethod" not in d2.keys():
             d2["CommsMethod"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return PipeFlowSensorCacGt(
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             MakeModel=d2["MakeModel"],
             DisplayName=d2["DisplayName"],
             CommsMethod=d2["CommsMethod"],
             TypeName=d2["TypeName"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/pipe_flow_sensor_component_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/pipe_flow_sensor_component_gt.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.components.pipe_flow_sensor_component import (
     PipeFlowSensorComponent,
 )
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
@@ -151,36 +151,36 @@
     def type_to_tuple(cls, t: str) -> PipeFlowSensorComponentGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> PipeFlowSensorComponentGt:
         d2 = dict(d)
         if "ComponentId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentId")
+            raise SchemaError(f"dict {d2} missing ComponentId")
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "I2cAddress" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing I2cAddress")
+            raise SchemaError(f"dict {d2} missing I2cAddress")
         if "ConversionFactor" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ConversionFactor")
+            raise SchemaError(f"dict {d2} missing ConversionFactor")
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "HwUid" not in d2.keys():
             d2["HwUid"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return PipeFlowSensorComponentGt(
             ComponentId=d2["ComponentId"],
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             I2cAddress=d2["I2cAddress"],
             ConversionFactor=d2["ConversionFactor"],
             DisplayName=d2["DisplayName"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/power_watts.py` & `gridworks_protocol-0.5.0/src/gwproto/types/power_watts.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 class PowerWatts(BaseModel):
     """Real-time power of TerminalAsset in Watts..
 
         Used by a SCADA -> Atn or Atn -> AggregatedTNode to report real-time power of their TerminalAsset. Positive number means WITHDRAWAL from the grid - so generating electricity creates a negative number. This message is considered worse than useless to send after the first attempt, and does not require an ack.
 
@@ -57,25 +57,25 @@
     def type_to_tuple(cls, t: str) -> PowerWatts:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> PowerWatts:
         d2 = dict(d)
         if "Watts" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Watts")
+            raise SchemaError(f"dict {d2} missing Watts")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return PowerWatts(
             Watts=d2["Watts"],
             TypeName=d2["TypeName"],
             Version="000",
         )
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/relay_cac_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/relay_cac_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from fastapi_utils.enums import StrEnum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.cacs.relay_cac import RelayCac
 from gwproto.enums import MakeModel as EnumMakeModel
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatMakeModel000SchemaEnum:
     enum_name: str = "spaceheat.make.model.000"
     symbols: List[str] = [
         "00000000",
@@ -69,24 +69,22 @@
         return [elt.value for elt in cls]
 
 
 class MakeModelMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumMakeModel:
         if not SpaceheatMakeModel000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
-                f"{symbol} must belong to SpaceheatMakeModel000 symbols"
-            )
+            raise SchemaError(f"{symbol} must belong to SpaceheatMakeModel000 symbols")
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumMakeModel, EnumMakeModel.default())
 
     @classmethod
     def local_to_type(cls, make_model: EnumMakeModel) -> str:
         if not isinstance(make_model, EnumMakeModel):
-            raise MpSchemaError(f"{make_model} must be of type {EnumMakeModel}")
+            raise SchemaError(f"{make_model} must be of type {EnumMakeModel}")
         versioned_enum = as_enum(
             make_model, SpaceheatMakeModel000, SpaceheatMakeModel000.default()
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
     type_to_versioned_enum_dict: Dict[str, SpaceheatMakeModel000] = {
         "00000000": SpaceheatMakeModel000.UNKNOWNMAKE__UNKNOWNMODEL,
@@ -242,36 +240,36 @@
     def type_to_tuple(cls, t: str) -> RelayCacGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> RelayCacGt:
         d2 = dict(d)
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "MakeModelGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
         if d2["MakeModelGtEnumSymbol"] in SpaceheatMakeModel000SchemaEnum.symbols:
             d2["MakeModel"] = MakeModelMap.type_to_local(d2["MakeModelGtEnumSymbol"])
         else:
             d2["MakeModel"] = EnumMakeModel.default()
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "TypicalResponseTimeMs" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypicalResponseTimeMs")
+            raise SchemaError(f"dict {d2} missing TypicalResponseTimeMs")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return RelayCacGt(
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             MakeModel=d2["MakeModel"],
             DisplayName=d2["DisplayName"],
             TypicalResponseTimeMs=d2["TypicalResponseTimeMs"],
             TypeName=d2["TypeName"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/relay_component_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/relay_component_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Optional
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.components.relay_component import RelayComponent
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
@@ -151,36 +151,36 @@
     def type_to_tuple(cls, t: str) -> RelayComponentGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> RelayComponentGt:
         d2 = dict(d)
         if "ComponentId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentId")
+            raise SchemaError(f"dict {d2} missing ComponentId")
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "Gpio" not in d2.keys():
             d2["Gpio"] = None
         if "HwUid" not in d2.keys():
             d2["HwUid"] = None
         if "NormallyOpen" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing NormallyOpen")
+            raise SchemaError(f"dict {d2} missing NormallyOpen")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return RelayComponentGt(
             ComponentId=d2["ComponentId"],
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             DisplayName=d2["DisplayName"],
             Gpio=d2["Gpio"],
             HwUid=d2["HwUid"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/resistive_heater_cac_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/resistive_heater_cac_gt.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from fastapi_utils.enums import StrEnum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.cacs.resistive_heater_cac import ResistiveHeaterCac
 from gwproto.enums import MakeModel as EnumMakeModel
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatMakeModel000SchemaEnum:
     enum_name: str = "spaceheat.make.model.000"
     symbols: List[str] = [
         "00000000",
@@ -69,24 +69,22 @@
         return [elt.value for elt in cls]
 
 
 class MakeModelMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumMakeModel:
         if not SpaceheatMakeModel000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
-                f"{symbol} must belong to SpaceheatMakeModel000 symbols"
-            )
+            raise SchemaError(f"{symbol} must belong to SpaceheatMakeModel000 symbols")
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumMakeModel, EnumMakeModel.default())
 
     @classmethod
     def local_to_type(cls, make_model: EnumMakeModel) -> str:
         if not isinstance(make_model, EnumMakeModel):
-            raise MpSchemaError(f"{make_model} must be of type {EnumMakeModel}")
+            raise SchemaError(f"{make_model} must be of type {EnumMakeModel}")
         versioned_enum = as_enum(
             make_model, SpaceheatMakeModel000, SpaceheatMakeModel000.default()
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
     type_to_versioned_enum_dict: Dict[str, SpaceheatMakeModel000] = {
         "00000000": SpaceheatMakeModel000.UNKNOWNMAKE__UNKNOWNMODEL,
@@ -246,38 +244,38 @@
     def type_to_tuple(cls, t: str) -> ResistiveHeaterCacGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> ResistiveHeaterCacGt:
         d2 = dict(d)
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "MakeModelGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
         if d2["MakeModelGtEnumSymbol"] in SpaceheatMakeModel000SchemaEnum.symbols:
             d2["MakeModel"] = MakeModelMap.type_to_local(d2["MakeModelGtEnumSymbol"])
         else:
             d2["MakeModel"] = EnumMakeModel.default()
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "NameplateMaxPowerW" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing NameplateMaxPowerW")
+            raise SchemaError(f"dict {d2} missing NameplateMaxPowerW")
         if "RatedVoltageV" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing RatedVoltageV")
+            raise SchemaError(f"dict {d2} missing RatedVoltageV")
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return ResistiveHeaterCacGt(
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             MakeModel=d2["MakeModel"],
             DisplayName=d2["DisplayName"],
             NameplateMaxPowerW=d2["NameplateMaxPowerW"],
             RatedVoltageV=d2["RatedVoltageV"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/resistive_heater_component_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/resistive_heater_component_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.components.resistive_heater_component import (
     ResistiveHeaterComponent,
 )
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
@@ -157,36 +157,36 @@
     def type_to_tuple(cls, t: str) -> ResistiveHeaterComponentGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> ResistiveHeaterComponentGt:
         d2 = dict(d)
         if "ComponentId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentId")
+            raise SchemaError(f"dict {d2} missing ComponentId")
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "HwUid" not in d2.keys():
             d2["HwUid"] = None
         if "TestedMaxHotMilliOhms" not in d2.keys():
             d2["TestedMaxHotMilliOhms"] = None
         if "TestedMaxColdMilliOhms" not in d2.keys():
             d2["TestedMaxColdMilliOhms"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return ResistiveHeaterComponentGt(
             ComponentId=d2["ComponentId"],
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             DisplayName=d2["DisplayName"],
             HwUid=d2["HwUid"],
             TestedMaxHotMilliOhms=d2["TestedMaxHotMilliOhms"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/simple_temp_sensor_cac_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/simple_temp_sensor_cac_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.cacs.simple_temp_sensor_cac import SimpleTempSensorCac
 from gwproto.enums import MakeModel as EnumMakeModel
 from gwproto.enums import TelemetryName as EnumTelemetryName
 from gwproto.enums import Unit
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatTelemetryName000SchemaEnum:
     enum_name: str = "spaceheat.telemetry.name.000"
     symbols: List[str] = [
         "00000000",
@@ -69,24 +69,24 @@
         return [elt.value for elt in cls]
 
 
 class TelemetryNameMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumTelemetryName:
         if not SpaceheatTelemetryName000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"{symbol} must belong to SpaceheatTelemetryName000 symbols"
             )
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumTelemetryName, EnumTelemetryName.default())
 
     @classmethod
     def local_to_type(cls, telemetry_name: EnumTelemetryName) -> str:
         if not isinstance(telemetry_name, EnumTelemetryName):
-            raise MpSchemaError(f"{telemetry_name} must be of type {EnumTelemetryName}")
+            raise SchemaError(f"{telemetry_name} must be of type {EnumTelemetryName}")
         versioned_enum = as_enum(
             telemetry_name,
             SpaceheatTelemetryName000,
             SpaceheatTelemetryName000.default(),
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
@@ -174,24 +174,22 @@
         return [elt.value for elt in cls]
 
 
 class MakeModelMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumMakeModel:
         if not SpaceheatMakeModel000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
-                f"{symbol} must belong to SpaceheatMakeModel000 symbols"
-            )
+            raise SchemaError(f"{symbol} must belong to SpaceheatMakeModel000 symbols")
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumMakeModel, EnumMakeModel.default())
 
     @classmethod
     def local_to_type(cls, make_model: EnumMakeModel) -> str:
         if not isinstance(make_model, EnumMakeModel):
-            raise MpSchemaError(f"{make_model} must be of type {EnumMakeModel}")
+            raise SchemaError(f"{make_model} must be of type {EnumMakeModel}")
         versioned_enum = as_enum(
             make_model, SpaceheatMakeModel000, SpaceheatMakeModel000.default()
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
     type_to_versioned_enum_dict: Dict[str, SpaceheatMakeModel000] = {
         "00000000": SpaceheatMakeModel000.UNKNOWNMAKE__UNKNOWNMODEL,
@@ -271,22 +269,22 @@
         return [elt.value for elt in cls]
 
 
 class UnitMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> Unit:
         if not SpaceheatUnit000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(f"{symbol} must belong to SpaceheatUnit000 symbols")
+            raise SchemaError(f"{symbol} must belong to SpaceheatUnit000 symbols")
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, Unit, Unit.default())
 
     @classmethod
     def local_to_type(cls, unit: Unit) -> str:
         if not isinstance(unit, Unit):
-            raise MpSchemaError(f"{unit} must be of type {Unit}")
+            raise SchemaError(f"{unit} must be of type {Unit}")
         versioned_enum = as_enum(unit, SpaceheatUnit000, SpaceheatUnit000.default())
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
     type_to_versioned_enum_dict: Dict[str, SpaceheatUnit000] = {
         "00000000": SpaceheatUnit000.Unknown,
         "ec972387": SpaceheatUnit000.Unitless,
         "f459a9c3": SpaceheatUnit000.W,
@@ -472,57 +470,57 @@
     def type_to_tuple(cls, t: str) -> SimpleTempSensorCacGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> SimpleTempSensorCacGt:
         d2 = dict(d)
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "MakeModelGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing MakeModelGtEnumSymbol")
         if d2["MakeModelGtEnumSymbol"] in SpaceheatMakeModel000SchemaEnum.symbols:
             d2["MakeModel"] = MakeModelMap.type_to_local(d2["MakeModelGtEnumSymbol"])
         else:
             d2["MakeModel"] = EnumMakeModel.default()
         if "TypicalResponseTimeMs" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypicalResponseTimeMs")
+            raise SchemaError(f"dict {d2} missing TypicalResponseTimeMs")
         if "Exponent" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Exponent")
+            raise SchemaError(f"dict {d2} missing Exponent")
         if "TempUnitGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TempUnitGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing TempUnitGtEnumSymbol")
         if d2["TempUnitGtEnumSymbol"] in SpaceheatUnit000SchemaEnum.symbols:
             d2["TempUnit"] = UnitMap.type_to_local(d2["TempUnitGtEnumSymbol"])
         else:
             d2["TempUnit"] = Unit.default()
         if "TelemetryNameGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TelemetryNameGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing TelemetryNameGtEnumSymbol")
         if (
             d2["TelemetryNameGtEnumSymbol"]
             in SpaceheatTelemetryName000SchemaEnum.symbols
         ):
             d2["TelemetryName"] = TelemetryNameMap.type_to_local(
                 d2["TelemetryNameGtEnumSymbol"]
             )
         else:
             d2["TelemetryName"] = EnumTelemetryName.default()
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "CommsMethod" not in d2.keys():
             d2["CommsMethod"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return SimpleTempSensorCacGt(
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             MakeModel=d2["MakeModel"],
             TypicalResponseTimeMs=d2["TypicalResponseTimeMs"],
             Exponent=d2["Exponent"],
             TempUnit=d2["TempUnit"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/simple_temp_sensor_component_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/simple_temp_sensor_component_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.components.simple_temp_sensor_component import (
     SimpleTempSensorComponent,
 )
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
@@ -151,34 +151,34 @@
     def type_to_tuple(cls, t: str) -> SimpleTempSensorComponentGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> SimpleTempSensorComponentGt:
         d2 = dict(d)
         if "ComponentId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentId")
+            raise SchemaError(f"dict {d2} missing ComponentId")
         if "ComponentAttributeClassId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ComponentAttributeClassId")
+            raise SchemaError(f"dict {d2} missing ComponentAttributeClassId")
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "HwUid" not in d2.keys():
             d2["HwUid"] = None
         if "Channel" not in d2.keys():
             d2["Channel"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return SimpleTempSensorComponentGt(
             ComponentId=d2["ComponentId"],
             ComponentAttributeClassId=d2["ComponentAttributeClassId"],
             DisplayName=d2["DisplayName"],
             HwUid=d2["HwUid"],
             Channel=d2["Channel"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/snapshot_spaceheat.py` & `gridworks_protocol-0.5.0/src/gwproto/types/snapshot_spaceheat.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Dict
 from typing import Literal
 
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.types.telemetry_snapshot_spaceheat import TelemetrySnapshotSpaceheat
 from gwproto.types.telemetry_snapshot_spaceheat import TelemetrySnapshotSpaceheat_Maker
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """Checks UuidCanonicalTextual format
 
@@ -152,36 +152,36 @@
     def type_to_tuple(cls, t: str) -> SnapshotSpaceheat:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> SnapshotSpaceheat:
         d2 = dict(d)
         if "FromGNodeAlias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing FromGNodeAlias")
+            raise SchemaError(f"dict {d2} missing FromGNodeAlias")
         if "FromGNodeInstanceId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing FromGNodeInstanceId")
+            raise SchemaError(f"dict {d2} missing FromGNodeInstanceId")
         if "Snapshot" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Snapshot")
+            raise SchemaError(f"dict {d2} missing Snapshot")
         if not isinstance(d2["Snapshot"], dict):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"d['Snapshot'] {d2['Snapshot']} must be a TelemetrySnapshotSpaceheat!"
             )
         snapshot = TelemetrySnapshotSpaceheat_Maker.dict_to_tuple(d2["Snapshot"])
         d2["Snapshot"] = snapshot
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return SnapshotSpaceheat(
             FromGNodeAlias=d2["FromGNodeAlias"],
             FromGNodeInstanceId=d2["FromGNodeInstanceId"],
             Snapshot=d2["Snapshot"],
             TypeName=d2["TypeName"],
             Version="000",
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/spaceheat_node_gt.py` & `gridworks_protocol-0.5.0/src/gwproto/types/spaceheat_node_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 from gwproto.data_classes.sh_node import ShNode
 from gwproto.enums import ActorClass as EnumActorClass
 from gwproto.enums import Role as EnumRole
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class ShActorClass000SchemaEnum:
     enum_name: str = "sh.actor.class.000"
     symbols: List[str] = [
         "00000000",
@@ -60,22 +60,22 @@
         return [elt.value for elt in cls]
 
 
 class ActorClassMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumActorClass:
         if not ShActorClass000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(f"{symbol} must belong to ShActorClass000 symbols")
+            raise SchemaError(f"{symbol} must belong to ShActorClass000 symbols")
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumActorClass, EnumActorClass.default())
 
     @classmethod
     def local_to_type(cls, actor_class: EnumActorClass) -> str:
         if not isinstance(actor_class, EnumActorClass):
-            raise MpSchemaError(f"{actor_class} must be of type {EnumActorClass}")
+            raise SchemaError(f"{actor_class} must be of type {EnumActorClass}")
         versioned_enum = as_enum(
             actor_class, ShActorClass000, ShActorClass000.default()
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
     type_to_versioned_enum_dict: Dict[str, ShActorClass000] = {
         "00000000": ShActorClass000.NoActor,
@@ -165,22 +165,22 @@
         return [elt.value for elt in cls]
 
 
 class RoleMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumRole:
         if not ShNodeRole000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(f"{symbol} must belong to ShNodeRole000 symbols")
+            raise SchemaError(f"{symbol} must belong to ShNodeRole000 symbols")
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumRole, EnumRole.default())
 
     @classmethod
     def local_to_type(cls, role: EnumRole) -> str:
         if not isinstance(role, EnumRole):
-            raise MpSchemaError(f"{role} must be of type {EnumRole}")
+            raise SchemaError(f"{role} must be of type {EnumRole}")
         versioned_enum = as_enum(role, ShNodeRole000, ShNodeRole000.default())
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
     type_to_versioned_enum_dict: Dict[str, ShNodeRole000] = {
         "00000000": ShNodeRole000.Unknown,
         "d0afb424": ShNodeRole000.Scada,
         "863e50d1": ShNodeRole000.HomeAlone,
@@ -445,34 +445,34 @@
     def type_to_tuple(cls, t: str) -> SpaceheatNodeGt:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> SpaceheatNodeGt:
         d2 = dict(d)
         if "ShNodeId" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ShNodeId")
+            raise SchemaError(f"dict {d2} missing ShNodeId")
         if "Alias" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Alias")
+            raise SchemaError(f"dict {d2} missing Alias")
         if "ActorClassGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ActorClassGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing ActorClassGtEnumSymbol")
         if d2["ActorClassGtEnumSymbol"] in ShActorClass000SchemaEnum.symbols:
             d2["ActorClass"] = ActorClassMap.type_to_local(d2["ActorClassGtEnumSymbol"])
         else:
             d2["ActorClass"] = EnumActorClass.default()
         if "RoleGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing RoleGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing RoleGtEnumSymbol")
         if d2["RoleGtEnumSymbol"] in ShNodeRole000SchemaEnum.symbols:
             d2["Role"] = RoleMap.type_to_local(d2["RoleGtEnumSymbol"])
         else:
             d2["Role"] = EnumRole.default()
         if "DisplayName" not in d2.keys():
             d2["DisplayName"] = None
         if "ComponentId" not in d2.keys():
@@ -482,15 +482,15 @@
         if "RatedVoltageV" not in d2.keys():
             d2["RatedVoltageV"] = None
         if "TypicalVoltageV" not in d2.keys():
             d2["TypicalVoltageV"] = None
         if "InPowerMetering" not in d2.keys():
             d2["InPowerMetering"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return SpaceheatNodeGt(
             ShNodeId=d2["ShNodeId"],
             Alias=d2["Alias"],
             ActorClass=d2["ActorClass"],
             Role=d2["Role"],
             DisplayName=d2["DisplayName"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/telemetry_reporting_config.py` & `gridworks_protocol-0.5.0/src/gwproto/types/telemetry_reporting_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import root_validator
 from pydantic import validator
 
 from gwproto.enums import TelemetryName as EnumTelemetryName
 from gwproto.enums import Unit as EnumUnit
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatTelemetryName000SchemaEnum:
     enum_name: str = "spaceheat.telemetry.name.000"
     symbols: List[str] = [
         "00000000",
@@ -68,24 +68,24 @@
         return [elt.value for elt in cls]
 
 
 class TelemetryNameMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumTelemetryName:
         if not SpaceheatTelemetryName000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"{symbol} must belong to SpaceheatTelemetryName000 symbols"
             )
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumTelemetryName, EnumTelemetryName.default())
 
     @classmethod
     def local_to_type(cls, telemetry_name: EnumTelemetryName) -> str:
         if not isinstance(telemetry_name, EnumTelemetryName):
-            raise MpSchemaError(f"{telemetry_name} must be of type {EnumTelemetryName}")
+            raise SchemaError(f"{telemetry_name} must be of type {EnumTelemetryName}")
         versioned_enum = as_enum(
             telemetry_name,
             SpaceheatTelemetryName000,
             SpaceheatTelemetryName000.default(),
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
@@ -165,22 +165,22 @@
         return [elt.value for elt in cls]
 
 
 class UnitMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> EnumUnit:
         if not SpaceheatUnit000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(f"{symbol} must belong to SpaceheatUnit000 symbols")
+            raise SchemaError(f"{symbol} must belong to SpaceheatUnit000 symbols")
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, EnumUnit, EnumUnit.default())
 
     @classmethod
     def local_to_type(cls, unit: EnumUnit) -> str:
         if not isinstance(unit, EnumUnit):
-            raise MpSchemaError(f"{unit} must be of type {EnumUnit}")
+            raise SchemaError(f"{unit} must be of type {EnumUnit}")
         versioned_enum = as_enum(unit, SpaceheatUnit000, SpaceheatUnit000.default())
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
     type_to_versioned_enum_dict: Dict[str, SpaceheatUnit000] = {
         "00000000": SpaceheatUnit000.Unknown,
         "ec972387": SpaceheatUnit000.Unitless,
         "f459a9c3": SpaceheatUnit000.W,
@@ -356,53 +356,53 @@
     def type_to_tuple(cls, t: str) -> TelemetryReportingConfig:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> TelemetryReportingConfig:
         d2 = dict(d)
         if "TelemetryNameGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TelemetryNameGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing TelemetryNameGtEnumSymbol")
         if (
             d2["TelemetryNameGtEnumSymbol"]
             in SpaceheatTelemetryName000SchemaEnum.symbols
         ):
             d2["TelemetryName"] = TelemetryNameMap.type_to_local(
                 d2["TelemetryNameGtEnumSymbol"]
             )
         else:
             d2["TelemetryName"] = EnumTelemetryName.default()
         if "AboutNodeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing AboutNodeName")
+            raise SchemaError(f"dict {d2} missing AboutNodeName")
         if "ReportOnChange" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ReportOnChange")
+            raise SchemaError(f"dict {d2} missing ReportOnChange")
         if "SamplePeriodS" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing SamplePeriodS")
+            raise SchemaError(f"dict {d2} missing SamplePeriodS")
         if "Exponent" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing Exponent")
+            raise SchemaError(f"dict {d2} missing Exponent")
         if "UnitGtEnumSymbol" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing UnitGtEnumSymbol")
+            raise SchemaError(f"dict {d2} missing UnitGtEnumSymbol")
         if d2["UnitGtEnumSymbol"] in SpaceheatUnit000SchemaEnum.symbols:
             d2["Unit"] = UnitMap.type_to_local(d2["UnitGtEnumSymbol"])
         else:
             d2["Unit"] = EnumUnit.default()
         if "AsyncReportThreshold" not in d2.keys():
             d2["AsyncReportThreshold"] = None
         if "NameplateMaxValue" not in d2.keys():
             d2["NameplateMaxValue"] = None
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return TelemetryReportingConfig(
             TelemetryName=d2["TelemetryName"],
             AboutNodeName=d2["AboutNodeName"],
             ReportOnChange=d2["ReportOnChange"],
             SamplePeriodS=d2["SamplePeriodS"],
             Exponent=d2["Exponent"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/types/telemetry_snapshot_spaceheat.py` & `gridworks_protocol-0.5.0/src/gwproto/types/telemetry_snapshot_spaceheat.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from fastapi_utils.enums import StrEnum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import root_validator
 from pydantic import validator
 
 from gwproto.enums import TelemetryName
-from gwproto.errors import MpSchemaError
+from gwproto.errors import SchemaError
 from gwproto.message import as_enum
 
 
 class SpaceheatTelemetryName000SchemaEnum:
     enum_name: str = "spaceheat.telemetry.name.000"
     symbols: List[str] = [
         "00000000",
@@ -66,24 +66,24 @@
         return [elt.value for elt in cls]
 
 
 class TelemetryNameMap:
     @classmethod
     def type_to_local(cls, symbol: str) -> TelemetryName:
         if not SpaceheatTelemetryName000SchemaEnum.is_symbol(symbol):
-            raise MpSchemaError(
+            raise SchemaError(
                 f"{symbol} must belong to SpaceheatTelemetryName000 symbols"
             )
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
         return as_enum(versioned_enum, TelemetryName, TelemetryName.default())
 
     @classmethod
     def local_to_type(cls, telemetry_name: TelemetryName) -> str:
         if not isinstance(telemetry_name, TelemetryName):
-            raise MpSchemaError(f"{telemetry_name} must be of type {TelemetryName}")
+            raise SchemaError(f"{telemetry_name} must be of type {TelemetryName}")
         versioned_enum = as_enum(
             telemetry_name,
             SpaceheatTelemetryName000,
             SpaceheatTelemetryName000.default(),
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
@@ -288,43 +288,43 @@
     def type_to_tuple(cls, t: str) -> TelemetrySnapshotSpaceheat:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
-            raise MpSchemaError("Type must be string or bytes!")
+            raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
-            raise MpSchemaError(f"Deserializing {t} must result in dict!")
+            raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
     def dict_to_tuple(cls, d: dict[str, Any]) -> TelemetrySnapshotSpaceheat:
         d2 = dict(d)
         if "ReportTimeUnixMs" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ReportTimeUnixMs")
+            raise SchemaError(f"dict {d2} missing ReportTimeUnixMs")
         if "AboutNodeAliasList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing AboutNodeAliasList")
+            raise SchemaError(f"dict {d2} missing AboutNodeAliasList")
         if "ValueList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing ValueList")
+            raise SchemaError(f"dict {d2} missing ValueList")
         if "TelemetryNameList" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TelemetryNameList")
+            raise SchemaError(f"dict {d2} missing TelemetryNameList")
         telemetry_name_list = []
         if not isinstance(d2["TelemetryNameList"], List):
-            raise MpSchemaError("TelemetryNameList must be a List!")
+            raise SchemaError("TelemetryNameList must be a List!")
         for elt in d2["TelemetryNameList"]:
             if elt in SpaceheatTelemetryName000SchemaEnum.symbols:
                 v = TelemetryNameMap.type_to_local(elt)
             else:
                 v = SpaceheatTelemetryName000.Unknown  #
 
             telemetry_name_list.append(v)
         d2["TelemetryNameList"] = telemetry_name_list
         if "TypeName" not in d2.keys():
-            raise MpSchemaError(f"dict {d2} missing TypeName")
+            raise SchemaError(f"dict {d2} missing TypeName")
 
         return TelemetrySnapshotSpaceheat(
             ReportTimeUnixMs=d2["ReportTimeUnixMs"],
             AboutNodeAliasList=d2["AboutNodeAliasList"],
             ValueList=d2["ValueList"],
             TelemetryNameList=d2["TelemetryNameList"],
             TypeName=d2["TypeName"],
```

### Comparing `gridworks_protocol-0.4.5/src/gwproto/utils.py` & `gridworks_protocol-0.5.0/src/gwproto/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks_protocol-0.4.5/setup.py` & `gridworks_protocol-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,21 @@
  'gwproto.types']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['fastapi-utils>=0.2.1,<0.3.0',
+ 'gridworks==0.2.2',
  'pendulum>=2.1.2,<3.0.0',
  'pydantic>=1.10.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'gridworks-protocol',
-    'version': '0.4.5',
+    'version': '0.5.0',
     'description': 'Gridworks Protocol',
     'long_description': "# Gridworks Protocol\n\n[![PyPI](https://img.shields.io/pypi/v/gridworks-protocol.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/gridworks-protocol.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/gridworks-protocol)][python version]\n[![License](https://img.shields.io/pypi/l/gridworks-protocol)][license]\n\n[![Read the documentation at https://gridworks-protocol.readthedocs.io/](https://img.shields.io/readthedocs/gridworks-protocol/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/thegridelectric/gridworks-protocol/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/thegridelectric/gridworks-protocol/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/gridworks-protocol/\n[status]: https://pypi.org/project/gridworks-protocol/\n[python version]: https://pypi.org/project/gridworks-protocol\n[read the docs]: https://gridworks-protocol.readthedocs.io/\n[tests]: https://github.com/thegridelectric/gridworks-protocol/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/thegridelectric/gridworks-protocol\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Features\n\n- TODO\n\n## Requirements\n\n- TODO\n\n## Installation\n\nYou can install _Gridworks Protocol_ via [pip] from [PyPI]:\n\n```console\n$ pip install gridworks-protocol\n```\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## License\n\nDistributed under the terms of the [MIT license][license],\n_Gridworks Protocol_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/thegridelectric/gridworks-protocol/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/thegridelectric/gridworks-protocol/blob/main/LICENSE\n[contributor guide]: https://github.com/thegridelectric/gridworks-protocol/blob/main/CONTRIBUTING.md\n",
     'author': 'Jessica Millar',
     'author_email': 'jmillar@gridworks-consulting.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/thegridelectric/gridworks-protocol',
```

### Comparing `gridworks_protocol-0.4.5/PKG-INFO` & `gridworks_protocol-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: gridworks-protocol
-Version: 0.4.5
+Version: 0.5.0
 Summary: Gridworks Protocol
 Home-page: https://github.com/thegridelectric/gridworks-protocol
 License: MIT
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi-utils (>=0.2.1,<0.3.0)
+Requires-Dist: gridworks (==0.2.2)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Project-URL: Changelog, https://github.com/thegridelectric/gridworks-protocol/releases
 Project-URL: Documentation, https://gridworks-protocol.readthedocs.io
 Project-URL: Repository, https://github.com/thegridelectric/gridworks-protocol
 Description-Content-Type: text/markdown
```

