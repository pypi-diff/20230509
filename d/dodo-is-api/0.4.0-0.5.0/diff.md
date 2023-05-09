# Comparing `tmp/dodo_is_api-0.4.0.tar.gz` & `tmp/dodo_is_api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dodo_is_api-0.4.0.tar", max compression
+gzip compressed data, was "dodo_is_api-0.5.0.tar", max compression
```

## Comparing `dodo_is_api-0.4.0.tar` & `dodo_is_api-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     3582 2023-03-18 11:36:04.459981 dodo_is_api-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-03-18 06:06:54.111388 dodo_is_api-0.4.0/dodo_is_api/__init__.py
--rw-r--r--   0        0        0       27 2023-03-18 06:06:54.111896 dodo_is_api-0.4.0/dodo_is_api/connection/__init__.py
--rw-r--r--   0        0        0     1801 2023-03-18 11:36:04.460267 dodo_is_api-0.4.0/dodo_is_api/connection/base.py
--rw-r--r--   0        0        0     2131 2023-03-18 06:06:54.112897 dodo_is_api-0.4.0/dodo_is_api/connection/http_clients.py
--rw-r--r--   0        0        0     5873 2023-03-20 05:00:36.990122 dodo_is_api-0.4.0/dodo_is_api/connection/synchronous.py
--rw-r--r--   0        0        0      248 2023-03-18 06:06:54.113625 dodo_is_api-0.4.0/dodo_is_api/exceptions.py
--rw-r--r--   0        0        0     5632 2023-03-20 03:58:02.072521 dodo_is_api-0.4.0/dodo_is_api/mappers.py
--rw-r--r--   0        0        0       45 2023-03-18 11:36:04.461463 dodo_is_api-0.4.0/dodo_is_api/models/__init__.py
--rw-r--r--   0        0        0     1971 2023-03-20 04:59:10.643848 dodo_is_api-0.4.0/dodo_is_api/models/dodo_is_api.py
--rw-r--r--   0        0        0     1079 2023-03-20 03:36:43.059695 dodo_is_api-0.4.0/dodo_is_api/models/raw.py
--rw-r--r--   0        0        0      539 2023-03-20 05:41:37.578549 dodo_is_api-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4363 1970-01-01 00:00:00.000000 dodo_is_api-0.4.0/setup.py
--rw-r--r--   0        0        0     3912 1970-01-01 00:00:00.000000 dodo_is_api-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-03-22 13:32:15.868970 dodo_is_api-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3628 2023-03-24 05:03:49.211961 dodo_is_api-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-18 06:06:54.111388 dodo_is_api-0.5.0/dodo_is_api/__init__.py
+-rw-r--r--   0        0        0       55 2023-05-09 10:02:09.923060 dodo_is_api-0.5.0/dodo_is_api/connection/__init__.py
+-rw-r--r--   0        0        0     1932 2023-05-09 09:57:16.078330 dodo_is_api-0.5.0/dodo_is_api/connection/asynchronous.py
+-rw-r--r--   0        0        0     1291 2023-05-09 10:07:07.658345 dodo_is_api-0.5.0/dodo_is_api/connection/base.py
+-rw-r--r--   0        0        0     2131 2023-03-18 06:06:54.112897 dodo_is_api-0.5.0/dodo_is_api/connection/http_clients.py
+-rw-r--r--   0        0        0     7300 2023-05-09 10:07:07.653484 dodo_is_api-0.5.0/dodo_is_api/connection/synchronous.py
+-rw-r--r--   0        0        0      248 2023-03-18 06:06:54.113625 dodo_is_api-0.5.0/dodo_is_api/exceptions.py
+-rw-r--r--   0        0        0     7200 2023-04-15 05:46:29.175976 dodo_is_api-0.5.0/dodo_is_api/mappers.py
+-rw-r--r--   0        0        0       45 2023-03-18 11:36:04.461463 dodo_is_api-0.5.0/dodo_is_api/models/__init__.py
+-rw-r--r--   0        0        0     2798 2023-04-15 05:38:46.839507 dodo_is_api-0.5.0/dodo_is_api/models/dodo_is_api.py
+-rw-r--r--   0        0        0     1685 2023-04-15 05:38:46.839663 dodo_is_api-0.5.0/dodo_is_api/models/raw.py
+-rw-r--r--   0        0        0      539 2023-05-09 10:15:21.294850 dodo_is_api-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4411 1970-01-01 00:00:00.000000 dodo_is_api-0.5.0/setup.py
+-rw-r--r--   0        0        0     3958 1970-01-01 00:00:00.000000 dodo_is_api-0.5.0/PKG-INFO
```

### Comparing `dodo_is_api-0.4.0/README.md` & `dodo_is_api-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+<div align="center">
 <a href="https://dodo-brands.stoplight.io">
