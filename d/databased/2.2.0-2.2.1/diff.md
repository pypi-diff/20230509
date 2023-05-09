# Comparing `tmp/databased-2.2.0.tar.gz` & `tmp/databased-2.2.1.tar.gz`

## Comparing `databased-2.2.0.tar` & `databased-2.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     6245 2020-02-02 00:00:00.000000 databased-2.2.0/CHANGELOG.md
--rw-r--r--   0        0        0    34933 2020-02-02 00:00:00.000000 databased-2.2.0/docs/databased.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-2.2.0/docs/index.html
--rw-r--r--   0        0        0    67193 2020-02-02 00:00:00.000000 databased-2.2.0/docs/search.js
--rw-r--r--   0        0        0    44745 2020-02-02 00:00:00.000000 databased-2.2.0/docs/databased/customshell.html
--rw-r--r--   0        0        0   445562 2020-02-02 00:00:00.000000 databased-2.2.0/docs/databased/databased.html
--rw-r--r--   0        0        0   127332 2020-02-02 00:00:00.000000 databased-2.2.0/docs/databased/dbparsers.html
--rw-r--r--   0        0        0   314278 2020-02-02 00:00:00.000000 databased-2.2.0/docs/databased/dbshell.html
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 databased-2.2.0/src/databased/__init__.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 databased-2.2.0/src/databased/customshell.py
--rw-r--r--   0        0        0    23516 2020-02-02 00:00:00.000000 databased-2.2.0/src/databased/databased.py
--rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 databased-2.2.0/src/databased/dbparsers.py
--rw-r--r--   0        0        0    14071 2020-02-02 00:00:00.000000 databased-2.2.0/src/databased/dbshell.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-2.2.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-2.2.0/LICENSE.txt
--rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 databased-2.2.0/README.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 databased-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 databased-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 databased-2.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0    34933 2020-02-02 00:00:00.000000 databased-2.2.1/docs/databased.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 databased-2.2.1/docs/index.html
+-rw-r--r--   0        0        0    67193 2020-02-02 00:00:00.000000 databased-2.2.1/docs/search.js
+-rw-r--r--   0        0        0    44745 2020-02-02 00:00:00.000000 databased-2.2.1/docs/databased/customshell.html
+-rw-r--r--   0        0        0   445565 2020-02-02 00:00:00.000000 databased-2.2.1/docs/databased/databased.html
+-rw-r--r--   0        0        0   127332 2020-02-02 00:00:00.000000 databased-2.2.1/docs/databased/dbparsers.html
+-rw-r--r--   0        0        0   315998 2020-02-02 00:00:00.000000 databased-2.2.1/docs/databased/dbshell.html
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 databased-2.2.1/src/databased/__init__.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 databased-2.2.1/src/databased/customshell.py
+-rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 databased-2.2.1/src/databased/databased.py
+-rw-r--r--   0        0        0     7079 2020-02-02 00:00:00.000000 databased-2.2.1/src/databased/dbparsers.py
+-rw-r--r--   0        0        0    14140 2020-02-02 00:00:00.000000 databased-2.2.1/src/databased/dbshell.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 databased-2.2.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 databased-2.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     7480 2020-02-02 00:00:00.000000 databased-2.2.1/README.md
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 databased-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 databased-2.2.1/PKG-INFO
```

### Comparing `databased-2.2.0/CHANGELOG.md` & `databased-2.2.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 # Changelog
 
-## 2.1.0 (2023-05-08)
+## 2.2.0 (2023-05-08)
+
+#### New Features
+
+* add timestamp option to dbshell backup command
+
+## v2.1.0 (2023-05-08)
 
 #### New Features
 
 * add _disconnect decorator
 * add vacuum()
 * add connection_timeout property
+#### Others
+
+* build v2.1.0
+* update changelog
 
 
 ## v2.0.1 (2023-05-07)
 
 #### Fixes
 
 * wrap table names in query statements in [] so things like colons don't trigger syntax errors
```

### Comparing `databased-2.2.0/docs/databased.html` & `databased-2.2.1/docs/databased.html`

 * *Files identical despite different names*

### Comparing `databased-2.2.0/docs/search.js` & `databased-2.2.1/docs/search.js`

 * *Files identical despite different names*

### Comparing `databased-2.2.0/docs/databased/customshell.html` & `databased-2.2.1/docs/databased/customshell.html`

 * *Files identical despite different names*

### Comparing `databased-2.2.0/docs/databased/databased.html` & `databased-2.2.1/docs/databased/databased.html`

 * *Files 0% similar despite different names*

```diff
@@ -302,15 +302,15 @@
 </span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; like &quot;%</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">%&quot;&#39;</span>
 </span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
 </span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>            <span class="p">)</span>
 </span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">)&quot;</span>
 </span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
 </span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="k">def</span> <span class="nf">vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 </span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>        <span class="sd">&quot;&quot;&quot;Reduce disk size of the database with a `VACUUM` query.&quot;&quot;&quot;</span>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="s2">&quot;VACUUM&quot;</span><span class="p">)</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="s2">&quot;VACUUM;&quot;</span><span class="p">)</span>
 </span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
 </span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>    <span class="nd">@_connect</span>
 </span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
 </span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and return the results.&quot;&quot;&quot;</span>
 </span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
 </span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
 </span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
@@ -912,15 +912,15 @@
 </span><span id="DataBased-184"><a href="#DataBased-184"><span class="linenos">184</span></a>                <span class="sa">f</span><span class="s1">&#39;&quot;</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="si">}</span><span class="s1">&quot; like &quot;%</span><span class="si">{</span><span class="n">column_row</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="si">}</span><span class="s1">%&quot;&#39;</span>
 </span><span id="DataBased-185"><a href="#DataBased-185"><span class="linenos">185</span></a>                <span class="k">for</span> <span class="n">column_row</span> <span class="ow">in</span> <span class="n">match_criteria</span>
 </span><span id="DataBased-186"><a href="#DataBased-186"><span class="linenos">186</span></a>            <span class="p">)</span>
 </span><span id="DataBased-187"><a href="#DataBased-187"><span class="linenos">187</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">conditions</span><span class="si">}</span><span class="s2">)&quot;</span>
 </span><span id="DataBased-188"><a href="#DataBased-188"><span class="linenos">188</span></a>
 </span><span id="DataBased-189"><a href="#DataBased-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 </span><span id="DataBased-190"><a href="#DataBased-190"><span class="linenos">190</span></a>        <span class="sd">&quot;&quot;&quot;Reduce disk size of the database with a `VACUUM` query.&quot;&quot;&quot;</span>
