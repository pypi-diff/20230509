# Comparing `tmp/equinix-metal-0.1.0.tar.gz` & `tmp/equinix-metal-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "equinix-metal-0.1.0.tar", last modified: Wed Mar 29 12:09:10 2023, max compression
+gzip compressed data, was "equinix-metal-0.2.0.tar", last modified: Tue May  9 07:27:38 2023, max compression
```

## Comparing `equinix-metal-0.1.0.tar` & `equinix-metal-0.2.0.tar`

### file list

```diff
@@ -1,171 +1,555 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:09:10.049487 equinix-metal-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-29 12:09:10.049487 equinix-metal-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:09:10.021487 equinix-metal-0.1.0/equinix_metal/
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:09:10.021487 equinix-metal-0.1.0/equinix_metal/api/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    70230 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/api/devices_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53941 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/api/ip_addresses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    56392 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/api/organizations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    44719 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/api/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/api/vrfs_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29465 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15170 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5098 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:09:10.037487 equinix-metal-0.1.0/equinix_metal/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/address.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/bond_port_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/create_device_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/device_actions_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/device_create_in_facility_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/device_create_in_metro_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/device_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/device_create_input_ip_addresses_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/device_created_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/device_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/device_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/device_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/device_project_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/device_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/facility_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/facility_input_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/find_ip_address_by_id200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/href.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ip_assignment_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ip_assignment_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ip_assignment_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ip_assignment_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ip_availabilities_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ip_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ip_reservation_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ip_reservation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ip_reservation_list_ip_addresses_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ip_reservation_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ip_reservation_request_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/metal_gateway_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/metro_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/operating_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3503 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/organization_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/organization_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/parent_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/plan_available_in_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/plan_available_in_inner_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/plan_available_in_metros_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/plan_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/plan_specs_cpus_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/plan_specs_drives_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/plan_specs_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/plan_specs_nics_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/port.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/port_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/project_create_from_root_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/project_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/project_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/project_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/request_ip_reservation201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/request_ip_reservation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/ssh_key_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/user_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/virtual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/vrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/vrf_ip_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/models/vrf_ip_reservation_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/equinix_metal/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:09:10.021487 equinix-metal-0.1.0/equinix_metal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-29 12:09:10.000000 equinix-metal-0.1.0/equinix_metal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-03-29 12:09:10.000000 equinix-metal-0.1.0/equinix_metal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 12:09:10.000000 equinix-metal-0.1.0/equinix_metal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-29 12:09:10.000000 equinix-metal-0.1.0/equinix_metal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-29 12:09:10.000000 equinix-metal-0.1.0/equinix_metal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-29 12:09:10.049487 equinix-metal-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:09:10.049487 equinix-metal-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_bond_port_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_create_device_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_device_actions_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_device_create_in_facility_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_device_create_in_metro_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_device_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_device_create_input_ip_addresses_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_device_created_by.py
--rw-r--r--   0 runner    (1001) docker     (123)    13419 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_device_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_device_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_device_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_device_project_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_device_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_devices_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_facility_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_facility_input_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_find_ip_address_by_id200_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_href.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_addresses_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_assignment_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_assignment_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_assignment_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_assignment_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_availabilities_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_reservation_facility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_reservation_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    14093 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_reservation_list_ip_addresses_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_reservation_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ip_reservation_request_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_metal_gateway_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_metro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_metro_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_operating_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_organization_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_organization_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_organizations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_parent_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_plan_available_in_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_plan_available_in_inner_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_plan_available_in_metros_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_plan_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_plan_specs_cpus_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_plan_specs_drives_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_plan_specs_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_plan_specs_nics_inner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_port_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_project_create_from_root_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_project_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_project_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_project_update_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_projects_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_request_ip_reservation201_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_request_ip_reservation_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_ssh_key_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_user_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_virtual_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_vrf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_vrf_ip_reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_vrf_ip_reservation_create_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-03-29 12:08:58.000000 equinix-metal-0.1.0/test/test_vrfs_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:27:38.071214 equinix-metal-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-09 07:27:38.071214 equinix-metal-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    51411 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:27:37.995213 equinix-metal-0.2.0/equinix_metal/
+-rw-r--r--   0 runner    (1001) docker     (123)    24048 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:27:38.003213 equinix-metal-0.2.0/equinix_metal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46223 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35443 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/batches_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53275 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/bgp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42522 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/capacity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139461 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/devices_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32320 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/emails_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79719 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30060 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/facilities_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40324 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/hardware_reservations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/incidents_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110259 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/interconnections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25332 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/invitations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58088 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/ip_addresses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42404 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/licenses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26100 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42371 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/metal_gateways_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16543 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/metros_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/operating_systems_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126100 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/organizations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27611 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/otps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16686 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/password_reset_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26446 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/payment_methods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21858 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109267 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/ports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88544 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26659 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/self_service_reservations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57754 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/spot_market_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65523 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/ssh_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/support_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25177 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/transfer_requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26624 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/two_factor_auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19788 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/usages_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/user_verification_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/userdata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58053 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34054 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/vlans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99745 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api/vrfs_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33612 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19317 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:27:38.035214 equinix-metal-0.2.0/equinix_metal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/activate_hardware_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/auth_token_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/auth_token_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/auth_token_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/auth_token_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6500 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/batches_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10095 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/bgp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/bgp_config_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/bgp_dynamic_neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/bgp_dynamic_neighbor_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/bgp_dynamic_neighbor_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/bgp_neighbor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/bgp_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7930 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/bgp_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/bgp_session_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6590 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/bgp_session_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/bgp_session_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/bond_port_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/capacity_check_per_facility_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/capacity_check_per_facility_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6798 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/capacity_check_per_metro_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/capacity_check_per_metro_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/capacity_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/capacity_level_per_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/capacity_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/capacity_per_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/capacity_per_metro_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/capacity_per_new_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/capacity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/create_device_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/create_email_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/create_metal_gateway_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/create_self_service_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/create_self_service_reservation_request_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17473 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_action_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_actions_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_create_in_facility_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_create_in_metro_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6826 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5964 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_project_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7424 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/device_usage_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/email_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/entitlement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/event_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/fabric_service_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/facility_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/facility_input_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/facility_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/find_ip_address_by_id200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/find_metal_gateway_by_id200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/find_traffic_timeframe_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/global_bgp_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/global_bgp_range_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/hardware_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7109 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/hardware_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/href.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/instances_batch_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17728 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/instances_batch_create_input_batches_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/instances_batch_create_input_batches_inner_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/interconnection_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/interconnection_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/interconnection_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/interconnection_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6635 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/interconnection_port_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/interconnection_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/invitation_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/invitation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_assignment_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_assignment_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_assignment_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_assignment_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_availabilities_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11271 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_reservation_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_reservation_list_ip_addresses_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_reservation_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ip_reservation_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/license_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/license_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/license_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/membership_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/membership_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7782 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metadata_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metadata_network_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metadata_network_network_bonding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metal_gateway_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metal_gateway_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metal_gateway_list_metal_gateways_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metal_gateway_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metro_capacity_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metro_capacity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metro_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metro_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/metro_server_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/move_hardware_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/new_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/operating_system_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9679 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7650 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/organization_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/organization_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/parent_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/payment_method_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/payment_method_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/payment_method_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/payment_method_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/plan_available_in_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/plan_available_in_inner_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/plan_available_in_metros_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/plan_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/plan_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/plan_specs_cpus_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/plan_specs_drives_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/plan_specs_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/plan_specs_nics_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/port_assign_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/port_convert_layer3_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/port_convert_layer3_input_request_ips_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/port_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/port_vlan_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/port_vlan_assignment_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/port_vlan_assignment_batch_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/port_vlan_assignment_batch_create_input_vlan_assignments_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/port_vlan_assignment_batch_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/port_vlan_assignment_batch_vlan_assignments_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/port_vlan_assignment_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/project_create_from_root_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/project_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6847 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/project_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/project_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/project_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/project_usage_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/recovery_code_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/request_ip_reservation201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/request_ip_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/self_service_reservation_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/self_service_reservation_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/self_service_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/self_service_reservation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/server_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_market_prices_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_market_prices_per_metro_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_market_prices_per_metro_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_market_request_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8501 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_market_request_create_input_instance_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_market_request_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_market_request_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_prices_datapoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_prices_history_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_prices_per_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_prices_per_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_prices_per_new_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/spot_prices_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ssh_key_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6118 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ssh_key_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/ssh_key_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/support_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/transfer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/transfer_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/transfer_request_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/update_email_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/user_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/user_limited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/user_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/user_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/user_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/userdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/verify_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/virtual_circuit_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/virtual_circuit_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/virtual_circuit_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/virtual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/virtual_network_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/virtual_network_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10895 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vlan_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vlan_virtual_circuit_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vlan_virtual_circuit_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7747 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10084 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_ip_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7116 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_ip_reservation_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_ip_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_metal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_metal_gateway_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_route_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_route_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_route_metal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_route_virtual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_route_vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_virtual_circuit_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/models/vrf_virtual_circuit_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16804 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/equinix_metal/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:27:37.995213 equinix-metal-0.2.0/equinix_metal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-09 07:27:37.000000 equinix-metal-0.2.0/equinix_metal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21108 2023-05-09 07:27:37.000000 equinix-metal-0.2.0/equinix_metal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 07:27:37.000000 equinix-metal-0.2.0/equinix_metal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 07:27:37.000000 equinix-metal-0.2.0/equinix_metal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 07:27:37.000000 equinix-metal-0.2.0/equinix_metal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-09 07:27:38.071214 equinix-metal-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9964 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 07:27:38.071214 equinix-metal-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_activate_hardware_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_auth_token_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_auth_token_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_auth_token_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6646 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_auth_token_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_batches_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_batches_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bgp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7298 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bgp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bgp_config_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15115 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bgp_dynamic_neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bgp_dynamic_neighbor_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bgp_dynamic_neighbor_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bgp_neighbor_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bgp_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bgp_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bgp_session_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6429 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bgp_session_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bgp_session_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_bond_port_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_capacity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_capacity_check_per_facility_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_capacity_check_per_facility_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_capacity_check_per_metro_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_capacity_check_per_metro_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_capacity_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_capacity_level_per_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7292 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_capacity_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_capacity_per_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_capacity_per_metro_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_capacity_per_new_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11851 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_capacity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_create_device_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_create_email_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_create_metal_gateway_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_create_self_service_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6029 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_create_self_service_reservation_request_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_action_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_actions_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_create_in_facility_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_create_in_metro_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_created_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17601 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_project_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_device_usage_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_devices_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_email_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_emails_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_entitlement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6809 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_event_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_events_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_fabric_service_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_facilities_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_facility_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_facility_input_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_facility_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20932 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_find_ip_address_by_id200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19764 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_find_metal_gateway_by_id200_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_find_traffic_timeframe_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_global_bgp_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_global_bgp_range_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21776 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_hardware_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21424 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_hardware_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_hardware_reservations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_href.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_incidents_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_instances_batch_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_instances_batch_create_input_batches_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_instances_batch_create_input_batches_inner_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_interconnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_interconnection_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_interconnection_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_interconnection_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_interconnection_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6456 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_interconnection_port_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_interconnection_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_interconnections_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_invitation_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_invitation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_invitations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_addresses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_assignment_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_assignment_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_assignment_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_assignment_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_availabilities_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8834 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_reservation_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20584 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_reservation_list_ip_addresses_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_reservation_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ip_reservation_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_license_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_license_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_license_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_licenses_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_membership_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_membership_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_memberships_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metadata_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metadata_network_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metadata_network_network_bonding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12128 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metal_gateway_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6234 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metal_gateway_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19800 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metal_gateway_list_metal_gateways_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metal_gateway_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metal_gateways_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metro_capacity_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20895 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metro_capacity_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metro_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metro_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metro_server_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_metros_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_move_hardware_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_new_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_operating_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_operating_system_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_operating_systems_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7679 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_organization_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_organization_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7705 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_organizations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_otps_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_parent_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_password_reset_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_payment_method_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_payment_method_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_payment_method_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_payment_method_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_payment_methods_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7999 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_plan_available_in_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_plan_available_in_inner_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_plan_available_in_metros_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_plan_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_plan_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_plan_specs_cpus_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_plan_specs_drives_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_plan_specs_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_plan_specs_nics_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_plans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_port_assign_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_port_convert_layer3_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_port_convert_layer3_input_request_ips_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_port_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6213 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_port_vlan_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_port_vlan_assignment_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_port_vlan_assignment_batch_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_port_vlan_assignment_batch_create_input_vlan_assignments_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9410 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_port_vlan_assignment_batch_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_port_vlan_assignment_batch_vlan_assignments_inner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_port_vlan_assignment_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ports_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7259 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_project_create_from_root_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_project_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_project_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_project_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_project_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_project_usage_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_recovery_code_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20556 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_request_ip_reservation201_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_request_ip_reservation_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_self_service_reservation_item_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_self_service_reservation_item_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_self_service_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_self_service_reservation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_self_service_reservations_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_server_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_market_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_market_prices_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_market_prices_per_metro_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_market_prices_per_metro_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_market_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_market_request_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_market_request_create_input_instance_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_market_request_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_market_request_metro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_prices_datapoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_prices_history_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5765 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_prices_per_baremetal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_prices_per_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_prices_per_new_facility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11893 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_spot_prices_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ssh_key_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ssh_key_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ssh_key_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_ssh_keys_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_support_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_support_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_transfer_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_transfer_request_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_transfer_request_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_transfer_requests_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5531 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_two_factor_auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_update_email_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5178 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_usages_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_user_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_user_limited.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_user_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_user_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_user_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_user_verification_tokens_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_userdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_userdata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_users_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_verify_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_virtual_circuit_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5769 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_virtual_circuit_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_virtual_circuit_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_virtual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_virtual_network_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_virtual_network_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vlan_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vlan_virtual_circuit_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vlan_virtual_circuit_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vlans_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12777 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19965 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_ip_reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_ip_reservation_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12104 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_ip_reservation_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19566 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_metal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_metal_gateway_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5863 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_route_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6916 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_route_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_route_metal_gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_route_virtual_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12904 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_route_vrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_virtual_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_virtual_circuit_create_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrf_virtual_circuit_update_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-05-09 07:27:29.000000 equinix-metal-0.2.0/test/test_vrfs_api.py
```

### Comparing `equinix-metal-0.1.0/equinix_metal/api/devices_api.py` & `equinix-metal-0.2.0/equinix_metal/api/events_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
@@ -16,93 +16,100 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictBool, StrictStr, conint, conlist
+from pydantic import Field, StrictStr, conint, conlist
 
 from typing import Optional
 
-from equinix_metal.models.create_device_request import CreateDeviceRequest
-from equinix_metal.models.device import Device
-from equinix_metal.models.device_list import DeviceList
-from equinix_metal.models.device_update_input import DeviceUpdateInput
-from equinix_metal.models.ip_assignment import IPAssignment
-from equinix_metal.models.ip_assignment_input import IPAssignmentInput
-from equinix_metal.models.ip_assignment_list import IPAssignmentList
+from equinix_metal.models.event import Event
+from equinix_metal.models.event_list import EventList
 
 from equinix_metal.api_client import ApiClient
 from equinix_metal.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class DevicesApi(object):
+class EventsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_device(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], create_device_request : Annotated[CreateDeviceRequest, Field(..., description="Device to create")], **kwargs) -> Device:  # noqa: E501
-        """Create a device  # noqa: E501
+    def find_device_events(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> EventList:  # noqa: E501
+        """Retrieve device's events  # noqa: E501
 
-        Creates a new device and provisions it in the specified location.  Device type-specific options are accepted.  For example, `baremetal` devices accept `operating_system`, `hostname`, and `plan`. These parameters may not be accepted for other device types. The default device type is `baremetal`.  # noqa: E501
+        Returns a list of events pertaining to a specific device  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_device(id, create_device_request, async_req=True)
+        >>> thread = api.find_device_events(id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param id: Project UUID (required)
+        :param id: Device UUID (required)
         :type id: str
-        :param create_device_request: Device to create (required)
-        :type create_device_request: CreateDeviceRequest
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Device
+        :rtype: EventList
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_device_with_http_info(id, create_device_request, **kwargs)  # noqa: E501
+        return self.find_device_events_with_http_info(id, include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_device_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], create_device_request : Annotated[CreateDeviceRequest, Field(..., description="Device to create")], **kwargs):  # noqa: E501
-        """Create a device  # noqa: E501
+    def find_device_events_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+        """Retrieve device's events  # noqa: E501
 
-        Creates a new device and provisions it in the specified location.  Device type-specific options are accepted.  For example, `baremetal` devices accept `operating_system`, `hostname`, and `plan`. These parameters may not be accepted for other device types. The default device type is `baremetal`.  # noqa: E501
+        Returns a list of events pertaining to a specific device  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_device_with_http_info(id, create_device_request, async_req=True)
+        >>> thread = api.find_device_events_with_http_info(id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param id: Project UUID (required)
+        :param id: Device UUID (required)
         :type id: str
-        :param create_device_request: Device to create (required)
-        :type create_device_request: CreateDeviceRequest
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -116,22 +123,25 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(Device, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(EventList, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'create_device_request'
+            'include',
+            'exclude',
+            'page',
+            'per_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -142,63 +152,66 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_device" % _key
+                    " to method find_device_events" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
+        if _params.get('page') is not None:  # noqa: E501
+            _query_params.append(('page', _params['page']))
+
+        if _params.get('per_page') is not None:  # noqa: E501
+            _query_params.append(('per_page', _params['per_page']))
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['create_device_request']:
-            _body_params = _params['create_device_request']
-
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '201': "Device",
+            '200': "EventList",
             '401': "Error",
             '403': "Error",
             '404': "Error",
-            '422': "Error",
         }
 
         return self.api_client.call_api(
-            '/projects/{id}/devices', 'POST',
+            '/devices/{id}/events', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -207,61 +220,65 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_ip_assignment(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], ip_assignment_input : Annotated[IPAssignmentInput, Field(..., description="IPAssignment to create")], **kwargs) -> IPAssignment:  # noqa: E501
-        """Create an ip assignment  # noqa: E501
+    def find_event_by_id(self, id : Annotated[StrictStr, Field(..., description="Event UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> Event:  # noqa: E501
+        """Retrieve an event  # noqa: E501
 
-        Creates an ip assignment for a device.  # noqa: E501
+        Returns a single event if the user has access  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_ip_assignment(id, ip_assignment_input, async_req=True)
+        >>> thread = api.find_event_by_id(id, include, exclude, async_req=True)
         >>> result = thread.get()
 
-        :param id: Device UUID (required)
+        :param id: Event UUID (required)
         :type id: str
-        :param ip_assignment_input: IPAssignment to create (required)
-        :type ip_assignment_input: IPAssignmentInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: IPAssignment
+        :rtype: Event
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_ip_assignment_with_http_info(id, ip_assignment_input, **kwargs)  # noqa: E501
+        return self.find_event_by_id_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_ip_assignment_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], ip_assignment_input : Annotated[IPAssignmentInput, Field(..., description="IPAssignment to create")], **kwargs):  # noqa: E501
-        """Create an ip assignment  # noqa: E501
+    def find_event_by_id_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Event UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
+        """Retrieve an event  # noqa: E501
 
-        Creates an ip assignment for a device.  # noqa: E501
+        Returns a single event if the user has access  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_ip_assignment_with_http_info(id, ip_assignment_input, async_req=True)
+        >>> thread = api.find_event_by_id_with_http_info(id, include, exclude, async_req=True)
         >>> result = thread.get()
 
-        :param id: Device UUID (required)
+        :param id: Event UUID (required)
         :type id: str