-<img src="https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg">
+<img width="350px" src="https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg">
 </a>
-
+</div>
+    
 <h1 align="center">
 🍕 Dodo IS API Wrapper
 </h1>
 
 <p align="center">
 <a href="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml">
 <img src="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml/badge.svg" alt="Test badge">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-[https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg]
+      [https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg]
                     ****** ð Dodo IS API Wrapper ******
  [Test_badge] [https://codecov.io/gh/goretsky-integration/dodo-is-api-python-
         wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD] [python]
 --- ### Installation Via pip: ```shell pip install dodo-is-api ``` Via poetry:
 ```shell poetry add dodo-is-api ``` --- #### ð [Changelog](https://
 github.com/goretsky-integration/dodo-is-api-python-wrapper/blob/main/
 CHANGELOG.md) is here. --- ### ð§ª Usage: - Delivery: - [Late delivery
```

### Comparing `dodo_is_api-0.4.0/dodo_is_api/connection/base.py` & `dodo_is_api-0.5.0/dodo_is_api/connection/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,20 @@
-import datetime
-from abc import ABC, abstractmethod
 from collections.abc import Iterable
 from uuid import UUID
 
 import httpx
 
 from .. import exceptions
 
 __all__ = (
-    'BaseConnection',
     'concatenate_uuids',
     'raise_for_status'
 )
 
 
