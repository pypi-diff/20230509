# Comparing `tmp/osm2geojson-0.2.3.tar.gz` & `tmp/osm2geojson-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm2geojson-0.2.3.tar", last modified: Sat Nov 12 13:09:12 2022, max compression
+gzip compressed data, was "osm2geojson-0.2.4.tar", last modified: Tue May  9 20:08:21 2023, max compression
```

## Comparing `osm2geojson-0.2.3.tar` & `osm2geojson-0.2.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 rapkin     (501) staff       (20)        0 2022-11-12 13:09:12.704783 osm2geojson-0.2.3/
--rw-r--r--   0 rapkin     (501) staff       (20)      101 2021-07-22 09:54:44.000000 osm2geojson-0.2.3/MANIFEST.in
--rw-r--r--   0 rapkin     (501) staff       (20)     4738 2022-11-12 13:09:12.704879 osm2geojson-0.2.3/PKG-INFO
--rw-r--r--   0 rapkin     (501) staff       (20)     3429 2022-03-22 01:10:08.000000 osm2geojson-0.2.3/README.md
-drwxr-xr-x   0 rapkin     (501) staff       (20)        0 2022-11-12 13:09:12.703855 osm2geojson-0.2.3/osm2geojson/
--rw-r--r--   0 rapkin     (501) staff       (20)      180 2021-07-22 09:54:44.000000 osm2geojson-0.2.3/osm2geojson/__init__.py
--rw-r--r--   0 rapkin     (501) staff       (20)     4273 2022-03-21 23:23:12.000000 osm2geojson-0.2.3/osm2geojson/__main__.py
--rw-r--r--   0 rapkin     (501) staff       (20)     3886 2021-07-22 09:54:44.000000 osm2geojson-0.2.3/osm2geojson/areaKeys.json
--rw-r--r--   0 rapkin     (501) staff       (20)     1411 2021-07-22 09:54:44.000000 osm2geojson-0.2.3/osm2geojson/helpers.py
--rw-r--r--   0 rapkin     (501) staff       (20)    17136 2022-11-12 13:06:54.000000 osm2geojson-0.2.3/osm2geojson/main.py
--rw-r--r--   0 rapkin     (501) staff       (20)     6042 2022-03-16 20:57:40.000000 osm2geojson-0.2.3/osm2geojson/parse_xml.py
--rw-r--r--   0 rapkin     (501) staff       (20)     2753 2021-07-22 09:54:44.000000 osm2geojson-0.2.3/osm2geojson/polygon-features.json
-drwxr-xr-x   0 rapkin     (501) staff       (20)        0 2022-11-12 13:09:12.704691 osm2geojson-0.2.3/osm2geojson.egg-info/
--rw-r--r--   0 rapkin     (501) staff       (20)     4738 2022-11-12 13:09:12.000000 osm2geojson-0.2.3/osm2geojson.egg-info/PKG-INFO
--rw-r--r--   0 rapkin     (501) staff       (20)      445 2022-11-12 13:09:12.000000 osm2geojson-0.2.3/osm2geojson.egg-info/SOURCES.txt
--rw-r--r--   0 rapkin     (501) staff       (20)        1 2022-11-12 13:09:12.000000 osm2geojson-0.2.3/osm2geojson.egg-info/dependency_links.txt
--rw-r--r--   0 rapkin     (501) staff       (20)       64 2022-11-12 13:09:12.000000 osm2geojson-0.2.3/osm2geojson.egg-info/entry_points.txt
--rw-r--r--   0 rapkin     (501) staff       (20)       17 2022-11-12 13:09:12.000000 osm2geojson-0.2.3/osm2geojson.egg-info/requires.txt
--rw-r--r--   0 rapkin     (501) staff       (20)       12 2022-11-12 13:09:12.000000 osm2geojson-0.2.3/osm2geojson.egg-info/top_level.txt
--rw-r--r--   0 rapkin     (501) staff       (20)       17 2021-07-22 09:54:44.000000 osm2geojson-0.2.3/requirements.txt
--rw-r--r--   0 rapkin     (501) staff       (20)       79 2022-11-12 13:09:12.705175 osm2geojson-0.2.3/setup.cfg
--rw-r--r--   0 rapkin     (501) staff       (20)      986 2022-11-12 13:08:41.000000 osm2geojson-0.2.3/setup.py
+drwxr-xr-x   0 rapkin     (501) staff       (20)        0 2023-05-09 20:08:21.689957 osm2geojson-0.2.4/
+-rw-r--r--   0 rapkin     (501) staff       (20)     1083 2021-07-22 09:54:44.000000 osm2geojson-0.2.4/LICENSE
+-rw-r--r--   0 rapkin     (501) staff       (20)      101 2021-07-22 09:54:44.000000 osm2geojson-0.2.4/MANIFEST.in
+-rw-r--r--   0 rapkin     (501) staff       (20)     3865 2023-05-09 20:08:21.690130 osm2geojson-0.2.4/PKG-INFO
+-rw-r--r--   0 rapkin     (501) staff       (20)     3541 2023-05-09 19:48:55.000000 osm2geojson-0.2.4/README.md
+drwxr-xr-x   0 rapkin     (501) staff       (20)        0 2023-05-09 20:08:21.688967 osm2geojson-0.2.4/osm2geojson/
+-rw-r--r--   0 rapkin     (501) staff       (20)      180 2021-07-22 09:54:44.000000 osm2geojson-0.2.4/osm2geojson/__init__.py
+-rw-r--r--   0 rapkin     (501) staff       (20)     4273 2022-03-21 23:23:12.000000 osm2geojson-0.2.4/osm2geojson/__main__.py
+-rw-r--r--   0 rapkin     (501) staff       (20)     3886 2021-07-22 09:54:44.000000 osm2geojson-0.2.4/osm2geojson/areaKeys.json
+-rw-r--r--   0 rapkin     (501) staff       (20)     1411 2021-07-22 09:54:44.000000 osm2geojson-0.2.4/osm2geojson/helpers.py
+-rw-r--r--   0 rapkin     (501) staff       (20)    20666 2023-05-09 20:04:45.000000 osm2geojson-0.2.4/osm2geojson/main.py
+-rw-r--r--   0 rapkin     (501) staff       (20)     6042 2022-03-16 20:57:40.000000 osm2geojson-0.2.4/osm2geojson/parse_xml.py
+-rw-r--r--   0 rapkin     (501) staff       (20)     2753 2021-07-22 09:54:44.000000 osm2geojson-0.2.4/osm2geojson/polygon-features.json
+drwxr-xr-x   0 rapkin     (501) staff       (20)        0 2023-05-09 20:08:21.689837 osm2geojson-0.2.4/osm2geojson.egg-info/
+-rw-r--r--   0 rapkin     (501) staff       (20)     3865 2023-05-09 20:08:21.000000 osm2geojson-0.2.4/osm2geojson.egg-info/PKG-INFO
+-rw-r--r--   0 rapkin     (501) staff       (20)      453 2023-05-09 20:08:21.000000 osm2geojson-0.2.4/osm2geojson.egg-info/SOURCES.txt
+-rw-r--r--   0 rapkin     (501) staff       (20)        1 2023-05-09 20:08:21.000000 osm2geojson-0.2.4/osm2geojson.egg-info/dependency_links.txt
+-rw-r--r--   0 rapkin     (501) staff       (20)       63 2023-05-09 20:08:21.000000 osm2geojson-0.2.4/osm2geojson.egg-info/entry_points.txt
+-rw-r--r--   0 rapkin     (501) staff       (20)       17 2023-05-09 20:08:21.000000 osm2geojson-0.2.4/osm2geojson.egg-info/requires.txt
+-rw-r--r--   0 rapkin     (501) staff       (20)       12 2023-05-09 20:08:21.000000 osm2geojson-0.2.4/osm2geojson.egg-info/top_level.txt
+-rw-r--r--   0 rapkin     (501) staff       (20)       17 2021-07-22 09:54:44.000000 osm2geojson-0.2.4/requirements.txt
+-rw-r--r--   0 rapkin     (501) staff       (20)       79 2023-05-09 20:08:21.690490 osm2geojson-0.2.4/setup.cfg
+-rw-r--r--   0 rapkin     (501) staff       (20)      986 2023-05-09 20:06:42.000000 osm2geojson-0.2.4/setup.py
```

### Comparing `osm2geojson-0.2.3/README.md` & `osm2geojson-0.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 Additional parameters for all functions:
 
 - `filter_used_refs` - (default: `True`) defines geometry filtration strategy (will return all geometry if set as `False`)
 - `log_level` - (default: `'ERROR'`) controls logging level (will print all logs if set as `'INFO'`). More details [here](https://docs.python.org/3/library/logging.html#logging-levels)
 - `area_keys` - (default: `None`) defines which keys and values of an area should be saved from the list of OSM tags, see `areaKeys.json` for the defaults
 - `polygon_features` - (default: `None`) defines a whitelist/blacklist of features to be included in resulting polygons, see `polygon-features.json` for the defaults
+- `raise_on_failure` - (default: `False`) controls whether to throw an exception when geometry generation fails
 
 Other handy methods:
 
 - `overpass_call(str query)` - runs query to overpass-api.de server (retries 5 times in case of error).
 - `shape_to_feature(Shape shape, dict properties)` - Converts Shape-object to GeoJSON with passed properties.
 
 **\*Shape-object - for convenience created simple dict to save Shapely object (geometry) and OSM-properties. Structure of this object:**
```

### Comparing `osm2geojson-0.2.3/osm2geojson/__main__.py` & `osm2geojson-0.2.4/osm2geojson/__main__.py`

 * *Files identical despite different names*

### Comparing `osm2geojson-0.2.3/osm2geojson/areaKeys.json` & `osm2geojson-0.2.4/osm2geojson/areaKeys.json`

 * *Files identical despite different names*

### Comparing `osm2geojson-0.2.3/osm2geojson/helpers.py` & `osm2geojson-0.2.4/osm2geojson/helpers.py`

 * *Files identical despite different names*

### Comparing `osm2geojson-0.2.3/osm2geojson/main.py` & `osm2geojson-0.2.4/osm2geojson/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,89 +28,97 @@
 if os.path.exists(DEFAULT_AREA_KEYS_FILE):
     with open(DEFAULT_AREA_KEYS_FILE) as f:
         _default_area_keys = json.load(f)['areaKeys']
 else:
     logger.warning("Default area keys file not found, using empty filter")
     _default_area_keys = {}
 
+def get_message(*args):
+    return ' '.join(args)
 
 def warning(*args):
     logger.warning(' '.join(args))
 
 
 def error(*args):
     logger.error(' '.join(args))
 
 
 def json2geojson(
         data, filter_used_refs=True, log_level='ERROR',
-        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None
+        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None,
+        raise_on_failure = False
 ):
     if isinstance(data, str):
         data = json.loads(data)
-    return _json2geojson(data, filter_used_refs, log_level, area_keys, polygon_features)
+    return _json2geojson(data, filter_used_refs, log_level, area_keys, polygon_features, raise_on_failure)
 
 
 def xml2geojson(
         xml_str, filter_used_refs=True, log_level='ERROR',
-        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None
+        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None,
+        raise_on_failure = False
 ):
     data = parse_xml(xml_str)
-    return _json2geojson(data, filter_used_refs, log_level, area_keys, polygon_features)
+    return _json2geojson(data, filter_used_refs, log_level, area_keys, polygon_features, raise_on_failure)
 
 
 def json2shapes(
         data, filter_used_refs=True, log_level='ERROR',
-        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None
+        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None,
+        raise_on_failure = False
 ):
     if isinstance(data, str):
         data = json.loads(data)
-    return _json2shapes(data, filter_used_refs, log_level, area_keys, polygon_features)
+    return _json2shapes(data, filter_used_refs, log_level, area_keys, polygon_features, raise_on_failure)
 
 
 def xml2shapes(
         xml_str, filter_used_refs=True, log_level='ERROR',
-        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None
+        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None,
+        raise_on_failure = False
 ):
     data = parse_xml(xml_str)
-    return _json2shapes(data, filter_used_refs, log_level, area_keys, polygon_features)
+    return _json2shapes(data, filter_used_refs, log_level, area_keys, polygon_features, raise_on_failure)
 
 
 def _json2geojson(
         data, filter_used_refs=True, log_level='ERROR',
-        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None
+        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None,
+        raise_on_failure = False
 ):
     features = []
-    for shape in _json2shapes(data, filter_used_refs, log_level, area_keys, polygon_features):
+    for shape in _json2shapes(data, filter_used_refs, log_level, area_keys, polygon_features, raise_on_failure):
         feature = shape_to_feature(shape['shape'], shape['properties'])
         features.append(feature)
 
     return {
         'type': 'FeatureCollection',
         'features': features
     }
 
 
 def _json2shapes(
         data, filter_used_refs=True, log_level='ERROR',
-        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None
+        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None,
+        raise_on_failure = False
 ):
     logger.setLevel(log_level)
     shapes = []
 
     refs = [
         el
         for el in data['elements']
         if el['type'] in ['node', 'way', 'relation']
     ]
 
     refs_index = build_refs_index(refs)
 
     for el in data['elements']:
-        shape = element_to_shape(el, refs_index, area_keys, polygon_features)
+        shape = element_to_shape(el, refs_index, area_keys, polygon_features, raise_on_failure=raise_on_failure)
         if shape is not None:
             shapes.append(shape)
         else:
             warning('Element not converted', pformat(el))
 
     if not filter_used_refs:
         return shapes
@@ -126,22 +134,22 @@
         if shape['properties']['id'] in used:
             continue
         filtered_shapes.append(shape)
 
     return filtered_shapes
 
 
-def element_to_shape(el, refs_index=None, area_keys: Optional[dict] = None, polygon_features: Optional[list] = None):
+def element_to_shape(el, refs_index=None, area_keys: Optional[dict] = None, polygon_features: Optional[list] = None, raise_on_failure = False):
     t = el['type']
     if t == 'node':
         return node_to_shape(el)
     if t == 'way':
-        return way_to_shape(el, refs_index, area_keys, polygon_features)
+        return way_to_shape(el, refs_index, area_keys, polygon_features, raise_on_failure=raise_on_failure)
     if t == 'relation':
-        return relation_to_shape(el, refs_index)
+        return relation_to_shape(el, refs_index, raise_on_failure=raise_on_failure)
     warning('Failed to convert element to shape')
     return None
 
 
 def _get_ref_name(el_type, id):
     return '%s/%s' % (el_type, id)
 
@@ -232,15 +240,16 @@
         if p.is_valid:
             logger.info('Geometry fixed!')
     return p
 
 
 def way_to_shape(
         way, refs_index: dict = None,
-        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None
+        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None,
+        raise_on_failure = False
 ):
     refs_index = refs_index or {}
     if 'center' in way:
         center = way['center']
         return {
             'shape': Point(center['lon'], center['lat']),
             'properties': get_element_props(way)
@@ -256,59 +265,78 @@
         coords = []
         for ref in way['nodes']:
             node = get_node_ref(ref, refs_index)
             if node:
                 node['used'] = way['id']
                 coords.append([node['lon'], node['lat']])
             else:
-                warning('Node not found in index', pformat(ref), 'for way', pformat(way))
+                message = get_message('Node not found in index', pformat(ref), 'for way', pformat(way))
+                warning(message)
+                if raise_on_failure:
+                    raise Exception(message)
                 return None
 
     elif 'ref' in way:
         ref = get_ref(way, refs_index)
         if not ref:
-            warning('Ref for way not found in index', pformat(way))
+            message = get_message('Ref for way not found in index', pformat(way))
+            warning(message)
+            if raise_on_failure:
+                raise Exception(message)
             return None
 
         if 'id' in way:
             ref['used'] = way['id']
         elif 'used' in way:
             ref['used'] = way['used']
         else:
             # filter will not work for this situation
             warning('Failed to mark ref as used', pformat(ref), 'for way', pformat(way))
-        ref_way = way_to_shape(ref, refs_index, area_keys, polygon_features)
+            # do we need to raise expection here? I don't think so
+        ref_way = way_to_shape(ref, refs_index, area_keys, polygon_features, raise_on_failure=raise_on_failure)
         if ref_way is None:
-            warning('Way by ref not converted to shape', pformat(way))
+            message = get_message('Way by ref not converted to shape', pformat(way))
+            warning(message)
+            if raise_on_failure:
+                raise Exception(message)
             return None
         coords = (
             ref_way['shape'].exterior
             if isinstance(ref_way['shape'], Polygon)
             else ref_way['shape']
         ).coords
 
     else:
         # throw exception
-        warning('Relation has way without nodes', pformat(way))
+        message = get_message('Relation has way without nodes', pformat(way))
+        warning(message)
+        if raise_on_failure:
+            raise Exception(message)
         return None
 
     if len(coords) < 2:
-        warning('Not found coords for way', pformat(way))
+        message = get_message('Not found coords for way', pformat(way))
+        warning(message)
+        if raise_on_failure:
+            raise Exception(message)
         return None
 
     props = get_element_props(way)
     if is_geometry_polygon(way, area_keys, polygon_features):
         try:
             poly = fix_invalid_polygon(Polygon(coords))
             return {
                 'shape': poly,
                 'properties': props
             }
         except Exception:
-            warning('Failed to generate polygon from way', pformat(way))
+            message = get_message('Failed to generate polygon from way', pformat(way))
+            warning(message)
+            if raise_on_failure:
+                raise Exception(message)
             return None
     else:
         return {
             'shape': LineString(coords),
             'properties': props
         }
 
@@ -366,209 +394,258 @@
             if rule['polygon'] == 'whitelist' and tags[rule['key']] in rule['values']:
                 return True
             if rule['polygon'] == 'blacklist':
                 return tags[rule['key']] not in rule['values']
     return False
 
 
-def relation_to_shape(rel, refs_index, area_keys: Optional[dict] = None, polygon_features: Optional[list] = None):
+def relation_to_shape(rel, refs_index, area_keys: Optional[dict] = None, polygon_features: Optional[list] = None, raise_on_failure = False):
     if 'center' in rel:
         center = rel['center']
         return {
             'shape': Point(center['lon'], center['lat']),
             'properties': get_element_props(rel)
         }
 
     try:
         if is_geometry_polygon(rel, area_keys, polygon_features):
-            return multipolygon_relation_to_shape(rel, refs_index)
+            return multipolygon_relation_to_shape(rel, refs_index, raise_on_failure=raise_on_failure)
         else:
-            return multiline_realation_to_shape(rel, refs_index)
+            return multiline_realation_to_shape(rel, refs_index, raise_on_failure=raise_on_failure)
     except Exception:
-        traceback.print_exc()
-        error('Failed to convert relation to shape', pformat(rel))
+        message = f'Failed to convert relation to shape: \n {pformat(rel)}'
+        error(message)
+        if raise_on_failure:
+            raise Exception(message)
 
 
 def multiline_realation_to_shape(
         rel, refs_index,
-        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None
+        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None,
+        raise_on_failure = False
 ):
     lines = []
 
     if 'members' in rel:
         members = rel['members']
     else:
         found_ref = get_ref(rel, refs_index)
         if not found_ref:
-            error('Ref for multiline relation not found in index', pformat(rel))
+            message = get_message('Ref for multiline relation not found in index', pformat(rel))
+            error(message)
+            if raise_on_failure:
+                raise Exception(message)
             return None
         members = found_ref['members']
 
     for member in members:
         if member['type'] == 'way':
-            way_shape = way_to_shape(member, refs_index, area_keys, polygon_features)
+            way_shape = way_to_shape(member, refs_index, area_keys, polygon_features, raise_on_failure=raise_on_failure)
         elif member['type'] == 'relation':
             found_member = get_ref(member, refs_index)
             if found_member:
                 found_member['used'] = rel['id']
-            way_shape = element_to_shape(member, refs_index, area_keys, polygon_features)
+            way_shape = element_to_shape(member, refs_index, area_keys, polygon_features, raise_on_failure=raise_on_failure)
         else:
-            warning('multiline member not handled', pformat(member))
+            message = get_message('multiline member not handled', pformat(member))
+            warning(message)
+            if raise_on_failure:
+                raise Exception(message)
             continue
 
         if way_shape is None:
             # throw exception
-            warning('Failed to make way in relation', pformat(rel))
+            message = get_message('Failed to make way in relation', pformat(rel))
+            warning(message)
+            if raise_on_failure:
+                raise Exception(message)
             continue
 
         if isinstance(way_shape['shape'], Polygon):
             # this should not happen on real data
             way_shape['shape'] = LineString(way_shape['shape'].exterior.coords)
         lines.append(way_shape['shape'])
 
     if len(lines) < 1:
-        warning('No lines for multiline relation', pformat(rel))
+        message = get_message('No lines for multiline relation', pformat(rel))
+        warning(message)
+        if raise_on_failure:
+            raise Exception(message)
         return None
 
     multiline = MultiLineString(lines)
     multiline = linemerge(multiline)
     return {
         'shape': multiline,
         'properties': get_element_props(rel)
     }
 
 
 def multipolygon_relation_to_shape(
         rel, refs_index,
-        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None
+        area_keys: Optional[dict] = None, polygon_features: Optional[list] = None,
+        raise_on_failure = False
 ):
     # List of Tuple (role, multipolygon)
     shapes = []
 
     if 'members' in rel:
         members = rel['members']
     else:
         found_ref = get_ref(rel, refs_index)
         if not found_ref:
-            error('Ref for multipolygon relation not found in index', pformat(rel))
+            message = get_message('Ref for multipolygon relation not found in index', pformat(rel))
+            error(message)
+            if raise_on_failure:
+                raise Exception(message)
             return None
         members = found_ref['members']
 
     for member in members:
         if member['type'] != 'way':
-            warning('Multipolygon member not handled', pformat(member))
+            message = get_message('Multipolygon member not handled', pformat(member))
+            warning(message)
+            if raise_on_failure:
+                raise Exception(message)
             continue
 
         member['used'] = rel['id']
 
-        way_shape = way_to_shape(member, refs_index, area_keys, polygon_features)
+        way_shape = way_to_shape(member, refs_index, area_keys, polygon_features, raise_on_failure=raise_on_failure)
         if way_shape is None:
             # throw exception
-            warning('Failed to make way', pformat(member), 'in relation', pformat(rel))
+            message = get_message('Failed to make way', pformat(member), 'in relation', pformat(rel))
+            warning(message)
+            if raise_on_failure:
+                raise Exception(message)
             continue
 
         if isinstance(way_shape['shape'], Polygon):
             way_shape['shape'] = LineString(way_shape['shape'].exterior.coords)
 
         shapes.append((member['role'], way_shape['shape']))
 
-    multipolygon = _convert_shapes_to_multipolygon(shapes)
+    multipolygon = _convert_shapes_to_multipolygon(shapes, raise_on_failure=raise_on_failure)
     if multipolygon is None:
-        warning('Failed to convert computed shapes to multipolygon', pformat(rel))
+        message = get_message('Failed to convert computed shapes to multipolygon', pformat(rel))
+        warning(message)
+        if raise_on_failure:
+            raise Exception(message)
         return None
 
     multipolygon = fix_invalid_polygon(multipolygon)
-    multipolygon = to_multipolygon(multipolygon)
+    multipolygon = to_multipolygon(multipolygon, raise_on_failure=raise_on_failure)
     multipolygon = orient_multipolygon(multipolygon)  # do we need this?
 
     if multipolygon is None:
-        warning('Failed to fix multipolygon. Report this in github please!', pformat(rel))
+        message = get_message('Failed to fix multipolygon. Report this in github please!', pformat(rel))
+        warning(message)
+        if raise_on_failure:
+            raise Exception(message)
         return None
 
     return {
         'shape': multipolygon,
         'properties': get_element_props(rel)
     }
 
 
-def to_multipolygon(obj):
+def to_multipolygon(obj, raise_on_failure=False):
     if isinstance(obj, MultiPolygon):
         return obj
 
     if isinstance(obj, GeometryCollection):
         p = [
             el for el in obj
             if isinstance(el, Polygon)
         ]
         return MultiPolygon(p)
 
     if isinstance(obj, Polygon):
         return MultiPolygon([obj])
 
     # throw exception
-    warning('Failed to convert to multipolygon', type(obj))
+    message = get_message('Failed to convert to multipolygon', type(obj))
+    warning(message)
+    if raise_on_failure:
+        raise Exception(message)
     return None
 
 
-def _convert_lines_to_multipolygon(lines):
+def _convert_lines_to_multipolygon(lines, raise_on_failure=False):
     multi_line = MultiLineString(lines)
     merged_line = linemerge(multi_line)
     if isinstance(merged_line, MultiLineString):
         polygons = []
         for line in merged_line.geoms:
             try:
                 poly = Polygon(line)
                 if poly.is_valid:
                     polygons.append(poly)
                 else:
                     polygons.append(poly.buffer(0))
             except Exception:
                 # throw exception
-                warning('Failed to build polygon', pformat(line))
-        return to_multipolygon(unary_union(polygons))
+                message = get_message('Failed to build polygon', pformat(line))
+                warning(message)
+                if raise_on_failure:
+                    raise Exception(message)
+        return to_multipolygon(unary_union(polygons), raise_on_failure=raise_on_failure)
     try:
         poly = Polygon(merged_line)
     except Exception as e:
-        warning('Failed to convert lines to polygon', pformat(e))
+        message = get_message('Failed to convert lines to polygon', pformat(e))
+        warning(message)
+        if raise_on_failure:
+            raise Exception(message)
         # traceback.print_exc()
         return None
-    return to_multipolygon(poly)
+    return to_multipolygon(poly, raise_on_failure=raise_on_failure)
 
 
-def _convert_shapes_to_multipolygon(shapes):
+def _convert_shapes_to_multipolygon(shapes, raise_on_failure=False):
     if len(shapes) < 1:
-        warning('Failed to create multipolygon (Empty)')
+        message = 'Failed to create multipolygon (Empty)'
+        warning(message)
+        if raise_on_failure:
+            raise Exception(message)
         return None
 
     # Intermediate groups
     groups = []
     # New group each time it switches role
     for role, group in itertools.groupby(shapes, lambda s: s[0]):
-        groups.append((role, _convert_lines_to_multipolygon([_[1] for _ in group])))
+        groups.append((role, _convert_lines_to_multipolygon([_[1] for _ in group], raise_on_failure=raise_on_failure)))
 
     multipolygon = None
     base_index = -1
     for i, (role, geom) in enumerate(groups):
         if role == 'outer':
             multipolygon = geom
             base_index = i
             break
 
     if base_index < 0:
-        warning('Failed to create multipolygon. Shape with "outer" role not found')
+        message = 'Failed to create multipolygon. Shape with "outer" role not found'
+        warning(message)
+        if raise_on_failure:
+            raise Exception(message)
         return None
 
     # Itterate over the rest if there are any
     for i, (role, geom) in enumerate(groups):
         if i == base_index:
             continue
 
         if role == "inner":
             multipolygon = multipolygon.difference(geom)
         else:
             multipolygon = multipolygon.union(geom)
 
         if multipolygon is None:
-            warning('Failed to compute multipolygon. Failing geometry:', role, geom)
+            message = get_message('Failed to compute multipolygon. Failing geometry:', role, geom)
+            warning(message)
+            if raise_on_failure:
+                raise Exception(message)
             return None
 
     return multipolygon
```

### Comparing `osm2geojson-0.2.3/osm2geojson/parse_xml.py` & `osm2geojson-0.2.4/osm2geojson/parse_xml.py`

 * *Files identical despite different names*

### Comparing `osm2geojson-0.2.3/osm2geojson/polygon-features.json` & `osm2geojson-0.2.4/osm2geojson/polygon-features.json`

 * *Files identical despite different names*

### Comparing `osm2geojson-0.2.3/setup.py` & `osm2geojson-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def parse_requirements(filename):
     lines = (line.strip() for line in open(path.join(dirname, filename)))
     return [line for line in lines if line and not line.startswith("#")]
 
 
 setup(
     name='osm2geojson',
-    version='0.2.3',
+    version='0.2.4',
     license='MIT',
     description='Parse OSM and Overpass JSON',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='geometry gis osm parsing',
     author='Parfeniuk Mykola',
     author_email='mikola.parfenyuck@gmail.com',
```