-</span><span id="DataBased-191"><a href="#DataBased-191"><span class="linenos">191</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="s2">&quot;VACUUM&quot;</span><span class="p">)</span>
+</span><span id="DataBased-191"><a href="#DataBased-191"><span class="linenos">191</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="s2">&quot;VACUUM;&quot;</span><span class="p">)</span>
 </span><span id="DataBased-192"><a href="#DataBased-192"><span class="linenos">192</span></a>
 </span><span id="DataBased-193"><a href="#DataBased-193"><span class="linenos">193</span></a>    <span class="nd">@_connect</span>
 </span><span id="DataBased-194"><a href="#DataBased-194"><span class="linenos">194</span></a>    <span class="k">def</span> <span class="nf">query</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">query_</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="n">Any</span><span class="p">]:</span>
 </span><span id="DataBased-195"><a href="#DataBased-195"><span class="linenos">195</span></a>        <span class="sd">&quot;&quot;&quot;Execute an arbitrary query and return the results.&quot;&quot;&quot;</span>
 </span><span id="DataBased-196"><a href="#DataBased-196"><span class="linenos">196</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span><span class="n">query_</span><span class="p">)</span>
 </span><span id="DataBased-197"><a href="#DataBased-197"><span class="linenos">197</span></a>        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">cursor</span><span class="o">.</span><span class="n">fetchall</span><span class="p">()</span>
 </span><span id="DataBased-198"><a href="#DataBased-198"><span class="linenos">198</span></a>
@@ -1430,15 +1430,15 @@
 
                 <label class="view-source-button" for="DataBased.vacuum-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DataBased.vacuum"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="DataBased.vacuum-189"><a href="#DataBased.vacuum-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
 </span><span id="DataBased.vacuum-190"><a href="#DataBased.vacuum-190"><span class="linenos">190</span></a>        <span class="sd">&quot;&quot;&quot;Reduce disk size of the database with a `VACUUM` query.&quot;&quot;&quot;</span>
-</span><span id="DataBased.vacuum-191"><a href="#DataBased.vacuum-191"><span class="linenos">191</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="s2">&quot;VACUUM&quot;</span><span class="p">)</span>
+</span><span id="DataBased.vacuum-191"><a href="#DataBased.vacuum-191"><span class="linenos">191</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">query</span><span class="p">(</span><span class="s2">&quot;VACUUM;&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Reduce disk size of the database with a <code>VACUUM</code> query.</p>
 </div>
```

#### html2text {}

```diff
@@ -226,15 +226,15 @@
 183                f'"{column_row[0]}" like "%{column_row[1]}%"'
 184                for column_row in match_criteria
 185            )
 186        return f"({conditions})"
 187
 188    def vacuum(self):
 189        """Reduce disk size of the database with a `VACUUM` query."""
-190        self.query("VACUUM")
+190        self.query("VACUUM;")
 191
 192    @_connect
 193    def query(self, query_) -> list[Any]:
 194        """Execute an arbitrary query and return the results."""
 195        self.cursor.execute(query_)
 196        return self.cursor.fetchall()
 197
@@ -883,15 +883,15 @@
 184                f'"{column_row[0]}" like "%{column_row[1]}%"'
 185                for column_row in match_criteria
 186            )
 187        return f"({conditions})"
 188
 189    def vacuum(self):
 190        """Reduce disk size of the database with a `VACUUM` query."""
-191        self.query("VACUUM")
+191        self.query("VACUUM;")
 192
 193    @_connect
 194    def query(self, query_) -> list[Any]:
 195        """Execute an arbitrary query and return the results."""
 196        self.cursor.execute(query_)
 197        return self.cursor.fetchall()
 198
@@ -1383,15 +1383,15 @@
 Save and close connection to db.
 Call this as soon as you are done using the database if you have multiple
 threads or processes using the same database.
 ⁰
 def vacuum(self): View Source
 189    def vacuum(self):
 190        """Reduce disk size of the database with a `VACUUM` query."""
-191        self.query("VACUUM")
+191        self.query("VACUUM;")
 Reduce disk size of the database with a VACUUM query.
 ⁰
 def query(self, query_) -> list[typing.Any]: View Source
 193    @_connect
 194    def query(self, query_) -> list[Any]:
 195        """Execute an arbitrary query and return the results."""
 196        self.cursor.execute(query_)
```

### Comparing `databased-2.2.0/docs/databased/dbparsers.html` & `databased-2.2.1/docs/databased/dbparsers.html`

 * *Files identical despite different names*

### Comparing `databased-2.2.0/docs/databased/dbshell.html` & `databased-2.2.1/docs/databased/dbshell.html`

 * *Files 0% similar despite different names*

```diff
@@ -357,76 +357,78 @@
 </span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
 </span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>
 </span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
 </span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
 </span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>            <span class="p">)</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>                    <span class="k">continue</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>                <span class="p">)</span>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
-</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
-</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
-</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>
-</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>
-</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>            <span class="p">)</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>                    <span class="k">continue</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>                <span class="p">)</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
+</span><span id="L-298"><a href="#L-298"><span class="linenos">298</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-299"><a href="#L-299"><span class="linenos">299</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="L-300"><a href="#L-300"><span class="linenos">300</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="L-301"><a href="#L-301"><span class="linenos">301</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+</span><span id="L-302"><a href="#L-302"><span class="linenos">302</span></a>
+</span><span id="L-303"><a href="#L-303"><span class="linenos">303</span></a>
+</span><span id="L-304"><a href="#L-304"><span class="linenos">304</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="L-305"><a href="#L-305"><span class="linenos">305</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
                 <section id="DBShell">
                             <input id="DBShell-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr class">
@@ -669,72 +671,74 @@
 </span><span id="DBShell-236"><a href="#DBShell-236"><span class="linenos">236</span></a>            <span class="n">custom_file</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">content</span><span class="p">)</span>
 </span><span id="DBShell-237"><a href="#DBShell-237"><span class="linenos">237</span></a>
 </span><span id="DBShell-238"><a href="#DBShell-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="DBShell-239"><a href="#DBShell-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
 </span><span id="DBShell-240"><a href="#DBShell-240"><span class="linenos">240</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
 </span><span id="DBShell-241"><a href="#DBShell-241"><span class="linenos">241</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="DBShell-242"><a href="#DBShell-242"><span class="linenos">242</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-243"><a href="#DBShell-243"><span class="linenos">243</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-244"><a href="#DBShell-244"><span class="linenos">244</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="DBShell-245"><a href="#DBShell-245"><span class="linenos">245</span></a>
