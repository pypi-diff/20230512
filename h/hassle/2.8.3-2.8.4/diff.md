# Comparing `tmp/hassle-2.8.3.tar.gz` & `tmp/hassle-2.8.4.tar.gz`

## Comparing `hassle-2.8.3.tar` & `hassle-2.8.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 hassle-2.8.3/CHANGELOG.md
--rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.8.3/docs/hassle.html
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.8.3/docs/index.html
--rw-r--r--   0        0        0    45086 2020-02-02 00:00:00.000000 hassle-2.8.3/docs/search.js
--rw-r--r--   0        0        0    93372 2020-02-02 00:00:00.000000 hassle-2.8.3/docs/hassle/generate_tests.html
--rw-r--r--   0        0        0   139420 2020-02-02 00:00:00.000000 hassle-2.8.3/docs/hassle/hassle.html
--rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.8.3/docs/hassle/hassle_config.html
--rw-r--r--   0        0        0   116364 2020-02-02 00:00:00.000000 hassle-2.8.3/docs/hassle/hassle_utilities.html
--rw-r--r--   0        0        0   165062 2020-02-02 00:00:00.000000 hassle-2.8.3/docs/hassle/new_project.html
--rw-r--r--   0        0        0    53608 2020-02-02 00:00:00.000000 hassle-2.8.3/docs/hassle/run_tests.html
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.8.3/src/hassle/.gitignore_template
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.8.3/src/hassle/.vscode_template
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.8.3/src/hassle/README_template.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.8.3/src/hassle/__init__.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 hassle-2.8.3/src/hassle/generate_tests.py
--rw-r--r--   0        0        0     8266 2020-02-02 00:00:00.000000 hassle-2.8.3/src/hassle/hassle.py
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.8.3/src/hassle/hassle_config.py
--rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 hassle-2.8.3/src/hassle/hassle_utilities.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.8.3/src/hassle/license_template.txt
--rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 hassle-2.8.3/src/hassle/new_project.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hassle-2.8.3/src/hassle/pyproject_template.toml
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 hassle-2.8.3/src/hassle/run_tests.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.8.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.8.3/LICENSE.txt
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.8.3/README.md
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 hassle-2.8.3/pyproject.toml
--rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 hassle-2.8.3/PKG-INFO
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 hassle-2.8.4/CHANGELOG.md
+-rw-r--r--   0        0        0    33936 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle.html
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/index.html
+-rw-r--r--   0        0        0    45086 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/search.js
+-rw-r--r--   0        0        0    93372 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle/generate_tests.html
+-rw-r--r--   0        0        0   139420 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle/hassle.html
+-rw-r--r--   0        0        0   107599 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle/hassle_config.html
+-rw-r--r--   0        0        0   116364 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle/hassle_utilities.html
+-rw-r--r--   0        0        0   165062 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle/new_project.html
+-rw-r--r--   0        0        0    54156 2020-02-02 00:00:00.000000 hassle-2.8.4/docs/hassle/run_tests.html
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/.gitignore_template
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/.vscode_template
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/README_template.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/__init__.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/generate_tests.py
+-rw-r--r--   0        0        0     8266 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/hassle.py
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/hassle_config.py
+-rw-r--r--   0        0        0     5246 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/hassle_utilities.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/license_template.txt
+-rw-r--r--   0        0        0     9187 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/new_project.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/pyproject_template.toml
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 hassle-2.8.4/src/hassle/run_tests.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 hassle-2.8.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hassle-2.8.4/LICENSE.txt
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 hassle-2.8.4/README.md
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 hassle-2.8.4/pyproject.toml
+-rw-r--r--   0        0        0    22533 2020-02-02 00:00:00.000000 hassle-2.8.4/PKG-INFO
```

### Comparing `hassle-2.8.3/CHANGELOG.md` & `hassle-2.8.4/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 # Changelog
 
