# Comparing `tmp/IP2Trace-3.1.3.tar.gz` & `tmp/IP2Trace-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IP2Trace-3.1.3.tar", last modified: Fri Jul  1 08:14:46 2022, max compression
+gzip compressed data, was "IP2Trace-3.2.0.tar", last modified: Tue May  9 07:32:46 2023, max compression
```

## Comparing `IP2Trace-3.1.3.tar` & `IP2Trace-3.2.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-07-01 08:14:46.648204 IP2Trace-3.1.3/
-drwxrwxrwx   0        0        0        0 2022-07-01 08:14:46.632821 IP2Trace-3.1.3/IP2Trace.egg-info/
--rw-rw-rw-   0        0        0     6144 2022-07-01 08:14:46.000000 IP2Trace-3.1.3/IP2Trace.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2022-07-01 08:14:46.000000 IP2Trace-3.1.3/IP2Trace.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-01 08:14:46.000000 IP2Trace-3.1.3/IP2Trace.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2022-07-01 08:14:46.000000 IP2Trace-3.1.3/IP2Trace.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2022-07-01 08:14:46.000000 IP2Trace-3.1.3/IP2Trace.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-07-01 08:14:46.000000 IP2Trace-3.1.3/IP2Trace.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1093 2022-07-01 07:44:03.000000 IP2Trace-3.1.3/LICENSE.TXT
--rw-rw-rw-   0        0        0       61 2021-12-08 05:35:04.000000 IP2Trace-3.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     6144 2022-07-01 08:14:46.648204 IP2Trace-3.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-07-01 08:14:46.633854 IP2Trace-3.1.3/data/
--rw-rw-rw-   0        0        0  5391050 2021-12-08 05:35:04.000000 IP2Trace-3.1.3/data/IP2LOCATION-LITE-DB1.IPV6.BIN
--rw-rw-rw-   0        0        0    22826 2022-07-01 06:45:12.000000 IP2Trace-3.1.3/ip2trace - Copy.py
--rw-rw-rw-   0        0        0    21781 2022-07-01 07:43:50.000000 IP2Trace-3.1.3/ip2trace.py
--rw-rw-rw-   0        0        0     5066 2022-07-01 07:55:43.000000 IP2Trace-3.1.3/readme.md
--rw-rw-rw-   0        0        0       42 2022-07-01 08:14:46.649187 IP2Trace-3.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1564 2022-07-01 01:39:57.000000 IP2Trace-3.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-09 07:32:46.160743 IP2Trace-3.2.0/
+drwxrwxrwx   0        0        0        0 2023-05-09 07:32:46.140742 IP2Trace-3.2.0/IP2Trace.egg-info/
+-rw-rw-rw-   0        0        0     6265 2023-05-09 07:32:46.000000 IP2Trace-3.2.0/IP2Trace.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-05-09 07:32:46.000000 IP2Trace-3.2.0/IP2Trace.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-09 07:32:46.000000 IP2Trace-3.2.0/IP2Trace.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-09 07:32:46.000000 IP2Trace-3.2.0/IP2Trace.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2023-05-09 07:32:46.000000 IP2Trace-3.2.0/IP2Trace.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-09 07:32:46.000000 IP2Trace-3.2.0/IP2Trace.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1093 2023-05-09 07:00:20.000000 IP2Trace-3.2.0/LICENSE.TXT
+-rw-rw-rw-   0        0        0       61 2021-12-08 05:35:04.000000 IP2Trace-3.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6265 2023-05-09 07:32:46.159762 IP2Trace-3.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-09 07:32:46.147747 IP2Trace-3.2.0/data/
+-rw-rw-rw-   0        0        0  5391050 2021-12-08 05:35:04.000000 IP2Trace-3.2.0/data/IP2LOCATION-LITE-DB1.IPV6.BIN
+-rw-rw-rw-   0        0        0    21903 2023-05-09 05:52:00.000000 IP2Trace-3.2.0/ip2trace.py
+-rw-rw-rw-   0        0        0     5187 2023-05-09 06:48:43.000000 IP2Trace-3.2.0/readme.md
+-rw-rw-rw-   0        0        0       42 2023-05-09 07:32:46.160743 IP2Trace-3.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1564 2023-05-09 05:25:09.000000 IP2Trace-3.2.0/setup.py
```

### Comparing `IP2Trace-3.1.3/IP2Trace.egg-info/PKG-INFO` & `IP2Trace-3.2.0/IP2Trace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IP2Trace
-Version: 3.1.3
+Version: 3.2.0
 Summary: A Python tool to display geolocation information in the traceroute.
 Home-page: https://github.com/ip2location/ip2trace-python
 Author: IP2Location
 Author-email: support@ip2location.com
 License: MIT
 Project-URL: Official Website, https://www.ip2location.com
 Keywords: IP2Location Geolocation