-</span><span id="DBShell-246"><a href="#DBShell-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
-</span><span id="DBShell-247"><a href="#DBShell-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
-</span><span id="DBShell-248"><a href="#DBShell-248"><span class="linenos">248</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell-249"><a href="#DBShell-249"><span class="linenos">249</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
-</span><span id="DBShell-250"><a href="#DBShell-250"><span class="linenos">250</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
-</span><span id="DBShell-251"><a href="#DBShell-251"><span class="linenos">251</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="DBShell-252"><a href="#DBShell-252"><span class="linenos">252</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="DBShell-253"><a href="#DBShell-253"><span class="linenos">253</span></a>            <span class="p">)</span>
-</span><span id="DBShell-254"><a href="#DBShell-254"><span class="linenos">254</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
-</span><span id="DBShell-255"><a href="#DBShell-255"><span class="linenos">255</span></a>            <span class="k">try</span><span class="p">:</span>
-</span><span id="DBShell-256"><a href="#DBShell-256"><span class="linenos">256</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
-</span><span id="DBShell-257"><a href="#DBShell-257"><span class="linenos">257</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
-</span><span id="DBShell-258"><a href="#DBShell-258"><span class="linenos">258</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-259"><a href="#DBShell-259"><span class="linenos">259</span></a>                    <span class="k">continue</span>
-</span><span id="DBShell-260"><a href="#DBShell-260"><span class="linenos">260</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
-</span><span id="DBShell-261"><a href="#DBShell-261"><span class="linenos">261</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="DBShell-262"><a href="#DBShell-262"><span class="linenos">262</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-263"><a href="#DBShell-263"><span class="linenos">263</span></a>
-</span><span id="DBShell-264"><a href="#DBShell-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DBShell-265"><a href="#DBShell-265"><span class="linenos">265</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
-</span><span id="DBShell-266"><a href="#DBShell-266"><span class="linenos">266</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
-</span><span id="DBShell-267"><a href="#DBShell-267"><span class="linenos">267</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
-</span><span id="DBShell-268"><a href="#DBShell-268"><span class="linenos">268</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DBShell-269"><a href="#DBShell-269"><span class="linenos">269</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell-270"><a href="#DBShell-270"><span class="linenos">270</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-271"><a href="#DBShell-271"><span class="linenos">271</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-272"><a href="#DBShell-272"><span class="linenos">272</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell-273"><a href="#DBShell-273"><span class="linenos">273</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell-274"><a href="#DBShell-274"><span class="linenos">274</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell-275"><a href="#DBShell-275"><span class="linenos">275</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell-276"><a href="#DBShell-276"><span class="linenos">276</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-277"><a href="#DBShell-277"><span class="linenos">277</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell-278"><a href="#DBShell-278"><span class="linenos">278</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell-279"><a href="#DBShell-279"><span class="linenos">279</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-280"><a href="#DBShell-280"><span class="linenos">280</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-281"><a href="#DBShell-281"><span class="linenos">281</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
-</span><span id="DBShell-282"><a href="#DBShell-282"><span class="linenos">282</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
-</span><span id="DBShell-283"><a href="#DBShell-283"><span class="linenos">283</span></a>                <span class="p">)</span>
-</span><span id="DBShell-284"><a href="#DBShell-284"><span class="linenos">284</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell-285"><a href="#DBShell-285"><span class="linenos">285</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="DBShell-286"><a href="#DBShell-286"><span class="linenos">286</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell-287"><a href="#DBShell-287"><span class="linenos">287</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
-</span><span id="DBShell-288"><a href="#DBShell-288"><span class="linenos">288</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell-289"><a href="#DBShell-289"><span class="linenos">289</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell-290"><a href="#DBShell-290"><span class="linenos">290</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell-291"><a href="#DBShell-291"><span class="linenos">291</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-292"><a href="#DBShell-292"><span class="linenos">292</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell-293"><a href="#DBShell-293"><span class="linenos">293</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell-294"><a href="#DBShell-294"><span class="linenos">294</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell-295"><a href="#DBShell-295"><span class="linenos">295</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-296"><a href="#DBShell-296"><span class="linenos">296</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
-</span><span id="DBShell-297"><a href="#DBShell-297"><span class="linenos">297</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell-298"><a href="#DBShell-298"><span class="linenos">298</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="DBShell-299"><a href="#DBShell-299"><span class="linenos">299</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="DBShell-300"><a href="#DBShell-300"><span class="linenos">300</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-243"><a href="#DBShell-243"><span class="linenos">243</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell-244"><a href="#DBShell-244"><span class="linenos">244</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
+</span><span id="DBShell-245"><a href="#DBShell-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-246"><a href="#DBShell-246"><span class="linenos">246</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="DBShell-247"><a href="#DBShell-247"><span class="linenos">247</span></a>
+</span><span id="DBShell-248"><a href="#DBShell-248"><span class="linenos">248</span></a>    <span class="k">def</span> <span class="nf">_choose_db</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">options</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="n">Pathier</span><span class="p">:</span>
+</span><span id="DBShell-249"><a href="#DBShell-249"><span class="linenos">249</span></a>        <span class="sd">&quot;&quot;&quot;Prompt the user to select from a list of files.&quot;&quot;&quot;</span>
+</span><span id="DBShell-250"><a href="#DBShell-250"><span class="linenos">250</span></a>        <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell-251"><a href="#DBShell-251"><span class="linenos">251</span></a>        <span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="o">.</span><span class="n">separate</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">options</span><span class="p">]</span>
+</span><span id="DBShell-252"><a href="#DBShell-252"><span class="linenos">252</span></a>        <span class="k">while</span> <span class="kc">True</span><span class="p">:</span>
+</span><span id="DBShell-253"><a href="#DBShell-253"><span class="linenos">253</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="DBShell-254"><a href="#DBShell-254"><span class="linenos">254</span></a>                <span class="sa">f</span><span class="s2">&quot;DB options:</span><span class="se">\n</span><span class="si">{</span><span class="s1">&#39; &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="sa">f</span><span class="s1">&#39;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s1">) </span><span class="si">{</span><span class="n">path</span><span class="si">}</span><span class="s1">&#39;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span><span class="n">path</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">paths</span><span class="p">,</span><span class="mi">1</span><span class="p">)])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="DBShell-255"><a href="#DBShell-255"><span class="linenos">255</span></a>            <span class="p">)</span>
+</span><span id="DBShell-256"><a href="#DBShell-256"><span class="linenos">256</span></a>            <span class="n">choice</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter the number of the option to use: &quot;</span><span class="p">)</span>
+</span><span id="DBShell-257"><a href="#DBShell-257"><span class="linenos">257</span></a>            <span class="k">try</span><span class="p">:</span>
+</span><span id="DBShell-258"><a href="#DBShell-258"><span class="linenos">258</span></a>                <span class="n">index</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">choice</span><span class="p">)</span>
+</span><span id="DBShell-259"><a href="#DBShell-259"><span class="linenos">259</span></a>                <span class="k">if</span> <span class="ow">not</span> <span class="mi">1</span> <span class="o">&lt;=</span> <span class="n">index</span> <span class="o">&lt;=</span> <span class="nb">len</span><span class="p">(</span><span class="n">options</span><span class="p">):</span>
+</span><span id="DBShell-260"><a href="#DBShell-260"><span class="linenos">260</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Choice out of range.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-261"><a href="#DBShell-261"><span class="linenos">261</span></a>                    <span class="k">continue</span>
+</span><span id="DBShell-262"><a href="#DBShell-262"><span class="linenos">262</span></a>                <span class="k">return</span> <span class="n">options</span><span class="p">[</span><span class="n">index</span> <span class="o">-</span> <span class="mi">1</span><span class="p">]</span>
+</span><span id="DBShell-263"><a href="#DBShell-263"><span class="linenos">263</span></a>            <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="DBShell-264"><a href="#DBShell-264"><span class="linenos">264</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">choice</span><span class="si">}</span><span class="s2"> is not a valid option.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-265"><a href="#DBShell-265"><span class="linenos">265</span></a>
+</span><span id="DBShell-266"><a href="#DBShell-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DBShell-267"><a href="#DBShell-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
+</span><span id="DBShell-268"><a href="#DBShell-268"><span class="linenos">268</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
+</span><span id="DBShell-269"><a href="#DBShell-269"><span class="linenos">269</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
+</span><span id="DBShell-270"><a href="#DBShell-270"><span class="linenos">270</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DBShell-271"><a href="#DBShell-271"><span class="linenos">271</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell-272"><a href="#DBShell-272"><span class="linenos">272</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-273"><a href="#DBShell-273"><span class="linenos">273</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-274"><a href="#DBShell-274"><span class="linenos">274</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell-275"><a href="#DBShell-275"><span class="linenos">275</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell-276"><a href="#DBShell-276"><span class="linenos">276</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell-277"><a href="#DBShell-277"><span class="linenos">277</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell-278"><a href="#DBShell-278"><span class="linenos">278</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-279"><a href="#DBShell-279"><span class="linenos">279</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell-280"><a href="#DBShell-280"><span class="linenos">280</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell-281"><a href="#DBShell-281"><span class="linenos">281</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-282"><a href="#DBShell-282"><span class="linenos">282</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-283"><a href="#DBShell-283"><span class="linenos">283</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
+</span><span id="DBShell-284"><a href="#DBShell-284"><span class="linenos">284</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
+</span><span id="DBShell-285"><a href="#DBShell-285"><span class="linenos">285</span></a>                <span class="p">)</span>
+</span><span id="DBShell-286"><a href="#DBShell-286"><span class="linenos">286</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell-287"><a href="#DBShell-287"><span class="linenos">287</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="DBShell-288"><a href="#DBShell-288"><span class="linenos">288</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell-289"><a href="#DBShell-289"><span class="linenos">289</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
+</span><span id="DBShell-290"><a href="#DBShell-290"><span class="linenos">290</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell-291"><a href="#DBShell-291"><span class="linenos">291</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell-292"><a href="#DBShell-292"><span class="linenos">292</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell-293"><a href="#DBShell-293"><span class="linenos">293</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-294"><a href="#DBShell-294"><span class="linenos">294</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell-295"><a href="#DBShell-295"><span class="linenos">295</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell-296"><a href="#DBShell-296"><span class="linenos">296</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell-297"><a href="#DBShell-297"><span class="linenos">297</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-298"><a href="#DBShell-298"><span class="linenos">298</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
+</span><span id="DBShell-299"><a href="#DBShell-299"><span class="linenos">299</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell-300"><a href="#DBShell-300"><span class="linenos">300</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="DBShell-301"><a href="#DBShell-301"><span class="linenos">301</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="DBShell-302"><a href="#DBShell-302"><span class="linenos">302</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Subclass this to create custom ArgShells.</p>
 </div>
 
 