-## 2.8.2 (2023-05-10)
+## 2.8.3 (2023-05-10)
+
+#### Fixes
+
+* fix bug where the package would get built before the version was incremented
+#### Others
+
+* build v2.8.2
+
+
+## v2.8.2 (2023-05-10)
 
 #### Fixes
 
 * swap build and increment_version order so version isn't incremented if build/tests fail
+#### Others
+
+* build v2.8.2
+* update changelog
 
 
 ## v2.8.1 (2023-05-10)
 
 #### Fixes
 
 * modify pip install invocation for better multi-platform support
@@ -28,15 +42,15 @@
 #### Fixes
 
 * catch Black.main()'s SystemExit
 * fix Pathier.mkcwd() usage
 * invoke build with sys.executable instead of py
 #### Refactorings
 
-* replace os.system calls to git with gitbetter.git methods
+* replace os.system call to git with gitbetter.git methods
 * replace os.system calls for black and isort with direct invocations
 * extract build process into it's own function
 * make run_tests() invoke pytest and coverage directly and return pytest result
 #### Others
 
 * build v2.8.0
 * update changelog
```

### Comparing `hassle-2.8.3/docs/hassle.html` & `hassle-2.8.4/docs/hassle.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/docs/search.js` & `hassle-2.8.4/docs/search.js`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/docs/hassle/generate_tests.html` & `hassle-2.8.4/docs/hassle/generate_tests.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/docs/hassle/hassle.html` & `hassle-2.8.4/docs/hassle/hassle.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/docs/hassle/hassle_config.html` & `hassle-2.8.4/docs/hassle/hassle_config.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/docs/hassle/hassle_utilities.html` & `hassle-2.8.4/docs/hassle/hassle_utilities.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/docs/hassle/new_project.html` & `hassle-2.8.4/docs/hassle/new_project.html`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/docs/hassle/run_tests.html` & `hassle-2.8.4/docs/hassle/run_tests.html`

 * *Files 1% similar despite different names*

```diff
@@ -94,26 +94,27 @@
 </span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>    <span class="n">package_path</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
 </span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>    <span class="n">cover</span> <span class="o">=</span> <span class="n">coverage</span><span class="o">.</span><span class="n">Coverage</span><span class="p">()</span>
 </span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
 </span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>    <span class="n">results</span> <span class="o">=</span> <span class="n">pytest</span><span class="o">.</span><span class="n">main</span><span class="p">([</span><span class="s2">&quot;-s&quot;</span><span class="p">])</span>
 </span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
 </span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">report</span><span class="p">()</span>
 </span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>    <span class="n">startdir</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>    <span class="k">return</span> <span class="n">results</span> <span class="o">==</span> <span class="mi">0</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>
+</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>    <span class="c1"># All tests passed (0) or Pytest couldn&#39;t find any tests (5)</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>    <span class="k">return</span> <span class="n">results</span> <span class="ow">in</span> <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">5</span><span class="p">]</span>
 </span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>
-</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>
+</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>
+</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
 </span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a>
-</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos">50</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a>
+</span><span id="L-50"><a href="#L-50"><span class="linenos">50</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos">51</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_args">
                             <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -167,15 +168,16 @@
 </span><span id="run_tests-33"><a href="#run_tests-33"><span class="linenos">33</span></a>    <span class="n">package_path</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
 </span><span id="run_tests-34"><a href="#run_tests-34"><span class="linenos">34</span></a>    <span class="n">cover</span> <span class="o">=</span> <span class="n">coverage</span><span class="o">.</span><span class="n">Coverage</span><span class="p">()</span>
 </span><span id="run_tests-35"><a href="#run_tests-35"><span class="linenos">35</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
 </span><span id="run_tests-36"><a href="#run_tests-36"><span class="linenos">36</span></a>    <span class="n">results</span> <span class="o">=</span> <span class="n">pytest</span><span class="o">.</span><span class="n">main</span><span class="p">([</span><span class="s2">&quot;-s&quot;</span><span class="p">])</span>
 </span><span id="run_tests-37"><a href="#run_tests-37"><span class="linenos">37</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
 </span><span id="run_tests-38"><a href="#run_tests-38"><span class="linenos">38</span></a>    <span class="n">cover</span><span class="o">.</span><span class="n">report</span><span class="p">()</span>
 </span><span id="run_tests-39"><a href="#run_tests-39"><span class="linenos">39</span></a>    <span class="n">startdir</span><span class="o">.</span><span class="n">mkcwd</span><span class="p">()</span>