@@ -22,15 +22,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 
 # IP2Trace Python
 
-IP2Trace Python is a Python tool allowing user to get IP address information such as country, region, city, latitude, longitude, zip code, time zone, ISP, domain name, connection type, area code, weather, mobile network, elevation, usage type from traceroute probes IP address.
+IP2Trace Python is a Python tool allowing user to get IP address information such as country, region, city, latitude, longitude, zip code, time zone, ISP, domain name, connection type, area code, weather, mobile network, elevation, usage type, address type, IAB category, district, autonomous system number (ASN) and autonomous system (AS) from traceroute probes IP address.
 
 *Note: This tool requires Python 2.7, or Python 3.5 or later.*
 
 ## Installation
 
 You can install this tool by using pip in Windows or Linux. To install this tool in Windows and Linux, just type `pip install IP2Trace` in your console and IP2Trace will be installed in your machine.
 
@@ -51,15 +51,15 @@
   If the database filename is specified but without the path, ip2tracepy will search the database file in /usr/local/share/ip2location/ for Linux or C:\Users\(your_Windows_username)\Documents\ for Windows.
 
   -t, --ttl
   Set the max number of hops. (Default: 30)
 
   -o, --output
   Set the desired IP2Location BIN database columns to output with.
-  Available columns are: country_code, country_name, region_name, city_name, isp, latitude, longitude, domain, zip_code, time_zone, net_speed, idd_code, area_code, weather_station_code, weather_station_name, mcc, mnc, mobile_brand, elevation, usage_type, address_type, category.
+  Available columns are: country_code, country_name, region_name, city_name, isp, latitude, longitude, domain, zip_code, time_zone, net_speed, idd_code, area_code, weather_station_code, weather_station_name, mcc, mnc, mobile_brand, elevation, usage_type, address_type, category, district, asn, as_name.
   
   -a, --all
   Print all the column(s) available based on the BIN file used.
 
   -h, -?, --help
   Display this guide.
 
@@ -74,16 +74,16 @@
 ```bash
 ip2tracepy 8.8.8.8 -d /usr/local/share/ip2location/DB3.BIN -a
 ```
 
 Example output:
 
 ```bash
-IP2Location Geolocation Traceroute (ip2trace) Version 3.1.3
-Copyright (c) 2021 IP2Location.com [MIT License]
+IP2Location Geolocation Traceroute (ip2trace) Version 3.2.0
+Copyright (c) 2023 IP2Location.com [MIT License]
 https://www.ip2location.com/free/traceroute-application
 
 Traceroute to dns.google ( 8.8.8.8 )
 
  1  37.123.114.1  0.3853ms ["GB","United Kingdom of Great Britain and Northern Ireland","England","London"]
  2  10.10.32.132  0.4084ms ["-","-","-","-"]
  3  10.10.32.17  0.2673ms ["-","-","-","-"]
@@ -100,16 +100,16 @@
 ```bash
 ip2tracepy google.com -d /usr/local/share/ip2location/DB3.BIN -a
 ```
 
 Example output:
 
 ```bash
-IP2Location Geolocation Traceroute (ip2trace) Version 3.1.3
-Copyright (c) 2021 IP2Location.com [MIT License]
+IP2Location Geolocation Traceroute (ip2trace) Version 3.2.0
+Copyright (c) 2023 IP2Location.com [MIT License]
 https://www.ip2location.com/free/traceroute-application
 
 Traceroute to dns.google ( 8.8.8.8 )
 
  1  37.123.114.1  0.3529ms ["GB","United Kingdom of Great Britain and Northern Ireland","England","London"]
  2  10.10.32.131  0.3686ms ["-","-","-","-"]
  3  10.10.32.17  0.2663ms ["-","-","-","-"]
```

### Comparing `IP2Trace-3.1.3/LICENSE.TXT` & `IP2Trace-3.2.0/LICENSE.TXT`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 IP2Location.com
+Copyright (c) 2023 IP2Location.com
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `IP2Trace-3.1.3/PKG-INFO` & `IP2Trace-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IP2Trace
-Version: 3.1.3
+Version: 3.2.0
 Summary: A Python tool to display geolocation information in the traceroute.
 Home-page: https://github.com/ip2location/ip2trace-python
 Author: IP2Location
 Author-email: support@ip2location.com
 License: MIT
 Project-URL: Official Website, https://www.ip2location.com
 Keywords: IP2Location Geolocation