@@ -1345,16 +1349,18 @@
     </div>
     <a class="headerlink" href="#DBShell.do_vacuum"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.do_vacuum-238"><a href="#DBShell.do_vacuum-238"><span class="linenos">238</span></a>    <span class="k">def</span> <span class="nf">do_vacuum</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="DBShell.do_vacuum-239"><a href="#DBShell.do_vacuum-239"><span class="linenos">239</span></a>        <span class="sd">&quot;&quot;&quot;Reduce database disk memory.&quot;&quot;&quot;</span>
 </span><span id="DBShell.do_vacuum-240"><a href="#DBShell.do_vacuum-240"><span class="linenos">240</span></a>        <span class="n">starting_size</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
 </span><span id="DBShell.do_vacuum-241"><a href="#DBShell.do_vacuum-241"><span class="linenos">241</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size before vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="DBShell.do_vacuum-242"><a href="#DBShell.do_vacuum-242"><span class="linenos">242</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Vacuuming database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_vacuum-243"><a href="#DBShell.do_vacuum-243"><span class="linenos">243</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.do_vacuum-244"><a href="#DBShell.do_vacuum-244"><span class="linenos">244</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="DBShell.do_vacuum-243"><a href="#DBShell.do_vacuum-243"><span class="linenos">243</span></a>        <span class="k">with</span> <span class="n">DataBased</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span> <span class="k">as</span> <span class="n">db</span><span class="p">:</span>
+</span><span id="DBShell.do_vacuum-244"><a href="#DBShell.do_vacuum-244"><span class="linenos">244</span></a>            <span class="n">db</span><span class="o">.</span><span class="n">vacuum</span><span class="p">()</span>
+</span><span id="DBShell.do_vacuum-245"><a href="#DBShell.do_vacuum-245"><span class="linenos">245</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Database size after vacuuming: </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">(</span><span class="kc">True</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.do_vacuum-246"><a href="#DBShell.do_vacuum-246"><span class="linenos">246</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Freed up </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">starting_size</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">size</span><span class="p">())</span><span class="si">}</span><span class="s2"> of disk space.&quot;</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Reduce database disk memory.</p>
 </div>
 
 
@@ -1366,51 +1372,51 @@
         <span class="def">def</span>
         <span class="name">preloop</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="DBShell.preloop-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#DBShell.preloop"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.preloop-264"><a href="#DBShell.preloop-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="DBShell.preloop-265"><a href="#DBShell.preloop-265"><span class="linenos">265</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