-        :param ip_assignment_input: IPAssignment to create (required)
-        :type ip_assignment_input: IPAssignmentInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -275,22 +292,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(IPAssignment, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(Event, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'ip_assignment_input'
+            'include',
+            'exclude'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -301,62 +319,60 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_ip_assignment" % _key
+                    " to method find_event_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['ip_assignment_input']:
-            _body_params = _params['ip_assignment_input']
-
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '201': "IPAssignment",
+            '200': "Event",
             '401': "Error",
+            '403': "Error",
             '404': "Error",
-            '422': "Error",
         }
 
         return self.api_client.call_api(
-            '/devices/{id}/ips', 'POST',
+            '/events/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -365,61 +381,69 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_device(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], force_delete : Annotated[Optional[StrictBool], Field(description="Force the deletion of the device, by detaching any storage volume still active.")] = None, **kwargs) -> None:  # noqa: E501
-        """Delete the device  # noqa: E501
+    def find_events(self, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> EventList:  # noqa: E501
+        """Retrieve current user's events  # noqa: E501
 
-        Deletes a device and deprovisions it in our datacenter.  # noqa: E501
+        Returns a list of the current user’s events  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_device(id, force_delete, async_req=True)
+        >>> thread = api.find_events(include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param id: Device UUID (required)
-        :type id: str
-        :param force_delete: Force the deletion of the device, by detaching any storage volume still active.
-        :type force_delete: bool
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: EventList
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_device_with_http_info(id, force_delete, **kwargs)  # noqa: E501
+        return self.find_events_with_http_info(include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_device_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], force_delete : Annotated[Optional[StrictBool], Field(description="Force the deletion of the device, by detaching any storage volume still active.")] = None, **kwargs):  # noqa: E501
-        """Delete the device  # noqa: E501
+    def find_events_with_http_info(self, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+        """Retrieve current user's events  # noqa: E501
 
-        Deletes a device and deprovisions it in our datacenter.  # noqa: E501
+        Returns a list of the current user’s events  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_device_with_http_info(id, force_delete, async_req=True)
+        >>> thread = api.find_events_with_http_info(include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param id: Device UUID (required)
-        :type id: str
-        :param force_delete: Force the deletion of the device, by detaching any storage volume still active.
-        :type force_delete: bool
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -433,22 +457,24 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(EventList, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
-            'force_delete'
+            'include',
+            'exclude',
+            'page',
+            'per_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -459,31 +485,39 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_device" % _key
+                    " to method find_events" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
 
         # process the query parameters
         _query_params = []
-        if _params.get('force_delete') is not None:  # noqa: E501
-            _query_params.append(('force_delete', _params['force_delete']))
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
+        if _params.get('page') is not None:  # noqa: E501
+            _query_params.append(('page', _params['page']))
+
+        if _params.get('per_page') is not None:  # noqa: E501
+            _query_params.append(('per_page', _params['per_page']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
@@ -491,18 +525,21 @@
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "EventList",
+            '401': "Error",
+        }
 
         return self.api_client.call_api(
-            '/devices/{id}', 'DELETE',
+            '/events', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -511,65 +548,73 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def find_device_by_id(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> Device:  # noqa: E501
-        """Retrieve a device  # noqa: E501
+    def find_interconnection_events(self, connection_id : Annotated[StrictStr, Field(..., description="Interconnection UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> EventList:  # noqa: E501
+        """Retrieve interconnection events  # noqa: E501
 
-        Type-specific options (such as facility for baremetal devices) will be included as part of the main data structure.                          State value can be one of: active inactive queued or provisioning  # noqa: E501
+        Returns a list of the interconnection events  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_device_by_id(id, include, exclude, async_req=True)
+        >>> thread = api.find_interconnection_events(connection_id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param id: Device UUID (required)
-        :type id: str
+        :param connection_id: Interconnection UUID (required)
+        :type connection_id: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Device
+        :rtype: EventList
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_device_by_id_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
+        return self.find_interconnection_events_with_http_info(connection_id, include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_device_by_id_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
-        """Retrieve a device  # noqa: E501
+    def find_interconnection_events_with_http_info(self, connection_id : Annotated[StrictStr, Field(..., description="Interconnection UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+        """Retrieve interconnection events  # noqa: E501
 
-        Type-specific options (such as facility for baremetal devices) will be included as part of the main data structure.                          State value can be one of: active inactive queued or provisioning  # noqa: E501
+        Returns a list of the interconnection events  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_device_by_id_with_http_info(id, include, exclude, async_req=True)
+        >>> thread = api.find_interconnection_events_with_http_info(connection_id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param id: Device UUID (required)
-        :type id: str
+        :param connection_id: Interconnection UUID (required)
+        :type connection_id: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -583,23 +628,25 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(Device, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(EventList, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
+            'connection_id',
             'include',
-            'exclude'
+            'exclude',
+            'page',
+            'per_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -610,37 +657,43 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method find_device_by_id" % _key
+                    " to method find_interconnection_events" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
+        if _params['connection_id']:
+            _path_params['connection_id'] = _params['connection_id']
 
 
         # process the query parameters
         _query_params = []
         if _params.get('include') is not None:  # noqa: E501
             _query_params.append(('include', _params['include']))
             _collection_formats['include'] = 'csv'
 
         if _params.get('exclude') is not None:  # noqa: E501
             _query_params.append(('exclude', _params['exclude']))
             _collection_formats['exclude'] = 'csv'
 
+        if _params.get('page') is not None:  # noqa: E501
+            _query_params.append(('page', _params['page']))
+
+        if _params.get('per_page') is not None:  # noqa: E501
+            _query_params.append(('per_page', _params['per_page']))
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
@@ -648,22 +701,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '200': "Device",
+            '200': "EventList",
             '401': "Error",
             '403': "Error",
             '404': "Error",
         }
 
         return self.api_client.call_api(
-            '/devices/{id}', 'GET',
+            '/connections/{connection_id}/events', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -672,65 +725,77 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def find_ip_assignments(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> IPAssignmentList:  # noqa: E501
-        """Retrieve all ip assignments  # noqa: E501
+    def find_interconnection_port_events(self, connection_id : Annotated[StrictStr, Field(..., description="Interconnection UUID")], id : Annotated[StrictStr, Field(..., description="Interconnection Port UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> Event:  # noqa: E501
+        """Retrieve interconnection port events  # noqa: E501
 
-        Returns all ip assignments for a device.  # noqa: E501
+        Returns a list of the interconnection port events  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_ip_assignments(id, include, exclude, async_req=True)
+        >>> thread = api.find_interconnection_port_events(connection_id, id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param id: Device UUID (required)
+        :param connection_id: Interconnection UUID (required)
+        :type connection_id: str
+        :param id: Interconnection Port UUID (required)
         :type id: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: IPAssignmentList
+        :rtype: Event
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_ip_assignments_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
+        return self.find_interconnection_port_events_with_http_info(connection_id, id, include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_ip_assignments_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
-        """Retrieve all ip assignments  # noqa: E501
+    def find_interconnection_port_events_with_http_info(self, connection_id : Annotated[StrictStr, Field(..., description="Interconnection UUID")], id : Annotated[StrictStr, Field(..., description="Interconnection Port UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+        """Retrieve interconnection port events  # noqa: E501
 
-        Returns all ip assignments for a device.  # noqa: E501
+        Returns a list of the interconnection port events  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_ip_assignments_with_http_info(id, include, exclude, async_req=True)
+        >>> thread = api.find_interconnection_port_events_with_http_info(connection_id, id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param id: Device UUID (required)
+        :param connection_id: Interconnection UUID (required)
+        :type connection_id: str
+        :param id: Interconnection Port UUID (required)
         :type id: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -744,23 +809,26 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(IPAssignmentList, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(Event, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'connection_id',
             'id',
             'include',
-            'exclude'
+            'exclude',
+            'page',
+            'per_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -771,37 +839,46 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method find_ip_assignments" % _key
+                    " to method find_interconnection_port_events" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['connection_id']:
+            _path_params['connection_id'] = _params['connection_id']
+
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
         if _params.get('include') is not None:  # noqa: E501
             _query_params.append(('include', _params['include']))
             _collection_formats['include'] = 'csv'
 
         if _params.get('exclude') is not None:  # noqa: E501
             _query_params.append(('exclude', _params['exclude']))
             _collection_formats['exclude'] = 'csv'
 
+        if _params.get('page') is not None:  # noqa: E501
+            _query_params.append(('page', _params['page']))
+
+        if _params.get('per_page') is not None:  # noqa: E501
+            _query_params.append(('per_page', _params['per_page']))
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
@@ -809,21 +886,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '200': "IPAssignmentList",
+            '200': "Event",
             '401': "Error",
+            '403': "Error",
             '404': "Error",
         }
 
         return self.api_client.call_api(
-            '/devices/{id}/ips', 'GET',
+            '/connections/{connection_id}/ports/{id}/events', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -832,36 +910,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def find_organization_devices(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], facility : Annotated[Optional[StrictStr], Field(description="Filter by device facility")] = None, hostname : Annotated[Optional[StrictStr], Field(description="Filter by partial hostname")] = None, reserved : Annotated[Optional[StrictBool], Field(description="Filter only reserved instances")] = None, tag : Annotated[Optional[StrictStr], Field(description="Filter by device tag")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter by instance type (ondemand,spot,reserved)")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> DeviceList:  # noqa: E501
-        """Retrieve all devices of an organization  # noqa: E501
+    def find_organization_events(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> EventList:  # noqa: E501
+        """Retrieve organization's events  # noqa: E501
 
-        Provides a collection of devices for a given organization.  # noqa: E501
+        Returns a list of events for a single organization  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_organization_devices(id, facility, hostname, reserved, tag, type, include, exclude, page, per_page, async_req=True)
+        >>> thread = api.find_organization_events(id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
         :param id: Organization UUID (required)
         :type id: str
-        :param facility: Filter by device facility
-        :type facility: str
-        :param hostname: Filter by partial hostname
-        :type hostname: str
-        :param reserved: Filter only reserved instances
-        :type reserved: bool
-        :param tag: Filter by device tag
-        :type tag: str
-        :param type: Filter by instance type (ondemand,spot,reserved)
-        :type type: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
@@ -875,42 +943,32 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: DeviceList
+        :rtype: EventList
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_organization_devices_with_http_info(id, facility, hostname, reserved, tag, type, include, exclude, page, per_page, **kwargs)  # noqa: E501
+        return self.find_organization_events_with_http_info(id, include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_organization_devices_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], facility : Annotated[Optional[StrictStr], Field(description="Filter by device facility")] = None, hostname : Annotated[Optional[StrictStr], Field(description="Filter by partial hostname")] = None, reserved : Annotated[Optional[StrictBool], Field(description="Filter only reserved instances")] = None, tag : Annotated[Optional[StrictStr], Field(description="Filter by device tag")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter by instance type (ondemand,spot,reserved)")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
-        """Retrieve all devices of an organization  # noqa: E501
+    def find_organization_events_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+        """Retrieve organization's events  # noqa: E501
 
-        Provides a collection of devices for a given organization.  # noqa: E501
+        Returns a list of events for a single organization  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_organization_devices_with_http_info(id, facility, hostname, reserved, tag, type, include, exclude, page, per_page, async_req=True)
+        >>> thread = api.find_organization_events_with_http_info(id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
         :param id: Organization UUID (required)
         :type id: str
-        :param facility: Filter by device facility
-        :type facility: str
-        :param hostname: Filter by partial hostname
-        :type hostname: str
-        :param reserved: Filter only reserved instances
-        :type reserved: bool
-        :param tag: Filter by device tag
-        :type tag: str
-        :param type: Filter by instance type (ondemand,spot,reserved)
-        :type type: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
@@ -932,26 +990,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(DeviceList, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(EventList, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'facility',
-            'hostname',
-            'reserved',
-            'tag',
-            'type',
             'include',
             'exclude',
             'page',
             'per_page'
         ]
         _all_params.extend(
             [
@@ -966,44 +1019,29 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method find_organization_devices" % _key
+                    " to method find_organization_events" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
-        if _params.get('facility') is not None:  # noqa: E501
-            _query_params.append(('facility', _params['facility']))
-
-        if _params.get('hostname') is not None:  # noqa: E501
-            _query_params.append(('hostname', _params['hostname']))
-
-        if _params.get('reserved') is not None:  # noqa: E501
-            _query_params.append(('reserved', _params['reserved']))
-
-        if _params.get('tag') is not None:  # noqa: E501
-            _query_params.append(('tag', _params['tag']))
-
-        if _params.get('type') is not None:  # noqa: E501
-            _query_params.append(('type', _params['type']))
-
         if _params.get('include') is not None:  # noqa: E501
             _query_params.append(('include', _params['include']))
             _collection_formats['include'] = 'csv'
 
         if _params.get('exclude') is not None:  # noqa: E501
             _query_params.append(('exclude', _params['exclude']))
             _collection_formats['exclude'] = 'csv'
@@ -1025,22 +1063,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '200': "DeviceList",
+            '200': "EventList",
             '401': "Error",
             '403': "Error",
             '404': "Error",
         }
 
         return self.api_client.call_api(
-            '/organizations/{id}/devices', 'GET',
+            '/organizations/{id}/events', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1049,36 +1087,26 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def find_project_devices(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], facility : Annotated[Optional[StrictStr], Field(description="Filter by device facility")] = None, hostname : Annotated[Optional[StrictStr], Field(description="Filter by partial hostname")] = None, reserved : Annotated[Optional[StrictBool], Field(description="Filter only reserved instances")] = None, tag : Annotated[Optional[StrictStr], Field(description="Filter by device tag")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter by instance type (ondemand,spot,reserved)")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> DeviceList:  # noqa: E501
-        """Retrieve all devices of a project  # noqa: E501
+    def find_project_events(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> EventList:  # noqa: E501
+        """Retrieve project's events  # noqa: E501
 
-        Provides a collection of devices for a given project.  # noqa: E501
+        Returns a list of events for a single project  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_project_devices(id, facility, hostname, reserved, tag, type, include, exclude, page, per_page, async_req=True)
+        >>> thread = api.find_project_events(id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
         :param id: Project UUID (required)
         :type id: str
-        :param facility: Filter by device facility
-        :type facility: str
-        :param hostname: Filter by partial hostname
-        :type hostname: str
-        :param reserved: Filter only reserved instances
-        :type reserved: bool
-        :param tag: Filter by device tag
-        :type tag: str
-        :param type: Filter by instance type (ondemand,spot,reserved)
-        :type type: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
@@ -1092,42 +1120,32 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: DeviceList
+        :rtype: EventList
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_project_devices_with_http_info(id, facility, hostname, reserved, tag, type, include, exclude, page, per_page, **kwargs)  # noqa: E501
+        return self.find_project_events_with_http_info(id, include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_project_devices_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], facility : Annotated[Optional[StrictStr], Field(description="Filter by device facility")] = None, hostname : Annotated[Optional[StrictStr], Field(description="Filter by partial hostname")] = None, reserved : Annotated[Optional[StrictBool], Field(description="Filter only reserved instances")] = None, tag : Annotated[Optional[StrictStr], Field(description="Filter by device tag")] = None, type : Annotated[Optional[StrictStr], Field(description="Filter by instance type (ondemand,spot,reserved)")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
-        """Retrieve all devices of a project  # noqa: E501
+    def find_project_events_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+        """Retrieve project's events  # noqa: E501
 
-        Provides a collection of devices for a given project.  # noqa: E501
+        Returns a list of events for a single project  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_project_devices_with_http_info(id, facility, hostname, reserved, tag, type, include, exclude, page, per_page, async_req=True)
+        >>> thread = api.find_project_events_with_http_info(id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
         :param id: Project UUID (required)
         :type id: str
-        :param facility: Filter by device facility
-        :type facility: str
-        :param hostname: Filter by partial hostname
-        :type hostname: str
-        :param reserved: Filter only reserved instances
-        :type reserved: bool
-        :param tag: Filter by device tag
-        :type tag: str
-        :param type: Filter by instance type (ondemand,spot,reserved)
-        :type type: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
@@ -1149,26 +1167,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(DeviceList, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(EventList, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'facility',
-            'hostname',
-            'reserved',
-            'tag',
-            'type',
             'include',
             'exclude',
             'page',
             'per_page'
         ]
         _all_params.extend(
             [
@@ -1183,44 +1196,29 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method find_project_devices" % _key
+                    " to method find_project_events" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
-        if _params.get('facility') is not None:  # noqa: E501
-            _query_params.append(('facility', _params['facility']))
-
-        if _params.get('hostname') is not None:  # noqa: E501
-            _query_params.append(('hostname', _params['hostname']))
-
-        if _params.get('reserved') is not None:  # noqa: E501
-            _query_params.append(('reserved', _params['reserved']))
-
-        if _params.get('tag') is not None:  # noqa: E501
-            _query_params.append(('tag', _params['tag']))
-
-        if _params.get('type') is not None:  # noqa: E501
-            _query_params.append(('type', _params['type']))
-
         if _params.get('include') is not None:  # noqa: E501
             _query_params.append(('include', _params['include']))
             _collection_formats['include'] = 'csv'
 
         if _params.get('exclude') is not None:  # noqa: E501
             _query_params.append(('exclude', _params['exclude']))
             _collection_formats['exclude'] = 'csv'
@@ -1242,22 +1240,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '200': "DeviceList",
+            '200': "EventList",
             '401': "Error",
             '403': "Error",
             '404': "Error",
         }
 
         return self.api_client.call_api(
-            '/projects/{id}/devices', 'GET',
+            '/projects/{id}/events', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1266,61 +1264,73 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_device(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], device_update_input : Annotated[DeviceUpdateInput, Field(..., description="Facility to update")], **kwargs) -> Device:  # noqa: E501
-        """Update the device  # noqa: E501
+    def find_virtual_circuit_events(self, id : Annotated[StrictStr, Field(..., description="Virtual Circuit UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> Event:  # noqa: E501
+        """Retrieve interconnection events  # noqa: E501
 
-        Updates the device.  # noqa: E501
+        Returns a list of the virtual circuit events  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_device(id, device_update_input, async_req=True)
+        >>> thread = api.find_virtual_circuit_events(id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param id: Device UUID (required)
+        :param id: Virtual Circuit UUID (required)
         :type id: str
-        :param device_update_input: Facility to update (required)
-        :type device_update_input: DeviceUpdateInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Device
+        :rtype: Event
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_device_with_http_info(id, device_update_input, **kwargs)  # noqa: E501
+        return self.find_virtual_circuit_events_with_http_info(id, include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_device_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Device UUID")], device_update_input : Annotated[DeviceUpdateInput, Field(..., description="Facility to update")], **kwargs):  # noqa: E501
-        """Update the device  # noqa: E501
+    def find_virtual_circuit_events_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Virtual Circuit UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+        """Retrieve interconnection events  # noqa: E501
 
-        Updates the device.  # noqa: E501
+        Returns a list of the virtual circuit events  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_device_with_http_info(id, device_update_input, async_req=True)
+        >>> thread = api.find_virtual_circuit_events_with_http_info(id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param id: Device UUID (required)
+        :param id: Virtual Circuit UUID (required)
         :type id: str
-        :param device_update_input: Facility to update (required)
-        :type device_update_input: DeviceUpdateInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1334,22 +1344,25 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(Device, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(Event, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'device_update_input'
+            'include',
+            'exclude',
+            'page',
+            'per_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1360,63 +1373,66 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_device" % _key
+                    " to method find_virtual_circuit_events" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
+        if _params.get('page') is not None:  # noqa: E501
+            _query_params.append(('page', _params['page']))
+
+        if _params.get('per_page') is not None:  # noqa: E501
+            _query_params.append(('per_page', _params['per_page']))
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['device_update_input']:
-            _body_params = _params['device_update_input']
-
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '200': "Device",
+            '200': "Event",
             '401': "Error",
             '403': "Error",
             '404': "Error",
-            '422': "Error",
         }
 
         return self.api_client.call_api(
-            '/devices/{id}', 'PUT',
+            '/virtual-circuits/{id}/events', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `equinix-metal-0.1.0/equinix_metal/api/ip_addresses_api.py` & `equinix-metal-0.2.0/equinix_metal/api/ip_addresses_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `equinix-metal-0.1.0/equinix_metal/api/organizations_api.py` & `equinix-metal-0.2.0/equinix_metal/api/users_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
@@ -20,84 +20,83 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr, conint, conlist
 
 from typing import Optional
 
-from equinix_metal.models.organization import Organization
-from equinix_metal.models.organization_input import OrganizationInput
-from equinix_metal.models.organization_list import OrganizationList
-from equinix_metal.models.project import Project
-from equinix_metal.models.project_create_input import ProjectCreateInput
-from equinix_metal.models.project_list import ProjectList
+from equinix_metal.models.invitation_list import InvitationList
+from equinix_metal.models.user import User
+from equinix_metal.models.user_create_input import UserCreateInput
+from equinix_metal.models.user_list import UserList
+from equinix_metal.models.user_update_input import UserUpdateInput
 
 from equinix_metal.api_client import ApiClient
 from equinix_metal.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class OrganizationsApi(object):
+class UsersApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_organization(self, organization_input : Annotated[OrganizationInput, Field(..., description="Organization to create")], **kwargs) -> Organization:  # noqa: E501
-        """Create an organization  # noqa: E501
+    def create_user(self, user_create_input : Annotated[UserCreateInput, Field(..., description="User to create")], **kwargs) -> User:  # noqa: E501
+        """Create a user  # noqa: E501
 
-        Creates an organization.  # noqa: E501
+        Creates a user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_organization(organization_input, async_req=True)
+        >>> thread = api.create_user(user_create_input, async_req=True)
         >>> result = thread.get()
 
-        :param organization_input: Organization to create (required)
-        :type organization_input: OrganizationInput
+        :param user_create_input: User to create (required)
+        :type user_create_input: UserCreateInput
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Organization
+        :rtype: User
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_organization_with_http_info(organization_input, **kwargs)  # noqa: E501
+        return self.create_user_with_http_info(user_create_input, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_organization_with_http_info(self, organization_input : Annotated[OrganizationInput, Field(..., description="Organization to create")], **kwargs):  # noqa: E501
-        """Create an organization  # noqa: E501
+    def create_user_with_http_info(self, user_create_input : Annotated[UserCreateInput, Field(..., description="User to create")], **kwargs):  # noqa: E501
+        """Create a user  # noqa: E501
 
-        Creates an organization.  # noqa: E501
+        Creates a user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_organization_with_http_info(organization_input, async_req=True)
+        >>> thread = api.create_user_with_http_info(user_create_input, async_req=True)
         >>> result = thread.get()
 
-        :param organization_input: Organization to create (required)
-        :type organization_input: OrganizationInput
+        :param user_create_input: User to create (required)
+        :type user_create_input: UserCreateInput
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -111,21 +110,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(Organization, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(User, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'organization_input'
+            'user_create_input'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -136,15 +135,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_organization" % _key
+                    " to method create_user" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -155,16 +154,16 @@
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['organization_input']:
-            _body_params = _params['organization_input']
+        if _params['user_create_input']:
+            _body_params = _params['user_create_input']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -173,22 +172,21 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '201': "Organization",
+            '201': "User",
             '401': "Error",
-            '404': "Error",
             '422': "Error",
         }
 
         return self.api_client.call_api(
-            '/organizations', 'POST',
+            '/users', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -197,61 +195,61 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_organization_project(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], project_create_input : Annotated[ProjectCreateInput, Field(..., description="Project to create")], **kwargs) -> Project:  # noqa: E501
-        """Create a project for the organization  # noqa: E501
+    def find_current_user(self, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> User:  # noqa: E501
+        """Retrieve the current user  # noqa: E501
 
-        Creates a new project for the organization  # noqa: E501
+        Returns the user object for the currently logged-in user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_organization_project(id, project_create_input, async_req=True)
+        >>> thread = api.find_current_user(include, exclude, async_req=True)
         >>> result = thread.get()
 
-        :param id: Organization UUID (required)
-        :type id: str
-        :param project_create_input: Project to create (required)
-        :type project_create_input: ProjectCreateInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Project
+        :rtype: User
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_organization_project_with_http_info(id, project_create_input, **kwargs)  # noqa: E501
+        return self.find_current_user_with_http_info(include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_organization_project_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], project_create_input : Annotated[ProjectCreateInput, Field(..., description="Project to create")], **kwargs):  # noqa: E501
-        """Create a project for the organization  # noqa: E501
+    def find_current_user_with_http_info(self, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
+        """Retrieve the current user  # noqa: E501
 
-        Creates a new project for the organization  # noqa: E501
+        Returns the user object for the currently logged-in user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_organization_project_with_http_info(id, project_create_input, async_req=True)
+        >>> thread = api.find_current_user_with_http_info(include, exclude, async_req=True)
         >>> result = thread.get()
 
-        :param id: Organization UUID (required)
-        :type id: str
-        :param project_create_input: Project to create (required)
-        :type project_create_input: ProjectCreateInput
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -265,22 +263,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(Project, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(User, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
-            'project_create_input'
+            'include',
+            'exclude'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -291,61 +289,55 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_organization_project" % _key
+                    " to method find_current_user" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['project_create_input']:
-            _body_params = _params['project_create_input']
-
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '201': "Project",
+            '200': "User",
             '401': "Error",
-            '422': "Error",
         }
 
         return self.api_client.call_api(
-            '/organizations/{id}/projects', 'POST',
+            '/user', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -354,57 +346,69 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_organization(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], **kwargs) -> None:  # noqa: E501
-        """Delete the organization  # noqa: E501
+    def find_invitations(self, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> InvitationList:  # noqa: E501
+        """Retrieve current user invitations  # noqa: E501
 
-        Deletes the organization.  # noqa: E501
+        Returns all invitations in current user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_organization(id, async_req=True)
+        >>> thread = api.find_invitations(include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param id: Organization UUID (required)
-        :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: InvitationList
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_organization_with_http_info(id, **kwargs)  # noqa: E501
+        return self.find_invitations_with_http_info(include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_organization_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], **kwargs):  # noqa: E501
-        """Delete the organization  # noqa: E501
+    def find_invitations_with_http_info(self, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+        """Retrieve current user invitations  # noqa: E501
 
-        Deletes the organization.  # noqa: E501
+        Returns all invitations in current user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_organization_with_http_info(id, async_req=True)
+        >>> thread = api.find_invitations_with_http_info(include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param id: Organization UUID (required)
-        :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -418,21 +422,24 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(InvitationList, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'include',
+            'exclude',
+            'page',
+            'per_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -443,47 +450,63 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_organization" % _key
+                    " to method find_invitations" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
+        if _params.get('page') is not None:  # noqa: E501
+            _query_params.append(('page', _params['page']))
+
+        if _params.get('per_page') is not None:  # noqa: E501
+            _query_params.append(('per_page', _params['per_page']))
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '200': "InvitationList",
+            '401': "Error",
+            '403': "Error",
+            '404': "Error",
+        }
 
         return self.api_client.call_api(
-            '/organizations/{id}', 'DELETE',
+            '/invitations', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -492,25 +515,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def find_organization_by_id(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> Organization:  # noqa: E501
-        """Retrieve an organization's details  # noqa: E501
+    def find_user_by_id(self, id : Annotated[StrictStr, Field(..., description="User UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> User:  # noqa: E501
+        """Retrieve a user  # noqa: E501
 
-        Returns a single organization's details, if the user is authorized to view it.  # noqa: E501
+        Returns a single user if the user has access  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_organization_by_id(id, include, exclude, async_req=True)
+        >>> thread = api.find_user_by_id(id, include, exclude, async_req=True)
         >>> result = thread.get()
 
-        :param id: Organization UUID (required)
+        :param id: User UUID (required)
         :type id: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -521,31 +544,31 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Organization
+        :rtype: User
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_organization_by_id_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
+        return self.find_user_by_id_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_organization_by_id_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
-        """Retrieve an organization's details  # noqa: E501
+    def find_user_by_id_with_http_info(self, id : Annotated[StrictStr, Field(..., description="User UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
+        """Retrieve a user  # noqa: E501
 
-        Returns a single organization's details, if the user is authorized to view it.  # noqa: E501
+        Returns a single user if the user has access  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_organization_by_id_with_http_info(id, include, exclude, async_req=True)
+        >>> thread = api.find_user_by_id_with_http_info(id, include, exclude, async_req=True)
         >>> result = thread.get()
 
-        :param id: Organization UUID (required)
+        :param id: User UUID (required)
         :type id: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -564,15 +587,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(Organization, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(User, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
             'include',
@@ -591,15 +614,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method find_organization_by_id" % _key
+                    " to method find_user_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -629,22 +652,22 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '200': "Organization",
+            '200': "User",
             '401': "Error",
             '403': "Error",
             '404': "Error",
         }
 
         return self.api_client.call_api(
-            '/organizations/{id}', 'GET',
+            '/users/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -653,77 +676,57 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def find_organization_projects(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, name : Annotated[Optional[StrictStr], Field(description="Search by name substring")] = None, **kwargs) -> ProjectList:  # noqa: E501
-        """Retrieve all projects of an organization  # noqa: E501
+    def find_user_customdata(self, id : Annotated[StrictStr, Field(..., description="User UUID")], **kwargs) -> None:  # noqa: E501
+        """Retrieve the custom metadata of a user  # noqa: E501
 
-        Returns a collection of projects that belong to the organization.  # noqa: E501
+        Provides the custom metadata stored for this user in json format  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_organization_projects(id, include, exclude, page, per_page, name, async_req=True)
+        >>> thread = api.find_user_customdata(id, async_req=True)
         >>> result = thread.get()
 
-        :param id: Organization UUID (required)
+        :param id: User UUID (required)
         :type id: str
-        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
-        :type include: List[str]
-        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
-        :type exclude: List[str]
-        :param page: Page to return
-        :type page: int
-        :param per_page: Items returned per page
-        :type per_page: int
-        :param name: Search by name substring
-        :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ProjectList
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_organization_projects_with_http_info(id, include, exclude, page, per_page, name, **kwargs)  # noqa: E501
+        return self.find_user_customdata_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_organization_projects_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, name : Annotated[Optional[StrictStr], Field(description="Search by name substring")] = None, **kwargs):  # noqa: E501
-        """Retrieve all projects of an organization  # noqa: E501
+    def find_user_customdata_with_http_info(self, id : Annotated[StrictStr, Field(..., description="User UUID")], **kwargs):  # noqa: E501
+        """Retrieve the custom metadata of a user  # noqa: E501
 
-        Returns a collection of projects that belong to the organization.  # noqa: E501
+        Provides the custom metadata stored for this user in json format  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_organization_projects_with_http_info(id, include, exclude, page, per_page, name, async_req=True)
+        >>> thread = api.find_user_customdata_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param id: Organization UUID (required)
+        :param id: User UUID (required)
         :type id: str
-        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
-        :type include: List[str]
-        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
-        :type exclude: List[str]
-        :param page: Page to return
-        :type page: int
-        :param per_page: Items returned per page
-        :type per_page: int
-        :param name: Search by name substring
-        :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -737,26 +740,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ProjectList, status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
-            'include',
-            'exclude',
-            'page',
-            'per_page',
-            'name'
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -767,67 +765,47 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method find_organization_projects" % _key
+                    " to method find_user_customdata" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
-        if _params.get('include') is not None:  # noqa: E501
-            _query_params.append(('include', _params['include']))
-            _collection_formats['include'] = 'csv'
-
-        if _params.get('exclude') is not None:  # noqa: E501
-            _query_params.append(('exclude', _params['exclude']))
-            _collection_formats['exclude'] = 'csv'
-
-        if _params.get('page') is not None:  # noqa: E501
-            _query_params.append(('page', _params['page']))
-
-        if _params.get('per_page') is not None:  # noqa: E501
-            _query_params.append(('per_page', _params['per_page']))
-
-        if _params.get('name') is not None:  # noqa: E501
-            _query_params.append(('name', _params['name']))
-
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
-        _response_types_map = {
-            '200': "ProjectList",
-            '401': "Error",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/organizations/{id}/projects', 'GET',
+            '/users/{id}/customdata', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -836,28 +814,24 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def find_organizations(self, personal : Annotated[Optional[StrictStr], Field(description="Include, exclude or show only personal organizations.")] = None, without_projects : Annotated[Optional[StrictStr], Field(description="Include, exclude or show only organizations that have no projects.")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> OrganizationList:  # noqa: E501
-        """Retrieve all organizations  # noqa: E501
+    def find_users(self, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> UserList:  # noqa: E501
+        """Retrieve all users  # noqa: E501
 
-        Returns a list of organizations that are accessible to the current user.  # noqa: E501
+        Returns a list of users that the are accessible to the current user (all users in the current user’s projects, essentially).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_organizations(personal, without_projects, include, exclude, page, per_page, async_req=True)
+        >>> thread = api.find_users(include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param personal: Include, exclude or show only personal organizations.
-        :type personal: str
-        :param without_projects: Include, exclude or show only organizations that have no projects.
-        :type without_projects: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
@@ -871,34 +845,30 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: OrganizationList
+        :rtype: UserList
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_organizations_with_http_info(personal, without_projects, include, exclude, page, per_page, **kwargs)  # noqa: E501
+        return self.find_users_with_http_info(include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_organizations_with_http_info(self, personal : Annotated[Optional[StrictStr], Field(description="Include, exclude or show only personal organizations.")] = None, without_projects : Annotated[Optional[StrictStr], Field(description="Include, exclude or show only organizations that have no projects.")] = None, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
-        """Retrieve all organizations  # noqa: E501
+    def find_users_with_http_info(self, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+        """Retrieve all users  # noqa: E501
 
-        Returns a list of organizations that are accessible to the current user.  # noqa: E501
+        Returns a list of users that the are accessible to the current user (all users in the current user’s projects, essentially).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_organizations_with_http_info(personal, without_projects, include, exclude, page, per_page, async_req=True)
+        >>> thread = api.find_users_with_http_info(include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param personal: Include, exclude or show only personal organizations.
-        :type personal: str
-        :param without_projects: Include, exclude or show only organizations that have no projects.
-        :type without_projects: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
@@ -920,22 +890,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(OrganizationList, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(UserList, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'personal',
-            'without_projects',
             'include',
             'exclude',
             'page',
             'per_page'
         ]
         _all_params.extend(
             [
@@ -950,32 +918,26 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method find_organizations" % _key
+                    " to method find_users" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
-        if _params.get('personal') is not None:  # noqa: E501
-            _query_params.append(('personal', _params['personal']))
-
-        if _params.get('without_projects') is not None:  # noqa: E501
-            _query_params.append(('without_projects', _params['without_projects']))
-
         if _params.get('include') is not None:  # noqa: E501
             _query_params.append(('include', _params['include']))
             _collection_formats['include'] = 'csv'
 
         if _params.get('exclude') is not None:  # noqa: E501
             _query_params.append(('exclude', _params['exclude']))
             _collection_formats['exclude'] = 'csv'
@@ -997,20 +959,20 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '200': "OrganizationList",
+            '200': "UserList",
             '401': "Error",
         }
 
         return self.api_client.call_api(
-            '/organizations', 'GET',
+            '/users', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1019,61 +981,57 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_organization(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], organization_input : Annotated[OrganizationInput, Field(..., description="Organization to update")], **kwargs) -> Organization:  # noqa: E501
-        """Update the organization  # noqa: E501
+    def update_current_user(self, user_update_input : Annotated[UserUpdateInput, Field(..., description="User to update")], **kwargs) -> User:  # noqa: E501
+        """Update the current user  # noqa: E501
 
-        Updates the organization.  # noqa: E501
+        Updates the currently logged-in user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_organization(id, organization_input, async_req=True)
+        >>> thread = api.update_current_user(user_update_input, async_req=True)
         >>> result = thread.get()
 
-        :param id: Organization UUID (required)
-        :type id: str
-        :param organization_input: Organization to update (required)
-        :type organization_input: OrganizationInput
+        :param user_update_input: User to update (required)
+        :type user_update_input: UserUpdateInput
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Organization
+        :rtype: User
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_organization_with_http_info(id, organization_input, **kwargs)  # noqa: E501
+        return self.update_current_user_with_http_info(user_update_input, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_organization_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Organization UUID")], organization_input : Annotated[OrganizationInput, Field(..., description="Organization to update")], **kwargs):  # noqa: E501
-        """Update the organization  # noqa: E501
+    def update_current_user_with_http_info(self, user_update_input : Annotated[UserUpdateInput, Field(..., description="User to update")], **kwargs):  # noqa: E501
+        """Update the current user  # noqa: E501
 
-        Updates the organization.  # noqa: E501
+        Updates the currently logged-in user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_organization_with_http_info(id, organization_input, async_req=True)
+        >>> thread = api.update_current_user_with_http_info(user_update_input, async_req=True)
         >>> result = thread.get()
 
-        :param id: Organization UUID (required)
-        :type id: str
-        :param organization_input: Organization to update (required)
-        :type organization_input: OrganizationInput
+        :param user_update_input: User to update (required)
+        :type user_update_input: UserUpdateInput
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1087,22 +1045,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(Organization, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(User, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id',
-            'organization_input'
+            'user_update_input'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1113,38 +1070,35 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_organization" % _key
+                    " to method update_current_user" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
 
         # process the query parameters
         _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['organization_input']:
-            _body_params = _params['organization_input']
+        if _params['user_update_input']:
+            _body_params = _params['user_update_input']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -1153,23 +1107,21 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '200': "Organization",
+            '200': "User",
             '401': "Error",
-            '403': "Error",
-            '404': "Error",
             '422': "Error",
         }
 
         return self.api_client.call_api(
-            '/organizations/{id}', 'PUT',
+            '/user', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `equinix-metal-0.1.0/equinix_metal/api/projects_api.py` & `equinix-metal-0.2.0/equinix_metal/api/metal_gateways_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
@@ -20,82 +20,101 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import Field, StrictStr, conint, conlist
 
 from typing import Optional
 
-from equinix_metal.models.project import Project
-from equinix_metal.models.project_create_from_root_input import ProjectCreateFromRootInput
-from equinix_metal.models.project_list import ProjectList
-from equinix_metal.models.project_update_input import ProjectUpdateInput
+from equinix_metal.models.create_metal_gateway_request import CreateMetalGatewayRequest
+from equinix_metal.models.find_metal_gateway_by_id200_response import FindMetalGatewayById200Response
+from equinix_metal.models.metal_gateway_list import MetalGatewayList
 
 from equinix_metal.api_client import ApiClient
 from equinix_metal.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ProjectsApi(object):
+class MetalGatewaysApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_project(self, project_create_from_root_input : Annotated[ProjectCreateFromRootInput, Field(..., description="Project to create")], **kwargs) -> Project:  # noqa: E501
-        """Create a project  # noqa: E501
+    def create_metal_gateway(self, project_id : Annotated[StrictStr, Field(..., description="Project UUID")], create_metal_gateway_request : Annotated[CreateMetalGatewayRequest, Field(..., description="Metal Gateway to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> FindMetalGatewayById200Response:  # noqa: E501
+        """Create a metal gateway  # noqa: E501
 
-        Creates a new project for the user default organization. If the user don't have an organization, a new one will be created.  # noqa: E501
+        Create a metal gateway in a project  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_project(project_create_from_root_input, async_req=True)
+        >>> thread = api.create_metal_gateway(project_id, create_metal_gateway_request, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param project_create_from_root_input: Project to create (required)
-        :type project_create_from_root_input: ProjectCreateFromRootInput
+        :param project_id: Project UUID (required)
+        :type project_id: str
+        :param create_metal_gateway_request: Metal Gateway to create (required)
+        :type create_metal_gateway_request: CreateMetalGatewayRequest
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Project
+        :rtype: FindMetalGatewayById200Response
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_project_with_http_info(project_create_from_root_input, **kwargs)  # noqa: E501
+        return self.create_metal_gateway_with_http_info(project_id, create_metal_gateway_request, include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_project_with_http_info(self, project_create_from_root_input : Annotated[ProjectCreateFromRootInput, Field(..., description="Project to create")], **kwargs):  # noqa: E501
-        """Create a project  # noqa: E501
+    def create_metal_gateway_with_http_info(self, project_id : Annotated[StrictStr, Field(..., description="Project UUID")], create_metal_gateway_request : Annotated[CreateMetalGatewayRequest, Field(..., description="Metal Gateway to create")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+        """Create a metal gateway  # noqa: E501
 
-        Creates a new project for the user default organization. If the user don't have an organization, a new one will be created.  # noqa: E501
+        Create a metal gateway in a project  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_project_with_http_info(project_create_from_root_input, async_req=True)
+        >>> thread = api.create_metal_gateway_with_http_info(project_id, create_metal_gateway_request, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
-        :param project_create_from_root_input: Project to create (required)
-        :type project_create_from_root_input: ProjectCreateFromRootInput
+        :param project_id: Project UUID (required)
+        :type project_id: str
+        :param create_metal_gateway_request: Metal Gateway to create (required)
+        :type create_metal_gateway_request: CreateMetalGatewayRequest
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
+        :param page: Page to return
+        :type page: int
+        :param per_page: Items returned per page
+        :type per_page: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -109,21 +128,26 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(Project, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(FindMetalGatewayById200Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'project_create_from_root_input'
+            'project_id',
+            'create_metal_gateway_request',
+            'include',
+            'exclude',
+            'page',
+            'per_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -134,35 +158,52 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_project" % _key
+                    " to method create_metal_gateway" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['project_id']:
+            _path_params['project_id'] = _params['project_id']
+
 
         # process the query parameters
         _query_params = []
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
+
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
+
+        if _params.get('page') is not None:  # noqa: E501
+            _query_params.append(('page', _params['page']))
+
+        if _params.get('per_page') is not None:  # noqa: E501
+            _query_params.append(('per_page', _params['per_page']))
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['project_create_from_root_input']:
-            _body_params = _params['project_create_from_root_input']
+        if _params['create_metal_gateway_request']:
+            _body_params = _params['create_metal_gateway_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
@@ -171,21 +212,22 @@
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '201': "Project",
+            '201': "FindMetalGatewayById200Response",
             '401': "Error",
+            '404': "Error",
             '422': "Error",
         }
 
         return self.api_client.call_api(
-            '/projects', 'POST',
+            '/projects/{project_id}/metal-gateways', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -194,57 +236,65 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_project(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], **kwargs) -> None:  # noqa: E501
-        """Delete the project  # noqa: E501
+    def delete_metal_gateway(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> FindMetalGatewayById200Response:  # noqa: E501
+        """Deletes the metal gateway  # noqa: E501
 
-        Deletes the project.  # noqa: E501
+        Deletes a specific metal gateway  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_project(id, async_req=True)
+        >>> thread = api.delete_metal_gateway(id, include, exclude, async_req=True)
         >>> result = thread.get()
 
-        :param id: Project UUID (required)
+        :param id: Metal Gateway UUID (required)
         :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: FindMetalGatewayById200Response
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_project_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_metal_gateway_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_project_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], **kwargs):  # noqa: E501
-        """Delete the project  # noqa: E501
+    def delete_metal_gateway_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
+        """Deletes the metal gateway  # noqa: E501
 
-        Deletes the project.  # noqa: E501
+        Deletes a specific metal gateway  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_project_with_http_info(id, async_req=True)
+        >>> thread = api.delete_metal_gateway_with_http_info(id, include, exclude, async_req=True)
         >>> result = thread.get()
 
-        :param id: Project UUID (required)
+        :param id: Metal Gateway UUID (required)
         :type id: str
+        :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
+        :type include: List[str]
+        :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
+        :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -258,21 +308,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: None
+        :rtype: tuple(FindMetalGatewayById200Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'id',
+            'include',
+            'exclude'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -283,193 +335,59 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_project" % _key
+                    " to method delete_metal_gateway" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
 
         # process the query parameters
         _query_params = []
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ['x_auth_token']  # noqa: E501
-
-        _response_types_map = {}
-
-        return self.api_client.call_api(
-            '/projects/{id}', 'DELETE',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def find_ip_reservation_customdata(self, project_id : Annotated[StrictStr, Field(..., description="Project UUID")], id : Annotated[StrictStr, Field(..., description="Ip Reservation UUID")], **kwargs) -> None:  # noqa: E501
-        """Retrieve the custom metadata of an IP Reservation  # noqa: E501
-
-        Provides the custom metadata stored for this IP Reservation in json format  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.find_ip_reservation_customdata(project_id, id, async_req=True)
-        >>> result = thread.get()
-
-        :param project_id: Project UUID (required)
-        :type project_id: str
-        :param id: Ip Reservation UUID (required)
-        :type id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: None
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.find_ip_reservation_customdata_with_http_info(project_id, id, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def find_ip_reservation_customdata_with_http_info(self, project_id : Annotated[StrictStr, Field(..., description="Project UUID")], id : Annotated[StrictStr, Field(..., description="Ip Reservation UUID")], **kwargs):  # noqa: E501
-        """Retrieve the custom metadata of an IP Reservation  # noqa: E501
-
-        Provides the custom metadata stored for this IP Reservation in json format  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.find_ip_reservation_customdata_with_http_info(project_id, id, async_req=True)
-        >>> result = thread.get()
-
-        :param project_id: Project UUID (required)
-        :type project_id: str
-        :param id: Ip Reservation UUID (required)
-        :type id: str
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: None
-        """
-
-        _params = locals()
-
-        _all_params = [
-            'project_id',
-            'id'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method find_ip_reservation_customdata" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-        if _params['project_id']:
-            _path_params['project_id'] = _params['project_id']
-
-        if _params['id']:
-            _path_params['id'] = _params['id']
+        if _params.get('include') is not None:  # noqa: E501
+            _query_params.append(('include', _params['include']))
+            _collection_formats['include'] = 'csv'
 
+        if _params.get('exclude') is not None:  # noqa: E501
+            _query_params.append(('exclude', _params['exclude']))
+            _collection_formats['exclude'] = 'csv'
 
-        # process the query parameters
-        _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
-        _response_types_map = {}
+        _response_types_map = {
+            '202': "FindMetalGatewayById200Response",
+            '401': "Error",
+            '404': "Error",
+        }
 
         return self.api_client.call_api(
-            '/projects/{project_id}/ips/{id}/customdata', 'GET',
+            '/metal-gateways/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -478,25 +396,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def find_project_by_id(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> Project:  # noqa: E501
-        """Retrieve a project  # noqa: E501
+    def find_metal_gateway_by_id(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs) -> FindMetalGatewayById200Response:  # noqa: E501
+        """Returns the metal gateway  # noqa: E501
 
-        Returns a single project if the user has access  # noqa: E501
+        Returns a specific metal gateway  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_project_by_id(id, include, exclude, async_req=True)
+        >>> thread = api.find_metal_gateway_by_id(id, include, exclude, async_req=True)
         >>> result = thread.get()
 
-        :param id: Project UUID (required)
+        :param id: Metal Gateway UUID (required)
         :type id: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -507,31 +425,31 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: Project
+        :rtype: FindMetalGatewayById200Response
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_project_by_id_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
+        return self.find_metal_gateway_by_id_with_http_info(id, include, exclude, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_project_by_id_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
-        """Retrieve a project  # noqa: E501
+    def find_metal_gateway_by_id_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Metal Gateway UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, **kwargs):  # noqa: E501
+        """Returns the metal gateway  # noqa: E501
 
-        Returns a single project if the user has access  # noqa: E501
+        Returns a specific metal gateway  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_project_by_id_with_http_info(id, include, exclude, async_req=True)
+        >>> thread = api.find_metal_gateway_by_id_with_http_info(id, include, exclude, async_req=True)
         >>> result = thread.get()
 
-        :param id: Project UUID (required)
+        :param id: Metal Gateway UUID (required)
         :type id: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
@@ -550,15 +468,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(Project, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(FindMetalGatewayById200Response, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
             'include',
@@ -577,15 +495,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method find_project_by_id" % _key
+                    " to method find_metal_gateway_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -615,22 +533,21 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '200': "Project",
+            '200': "FindMetalGatewayById200Response",
             '401': "Error",
-            '403': "Error",
             '404': "Error",
         }
 
         return self.api_client.call_api(
-            '/projects/{id}', 'GET',
+            '/metal-gateways/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -639,73 +556,73 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def find_projects(self, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, name : Annotated[Optional[StrictStr], Field(description="Search by name substring")] = None, **kwargs) -> ProjectList:  # noqa: E501
-        """Retrieve all projects  # noqa: E501
+    def find_metal_gateways_by_project(self, project_id : Annotated[StrictStr, Field(..., description="Project UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs) -> MetalGatewayList:  # noqa: E501
+        """Returns all metal gateways for a project  # noqa: E501
 
-        Returns a collection of projects that the current user is a member of.  # noqa: E501
+        Return all metal gateways for a project  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_projects(include, exclude, page, per_page, name, async_req=True)
+        >>> thread = api.find_metal_gateways_by_project(project_id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
+        :param project_id: Project UUID (required)
+        :type project_id: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
         :type per_page: int
-        :param name: Search by name substring
-        :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ProjectList
+        :rtype: MetalGatewayList
         """
         kwargs['_return_http_data_only'] = True
-        return self.find_projects_with_http_info(include, exclude, page, per_page, name, **kwargs)  # noqa: E501
+        return self.find_metal_gateways_by_project_with_http_info(project_id, include, exclude, page, per_page, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def find_projects_with_http_info(self, include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, name : Annotated[Optional[StrictStr], Field(description="Search by name substring")] = None, **kwargs):  # noqa: E501
-        """Retrieve all projects  # noqa: E501
+    def find_metal_gateways_by_project_with_http_info(self, project_id : Annotated[StrictStr, Field(..., description="Project UUID")], include : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.")] = None, exclude : Annotated[Optional[conlist(StrictStr)], Field(description="Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.")] = None, page : Annotated[Optional[conint(strict=True, le=100000, ge=1)], Field(description="Page to return")] = None, per_page : Annotated[Optional[conint(strict=True, le=1000, ge=1)], Field(description="Items returned per page")] = None, **kwargs):  # noqa: E501
+        """Returns all metal gateways for a project  # noqa: E501
 
-        Returns a collection of projects that the current user is a member of.  # noqa: E501
+        Return all metal gateways for a project  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.find_projects_with_http_info(include, exclude, page, per_page, name, async_req=True)
+        >>> thread = api.find_metal_gateways_by_project_with_http_info(project_id, include, exclude, page, per_page, async_req=True)
         >>> result = thread.get()
 
+        :param project_id: Project UUID (required)
+        :type project_id: str
         :param include: Nested attributes to include. Included objects will return their full attributes. Attribute names can be dotted (up to 3 levels) to included deeply nested objects.
         :type include: List[str]
         :param exclude: Nested attributes to exclude. Excluded objects will return only the href attribute. Attribute names can be dotted (up to 3 levels) to exclude deeply nested objects.
         :type exclude: List[str]
         :param page: Page to return
         :type page: int
         :param per_page: Items returned per page
         :type per_page: int
-        :param name: Search by name substring
-        :type name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -719,25 +636,25 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ProjectList, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(MetalGatewayList, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'project_id',
             'include',
             'exclude',
             'page',
-            'per_page',
-            'name'
+            'per_page'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -748,23 +665,26 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method find_projects" % _key
+                    " to method find_metal_gateways_by_project" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['project_id']:
+            _path_params['project_id'] = _params['project_id']
+
 
         # process the query parameters
         _query_params = []
         if _params.get('include') is not None:  # noqa: E501
             _query_params.append(('include', _params['include']))
             _collection_formats['include'] = 'csv'
 
@@ -774,197 +694,36 @@
 
         if _params.get('page') is not None:  # noqa: E501
             _query_params.append(('page', _params['page']))
 
         if _params.get('per_page') is not None:  # noqa: E501
             _query_params.append(('per_page', _params['per_page']))
 
-        if _params.get('name') is not None:  # noqa: E501
-            _query_params.append(('name', _params['name']))
-
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-        # process the form parameters
-        _form_params = []
-        _files = {}
-        # process the body parameter
-        _body_params = None
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['application/json'])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ['x_auth_token']  # noqa: E501
-
-        _response_types_map = {
-            '200': "ProjectList",
-            '401': "Error",
-        }
-
-        return self.api_client.call_api(
-            '/projects', 'GET',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def update_project(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], project_update_input : Annotated[ProjectUpdateInput, Field(..., description="Project to update")], **kwargs) -> Project:  # noqa: E501
-        """Update the project  # noqa: E501
-
-        Updates the project.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.update_project(id, project_update_input, async_req=True)
-        >>> result = thread.get()
-
-        :param id: Project UUID (required)
-        :type id: str
-        :param project_update_input: Project to update (required)
-        :type project_update_input: ProjectUpdateInput
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: Project
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.update_project_with_http_info(id, project_update_input, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def update_project_with_http_info(self, id : Annotated[StrictStr, Field(..., description="Project UUID")], project_update_input : Annotated[ProjectUpdateInput, Field(..., description="Project to update")], **kwargs):  # noqa: E501
-        """Update the project  # noqa: E501
-
-        Updates the project.  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.update_project_with_http_info(id, project_update_input, async_req=True)
-        >>> result = thread.get()
-
-        :param id: Project UUID (required)
-        :type id: str
-        :param project_update_input: Project to update (required)
-        :type project_update_input: ProjectUpdateInput
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(Project, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = [
-            'id',
-            'project_update_input'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method update_project" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
-
-        # process the query parameters
-        _query_params = []
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
-        if _params['project_update_input']:
-            _body_params = _params['project_update_input']
-
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['x_auth_token']  # noqa: E501
 
         _response_types_map = {
-            '200': "Project",
+            '200': "MetalGatewayList",
             '401': "Error",
-            '403': "Error",
             '404': "Error",
-            '422': "Error",
         }
 
         return self.api_client.call_api(
-            '/projects/{id}', 'PUT',
+            '/projects/{project_id}/metal-gateways', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `equinix-metal-0.1.0/equinix_metal/api_client.py` & `equinix-metal-0.2.0/equinix_metal/api_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
@@ -72,15 +72,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'metal-python/0.1.0'
+        self.user_agent = 'metal-python/0.2.0'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `equinix-metal-0.1.0/equinix_metal/configuration.py` & `equinix-metal-0.2.0/equinix_metal/configuration.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
@@ -392,15 +392,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 0.1.0".\
+               "SDK Package Version: 0.2.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `equinix-metal-0.1.0/equinix_metal/models/device.py` & `equinix-metal-0.2.0/equinix_metal/models/ip_reservation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
@@ -17,79 +17,60 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist, validator
-from equinix_metal.models.device_actions_inner import DeviceActionsInner
-from equinix_metal.models.device_created_by import DeviceCreatedBy
-from equinix_metal.models.device_metro import DeviceMetro
-from equinix_metal.models.device_project import DeviceProject
-from equinix_metal.models.device_project_lite import DeviceProjectLite
-from equinix_metal.models.event import Event
-from equinix_metal.models.facility import Facility
+from pydantic import BaseModel, StrictBool, StrictInt, StrictStr, conlist, validator
 from equinix_metal.models.href import Href
-from equinix_metal.models.ip_assignment import IPAssignment
-from equinix_metal.models.operating_system import OperatingSystem
-from equinix_metal.models.plan import Plan
-from equinix_metal.models.port import Port
+from equinix_metal.models.ip_reservation_facility import IPReservationFacility
+from equinix_metal.models.ip_reservation_metro import IPReservationMetro
+from equinix_metal.models.metal_gateway_lite import MetalGatewayLite
+from equinix_metal.models.project import Project
 
-class Device(BaseModel):
+class IPReservation(BaseModel):
     """
-    Device
+    IPReservation
     """
-    actions: Optional[conlist(DeviceActionsInner)] = Field(None, description="Actions supported by the device instance.")
-    always_pxe: Optional[StrictBool] = None
-    billing_cycle: Optional[StrictStr] = None
-    bonding_mode: Optional[StrictInt] = None
+    addon: Optional[StrictBool] = None
+    address: Optional[StrictStr] = None
+    address_family: Optional[StrictInt] = None
+    assignments: Optional[conlist(Href)] = None
+    available: Optional[StrictStr] = None
+    bill: Optional[StrictBool] = None
+    cidr: Optional[StrictInt] = None
     created_at: Optional[datetime] = None
-    created_by: Optional[DeviceCreatedBy] = None
     customdata: Optional[Dict[str, Any]] = None
-    description: Optional[StrictStr] = None
-    facility: Optional[Facility] = None
-    hardware_reservation: Optional[Href] = None
-    hostname: Optional[StrictStr] = None
+    details: Optional[StrictStr] = None
+    enabled: Optional[StrictBool] = None
+    facility: Optional[IPReservationFacility] = None
+    gateway: Optional[StrictStr] = None
+    global_ip: Optional[StrictBool] = None
     href: Optional[StrictStr] = None
     id: Optional[StrictStr] = None
-    image_url: Optional[StrictStr] = None
-    ip_addresses: Optional[conlist(IPAssignment)] = None
-    ipxe_script_url: Optional[StrictStr] = None
-    iqn: Optional[StrictStr] = None
-    locked: Optional[StrictBool] = None
-    metro: Optional[DeviceMetro] = None
-    network_ports: Optional[conlist(Port)] = Field(None, description="By default, servers at Equinix Metal are configured in a “bonded” mode using LACP (Link Aggregation Control Protocol). Each 2-NIC server is configured with a single bond (namely bond0) with both interfaces eth0 and eth1 as members of the bond in a default Layer 3 mode. Some device plans may have a different number of ports and bonds available.")
-    operating_system: Optional[OperatingSystem] = None
-    plan: Optional[Plan] = None
-    project: Optional[DeviceProject] = None
-    project_lite: Optional[DeviceProjectLite] = None
-    provisioning_events: Optional[conlist(Event)] = None
-    provisioning_percentage: Optional[StrictFloat] = Field(None, description="Only visible while device provisioning")
-    root_password: Optional[StrictStr] = Field(None, description="Root password is automatically generated when server is provisioned and it is removed after 24 hours")
-    short_id: Optional[StrictStr] = None
-    spot_instance: Optional[StrictBool] = Field(None, description="Whether or not the device is a spot instance.")
-    spot_price_max: Optional[StrictFloat] = Field(None, description="The maximum price per hour you are willing to pay to keep this spot instance.  If you are outbid, the termination will be set allowing two minutes before shutdown.")
-    ssh_keys: Optional[conlist(Href)] = None
+    manageable: Optional[StrictBool] = None
+    management: Optional[StrictBool] = None
+    metal_gateway: Optional[MetalGatewayLite] = None
+    metro: Optional[IPReservationMetro] = None
+    netmask: Optional[StrictStr] = None
+    network: Optional[StrictStr] = None
+    project: Optional[Project] = None
+    project_lite: Optional[Href] = None
+    public: Optional[StrictBool] = None
+    requested_by: Optional[Href] = None
     state: Optional[StrictStr] = None
-    switch_uuid: Optional[StrictStr] = Field(None, description="Switch short id. This can be used to determine if two devices are connected to the same switch, for example.")
     tags: Optional[conlist(StrictStr)] = None
-    termination_time: Optional[datetime] = Field(None, description="When the device will be terminated. This is commonly set in advance for ephemeral spot market instances but this field may also be set with on-demand and reservation instances to automatically delete the resource at a given time. The termination time can also be used to release a hardware reservation instance at a given time, keeping the reservation open for other uses.  On a spot market device, the termination time will be set automatically when outbid.")
-    updated_at: Optional[datetime] = None
-    user: Optional[StrictStr] = None
-    userdata: Optional[StrictStr] = None
-    volumes: Optional[conlist(Href)] = None
-    __properties = ["actions", "always_pxe", "billing_cycle", "bonding_mode", "created_at", "created_by", "customdata", "description", "facility", "hardware_reservation", "hostname", "href", "id", "image_url", "ip_addresses", "ipxe_script_url", "iqn", "locked", "metro", "network_ports", "operating_system", "plan", "project", "project_lite", "provisioning_events", "provisioning_percentage", "root_password", "short_id", "spot_instance", "spot_price_max", "ssh_keys", "state", "switch_uuid", "tags", "termination_time", "updated_at", "user", "userdata", "volumes"]
-
-    @validator('state')
-    def state_validate_enum(cls, v):
-        if v is None:
-            return v
-        if v not in ('active', 'deleted', 'deprovisioning', 'failed', 'inactive', 'queued', 'reinstalling', 'post_provisioning', 'powering_on', 'powering_off', 'provisioning'):
-            raise ValueError("must be one of enum values ('active', 'deleted', 'deprovisioning', 'failed', 'inactive', 'queued', 'reinstalling', 'post_provisioning', 'powering_on', 'powering_off', 'provisioning')")
+    type: StrictStr = ...
+    __properties = ["addon", "address", "address_family", "assignments", "available", "bill", "cidr", "created_at", "customdata", "details", "enabled", "facility", "gateway", "global_ip", "href", "id", "manageable", "management", "metal_gateway", "metro", "netmask", "network", "project", "project_lite", "public", "requested_by", "state", "tags", "type"]
+
+    @validator('type')
+    def type_validate_enum(cls, v):
+        if v not in ('global_ipv4', 'public_ipv4', 'private_ipv4', 'public_ipv6'):
+            raise ValueError("must be one of enum values ('global_ipv4', 'public_ipv4', 'private_ipv4', 'public_ipv6')")
         return v
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -97,137 +78,86 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> Device:
-        """Create an instance of Device from a JSON string"""
+    def from_json(cls, json_str: str) -> IPReservation:
+        """Create an instance of IPReservation from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in actions (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in assignments (list)
         _items = []
-        if self.actions:
-            for _item in self.actions:
+        if self.assignments:
+            for _item in self.assignments:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['actions'] = _items
-        # override the default output from pydantic by calling `to_dict()` of created_by
-        if self.created_by:
-            _dict['created_by'] = self.created_by.to_dict()
+            _dict['assignments'] = _items
         # override the default output from pydantic by calling `to_dict()` of facility
         if self.facility:
             _dict['facility'] = self.facility.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of hardware_reservation
-        if self.hardware_reservation:
-            _dict['hardware_reservation'] = self.hardware_reservation.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in ip_addresses (list)
-        _items = []
-        if self.ip_addresses:
-            for _item in self.ip_addresses:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['ip_addresses'] = _items
+        # override the default output from pydantic by calling `to_dict()` of metal_gateway
+        if self.metal_gateway:
+            _dict['metal_gateway'] = self.metal_gateway.to_dict()
         # override the default output from pydantic by calling `to_dict()` of metro
         if self.metro:
             _dict['metro'] = self.metro.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in network_ports (list)
-        _items = []
-        if self.network_ports:
-            for _item in self.network_ports:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['network_ports'] = _items
-        # override the default output from pydantic by calling `to_dict()` of operating_system
-        if self.operating_system:
-            _dict['operating_system'] = self.operating_system.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of plan
-        if self.plan:
-            _dict['plan'] = self.plan.to_dict()
         # override the default output from pydantic by calling `to_dict()` of project
         if self.project:
             _dict['project'] = self.project.to_dict()
         # override the default output from pydantic by calling `to_dict()` of project_lite
         if self.project_lite:
             _dict['project_lite'] = self.project_lite.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in provisioning_events (list)
-        _items = []
-        if self.provisioning_events:
-            for _item in self.provisioning_events:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['provisioning_events'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in ssh_keys (list)
-        _items = []
-        if self.ssh_keys:
-            for _item in self.ssh_keys:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['ssh_keys'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in volumes (list)
-        _items = []
-        if self.volumes:
-            for _item in self.volumes:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['volumes'] = _items
+        # override the default output from pydantic by calling `to_dict()` of requested_by
+        if self.requested_by:
+            _dict['requested_by'] = self.requested_by.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Device:
-        """Create an instance of Device from a dict"""
+    def from_dict(cls, obj: dict) -> IPReservation:
+        """Create an instance of IPReservation from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return Device.parse_obj(obj)
+            return IPReservation.parse_obj(obj)
 
-        _obj = Device.parse_obj({
-            "actions": [DeviceActionsInner.from_dict(_item) for _item in obj.get("actions")] if obj.get("actions") is not None else None,
-            "always_pxe": obj.get("always_pxe"),
-            "billing_cycle": obj.get("billing_cycle"),
-            "bonding_mode": obj.get("bonding_mode"),
+        _obj = IPReservation.parse_obj({
+            "addon": obj.get("addon"),
+            "address": obj.get("address"),
+            "address_family": obj.get("address_family"),
+            "assignments": [Href.from_dict(_item) for _item in obj.get("assignments")] if obj.get("assignments") is not None else None,
+            "available": obj.get("available"),
+            "bill": obj.get("bill"),
+            "cidr": obj.get("cidr"),
             "created_at": obj.get("created_at"),
-            "created_by": DeviceCreatedBy.from_dict(obj.get("created_by")) if obj.get("created_by") is not None else None,
             "customdata": obj.get("customdata"),
-            "description": obj.get("description"),
-            "facility": Facility.from_dict(obj.get("facility")) if obj.get("facility") is not None else None,
-            "hardware_reservation": Href.from_dict(obj.get("hardware_reservation")) if obj.get("hardware_reservation") is not None else None,
-            "hostname": obj.get("hostname"),
+            "details": obj.get("details"),
+            "enabled": obj.get("enabled"),
+            "facility": IPReservationFacility.from_dict(obj.get("facility")) if obj.get("facility") is not None else None,
+            "gateway": obj.get("gateway"),
+            "global_ip": obj.get("global_ip"),
             "href": obj.get("href"),
             "id": obj.get("id"),
-            "image_url": obj.get("image_url"),
-            "ip_addresses": [IPAssignment.from_dict(_item) for _item in obj.get("ip_addresses")] if obj.get("ip_addresses") is not None else None,
-            "ipxe_script_url": obj.get("ipxe_script_url"),
-            "iqn": obj.get("iqn"),
-            "locked": obj.get("locked"),
-            "metro": DeviceMetro.from_dict(obj.get("metro")) if obj.get("metro") is not None else None,
-            "network_ports": [Port.from_dict(_item) for _item in obj.get("network_ports")] if obj.get("network_ports") is not None else None,
-            "operating_system": OperatingSystem.from_dict(obj.get("operating_system")) if obj.get("operating_system") is not None else None,
-            "plan": Plan.from_dict(obj.get("plan")) if obj.get("plan") is not None else None,
-            "project": DeviceProject.from_dict(obj.get("project")) if obj.get("project") is not None else None,
-            "project_lite": DeviceProjectLite.from_dict(obj.get("project_lite")) if obj.get("project_lite") is not None else None,
-            "provisioning_events": [Event.from_dict(_item) for _item in obj.get("provisioning_events")] if obj.get("provisioning_events") is not None else None,
-            "provisioning_percentage": obj.get("provisioning_percentage"),
-            "root_password": obj.get("root_password"),
-            "short_id": obj.get("short_id"),
-            "spot_instance": obj.get("spot_instance"),
-            "spot_price_max": obj.get("spot_price_max"),
-            "ssh_keys": [Href.from_dict(_item) for _item in obj.get("ssh_keys")] if obj.get("ssh_keys") is not None else None,
+            "manageable": obj.get("manageable"),
+            "management": obj.get("management"),
+            "metal_gateway": MetalGatewayLite.from_dict(obj.get("metal_gateway")) if obj.get("metal_gateway") is not None else None,
+            "metro": IPReservationMetro.from_dict(obj.get("metro")) if obj.get("metro") is not None else None,
+            "netmask": obj.get("netmask"),
+            "network": obj.get("network"),
+            "project": Project.from_dict(obj.get("project")) if obj.get("project") is not None else None,
+            "project_lite": Href.from_dict(obj.get("project_lite")) if obj.get("project_lite") is not None else None,
+            "public": obj.get("public"),
+            "requested_by": Href.from_dict(obj.get("requested_by")) if obj.get("requested_by") is not None else None,
             "state": obj.get("state"),
-            "switch_uuid": obj.get("switch_uuid"),
             "tags": obj.get("tags"),
-            "termination_time": obj.get("termination_time"),
-            "updated_at": obj.get("updated_at"),
-            "user": obj.get("user"),
-            "userdata": obj.get("userdata"),
-            "volumes": [Href.from_dict(_item) for _item in obj.get("volumes")] if obj.get("volumes") is not None else None
+            "type": obj.get("type")
         })
         return _obj
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `equinix-metal-0.1.0/equinix_metal/models/device_create_in_facility_input.py` & `equinix-metal-0.2.0/equinix_metal/models/device_create_input.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
@@ -18,32 +18,30 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist, validator
-from equinix_metal.models.device_create_input_ip_addresses_inner import DeviceCreateInputIpAddressesInner
-from equinix_metal.models.facility_input_facility import FacilityInputFacility
+from equinix_metal.models.ip_address import IPAddress
 from equinix_metal.models.ssh_key_input import SSHKeyInput
 
-class DeviceCreateInFacilityInput(BaseModel):
+class DeviceCreateInput(BaseModel):
     """
-    DeviceCreateInFacilityInput
+    DeviceCreateInput
     """
-    facility: FacilityInputFacility = ...
-    href: Optional[StrictStr] = None
     always_pxe: Optional[StrictBool] = Field(None, description="When true, devices with a `custom_ipxe` OS will always boot to iPXE. The default setting of false ensures that iPXE will be used on only the first boot.")
     billing_cycle: Optional[StrictStr] = Field(None, description="The billing cycle of the device.")
     customdata: Optional[Dict[str, Any]] = Field(None, description="Customdata is an arbitrary JSON value that can be accessed via the metadata service.")
     description: Optional[StrictStr] = Field(None, description="Any description of the device or how it will be used. This may be used to inform other API consumers with project access.")
     features: Optional[conlist(StrictStr)] = Field(None, description="The features attribute allows you to optionally specify what features your server should have.  In the API shorthand syntax, all features listed are `required`:  ``` { \"features\": [\"tpm\"] } ```  Alternatively, if you do not require a certain feature, but would prefer to be assigned a server with that feature if there are any available, you may specify that feature with a `preferred` value. The request will not fail if we have no servers with that feature in our inventory. The API offers an alternative syntax for mixing preferred and required features:  ``` { \"features\": { \"tpm\": \"required\", \"raid\": \"preferred\" } } ```  The request will only fail if there are no available servers matching the required `tpm` criteria.")
     hardware_reservation_id: Optional[StrictStr] = Field(None, description="The Hardware Reservation UUID to provision. Alternatively, `next-available` can be specified to select from any of the available hardware reservations. An error will be returned if the requested reservation option is not available.  See [Reserved Hardware](https://metal.equinix.com/developers/docs/deploy/reserved/) for more details.")
     hostname: Optional[StrictStr] = Field(None, description="The hostname to use within the operating system. The same hostname may be used on multiple devices within a project.")
-    ip_addresses: Optional[conlist(DeviceCreateInputIpAddressesInner)] = Field(None, description="The `ip_addresses attribute will allow you to specify the addresses you want created with your device.  The default value configures public IPv4, public IPv6, and private IPv4.  Private IPv4 address is required. When specifying `ip_addresses`, one of the array items must enable private IPv4.  Some operating systems require public IPv4 address. In those cases you will receive an error message if public IPv4 is not enabled.  For example, to only configure your server with a private IPv4 address, you can send `{ \"ip_addresses\": [{ \"address_family\": 4, \"public\": false }] }`.  It is possible to request a subnet size larger than a `/30` by assigning addresses using the UUID(s) of ip_reservations in your project.  For example, `{ \"ip_addresses\": [..., {\"address_family\": 4, \"public\": true, \"ip_reservations\": [\"uuid1\", \"uuid2\"]}] }`  To access a server without public IPs, you can use our Out-of-Band console access (SOS) or proxy through another server in the project with public IPs enabled.")
+    href: Optional[StrictStr] = None
+    ip_addresses: Optional[conlist(IPAddress)] = Field(None, description="The `ip_addresses attribute will allow you to specify the addresses you want created with your device.  The default value configures public IPv4, public IPv6, and private IPv4.  Private IPv4 address is required. When specifying `ip_addresses`, one of the array items must enable private IPv4.  Some operating systems require public IPv4 address. In those cases you will receive an error message if public IPv4 is not enabled.  For example, to only configure your server with a private IPv4 address, you can send `{ \"ip_addresses\": [{ \"address_family\": 4, \"public\": false }] }`.  It is possible to request a subnet size larger than a `/30` by assigning addresses using the UUID(s) of ip_reservations in your project.  For example, `{ \"ip_addresses\": [..., {\"address_family\": 4, \"public\": true, \"ip_reservations\": [\"uuid1\", \"uuid2\"]}] }`  To access a server without public IPs, you can use our Out-of-Band console access (SOS) or proxy through another server in the project with public IPs enabled.")
     ipxe_script_url: Optional[StrictStr] = Field(None, description="When set, the device will chainload an iPXE Script at boot fetched from the supplied URL.  See [Custom iPXE](https://metal.equinix.com/developers/docs/operating-systems/custom-ipxe/) for more details.")
     locked: Optional[StrictBool] = Field(False, description="Whether the device should be locked, preventing accidental deletion.")
     no_ssh_keys: Optional[StrictBool] = Field(False, description="Overrides default behaviour of attaching all of the organization members ssh keys and project ssh keys to device if no specific keys specified")
     operating_system: StrictStr = Field(..., description="The slug of the operating system to provision. Check the Equinix Metal operating system documentation for rules that may be imposed per operating system, including restrictions on IP address options and device plans.")
     plan: StrictStr = Field(..., description="The slug of the device plan to provision.")
     private_ipv4_subnet_size: Optional[StrictInt] = Field(28, description="Deprecated. Use ip_addresses. Subnet range for addresses allocated to this device.")
     project_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the device parent project that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
@@ -51,15 +49,15 @@
     spot_instance: Optional[StrictBool] = Field(None, description="Create a spot instance. Spot instances are created with a maximum bid price. If the bid price is not met, the spot instance will be terminated as indicated by the `termination_time` field.")
     spot_price_max: Optional[StrictFloat] = Field(None, description="The maximum amount to bid for a spot instance.")
     ssh_keys: Optional[conlist(SSHKeyInput)] = Field(None, description="A list of new or existing project ssh_keys that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  These keys are added in addition to any keys defined by   `project_ssh_keys` and `user_ssh_keys`. ")
     tags: Optional[conlist(StrictStr)] = None
     termination_time: Optional[datetime] = None
     user_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the users that should be authorized to access this device (typically via /root/.ssh/authorized_keys).  These keys will also appear in the device metadata.  The users must be members of the project or organization.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
     userdata: Optional[StrictStr] = Field(None, description="The userdata presented in the metadata service for this device.  Userdata is fetched and interpreted by the operating system installed on the device. Acceptable formats are determined by the operating system, with the exception of a special iPXE enabling syntax which is handled before the operating system starts.  See [Server User Data](https://metal.equinix.com/developers/docs/servers/user-data/) and [Provisioning with Custom iPXE](https://metal.equinix.com/developers/docs/operating-systems/custom-ipxe/#provisioning-with-custom-ipxe) for more details.")
-    __properties = ["facility", "href", "always_pxe", "billing_cycle", "customdata", "description", "features", "hardware_reservation_id", "hostname", "ip_addresses", "ipxe_script_url", "locked", "no_ssh_keys", "operating_system", "plan", "private_ipv4_subnet_size", "project_ssh_keys", "public_ipv4_subnet_size", "spot_instance", "spot_price_max", "ssh_keys", "tags", "termination_time", "user_ssh_keys", "userdata"]
+    __properties = ["always_pxe", "billing_cycle", "customdata", "description", "features", "hardware_reservation_id", "hostname", "href", "ip_addresses", "ipxe_script_url", "locked", "no_ssh_keys", "operating_system", "plan", "private_ipv4_subnet_size", "project_ssh_keys", "public_ipv4_subnet_size", "spot_instance", "spot_price_max", "ssh_keys", "tags", "termination_time", "user_ssh_keys", "userdata"]
 
     @validator('billing_cycle')
     def billing_cycle_validate_enum(cls, v):
         if v is None:
             return v
         if v not in ('hourly', 'daily', 'monthly', 'yearly'):
             raise ValueError("must be one of enum values ('hourly', 'daily', 'monthly', 'yearly')")
@@ -74,27 +72,24 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DeviceCreateInFacilityInput:
-        """Create an instance of DeviceCreateInFacilityInput from a JSON string"""
+    def from_json(cls, json_str: str) -> DeviceCreateInput:
+        """Create an instance of DeviceCreateInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of facility
-        if self.facility:
-            _dict['facility'] = self.facility.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in ip_addresses (list)
         _items = []
         if self.ip_addresses:
             for _item in self.ip_addresses:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['ip_addresses'] = _items
@@ -104,33 +99,32 @@
             for _item in self.ssh_keys:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['ssh_keys'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DeviceCreateInFacilityInput:
-        """Create an instance of DeviceCreateInFacilityInput from a dict"""
+    def from_dict(cls, obj: dict) -> DeviceCreateInput:
+        """Create an instance of DeviceCreateInput from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return DeviceCreateInFacilityInput.parse_obj(obj)
+            return DeviceCreateInput.parse_obj(obj)
 
-        _obj = DeviceCreateInFacilityInput.parse_obj({
-            "facility": FacilityInputFacility.from_dict(obj.get("facility")) if obj.get("facility") is not None else None,
-            "href": obj.get("href"),
+        _obj = DeviceCreateInput.parse_obj({
             "always_pxe": obj.get("always_pxe"),
             "billing_cycle": obj.get("billing_cycle"),
             "customdata": obj.get("customdata"),
             "description": obj.get("description"),
             "features": obj.get("features"),
             "hardware_reservation_id": obj.get("hardware_reservation_id"),
             "hostname": obj.get("hostname"),
-            "ip_addresses": [DeviceCreateInputIpAddressesInner.from_dict(_item) for _item in obj.get("ip_addresses")] if obj.get("ip_addresses") is not None else None,
+            "href": obj.get("href"),
+            "ip_addresses": [IPAddress.from_dict(_item) for _item in obj.get("ip_addresses")] if obj.get("ip_addresses") is not None else None,
             "ipxe_script_url": obj.get("ipxe_script_url"),
             "locked": obj.get("locked") if obj.get("locked") is not None else False,
             "no_ssh_keys": obj.get("no_ssh_keys") if obj.get("no_ssh_keys") is not None else False,
             "operating_system": obj.get("operating_system"),
             "plan": obj.get("plan"),
             "private_ipv4_subnet_size": obj.get("private_ipv4_subnet_size") if obj.get("private_ipv4_subnet_size") is not None else 28,
             "project_ssh_keys": obj.get("project_ssh_keys"),
```

### Comparing `equinix-metal-0.1.0/equinix_metal/models/device_create_in_metro_input.py` & `equinix-metal-0.2.0/equinix_metal/models/device_create_in_facility_input.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
@@ -18,31 +18,32 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist, validator
-from equinix_metal.models.device_create_input_ip_addresses_inner import DeviceCreateInputIpAddressesInner
+from equinix_metal.models.facility_input_facility import FacilityInputFacility
+from equinix_metal.models.ip_address import IPAddress
 from equinix_metal.models.ssh_key_input import SSHKeyInput
 
-class DeviceCreateInMetroInput(BaseModel):
+class DeviceCreateInFacilityInput(BaseModel):
     """
-    DeviceCreateInMetroInput
+    DeviceCreateInFacilityInput
     """
+    facility: FacilityInputFacility = ...
     href: Optional[StrictStr] = None
-    metro: StrictStr = Field(..., description="Metro code or ID of where the instance should be provisioned in. Either metro or facility must be provided.")
     always_pxe: Optional[StrictBool] = Field(None, description="When true, devices with a `custom_ipxe` OS will always boot to iPXE. The default setting of false ensures that iPXE will be used on only the first boot.")
     billing_cycle: Optional[StrictStr] = Field(None, description="The billing cycle of the device.")
     customdata: Optional[Dict[str, Any]] = Field(None, description="Customdata is an arbitrary JSON value that can be accessed via the metadata service.")
     description: Optional[StrictStr] = Field(None, description="Any description of the device or how it will be used. This may be used to inform other API consumers with project access.")
     features: Optional[conlist(StrictStr)] = Field(None, description="The features attribute allows you to optionally specify what features your server should have.  In the API shorthand syntax, all features listed are `required`:  ``` { \"features\": [\"tpm\"] } ```  Alternatively, if you do not require a certain feature, but would prefer to be assigned a server with that feature if there are any available, you may specify that feature with a `preferred` value. The request will not fail if we have no servers with that feature in our inventory. The API offers an alternative syntax for mixing preferred and required features:  ``` { \"features\": { \"tpm\": \"required\", \"raid\": \"preferred\" } } ```  The request will only fail if there are no available servers matching the required `tpm` criteria.")
     hardware_reservation_id: Optional[StrictStr] = Field(None, description="The Hardware Reservation UUID to provision. Alternatively, `next-available` can be specified to select from any of the available hardware reservations. An error will be returned if the requested reservation option is not available.  See [Reserved Hardware](https://metal.equinix.com/developers/docs/deploy/reserved/) for more details.")
     hostname: Optional[StrictStr] = Field(None, description="The hostname to use within the operating system. The same hostname may be used on multiple devices within a project.")
-    ip_addresses: Optional[conlist(DeviceCreateInputIpAddressesInner)] = Field(None, description="The `ip_addresses attribute will allow you to specify the addresses you want created with your device.  The default value configures public IPv4, public IPv6, and private IPv4.  Private IPv4 address is required. When specifying `ip_addresses`, one of the array items must enable private IPv4.  Some operating systems require public IPv4 address. In those cases you will receive an error message if public IPv4 is not enabled.  For example, to only configure your server with a private IPv4 address, you can send `{ \"ip_addresses\": [{ \"address_family\": 4, \"public\": false }] }`.  It is possible to request a subnet size larger than a `/30` by assigning addresses using the UUID(s) of ip_reservations in your project.  For example, `{ \"ip_addresses\": [..., {\"address_family\": 4, \"public\": true, \"ip_reservations\": [\"uuid1\", \"uuid2\"]}] }`  To access a server without public IPs, you can use our Out-of-Band console access (SOS) or proxy through another server in the project with public IPs enabled.")
+    ip_addresses: Optional[conlist(IPAddress)] = Field(None, description="The `ip_addresses attribute will allow you to specify the addresses you want created with your device.  The default value configures public IPv4, public IPv6, and private IPv4.  Private IPv4 address is required. When specifying `ip_addresses`, one of the array items must enable private IPv4.  Some operating systems require public IPv4 address. In those cases you will receive an error message if public IPv4 is not enabled.  For example, to only configure your server with a private IPv4 address, you can send `{ \"ip_addresses\": [{ \"address_family\": 4, \"public\": false }] }`.  It is possible to request a subnet size larger than a `/30` by assigning addresses using the UUID(s) of ip_reservations in your project.  For example, `{ \"ip_addresses\": [..., {\"address_family\": 4, \"public\": true, \"ip_reservations\": [\"uuid1\", \"uuid2\"]}] }`  To access a server without public IPs, you can use our Out-of-Band console access (SOS) or proxy through another server in the project with public IPs enabled.")
     ipxe_script_url: Optional[StrictStr] = Field(None, description="When set, the device will chainload an iPXE Script at boot fetched from the supplied URL.  See [Custom iPXE](https://metal.equinix.com/developers/docs/operating-systems/custom-ipxe/) for more details.")
     locked: Optional[StrictBool] = Field(False, description="Whether the device should be locked, preventing accidental deletion.")
     no_ssh_keys: Optional[StrictBool] = Field(False, description="Overrides default behaviour of attaching all of the organization members ssh keys and project ssh keys to device if no specific keys specified")
     operating_system: StrictStr = Field(..., description="The slug of the operating system to provision. Check the Equinix Metal operating system documentation for rules that may be imposed per operating system, including restrictions on IP address options and device plans.")
     plan: StrictStr = Field(..., description="The slug of the device plan to provision.")
     private_ipv4_subnet_size: Optional[StrictInt] = Field(28, description="Deprecated. Use ip_addresses. Subnet range for addresses allocated to this device.")
     project_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the device parent project that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
@@ -50,15 +51,15 @@
     spot_instance: Optional[StrictBool] = Field(None, description="Create a spot instance. Spot instances are created with a maximum bid price. If the bid price is not met, the spot instance will be terminated as indicated by the `termination_time` field.")
     spot_price_max: Optional[StrictFloat] = Field(None, description="The maximum amount to bid for a spot instance.")
     ssh_keys: Optional[conlist(SSHKeyInput)] = Field(None, description="A list of new or existing project ssh_keys that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  These keys are added in addition to any keys defined by   `project_ssh_keys` and `user_ssh_keys`. ")
     tags: Optional[conlist(StrictStr)] = None
     termination_time: Optional[datetime] = None
     user_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the users that should be authorized to access this device (typically via /root/.ssh/authorized_keys).  These keys will also appear in the device metadata.  The users must be members of the project or organization.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
     userdata: Optional[StrictStr] = Field(None, description="The userdata presented in the metadata service for this device.  Userdata is fetched and interpreted by the operating system installed on the device. Acceptable formats are determined by the operating system, with the exception of a special iPXE enabling syntax which is handled before the operating system starts.  See [Server User Data](https://metal.equinix.com/developers/docs/servers/user-data/) and [Provisioning with Custom iPXE](https://metal.equinix.com/developers/docs/operating-systems/custom-ipxe/#provisioning-with-custom-ipxe) for more details.")
-    __properties = ["href", "metro", "always_pxe", "billing_cycle", "customdata", "description", "features", "hardware_reservation_id", "hostname", "ip_addresses", "ipxe_script_url", "locked", "no_ssh_keys", "operating_system", "plan", "private_ipv4_subnet_size", "project_ssh_keys", "public_ipv4_subnet_size", "spot_instance", "spot_price_max", "ssh_keys", "tags", "termination_time", "user_ssh_keys", "userdata"]
+    __properties = ["facility", "href", "always_pxe", "billing_cycle", "customdata", "description", "features", "hardware_reservation_id", "hostname", "ip_addresses", "ipxe_script_url", "locked", "no_ssh_keys", "operating_system", "plan", "private_ipv4_subnet_size", "project_ssh_keys", "public_ipv4_subnet_size", "spot_instance", "spot_price_max", "ssh_keys", "tags", "termination_time", "user_ssh_keys", "userdata"]
 
     @validator('billing_cycle')
     def billing_cycle_validate_enum(cls, v):
         if v is None:
             return v
         if v not in ('hourly', 'daily', 'monthly', 'yearly'):
             raise ValueError("must be one of enum values ('hourly', 'daily', 'monthly', 'yearly')")
@@ -73,24 +74,27 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DeviceCreateInMetroInput:
-        """Create an instance of DeviceCreateInMetroInput from a JSON string"""
+    def from_json(cls, json_str: str) -> DeviceCreateInFacilityInput:
+        """Create an instance of DeviceCreateInFacilityInput from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
+        # override the default output from pydantic by calling `to_dict()` of facility
+        if self.facility:
+            _dict['facility'] = self.facility.to_dict()
         # override the default output from pydantic by calling `to_dict()` of each item in ip_addresses (list)
         _items = []
         if self.ip_addresses:
             for _item in self.ip_addresses:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['ip_addresses'] = _items
@@ -100,33 +104,33 @@
             for _item in self.ssh_keys:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['ssh_keys'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DeviceCreateInMetroInput:
-        """Create an instance of DeviceCreateInMetroInput from a dict"""
+    def from_dict(cls, obj: dict) -> DeviceCreateInFacilityInput:
+        """Create an instance of DeviceCreateInFacilityInput from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return DeviceCreateInMetroInput.parse_obj(obj)
+            return DeviceCreateInFacilityInput.parse_obj(obj)
 
-        _obj = DeviceCreateInMetroInput.parse_obj({
+        _obj = DeviceCreateInFacilityInput.parse_obj({
+            "facility": FacilityInputFacility.from_dict(obj.get("facility")) if obj.get("facility") is not None else None,
             "href": obj.get("href"),
-            "metro": obj.get("metro"),
             "always_pxe": obj.get("always_pxe"),
             "billing_cycle": obj.get("billing_cycle"),
             "customdata": obj.get("customdata"),
             "description": obj.get("description"),
             "features": obj.get("features"),
             "hardware_reservation_id": obj.get("hardware_reservation_id"),
             "hostname": obj.get("hostname"),
-            "ip_addresses": [DeviceCreateInputIpAddressesInner.from_dict(_item) for _item in obj.get("ip_addresses")] if obj.get("ip_addresses") is not None else None,
+            "ip_addresses": [IPAddress.from_dict(_item) for _item in obj.get("ip_addresses")] if obj.get("ip_addresses") is not None else None,
             "ipxe_script_url": obj.get("ipxe_script_url"),
             "locked": obj.get("locked") if obj.get("locked") is not None else False,
             "no_ssh_keys": obj.get("no_ssh_keys") if obj.get("no_ssh_keys") is not None else False,
             "operating_system": obj.get("operating_system"),
             "plan": obj.get("plan"),
             "private_ipv4_subnet_size": obj.get("private_ipv4_subnet_size") if obj.get("private_ipv4_subnet_size") is not None else 28,
             "project_ssh_keys": obj.get("project_ssh_keys"),
```

### Comparing `equinix-metal-0.1.0/equinix_metal/models/device_create_input.py` & `equinix-metal-0.2.0/equinix_metal/models/instances_batch_create_input_batches_inner.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
@@ -18,30 +18,34 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, conlist, validator
-from equinix_metal.models.device_create_input_ip_addresses_inner import DeviceCreateInputIpAddressesInner
+from equinix_metal.models.facility_input_facility import FacilityInputFacility
+from equinix_metal.models.ip_address import IPAddress
 from equinix_metal.models.ssh_key_input import SSHKeyInput
 
-class DeviceCreateInput(BaseModel):
+class InstancesBatchCreateInputBatchesInner(BaseModel):
     """
-    DeviceCreateInput
+    InstancesBatchCreateInputBatchesInner
     """
+    hostnames: Optional[conlist(StrictStr)] = None
+    href: Optional[StrictStr] = None
+    quantity: Optional[StrictInt] = Field(None, description="The number of devices to create in this batch. The hostname may contain an `{{index}}` placeholder, which will be replaced with the index of the device in the batch. For example, if the hostname is `device-{{index}}`, the first device in the batch will have the hostname `device-01`, the second device will have the hostname `device-02`, and so on.")
+    metro: StrictStr = Field(..., description="Metro code or ID of where the instance should be provisioned in. Either metro or facility must be provided.")
     always_pxe: Optional[StrictBool] = Field(None, description="When true, devices with a `custom_ipxe` OS will always boot to iPXE. The default setting of false ensures that iPXE will be used on only the first boot.")
     billing_cycle: Optional[StrictStr] = Field(None, description="The billing cycle of the device.")
     customdata: Optional[Dict[str, Any]] = Field(None, description="Customdata is an arbitrary JSON value that can be accessed via the metadata service.")
     description: Optional[StrictStr] = Field(None, description="Any description of the device or how it will be used. This may be used to inform other API consumers with project access.")
     features: Optional[conlist(StrictStr)] = Field(None, description="The features attribute allows you to optionally specify what features your server should have.  In the API shorthand syntax, all features listed are `required`:  ``` { \"features\": [\"tpm\"] } ```  Alternatively, if you do not require a certain feature, but would prefer to be assigned a server with that feature if there are any available, you may specify that feature with a `preferred` value. The request will not fail if we have no servers with that feature in our inventory. The API offers an alternative syntax for mixing preferred and required features:  ``` { \"features\": { \"tpm\": \"required\", \"raid\": \"preferred\" } } ```  The request will only fail if there are no available servers matching the required `tpm` criteria.")
     hardware_reservation_id: Optional[StrictStr] = Field(None, description="The Hardware Reservation UUID to provision. Alternatively, `next-available` can be specified to select from any of the available hardware reservations. An error will be returned if the requested reservation option is not available.  See [Reserved Hardware](https://metal.equinix.com/developers/docs/deploy/reserved/) for more details.")
     hostname: Optional[StrictStr] = Field(None, description="The hostname to use within the operating system. The same hostname may be used on multiple devices within a project.")
-    href: Optional[StrictStr] = None
-    ip_addresses: Optional[conlist(DeviceCreateInputIpAddressesInner)] = Field(None, description="The `ip_addresses attribute will allow you to specify the addresses you want created with your device.  The default value configures public IPv4, public IPv6, and private IPv4.  Private IPv4 address is required. When specifying `ip_addresses`, one of the array items must enable private IPv4.  Some operating systems require public IPv4 address. In those cases you will receive an error message if public IPv4 is not enabled.  For example, to only configure your server with a private IPv4 address, you can send `{ \"ip_addresses\": [{ \"address_family\": 4, \"public\": false }] }`.  It is possible to request a subnet size larger than a `/30` by assigning addresses using the UUID(s) of ip_reservations in your project.  For example, `{ \"ip_addresses\": [..., {\"address_family\": 4, \"public\": true, \"ip_reservations\": [\"uuid1\", \"uuid2\"]}] }`  To access a server without public IPs, you can use our Out-of-Band console access (SOS) or proxy through another server in the project with public IPs enabled.")
+    ip_addresses: Optional[conlist(IPAddress)] = Field(None, description="The `ip_addresses attribute will allow you to specify the addresses you want created with your device.  The default value configures public IPv4, public IPv6, and private IPv4.  Private IPv4 address is required. When specifying `ip_addresses`, one of the array items must enable private IPv4.  Some operating systems require public IPv4 address. In those cases you will receive an error message if public IPv4 is not enabled.  For example, to only configure your server with a private IPv4 address, you can send `{ \"ip_addresses\": [{ \"address_family\": 4, \"public\": false }] }`.  It is possible to request a subnet size larger than a `/30` by assigning addresses using the UUID(s) of ip_reservations in your project.  For example, `{ \"ip_addresses\": [..., {\"address_family\": 4, \"public\": true, \"ip_reservations\": [\"uuid1\", \"uuid2\"]}] }`  To access a server without public IPs, you can use our Out-of-Band console access (SOS) or proxy through another server in the project with public IPs enabled.")
     ipxe_script_url: Optional[StrictStr] = Field(None, description="When set, the device will chainload an iPXE Script at boot fetched from the supplied URL.  See [Custom iPXE](https://metal.equinix.com/developers/docs/operating-systems/custom-ipxe/) for more details.")
     locked: Optional[StrictBool] = Field(False, description="Whether the device should be locked, preventing accidental deletion.")
     no_ssh_keys: Optional[StrictBool] = Field(False, description="Overrides default behaviour of attaching all of the organization members ssh keys and project ssh keys to device if no specific keys specified")
     operating_system: StrictStr = Field(..., description="The slug of the operating system to provision. Check the Equinix Metal operating system documentation for rules that may be imposed per operating system, including restrictions on IP address options and device plans.")
     plan: StrictStr = Field(..., description="The slug of the device plan to provision.")
     private_ipv4_subnet_size: Optional[StrictInt] = Field(28, description="Deprecated. Use ip_addresses. Subnet range for addresses allocated to this device.")
     project_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the device parent project that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
@@ -49,15 +53,16 @@
     spot_instance: Optional[StrictBool] = Field(None, description="Create a spot instance. Spot instances are created with a maximum bid price. If the bid price is not met, the spot instance will be terminated as indicated by the `termination_time` field.")
     spot_price_max: Optional[StrictFloat] = Field(None, description="The maximum amount to bid for a spot instance.")
     ssh_keys: Optional[conlist(SSHKeyInput)] = Field(None, description="A list of new or existing project ssh_keys that should be authorized to access this device (typically via /root/.ssh/authorized_keys). These keys will also appear in the device metadata.  These keys are added in addition to any keys defined by   `project_ssh_keys` and `user_ssh_keys`. ")
     tags: Optional[conlist(StrictStr)] = None
     termination_time: Optional[datetime] = None
     user_ssh_keys: Optional[conlist(StrictStr)] = Field(None, description="A list of UUIDs identifying the users that should be authorized to access this device (typically via /root/.ssh/authorized_keys).  These keys will also appear in the device metadata.  The users must be members of the project or organization.  If no SSH keys are specified (`user_ssh_keys`, `project_ssh_keys`, and `ssh_keys` are all empty lists or omitted), all parent project keys, parent project members keys and organization members keys will be included. This behaviour can be changed with 'no_ssh_keys' option to omit any SSH key being added. ")
     userdata: Optional[StrictStr] = Field(None, description="The userdata presented in the metadata service for this device.  Userdata is fetched and interpreted by the operating system installed on the device. Acceptable formats are determined by the operating system, with the exception of a special iPXE enabling syntax which is handled before the operating system starts.  See [Server User Data](https://metal.equinix.com/developers/docs/servers/user-data/) and [Provisioning with Custom iPXE](https://metal.equinix.com/developers/docs/operating-systems/custom-ipxe/#provisioning-with-custom-ipxe) for more details.")
-    __properties = ["always_pxe", "billing_cycle", "customdata", "description", "features", "hardware_reservation_id", "hostname", "href", "ip_addresses", "ipxe_script_url", "locked", "no_ssh_keys", "operating_system", "plan", "private_ipv4_subnet_size", "project_ssh_keys", "public_ipv4_subnet_size", "spot_instance", "spot_price_max", "ssh_keys", "tags", "termination_time", "user_ssh_keys", "userdata"]
+    facility: FacilityInputFacility = ...
+    __properties = ["hostnames", "href", "quantity", "metro", "always_pxe", "billing_cycle", "customdata", "description", "features", "hardware_reservation_id", "hostname", "ip_addresses", "ipxe_script_url", "locked", "no_ssh_keys", "operating_system", "plan", "private_ipv4_subnet_size", "project_ssh_keys", "public_ipv4_subnet_size", "spot_instance", "spot_price_max", "ssh_keys", "tags", "termination_time", "user_ssh_keys", "userdata", "facility"]
 
     @validator('billing_cycle')
     def billing_cycle_validate_enum(cls, v):
         if v is None:
             return v
         if v not in ('hourly', 'daily', 'monthly', 'yearly'):
             raise ValueError("must be one of enum values ('hourly', 'daily', 'monthly', 'yearly')")
@@ -72,16 +77,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> DeviceCreateInput:
-        """Create an instance of DeviceCreateInput from a JSON string"""
+    def from_json(cls, json_str: str) -> InstancesBatchCreateInputBatchesInner:
+        """Create an instance of InstancesBatchCreateInputBatchesInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -96,46 +101,53 @@
         # override the default output from pydantic by calling `to_dict()` of each item in ssh_keys (list)
         _items = []
         if self.ssh_keys:
             for _item in self.ssh_keys:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['ssh_keys'] = _items
+        # override the default output from pydantic by calling `to_dict()` of facility
+        if self.facility:
+            _dict['facility'] = self.facility.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> DeviceCreateInput:
-        """Create an instance of DeviceCreateInput from a dict"""
+    def from_dict(cls, obj: dict) -> InstancesBatchCreateInputBatchesInner:
+        """Create an instance of InstancesBatchCreateInputBatchesInner from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return DeviceCreateInput.parse_obj(obj)
+            return InstancesBatchCreateInputBatchesInner.parse_obj(obj)
 
-        _obj = DeviceCreateInput.parse_obj({
+        _obj = InstancesBatchCreateInputBatchesInner.parse_obj({
+            "hostnames": obj.get("hostnames"),
+            "href": obj.get("href"),
+            "quantity": obj.get("quantity"),
+            "metro": obj.get("metro"),
             "always_pxe": obj.get("always_pxe"),
             "billing_cycle": obj.get("billing_cycle"),
             "customdata": obj.get("customdata"),
             "description": obj.get("description"),
             "features": obj.get("features"),
             "hardware_reservation_id": obj.get("hardware_reservation_id"),
             "hostname": obj.get("hostname"),
-            "href": obj.get("href"),
-            "ip_addresses": [DeviceCreateInputIpAddressesInner.from_dict(_item) for _item in obj.get("ip_addresses")] if obj.get("ip_addresses") is not None else None,
+            "ip_addresses": [IPAddress.from_dict(_item) for _item in obj.get("ip_addresses")] if obj.get("ip_addresses") is not None else None,
             "ipxe_script_url": obj.get("ipxe_script_url"),
             "locked": obj.get("locked") if obj.get("locked") is not None else False,
             "no_ssh_keys": obj.get("no_ssh_keys") if obj.get("no_ssh_keys") is not None else False,
             "operating_system": obj.get("operating_system"),
             "plan": obj.get("plan"),
             "private_ipv4_subnet_size": obj.get("private_ipv4_subnet_size") if obj.get("private_ipv4_subnet_size") is not None else 28,
             "project_ssh_keys": obj.get("project_ssh_keys"),
             "public_ipv4_subnet_size": obj.get("public_ipv4_subnet_size") if obj.get("public_ipv4_subnet_size") is not None else 31,
             "spot_instance": obj.get("spot_instance"),
             "spot_price_max": obj.get("spot_price_max"),
             "ssh_keys": [SSHKeyInput.from_dict(_item) for _item in obj.get("ssh_keys")] if obj.get("ssh_keys") is not None else None,
             "tags": obj.get("tags"),
             "termination_time": obj.get("termination_time"),
             "user_ssh_keys": obj.get("user_ssh_keys"),
-            "userdata": obj.get("userdata")
+            "userdata": obj.get("userdata"),
+            "facility": FacilityInputFacility.from_dict(obj.get("facility")) if obj.get("facility") is not None else None
         })
         return _obj
```

### Comparing `equinix-metal-0.1.0/pyproject.toml` & `equinix-metal-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "equinix_metal"
-version = "0.1.0"
+version = "0.2.0"
 description = "Metal API"
 authors = ["support@equinixmetal.com"]
 license = "Equinix Metal"
 readme = "README.md"
 repository = "https://github.com/metal-python/equinix-labs"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Metal API"]
```

### Comparing `equinix-metal-0.1.0/test/test_ip_reservation_list_ip_addresses_inner.py` & `equinix-metal-0.2.0/test/test_bgp_dynamic_neighbor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
@@ -15,306 +15,208 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.ip_reservation_list_ip_addresses_inner import IPReservationListIpAddressesInner  # noqa: E501
+from equinix_metal.models.bgp_dynamic_neighbor import BgpDynamicNeighbor  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestIPReservationListIpAddressesInner(unittest.TestCase):
-    """IPReservationListIpAddressesInner unit test stubs"""
+class TestBgpDynamicNeighbor(unittest.TestCase):
+    """BgpDynamicNeighbor unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test IPReservationListIpAddressesInner
+        """Test BgpDynamicNeighbor
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `IPReservationListIpAddressesInner`
+        # uncomment below to create an instance of `BgpDynamicNeighbor`
         """
-        model = equinix_metal.models.ip_reservation_list_ip_addresses_inner.IPReservationListIpAddressesInner()  # noqa: E501
+        model = equinix_metal.models.bgp_dynamic_neighbor.BgpDynamicNeighbor()  # noqa: E501
         if include_optional :
-            return IPReservationListIpAddressesInner(
-                addon = True, 
-                address = '', 
-                address_family = 56, 
-                assignments = [
-                    equinix_metal.models.href.Href(
-                        href = '', )
-                    ], 
-                available = '', 
-                bill = True, 
-                cidr = 56, 
+            return BgpDynamicNeighbor(
+                bgp_neighbor_asn = 12345, 
+                bgp_neighbor_range = '192.168.1.0/25', 
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                customdata = equinix_metal.models.customdata.customdata(), 
-                details = '', 
-                enabled = True, 
-                facility = None, 
-                gateway = '', 
-                global_ip = True, 
-                href = '', 
-                id = '', 
-                manageable = True, 
-                management = True, 
-                metal_gateway = equinix_metal.models.metal_gateway_lite.MetalGatewayLite(
+                created_by = equinix_metal.models.user_limited.UserLimited(
+                    avatar_thumb_url = '', 
+                    avatar_url = '', 
+                    full_name = '', 
+                    href = '', 
+                    id = '', ), 
+                href = '/bgp-dynamic-neighbors/aea82f16-57ec-412c-9523-b7f2b27635b2', 
+                id = 'aea82f16-57ec-412c-9523-b7f2b27635b2', 
+                metal_gateway = equinix_metal.models.vrf_metal_gateway.VrfMetalGateway(
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    gateway_address = '10.1.2.1/27', 
-                    href = '', 
-                    id = '', 
-                    state = 'ready', 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    vlan = 1001, ), 
-                metro = equinix_metal.models.metro.Metro(
-                    code = '', 
-                    country = '', 
-                    href = '', 
-                    id = '', 
-                    name = '', ), 
-                netmask = '', 
-                network = '', 
-                project = equinix_metal.models.project.Project(
-                    backend_transfer_enabled = True, 
-                    bgp_config = equinix_metal.models.href.Href(
+                    created_by = equinix_metal.models.href.Href(
                         href = '', ), 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    customdata = equinix_metal.models.customdata.customdata(), 
-                    devices = [
-                        equinix_metal.models.href.Href(
-                            href = '', )
-                        ], 
                     href = '', 
                     id = '', 
-                    invitations = [
-                        
-                        ], 
-                    max_devices = equinix_metal.models.max_devices.max_devices(), 
-                    members = [
-                        
-                        ], 
-                    memberships = [
-                        
-                        ], 
-                    name = '', 
-                    network_status = equinix_metal.models.network_status.network_status(), 
-                    organization = , 
-                    payment_method = , 
-                    ssh_keys = [
-                        
-                        ], 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    volumes = [
-                        
-                        ], ), 
-                project_lite = equinix_metal.models.project.Project(
-                    backend_transfer_enabled = True, 
-                    bgp_config = equinix_metal.models.href.Href(
-                        href = '', ), 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    customdata = equinix_metal.models.customdata.customdata(), 
-                    devices = [
-                        equinix_metal.models.href.Href(
-                            href = '', )
-                        ], 
-                    href = '', 
-                    id = '', 
-                    invitations = [
-                        
-                        ], 
-                    max_devices = equinix_metal.models.max_devices.max_devices(), 
-                    members = [
-                        
-                        ], 
-                    memberships = [
-                        
-                        ], 
-                    name = '', 
-                    network_status = equinix_metal.models.network_status.network_status(), 
-                    organization = , 
-                    payment_method = , 
-                    ssh_keys = [
-                        
-                        ], 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    volumes = [
-                        
-                        ], ), 
-                public = True, 
-                requested_by = equinix_metal.models.href.Href(
-                    href = '', ), 
-                state = '', 
-                tags = [
-                    ''
-                    ], 
-                type = 'vrf', 
-                created_by = equinix_metal.models.href.Href(
-                    href = '', ), 
-                vrf = equinix_metal.models.vrf.Vrf(
-                    bgp_dynamic_neighbors_enabled = True, 
-                    bgp_dynamic_neighbors_export_route_map = True, 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    created_by = equinix_metal.models.user.User(
-                        avatar_thumb_url = '', 
-                        avatar_url = '', 
+                    ip_reservation = equinix_metal.models.vrf_ip_reservation.VrfIpReservation(
+                        address = '', 
+                        address_family = 56, 
+                        bill = True, 
+                        cidr = 56, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
-                        email = '', 
-                        emails = [
-                            equinix_metal.models.href.Href(
-                                href = '', )
-                            ], 
-                        first_name = '', 
-                        fraud_score = '', 
-                        full_name = '', 
+                        details = '', 
+                        gateway = '', 
                         href = '', 
                         id = '', 
-                        last_login_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        last_name = '', 
-                        max_organizations = 56, 
-                        max_projects = 56, 
-                        phone_number = '', 
-                        short_id = '', 
-                        timezone = '', 
-                        two_factor_auth = '', 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), 
-                    description = '', 
-                    href = '', 
-                    id = '', 
-                    ip_ranges = [
-                        ''
-                        ], 
-                    local_asn = 56, 
-                    metro = equinix_metal.models.metro.Metro(
-                        code = '', 
-                        country = '', 
-                        href = '', 
-                        id = '', 
-                        name = '', ), 
-                    name = '', 
-                    project = equinix_metal.models.project.Project(
-                        backend_transfer_enabled = True, 
-                        bgp_config = equinix_metal.models.href.Href(
-                            href = '', ), 
+                        manageable = True, 
+                        management = True, 
+                        metal_gateway = equinix_metal.models.metal_gateway_lite.MetalGatewayLite(
+                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            gateway_address = '10.1.2.1/27', 
+                            href = '', 
+                            id = '', 
+                            state = 'ready', 
+                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            vlan = 1001, ), 
+                        metro = equinix_metal.models.metro.Metro(
+                            code = '', 
+                            country = '', 
+                            href = '', 
+                            id = '', 
+                            name = '', ), 
+                        netmask = '', 
+                        network = '', 
+                        project = equinix_metal.models.project.Project(
+                            backend_transfer_enabled = True, 
+                            bgp_config = equinix_metal.models.href.Href(
+                                href = '', ), 
+                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            customdata = equinix_metal.models.customdata.customdata(), 
+                            devices = [
+                                
+                                ], 
+                            href = '', 
+                            id = '', 
+                            invitations = [
+                                
+                                ], 
+                            max_devices = equinix_metal.models.max_devices.max_devices(), 
+                            members = [
+                                
+                                ], 
+                            memberships = [
+                                
+                                ], 
+                            name = '', 
+                            network_status = equinix_metal.models.network_status.network_status(), 
+                            organization = , 
+                            payment_method = , 
+                            ssh_keys = [
+                                
+                                ], 
+                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            volumes = [
+                                
+                                ], ), 
+                        project_lite = equinix_metal.models.project.Project(
+                            backend_transfer_enabled = True, 
+                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            customdata = equinix_metal.models.customdata.customdata(), 
+                            href = '', 
+                            id = '', 
+                            max_devices = equinix_metal.models.max_devices.max_devices(), 
+                            name = '', 
+                            network_status = equinix_metal.models.network_status.network_status(), 
+                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), 
+                        public = True, 
+                        state = '', 
+                        tags = [
+                            ''
+                            ], 
+                        type = 'vrf', 
+                        vrf = equinix_metal.models.vrf.Vrf(
+                            bgp_dynamic_neighbors_bfd_enabled = True, 
+                            bgp_dynamic_neighbors_enabled = True, 
+                            bgp_dynamic_neighbors_export_route_map = True, 
+                            bill = True, 
+                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            description = '', 
+                            href = '', 
+                            id = '', 
+                            ip_ranges = [
+                                ''
+                                ], 
+                            local_asn = 56, 
+                            name = '', 
+                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            virtual_circuits = [
+                                equinix_metal.models.vrf_virtual_circuit.VrfVirtualCircuit(
+                                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                    customer_ip = '12.0.0.2', 
+                                    description = '', 
+                                    href = '', 
+                                    id = '', 
+                                    md5 = '', 
+                                    metal_ip = '12.0.0.1', 
+                                    name = '', 
+                                    nni_vlan = 56, 
+                                    peer_asn = 56, 
+                                    port = , 
+                                    speed = 56, 
+                                    status = '', 
+                                    subnet = '12.0.0.0/30', 
+                                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                                ], ), ), 
+                    project = , 
+                    state = 'ready', 
+                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    virtual_network = equinix_metal.models.virtual_network.VirtualNetwork(
+                        assigned_to = , 
+                        assigned_to_virtual_circuit = True, 
+                        description = '', 
+                        facility = , 
+                        href = '', 
+                        id = '', 
+                        instances = [
+                            
+                            ], 
+                        metal_gateways = [
+                            equinix_metal.models.metal_gateway_lite.MetalGatewayLite(
+                                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                gateway_address = '10.1.2.1/27', 
+                                href = '', 
+                                id = '', 
+                                state = 'ready', 
+                                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                vlan = 1001, )
+                            ], 
+                        metro_code = '', 
+                        vxlan = 56, ), 
+                    vrf = equinix_metal.models.vrf.Vrf(
+                        bgp_dynamic_neighbors_bfd_enabled = True, 
+                        bgp_dynamic_neighbors_enabled = True, 
+                        bgp_dynamic_neighbors_export_route_map = True, 
+                        bill = True, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        customdata = equinix_metal.models.customdata.customdata(), 
-                        devices = [
-                            
-                            ], 
+                        description = '', 
                         href = '', 
                         id = '', 
-                        invitations = [
-                            
-                            ], 
-                        max_devices = equinix_metal.models.max_devices.max_devices(), 
-                        members = [
-                            
-                            ], 
-                        memberships = [
-                            
-                            ], 
+                        local_asn = 56, 
                         name = '', 
-                        network_status = equinix_metal.models.network_status.network_status(), 
-                        organization = , 
-                        payment_method = , 
-                        ssh_keys = [
-                            
-                            ], 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        volumes = [
-                            
-                            ], ), 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), ), 
+                state = 'active', 
+                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
             )
         else :
-            return IPReservationListIpAddressesInner(
-                type = 'vrf',
-                vrf = equinix_metal.models.vrf.Vrf(
-                    bgp_dynamic_neighbors_enabled = True, 
-                    bgp_dynamic_neighbors_export_route_map = True, 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    created_by = equinix_metal.models.user.User(
-                        avatar_thumb_url = '', 
-                        avatar_url = '', 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        customdata = equinix_metal.models.customdata.customdata(), 
-                        email = '', 
-                        emails = [
-                            equinix_metal.models.href.Href(
-                                href = '', )
-                            ], 
-                        first_name = '', 
-                        fraud_score = '', 
-                        full_name = '', 
-                        href = '', 
-                        id = '', 
-                        last_login_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        last_name = '', 
-                        max_organizations = 56, 
-                        max_projects = 56, 
-                        phone_number = '', 
-                        short_id = '', 
-                        timezone = '', 
-                        two_factor_auth = '', 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), 
-                    description = '', 
-                    href = '', 
-                    id = '', 
-                    ip_ranges = [
-                        ''
-                        ], 
-                    local_asn = 56, 
-                    metro = equinix_metal.models.metro.Metro(
-                        code = '', 
-                        country = '', 
-                        href = '', 
-                        id = '', 
-                        name = '', ), 
-                    name = '', 
-                    project = equinix_metal.models.project.Project(
-                        backend_transfer_enabled = True, 
-                        bgp_config = equinix_metal.models.href.Href(
-                            href = '', ), 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        customdata = equinix_metal.models.customdata.customdata(), 
-                        devices = [
-                            
-                            ], 
-                        href = '', 
-                        id = '', 
-                        invitations = [
-                            
-                            ], 
-                        max_devices = equinix_metal.models.max_devices.max_devices(), 
-                        members = [
-                            
-                            ], 
-                        memberships = [
-                            
-                            ], 
-                        name = '', 
-                        network_status = equinix_metal.models.network_status.network_status(), 
-                        organization = , 
-                        payment_method = , 
-                        ssh_keys = [
-                            
-                            ], 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        volumes = [
-                            
-                            ], ), 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ),
+            return BgpDynamicNeighbor(
         )
         """
 
-    def testIPReservationListIpAddressesInner(self):
-        """Test IPReservationListIpAddressesInner"""
+    def testBgpDynamicNeighbor(self):
+        """Test BgpDynamicNeighbor"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.1.0/test/test_request_ip_reservation201_response.py` & `equinix-metal-0.2.0/test/test_metal_gateway.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
@@ -15,191 +15,74 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.request_ip_reservation201_response import RequestIPReservation201Response  # noqa: E501
+from equinix_metal.models.metal_gateway import MetalGateway  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestRequestIPReservation201Response(unittest.TestCase):
-    """RequestIPReservation201Response unit test stubs"""
+class TestMetalGateway(unittest.TestCase):
+    """MetalGateway unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test RequestIPReservation201Response
+        """Test MetalGateway
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `RequestIPReservation201Response`
+        # uncomment below to create an instance of `MetalGateway`
         """
-        model = equinix_metal.models.request_ip_reservation201_response.RequestIPReservation201Response()  # noqa: E501
+        model = equinix_metal.models.metal_gateway.MetalGateway()  # noqa: E501
         if include_optional :
-            return RequestIPReservation201Response(
-                addon = True, 
-                address = '', 
-                address_family = 56, 
-                assignments = [
-                    equinix_metal.models.href.Href(
-                        href = '', )
-                    ], 
-                available = '', 
-                bill = True, 
-                cidr = 56, 
+            return MetalGateway(
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                customdata = equinix_metal.models.customdata.customdata(), 
-                details = '', 
-                enabled = True, 
-                facility = None, 
-                gateway = '', 
-                global_ip = True, 
+                created_by = equinix_metal.models.href.Href(
+                    href = '', ), 
                 href = '', 
                 id = '', 
-                manageable = True, 
-                management = True, 
-                metal_gateway = equinix_metal.models.metal_gateway_lite.MetalGatewayLite(
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    gateway_address = '10.1.2.1/27', 
-                    href = '', 
-                    id = '', 
-                    state = 'ready', 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    vlan = 1001, ), 
-                metro = equinix_metal.models.metro.Metro(
-                    code = '', 
-                    country = '', 
-                    href = '', 
-                    id = '', 
-                    name = '', ), 
-                netmask = '', 
-                network = '', 
-                project = equinix_metal.models.project.Project(
-                    backend_transfer_enabled = True, 
-                    bgp_config = equinix_metal.models.href.Href(
-                        href = '', ), 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    customdata = equinix_metal.models.customdata.customdata(), 
-                    devices = [
+                ip_reservation = equinix_metal.models.ip_reservation.IPReservation(
+                    addon = True, 
+                    address = '', 
+                    address_family = 56, 
+                    assignments = [
                         equinix_metal.models.href.Href(
                             href = '', )
                         ], 
-                    href = '', 
-                    id = '', 
-                    invitations = [
-                        
-                        ], 
-                    max_devices = equinix_metal.models.max_devices.max_devices(), 
-                    members = [
-                        
-                        ], 
-                    memberships = [
-                        
-                        ], 
-                    name = '', 
-                    network_status = equinix_metal.models.network_status.network_status(), 
-                    organization = , 
-                    payment_method = , 
-                    ssh_keys = [
-                        
-                        ], 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    volumes = [
-                        
-                        ], ), 
-                project_lite = equinix_metal.models.project.Project(
-                    backend_transfer_enabled = True, 
-                    bgp_config = equinix_metal.models.href.Href(
-                        href = '', ), 
+                    available = '', 
+                    bill = True, 
+                    cidr = 56, 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                     customdata = equinix_metal.models.customdata.customdata(), 
-                    devices = [
-                        equinix_metal.models.href.Href(
-                            href = '', )
-                        ], 
+                    details = '', 
+                    enabled = True, 
+                    facility = null, 
+                    gateway = '', 
+                    global_ip = True, 
                     href = '', 
                     id = '', 
-                    invitations = [
-                        
-                        ], 
-                    max_devices = equinix_metal.models.max_devices.max_devices(), 
-                    members = [
-                        
-                        ], 
-                    memberships = [
-                        
-                        ], 
-                    name = '', 
-                    network_status = equinix_metal.models.network_status.network_status(), 
-                    organization = , 
-                    payment_method = , 
-                    ssh_keys = [
-                        
-                        ], 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    volumes = [
-                        
-                        ], ), 
-                public = True, 
-                requested_by = equinix_metal.models.href.Href(
-                    href = '', ), 
-                state = '', 
-                tags = [
-                    ''
-                    ], 
-                type = 'vrf', 
-                created_by = equinix_metal.models.href.Href(
-                    href = '', ), 
-                vrf = equinix_metal.models.vrf.Vrf(
-                    bgp_dynamic_neighbors_enabled = True, 
-                    bgp_dynamic_neighbors_export_route_map = True, 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    created_by = equinix_metal.models.user.User(
-                        avatar_thumb_url = '', 
-                        avatar_url = '', 
+                    manageable = True, 
+                    management = True, 
+                    metal_gateway = equinix_metal.models.metal_gateway_lite.MetalGatewayLite(
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        customdata = equinix_metal.models.customdata.customdata(), 
-                        email = '', 
-                        emails = [
-                            equinix_metal.models.href.Href(
-                                href = '', )
-                            ], 
-                        first_name = '', 
-                        fraud_score = '', 
-                        full_name = '', 
+                        gateway_address = '10.1.2.1/27', 
                         href = '', 
                         id = '', 
-                        last_login_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        last_name = '', 
-                        max_organizations = 56, 
-                        max_projects = 56, 
-                        phone_number = '', 
-                        short_id = '', 
-                        timezone = '', 
-                        two_factor_auth = '', 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), 
-                    description = '', 
-                    href = '', 
-                    id = '', 
-                    ip_ranges = [
-                        ''
-                        ], 
-                    local_asn = 56, 
-                    metro = equinix_metal.models.metro.Metro(
-                        code = '', 
-                        country = '', 
-                        href = '', 
-                        id = '', 
-                        name = '', ), 
-                    name = '', 
+                        state = 'ready', 
+                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                        vlan = 1001, ), 
+                    metro = null, 
+                    netmask = '', 
+                    network = '', 
                     project = equinix_metal.models.project.Project(
                         backend_transfer_enabled = True, 
                         bgp_config = equinix_metal.models.href.Href(
                             href = '', ), 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
                         devices = [
@@ -224,97 +107,88 @@
                         ssh_keys = [
                             
                             ], 
                         updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         volumes = [
                             
                             ], ), 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
-            )
-        else :
-            return RequestIPReservation201Response(
-                type = 'vrf',
-                vrf = equinix_metal.models.vrf.Vrf(
-                    bgp_dynamic_neighbors_enabled = True, 
-                    bgp_dynamic_neighbors_export_route_map = True, 
+                    project_lite = , 
+                    public = True, 
+                    requested_by = , 
+                    state = '', 
+                    tags = [
+                        ''
+                        ], 
+                    type = 'global_ipv4', ), 
+                project = equinix_metal.models.project.Project(
+                    backend_transfer_enabled = True, 
+                    bgp_config = equinix_metal.models.href.Href(
+                        href = '', ), 
                     created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    created_by = equinix_metal.models.user.User(
-                        avatar_thumb_url = '', 
-                        avatar_url = '', 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        customdata = equinix_metal.models.customdata.customdata(), 
-                        email = '', 
-                        emails = [
-                            equinix_metal.models.href.Href(
-                                href = '', )
-                            ], 
-                        first_name = '', 
-                        fraud_score = '', 
-                        full_name = '', 
-                        href = '', 
-                        id = '', 
-                        last_login_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        last_name = '', 
-                        max_organizations = 56, 
-                        max_projects = 56, 
-                        phone_number = '', 
-                        short_id = '', 
-                        timezone = '', 
-                        two_factor_auth = '', 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), 
-                    description = '', 
+                    customdata = equinix_metal.models.customdata.customdata(), 
+                    devices = [
+                        equinix_metal.models.href.Href(
+                            href = '', )
+                        ], 
                     href = '', 
                     id = '', 
-                    ip_ranges = [
-                        ''
+                    invitations = [
+                        
+                        ], 
+                    max_devices = equinix_metal.models.max_devices.max_devices(), 
+                    members = [
+                        
+                        ], 
+                    memberships = [
+                        
                         ], 
-                    local_asn = 56, 
-                    metro = equinix_metal.models.metro.Metro(
-                        code = '', 
-                        country = '', 
-                        href = '', 
-                        id = '', 
-                        name = '', ), 
                     name = '', 
-                    project = equinix_metal.models.project.Project(
-                        backend_transfer_enabled = True, 
-                        bgp_config = equinix_metal.models.href.Href(
-                            href = '', ), 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        customdata = equinix_metal.models.customdata.customdata(), 
-                        devices = [
-                            
-                            ], 
-                        href = '', 
-                        id = '', 
-                        invitations = [
-                            
-                            ], 
-                        max_devices = equinix_metal.models.max_devices.max_devices(), 
-                        members = [
-                            
-                            ], 
-                        memberships = [
-                            
-                            ], 
-                        name = '', 
-                        network_status = equinix_metal.models.network_status.network_status(), 
-                        organization = , 
-                        payment_method = , 
-                        ssh_keys = [
-                            
-                            ], 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        volumes = [
-                            
-                            ], ), 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ),
+                    network_status = equinix_metal.models.network_status.network_status(), 
+                    organization = , 
+                    payment_method = , 
+                    ssh_keys = [
+                        
+                        ], 
+                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                    volumes = [
+                        
+                        ], ), 
+                state = 'ready', 
+                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                virtual_network = equinix_metal.models.virtual_network.VirtualNetwork(
+                    assigned_to = equinix_metal.models.href.Href(
+                        href = '', ), 
+                    assigned_to_virtual_circuit = True, 
+                    description = '', 
+                    facility = equinix_metal.models.href.Href(
+                        href = '', ), 
+                    href = '', 
+                    id = '', 
+                    instances = [
+                        
+                        ], 
+                    metal_gateways = [
+                        equinix_metal.models.metal_gateway_lite.MetalGatewayLite(
+                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            gateway_address = '10.1.2.1/27', 
+                            href = '', 
+                            id = '', 
+                            state = 'ready', 
+                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            vlan = 1001, )
+                        ], 
+                    metro = , 
+                    metro_code = '', 
+                    vxlan = 56, )
+            )
+        else :
+            return MetalGateway(
         )
         """
 
-    def testRequestIPReservation201Response(self):
-        """Test RequestIPReservation201Response"""
+    def testMetalGateway(self):
+        """Test MetalGateway"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `equinix-metal-0.1.0/test/test_vrf_ip_reservation.py` & `equinix-metal-0.2.0/test/test_vrf_ip_reservation_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Metal API
 
-    desc  # noqa: E501
+    # Introduction Equinix Metal provides a RESTful HTTP API which can be reached at <https://api.equinix.com/metal/v1>. This document describes the API and how to use it.  The API allows you to programmatically interact with all of your Equinix Metal resources, including devices, networks, addresses, organizations, projects, and your user account. Every feature of the Equinix Metal web interface is accessible through the API.  The API docs are generated from the Equinix Metal OpenAPI specification and are officially hosted at <https://metal.equinix.com/developers/api>.  # Common Parameters  The Equinix Metal API uses a few methods to minimize network traffic and improve throughput. These parameters are not used in all API calls, but are used often enough to warrant their own section. Look for these parameters in the documentation for the API calls that support them.  ## Pagination  Pagination is used to limit the number of results returned in a single request. The API will return a maximum of 100 results per page. To retrieve additional results, you can use the `page` and `per_page` query parameters.  The `page` parameter is used to specify the page number. The first page is `1`. The `per_page` parameter is used to specify the number of results per page. The maximum number of results differs by resource type.  ## Sorting  Where offered, the API allows you to sort results by a specific field. To sort results use the `sort_by` query parameter with the root level field name as the value. The `sort_direction` parameter is used to specify the sort direction, either either `asc` (ascending) or `desc` (descending).  ## Filtering  Filtering is used to limit the results returned in a single request. The API supports filtering by certain fields in the response. To filter results, you can use the field as a query parameter.  For example, to filter the IP list to only return public IPv4 addresses, you can filter by the `type` field, as in the following request:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/projects/id/ips?type=public_ipv4 ```  Only IP addresses with the `type` field set to `public_ipv4` will be returned.  ## Searching  Searching is used to find matching resources using multiple field comparissons. The API supports searching in resources that define this behavior. The fields available for search differ by resource, as does the search strategy.  To search resources you can use the `search` query parameter.  ## Include and Exclude  For resources that contain references to other resources, sucha as a Device that refers to the Project it resides in, the Equinix Metal API will returns `href` values (API links) to the associated resource.  ```json {   ...   \"project\": {     \"href\": \"/metal/v1/projects/f3f131c8-f302-49ef-8c44-9405022dc6dd\"   } } ```  If you're going need the project details, you can avoid a second API request.  Specify the contained `href` resources and collections that you'd like to have included in the response using the `include` query parameter.  For example:  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=projects ```  The `include` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests where `href` resources are presented.  To have multiple resources include, use a comma-separated list (e.g. `?include=emails,projects,memberships`).  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=emails,projects,memberships ```  You may also include nested associations up to three levels deep using dot notation (`?include=memberships.projects`):  ```sh curl -H 'X-Auth-Token: my_authentication_token' \\   https://api.equinix.com/metal/v1/user?include=memberships.projects ```  To exclude resources, and optimize response delivery, use the `exclude` query parameter. The `exclude` parameter is generally accepted in `GET`, `POST`, `PUT`, and `PATCH` requests for fields with nested object responses. When excluded, these fields will be replaced with an object that contains only an `href` field.   # noqa: E501
 
     The version of the OpenAPI document: 1.0.0
     Contact: support@equinixmetal.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
@@ -15,295 +15,157 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import equinix_metal
-from equinix_metal.models.vrf_ip_reservation import VrfIpReservation  # noqa: E501
+from equinix_metal.models.vrf_ip_reservation_list import VrfIpReservationList  # noqa: E501
 from equinix_metal.rest import ApiException
 
-class TestVrfIpReservation(unittest.TestCase):
-    """VrfIpReservation unit test stubs"""
+class TestVrfIpReservationList(unittest.TestCase):
+    """VrfIpReservationList unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test VrfIpReservation
+        """Test VrfIpReservationList
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `VrfIpReservation`
+        # uncomment below to create an instance of `VrfIpReservationList`
         """
-        model = equinix_metal.models.vrf_ip_reservation.VrfIpReservation()  # noqa: E501
+        model = equinix_metal.models.vrf_ip_reservation_list.VrfIpReservationList()  # noqa: E501
         if include_optional :
-            return VrfIpReservation(
-                address = '', 
-                address_family = 56, 
-                bill = True, 
-                cidr = 56, 
-                created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                created_by = equinix_metal.models.href.Href(
-                    href = '', ), 
-                customdata = equinix_metal.models.customdata.customdata(), 
-                details = '', 
-                gateway = '', 
+            return VrfIpReservationList(
                 href = '', 
-                id = '', 
-                manageable = True, 
-                management = True, 
-                metal_gateway = equinix_metal.models.metal_gateway_lite.MetalGatewayLite(
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    gateway_address = '10.1.2.1/27', 
-                    href = '', 
-                    id = '', 
-                    state = 'ready', 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    vlan = 1001, ), 
-                metro = equinix_metal.models.metro.Metro(
-                    code = '', 
-                    country = '', 
-                    href = '', 
-                    id = '', 
-                    name = '', ), 
-                netmask = '', 
-                network = '', 
-                project = equinix_metal.models.project.Project(
-                    backend_transfer_enabled = True, 
-                    bgp_config = equinix_metal.models.href.Href(
-                        href = '', ), 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    customdata = equinix_metal.models.customdata.customdata(), 
-                    devices = [
-                        equinix_metal.models.href.Href(
-                            href = '', )
-                        ], 
-                    href = '', 
-                    id = '', 
-                    invitations = [
-                        
-                        ], 
-                    max_devices = equinix_metal.models.max_devices.max_devices(), 
-                    members = [
-                        
-                        ], 
-                    memberships = [
-                        
-                        ], 
-                    name = '', 
-                    network_status = equinix_metal.models.network_status.network_status(), 
-                    organization = , 
-                    payment_method = , 
-                    ssh_keys = [
-                        
-                        ], 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    volumes = [
-                        
-                        ], ), 
-                project_lite = equinix_metal.models.project.Project(
-                    backend_transfer_enabled = True, 
-                    bgp_config = equinix_metal.models.href.Href(
-                        href = '', ), 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    customdata = equinix_metal.models.customdata.customdata(), 
-                    devices = [
-                        equinix_metal.models.href.Href(
-                            href = '', )
-                        ], 
-                    href = '', 
-                    id = '', 
-                    invitations = [
-                        
-                        ], 
-                    max_devices = equinix_metal.models.max_devices.max_devices(), 
-                    members = [
-                        
-                        ], 
-                    memberships = [
-                        
-                        ], 
-                    name = '', 
-                    network_status = equinix_metal.models.network_status.network_status(), 
-                    organization = , 
-                    payment_method = , 
-                    ssh_keys = [
-                        
-                        ], 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    volumes = [
-                        
-                        ], ), 
-                public = True, 
-                state = '', 
-                tags = [
-                    ''
-                    ], 
-                type = 'vrf', 
-                vrf = equinix_metal.models.vrf.Vrf(
-                    bgp_dynamic_neighbors_enabled = True, 
-                    bgp_dynamic_neighbors_export_route_map = True, 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    created_by = equinix_metal.models.user.User(
-                        avatar_thumb_url = '', 
-                        avatar_url = '', 
+                ip_addresses = [
+                    equinix_metal.models.vrf_ip_reservation.VrfIpReservation(
+                        address = '', 
+                        address_family = 56, 
+                        bill = True, 
+                        cidr = 56, 
                         created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        customdata = equinix_metal.models.customdata.customdata(), 
-                        email = '', 
-                        emails = [
-                            equinix_metal.models.href.Href(
-                                href = '', )
-                            ], 
-                        first_name = '', 
-                        fraud_score = '', 
-                        full_name = '', 
-                        href = '', 
-                        id = '', 
-                        last_login_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        last_name = '', 
-                        max_organizations = 56, 
-                        max_projects = 56, 
-                        phone_number = '', 
-                        short_id = '', 
-                        timezone = '', 
-                        two_factor_auth = '', 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), 
-                    description = '', 
-                    href = '', 
-                    id = '', 
-                    ip_ranges = [
-                        ''
-                        ], 
-                    local_asn = 56, 
-                    metro = equinix_metal.models.metro.Metro(
-                        code = '', 
-                        country = '', 
-                        href = '', 
-                        id = '', 
-                        name = '', ), 
-                    name = '', 
-                    project = equinix_metal.models.project.Project(
-                        backend_transfer_enabled = True, 
-                        bgp_config = equinix_metal.models.href.Href(
+                        created_by = equinix_metal.models.href.Href(
                             href = '', ), 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
                         customdata = equinix_metal.models.customdata.customdata(), 
-                        devices = [
-                            
-                            ], 
+                        details = '', 
+                        gateway = '', 
                         href = '', 
                         id = '', 
-                        invitations = [
-                            
-                            ], 
-                        max_devices = equinix_metal.models.max_devices.max_devices(), 
-                        members = [
-                            
-                            ], 
-                        memberships = [
-                            
-                            ], 
-                        name = '', 
-                        network_status = equinix_metal.models.network_status.network_status(), 
-                        organization = , 
-                        payment_method = , 
-                        ssh_keys = [
-                            
-                            ], 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        volumes = [
-                            
-                            ], ), 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                        manageable = True, 
+                        management = True, 
+                        metal_gateway = equinix_metal.models.metal_gateway_lite.MetalGatewayLite(
+                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            gateway_address = '10.1.2.1/27', 
+                            href = '', 
+                            id = '', 
+                            state = 'ready', 
+                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            vlan = 1001, ), 
+                        metro = equinix_metal.models.metro.Metro(
+                            code = '', 
+                            country = '', 
+                            href = '', 
+                            id = '', 
+                            name = '', ), 
+                        netmask = '', 
+                        network = '', 
+                        project = equinix_metal.models.project.Project(
+                            backend_transfer_enabled = True, 
+                            bgp_config = equinix_metal.models.href.Href(
+                                href = '', ), 
+                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            customdata = equinix_metal.models.customdata.customdata(), 
+                            devices = [
+                                
+                                ], 
+                            href = '', 
+                            id = '', 
+                            invitations = [
+                                
+                                ], 
+                            max_devices = equinix_metal.models.max_devices.max_devices(), 
+                            members = [
+                                
+                                ], 
+                            memberships = [
+                                
+                                ], 
+                            name = '', 
+                            network_status = equinix_metal.models.network_status.network_status(), 
+                            organization = , 
+                            payment_method = , 
+                            ssh_keys = [
+                                
+                                ], 
+                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            volumes = [
+                                
+                                ], ), 
+                        project_lite = equinix_metal.models.project.Project(
+                            backend_transfer_enabled = True, 
+                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            customdata = equinix_metal.models.customdata.customdata(), 
+                            href = '', 
+                            id = '', 
+                            max_devices = equinix_metal.models.max_devices.max_devices(), 
+                            name = '', 
+                            network_status = equinix_metal.models.network_status.network_status(), 
+                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), 
+                        public = True, 
+                        state = '', 
+                        tags = [
+                            ''
+                            ], 
+                        type = 'vrf', 
+                        vrf = equinix_metal.models.vrf.Vrf(
+                            bgp_dynamic_neighbors_bfd_enabled = True, 
+                            bgp_dynamic_neighbors_enabled = True, 
+                            bgp_dynamic_neighbors_export_route_map = True, 
+                            bill = True, 
+                            created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            description = '', 
+                            href = '', 
+                            id = '', 
+                            ip_ranges = [
+                                ''
+                                ], 
+                            local_asn = 56, 
+                            name = '', 
+                            updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                            virtual_circuits = [
+                                equinix_metal.models.vrf_virtual_circuit.VrfVirtualCircuit(
+                                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
+                                    customer_ip = '12.0.0.2', 
+                                    description = '', 
+                                    href = '', 
+                                    id = '', 
+                                    md5 = '', 
+                                    metal_ip = '12.0.0.1', 
+                                    name = '', 
+                                    nni_vlan = 56, 
+                                    peer_asn = 56, 
+                                    port = , 
+                                    speed = 56, 
+                                    status = '', 
+                                    subnet = '12.0.0.0/30', 
+                                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), )
+                                ], ), )
+                    ]
             )
         else :
-            return VrfIpReservation(
-                type = 'vrf',
-                vrf = equinix_metal.models.vrf.Vrf(
-                    bgp_dynamic_neighbors_enabled = True, 
-                    bgp_dynamic_neighbors_export_route_map = True, 
-                    created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                    created_by = equinix_metal.models.user.User(
-                        avatar_thumb_url = '', 
-                        avatar_url = '', 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        customdata = equinix_metal.models.customdata.customdata(), 
-                        email = '', 
-                        emails = [
-                            equinix_metal.models.href.Href(
-                                href = '', )
-                            ], 
-                        first_name = '', 
-                        fraud_score = '', 
-                        full_name = '', 
-                        href = '', 
-                        id = '', 
-                        last_login_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        last_name = '', 
-                        max_organizations = 56, 
-                        max_projects = 56, 
-                        phone_number = '', 
-                        short_id = '', 
-                        timezone = '', 
-                        two_factor_auth = '', 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ), 
-                    description = '', 
-                    href = '', 
-                    id = '', 
-                    ip_ranges = [
-                        ''
-                        ], 
-                    local_asn = 56, 
-                    metro = equinix_metal.models.metro.Metro(
-                        code = '', 
-                        country = '', 
-                        href = '', 
-                        id = '', 
-                        name = '', ), 
-                    name = '', 
-                    project = equinix_metal.models.project.Project(
-                        backend_transfer_enabled = True, 
-                        bgp_config = equinix_metal.models.href.Href(
-                            href = '', ), 
-                        created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        customdata = equinix_metal.models.customdata.customdata(), 
-                        devices = [
-                            
-                            ], 
-                        href = '', 
-                        id = '', 
-                        invitations = [
-                            
-                            ], 
-                        max_devices = equinix_metal.models.max_devices.max_devices(), 
-                        members = [
-                            
-                            ], 
-                        memberships = [
-                            
-                            ], 
-                        name = '', 
-                        network_status = equinix_metal.models.network_status.network_status(), 
-                        organization = , 
-                        payment_method = , 
-                        ssh_keys = [
-                            
-                            ], 
-                        updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), 
-                        volumes = [
-                            
-                            ], ), 
-                    updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'), ),
+            return VrfIpReservationList(
         )
         """
 
-    def testVrfIpReservation(self):
-        """Test VrfIpReservation"""
+    def testVrfIpReservationList(self):
+        """Test VrfIpReservationList"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

