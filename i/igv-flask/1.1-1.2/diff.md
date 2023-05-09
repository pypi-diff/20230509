# Comparing `tmp/igv-flask-1.1.tar.gz` & `tmp/igv-flask-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/igv-flask-1.1.tar", last modified: Sun May  7 21:49:38 2023, max compression
+gzip compressed data, was "dist/igv-flask-1.2.tar", last modified: Tue May  9 18:51:58 2023, max compression
```

## Comparing `igv-flask-1.1.tar` & `igv-flask-1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-07 21:49:38.000000 igv-flask-1.1/
--rw-r--r--   0 fabio      (501) staff       (20)     1068 2023-05-07 18:53:13.000000 igv-flask-1.1/LICENSE
--rw-r--r--   0 fabio      (501) staff       (20)     1443 2023-05-07 21:49:38.000000 igv-flask-1.1/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)      493 2023-05-07 21:48:53.000000 igv-flask-1.1/README.md
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-07 21:49:38.000000 igv-flask-1.1/igv/
--rw-r--r--   0 fabio      (501) staff       (20)        0 2022-07-05 20:57:40.000000 igv-flask-1.1/igv/__init__.py
--rw-r--r--   0 fabio      (501) staff       (20)     5468 2023-05-07 21:39:51.000000 igv-flask-1.1/igv/igv.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-07 21:49:38.000000 igv-flask-1.1/igv/routes/
--rw-r--r--   0 fabio      (501) staff       (20)      115 2023-05-05 04:05:16.000000 igv-flask-1.1/igv/routes/__init__.py
--rw-r--r--   0 fabio      (501) staff       (20)     1385 2023-05-06 02:43:41.000000 igv-flask-1.1/igv/routes/basics.py
--rw-r--r--   0 fabio      (501) staff       (20)     1672 2023-05-07 21:40:43.000000 igv-flask-1.1/igv/routes/web.py
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-07 21:49:38.000000 igv-flask-1.1/igv/static/
--rw-r--r--   0 fabio      (501) staff       (20)        0 2023-05-07 20:52:22.000000 igv-flask-1.1/igv/static/static
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-07 21:49:38.000000 igv-flask-1.1/igv/templates/
--rw-r--r--   0 fabio      (501) staff       (20)     1677 2023-05-07 21:41:15.000000 igv-flask-1.1/igv/templates/custom.html
--rw-r--r--   0 fabio      (501) staff       (20)     1413 2023-05-06 02:42:29.000000 igv-flask-1.1/igv/templates/demo.html
--rw-r--r--   0 fabio      (501) staff       (20)        0 2023-05-07 20:52:38.000000 igv-flask-1.1/igv/templates/templates
-drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-07 21:49:38.000000 igv-flask-1.1/igv_flask.egg-info/
--rw-r--r--   0 fabio      (501) staff       (20)     1443 2023-05-07 21:49:37.000000 igv-flask-1.1/igv_flask.egg-info/PKG-INFO
--rw-r--r--   0 fabio      (501) staff       (20)      439 2023-05-07 21:49:37.000000 igv-flask-1.1/igv_flask.egg-info/SOURCES.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-05-07 21:49:37.000000 igv-flask-1.1/igv_flask.egg-info/dependency_links.txt
--rw-r--r--   0 fabio      (501) staff       (20)       38 2023-05-07 21:49:37.000000 igv-flask-1.1/igv_flask.egg-info/entry_points.txt
--rw-r--r--   0 fabio      (501) staff       (20)        1 2023-05-07 21:49:37.000000 igv-flask-1.1/igv_flask.egg-info/not-zip-safe
--rw-r--r--   0 fabio      (501) staff       (20)       13 2023-05-07 21:49:37.000000 igv-flask-1.1/igv_flask.egg-info/requires.txt
--rw-r--r--   0 fabio      (501) staff       (20)        4 2023-05-07 21:49:37.000000 igv-flask-1.1/igv_flask.egg-info/top_level.txt
--rw-r--r--   0 fabio      (501) staff       (20)       38 2023-05-07 21:49:38.000000 igv-flask-1.1/setup.cfg
--rw-r--r--   0 fabio      (501) staff       (20)     1620 2023-05-07 20:35:44.000000 igv-flask-1.1/setup.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-09 18:51:58.000000 igv-flask-1.2/
+-rw-r--r--   0 fabio      (501) staff       (20)     1068 2023-05-07 18:53:13.000000 igv-flask-1.2/LICENSE
+-rw-r--r--   0 fabio      (501) staff       (20)     1506 2023-05-09 18:51:58.000000 igv-flask-1.2/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)      556 2023-05-09 18:39:02.000000 igv-flask-1.2/README.md
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-09 18:51:58.000000 igv-flask-1.2/igv/
+-rw-r--r--   0 fabio      (501) staff       (20)        0 2022-07-05 20:57:40.000000 igv-flask-1.2/igv/__init__.py
+-rw-r--r--   0 fabio      (501) staff       (20)     8196 2023-05-09 18:37:39.000000 igv-flask-1.2/igv/igv.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-09 18:51:58.000000 igv-flask-1.2/igv/routes/
+-rw-r--r--   0 fabio      (501) staff       (20)      115 2023-05-05 04:05:16.000000 igv-flask-1.2/igv/routes/__init__.py
+-rw-r--r--   0 fabio      (501) staff       (20)     1385 2023-05-06 02:43:41.000000 igv-flask-1.2/igv/routes/basics.py
+-rw-r--r--   0 fabio      (501) staff       (20)     1889 2023-05-09 15:30:49.000000 igv-flask-1.2/igv/routes/web.py
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-09 18:51:58.000000 igv-flask-1.2/igv/static/
+-rw-r--r--   0 fabio      (501) staff       (20)        0 2023-05-07 20:52:22.000000 igv-flask-1.2/igv/static/static
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-09 18:51:58.000000 igv-flask-1.2/igv/templates/
+-rw-r--r--   0 fabio      (501) staff       (20)     2189 2023-05-09 17:04:50.000000 igv-flask-1.2/igv/templates/custom.html
+-rw-r--r--   0 fabio      (501) staff       (20)     1413 2023-05-06 02:42:29.000000 igv-flask-1.2/igv/templates/demo.html
+-rw-r--r--   0 fabio      (501) staff       (20)        0 2023-05-07 20:52:38.000000 igv-flask-1.2/igv/templates/templates
+drwxr-xr-x   0 fabio      (501) staff       (20)        0 2023-05-09 18:51:58.000000 igv-flask-1.2/igv_flask.egg-info/
+-rw-r--r--   0 fabio      (501) staff       (20)     1506 2023-05-09 18:51:57.000000 igv-flask-1.2/igv_flask.egg-info/PKG-INFO
+-rw-r--r--   0 fabio      (501) staff       (20)      439 2023-05-09 18:51:57.000000 igv-flask-1.2/igv_flask.egg-info/SOURCES.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-05-09 18:51:57.000000 igv-flask-1.2/igv_flask.egg-info/dependency_links.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       38 2023-05-09 18:51:57.000000 igv-flask-1.2/igv_flask.egg-info/entry_points.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        1 2023-05-09 18:51:57.000000 igv-flask-1.2/igv_flask.egg-info/not-zip-safe
+-rw-r--r--   0 fabio      (501) staff       (20)       13 2023-05-09 18:51:57.000000 igv-flask-1.2/igv_flask.egg-info/requires.txt
+-rw-r--r--   0 fabio      (501) staff       (20)        4 2023-05-09 18:51:57.000000 igv-flask-1.2/igv_flask.egg-info/top_level.txt
+-rw-r--r--   0 fabio      (501) staff       (20)       38 2023-05-09 18:51:58.000000 igv-flask-1.2/setup.cfg
+-rw-r--r--   0 fabio      (501) staff       (20)     1620 2023-05-07 20:35:44.000000 igv-flask-1.2/setup.py
```

### Comparing `igv-flask-1.1/LICENSE` & `igv-flask-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `igv-flask-1.1/PKG-INFO` & `igv-flask-1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igv-flask
-Version: 1.1
+Version: 1.2
 Summary: Flask webserver for rendering igv.js
 Home-page: http://github.com/cumbof/igv-flask
 Author: Fabio Cumbo
 Author-email: fabio.cumbo@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/igv-flask/
 Project-URL: Source, https://github.com/cumbof/igv-flask
@@ -20,15 +20,15 @@
         ```
         
         ## How to start the webserver
         
         In order to start the Flask webserver and rendering `igv.js` over an input fasta file, open your terminal and run the following command:
         
         ```
-        igv --host "0.0.0.0" --port 5000 --input ~/myfasta.fna --index ~/myfasta.fai
+        igv --host "0.0.0.0" --port 5000 --input ~/myfasta.fna --index ~/myfasta.fai --cytoband ~/mycytoband.txt --tracks ~/track1.txt ~/track2.txt
         ```
         
         Run `igv --help` for a complite list of available options.
         
 Keywords: bioinformatics,visualization
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `igv-flask-1.1/igv/routes/basics.py` & `igv-flask-1.2/igv/routes/basics.py`

 * *Files identical despite different names*