-</span><span id="DBShell.preloop-266"><a href="#DBShell.preloop-266"><span class="linenos">266</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
-</span><span id="DBShell.preloop-267"><a href="#DBShell.preloop-267"><span class="linenos">267</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
-</span><span id="DBShell.preloop-268"><a href="#DBShell.preloop-268"><span class="linenos">268</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
-</span><span id="DBShell.preloop-269"><a href="#DBShell.preloop-269"><span class="linenos">269</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-270"><a href="#DBShell.preloop-270"><span class="linenos">270</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.preloop-271"><a href="#DBShell.preloop-271"><span class="linenos">271</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-272"><a href="#DBShell.preloop-272"><span class="linenos">272</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="DBShell.preloop-273"><a href="#DBShell.preloop-273"><span class="linenos">273</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell.preloop-274"><a href="#DBShell.preloop-274"><span class="linenos">274</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell.preloop-275"><a href="#DBShell.preloop-275"><span class="linenos">275</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell.preloop-276"><a href="#DBShell.preloop-276"><span class="linenos">276</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-277"><a href="#DBShell.preloop-277"><span class="linenos">277</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell.preloop-278"><a href="#DBShell.preloop-278"><span class="linenos">278</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell.preloop-279"><a href="#DBShell.preloop-279"><span class="linenos">279</span></a>            <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.preloop-280"><a href="#DBShell.preloop-280"><span class="linenos">280</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-281"><a href="#DBShell.preloop-281"><span class="linenos">281</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
-</span><span id="DBShell.preloop-282"><a href="#DBShell.preloop-282"><span class="linenos">282</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
-</span><span id="DBShell.preloop-283"><a href="#DBShell.preloop-283"><span class="linenos">283</span></a>                <span class="p">)</span>
-</span><span id="DBShell.preloop-284"><a href="#DBShell.preloop-284"><span class="linenos">284</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell.preloop-285"><a href="#DBShell.preloop-285"><span class="linenos">285</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="DBShell.preloop-286"><a href="#DBShell.preloop-286"><span class="linenos">286</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
-</span><span id="DBShell.preloop-287"><a href="#DBShell.preloop-287"><span class="linenos">287</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-288"><a href="#DBShell.preloop-288"><span class="linenos">288</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
-</span><span id="DBShell.preloop-289"><a href="#DBShell.preloop-289"><span class="linenos">289</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
-</span><span id="DBShell.preloop-290"><a href="#DBShell.preloop-290"><span class="linenos">290</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
-</span><span id="DBShell.preloop-291"><a href="#DBShell.preloop-291"><span class="linenos">291</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-292"><a href="#DBShell.preloop-292"><span class="linenos">292</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
-</span><span id="DBShell.preloop-293"><a href="#DBShell.preloop-293"><span class="linenos">293</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
-</span><span id="DBShell.preloop-294"><a href="#DBShell.preloop-294"><span class="linenos">294</span></a>                    <span class="k">else</span><span class="p">:</span>
-</span><span id="DBShell.preloop-295"><a href="#DBShell.preloop-295"><span class="linenos">295</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-296"><a href="#DBShell.preloop-296"><span class="linenos">296</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
-</span><span id="DBShell.preloop-297"><a href="#DBShell.preloop-297"><span class="linenos">297</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="DBShell.preloop-298"><a href="#DBShell.preloop-298"><span class="linenos">298</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
-</span><span id="DBShell.preloop-299"><a href="#DBShell.preloop-299"><span class="linenos">299</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="DBShell.preloop-300"><a href="#DBShell.preloop-300"><span class="linenos">300</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="DBShell.preloop-266"><a href="#DBShell.preloop-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">preloop</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+</span><span id="DBShell.preloop-267"><a href="#DBShell.preloop-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Scan the current directory for a .db file to use.</span>
+</span><span id="DBShell.preloop-268"><a href="#DBShell.preloop-268"><span class="linenos">268</span></a><span class="sd">        If not found, prompt the user for one or to try again recursively.&quot;&quot;&quot;</span>
+</span><span id="DBShell.preloop-269"><a href="#DBShell.preloop-269"><span class="linenos">269</span></a>        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">:</span>
+</span><span id="DBShell.preloop-270"><a href="#DBShell.preloop-270"><span class="linenos">270</span></a>            <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="p">)</span>
+</span><span id="DBShell.preloop-271"><a href="#DBShell.preloop-271"><span class="linenos">271</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Defaulting to database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-272"><a href="#DBShell.preloop-272"><span class="linenos">272</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.preloop-273"><a href="#DBShell.preloop-273"><span class="linenos">273</span></a>            <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching for database...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-274"><a href="#DBShell.preloop-274"><span class="linenos">274</span></a>            <span class="n">cwd</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="DBShell.preloop-275"><a href="#DBShell.preloop-275"><span class="linenos">275</span></a>            <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell.preloop-276"><a href="#DBShell.preloop-276"><span class="linenos">276</span></a>            <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell.preloop-277"><a href="#DBShell.preloop-277"><span class="linenos">277</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell.preloop-278"><a href="#DBShell.preloop-278"><span class="linenos">278</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-279"><a href="#DBShell.preloop-279"><span class="linenos">279</span></a>            <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell.preloop-280"><a href="#DBShell.preloop-280"><span class="linenos">280</span></a>                <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell.preloop-281"><a href="#DBShell.preloop-281"><span class="linenos">281</span></a>            <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.preloop-282"><a href="#DBShell.preloop-282"><span class="linenos">282</span></a>                <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Could not find a .db file in </span><span class="si">{</span><span class="n">cwd</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-283"><a href="#DBShell.preloop-283"><span class="linenos">283</span></a>                <span class="n">path</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span>
+</span><span id="DBShell.preloop-284"><a href="#DBShell.preloop-284"><span class="linenos">284</span></a>                    <span class="s2">&quot;Enter path to .db file to use or press enter to search again recursively: &quot;</span>
+</span><span id="DBShell.preloop-285"><a href="#DBShell.preloop-285"><span class="linenos">285</span></a>                <span class="p">)</span>
+</span><span id="DBShell.preloop-286"><a href="#DBShell.preloop-286"><span class="linenos">286</span></a>                <span class="k">if</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell.preloop-287"><a href="#DBShell.preloop-287"><span class="linenos">287</span></a>                    <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="DBShell.preloop-288"><a href="#DBShell.preloop-288"><span class="linenos">288</span></a>                <span class="k">elif</span> <span class="ow">not</span> <span class="n">path</span><span class="p">:</span>
+</span><span id="DBShell.preloop-289"><a href="#DBShell.preloop-289"><span class="linenos">289</span></a>                    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Searching recursively...&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-290"><a href="#DBShell.preloop-290"><span class="linenos">290</span></a>                    <span class="n">dbs</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">cwd</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.db&quot;</span><span class="p">))</span>
+</span><span id="DBShell.preloop-291"><a href="#DBShell.preloop-291"><span class="linenos">291</span></a>                    <span class="k">if</span> <span class="nb">len</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span> <span class="o">==</span> <span class="mi">1</span><span class="p">:</span>
+</span><span id="DBShell.preloop-292"><a href="#DBShell.preloop-292"><span class="linenos">292</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">dbs</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+</span><span id="DBShell.preloop-293"><a href="#DBShell.preloop-293"><span class="linenos">293</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Using database </span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-294"><a href="#DBShell.preloop-294"><span class="linenos">294</span></a>                    <span class="k">elif</span> <span class="n">dbs</span><span class="p">:</span>
+</span><span id="DBShell.preloop-295"><a href="#DBShell.preloop-295"><span class="linenos">295</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_choose_db</span><span class="p">(</span><span class="n">dbs</span><span class="p">)</span>
+</span><span id="DBShell.preloop-296"><a href="#DBShell.preloop-296"><span class="linenos">296</span></a>                    <span class="k">else</span><span class="p">:</span>
+</span><span id="DBShell.preloop-297"><a href="#DBShell.preloop-297"><span class="linenos">297</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Could not find a .db file.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-298"><a href="#DBShell.preloop-298"><span class="linenos">298</span></a>                        <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="nb">input</span><span class="p">(</span><span class="s2">&quot;Enter path to a .db file: &quot;</span><span class="p">))</span>
+</span><span id="DBShell.preloop-299"><a href="#DBShell.preloop-299"><span class="linenos">299</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="DBShell.preloop-300"><a href="#DBShell.preloop-300"><span class="linenos">300</span></a>            <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> does not exist.&quot;</span><span class="p">)</span>
+</span><span id="DBShell.preloop-301"><a href="#DBShell.preloop-301"><span class="linenos">301</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="DBShell.preloop-302"><a href="#DBShell.preloop-302"><span class="linenos">302</span></a>            <span class="k">raise</span> <span class="ne">ValueError</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">dbpath</span><span class="si">}</span><span class="s2"> is not a file.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Scan the current directory for a .db file to use.
 If not found, prompt the user for one or to try again recursively.</p>
 </div>
 