@@ -22,15 +22,15 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 
 # IP2Trace Python
 
-IP2Trace Python is a Python tool allowing user to get IP address information such as country, region, city, latitude, longitude, zip code, time zone, ISP, domain name, connection type, area code, weather, mobile network, elevation, usage type from traceroute probes IP address.
+IP2Trace Python is a Python tool allowing user to get IP address information such as country, region, city, latitude, longitude, zip code, time zone, ISP, domain name, connection type, area code, weather, mobile network, elevation, usage type, address type, IAB category, district, autonomous system number (ASN) and autonomous system (AS) from traceroute probes IP address.
 
 *Note: This tool requires Python 2.7, or Python 3.5 or later.*
 
 ## Installation
 
 You can install this tool by using pip in Windows or Linux. To install this tool in Windows and Linux, just type `pip install IP2Trace` in your console and IP2Trace will be installed in your machine.
 
@@ -51,15 +51,15 @@
   If the database filename is specified but without the path, ip2tracepy will search the database file in /usr/local/share/ip2location/ for Linux or C:\Users\(your_Windows_username)\Documents\ for Windows.
 
   -t, --ttl
   Set the max number of hops. (Default: 30)
 
   -o, --output
   Set the desired IP2Location BIN database columns to output with.
-  Available columns are: country_code, country_name, region_name, city_name, isp, latitude, longitude, domain, zip_code, time_zone, net_speed, idd_code, area_code, weather_station_code, weather_station_name, mcc, mnc, mobile_brand, elevation, usage_type, address_type, category.
+  Available columns are: country_code, country_name, region_name, city_name, isp, latitude, longitude, domain, zip_code, time_zone, net_speed, idd_code, area_code, weather_station_code, weather_station_name, mcc, mnc, mobile_brand, elevation, usage_type, address_type, category, district, asn, as_name.
   
   -a, --all
   Print all the column(s) available based on the BIN file used.
 
   -h, -?, --help
   Display this guide.
 
@@ -74,16 +74,16 @@
 ```bash
 ip2tracepy 8.8.8.8 -d /usr/local/share/ip2location/DB3.BIN -a
 ```
 
 Example output:
 
 ```bash
-IP2Location Geolocation Traceroute (ip2trace) Version 3.1.3
-Copyright (c) 2021 IP2Location.com [MIT License]
+IP2Location Geolocation Traceroute (ip2trace) Version 3.2.0
+Copyright (c) 2023 IP2Location.com [MIT License]
 https://www.ip2location.com/free/traceroute-application
 
 Traceroute to dns.google ( 8.8.8.8 )
 
  1  37.123.114.1  0.3853ms ["GB","United Kingdom of Great Britain and Northern Ireland","England","London"]
  2  10.10.32.132  0.4084ms ["-","-","-","-"]
  3  10.10.32.17  0.2673ms ["-","-","-","-"]
@@ -100,16 +100,16 @@
 ```bash
 ip2tracepy google.com -d /usr/local/share/ip2location/DB3.BIN -a
 ```
 
 Example output:
 
 ```bash
-IP2Location Geolocation Traceroute (ip2trace) Version 3.1.3
-Copyright (c) 2021 IP2Location.com [MIT License]
+IP2Location Geolocation Traceroute (ip2trace) Version 3.2.0
+Copyright (c) 2023 IP2Location.com [MIT License]
 https://www.ip2location.com/free/traceroute-application
 
 Traceroute to dns.google ( 8.8.8.8 )
 
  1  37.123.114.1  0.3529ms ["GB","United Kingdom of Great Britain and Northern Ireland","England","London"]
  2  10.10.32.131  0.3686ms ["-","-","-","-"]
  3  10.10.32.17  0.2663ms ["-","-","-","-"]
```

### Comparing `IP2Trace-3.1.3/data/IP2LOCATION-LITE-DB1.IPV6.BIN` & `IP2Trace-3.2.0/data/IP2LOCATION-LITE-DB1.IPV6.BIN`

 * *Files identical despite different names*

### Comparing `IP2Trace-3.1.3/ip2trace - Copy.py` & `IP2Trace-3.2.0/ip2trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,17 @@
 from shutil import copyfile
 
 ICMP_ECHO = 8
 ICMP_V6_ECHO = 128
 ICMP_ECHO_REPLY = 0
 ICMP_V6_ECHO_REPLY = 129
 ICMP_TIME_EXCEEDED = 11