### Comparing `igv-flask-1.1/igv/routes/web.py` & `igv-flask-1.2/igv/routes/web.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from flask import current_app, render_template, Response, request
 from . import blueprint
 
 
 @blueprint.route("/")
 def root_route():
-    if "input" in current_app.config and "index" in current_app.config:
+    if "input" in current_app.config:
         return web("custom")
 
     return web("demo")
 
 
 @blueprint.errorhandler(404)
 def page_not_found():
@@ -21,22 +21,28 @@
         "status": 404
     }
     js = json.dumps(err, indent=4, sort_keys=True)
     resp = Response(js, status=404, mimetype="application/json")
     return resp
 
 
-@blueprint.route("/igv/<string:page>", methods = ["GET", "POST"])
+@blueprint.route("/igv/<string:page>")
 def web(page):
     if page.strip() == "demo" or page.strip() == "index" or page.strip() == "home":
         return render_template("demo.html")
 
     elif page.strip() == "custom":
-        # An IGV session is already into config in case of --igv-session
-        return render_template("custom.html", fasta=current_app.config["input"], index=current_app.config["index"])
+        return render_template(
+            "custom.html",
+            name=os.path.splitext(current_app.config["input"])[0],
+            fasta=current_app.config["input"],
+            index=current_app.config["index"] if "index" in current_app.config else False,
+            cytoband=current_app.config["cytoband"] if "cytoband" in current_app.config else False,
+            tracks=current_app.config["tracks"] if "tracks" in current_app.config else False
+        )
 
     elif page.strip() == "session":
         igv_session = request.get_json()
 
         if "igv_session" in current_app.config:
             with open(current_app.config["igv_session"], "w+") as igv:
                 igv.write(json.dumps(igv_session))