@@ -1454,16 +1460,16 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-303"><a href="#main-303"><span class="linenos">303</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="main-304"><a href="#main-304"><span class="linenos">304</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-305"><a href="#main-305"><span class="linenos">305</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="main-306"><a href="#main-306"><span class="linenos">306</span></a>    <span class="n">DBShell</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -297,81 +297,83 @@
 235            custom_file.write_text(content)
 236
 237    def do_vacuum(self, arg: str):
 238        """Reduce database disk memory."""
 239        starting_size = self.dbpath.size()
 240        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
 241        print("Vacuuming database...")
-242        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-243        print(f"Freed up {Pathier.format_size(starting_size -
+242        with DataBased(self.dbpath) as db:
+243            db.vacuum()
+244        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
+245        print(f"Freed up {Pathier.format_size(starting_size -
 self.dbpath.size())} of disk space.")  # type: ignore
-244
-245    def _choose_db(self, options: list[Pathier]) -> Pathier:
-246        """Prompt the user to select from a list of files."""
-247        cwd = Pathier.cwd()
-248        paths = [path.separate(cwd.stem) for path in options]
-249        while True:
-250            print(
-251                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
+246
+247    def _choose_db(self, options: list[Pathier]) -> Pathier:
+248        """Prompt the user to select from a list of files."""
+249        cwd = Pathier.cwd()
+250        paths = [path.separate(cwd.stem) for path in options]
+251        while True:
+252            print(
+253                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
 enumerate(paths,1)])}"