-# MIN_SLEEP = 1000
 
-# Windows IPv6 compatibility
-# if PLATFORM_WINDOWS:
-# if platform.system() == 'Windows':
-    # socket.IPPROTO_IPV6 = 41
-    # socket.IPPROTO_ICMPV6 = 58
-
-ip2location_result_fields = ['country_short', 'country_long', 'region', 'city', 'isp', 'latitude', 'longitude', 'domain', 'zipcode', 'timezone', 'netspeed', 'idd_code', 'area_code', 'weather_code', 'weather_name', 'mcc', 'mnc', 'mobile_brand', 'elevation', 'usage_type', 'address_type', 'category', ]
-ip2location_outputs_reference = ['country_code', 'country_name', 'region_name', 'city_name', 'isp', 'latitude', 'longitude', 'domain', 'zip_code', 'time_zone', 'net_speed', 'idd_code', 'area_code', 'weather_station_code', 'weather_station_name', 'mcc', 'mnc', 'mobile_brand', 'elevation', 'usage_type', 'address_type', 'category', ]
+ip2location_result_fields = ['country_short', 'country_long', 'region', 'city', 'isp', 'latitude', 'longitude', 'domain', 'zipcode', 'timezone', 'netspeed', 'idd_code', 'area_code', 'weather_code', 'weather_name', 'mcc', 'mnc', 'mobile_brand', 'elevation', 'usage_type', 'address_type', 'category', 'district', 'asn', 'as_name', ]
+ip2location_outputs_reference = ['country_code', 'country_name', 'region_name', 'city_name', 'isp', 'latitude', 'longitude', 'domain', 'zip_code', 'time_zone', 'net_speed', 'idd_code', 'area_code', 'weather_station_code', 'weather_station_name', 'mcc', 'mnc', 'mobile_brand', 'elevation', 'usage_type', 'address_type', 'category', 'district', 'asn', 'as_name', ]
 
 if platform.system() == 'Windows':
     # Windows IPv6 compatibility
     socket.IPPROTO_IPV6 = 41
     socket.IPPROTO_ICMPV6 = 58
     MIN_SLEEP = 500
     # Define BIN database default path
@@ -141,29 +134,29 @@
 "  If the database filename is specified but without the path, ip2tracepy will search the database file in /usr/share/ip2location/ for Linux or C:\\Users\\(your_Windows_username)\\Documents\\ for Windows.\n"
 "\n"
 "  -t, --ttl\n"
 "  Set the max number of hops. (Default: 30)\n"
 "\n"
 "  -o, --output\n"
 "  Set the desired IP2Location BIN database columns to output with.\n"
-"  Available columns are: country_code, country_name, region_name, city_name, isp, latitude, longitude, domain, zip_code, time_zone, net_speed, idd_code, area_code, weather_station_code, weather_station_name, mcc, mnc, mobile_brand, elevation, usage_type, address_type, category.\n"
+"  Available columns are: country_code, country_name, region_name, city_name, isp, latitude, longitude, domain, zip_code, time_zone, net_speed, idd_code, area_code, weather_station_code, weather_station_name, mcc, mnc, mobile_brand, elevation, usage_type, address_type, category, district, asn, as_name.\n"
 "\n"
 "  -a, --all\n"
 "Print all the column(s) available based on the BIN file used.\n"
 "\n"
 "  -h, -?, --help\n"
 "  Display this guide.\n"
 "\n"
 "  -v, --version\n"
 "  Print the version of the IP2Location version.\n")
 
 def print_version():
     print(
-"IP2Location Geolocation Traceroute (ip2trace) Version 3.1.3\n"
-"Copyright (c) 2022 IP2Location.com [MIT License]\n"
+"IP2Location Geolocation Traceroute (ip2trace) Version 3.2.0\n"
+"Copyright (c) 2023 IP2Location.com [MIT License]\n"
 "https://www.ip2location.com/free/traceroute-application\n")
 
 def traceroute(destination_server, database, ttl, output, all):
     t = Traceroute(destination_server, database, ttl, output, all)
     t.start_traceroute()
 
 class Traceroute:
@@ -227,19 +220,19 @@
                 print("Missing IP2Location BIN database. Please enter 'ip2trace -h' for more information.")
                 sys.exit()
 
         # check the output list
         if (self.output is not None):
             for i in self.output:
                 if i not in ip2location_outputs_reference:
