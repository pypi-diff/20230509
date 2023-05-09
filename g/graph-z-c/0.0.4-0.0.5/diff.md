# Comparing `tmp/graph_z_c-0.0.4.tar.gz` & `tmp/graph_z_c-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_z_c-0.0.4.tar", last modified: Tue May  9 13:12:25 2023, max compression
+gzip compressed data, was "graph_z_c-0.0.5.tar", last modified: Tue May  9 13:41:03 2023, max compression
```

## Comparing `graph_z_c-0.0.4.tar` & `graph_z_c-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-09 13:12:25.012921 graph_z_c-0.0.4/
--rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-09 13:12:25.012673 graph_z_c-0.0.4/PKG-INFO
--rw-r--r--   0 zelpha     (501) staff       (20)        0 2023-05-08 02:13:18.000000 graph_z_c-0.0.4/README.md
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-09 13:12:25.011509 graph_z_c-0.0.4/graph_z/
--rw-r--r--   0 zelpha     (501) staff       (20)       46 2023-05-08 02:22:00.000000 graph_z_c-0.0.4/graph_z/__init__.py
--rw-r--r--   0 zelpha     (501) staff       (20)     3837 2023-05-09 13:12:10.000000 graph_z_c-0.0.4/graph_z/graph_z.py
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-09 13:12:25.012405 graph_z_c-0.0.4/graph_z_c.egg-info/
--rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-09 13:12:24.000000 graph_z_c-0.0.4/graph_z_c.egg-info/PKG-INFO
--rw-r--r--   0 zelpha     (501) staff       (20)      189 2023-05-09 13:12:24.000000 graph_z_c-0.0.4/graph_z_c.egg-info/SOURCES.txt
--rw-r--r--   0 zelpha     (501) staff       (20)        1 2023-05-09 13:12:24.000000 graph_z_c-0.0.4/graph_z_c.egg-info/dependency_links.txt
--rw-r--r--   0 zelpha     (501) staff       (20)        8 2023-05-09 13:12:24.000000 graph_z_c-0.0.4/graph_z_c.egg-info/top_level.txt
--rw-r--r--   0 zelpha     (501) staff       (20)       38 2023-05-09 13:12:25.012995 graph_z_c-0.0.4/setup.cfg
--rw-r--r--   0 zelpha     (501) staff       (20)      174 2023-05-09 13:12:17.000000 graph_z_c-0.0.4/setup.py
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-09 13:41:03.557340 graph_z_c-0.0.5/
+-rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-09 13:41:03.557155 graph_z_c-0.0.5/PKG-INFO
+-rw-r--r--   0 zelpha     (501) staff       (20)        0 2023-05-08 02:13:18.000000 graph_z_c-0.0.5/README.md
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-09 13:41:03.556443 graph_z_c-0.0.5/graph_z/
+-rw-r--r--   0 zelpha     (501) staff       (20)       73 2023-05-09 13:29:04.000000 graph_z_c-0.0.5/graph_z/__init__.py
+-rw-r--r--   0 zelpha     (501) staff       (20)     4697 2023-05-09 13:38:40.000000 graph_z_c-0.0.5/graph_z/graph_z.py
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-09 13:41:03.556968 graph_z_c-0.0.5/graph_z_c.egg-info/
+-rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-09 13:41:03.000000 graph_z_c-0.0.5/graph_z_c.egg-info/PKG-INFO
+-rw-r--r--   0 zelpha     (501) staff       (20)      189 2023-05-09 13:41:03.000000 graph_z_c-0.0.5/graph_z_c.egg-info/SOURCES.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)        1 2023-05-09 13:41:03.000000 graph_z_c-0.0.5/graph_z_c.egg-info/dependency_links.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)        8 2023-05-09 13:41:03.000000 graph_z_c-0.0.5/graph_z_c.egg-info/top_level.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)       38 2023-05-09 13:41:03.557389 graph_z_c-0.0.5/setup.cfg
+-rw-r--r--   0 zelpha     (501) staff       (20)      174 2023-05-09 13:40:49.000000 graph_z_c-0.0.5/setup.py
```

### Comparing `graph_z_c-0.0.4/graph_z/graph_z.py` & `graph_z_c-0.0.5/graph_z/graph_z.py`

 * *Files 14% similar despite different names*

```diff
@@ -115,11 +115,36 @@
         return pd.DataFrame({
             "IDs": self.ids,
             "Values": values,
             "Paths (id, cost)": paths,
         })
 
 
+def generate_random_graph(num_vertices, num_paths=0, value_range=(0, 10), path_cost_range=(1, 10), random_ids=False,):
+
+    vertex_values = np.random.randint(*value_range, size=num_vertices)
+    if random_ids:
+        vertex_ids = np.random.randint(0, 2**16, size=num_vertices)
+    else:
+        vertex_ids = np.arange(1, num_vertices+1, 1)
+    
+    graph = Graph()
+    for i in range(num_vertices):
+        vertex = Vertex(vertex_ids[i], vertex_values[i])
+        graph.add_vertex(vertex)
+    
+    path_costs = np.random.randint(*path_cost_range, size=num_paths)
+    for i in range(num_paths):
+        vertex_ids = [v.id for v in graph.vertices]  # get list of vertex IDs in the graph
+        rand_id1, rand_id2 = np.random.choice(vertex_ids, size=2, replace=False)
+        graph.add_path(rand_id1, rand_id2, path_costs[i])
+    
+    return graph
+
+
+    
+
+
```