-252            )
-253            choice = input("Enter the number of the option to use: ")
-254            try:
-255                index = int(choice)
-256                if not 1 <= index <= len(options):
-257                    print("Choice out of range.")
-258                    continue
-259                return options[index - 1]
-260            except Exception as e:
-261                print(f"{choice} is not a valid option.")
-262
-263    def preloop(self):
-264        """Scan the current directory for a .db file to use.
-265        If not found, prompt the user for one or to try again
+254            )
+255            choice = input("Enter the number of the option to use: ")
+256            try:
+257                index = int(choice)
+258                if not 1 <= index <= len(options):
+259                    print("Choice out of range.")
+260                    continue
+261                return options[index - 1]
+262            except Exception as e:
+263                print(f"{choice} is not a valid option.")
+264
+265    def preloop(self):
+266        """Scan the current directory for a .db file to use.
+267        If not found, prompt the user for one or to try again
 recursively."""
-266        if self.dbpath:
-267            self.dbpath = Pathier(self.dbpath)
-268            print(f"Defaulting to database {self.dbpath}")
-269        else:
-270            print("Searching for database...")
-271            cwd = Pathier.cwd()
-272            dbs = list(cwd.glob("*.db"))
-273            if len(dbs) == 1:
-274                self.dbpath = dbs[0]
-275                print(f"Using database {self.dbpath}.")
-276            elif dbs:
-277                self.dbpath = self._choose_db(dbs)
-278            else:
-279                print(f"Could not find a .db file in {cwd}.")
-280                path = input(
-281                    "Enter path to .db file to use or press enter to search
+268        if self.dbpath:
+269            self.dbpath = Pathier(self.dbpath)
+270            print(f"Defaulting to database {self.dbpath}")
+271        else:
+272            print("Searching for database...")
+273            cwd = Pathier.cwd()
+274            dbs = list(cwd.glob("*.db"))
+275            if len(dbs) == 1:
+276                self.dbpath = dbs[0]
+277                print(f"Using database {self.dbpath}.")
+278            elif dbs:
+279                self.dbpath = self._choose_db(dbs)
+280            else:
+281                print(f"Could not find a .db file in {cwd}.")
+282                path = input(
+283                    "Enter path to .db file to use or press enter to search
 again recursively: "
-282                )
-283                if path:
-284                    self.dbpath = Pathier(path)
-285                elif not path:
-286                    print("Searching recursively...")
-287                    dbs = list(cwd.rglob("*.db"))
-288                    if len(dbs) == 1:
-289                        self.dbpath = dbs[0]
-290                        print(f"Using database {self.dbpath}.")
-291                    elif dbs:
-292                        self.dbpath = self._choose_db(dbs)
-293                    else:
-294                        print("Could not find a .db file.")
-295                        self.dbpath = Pathier(input("Enter path to a .db
+284                )
+285                if path:
+286                    self.dbpath = Pathier(path)
+287                elif not path:
+288                    print("Searching recursively...")
+289                    dbs = list(cwd.rglob("*.db"))
+290                    if len(dbs) == 1:
+291                        self.dbpath = dbs[0]
+292                        print(f"Using database {self.dbpath}.")
+293                    elif dbs:
+294                        self.dbpath = self._choose_db(dbs)
+295                    else:
+296                        print("Could not find a .db file.")
+297                        self.dbpath = Pathier(input("Enter path to a .db
 file: "))
-296        if not self.dbpath.exists():
-297            raise FileNotFoundError(f"{self.dbpath} does not exist.")
-298        if not self.dbpath.is_file():
-299            raise ValueError(f"{self.dbpath} is not a file.")
-300
-301
-302def main():
-303    DBShell().cmdloop()
+298        if not self.dbpath.exists():
+299            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+300        if not self.dbpath.is_file():
+301            raise ValueError(f"{self.dbpath} is not a file.")
+302
+303
+304def main():
+305    DBShell().cmdloop()
   ⁰
 class DBShell(argshell.argshell.ArgShell): View Source
 __8class DBShell(argshell.ArgShell):
 __9    intro = "Starting dbshell (enter help or ? for arg info)..."
 _10    prompt = "based>"
 _11    dbpath: Pathier = None  # type: ignore
 _12
@@ -632,77 +634,79 @@
 236            custom_file.write_text(content)
 237
 238    def do_vacuum(self, arg: str):
 239        """Reduce database disk memory."""
 240        starting_size = self.dbpath.size()
 241        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
 242        print("Vacuuming database...")
-243        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-244        print(f"Freed up {Pathier.format_size(starting_size -
+243        with DataBased(self.dbpath) as db:
+244            db.vacuum()
+245        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
+246        print(f"Freed up {Pathier.format_size(starting_size -
 self.dbpath.size())} of disk space.")  # type: ignore
-245
-246    def _choose_db(self, options: list[Pathier]) -> Pathier:
-247        """Prompt the user to select from a list of files."""
-248        cwd = Pathier.cwd()
-249        paths = [path.separate(cwd.stem) for path in options]
-250        while True:
-251            print(
-252                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
+247
+248    def _choose_db(self, options: list[Pathier]) -> Pathier:
+249        """Prompt the user to select from a list of files."""
+250        cwd = Pathier.cwd()
+251        paths = [path.separate(cwd.stem) for path in options]
+252        while True:
+253            print(
+254                f"DB options:\n{' '.join([f'({i}) {path}' for i,path in
 enumerate(paths,1)])}"
-253            )
-254            choice = input("Enter the number of the option to use: ")
-255            try:
-256                index = int(choice)
-257                if not 1 <= index <= len(options):
-258                    print("Choice out of range.")
-259                    continue
-260                return options[index - 1]
-261            except Exception as e:
-262                print(f"{choice} is not a valid option.")
-263
-264    def preloop(self):
-265        """Scan the current directory for a .db file to use.
-266        If not found, prompt the user for one or to try again
+255            )
+256            choice = input("Enter the number of the option to use: ")
+257            try:
+258                index = int(choice)
+259                if not 1 <= index <= len(options):
+260                    print("Choice out of range.")
+261                    continue
+262                return options[index - 1]
+263            except Exception as e:
+264                print(f"{choice} is not a valid option.")
+265
+266    def preloop(self):
+267        """Scan the current directory for a .db file to use.
+268        If not found, prompt the user for one or to try again
 recursively."""