```

### Comparing `igv-flask-1.1/igv/templates/custom.html` & `igv-flask-1.2/igv/templates/custom.html`

 * *Files 10% similar despite different names*

```diff
@@ -18,16 +18,36 @@
 
 		<script type="module">
 			var igvDiv = document.getElementById("igv-div");
 
 			var options =
 			{
 				reference: {
+					"id": "{{ name }}",
+					"name": "{{ name }}",
 					"fastaURL": "{{ url_for('static', filename=fasta) }}",
-					"indexURL": "{{ url_for('static', filename=index) }}",
+					{% if index %}
+						"indexURL": "{{ url_for('static', filename=index) }}",
+					{% else %}
+						"indexed": false,
+					{% endif %}
+					{% if cytoband %}
+						"cytobandURL": "{{ url_for('static', filename=cytoband) }}",
+					{% endif %}
+					"wholeGenomeView": true,
+					{% if tracks %}
+						"tracks": [
+							{% for track in tracks %}
+								{
+									"name": "{{ track['name'] }}",
+									"url": "{{ url_for('static', filename=track['track']) }}",
+								}
+							{% endfor %}
+						]
+					{% endif %}
 				}
 			};
 
 			igv.createBrowser(igvDiv, options)
 					.then(function (browser) {
 						{% if config.igv_session %}
 							browser.loadSessionObject(JSON.parse('{{ config["igv_session"]|tojson }}'));
```

### Comparing `igv-flask-1.1/igv/templates/demo.html` & `igv-flask-1.2/igv/templates/demo.html`

 * *Files identical despite different names*

### Comparing `igv-flask-1.1/igv_flask.egg-info/PKG-INFO` & `igv-flask-1.2/igv_flask.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igv-flask
-Version: 1.1
+Version: 1.2
 Summary: Flask webserver for rendering igv.js
 Home-page: http://github.com/cumbof/igv-flask
 Author: Fabio Cumbo
 Author-email: fabio.cumbo@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/igv-flask/
 Project-URL: Source, https://github.com/cumbof/igv-flask
@@ -20,15 +20,15 @@
         ```
         
         ## How to start the webserver
         
         In order to start the Flask webserver and rendering `igv.js` over an input fasta file, open your terminal and run the following command:
         
         ```
-        igv --host "0.0.0.0" --port 5000 --input ~/myfasta.fna --index ~/myfasta.fai
+        igv --host "0.0.0.0" --port 5000 --input ~/myfasta.fna --index ~/myfasta.fai --cytoband ~/mycytoband.txt --tracks ~/track1.txt ~/track2.txt
         ```
         
         Run `igv --help` for a complite list of available options.
         
 Keywords: bioinformatics,visualization
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `igv-flask-1.1/setup.py` & `igv-flask-1.2/setup.py`

 * *Files identical despite different names*