-</span><span id="run_tests-40"><a href="#run_tests-40"><span class="linenos">40</span></a>    <span class="k">return</span> <span class="n">results</span> <span class="o">==</span> <span class="mi">0</span>
+</span><span id="run_tests-40"><a href="#run_tests-40"><span class="linenos">40</span></a>    <span class="c1"># All tests passed (0) or Pytest couldn&#39;t find any tests (5)</span>
+</span><span id="run_tests-41"><a href="#run_tests-41"><span class="linenos">41</span></a>    <span class="k">return</span> <span class="n">results</span> <span class="ow">in</span> <span class="p">[</span><span class="mi">0</span><span class="p">,</span> <span class="mi">5</span><span class="p">]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Run tests with coverage and pytest.</p>
 
 <p>Returns True if all tests passed.</p>
 </div>
@@ -189,19 +191,19 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-43"><a href="#main-43"><span class="linenos">43</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="main-44"><a href="#main-44"><span class="linenos">44</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="main-45"><a href="#main-45"><span class="linenos">45</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-46"><a href="#main-46"><span class="linenos">46</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
-</span><span id="main-47"><a href="#main-47"><span class="linenos">47</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-44"><a href="#main-44"><span class="linenos">44</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-45"><a href="#main-45"><span class="linenos">45</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-46"><a href="#main-46"><span class="linenos">46</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-47"><a href="#main-47"><span class="linenos">47</span></a>    <span class="n">package_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">package_name</span><span class="p">)</span><span class="o">.</span><span class="n">resolve</span><span class="p">()</span>
+</span><span id="main-48"><a href="#main-48"><span class="linenos">48</span></a>    <span class="n">run_tests</span><span class="p">(</span><span class="n">package_path</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -44,26 +44,27 @@
 32    package_path.mkcwd()
 33    cover = coverage.Coverage()
 34    cover.start()
 35    results = pytest.main(["-s"])
 36    cover.stop()
 37    cover.report()
 38    startdir.mkcwd()
-39    return results == 0
-40
+39    # All tests passed (0) or Pytest couldn't find any tests (5)
+40    return results in [0, 5]
 41
-42def main(args: argparse.Namespace = None):
-43    if not args:
-44        args = get_args()
-45    package_path = Pathier(args.package_name).resolve()
-46    run_tests(package_path)
-47
+42
+43def main(args: argparse.Namespace = None):
+44    if not args:
+45        args = get_args()
+46    package_path = Pathier(args.package_name).resolve()
+47    run_tests(package_path)
 48
-49if __name__ == "__main__":
-50    main(get_args())
+49
+50if __name__ == "__main__":
+51    main(get_args())
   ⁰
 def get_args() -> argparse.Namespace: View Source
 _9def get_args() -> argparse.Namespace:
 10    parser = argparse.ArgumentParser()
 11
 12    parser.add_argument(
 13        "package_name",
@@ -89,18 +90,19 @@
 33    package_path.mkcwd()
 34    cover = coverage.Coverage()
 35    cover.start()
 36    results = pytest.main(["-s"])
 37    cover.stop()
 38    cover.report()
 39    startdir.mkcwd()
-40    return results == 0
+40    # All tests passed (0) or Pytest couldn't find any tests (5)
+41    return results in [0, 5]
 Run tests with coverage and pytest.
 Returns True if all tests passed.
   ⁰
 def main(args: argparse.Namespace = None): View Source
-43def main(args: argparse.Namespace = None):
-44    if not args:
-45        args = get_args()
-46    package_path = Pathier(args.package_name).resolve()
-47    run_tests(package_path)
+44def main(args: argparse.Namespace = None):
+45    if not args:
+46        args = get_args()
+47    package_path = Pathier(args.package_name).resolve()
+48    run_tests(package_path)
```

### Comparing `hassle-2.8.3/src/hassle/generate_tests.py` & `hassle-2.8.4/src/hassle/generate_tests.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/src/hassle/hassle.py` & `hassle-2.8.4/src/hassle/hassle.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/src/hassle/hassle_config.py` & `hassle-2.8.4/src/hassle/hassle_config.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/src/hassle/hassle_utilities.py` & `hassle-2.8.4/src/hassle/hassle_utilities.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/src/hassle/license_template.txt` & `hassle-2.8.4/src/hassle/license_template.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/src/hassle/new_project.py` & `hassle-2.8.4/src/hassle/new_project.py`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/src/hassle/pyproject_template.toml` & `hassle-2.8.4/src/hassle/pyproject_template.toml`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/src/hassle/run_tests.py` & `hassle-2.8.4/src/hassle/run_tests.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     package_path.mkcwd()
     cover = coverage.Coverage()
     cover.start()
     results = pytest.main(["-s"])
     cover.stop()
     cover.report()
     startdir.mkcwd()
-    return results == 0
+    # All tests passed (0) or Pytest couldn't find any tests (5)
+    return results in [0, 5]
 
 
 def main(args: argparse.Namespace = None):
     if not args:
         args = get_args()
     package_path = Pathier(args.package_name).resolve()
     run_tests(package_path)
```

### Comparing `hassle-2.8.3/LICENSE.txt` & `hassle-2.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/README.md` & `hassle-2.8.4/README.md`

 * *Files identical despite different names*

### Comparing `hassle-2.8.3/pyproject.toml` & `hassle-2.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 226d 6174 746d 616e 6573 4070 6d2e 6d65  "mattmanes@pm.me
 000000a0: 227d 5d0d 0a64 6573 6372 6970 7469 6f6e  "}]..description
 000000b0: 203d 2022 4372 6561 7465 2c20 6275 696c   = "Create, buil
 000000c0: 642c 2074 6573 742c 2061 6e64 2070 7562  d, test, and pub
 000000d0: 6c69 7368 2050 7974 686f 6e20 7072 6f6a  lish Python proj
 000000e0: 6563 7473 2061 6e64 2070 6163 6b61 6765  ects and package
 000000f0: 732e 220d 0a76 6572 7369 6f6e 203d 2022  s."..version = "
-00000100: 322e 382e 3322 0d0a 7265 7175 6972 6573  2.8.3"..requires
+00000100: 322e 382e 3422 0d0a 7265 7175 6972 6573  2.8.4"..requires
 00000110: 2d70 7974 686f 6e20 3d20 223e 3d33 2e31  -python = ">=3.1
 00000120: 3022 0d0a 6465 7065 6e64 656e 6369 6573  0"..dependencies
 00000130: 203d 205b 0d0a 2020 2020 2262 6c61 636b   = [..    "black
 00000140: 222c 200d 0a20 2020 2022 6973 6f72 7422  ", ..    "isort"
 00000150: 2c20 0d0a 2020 2020 2270 7974 6573 747e  , ..    "pytest~
 00000160: 3d37 2e32 2e31 222c 200d 0a20 2020 2022  =7.2.1", ..    "
 00000170: 636f 7665 7261 6765 222c 0d0a 2020 2020  coverage",..
```

### Comparing `hassle-2.8.3/PKG-INFO` & `hassle-2.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassle
-Version: 2.8.3
+Version: 2.8.4
 Summary: Create, build, test, and publish Python projects and packages.
 Project-URL: Homepage, https://github.com/matt-manes/hassle
 Project-URL: Documentation, https://github.com/matt-manes/hassle/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/hassle/tree/main/src/hassle
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: automation,build,devops,packaging,test
```