-267        if self.dbpath:
-268            self.dbpath = Pathier(self.dbpath)
-269            print(f"Defaulting to database {self.dbpath}")
-270        else:
-271            print("Searching for database...")
-272            cwd = Pathier.cwd()
-273            dbs = list(cwd.glob("*.db"))
-274            if len(dbs) == 1:
-275                self.dbpath = dbs[0]
-276                print(f"Using database {self.dbpath}.")
-277            elif dbs:
-278                self.dbpath = self._choose_db(dbs)
-279            else:
-280                print(f"Could not find a .db file in {cwd}.")
-281                path = input(
-282                    "Enter path to .db file to use or press enter to search
+269        if self.dbpath:
+270            self.dbpath = Pathier(self.dbpath)
+271            print(f"Defaulting to database {self.dbpath}")
+272        else:
+273            print("Searching for database...")
+274            cwd = Pathier.cwd()
+275            dbs = list(cwd.glob("*.db"))
+276            if len(dbs) == 1:
+277                self.dbpath = dbs[0]
+278                print(f"Using database {self.dbpath}.")
+279            elif dbs:
+280                self.dbpath = self._choose_db(dbs)
+281            else:
+282                print(f"Could not find a .db file in {cwd}.")
+283                path = input(
+284                    "Enter path to .db file to use or press enter to search
 again recursively: "
-283                )
-284                if path:
-285                    self.dbpath = Pathier(path)
-286                elif not path:
-287                    print("Searching recursively...")
-288                    dbs = list(cwd.rglob("*.db"))
-289                    if len(dbs) == 1:
-290                        self.dbpath = dbs[0]
-291                        print(f"Using database {self.dbpath}.")
-292                    elif dbs:
-293                        self.dbpath = self._choose_db(dbs)
-294                    else:
-295                        print("Could not find a .db file.")
-296                        self.dbpath = Pathier(input("Enter path to a .db
+285                )
+286                if path:
+287                    self.dbpath = Pathier(path)
+288                elif not path:
+289                    print("Searching recursively...")
+290                    dbs = list(cwd.rglob("*.db"))
+291                    if len(dbs) == 1:
+292                        self.dbpath = dbs[0]
+293                        print(f"Using database {self.dbpath}.")
+294                    elif dbs:
+295                        self.dbpath = self._choose_db(dbs)
+296                    else:
+297                        print("Could not find a .db file.")
+298                        self.dbpath = Pathier(input("Enter path to a .db
 file: "))
-297        if not self.dbpath.exists():
-298            raise FileNotFoundError(f"{self.dbpath} does not exist.")
-299        if not self.dbpath.is_file():
-300            raise ValueError(f"{self.dbpath} is not a file.")
+299        if not self.dbpath.exists():
+300            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+301        if not self.dbpath.is_file():
+302            raise ValueError(f"{self.dbpath} is not a file.")
 Subclass this to create custom ArgShells.
 ⁰
 def do_use_db(self, arg: str): View Source
 13    def do_use_db(self, arg: str):
 14        """Set which database file to use."""
 15        dbpath = Pathier(arg)
 16        if not dbpath.exists():
@@ -1038,61 +1042,63 @@
 ⁰
 def do_vacuum(self, arg: str): View Source
 238    def do_vacuum(self, arg: str):
 239        """Reduce database disk memory."""
 240        starting_size = self.dbpath.size()
 241        print(f"Database size before vacuuming: {self.dbpath.size(True)}")
 242        print("Vacuuming database...")
-243        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
-244        print(f"Freed up {Pathier.format_size(starting_size -
+243        with DataBased(self.dbpath) as db:
+244            db.vacuum()
+245        print(f"Database size after vacuuming: {self.dbpath.size(True)}")
+246        print(f"Freed up {Pathier.format_size(starting_size -
 self.dbpath.size())} of disk space.")  # type: ignore
 Reduce database disk memory.
 ⁰
 def preloop(self): View Source
-264    def preloop(self):
-265        """Scan the current directory for a .db file to use.
-266        If not found, prompt the user for one or to try again
+266    def preloop(self):
+267        """Scan the current directory for a .db file to use.
+268        If not found, prompt the user for one or to try again
 recursively."""
-267        if self.dbpath:
-268            self.dbpath = Pathier(self.dbpath)
-269            print(f"Defaulting to database {self.dbpath}")
-270        else:
-271            print("Searching for database...")
-272            cwd = Pathier.cwd()
-273            dbs = list(cwd.glob("*.db"))
-274            if len(dbs) == 1:
-275                self.dbpath = dbs[0]
-276                print(f"Using database {self.dbpath}.")
-277            elif dbs:
-278                self.dbpath = self._choose_db(dbs)
-279            else:
-280                print(f"Could not find a .db file in {cwd}.")
-281                path = input(
-282                    "Enter path to .db file to use or press enter to search
+269        if self.dbpath:
+270            self.dbpath = Pathier(self.dbpath)
+271            print(f"Defaulting to database {self.dbpath}")
+272        else:
+273            print("Searching for database...")
+274            cwd = Pathier.cwd()
+275            dbs = list(cwd.glob("*.db"))
+276            if len(dbs) == 1:
+277                self.dbpath = dbs[0]
+278                print(f"Using database {self.dbpath}.")
+279            elif dbs:
+280                self.dbpath = self._choose_db(dbs)
+281            else:
+282                print(f"Could not find a .db file in {cwd}.")
+283                path = input(
+284                    "Enter path to .db file to use or press enter to search
 again recursively: "
-283                )
-284                if path:
-285                    self.dbpath = Pathier(path)
-286                elif not path:
-287                    print("Searching recursively...")
-288                    dbs = list(cwd.rglob("*.db"))
-289                    if len(dbs) == 1:
-290                        self.dbpath = dbs[0]
-291                        print(f"Using database {self.dbpath}.")
-292                    elif dbs:
-293                        self.dbpath = self._choose_db(dbs)
-294                    else:
-295                        print("Could not find a .db file.")
-296                        self.dbpath = Pathier(input("Enter path to a .db
+285                )
+286                if path:
+287                    self.dbpath = Pathier(path)
+288                elif not path:
+289                    print("Searching recursively...")
+290                    dbs = list(cwd.rglob("*.db"))
+291                    if len(dbs) == 1:
+292                        self.dbpath = dbs[0]
+293                        print(f"Using database {self.dbpath}.")
+294                    elif dbs:
+295                        self.dbpath = self._choose_db(dbs)
+296                    else:
+297                        print("Could not find a .db file.")
+298                        self.dbpath = Pathier(input("Enter path to a .db
 file: "))
-297        if not self.dbpath.exists():
-298            raise FileNotFoundError(f"{self.dbpath} does not exist.")
-299        if not self.dbpath.is_file():
-300            raise ValueError(f"{self.dbpath} is not a file.")
+299        if not self.dbpath.exists():
+300            raise FileNotFoundError(f"{self.dbpath} does not exist.")
+301        if not self.dbpath.is_file():
+302            raise ValueError(f"{self.dbpath} is not a file.")
 Scan the current directory for a .db file to use. If not found, prompt the user
 for one or to try again recursively.
 ** Inherited Members **
   ⁰
 def main(): View Source
-303def main():
-304    DBShell().cmdloop()
+305def main():
+306    DBShell().cmdloop()
```

### Comparing `databased-2.2.0/src/databased/customshell.py` & `databased-2.2.1/src/databased/customshell.py`

 * *Files identical despite different names*

### Comparing `databased-2.2.0/src/databased/databased.py` & `databased-2.2.1/src/databased/databased.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
                 f'"{column_row[0]}" like "%{column_row[1]}%"'
                 for column_row in match_criteria
             )
         return f"({conditions})"
 
     def vacuum(self):
         """Reduce disk size of the database with a `VACUUM` query."""
-        self.query("VACUUM")
+        self.query("VACUUM;")
 
     @_connect
     def query(self, query_) -> list[Any]:
         """Execute an arbitrary query and return the results."""
         self.cursor.execute(query_)
         return self.cursor.fetchall()
```

### Comparing `databased-2.2.0/src/databased/dbparsers.py` & `databased-2.2.1/src/databased/dbparsers.py`

 * *Files identical despite different names*

### Comparing `databased-2.2.0/src/databased/dbshell.py` & `databased-2.2.1/src/databased/dbshell.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,14 +235,16 @@
             custom_file.write_text(content)
 
     def do_vacuum(self, arg: str):
         """Reduce database disk memory."""
         starting_size = self.dbpath.size()
         print(f"Database size before vacuuming: {self.dbpath.size(True)}")
         print("Vacuuming database...")
+        with DataBased(self.dbpath) as db:
+            db.vacuum()
         print(f"Database size after vacuuming: {self.dbpath.size(True)}")
         print(f"Freed up {Pathier.format_size(starting_size - self.dbpath.size())} of disk space.")  # type: ignore
 
     def _choose_db(self, options: list[Pathier]) -> Pathier:
         """Prompt the user to select from a list of files."""
         cwd = Pathier.cwd()
         paths = [path.separate(cwd.stem) for path in options]
```

### Comparing `databased-2.2.0/LICENSE.txt` & `databased-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `databased-2.2.0/README.md` & `databased-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `databased-2.2.0/pyproject.toml` & `databased-2.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "databased"
 authors = [{name="Matt Manes"}]
 description = "Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier."
-version = "2.2.0"
+version = "2.2.1"
 requires-python = ">=3.10"
 dependencies = ["pandas", "tabulate", "pytest", "argshell", "pathier"]
 readme = "README.md"
 keywords = [
     "database",
     "sqlite",
     "sqlite3"
```

### Comparing `databased-2.2.0/PKG-INFO` & `databased-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databased
-Version: 2.2.0
+Version: 2.2.1
 Summary: Wrapper for the standard library Sqlite3 module to make setting up and using a database quicker and easier.
 Project-URL: Homepage, https://github.com/matt-manes/databased
 Project-URL: Documentation, https://github.com/matt-manes/databased/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/databased/tree/main/src/databased
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: database,sqlite,sqlite3
```