-                    print("The column name is invalid. Please get a list of valid column names at https://ip2location.com/database/db24-ip-country-region-city-latitude-longitude-zipcode-timezone-isp-domain-netspeed-areacode-weather-mobile-elevation-usagetype.")
+                    print("The column name is invalid. Please get a list of valid column names at https://www.ip2location.com/database/db26-ip-country-region-city-latitude-longitude-zipcode-timezone-isp-domain-netspeed-areacode-weather-mobile-elevation-usagetype-addresstype-category-district-asn.")
                     sys.exit()
 
     def print_start(self):
-        print("IP2Location Geolocation Traceroute (ip2trace) Version 3.1.3\n"
+        print("IP2Location Geolocation Traceroute (ip2trace) Version 3.2.0\n"
 "Copyright (c) 2022 IP2Location.com [MIT License]\n"
 "https://www.ip2location.com/free/traceroute-application\n\n")
         if self.destination_domain_name is not None:
             print("Traceroute to", self.destination_domain_name[0], "(", self.destination_ip, ")\n\n", end="")
         else:
             print("Traceroute to", self.destination_ip, "\n\n", end="")
 
@@ -256,16 +249,14 @@
         if self.seq_no == self.count_of_packets:
             print()
 
     # def print_trace(self, delay, ip_header):
     def print_trace(self, delays, ip_header):
         total_delays = 0
         ip = socket.inet_ntoa(struct.pack('!I', ip_header['Source_IP']))
-        # ip = socket.inet_ntoa(struct.pack('!I', ip_header['Destination_IP']))
-        # print(ip_header['Source_IP'])
         try:
             sender_hostname = socket.gethostbyaddr(ip)[0]
         except socket.herror:
             sender_hostname = ip
         if self.prev_sender_hostname != sender_hostname:
             record = None
             if is_valid_ip(ip):
@@ -409,19 +400,14 @@
             for i in range(start_value, start_value+self.packet_size):
                 payload.append(i & 0xff)
             data = bytearray(payload)
         elif is_ipv6(self.destination_ip) == 6:
             header = struct.pack("!BBHHH", ICMP_V6_ECHO, 0, 0, self.identifier, self.seq_no)
             # header = struct.pack("!2B3H", ICMP_V6_ECHO, 0, 0, self.identifier, self.seq_no)
             data = self.random_byte_message(56)
-        '''
-        for i in range(start_value, start_value+self.packet_size):
-            payload.append(i & 0xff)
-        data = bytearray(payload)'''
-        # data = self.random_byte_message(56)
         checksum = calculate_checksum(header + data)
         if is_ipv4(self.destination_ip) == 4:
             header = struct.pack("!BBHHH", ICMP_ECHO, 0, checksum, self.identifier, self.seq_no)
             # header = struct.pack("!2B3H", ICMP_ECHO, 0, checksum, self.identifier, self.seq_no)
         elif is_ipv6(self.destination_ip) == 6:
             header = struct.pack("!BBHHH", ICMP_V6_ECHO, 0, checksum, self.identifier, self.seq_no)
             # header = struct.pack("!2B3H", ICMP_V6_ECHO, 0, checksum, self.identifier, self.seq_no)
@@ -442,30 +428,18 @@
         while True:
             inputReady, _, _ = select.select([icmp_socket], [], [], timeout)
             receive_time = timer()
             if receive_time > time_limit:  # timeout
                 # self.print_timeout()
                 return None, None, None
             packet_data, address = icmp_socket.recvfrom(1024)
-            '''
-            response = icmp_socket.recvfrom(1024)
-            packet = response[0]
-            source = response[1][0]
-            bytes_received = len(packet) - (-1)
-            if len(packet) > (-1 + 2):
-                type, code = unpack('!2B', packet[-1:2])
-                if type != -1:
-                    packet = packet[((-1 + 8) - (-1) + (-1)):]
-                if len(packet) > (-1 + 8):
-                    id, sequence = unpack('!2H', packet[(-1 + 4): (-1 + 8)])'''
             icmp_keys = ['type', 'code', 'checksum', 'identifier', 'sequence number']
             icmp_header = self.header_to_dict(icmp_keys, packet_data[20:28], "!BBHHH")
             ip_keys = ['VersionIHL', 'Type_of_Service', 'Total_Length', 'Identification', 'Flags_FragOffset', 'TTL', 'Protocol', 'Header_Checksum', 'Source_IP', 'Destination_IP']
             ip_header = self.header_to_dict(ip_keys, packet_data[:20], "!BBHHHBBHII")
-            # print(ip_header)
             # print ("Source_IP1", ip_header['Source_IP'])
             return receive_time, icmp_header, ip_header
 
 # if __name__ == '__main__':
 def main():
     is_help = False
     # print(sys.argv)
```

### Comparing `IP2Trace-3.1.3/readme.md` & `IP2Trace-3.2.0/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # IP2Trace Python
 
-IP2Trace Python is a Python tool allowing user to get IP address information such as country, region, city, latitude, longitude, zip code, time zone, ISP, domain name, connection type, area code, weather, mobile network, elevation, usage type from traceroute probes IP address.
+IP2Trace Python is a Python tool allowing user to get IP address information such as country, region, city, latitude, longitude, zip code, time zone, ISP, domain name, connection type, area code, weather, mobile network, elevation, usage type, address type, IAB category, district, autonomous system number (ASN) and autonomous system (AS) from traceroute probes IP address.
 
 *Note: This tool requires Python 2.7, or Python 3.5 or later.*
 
 ## Installation
 
 You can install this tool by using pip in Windows or Linux. To install this tool in Windows and Linux, just type `pip install IP2Trace` in your console and IP2Trace will be installed in your machine.
 
@@ -25,15 +25,15 @@
   If the database filename is specified but without the path, ip2tracepy will search the database file in /usr/local/share/ip2location/ for Linux or C:\Users\(your_Windows_username)\Documents\ for Windows.
 
   -t, --ttl
   Set the max number of hops. (Default: 30)
 
   -o, --output
   Set the desired IP2Location BIN database columns to output with.
-  Available columns are: country_code, country_name, region_name, city_name, isp, latitude, longitude, domain, zip_code, time_zone, net_speed, idd_code, area_code, weather_station_code, weather_station_name, mcc, mnc, mobile_brand, elevation, usage_type, address_type, category.
+  Available columns are: country_code, country_name, region_name, city_name, isp, latitude, longitude, domain, zip_code, time_zone, net_speed, idd_code, area_code, weather_station_code, weather_station_name, mcc, mnc, mobile_brand, elevation, usage_type, address_type, category, district, asn, as_name.
   
   -a, --all
   Print all the column(s) available based on the BIN file used.
 
   -h, -?, --help
   Display this guide.
 
@@ -48,16 +48,16 @@
 ```bash
 ip2tracepy 8.8.8.8 -d /usr/local/share/ip2location/DB3.BIN -a
 ```
 
 Example output:
 
 ```bash
-IP2Location Geolocation Traceroute (ip2trace) Version 3.1.3
-Copyright (c) 2021 IP2Location.com [MIT License]
+IP2Location Geolocation Traceroute (ip2trace) Version 3.2.0
+Copyright (c) 2023 IP2Location.com [MIT License]
 https://www.ip2location.com/free/traceroute-application
 
 Traceroute to dns.google ( 8.8.8.8 )
 
  1  37.123.114.1  0.3853ms ["GB","United Kingdom of Great Britain and Northern Ireland","England","London"]
  2  10.10.32.132  0.4084ms ["-","-","-","-"]
  3  10.10.32.17  0.2673ms ["-","-","-","-"]
@@ -74,16 +74,16 @@
 ```bash
 ip2tracepy google.com -d /usr/local/share/ip2location/DB3.BIN -a
 ```
 
 Example output:
 
 ```bash
-IP2Location Geolocation Traceroute (ip2trace) Version 3.1.3
-Copyright (c) 2021 IP2Location.com [MIT License]
+IP2Location Geolocation Traceroute (ip2trace) Version 3.2.0
+Copyright (c) 2023 IP2Location.com [MIT License]
 https://www.ip2location.com/free/traceroute-application
 
 Traceroute to dns.google ( 8.8.8.8 )
 
  1  37.123.114.1  0.3529ms ["GB","United Kingdom of Great Britain and Northern Ireland","England","London"]
  2  10.10.32.131  0.3686ms ["-","-","-","-"]
  3  10.10.32.17  0.2663ms ["-","-","-","-"]
```

### Comparing `IP2Trace-3.1.3/setup.py` & `IP2Trace-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import platform, os
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="IP2Trace",
-    version="3.1.3",
+    version="3.2.0",
     description="A Python tool to display geolocation information in the traceroute.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     entry_points={
         'console_scripts': [
             'ip2tracepy=ip2trace:main'
         ]
```