-class BaseConnection(ABC):
-
-    @abstractmethod
-    def iter_late_delivery_vouchers(
-            self,
-            *,
-            from_date: datetime.datetime,
-            to_date: datetime.datetime,
-            units: Iterable[UUID],
-            skip: int = 0,
-            take: int = 1000,
-    ) -> Iterable[list[dict]]:
-        """
-        Corresponds to this API endpoint:
-        https://dodo-brands.stoplight.io/docs/dodo-is/f3c261f246fc0-dostavka-sertifikaty-za-opozdanie
-        """
-
-
 def concatenate_uuids(uuids: Iterable[UUID], join_symbol: str = ',') -> str:
     """Convert UUIDs collection to UUIDs string suitable for Dodo IS API.
 
     Examples:
          >>> concatenate_uuids([UUID('6ff7d64d-1457-47f2-a396-1174994c1e20'), UUID('e27b64cf-346f-4f69-817c-c8ccd4814826')])
          '6ff7d64d145747f2a3961174994c1e20,e27b64cf346f4f69817cc8ccd4814826'
 
@@ -54,9 +33,10 @@
         return
     status_code_to_exception_class = {
         429: exceptions.TooManyRequestsError,
         403: exceptions.ForbiddenError,
         401: exceptions.UnauthorizedError,
         400: exceptions.BadRequestError,
     }
-    exception_class = status_code_to_exception_class.get(response.status_code, exceptions.DodoISAPIError)
+    exception_class = status_code_to_exception_class.get(response.status_code,
+                                                         exceptions.DodoISAPIError)
     raise exception_class
```

### Comparing `dodo_is_api-0.4.0/dodo_is_api/connection/http_clients.py` & `dodo_is_api-0.5.0/dodo_is_api/connection/http_clients.py`

 * *Files identical despite different names*

### Comparing `dodo_is_api-0.4.0/dodo_is_api/connection/synchronous.py` & `dodo_is_api-0.5.0/dodo_is_api/connection/synchronous.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import datetime
 from collections.abc import Iterable, Generator
 from uuid import UUID
 
 import httpx
 
-from .base import BaseConnection, concatenate_uuids, raise_for_status
+from .base import concatenate_uuids, raise_for_status
 from ..models import raw as raw_models
 
 __all__ = ('DodoISAPIConnection',)
 
 
-class DodoISAPIConnection(BaseConnection):
+class DodoISAPIConnection:
     __slots__ = ('__http_client',)
 
     def __init__(self, *, http_client: httpx.Client):
         self.__http_client = http_client
 
     def iter_late_delivery_vouchers(
             self,
@@ -163,7 +163,49 @@
             'units': concatenate_uuids(units),
         }
         response = self.__http_client.get(url, params=request_query_params)
         raise_for_status(response)
 
         response_data: dict = response.json()
         return response_data['unitsStatistics']
+
+    def iter_courier_orders(
+            self,
+            *,
+            from_date: datetime.datetime,
+            to_date: datetime.datetime,
+            units: Iterable[UUID],
+            skip: int = 0,
+            take: int = 1000,
+    ) -> Generator[list[raw_models.CourierOrderTypedDict], None, None]:
+        """
+        References:
+            Documentation: https://dodo-brands.stoplight.io/docs/dodo-is/14c586221ab77-dostavka-zakazy-kurerov.
+
+        Keyword Args:
+            from_date: start of period in ISO 8601 format.
+            to_date: end of period in ISO 8601 format.
+            units: collection of unit's UUIDs.
+            skip: items count to skip.
+            take: items count to take.
+
+        Returns:
+            List of unit's delivery statistics.
+        """
+        url = '/delivery/couriers-orders'
+        request_query_params = {
+            'from': from_date.strftime('%Y-%m-%dT%H:%M:%S'),
+            'to': to_date.strftime('%Y-%m-%dT%H:%M:%S'),
+            'units': concatenate_uuids(units),
+            'skip': skip,
+            'take': take,
+        }
+
+        while True:
+            response = self.__http_client.get(url, params=request_query_params)
+            raise_for_status(response)
+
+            response_data: dict = response.json()
+            yield response_data['couriersOrders']
+            if response_data['isEndOfListReached']:
+                break
+            request_query_params['skip'] += take
```

### Comparing `dodo_is_api-0.4.0/dodo_is_api/mappers.py` & `dodo_is_api-0.5.0/dodo_is_api/mappers.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 __all__ = (
     'map_late_delivery_voucher_dto',
     'map_stop_sale_by_sales_channel_dto',
     'map_stop_sale_by_product_dto',
     'map_stop_sale_by_ingredient_dto',
     'map_unit_delivery_statistics_dto',
+    'map_courier_order_dto',
 )
 
 
 def parse_to_datetime_or_none(value: str | None) -> datetime | None | NoReturn:
     match value:
         case str():
             return datetime.fromisoformat(value)
@@ -124,7 +125,41 @@
         average_order_trip_time=unit_delivery_statistics['avgOrderTripTime'],
         late_orders_count=unit_delivery_statistics['lateOrdersCount'],
         trips_count=unit_delivery_statistics['tripsCount'],
         trips_duration=unit_delivery_statistics['tripsDuration'],
         couriers_shifts_duration=unit_delivery_statistics['couriersShiftsDuration'],
         orders_with_courier_app_count=unit_delivery_statistics['ordersWithCourierAppCount'],
     )
+
+
+def map_courier_order_dto(
+        courier_order: raw_models.CourierOrderTypedDict,
+) -> models.CourierOrder:
+    return models.CourierOrder(
+        courier_staff_id=UUID(courier_order['courierStaffId']),
+        delivery_time=courier_order['deliveryTime'],
+        delivery_transport_name=models.DeliveryTransportName(
+            courier_order['deliveryTransportName'],
+        ),
+        handed_over_to_delivery_at=datetime.fromisoformat(
+            courier_order['handedOverToDeliveryAt'],
+        ),
+        handed_over_to_delivery_at_local=datetime.fromisoformat(
+            courier_order['handedOverToDeliveryAt'],
+        ),
+        heated_shelf_time=courier_order['heatedShelfTime'],
+        is_false_delivery=courier_order['isFalseDelivery'],
+        is_problematic_delivery=courier_order['isProblematicDelivery'],
+        order_assembly_average_time=courier_order['orderAssemblyAvgTime'],
+        order_fulfilment_flag_at=parse_to_datetime_or_none(
+            courier_order['orderFulfilmentFlagAt'],
+        ),
+        order_id=UUID(courier_order['orderId']),
+        order_number=courier_order['orderNumber'],
+        predicted_delivery_time=courier_order['predictedDeliveryTime'],
+        problematic_delivery_reason=courier_order['problematicDeliveryReason'],
+        trip_orders_count=courier_order['tripOrdersCount'],
+        unit_uuid=UUID(courier_order['unitId']),
+        unit_name=courier_order['unitName'],
+        was_late_delivery_voucher_given=courier_order[
+            'wasLateDeliveryVoucherGiven'],
+    )
```

### Comparing `dodo_is_api-0.4.0/dodo_is_api/models/dodo_is_api.py` & `dodo_is_api-0.5.0/dodo_is_api/models/dodo_is_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     'StopSale',
     'StopSaleByProduct',
     'StopSaleByIngredient',
     'StopSaleBySalesChannel',
     'SalesChannel',
     'ChannelStopType',
     'UnitDeliveryStatistics',
+    'CourierOrder',
+    'DeliveryTransportName',
 )
 
 
 @dataclass(frozen=True, slots=True)
 class LateDeliveryVoucher:
     order_id: UUID
     order_number: str
@@ -78,7 +80,35 @@
     average_heated_shelf_time: int
     average_order_trip_time: int
     late_orders_count: int
     trips_count: int
     trips_duration: int
     couriers_shifts_duration: int
     orders_with_courier_app_count: int
+
+
+class DeliveryTransportName(enum.Enum):
+    VEHICLE = 'Vehicle'
+    ON_FOOT = 'OnFoot'
+    BICYCLE = 'Bicycle'
+
+
+@dataclass(frozen=True, slots=True)
+class CourierOrder:
+    courier_staff_id: UUID
+    delivery_time: int
+    delivery_transport_name: DeliveryTransportName
+    handed_over_to_delivery_at: datetime.datetime
+    handed_over_to_delivery_at_local: datetime.datetime
+    heated_shelf_time: int
+    is_false_delivery: bool
+    is_problematic_delivery: bool
+    order_assembly_average_time: int
+    order_fulfilment_flag_at: datetime.datetime | None
+    order_id: UUID
+    order_number: str
+    predicted_delivery_time: int
+    problematic_delivery_reason: str
+    trip_orders_count: int
+    unit_uuid: UUID
+    unit_name: str
+    was_late_delivery_voucher_given: bool
```

### Comparing `dodo_is_api-0.4.0/dodo_is_api/models/raw.py` & `dodo_is_api-0.5.0/dodo_is_api/models/raw.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from typing import TypedDict
+from typing import TypedDict, Literal
 
 __all__ = (
     'StopSaleTypedDict',
     'StopSaleByIngredientTypedDict',
     'StopSaleBySalesChannelTypedDict',
     'StopSaleByProductTypedDict',
     'UnitDeliveryStatisticsTypedDict',
+    'CourierOrderTypedDict',
 )
 
 
 class StopSaleTypedDict(TypedDict):
     id: str
     unitId: str
     unitName: str
@@ -43,7 +44,28 @@
     avgHeatedShelfTime: int
     avgOrderTripTime: int
     lateOrdersCount: int
     tripsCount: int
     tripsDuration: int
     couriersShiftsDuration: int
     ordersWithCourierAppCount: int
+
+
+class CourierOrderTypedDict(TypedDict):
+    orderId: str
+    orderNumber: str
+    courierStaffId: str
+    unitId: str
+    unitName: str
+    handedOverToDeliveryAt: str
+    predictedDeliveryTime: int
+    deliveryTime: int
+    orderFulfilmentFlagAt: str
+    orderFulfilmentFlagAtLocal: str
+    isFalseDelivery: bool
+    deliveryTransportName: Literal['Vehicle', 'OnFoot', 'Bicycle']
+    tripOrdersCount: int
+    heatedShelfTime: int
+    orderAssemblyAvgTime: int
+    isProblematicDelivery: bool
+    problematicDeliveryReason: str
+    wasLateDeliveryVoucherGiven: bool
```

### Comparing `dodo_is_api-0.4.0/pyproject.toml` & `dodo_is_api-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dodo-is-api"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Eldos <eldos.baktybekov@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dodo_is_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `dodo_is_api-0.4.0/setup.py` & `dodo_is_api-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['httpx>=0.23.3,<0.24.0']
 
 setup_kwargs = {
     'name': 'dodo-is-api',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': '',
-    'long_description': '<a href="https://dodo-brands.stoplight.io">\n<img src="https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg">\n</a>\n\n<h1 align="center">\n🍕 Dodo IS API Wrapper\n</h1>\n\n<p align="center">\n<a href="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml">\n<img src="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml/badge.svg" alt="Test badge">\n</a>\n<a href="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper">\n<img src="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD"/>\n</a>\n<img src="https://img.shields.io/badge/python-3.11-brightgreen" alt="python">\n</p>\n\n---\n\n### Installation\n\nVia pip:\n```shell\npip install dodo-is-api\n```\n\nVia poetry:\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n#### 📝 [Changelog](https://github.com/goretsky-integration/dodo-is-api-python-wrapper/blob/main/CHANGELOG.md) is here.\n\n---\n\n### 🧪 Usage:\n\n- Delivery:\n    - [Late delivery vouchers](#get-late-delivery-vouchers-)\n- Production:\n    - [Stop sales](#get-stop-sales-)\n\n---\n\n#### 🛵 Get late delivery vouchers:\n\n```python\nimport datetime\nfrom uuid import UUID\n\nfrom dodo_is_api.connection import DodoISAPIConnection\nfrom dodo_is_api.connection.http_clients import closing_http_client\nfrom dodo_is_api.mappers import map_late_delivery_voucher_dto\n\naccess_token = \'my-token\'\ncountry_code = \'kg\'\n\nunits = [UUID(\'e0ce0423-3064-4e04-ad3e-39906643ef14\'), UUID(\'bd09b0a8-147d-46f7-8908-874f5f59c9a2\')]\nfrom_date = datetime.datetime(year=2023, month=3, day=16)\nto_date = datetime.datetime(year=2023, month=3, day=17)\n\nwith closing_http_client(access_token=access_token, country_code=country_code) as http_client:\n    dodo_is_api_connection = DodoISAPIConnection(http_client=http_client)\n\n    # it will handle pagination for you\n    for late_delivery_vouchers in dodo_is_api_connection.iter_late_delivery_vouchers(\n            from_date=from_date,\n            to_date=to_date,\n            units=units\n    ):\n        # map to dataclass DTO if you need\n        late_delivery_voucher_dtos = [\n            map_late_delivery_voucher_dto(late_delivery_voucher)\n            for late_delivery_voucher in late_delivery_vouchers\n        ]\n        ...\n```\n\n---\n\n#### 📦 Get stop sales:\n\n```python\nimport datetime\nfrom uuid import UUID\n\nfrom dodo_is_api.connection import DodoISAPIConnection\nfrom dodo_is_api.connection.http_clients import closing_http_client\nfrom dodo_is_api.mappers import map_stop_sale_by_ingredient_dto\n\naccess_token = \'my-token\'\ncountry_code = \'kg\'\n\nunits = [UUID(\'e0ce0423-3064-4e04-ad3e-39906643ef14\'), UUID(\'bd09b0a8-147d-46f7-8908-874f5f59c9a2\')]\nfrom_date = datetime.datetime(year=2023, month=3, day=16)\nto_date = datetime.datetime(year=2023, month=3, day=17)\n\nwith closing_http_client(access_token=access_token, country_code=country_code) as http_client:\n    dodo_is_api_connection = DodoISAPIConnection(http_client=http_client)\n\n    # for products - dodo_is_api_connection.get_stop_sales_by_products\n    # for sales channels - dodo_is_api_connection.get_stop_sales_by_sales_channels\n    stop_sales = dodo_is_api_connection.get_stop_sales_by_ingredients(\n        from_date=from_date,\n        to_date=to_date,\n        units=units\n    )\n\n    # map to dataclass DTO if you need\n    # use suitable mapper\n    # in this case, ingredient stop sale mapper is used\n    late_delivery_voucher_dtos = [\n        map_stop_sale_by_ingredient_dto(stop_sale)\n        for stop_sale in stop_sales\n    ]\n    ...\n```\n',
+    'long_description': '<div align="center">\n<a href="https://dodo-brands.stoplight.io">\n<img width="350px" src="https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg">\n</a>\n</div>\n    \n<h1 align="center">\n🍕 Dodo IS API Wrapper\n</h1>\n\n<p align="center">\n<a href="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml">\n<img src="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml/badge.svg" alt="Test badge">\n</a>\n<a href="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper">\n<img src="https://codecov.io/gh/goretsky-integration/dodo-is-api-python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD"/>\n</a>\n<img src="https://img.shields.io/badge/python-3.11-brightgreen" alt="python">\n</p>\n\n---\n\n### Installation\n\nVia pip:\n```shell\npip install dodo-is-api\n```\n\nVia poetry:\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n#### 📝 [Changelog](https://github.com/goretsky-integration/dodo-is-api-python-wrapper/blob/main/CHANGELOG.md) is here.\n\n---\n\n### 🧪 Usage:\n\n- Delivery:\n    - [Late delivery vouchers](#get-late-delivery-vouchers-)\n- Production:\n    - [Stop sales](#get-stop-sales-)\n\n---\n\n#### 🛵 Get late delivery vouchers:\n\n```python\nimport datetime\nfrom uuid import UUID\n\nfrom dodo_is_api.connection import DodoISAPIConnection\nfrom dodo_is_api.connection.http_clients import closing_http_client\nfrom dodo_is_api.mappers import map_late_delivery_voucher_dto\n\naccess_token = \'my-token\'\ncountry_code = \'kg\'\n\nunits = [UUID(\'e0ce0423-3064-4e04-ad3e-39906643ef14\'), UUID(\'bd09b0a8-147d-46f7-8908-874f5f59c9a2\')]\nfrom_date = datetime.datetime(year=2023, month=3, day=16)\nto_date = datetime.datetime(year=2023, month=3, day=17)\n\nwith closing_http_client(access_token=access_token, country_code=country_code) as http_client:\n    dodo_is_api_connection = DodoISAPIConnection(http_client=http_client)\n\n    # it will handle pagination for you\n    for late_delivery_vouchers in dodo_is_api_connection.iter_late_delivery_vouchers(\n            from_date=from_date,\n            to_date=to_date,\n            units=units\n    ):\n        # map to dataclass DTO if you need\n        late_delivery_voucher_dtos = [\n            map_late_delivery_voucher_dto(late_delivery_voucher)\n            for late_delivery_voucher in late_delivery_vouchers\n        ]\n        ...\n```\n\n---\n\n#### 📦 Get stop sales:\n\n```python\nimport datetime\nfrom uuid import UUID\n\nfrom dodo_is_api.connection import DodoISAPIConnection\nfrom dodo_is_api.connection.http_clients import closing_http_client\nfrom dodo_is_api.mappers import map_stop_sale_by_ingredient_dto\n\naccess_token = \'my-token\'\ncountry_code = \'kg\'\n\nunits = [UUID(\'e0ce0423-3064-4e04-ad3e-39906643ef14\'), UUID(\'bd09b0a8-147d-46f7-8908-874f5f59c9a2\')]\nfrom_date = datetime.datetime(year=2023, month=3, day=16)\nto_date = datetime.datetime(year=2023, month=3, day=17)\n\nwith closing_http_client(access_token=access_token, country_code=country_code) as http_client:\n    dodo_is_api_connection = DodoISAPIConnection(http_client=http_client)\n\n    # for products - dodo_is_api_connection.get_stop_sales_by_products\n    # for sales channels - dodo_is_api_connection.get_stop_sales_by_sales_channels\n    stop_sales = dodo_is_api_connection.get_stop_sales_by_ingredients(\n        from_date=from_date,\n        to_date=to_date,\n        units=units\n    )\n\n    # map to dataclass DTO if you need\n    # use suitable mapper\n    # in this case, ingredient stop sale mapper is used\n    late_delivery_voucher_dtos = [\n        map_stop_sale_by_ingredient_dto(stop_sale)\n        for stop_sale in stop_sales\n    ]\n    ...\n```\n',
     'author': 'Eldos',
     'author_email': 'eldos.baktybekov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['dodo_is_api', 'dodo_is_api.connection', 'dodo_is_api.models'] package_data =
 \ {'': ['*']} install_requires = \ ['httpx>=0.23.3,<0.24.0'] setup_kwargs =
-{ 'name': 'dodo-is-api', 'version': '0.4.0', 'description': '',
-'long_description': '\n[https://api.huntflow.io/logo/
-866df3c58ea44c158c6e36010631fd9f.jpg]\n\n\n
+{ 'name': 'dodo-is-api', 'version': '0.5.0', 'description': '',
+'long_description': '
+  \n\n[https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg]\n\n
+\n \n
                   ****** \nð Dodo IS API Wrapper\n ******
 \n\n
 \n\n[Test_badge]\n\n\n[https://codecov.io/gh/goretsky-integration/dodo-is-api-
   python-wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD]\n\n[python]\n
 \n\n---\n\n### Installation\n\nVia pip:\n```shell\npip install dodo-is-
 api\n```\n\nVia poetry:\n```shell\npoetry add dodo-is-api\n```\n\n---\n\n####
 ð [Changelog](https://github.com/goretsky-integration/dodo-is-api-python-
```

### Comparing `dodo_is_api-0.4.0/PKG-INFO` & `dodo_is_api-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: dodo-is-api
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: Eldos
 Author-email: eldos.baktybekov@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Description-Content-Type: text/markdown
 
+<div align="center">
 <a href="https://dodo-brands.stoplight.io">
-<img src="https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg">
+<img width="350px" src="https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg">
 </a>
-
+</div>
+    
 <h1 align="center">
 🍕 Dodo IS API Wrapper
 </h1>
 
 <p align="center">
 <a href="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml">
 <img src="https://github.com/goretsky-integration/dodo-is-api-python-wrapper/actions/workflows/unittest.yaml/badge.svg" alt="Test badge">
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: dodo-is-api Version: 0.4.0 Summary: Author: Eldos
+Metadata-Version: 2.1 Name: dodo-is-api Version: 0.5.0 Summary: Author: Eldos
 Author-email: eldos.baktybekov@gmail.com Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: httpx (>=0.23.3,<0.24.0) Description-
-Content-Type: text/markdown [https://api.huntflow.io/logo/
-866df3c58ea44c158c6e36010631fd9f.jpg]
+Content-Type: text/markdown
+      [https://api.huntflow.io/logo/866df3c58ea44c158c6e36010631fd9f.jpg]
                     ****** ð Dodo IS API Wrapper ******
  [Test_badge] [https://codecov.io/gh/goretsky-integration/dodo-is-api-python-
         wrapper/branch/main/graph/badge.svg?token=unzlMmAjsD] [python]
 --- ### Installation Via pip: ```shell pip install dodo-is-api ``` Via poetry:
 ```shell poetry add dodo-is-api ``` --- #### ð [Changelog](https://
 github.com/goretsky-integration/dodo-is-api-python-wrapper/blob/main/
 CHANGELOG.md) is here. --- ### ð§ª Usage: - Delivery: - [Late delivery
```

