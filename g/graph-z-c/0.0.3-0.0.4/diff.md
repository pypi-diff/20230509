# Comparing `tmp/graph_z_c-0.0.3.tar.gz` & `tmp/graph_z_c-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_z_c-0.0.3.tar", last modified: Mon May  8 02:22:14 2023, max compression
+gzip compressed data, was "graph_z_c-0.0.4.tar", last modified: Tue May  9 13:12:25 2023, max compression
```

## Comparing `graph_z_c-0.0.3.tar` & `graph_z_c-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-08 02:22:14.602539 graph_z_c-0.0.3/
--rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-08 02:22:14.602171 graph_z_c-0.0.3/PKG-INFO
--rw-r--r--   0 zelpha     (501) staff       (20)        0 2023-05-08 02:13:18.000000 graph_z_c-0.0.3/README.md
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-08 02:22:14.601396 graph_z_c-0.0.3/graph_z/
--rw-r--r--   0 zelpha     (501) staff       (20)       46 2023-05-08 02:22:00.000000 graph_z_c-0.0.3/graph_z/__init__.py
--rw-r--r--   0 zelpha     (501) staff       (20)     4101 2023-05-08 01:58:50.000000 graph_z_c-0.0.3/graph_z/graph_z.py
-drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-08 02:22:14.601959 graph_z_c-0.0.3/graph_z_c.egg-info/
--rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-08 02:22:14.000000 graph_z_c-0.0.3/graph_z_c.egg-info/PKG-INFO
--rw-r--r--   0 zelpha     (501) staff       (20)      189 2023-05-08 02:22:14.000000 graph_z_c-0.0.3/graph_z_c.egg-info/SOURCES.txt
--rw-r--r--   0 zelpha     (501) staff       (20)        1 2023-05-08 02:22:14.000000 graph_z_c-0.0.3/graph_z_c.egg-info/dependency_links.txt
--rw-r--r--   0 zelpha     (501) staff       (20)        8 2023-05-08 02:22:14.000000 graph_z_c-0.0.3/graph_z_c.egg-info/top_level.txt
--rw-r--r--   0 zelpha     (501) staff       (20)       38 2023-05-08 02:22:14.602637 graph_z_c-0.0.3/setup.cfg
--rw-r--r--   0 zelpha     (501) staff       (20)      174 2023-05-08 02:21:58.000000 graph_z_c-0.0.3/setup.py
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-09 13:12:25.012921 graph_z_c-0.0.4/
+-rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-09 13:12:25.012673 graph_z_c-0.0.4/PKG-INFO
+-rw-r--r--   0 zelpha     (501) staff       (20)        0 2023-05-08 02:13:18.000000 graph_z_c-0.0.4/README.md
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-09 13:12:25.011509 graph_z_c-0.0.4/graph_z/
+-rw-r--r--   0 zelpha     (501) staff       (20)       46 2023-05-08 02:22:00.000000 graph_z_c-0.0.4/graph_z/__init__.py
+-rw-r--r--   0 zelpha     (501) staff       (20)     3837 2023-05-09 13:12:10.000000 graph_z_c-0.0.4/graph_z/graph_z.py
+drwxr-xr-x   0 zelpha     (501) staff       (20)        0 2023-05-09 13:12:25.012405 graph_z_c-0.0.4/graph_z_c.egg-info/
+-rw-r--r--   0 zelpha     (501) staff       (20)      157 2023-05-09 13:12:24.000000 graph_z_c-0.0.4/graph_z_c.egg-info/PKG-INFO
+-rw-r--r--   0 zelpha     (501) staff       (20)      189 2023-05-09 13:12:24.000000 graph_z_c-0.0.4/graph_z_c.egg-info/SOURCES.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)        1 2023-05-09 13:12:24.000000 graph_z_c-0.0.4/graph_z_c.egg-info/dependency_links.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)        8 2023-05-09 13:12:24.000000 graph_z_c-0.0.4/graph_z_c.egg-info/top_level.txt
+-rw-r--r--   0 zelpha     (501) staff       (20)       38 2023-05-09 13:12:25.012995 graph_z_c-0.0.4/setup.cfg
+-rw-r--r--   0 zelpha     (501) staff       (20)      174 2023-05-09 13:12:17.000000 graph_z_c-0.0.4/setup.py
```

### Comparing `graph_z_c-0.0.3/graph_z/graph_z.py` & `graph_z_c-0.0.4/graph_z/graph_z.py`

 * *Files 10% similar despite different names*

```diff
@@ -79,44 +79,47 @@
     def bar_visuals(self):
         values = [vertex.value for vertex in self.vertices]
         sns.barplot(pd.DataFrame({
             'IDs': self.ids,
             'Values': values
         }), x='IDs', y='Values')
 
-    def circle_visuals(self):
-        n = len(self.vertices) # Number of vertices
-        angles = np.array([(2*np.pi)*k/n for k in range(n)])
-        x = np.cos(angles)
-        y = np.sin(angles)
+
+    def plot_graph(self):
         fig, ax = plt.subplots()
-        ax.scatter(x, y)
+        ax.set_aspect('equal')
 
-        # Annotate each vertice with its ID and Value
-        for i, vertex in enumerate(self.vertices):
-            ax.annotate('ID: {}, Value: {}'.format(vertex.id, vertex.value), (x[i], y[i]), textcoords="offset points", xytext=(0,10), ha='center')
-            vertex.circle_coordinates = (x[i], y[i])
+        n = len(self.vertices)
+        theta = np.linspace(0, 2*np.pi, n, endpoint=False)
+        x, y = np.cos(theta), np.sin(theta)
 
-        # Draw paths
-        for path in self.all_paths:
-            p1 = self.get_vertex(path[0]).circle_coordinates
-            p2 = self.get_vertex(path[1]).circle_coordinates
-            path_cost = path[2]
-            plot_line_segment(p1, p2)
-            plt.annotate('{}'.format(path_cost), get_midpoint(p1, p2), textcoords="offset points", xytext=(0, 0.01), ha='center')
+        # Plot the vertices
+        ax.scatter(x, y)
+        for i, vertex in enumerate(self.vertices):
+            ax.annotate(f"{vertex.id}:{vertex.value}", (x[i], y[i]))
 
+        # Plot the edges
+        for id1, id2, cost in self.all_paths:
+            vertex1, vertex2 = self.get_vertex(id1), self.get_vertex(id2)
+            i1, i2 = self.ids.index(id1), self.ids.index(id2)
+            ax.plot([x[i1], x[i2]], [y[i1], y[i2]])
+            ax.annotate(cost, ((x[i1]+x[i2])/2, (y[i1]+y[i2])/2))
 
-        ax.set_xlim(-2, 2)
-        ax.set_ylim(-2, 2)
         plt.show()
 
     def get_detailed_dataframe(self):
         values = []
         paths = []
         for vertex in self.vertices:
             values.append(vertex.value)
             paths.append(vertex.paths)
         return pd.DataFrame({
             "IDs": self.ids,
             "Values": values,
             "Paths (id, cost)": paths,
         })
+
+
+
+
+
+
```

