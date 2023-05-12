# Comparing `tmp/gitbetter-0.4.0.tar.gz` & `tmp/gitbetter-0.5.0.tar.gz`

## Comparing `gitbetter-0.4.0.tar` & `gitbetter-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 gitbetter-0.4.0/CHANGELOG.md
--rw-r--r--   0        0        0    34124 2020-02-02 00:00:00.000000 gitbetter-0.4.0/docs/gitbetter.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-0.4.0/docs/index.html
--rw-r--r--   0        0        0    57211 2020-02-02 00:00:00.000000 gitbetter-0.4.0/docs/search.js
--rw-r--r--   0        0        0   132406 2020-02-02 00:00:00.000000 gitbetter-0.4.0/docs/gitbetter/git.html
--rw-r--r--   0        0        0   250092 2020-02-02 00:00:00.000000 gitbetter-0.4.0/docs/gitbetter/gitbetter.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gitbetter-0.4.0/src/gitbetter/__init__.py
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 gitbetter-0.4.0/src/gitbetter/git.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 gitbetter-0.4.0/src/gitbetter/gitbetter.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-0.4.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 gitbetter-0.4.0/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 gitbetter-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 gitbetter-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34124 2020-02-02 00:00:00.000000 gitbetter-0.5.0/docs/gitbetter.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-0.5.0/docs/index.html
+-rw-r--r--   0        0        0    57989 2020-02-02 00:00:00.000000 gitbetter-0.5.0/docs/search.js
+-rw-r--r--   0        0        0   138209 2020-02-02 00:00:00.000000 gitbetter-0.5.0/docs/gitbetter/git.html
+-rw-r--r--   0        0        0   248978 2020-02-02 00:00:00.000000 gitbetter-0.5.0/docs/gitbetter/gitbetter.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gitbetter-0.5.0/src/gitbetter/__init__.py
+-rw-r--r--   0        0        0     5856 2020-02-02 00:00:00.000000 gitbetter-0.5.0/src/gitbetter/git.py
+-rw-r--r--   0        0        0    10209 2020-02-02 00:00:00.000000 gitbetter-0.5.0/src/gitbetter/gitbetter.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 gitbetter-0.5.0/README.md
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     4786 2020-02-02 00:00:00.000000 gitbetter-0.5.0/PKG-INFO
```

### Comparing `gitbetter-0.4.0/CHANGELOG.md` & `gitbetter-0.5.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
-## 0.3.0 (2023-05-02)
+## 0.4.0 (2023-05-04)
+
+#### New Features
+
+* add status command
+
+
+## v0.3.0 (2023-05-02)
 
 #### Refactorings
 
 * remove do_cmd as it's now covered by parent class's do_sys
+#### Others
+
+* build v0.3.0
+* update changelog
 
 
 ## v0.2.0 (2023-05-02)
 
 #### New Features
 
 * override do_help to display unrecognized_command_behavior_status after standard help message
```

### Comparing `gitbetter-0.4.0/docs/gitbetter.html` & `gitbetter-0.5.0/docs/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-0.4.0/docs/search.js` & `gitbetter-0.5.0/docs/search.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -881,14 +881,22 @@
         "modulename": "gitbetter.git",
         "qualname": "create_remote",
         "kind": "function",
         "doc": "<p>Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>name</code>: The name for the repo.</p>\n\n<p><code>public</code>: Set to <code>True</code> to create the repo as public, otherwise it'll be created as private.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">public</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
+        "fullname": "gitbetter.git.create_remote_from_cwd",
+        "modulename": "gitbetter.git",
+        "qualname": "create_remote_from_cwd",
+        "kind": "function",
+        "doc": "<p>Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from\nthe current working directory repo and add its url as this repo's remote origin.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>public</code>: Create the GitHub repo as a public repo, default is to create it as private.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">public</span><span class=\"p\">:</span> <span class=\"nb\">bool</span> <span class=\"o\">=</span> <span class=\"kc\">False</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
         "fullname": "gitbetter.git.make_private",
         "modulename": "gitbetter.git",
         "qualname": "make_private",
         "kind": "function",
         "doc": "<p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to private.</p>\n\n<h4 id=\"params\">:params:</h4>\n\n<p><code>owner</code>: The repo owner.</p>\n\n<p><code>name</code>: The name of the repo to edit.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">owner</span><span class=\"p\">:</span> <span class=\"nb\">str</span>, </span><span class=\"param\"><span class=\"n\">name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
@@ -1089,15 +1097,15 @@
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">branch_name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "gitbetter.gitbetter.GitBetter.do_add_url",
         "modulename": "gitbetter.gitbetter",
         "qualname": "GitBetter.do_add_url",
         "kind": "function",
-        "doc": "<p>Add remote url for repo and push repo.</p>\n",
+        "doc": "<p>Add remote origin url for repo and push repo.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">url</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "gitbetter.gitbetter.GitBetter.do_push_new",
         "modulename": "gitbetter.gitbetter",
         "qualname": "GitBetter.do_push_new",
         "kind": "function",
@@ -1117,17 +1125,17 @@
         "modulename": "gitbetter.gitbetter",
         "qualname": "GitBetter.do_pull",
         "kind": "function",
         "doc": "<p>Execute <code>git pull</code>.</p>\n\n<p><code>args</code> can be any additional args that <code>git pull</code> accepts.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "gitbetter.gitbetter.GitBetter.do_list_branches",
+        "fullname": "gitbetter.gitbetter.GitBetter.do_branches",
         "modulename": "gitbetter.gitbetter",
-        "qualname": "GitBetter.do_list_branches",
+        "qualname": "GitBetter.do_branches",
         "kind": "function",
         "doc": "<p>Show local and remote branches.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">_</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "gitbetter.gitbetter.GitBetter.do_loggy",
         "modulename": "gitbetter.gitbetter",
```

### Comparing `gitbetter-0.4.0/docs/gitbetter/git.html` & `gitbetter-0.5.0/docs/gitbetter/git.html`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,17 @@
             <li>
                     <a class="function" href="#merge">merge</a>
             </li>
             <li>
                     <a class="function" href="#create_remote">create_remote</a>
             </li>
             <li>
+                    <a class="function" href="#create_remote_from_cwd">create_remote_from_cwd</a>
+            </li>
+            <li>
                     <a class="function" href="#make_private">make_private</a>
             </li>
             <li>
                     <a class="function" href="#make_public">make_public</a>
             </li>
             <li>
                     <a class="function" href="#delete_remote">delete_remote</a>
@@ -301,45 +304,56 @@
 </span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">    `name`: The name for the repo.</span>
 </span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>
 </span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a><span class="sd">    `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
 </span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
 </span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>
 </span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">    #### :params:</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a><span class="sd">    `owner`: The repo owner.</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility private&quot;</span><span class="p">)</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="sd">    the current working directory repo and add its url as this repo&#39;s remote origin.</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="sd">    `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create --source . --</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
 </span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
 </span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
 </span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="sd">    #### :params:</span>
 </span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>
 </span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">    `owner`: The repo owner.</span>
 </span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
 </span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility public&quot;</span><span class="p">)</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility private&quot;</span><span class="p">)</span>
 </span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>
 </span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
 </span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>
 </span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="sd">    #### :params:</span>
 </span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>
 </span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">    `owner`: The repo owner.</span>
 </span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">    `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo delete </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --yes&quot;</span><span class="p">)</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility public&quot;</span><span class="p">)</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a><span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">    `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo delete </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --yes&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             </section>
                 <section id="execute">
                             <input id="execute-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -956,34 +970,67 @@
 <p><code>name</code>: The name for the repo.</p>
 
 <p><code>public</code>: Set to <code>True</code> to create the repo as public, otherwise it'll be created as private.</p>
 </div>
 
 
                 </section>
+                <section id="create_remote_from_cwd">
+                            <input id="create_remote_from_cwd-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">create_remote_from_cwd</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="create_remote_from_cwd-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#create_remote_from_cwd"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_remote_from_cwd-175"><a href="#create_remote_from_cwd-175"><span class="linenos">175</span></a><span class="k">def</span> <span class="nf">create_remote_from_cwd</span><span class="p">(</span><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="create_remote_from_cwd-176"><a href="#create_remote_from_cwd-176"><span class="linenos">176</span></a>    <span class="sd">&quot;&quot;&quot;Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from</span>
+</span><span id="create_remote_from_cwd-177"><a href="#create_remote_from_cwd-177"><span class="linenos">177</span></a><span class="sd">    the current working directory repo and add its url as this repo&#39;s remote origin.</span>
+</span><span id="create_remote_from_cwd-178"><a href="#create_remote_from_cwd-178"><span class="linenos">178</span></a>
+</span><span id="create_remote_from_cwd-179"><a href="#create_remote_from_cwd-179"><span class="linenos">179</span></a><span class="sd">    #### :params:</span>
+</span><span id="create_remote_from_cwd-180"><a href="#create_remote_from_cwd-180"><span class="linenos">180</span></a>
+</span><span id="create_remote_from_cwd-181"><a href="#create_remote_from_cwd-181"><span class="linenos">181</span></a><span class="sd">    `public`: Create the GitHub repo as a public repo, default is to create it as private.&quot;&quot;&quot;</span>
+</span><span id="create_remote_from_cwd-182"><a href="#create_remote_from_cwd-182"><span class="linenos">182</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;private&quot;</span>
+</span><span id="create_remote_from_cwd-183"><a href="#create_remote_from_cwd-183"><span class="linenos">183</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create --source . --</span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from
+the current working directory repo and add its url as this repo's remote origin.</p>
+
+<h4 id="params">:params:</h4>
+
+<p><code>public</code>: Create the GitHub repo as a public repo, default is to create it as private.</p>
+</div>
+
+
+                </section>
                 <section id="make_private">
                             <input id="make_private-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">make_private</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="make_private-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#make_private"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="make_private-175"><a href="#make_private-175"><span class="linenos">175</span></a><span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="make_private-176"><a href="#make_private-176"><span class="linenos">176</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
-</span><span id="make_private-177"><a href="#make_private-177"><span class="linenos">177</span></a>
-</span><span id="make_private-178"><a href="#make_private-178"><span class="linenos">178</span></a><span class="sd">    #### :params:</span>
-</span><span id="make_private-179"><a href="#make_private-179"><span class="linenos">179</span></a>
-</span><span id="make_private-180"><a href="#make_private-180"><span class="linenos">180</span></a><span class="sd">    `owner`: The repo owner.</span>
-</span><span id="make_private-181"><a href="#make_private-181"><span class="linenos">181</span></a>
-</span><span id="make_private-182"><a href="#make_private-182"><span class="linenos">182</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="make_private-183"><a href="#make_private-183"><span class="linenos">183</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility private&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="make_private-186"><a href="#make_private-186"><span class="linenos">186</span></a><span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="make_private-187"><a href="#make_private-187"><span class="linenos">187</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
+</span><span id="make_private-188"><a href="#make_private-188"><span class="linenos">188</span></a>
+</span><span id="make_private-189"><a href="#make_private-189"><span class="linenos">189</span></a><span class="sd">    #### :params:</span>
+</span><span id="make_private-190"><a href="#make_private-190"><span class="linenos">190</span></a>
+</span><span id="make_private-191"><a href="#make_private-191"><span class="linenos">191</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="make_private-192"><a href="#make_private-192"><span class="linenos">192</span></a>
+</span><span id="make_private-193"><a href="#make_private-193"><span class="linenos">193</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="make_private-194"><a href="#make_private-194"><span class="linenos">194</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility private&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to private.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1001,23 +1048,23 @@
         <span class="def">def</span>
         <span class="name">make_public</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="make_public-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#make_public"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="make_public-186"><a href="#make_public-186"><span class="linenos">186</span></a><span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="make_public-187"><a href="#make_public-187"><span class="linenos">187</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
-</span><span id="make_public-188"><a href="#make_public-188"><span class="linenos">188</span></a>
-</span><span id="make_public-189"><a href="#make_public-189"><span class="linenos">189</span></a><span class="sd">    #### :params:</span>
-</span><span id="make_public-190"><a href="#make_public-190"><span class="linenos">190</span></a>
-</span><span id="make_public-191"><a href="#make_public-191"><span class="linenos">191</span></a><span class="sd">    `owner`: The repo owner.</span>
-</span><span id="make_public-192"><a href="#make_public-192"><span class="linenos">192</span></a>
-</span><span id="make_public-193"><a href="#make_public-193"><span class="linenos">193</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="make_public-194"><a href="#make_public-194"><span class="linenos">194</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility public&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="make_public-197"><a href="#make_public-197"><span class="linenos">197</span></a><span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="make_public-198"><a href="#make_public-198"><span class="linenos">198</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
+</span><span id="make_public-199"><a href="#make_public-199"><span class="linenos">199</span></a>
+</span><span id="make_public-200"><a href="#make_public-200"><span class="linenos">200</span></a><span class="sd">    #### :params:</span>
+</span><span id="make_public-201"><a href="#make_public-201"><span class="linenos">201</span></a>
+</span><span id="make_public-202"><a href="#make_public-202"><span class="linenos">202</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="make_public-203"><a href="#make_public-203"><span class="linenos">203</span></a>
+</span><span id="make_public-204"><a href="#make_public-204"><span class="linenos">204</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="make_public-205"><a href="#make_public-205"><span class="linenos">205</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility public&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to public.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1035,23 +1082,23 @@
         <span class="def">def</span>
         <span class="name">delete_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="delete_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#delete_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_remote-197"><a href="#delete_remote-197"><span class="linenos">197</span></a><span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="delete_remote-198"><a href="#delete_remote-198"><span class="linenos">198</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
-</span><span id="delete_remote-199"><a href="#delete_remote-199"><span class="linenos">199</span></a>
-</span><span id="delete_remote-200"><a href="#delete_remote-200"><span class="linenos">200</span></a><span class="sd">    #### :params:</span>
-</span><span id="delete_remote-201"><a href="#delete_remote-201"><span class="linenos">201</span></a>
-</span><span id="delete_remote-202"><a href="#delete_remote-202"><span class="linenos">202</span></a><span class="sd">    `owner`: The repo owner.</span>
-</span><span id="delete_remote-203"><a href="#delete_remote-203"><span class="linenos">203</span></a>
-</span><span id="delete_remote-204"><a href="#delete_remote-204"><span class="linenos">204</span></a><span class="sd">    `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
-</span><span id="delete_remote-205"><a href="#delete_remote-205"><span class="linenos">205</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo delete </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --yes&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_remote-208"><a href="#delete_remote-208"><span class="linenos">208</span></a><span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="delete_remote-209"><a href="#delete_remote-209"><span class="linenos">209</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
+</span><span id="delete_remote-210"><a href="#delete_remote-210"><span class="linenos">210</span></a>
+</span><span id="delete_remote-211"><a href="#delete_remote-211"><span class="linenos">211</span></a><span class="sd">    #### :params:</span>
+</span><span id="delete_remote-212"><a href="#delete_remote-212"><span class="linenos">212</span></a>
+</span><span id="delete_remote-213"><a href="#delete_remote-213"><span class="linenos">213</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="delete_remote-214"><a href="#delete_remote-214"><span class="linenos">214</span></a>
+</span><span id="delete_remote-215"><a href="#delete_remote-215"><span class="linenos">215</span></a><span class="sd">    `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
+</span><span id="delete_remote-216"><a href="#delete_remote-216"><span class="linenos">216</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo delete </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --yes&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</p>
 
 <h4 id="params">:params:</h4>
```

#### html2text {}

```diff
@@ -23,14 +23,15 @@
     * checkout
     * switch_branch
     * create_new_branch
     * delete_branch
     * undo
     * merge
     * create_remote
+    * create_remote_from_cwd
     * make_private
     * make_public
     * delete_remote
 built_with_pdoc[pdoc_logo]
 
 ****** gitbetter.git ******
 ⁰ View Source
@@ -211,48 +212,62 @@
 168
 169    `public`: Set to `True` to create the repo as public, otherwise it'll be
 created as private."""
 170    visibility = "--public" if public else "--private"
 171    os.system(f"gh repo create {name} {visibility}")
 172
 173
-174def make_private(owner: str, name: str):
-175    """Uses GitHub CLI (must be installed and configured) to set the repo's
-visibility to private.
-176
-177    #### :params:
-178
-179    `owner`: The repo owner.
-180
-181    `name`: The name of the repo to edit."""
-182    os.system(f"gh repo edit {owner}/{name} --visibility private")
+174def create_remote_from_cwd(public: bool = False):
+175    """Use GitHub CLI (must be installed and configured) to create a remote
+GitHub repo from
+176    the current working directory repo and add its url as this repo's remote
+origin.
+177
+178    #### :params:
+179
+180    `public`: Create the GitHub repo as a public repo, default is to create
+it as private."""
+181    visibility = "public" if public else "private"
+182    os.system(f"gh repo create --source . --{visibility}")
 183
 184
-185def make_public(owner: str, name: str):
+185def make_private(owner: str, name: str):
 186    """Uses GitHub CLI (must be installed and configured) to set the repo's
-visibility to public.
+visibility to private.
 187
 188    #### :params:
 189
 190    `owner`: The repo owner.
 191
 192    `name`: The name of the repo to edit."""
-193    os.system(f"gh repo edit {owner}/{name} --visibility public")
+193    os.system(f"gh repo edit {owner}/{name} --visibility private")
 194
 195
-196def delete_remote(owner: str, name: str):
-197    """Uses GitHub CLI (must be isntalled and configured) to delete the
-remote for this repo.
+196def make_public(owner: str, name: str):
+197    """Uses GitHub CLI (must be installed and configured) to set the repo's
+visibility to public.
 198
 199    #### :params:
 200
 201    `owner`: The repo owner.
 202
-203    `name`: The name of the remote repo to delete."""
-204    os.system(f"gh repo delete {owner}/{name} --yes")
+203    `name`: The name of the repo to edit."""
+204    os.system(f"gh repo edit {owner}/{name} --visibility public")
+205
+206
+207def delete_remote(owner: str, name: str):
+208    """Uses GitHub CLI (must be isntalled and configured) to delete the
+remote for this repo.
+209
+210    #### :params:
+211
+212    `owner`: The repo owner.
+213
+214    `name`: The name of the remote repo to delete."""
+215    os.system(f"gh repo delete {owner}/{name} --yes")
   ⁰
 def execute(command: str) -> int: View Source
 _5def execute(command: str) -> int:
 _6    """Execute git command.
 _7
 _8    Equivalent to `os.system(f"git {command}")`
 _9
@@ -460,58 +475,78 @@
 Uses GitHub CLI (must be installed and configured) to create a remote GitHub
 repo.
 *** :params: ***
 name: The name for the repo.
 public: Set to True to create the repo as public, otherwise it'll be created as
 private.
   ⁰
-def make_private(owner: str, name: str): View Source
-175def make_private(owner: str, name: str):
-176    """Uses GitHub CLI (must be installed and configured) to set the repo's
-visibility to private.
-177
-178    #### :params:
-179
-180    `owner`: The repo owner.
-181
-182    `name`: The name of the repo to edit."""
-183    os.system(f"gh repo edit {owner}/{name} --visibility private")
-Uses GitHub CLI (must be installed and configured) to set the repo's visibility
-to private.
+def create_remote_from_cwd(public: bool = False): View Source
+175def create_remote_from_cwd(public: bool = False):
+176    """Use GitHub CLI (must be installed and configured) to create a remote
+GitHub repo from
+177    the current working directory repo and add its url as this repo's remote
+origin.
+178
+179    #### :params:
+180
+181    `public`: Create the GitHub repo as a public repo, default is to create
+it as private."""
+182    visibility = "public" if public else "private"
+183    os.system(f"gh repo create --source . --{visibility}")
+Use GitHub CLI (must be installed and configured) to create a remote GitHub
+repo from the current working directory repo and add its url as this repo's
+remote origin.
 *** :params: ***
-owner: The repo owner.
-name: The name of the repo to edit.
+public: Create the GitHub repo as a public repo, default is to create it as
+private.
   ⁰
-def make_public(owner: str, name: str): View Source
-186def make_public(owner: str, name: str):
+def make_private(owner: str, name: str): View Source
+186def make_private(owner: str, name: str):
 187    """Uses GitHub CLI (must be installed and configured) to set the repo's
-visibility to public.
+visibility to private.
 188
 189    #### :params:
 190
 191    `owner`: The repo owner.
 192
 193    `name`: The name of the repo to edit."""
-194    os.system(f"gh repo edit {owner}/{name} --visibility public")
+194    os.system(f"gh repo edit {owner}/{name} --visibility private")
 Uses GitHub CLI (must be installed and configured) to set the repo's visibility
-to public.
+to private.
 *** :params: ***
 owner: The repo owner.
 name: The name of the repo to edit.
   ⁰
-def delete_remote(owner: str, name: str): View Source
-197def delete_remote(owner: str, name: str):
-198    """Uses GitHub CLI (must be isntalled and configured) to delete the
-remote for this repo.
+def make_public(owner: str, name: str): View Source
+197def make_public(owner: str, name: str):
+198    """Uses GitHub CLI (must be installed and configured) to set the repo's
+visibility to public.
 199
 200    #### :params:
 201
 202    `owner`: The repo owner.
 203
-204    `name`: The name of the remote repo to delete."""
-205    os.system(f"gh repo delete {owner}/{name} --yes")
+204    `name`: The name of the repo to edit."""
+205    os.system(f"gh repo edit {owner}/{name} --visibility public")
+Uses GitHub CLI (must be installed and configured) to set the repo's visibility
+to public.
+*** :params: ***
+owner: The repo owner.
+name: The name of the repo to edit.
+  ⁰
+def delete_remote(owner: str, name: str): View Source
+208def delete_remote(owner: str, name: str):
+209    """Uses GitHub CLI (must be isntalled and configured) to delete the
+remote for this repo.
+210
+211    #### :params:
+212
+213    `owner`: The repo owner.
+214
+215    `name`: The name of the remote repo to delete."""
+216    os.system(f"gh repo delete {owner}/{name} --yes")
 Uses GitHub CLI (must be isntalled and configured) to delete the remote for
 this repo.
 *** :params: ***
 owner: The repo owner.
 name: The name of the remote repo to delete.
```

### Comparing `gitbetter-0.4.0/docs/gitbetter/gitbetter.html` & `gitbetter-0.5.0/docs/gitbetter/gitbetter.html`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                         <li>
                                 <a class="function" href="#GitBetter.do_push">do_push</a>
                         </li>
                         <li>
                                 <a class="function" href="#GitBetter.do_pull">do_pull</a>
                         </li>
                         <li>
-                                <a class="function" href="#GitBetter.do_list_branches">do_list_branches</a>
+                                <a class="function" href="#GitBetter.do_branches">do_branches</a>
                         </li>
                         <li>
                                 <a class="function" href="#GitBetter.do_loggy">do_loggy</a>
                         </li>
                         <li>
                                 <a class="function" href="#GitBetter.do_status">do_status</a>
                         </li>
@@ -291,15 +291,15 @@
 </span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>                <span class="nb">print</span><span class="p">(</span>
 </span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
 </span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>                <span class="p">)</span>
 </span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>        <span class="nb">print</span><span class="p">()</span>
 </span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>
 </span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="nd">@property</span>
 </span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="k">def</span> <span class="nf">unrecognized_command_behavior_status</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute in shell with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
 </span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
 </span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
 </span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
 </span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
 </span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
@@ -326,152 +326,151 @@
 </span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
 </span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>
 </span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
 </span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
 </span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
 </span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
 </span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>        <span class="n">name</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
-</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
-</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>
-</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url for repo and push repo.&quot;&quot;&quot;</span>
-</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
-</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>
-</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
-</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>
-</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
-</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a>
-</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
-</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>
-</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
-</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a>
-</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
-</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>
-</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>    <span class="k">def</span> <span class="nf">do_list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
-</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
-</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
-</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
-</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
-</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
-</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>
-</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
+</span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
+</span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>
+</span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="L-205"><a href="#L-205"><span class="linenos">205</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
+</span><span id="L-206"><a href="#L-206"><span class="linenos">206</span></a>
+</span><span id="L-207"><a href="#L-207"><span class="linenos">207</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-208"><a href="#L-208"><span class="linenos">208</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
+</span><span id="L-209"><a href="#L-209"><span class="linenos">209</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-210"><a href="#L-210"><span class="linenos">210</span></a>
+</span><span id="L-211"><a href="#L-211"><span class="linenos">211</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-212"><a href="#L-212"><span class="linenos">212</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
+</span><span id="L-213"><a href="#L-213"><span class="linenos">213</span></a>
+</span><span id="L-214"><a href="#L-214"><span class="linenos">214</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
+</span><span id="L-215"><a href="#L-215"><span class="linenos">215</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-216"><a href="#L-216"><span class="linenos">216</span></a>
+</span><span id="L-217"><a href="#L-217"><span class="linenos">217</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-218"><a href="#L-218"><span class="linenos">218</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
+</span><span id="L-219"><a href="#L-219"><span class="linenos">219</span></a>
+</span><span id="L-220"><a href="#L-220"><span class="linenos">220</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
+</span><span id="L-221"><a href="#L-221"><span class="linenos">221</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="L-222"><a href="#L-222"><span class="linenos">222</span></a>
+</span><span id="L-223"><a href="#L-223"><span class="linenos">223</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-224"><a href="#L-224"><span class="linenos">224</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
+</span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
+</span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>
+</span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+</span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>
+</span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>
+</span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>
+</span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>
+</span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>
+</span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>
+</span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>
 </span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>
-</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+</span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>
 </span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>
-</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>
-</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>    <span class="n">main</span><span class="p">()</span>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a>    <span class="n">main</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
                 <section id="new_remote_parser">
                             <input id="new_remote_parser-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -685,15 +684,15 @@
 </span><span id="GitBetter-119"><a href="#GitBetter-119"><span class="linenos">119</span></a>                <span class="nb">print</span><span class="p">(</span>
 </span><span id="GitBetter-120"><a href="#GitBetter-120"><span class="linenos">120</span></a>                    <span class="s2">&quot;^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^&quot;</span>
 </span><span id="GitBetter-121"><a href="#GitBetter-121"><span class="linenos">121</span></a>                <span class="p">)</span>
 </span><span id="GitBetter-122"><a href="#GitBetter-122"><span class="linenos">122</span></a>        <span class="nb">print</span><span class="p">()</span>
 </span><span id="GitBetter-123"><a href="#GitBetter-123"><span class="linenos">123</span></a>
 </span><span id="GitBetter-124"><a href="#GitBetter-124"><span class="linenos">124</span></a>    <span class="nd">@property</span>
 </span><span id="GitBetter-125"><a href="#GitBetter-125"><span class="linenos">125</span></a>    <span class="k">def</span> <span class="nf">unrecognized_command_behavior_status</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
-</span><span id="GitBetter-126"><a href="#GitBetter-126"><span class="linenos">126</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="GitBetter-126"><a href="#GitBetter-126"><span class="linenos">126</span></a>        <span class="k">return</span> <span class="sa">f</span><span class="s2">&quot;Unrecognized command behavior: </span><span class="si">{</span><span class="s1">&#39;Execute in shell with os.system()&#39;</span> <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="k">else</span> <span class="s1">&#39;Print unknown syntax error&#39;</span><span class="si">}</span><span class="s2">&quot;</span>
 </span><span id="GitBetter-127"><a href="#GitBetter-127"><span class="linenos">127</span></a>
 </span><span id="GitBetter-128"><a href="#GitBetter-128"><span class="linenos">128</span></a>    <span class="k">def</span> <span class="nf">do_toggle_unrecognized_command_behavior</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">arg</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="GitBetter-129"><a href="#GitBetter-129"><span class="linenos">129</span></a>        <span class="sd">&quot;&quot;&quot;Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.</span>
 </span><span id="GitBetter-130"><a href="#GitBetter-130"><span class="linenos">130</span></a><span class="sd">        When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.</span>
 </span><span id="GitBetter-131"><a href="#GitBetter-131"><span class="linenos">131</span></a><span class="sd">        When off, an `unknown syntax` message will be printed and no commands will be executed.&quot;&quot;&quot;</span>
 </span><span id="GitBetter-132"><a href="#GitBetter-132"><span class="linenos">132</span></a>        <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span> <span class="o">=</span> <span class="p">(</span>
 </span><span id="GitBetter-133"><a href="#GitBetter-133"><span class="linenos">133</span></a>            <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">execute_in_terminal_if_unrecognized</span>
@@ -720,144 +719,143 @@
 </span><span id="GitBetter-154"><a href="#GitBetter-154"><span class="linenos">154</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_new_branch</span><span class="p">(</span><span class="n">name</span><span class="p">)</span>
 </span><span id="GitBetter-155"><a href="#GitBetter-155"><span class="linenos">155</span></a>
 </span><span id="GitBetter-156"><a href="#GitBetter-156"><span class="linenos">156</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
 </span><span id="GitBetter-157"><a href="#GitBetter-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
 </span><span id="GitBetter-158"><a href="#GitBetter-158"><span class="linenos">158</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
 </span><span id="GitBetter-159"><a href="#GitBetter-159"><span class="linenos">159</span></a>
 </span><span id="GitBetter-160"><a href="#GitBetter-160"><span class="linenos">160</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-161"><a href="#GitBetter-161"><span class="linenos">161</span></a>        <span class="n">name</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="GitBetter-162"><a href="#GitBetter-162"><span class="linenos">162</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
-</span><span id="GitBetter-163"><a href="#GitBetter-163"><span class="linenos">163</span></a>
-</span><span id="GitBetter-164"><a href="#GitBetter-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-165"><a href="#GitBetter-165"><span class="linenos">165</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-166"><a href="#GitBetter-166"><span class="linenos">166</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
-</span><span id="GitBetter-167"><a href="#GitBetter-167"><span class="linenos">167</span></a>
-</span><span id="GitBetter-168"><a href="#GitBetter-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-169"><a href="#GitBetter-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-170"><a href="#GitBetter-170"><span class="linenos">170</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
-</span><span id="GitBetter-171"><a href="#GitBetter-171"><span class="linenos">171</span></a>
-</span><span id="GitBetter-172"><a href="#GitBetter-172"><span class="linenos">172</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-173"><a href="#GitBetter-173"><span class="linenos">173</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-174"><a href="#GitBetter-174"><span class="linenos">174</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="GitBetter-175"><a href="#GitBetter-175"><span class="linenos">175</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-176"><a href="#GitBetter-176"><span class="linenos">176</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="GitBetter-177"><a href="#GitBetter-177"><span class="linenos">177</span></a>
-</span><span id="GitBetter-178"><a href="#GitBetter-178"><span class="linenos">178</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-179"><a href="#GitBetter-179"><span class="linenos">179</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-180"><a href="#GitBetter-180"><span class="linenos">180</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-181"><a href="#GitBetter-181"><span class="linenos">181</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter-182"><a href="#GitBetter-182"><span class="linenos">182</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-183"><a href="#GitBetter-183"><span class="linenos">183</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter-184"><a href="#GitBetter-184"><span class="linenos">184</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-185"><a href="#GitBetter-185"><span class="linenos">185</span></a>
-</span><span id="GitBetter-186"><a href="#GitBetter-186"><span class="linenos">186</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-187"><a href="#GitBetter-187"><span class="linenos">187</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-188"><a href="#GitBetter-188"><span class="linenos">188</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-189"><a href="#GitBetter-189"><span class="linenos">189</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
-</span><span id="GitBetter-190"><a href="#GitBetter-190"><span class="linenos">190</span></a>
-</span><span id="GitBetter-191"><a href="#GitBetter-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-192"><a href="#GitBetter-192"><span class="linenos">192</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-193"><a href="#GitBetter-193"><span class="linenos">193</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-194"><a href="#GitBetter-194"><span class="linenos">194</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter-195"><a href="#GitBetter-195"><span class="linenos">195</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter-196"><a href="#GitBetter-196"><span class="linenos">196</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter-197"><a href="#GitBetter-197"><span class="linenos">197</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
-</span><span id="GitBetter-198"><a href="#GitBetter-198"><span class="linenos">198</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-199"><a href="#GitBetter-199"><span class="linenos">199</span></a>
-</span><span id="GitBetter-200"><a href="#GitBetter-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-201"><a href="#GitBetter-201"><span class="linenos">201</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-202"><a href="#GitBetter-202"><span class="linenos">202</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="GitBetter-203"><a href="#GitBetter-203"><span class="linenos">203</span></a>
-</span><span id="GitBetter-204"><a href="#GitBetter-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-205"><a href="#GitBetter-205"><span class="linenos">205</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url for repo and push repo.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-206"><a href="#GitBetter-206"><span class="linenos">206</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="GitBetter-207"><a href="#GitBetter-207"><span class="linenos">207</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-208"><a href="#GitBetter-208"><span class="linenos">208</span></a>
-</span><span id="GitBetter-209"><a href="#GitBetter-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-210"><a href="#GitBetter-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-211"><a href="#GitBetter-211"><span class="linenos">211</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="GitBetter-212"><a href="#GitBetter-212"><span class="linenos">212</span></a>
-</span><span id="GitBetter-213"><a href="#GitBetter-213"><span class="linenos">213</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-214"><a href="#GitBetter-214"><span class="linenos">214</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
-</span><span id="GitBetter-215"><a href="#GitBetter-215"><span class="linenos">215</span></a>
-</span><span id="GitBetter-216"><a href="#GitBetter-216"><span class="linenos">216</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-217"><a href="#GitBetter-217"><span class="linenos">217</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="GitBetter-218"><a href="#GitBetter-218"><span class="linenos">218</span></a>
-</span><span id="GitBetter-219"><a href="#GitBetter-219"><span class="linenos">219</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-220"><a href="#GitBetter-220"><span class="linenos">220</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
-</span><span id="GitBetter-221"><a href="#GitBetter-221"><span class="linenos">221</span></a>
-</span><span id="GitBetter-222"><a href="#GitBetter-222"><span class="linenos">222</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-223"><a href="#GitBetter-223"><span class="linenos">223</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
-</span><span id="GitBetter-224"><a href="#GitBetter-224"><span class="linenos">224</span></a>
-</span><span id="GitBetter-225"><a href="#GitBetter-225"><span class="linenos">225</span></a>    <span class="k">def</span> <span class="nf">do_list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-226"><a href="#GitBetter-226"><span class="linenos">226</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-227"><a href="#GitBetter-227"><span class="linenos">227</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
-</span><span id="GitBetter-228"><a href="#GitBetter-228"><span class="linenos">228</span></a>
-</span><span id="GitBetter-229"><a href="#GitBetter-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-230"><a href="#GitBetter-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-231"><a href="#GitBetter-231"><span class="linenos">231</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
-</span><span id="GitBetter-232"><a href="#GitBetter-232"><span class="linenos">232</span></a>
-</span><span id="GitBetter-233"><a href="#GitBetter-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-234"><a href="#GitBetter-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-235"><a href="#GitBetter-235"><span class="linenos">235</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
-</span><span id="GitBetter-236"><a href="#GitBetter-236"><span class="linenos">236</span></a>
-</span><span id="GitBetter-237"><a href="#GitBetter-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-238"><a href="#GitBetter-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-239"><a href="#GitBetter-239"><span class="linenos">239</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="GitBetter-240"><a href="#GitBetter-240"><span class="linenos">240</span></a>
-</span><span id="GitBetter-241"><a href="#GitBetter-241"><span class="linenos">241</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-242"><a href="#GitBetter-242"><span class="linenos">242</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-243"><a href="#GitBetter-243"><span class="linenos">243</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
-</span><span id="GitBetter-244"><a href="#GitBetter-244"><span class="linenos">244</span></a>
-</span><span id="GitBetter-245"><a href="#GitBetter-245"><span class="linenos">245</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-246"><a href="#GitBetter-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-247"><a href="#GitBetter-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-248"><a href="#GitBetter-248"><span class="linenos">248</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="GitBetter-249"><a href="#GitBetter-249"><span class="linenos">249</span></a>
-</span><span id="GitBetter-250"><a href="#GitBetter-250"><span class="linenos">250</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="GitBetter-251"><a href="#GitBetter-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-252"><a href="#GitBetter-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-253"><a href="#GitBetter-253"><span class="linenos">253</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
-</span><span id="GitBetter-254"><a href="#GitBetter-254"><span class="linenos">254</span></a>
-</span><span id="GitBetter-255"><a href="#GitBetter-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-256"><a href="#GitBetter-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-257"><a href="#GitBetter-257"><span class="linenos">257</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
-</span><span id="GitBetter-258"><a href="#GitBetter-258"><span class="linenos">258</span></a>
-</span><span id="GitBetter-259"><a href="#GitBetter-259"><span class="linenos">259</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-260"><a href="#GitBetter-260"><span class="linenos">260</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-261"><a href="#GitBetter-261"><span class="linenos">261</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="GitBetter-262"><a href="#GitBetter-262"><span class="linenos">262</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-263"><a href="#GitBetter-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-264"><a href="#GitBetter-264"><span class="linenos">264</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
-</span><span id="GitBetter-265"><a href="#GitBetter-265"><span class="linenos">265</span></a>
-</span><span id="GitBetter-266"><a href="#GitBetter-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-267"><a href="#GitBetter-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="GitBetter-268"><a href="#GitBetter-268"><span class="linenos">268</span></a>
-</span><span id="GitBetter-269"><a href="#GitBetter-269"><span class="linenos">269</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter-270"><a href="#GitBetter-270"><span class="linenos">270</span></a>
-</span><span id="GitBetter-271"><a href="#GitBetter-271"><span class="linenos">271</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-272"><a href="#GitBetter-272"><span class="linenos">272</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="GitBetter-273"><a href="#GitBetter-273"><span class="linenos">273</span></a>
-</span><span id="GitBetter-274"><a href="#GitBetter-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-275"><a href="#GitBetter-275"><span class="linenos">275</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="GitBetter-276"><a href="#GitBetter-276"><span class="linenos">276</span></a>
-</span><span id="GitBetter-277"><a href="#GitBetter-277"><span class="linenos">277</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter-278"><a href="#GitBetter-278"><span class="linenos">278</span></a>
-</span><span id="GitBetter-279"><a href="#GitBetter-279"><span class="linenos">279</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-280"><a href="#GitBetter-280"><span class="linenos">280</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="GitBetter-281"><a href="#GitBetter-281"><span class="linenos">281</span></a>
-</span><span id="GitBetter-282"><a href="#GitBetter-282"><span class="linenos">282</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-283"><a href="#GitBetter-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="GitBetter-284"><a href="#GitBetter-284"><span class="linenos">284</span></a>
-</span><span id="GitBetter-285"><a href="#GitBetter-285"><span class="linenos">285</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter-286"><a href="#GitBetter-286"><span class="linenos">286</span></a>
-</span><span id="GitBetter-287"><a href="#GitBetter-287"><span class="linenos">287</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="GitBetter-288"><a href="#GitBetter-288"><span class="linenos">288</span></a>
-</span><span id="GitBetter-289"><a href="#GitBetter-289"><span class="linenos">289</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-290"><a href="#GitBetter-290"><span class="linenos">290</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-161"><a href="#GitBetter-161"><span class="linenos">161</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+</span><span id="GitBetter-162"><a href="#GitBetter-162"><span class="linenos">162</span></a>
+</span><span id="GitBetter-163"><a href="#GitBetter-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-164"><a href="#GitBetter-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-165"><a href="#GitBetter-165"><span class="linenos">165</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
+</span><span id="GitBetter-166"><a href="#GitBetter-166"><span class="linenos">166</span></a>
+</span><span id="GitBetter-167"><a href="#GitBetter-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-168"><a href="#GitBetter-168"><span class="linenos">168</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-169"><a href="#GitBetter-169"><span class="linenos">169</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+</span><span id="GitBetter-170"><a href="#GitBetter-170"><span class="linenos">170</span></a>
+</span><span id="GitBetter-171"><a href="#GitBetter-171"><span class="linenos">171</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-172"><a href="#GitBetter-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-173"><a href="#GitBetter-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="GitBetter-174"><a href="#GitBetter-174"><span class="linenos">174</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-175"><a href="#GitBetter-175"><span class="linenos">175</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="GitBetter-176"><a href="#GitBetter-176"><span class="linenos">176</span></a>
+</span><span id="GitBetter-177"><a href="#GitBetter-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-178"><a href="#GitBetter-178"><span class="linenos">178</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-179"><a href="#GitBetter-179"><span class="linenos">179</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter-180"><a href="#GitBetter-180"><span class="linenos">180</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="GitBetter-181"><a href="#GitBetter-181"><span class="linenos">181</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter-182"><a href="#GitBetter-182"><span class="linenos">182</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="GitBetter-183"><a href="#GitBetter-183"><span class="linenos">183</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-184"><a href="#GitBetter-184"><span class="linenos">184</span></a>
+</span><span id="GitBetter-185"><a href="#GitBetter-185"><span class="linenos">185</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-186"><a href="#GitBetter-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-187"><a href="#GitBetter-187"><span class="linenos">187</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-188"><a href="#GitBetter-188"><span class="linenos">188</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
+</span><span id="GitBetter-189"><a href="#GitBetter-189"><span class="linenos">189</span></a>
+</span><span id="GitBetter-190"><a href="#GitBetter-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-191"><a href="#GitBetter-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-192"><a href="#GitBetter-192"><span class="linenos">192</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter-193"><a href="#GitBetter-193"><span class="linenos">193</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="GitBetter-194"><a href="#GitBetter-194"><span class="linenos">194</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter-195"><a href="#GitBetter-195"><span class="linenos">195</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="GitBetter-196"><a href="#GitBetter-196"><span class="linenos">196</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="GitBetter-197"><a href="#GitBetter-197"><span class="linenos">197</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-198"><a href="#GitBetter-198"><span class="linenos">198</span></a>
+</span><span id="GitBetter-199"><a href="#GitBetter-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-200"><a href="#GitBetter-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-201"><a href="#GitBetter-201"><span class="linenos">201</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-202"><a href="#GitBetter-202"><span class="linenos">202</span></a>
+</span><span id="GitBetter-203"><a href="#GitBetter-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-204"><a href="#GitBetter-204"><span class="linenos">204</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-205"><a href="#GitBetter-205"><span class="linenos">205</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="GitBetter-206"><a href="#GitBetter-206"><span class="linenos">206</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-207"><a href="#GitBetter-207"><span class="linenos">207</span></a>
+</span><span id="GitBetter-208"><a href="#GitBetter-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-209"><a href="#GitBetter-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-210"><a href="#GitBetter-210"><span class="linenos">210</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-211"><a href="#GitBetter-211"><span class="linenos">211</span></a>
+</span><span id="GitBetter-212"><a href="#GitBetter-212"><span class="linenos">212</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-213"><a href="#GitBetter-213"><span class="linenos">213</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
+</span><span id="GitBetter-214"><a href="#GitBetter-214"><span class="linenos">214</span></a>
+</span><span id="GitBetter-215"><a href="#GitBetter-215"><span class="linenos">215</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-216"><a href="#GitBetter-216"><span class="linenos">216</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="GitBetter-217"><a href="#GitBetter-217"><span class="linenos">217</span></a>
+</span><span id="GitBetter-218"><a href="#GitBetter-218"><span class="linenos">218</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-219"><a href="#GitBetter-219"><span class="linenos">219</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
+</span><span id="GitBetter-220"><a href="#GitBetter-220"><span class="linenos">220</span></a>
+</span><span id="GitBetter-221"><a href="#GitBetter-221"><span class="linenos">221</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-222"><a href="#GitBetter-222"><span class="linenos">222</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+</span><span id="GitBetter-223"><a href="#GitBetter-223"><span class="linenos">223</span></a>
+</span><span id="GitBetter-224"><a href="#GitBetter-224"><span class="linenos">224</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-225"><a href="#GitBetter-225"><span class="linenos">225</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-226"><a href="#GitBetter-226"><span class="linenos">226</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
+</span><span id="GitBetter-227"><a href="#GitBetter-227"><span class="linenos">227</span></a>
+</span><span id="GitBetter-228"><a href="#GitBetter-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-229"><a href="#GitBetter-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-230"><a href="#GitBetter-230"><span class="linenos">230</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+</span><span id="GitBetter-231"><a href="#GitBetter-231"><span class="linenos">231</span></a>
+</span><span id="GitBetter-232"><a href="#GitBetter-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-233"><a href="#GitBetter-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-234"><a href="#GitBetter-234"><span class="linenos">234</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
+</span><span id="GitBetter-235"><a href="#GitBetter-235"><span class="linenos">235</span></a>
+</span><span id="GitBetter-236"><a href="#GitBetter-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-237"><a href="#GitBetter-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-238"><a href="#GitBetter-238"><span class="linenos">238</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-239"><a href="#GitBetter-239"><span class="linenos">239</span></a>
+</span><span id="GitBetter-240"><a href="#GitBetter-240"><span class="linenos">240</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-241"><a href="#GitBetter-241"><span class="linenos">241</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-242"><a href="#GitBetter-242"><span class="linenos">242</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="GitBetter-243"><a href="#GitBetter-243"><span class="linenos">243</span></a>
+</span><span id="GitBetter-244"><a href="#GitBetter-244"><span class="linenos">244</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-245"><a href="#GitBetter-245"><span class="linenos">245</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-246"><a href="#GitBetter-246"><span class="linenos">246</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-247"><a href="#GitBetter-247"><span class="linenos">247</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="GitBetter-248"><a href="#GitBetter-248"><span class="linenos">248</span></a>
+</span><span id="GitBetter-249"><a href="#GitBetter-249"><span class="linenos">249</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="GitBetter-250"><a href="#GitBetter-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-251"><a href="#GitBetter-251"><span class="linenos">251</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-252"><a href="#GitBetter-252"><span class="linenos">252</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+</span><span id="GitBetter-253"><a href="#GitBetter-253"><span class="linenos">253</span></a>
+</span><span id="GitBetter-254"><a href="#GitBetter-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-255"><a href="#GitBetter-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-256"><a href="#GitBetter-256"><span class="linenos">256</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+</span><span id="GitBetter-257"><a href="#GitBetter-257"><span class="linenos">257</span></a>
+</span><span id="GitBetter-258"><a href="#GitBetter-258"><span class="linenos">258</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-259"><a href="#GitBetter-259"><span class="linenos">259</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-260"><a href="#GitBetter-260"><span class="linenos">260</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="GitBetter-261"><a href="#GitBetter-261"><span class="linenos">261</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-262"><a href="#GitBetter-262"><span class="linenos">262</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-263"><a href="#GitBetter-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+</span><span id="GitBetter-264"><a href="#GitBetter-264"><span class="linenos">264</span></a>
+</span><span id="GitBetter-265"><a href="#GitBetter-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-266"><a href="#GitBetter-266"><span class="linenos">266</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="GitBetter-267"><a href="#GitBetter-267"><span class="linenos">267</span></a>
+</span><span id="GitBetter-268"><a href="#GitBetter-268"><span class="linenos">268</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-269"><a href="#GitBetter-269"><span class="linenos">269</span></a>
+</span><span id="GitBetter-270"><a href="#GitBetter-270"><span class="linenos">270</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-271"><a href="#GitBetter-271"><span class="linenos">271</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-272"><a href="#GitBetter-272"><span class="linenos">272</span></a>
+</span><span id="GitBetter-273"><a href="#GitBetter-273"><span class="linenos">273</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-274"><a href="#GitBetter-274"><span class="linenos">274</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="GitBetter-275"><a href="#GitBetter-275"><span class="linenos">275</span></a>
+</span><span id="GitBetter-276"><a href="#GitBetter-276"><span class="linenos">276</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-277"><a href="#GitBetter-277"><span class="linenos">277</span></a>
+</span><span id="GitBetter-278"><a href="#GitBetter-278"><span class="linenos">278</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-279"><a href="#GitBetter-279"><span class="linenos">279</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-280"><a href="#GitBetter-280"><span class="linenos">280</span></a>
+</span><span id="GitBetter-281"><a href="#GitBetter-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-282"><a href="#GitBetter-282"><span class="linenos">282</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="GitBetter-283"><a href="#GitBetter-283"><span class="linenos">283</span></a>
+</span><span id="GitBetter-284"><a href="#GitBetter-284"><span class="linenos">284</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-285"><a href="#GitBetter-285"><span class="linenos">285</span></a>
+</span><span id="GitBetter-286"><a href="#GitBetter-286"><span class="linenos">286</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="GitBetter-287"><a href="#GitBetter-287"><span class="linenos">287</span></a>
+</span><span id="GitBetter-288"><a href="#GitBetter-288"><span class="linenos">288</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-289"><a href="#GitBetter-289"><span class="linenos">289</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>GitBetter Shell.</p>
 </div>
 
 
@@ -1052,16 +1050,15 @@
     </div>
     <a class="headerlink" href="#GitBetter.do_new_gh_remote"></a>
             <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_new_gh_remote-156"><a href="#GitBetter.do_new_gh_remote-156"><span class="linenos">156</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">new_remote_parser</span><span class="p">)</span>
 </span><span id="GitBetter.do_new_gh_remote-157"><a href="#GitBetter.do_new_gh_remote-157"><span class="linenos">157</span></a>    <span class="k">def</span> <span class="nf">do_new_gh_remote</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
 </span><span id="GitBetter.do_new_gh_remote-158"><a href="#GitBetter.do_new_gh_remote-158"><span class="linenos">158</span></a>        <span class="sd">&quot;&quot;&quot;Create a remote GitHub repository for this repo.</span>
 </span><span id="GitBetter.do_new_gh_remote-159"><a href="#GitBetter.do_new_gh_remote-159"><span class="linenos">159</span></a>
 </span><span id="GitBetter.do_new_gh_remote-160"><a href="#GitBetter.do_new_gh_remote-160"><span class="linenos">160</span></a><span class="sd">        GitHub CLI must be installed and configured for this to work.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_new_gh_remote-161"><a href="#GitBetter.do_new_gh_remote-161"><span class="linenos">161</span></a>        <span class="n">name</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span>
-</span><span id="GitBetter.do_new_gh_remote-162"><a href="#GitBetter.do_new_gh_remote-162"><span class="linenos">162</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
+</span><span id="GitBetter.do_new_gh_remote-161"><a href="#GitBetter.do_new_gh_remote-161"><span class="linenos">161</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">create_remote_from_cwd</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">public</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create a remote GitHub repository for this repo.</p>
 
 <p>GitHub CLI must be installed and configured for this to work.</p>
 </div>
@@ -1075,17 +1072,17 @@
         <span class="def">def</span>
         <span class="name">do_initcommit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_initcommit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_initcommit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_initcommit-164"><a href="#GitBetter.do_initcommit-164"><span class="linenos">164</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_initcommit-165"><a href="#GitBetter.do_initcommit-165"><span class="linenos">165</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_initcommit-166"><a href="#GitBetter.do_initcommit-166"><span class="linenos">166</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_initcommit-163"><a href="#GitBetter.do_initcommit-163"><span class="linenos">163</span></a>    <span class="k">def</span> <span class="nf">do_initcommit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_initcommit-164"><a href="#GitBetter.do_initcommit-164"><span class="linenos">164</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with message &quot;Initial Commit&quot;.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_initcommit-165"><a href="#GitBetter.do_initcommit-165"><span class="linenos">165</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">initcommit</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit all files with message "Initial Commit".</p>
 </div>
 
 
@@ -1097,17 +1094,17 @@
         <span class="def">def</span>
         <span class="name">do_undo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_undo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_undo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_undo-168"><a href="#GitBetter.do_undo-168"><span class="linenos">168</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_undo-169"><a href="#GitBetter.do_undo-169"><span class="linenos">169</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_undo-170"><a href="#GitBetter.do_undo-170"><span class="linenos">170</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_undo-167"><a href="#GitBetter.do_undo-167"><span class="linenos">167</span></a>    <span class="k">def</span> <span class="nf">do_undo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_undo-168"><a href="#GitBetter.do_undo-168"><span class="linenos">168</span></a>        <span class="sd">&quot;&quot;&quot;Undo all uncommitted changes.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_undo-169"><a href="#GitBetter.do_undo-169"><span class="linenos">169</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">undo</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Undo all uncommitted changes.</p>
 </div>
 
 
@@ -1120,19 +1117,19 @@
         <span class="def">def</span>
         <span class="name">do_add</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_add-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_add"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add-172"><a href="#GitBetter.do_add-172"><span class="linenos">172</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_add-173"><a href="#GitBetter.do_add-173"><span class="linenos">173</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_add-174"><a href="#GitBetter.do_add-174"><span class="linenos">174</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="GitBetter.do_add-175"><a href="#GitBetter.do_add-175"><span class="linenos">175</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_add-176"><a href="#GitBetter.do_add-176"><span class="linenos">176</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add-171"><a href="#GitBetter.do_add-171"><span class="linenos">171</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_add-172"><a href="#GitBetter.do_add-172"><span class="linenos">172</span></a>    <span class="k">def</span> <span class="nf">do_add</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_add-173"><a href="#GitBetter.do_add-173"><span class="linenos">173</span></a>        <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="GitBetter.do_add-174"><a href="#GitBetter.do_add-174"><span class="linenos">174</span></a><span class="sd">        If no files are given, all files will be added.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_add-175"><a href="#GitBetter.do_add-175"><span class="linenos">175</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">(</span><span class="kc">None</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span> <span class="k">else</span> <span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage a list of files.
 If no files are given, all files will be added.</p>
 </div>
 
@@ -1145,21 +1142,21 @@
         <span class="def">def</span>
         <span class="name">do_commit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">message</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_commit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_commit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commit-178"><a href="#GitBetter.do_commit-178"><span class="linenos">178</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_commit-179"><a href="#GitBetter.do_commit-179"><span class="linenos">179</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commit-180"><a href="#GitBetter.do_commit-180"><span class="linenos">180</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commit-181"><a href="#GitBetter.do_commit-181"><span class="linenos">181</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter.do_commit-182"><a href="#GitBetter.do_commit-182"><span class="linenos">182</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commit-183"><a href="#GitBetter.do_commit-183"><span class="linenos">183</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter.do_commit-184"><a href="#GitBetter.do_commit-184"><span class="linenos">184</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commit-177"><a href="#GitBetter.do_commit-177"><span class="linenos">177</span></a>    <span class="k">def</span> <span class="nf">do_commit</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_commit-178"><a href="#GitBetter.do_commit-178"><span class="linenos">178</span></a>        <span class="sd">&quot;&quot;&quot;Commit staged files with this message.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_commit-179"><a href="#GitBetter.do_commit-179"><span class="linenos">179</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter.do_commit-180"><a href="#GitBetter.do_commit-180"><span class="linenos">180</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="GitBetter.do_commit-181"><a href="#GitBetter.do_commit-181"><span class="linenos">181</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter.do_commit-182"><a href="#GitBetter.do_commit-182"><span class="linenos">182</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="GitBetter.do_commit-183"><a href="#GitBetter.do_commit-183"><span class="linenos">183</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Commit staged files with this message.</p>
 </div>
 
 
@@ -1172,18 +1169,18 @@
         <span class="def">def</span>
         <span class="name">do_commitf</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_commitf-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_commitf"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitf-186"><a href="#GitBetter.do_commitf-186"><span class="linenos">186</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_commitf-187"><a href="#GitBetter.do_commitf-187"><span class="linenos">187</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitf-188"><a href="#GitBetter.do_commitf-188"><span class="linenos">188</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commitf-189"><a href="#GitBetter.do_commitf-189"><span class="linenos">189</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitf-185"><a href="#GitBetter.do_commitf-185"><span class="linenos">185</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">commit_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_commitf-186"><a href="#GitBetter.do_commitf-186"><span class="linenos">186</span></a>    <span class="k">def</span> <span class="nf">do_commitf</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitf-187"><a href="#GitBetter.do_commitf-187"><span class="linenos">187</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit a list of files.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_commitf-188"><a href="#GitBetter.do_commitf-188"><span class="linenos">188</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit_files</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">message</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit a list of files.</p>
 </div>
 
 
@@ -1195,22 +1192,22 @@
         <span class="def">def</span>
         <span class="name">do_commitall</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">message</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_commitall-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_commitall"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitall-191"><a href="#GitBetter.do_commitall-191"><span class="linenos">191</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitall-192"><a href="#GitBetter.do_commitall-192"><span class="linenos">192</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_commitall-193"><a href="#GitBetter.do_commitall-193"><span class="linenos">193</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitall-194"><a href="#GitBetter.do_commitall-194"><span class="linenos">194</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
-</span><span id="GitBetter.do_commitall-195"><a href="#GitBetter.do_commitall-195"><span class="linenos">195</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
-</span><span id="GitBetter.do_commitall-196"><a href="#GitBetter.do_commitall-196"><span class="linenos">196</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
-</span><span id="GitBetter.do_commitall-197"><a href="#GitBetter.do_commitall-197"><span class="linenos">197</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
-</span><span id="GitBetter.do_commitall-198"><a href="#GitBetter.do_commitall-198"><span class="linenos">198</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_commitall-190"><a href="#GitBetter.do_commitall-190"><span class="linenos">190</span></a>    <span class="k">def</span> <span class="nf">do_commitall</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitall-191"><a href="#GitBetter.do_commitall-191"><span class="linenos">191</span></a>        <span class="sd">&quot;&quot;&quot;Stage and commit all files with this message.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_commitall-192"><a href="#GitBetter.do_commitall-192"><span class="linenos">192</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitall-193"><a href="#GitBetter.do_commitall-193"><span class="linenos">193</span></a>            <span class="n">message</span> <span class="o">=</span> <span class="s1">&#39;&quot;&#39;</span> <span class="o">+</span> <span class="n">message</span>
+</span><span id="GitBetter.do_commitall-194"><a href="#GitBetter.do_commitall-194"><span class="linenos">194</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">message</span><span class="o">.</span><span class="n">endswith</span><span class="p">(</span><span class="s1">&#39;&quot;&#39;</span><span class="p">):</span>
+</span><span id="GitBetter.do_commitall-195"><a href="#GitBetter.do_commitall-195"><span class="linenos">195</span></a>            <span class="n">message</span> <span class="o">+=</span> <span class="s1">&#39;&quot;&#39;</span>
+</span><span id="GitBetter.do_commitall-196"><a href="#GitBetter.do_commitall-196"><span class="linenos">196</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add</span><span class="p">()</span>
+</span><span id="GitBetter.do_commitall-197"><a href="#GitBetter.do_commitall-197"><span class="linenos">197</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-m </span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit all files with this message.</p>
 </div>
 
 
@@ -1222,17 +1219,17 @@
         <span class="def">def</span>
         <span class="name">do_switch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_switch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_switch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_switch-200"><a href="#GitBetter.do_switch-200"><span class="linenos">200</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_switch-201"><a href="#GitBetter.do_switch-201"><span class="linenos">201</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_switch-202"><a href="#GitBetter.do_switch-202"><span class="linenos">202</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_switch-199"><a href="#GitBetter.do_switch-199"><span class="linenos">199</span></a>    <span class="k">def</span> <span class="nf">do_switch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_switch-200"><a href="#GitBetter.do_switch-200"><span class="linenos">200</span></a>        <span class="sd">&quot;&quot;&quot;Switch to this branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_switch-201"><a href="#GitBetter.do_switch-201"><span class="linenos">201</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Switch to this branch.</p>
 </div>
 
 
@@ -1244,22 +1241,22 @@
         <span class="def">def</span>
         <span class="name">do_add_url</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">url</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_add_url-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_add_url"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add_url-204"><a href="#GitBetter.do_add_url-204"><span class="linenos">204</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_add_url-205"><a href="#GitBetter.do_add_url-205"><span class="linenos">205</span></a>        <span class="sd">&quot;&quot;&quot;Add remote url for repo and push repo.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_add_url-206"><a href="#GitBetter.do_add_url-206"><span class="linenos">206</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
-</span><span id="GitBetter.do_add_url-207"><a href="#GitBetter.do_add_url-207"><span class="linenos">207</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_add_url-203"><a href="#GitBetter.do_add_url-203"><span class="linenos">203</span></a>    <span class="k">def</span> <span class="nf">do_add_url</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_add_url-204"><a href="#GitBetter.do_add_url-204"><span class="linenos">204</span></a>        <span class="sd">&quot;&quot;&quot;Add remote origin url for repo and push repo.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_add_url-205"><a href="#GitBetter.do_add_url-205"><span class="linenos">205</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">)</span>
+</span><span id="GitBetter.do_add_url-206"><a href="#GitBetter.do_add_url-206"><span class="linenos">206</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="s2">&quot;-u origin main&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
-            <div class="docstring"><p>Add remote url for repo and push repo.</p>
+            <div class="docstring"><p>Add remote origin url for repo and push repo.</p>
 </div>
 
 
                             </div>
                             <div id="GitBetter.do_push_new" class="classattr">
                                         <input id="GitBetter.do_push_new-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -1267,17 +1264,17 @@
         <span class="def">def</span>
         <span class="name">do_push_new</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_push_new-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_push_new"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push_new-209"><a href="#GitBetter.do_push_new-209"><span class="linenos">209</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_push_new-210"><a href="#GitBetter.do_push_new-210"><span class="linenos">210</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_push_new-211"><a href="#GitBetter.do_push_new-211"><span class="linenos">211</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push_new-208"><a href="#GitBetter.do_push_new-208"><span class="linenos">208</span></a>    <span class="k">def</span> <span class="nf">do_push_new</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_push_new-209"><a href="#GitBetter.do_push_new-209"><span class="linenos">209</span></a>        <span class="sd">&quot;&quot;&quot;Push this new branch to origin with -u flag.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_push_new-210"><a href="#GitBetter.do_push_new-210"><span class="linenos">210</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Push this new branch to origin with -u flag.</p>
 </div>
 
 
@@ -1289,19 +1286,19 @@
         <span class="def">def</span>
         <span class="name">do_push</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_push-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_push"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push-213"><a href="#GitBetter.do_push-213"><span class="linenos">213</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_push-214"><a href="#GitBetter.do_push-214"><span class="linenos">214</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
-</span><span id="GitBetter.do_push-215"><a href="#GitBetter.do_push-215"><span class="linenos">215</span></a>
-</span><span id="GitBetter.do_push-216"><a href="#GitBetter.do_push-216"><span class="linenos">216</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_push-217"><a href="#GitBetter.do_push-217"><span class="linenos">217</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_push-212"><a href="#GitBetter.do_push-212"><span class="linenos">212</span></a>    <span class="k">def</span> <span class="nf">do_push</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_push-213"><a href="#GitBetter.do_push-213"><span class="linenos">213</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git push`.</span>
+</span><span id="GitBetter.do_push-214"><a href="#GitBetter.do_push-214"><span class="linenos">214</span></a>
+</span><span id="GitBetter.do_push-215"><a href="#GitBetter.do_push-215"><span class="linenos">215</span></a><span class="sd">        `args` can be any additional args that `git push` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_push-216"><a href="#GitBetter.do_push-216"><span class="linenos">216</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">push</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git push</code>.</p>
 
 <p><code>args</code> can be any additional args that <code>git push</code> accepts.</p>
 </div>
@@ -1315,43 +1312,43 @@
         <span class="def">def</span>
         <span class="name">do_pull</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_pull-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_pull"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull-219"><a href="#GitBetter.do_pull-219"><span class="linenos">219</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_pull-220"><a href="#GitBetter.do_pull-220"><span class="linenos">220</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
-</span><span id="GitBetter.do_pull-221"><a href="#GitBetter.do_pull-221"><span class="linenos">221</span></a>
-</span><span id="GitBetter.do_pull-222"><a href="#GitBetter.do_pull-222"><span class="linenos">222</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_pull-223"><a href="#GitBetter.do_pull-223"><span class="linenos">223</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull-218"><a href="#GitBetter.do_pull-218"><span class="linenos">218</span></a>    <span class="k">def</span> <span class="nf">do_pull</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_pull-219"><a href="#GitBetter.do_pull-219"><span class="linenos">219</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git pull`.</span>
+</span><span id="GitBetter.do_pull-220"><a href="#GitBetter.do_pull-220"><span class="linenos">220</span></a>
+</span><span id="GitBetter.do_pull-221"><a href="#GitBetter.do_pull-221"><span class="linenos">221</span></a><span class="sd">        `args` can be any additional args that `git pull` accepts.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_pull-222"><a href="#GitBetter.do_pull-222"><span class="linenos">222</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull</span><span class="p">(</span><span class="n">args</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git pull</code>.</p>
 
 <p><code>args</code> can be any additional args that <code>git pull</code> accepts.</p>
 </div>
 
 
                             </div>
-                            <div id="GitBetter.do_list_branches" class="classattr">
-                                        <input id="GitBetter.do_list_branches-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                            <div id="GitBetter.do_branches" class="classattr">
+                                        <input id="GitBetter.do_branches-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">do_list_branches</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
+        <span class="name">do_branches</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
-                <label class="view-source-button" for="GitBetter.do_list_branches-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="GitBetter.do_branches-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#GitBetter.do_list_branches"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_list_branches-225"><a href="#GitBetter.do_list_branches-225"><span class="linenos">225</span></a>    <span class="k">def</span> <span class="nf">do_list_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_list_branches-226"><a href="#GitBetter.do_list_branches-226"><span class="linenos">226</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_list_branches-227"><a href="#GitBetter.do_list_branches-227"><span class="linenos">227</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
+    <a class="headerlink" href="#GitBetter.do_branches"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_branches-224"><a href="#GitBetter.do_branches-224"><span class="linenos">224</span></a>    <span class="k">def</span> <span class="nf">do_branches</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_branches-225"><a href="#GitBetter.do_branches-225"><span class="linenos">225</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_branches-226"><a href="#GitBetter.do_branches-226"><span class="linenos">226</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Show local and remote branches.</p>
 </div>
 
 
@@ -1363,17 +1360,17 @@
         <span class="def">def</span>
         <span class="name">do_loggy</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_loggy-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_loggy"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_loggy-229"><a href="#GitBetter.do_loggy-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_loggy-230"><a href="#GitBetter.do_loggy-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_loggy-231"><a href="#GitBetter.do_loggy-231"><span class="linenos">231</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_loggy-228"><a href="#GitBetter.do_loggy-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_loggy-229"><a href="#GitBetter.do_loggy-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_loggy-230"><a href="#GitBetter.do_loggy-230"><span class="linenos">230</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git --oneline --name-only --abbrev-commit --graph</code>.</p>
 </div>
 
 
@@ -1385,17 +1382,17 @@
         <span class="def">def</span>
         <span class="name">do_status</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_status-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_status"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_status-233"><a href="#GitBetter.do_status-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_status-234"><a href="#GitBetter.do_status-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_status-235"><a href="#GitBetter.do_status-235"><span class="linenos">235</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_status-232"><a href="#GitBetter.do_status-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_status-233"><a href="#GitBetter.do_status-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_status-234"><a href="#GitBetter.do_status-234"><span class="linenos">234</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Execute <code>git status</code>.</p>
 </div>
 
 
@@ -1407,17 +1404,17 @@
         <span class="def">def</span>
         <span class="name">do_merge</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_merge-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_merge"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_merge-237"><a href="#GitBetter.do_merge-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_merge-238"><a href="#GitBetter.do_merge-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_merge-239"><a href="#GitBetter.do_merge-239"><span class="linenos">239</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_merge-236"><a href="#GitBetter.do_merge-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_merge-237"><a href="#GitBetter.do_merge-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_merge-238"><a href="#GitBetter.do_merge-238"><span class="linenos">238</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Merge supplied <code>branch_name</code> with the currently active branch.</p>
 </div>
 
 
@@ -1429,17 +1426,17 @@
         <span class="def">def</span>
         <span class="name">do_tag</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_tag-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_tag"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_tag-241"><a href="#GitBetter.do_tag-241"><span class="linenos">241</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_tag-242"><a href="#GitBetter.do_tag-242"><span class="linenos">242</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_tag-243"><a href="#GitBetter.do_tag-243"><span class="linenos">243</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_tag-240"><a href="#GitBetter.do_tag-240"><span class="linenos">240</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_tag-241"><a href="#GitBetter.do_tag-241"><span class="linenos">241</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_tag-242"><a href="#GitBetter.do_tag-242"><span class="linenos">242</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Tag current commit with <code>tag_id</code>.</p>
 </div>
 
 
@@ -1452,18 +1449,18 @@
         <span class="def">def</span>
         <span class="name">do_amend</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_amend-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_amend"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_amend-245"><a href="#GitBetter.do_amend-245"><span class="linenos">245</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_amend-246"><a href="#GitBetter.do_amend-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_amend-247"><a href="#GitBetter.do_amend-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_amend-248"><a href="#GitBetter.do_amend-248"><span class="linenos">248</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_amend-244"><a href="#GitBetter.do_amend-244"><span class="linenos">244</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_amend-245"><a href="#GitBetter.do_amend-245"><span class="linenos">245</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_amend-246"><a href="#GitBetter.do_amend-246"><span class="linenos">246</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_amend-247"><a href="#GitBetter.do_amend-247"><span class="linenos">247</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage files and add to previous commit.</p>
 </div>
 
 
@@ -1476,18 +1473,18 @@
         <span class="def">def</span>
         <span class="name">do_delete_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_delete_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_delete_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_branch-250"><a href="#GitBetter.do_delete_branch-250"><span class="linenos">250</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="GitBetter.do_delete_branch-251"><a href="#GitBetter.do_delete_branch-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_delete_branch-252"><a href="#GitBetter.do_delete_branch-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_delete_branch-253"><a href="#GitBetter.do_delete_branch-253"><span class="linenos">253</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_branch-249"><a href="#GitBetter.do_delete_branch-249"><span class="linenos">249</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="GitBetter.do_delete_branch-250"><a href="#GitBetter.do_delete_branch-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_delete_branch-251"><a href="#GitBetter.do_delete_branch-251"><span class="linenos">251</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_delete_branch-252"><a href="#GitBetter.do_delete_branch-252"><span class="linenos">252</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete branch.</p>
 </div>
 
 
@@ -1499,17 +1496,17 @@
         <span class="def">def</span>
         <span class="name">do_pull_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_pull_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_pull_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull_branch-255"><a href="#GitBetter.do_pull_branch-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_pull_branch-256"><a href="#GitBetter.do_pull_branch-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_pull_branch-257"><a href="#GitBetter.do_pull_branch-257"><span class="linenos">257</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull_branch-254"><a href="#GitBetter.do_pull_branch-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_pull_branch-255"><a href="#GitBetter.do_pull_branch-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_pull_branch-256"><a href="#GitBetter.do_pull_branch-256"><span class="linenos">256</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Pull this branch from the origin.</p>
 </div>
 
 
@@ -1521,20 +1518,20 @@
         <span class="def">def</span>
         <span class="name">do_ignore</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_ignore-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_ignore"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_ignore-259"><a href="#GitBetter.do_ignore-259"><span class="linenos">259</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_ignore-260"><a href="#GitBetter.do_ignore-260"><span class="linenos">260</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_ignore-261"><a href="#GitBetter.do_ignore-261"><span class="linenos">261</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="GitBetter.do_ignore-262"><a href="#GitBetter.do_ignore-262"><span class="linenos">262</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="GitBetter.do_ignore-263"><a href="#GitBetter.do_ignore-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter.do_ignore-264"><a href="#GitBetter.do_ignore-264"><span class="linenos">264</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_ignore-258"><a href="#GitBetter.do_ignore-258"><span class="linenos">258</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_ignore-259"><a href="#GitBetter.do_ignore-259"><span class="linenos">259</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_ignore-260"><a href="#GitBetter.do_ignore-260"><span class="linenos">260</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="GitBetter.do_ignore-261"><a href="#GitBetter.do_ignore-261"><span class="linenos">261</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="GitBetter.do_ignore-262"><a href="#GitBetter.do_ignore-262"><span class="linenos">262</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter.do_ignore-263"><a href="#GitBetter.do_ignore-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add the list of patterns to <code>.gitignore</code>.</p>
 </div>
 
 
@@ -1546,21 +1543,21 @@
         <span class="def">def</span>
         <span class="name">do_make_private</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_make_private-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_make_private"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_private-266"><a href="#GitBetter.do_make_private-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_make_private-267"><a href="#GitBetter.do_make_private-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="GitBetter.do_make_private-268"><a href="#GitBetter.do_make_private-268"><span class="linenos">268</span></a>
-</span><span id="GitBetter.do_make_private-269"><a href="#GitBetter.do_make_private-269"><span class="linenos">269</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_make_private-270"><a href="#GitBetter.do_make_private-270"><span class="linenos">270</span></a>
-</span><span id="GitBetter.do_make_private-271"><a href="#GitBetter.do_make_private-271"><span class="linenos">271</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_make_private-272"><a href="#GitBetter.do_make_private-272"><span class="linenos">272</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_private-265"><a href="#GitBetter.do_make_private-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_make_private-266"><a href="#GitBetter.do_make_private-266"><span class="linenos">266</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="GitBetter.do_make_private-267"><a href="#GitBetter.do_make_private-267"><span class="linenos">267</span></a>
+</span><span id="GitBetter.do_make_private-268"><a href="#GitBetter.do_make_private-268"><span class="linenos">268</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_make_private-269"><a href="#GitBetter.do_make_private-269"><span class="linenos">269</span></a>
+</span><span id="GitBetter.do_make_private-270"><a href="#GitBetter.do_make_private-270"><span class="linenos">270</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_make_private-271"><a href="#GitBetter.do_make_private-271"><span class="linenos">271</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make the GitHub remote for this repo private.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1576,21 +1573,21 @@
         <span class="def">def</span>
         <span class="name">do_make_public</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_make_public-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_make_public"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_public-274"><a href="#GitBetter.do_make_public-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_make_public-275"><a href="#GitBetter.do_make_public-275"><span class="linenos">275</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="GitBetter.do_make_public-276"><a href="#GitBetter.do_make_public-276"><span class="linenos">276</span></a>
-</span><span id="GitBetter.do_make_public-277"><a href="#GitBetter.do_make_public-277"><span class="linenos">277</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_make_public-278"><a href="#GitBetter.do_make_public-278"><span class="linenos">278</span></a>
-</span><span id="GitBetter.do_make_public-279"><a href="#GitBetter.do_make_public-279"><span class="linenos">279</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_make_public-280"><a href="#GitBetter.do_make_public-280"><span class="linenos">280</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_public-273"><a href="#GitBetter.do_make_public-273"><span class="linenos">273</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_make_public-274"><a href="#GitBetter.do_make_public-274"><span class="linenos">274</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="GitBetter.do_make_public-275"><a href="#GitBetter.do_make_public-275"><span class="linenos">275</span></a>
+</span><span id="GitBetter.do_make_public-276"><a href="#GitBetter.do_make_public-276"><span class="linenos">276</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_make_public-277"><a href="#GitBetter.do_make_public-277"><span class="linenos">277</span></a>
+</span><span id="GitBetter.do_make_public-278"><a href="#GitBetter.do_make_public-278"><span class="linenos">278</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_make_public-279"><a href="#GitBetter.do_make_public-279"><span class="linenos">279</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make the GitHub remote for this repo public.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1606,23 +1603,23 @@
         <span class="def">def</span>
         <span class="name">do_delete_gh_repo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_delete_gh_repo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_delete_gh_repo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_gh_repo-282"><a href="#GitBetter.do_delete_gh_repo-282"><span class="linenos">282</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_delete_gh_repo-283"><a href="#GitBetter.do_delete_gh_repo-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="GitBetter.do_delete_gh_repo-284"><a href="#GitBetter.do_delete_gh_repo-284"><span class="linenos">284</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-285"><a href="#GitBetter.do_delete_gh_repo-285"><span class="linenos">285</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_delete_gh_repo-286"><a href="#GitBetter.do_delete_gh_repo-286"><span class="linenos">286</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-287"><a href="#GitBetter.do_delete_gh_repo-287"><span class="linenos">287</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
-</span><span id="GitBetter.do_delete_gh_repo-288"><a href="#GitBetter.do_delete_gh_repo-288"><span class="linenos">288</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-289"><a href="#GitBetter.do_delete_gh_repo-289"><span class="linenos">289</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_delete_gh_repo-290"><a href="#GitBetter.do_delete_gh_repo-290"><span class="linenos">290</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_gh_repo-281"><a href="#GitBetter.do_delete_gh_repo-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_delete_gh_repo-282"><a href="#GitBetter.do_delete_gh_repo-282"><span class="linenos">282</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
+</span><span id="GitBetter.do_delete_gh_repo-283"><a href="#GitBetter.do_delete_gh_repo-283"><span class="linenos">283</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-284"><a href="#GitBetter.do_delete_gh_repo-284"><span class="linenos">284</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_delete_gh_repo-285"><a href="#GitBetter.do_delete_gh_repo-285"><span class="linenos">285</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-286"><a href="#GitBetter.do_delete_gh_repo-286"><span class="linenos">286</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="GitBetter.do_delete_gh_repo-287"><a href="#GitBetter.do_delete_gh_repo-287"><span class="linenos">287</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-288"><a href="#GitBetter.do_delete_gh_repo-288"><span class="linenos">288</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_delete_gh_repo-289"><a href="#GitBetter.do_delete_gh_repo-289"><span class="linenos">289</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete this repo from GitHub.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1670,16 +1667,16 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-293"><a href="#main-293"><span class="linenos">293</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="main-294"><a href="#main-294"><span class="linenos">294</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-292"><a href="#main-292"><span class="linenos">292</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="main-293"><a href="#main-293"><span class="linenos">293</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -25,15 +25,15 @@
           o do_commitf
           o do_commitall
           o do_switch
           o do_add_url
           o do_push_new
           o do_push
           o do_pull
-          o do_list_branches
+          o do_branches
           o do_loggy
           o do_status
           o do_merge
           o do_tag
           o do_amend
           o do_delete_branch
           o do_pull_branch
@@ -178,16 +178,17 @@
 119                    "^Essentially makes this shell function as a super-shell
 of whatever shell you launched gitbetter from.^"
 120                )
 121        print()
 122
 123    @property
 124    def unrecognized_command_behavior_status(self):
-125        return f"Unrecognized command behavior: {'Execute with os.system()'
-if self.execute_in_terminal_if_unrecognized else 'Print unknown syntax error'}"
+125        return f"Unrecognized command behavior: {'Execute in shell with
+os.system()' if self.execute_in_terminal_if_unrecognized else 'Print unknown
+syntax error'}"
 126
 127    def do_toggle_unrecognized_command_behavior(self, arg: str):
 128        """Toggle whether the shell will attempt to execute unrecognized
 commands as system commands in the terminal.
 129        When on (the default), `GitBetter` will treat unrecognized commands
 as if you added the `sys` command in front of the input, i.e. `os.system
 (your_input)`.
@@ -219,157 +220,156 @@
 153        git.create_new_branch(name)
 154
 155    @with_parser(new_remote_parser)
 156    def do_new_gh_remote(self, args: Namespace):
 157        """Create a remote GitHub repository for this repo.
 158
 159        GitHub CLI must be installed and configured for this to work."""
-160        name = Pathier.cwd().stem
-161        git.create_remote(name, args.public)
-162
-163    def do_initcommit(self, _: str):
-164        """Stage and commit all files with message "Initial Commit"."""
-165        git.initcommit()
-166
-167    def do_undo(self, _: str):
-168        """Undo all uncommitted changes."""
-169        git.undo()
-170
-171    @with_parser(amend_files_parser, [files_postparser])
-172    def do_add(self, args: Namespace):
-173        """Stage a list of files.
-174        If no files are given, all files will be added."""
-175        git.add(None if not args.files else args.files)
-176
-177    def do_commit(self, message: str):
-178        """Commit staged files with this message."""
-179        if not message.startswith('"'):
-180            message = '"' + message
-181        if not message.endswith('"'):
-182            message += '"'
-183        git.commit(f"-m {message}")
-184
-185    @with_parser(commit_files_parser, [files_postparser])
-186    def do_commitf(self, args: Namespace):
-187        """Stage and commit a list of files."""
-188        git.commit_files(args.files, args.message)
-189
-190    def do_commitall(self, message: str):
-191        """Stage and commit all files with this message."""
-192        if not message.startswith('"'):
-193            message = '"' + message
-194        if not message.endswith('"'):
-195            message += '"'
-196        git.add()
-197        git.commit(f"-m {message}")
-198
-199    def do_switch(self, branch_name: str):
-200        """Switch to this branch."""
-201        git.switch_branch(branch_name)
-202
-203    def do_add_url(self, url: str):
-204        """Add remote url for repo and push repo."""
-205        git.add_remote_url(url)
-206        git.push("-u origin main")
-207
-208    def do_push_new(self, branch_name: str):
-209        """Push this new branch to origin with -u flag."""
-210        git.push_new_branch(branch_name)
-211
-212    def do_push(self, args: str):
-213        """Execute `git push`.
-214
-215        `args` can be any additional args that `git push` accepts."""
-216        git.push(args)
-217
-218    def do_pull(self, args: str):
-219        """Execute `git pull`.
-220
-221        `args` can be any additional args that `git pull` accepts."""
-222        git.pull(args)
-223
-224    def do_list_branches(self, _: str):
-225        """Show local and remote branches."""
-226        git.list_branches()
-227
-228    def do_loggy(self, _: str):
-229        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
-230        git.loggy()
-231
-232    def do_status(self, _: str):
-233        """Execute `git status`."""
-234        git.status()
-235
-236    def do_merge(self, branch_name: str):
-237        """Merge supplied `branch_name` with the currently active branch."""
-238        git.merge(branch_name)
-239
-240    def do_tag(self, tag_id: str):
-241        """Tag current commit with `tag_id`."""
-242        git.tag(tag_id)
-243
-244    @with_parser(amend_files_parser, [files_postparser])
-245    def do_amend(self, args: Namespace):
-246        """Stage files and add to previous commit."""
-247        git.amend(args.files)
-248
-249    @with_parser(delete_branch_parser)
-250    def do_delete_branch(self, args: Namespace):
-251        """Delete branch."""
-252        git.delete_branch(args.branch, not args.remote)
-253
-254    def do_pull_branch(self, branch: str):
-255        """Pull this branch from the origin."""
-256        git.pull_branch(branch)
-257
-258    def do_ignore(self, patterns: str):
-259        """Add the list of patterns to `.gitignore`."""
-260        patterns = "\n".join(patterns.split())
-261        path = Pathier(".gitignore")
-262        path.append("\n")
-263        path.append(patterns, False)
-264
-265    def do_make_private(self, owner: str):
-266        """Make the GitHub remote for this repo private.
-267
-268        Expects an argument for the repo owner, i.e. the `OWNER` in
+160        git.create_remote_from_cwd(args.public)
+161
+162    def do_initcommit(self, _: str):
+163        """Stage and commit all files with message "Initial Commit"."""
+164        git.initcommit()
+165
+166    def do_undo(self, _: str):
+167        """Undo all uncommitted changes."""
+168        git.undo()
+169
+170    @with_parser(amend_files_parser, [files_postparser])
+171    def do_add(self, args: Namespace):
+172        """Stage a list of files.
+173        If no files are given, all files will be added."""
+174        git.add(None if not args.files else args.files)
+175
+176    def do_commit(self, message: str):
+177        """Commit staged files with this message."""
+178        if not message.startswith('"'):
+179            message = '"' + message
+180        if not message.endswith('"'):
+181            message += '"'
+182        git.commit(f"-m {message}")
+183
+184    @with_parser(commit_files_parser, [files_postparser])
+185    def do_commitf(self, args: Namespace):
+186        """Stage and commit a list of files."""
+187        git.commit_files(args.files, args.message)
+188
+189    def do_commitall(self, message: str):
+190        """Stage and commit all files with this message."""
+191        if not message.startswith('"'):
+192            message = '"' + message
+193        if not message.endswith('"'):
+194            message += '"'
+195        git.add()
+196        git.commit(f"-m {message}")
+197
+198    def do_switch(self, branch_name: str):
+199        """Switch to this branch."""
+200        git.switch_branch(branch_name)
+201
+202    def do_add_url(self, url: str):
+203        """Add remote origin url for repo and push repo."""
+204        git.add_remote_url(url)
+205        git.push("-u origin main")
+206
+207    def do_push_new(self, branch_name: str):
+208        """Push this new branch to origin with -u flag."""
+209        git.push_new_branch(branch_name)
+210
+211    def do_push(self, args: str):
+212        """Execute `git push`.
+213
+214        `args` can be any additional args that `git push` accepts."""
+215        git.push(args)
+216
+217    def do_pull(self, args: str):
+218        """Execute `git pull`.
+219
+220        `args` can be any additional args that `git pull` accepts."""
+221        git.pull(args)
+222
+223    def do_branches(self, _: str):
+224        """Show local and remote branches."""
+225        git.list_branches()
+226
+227    def do_loggy(self, _: str):
+228        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
+229        git.loggy()
+230
+231    def do_status(self, _: str):
+232        """Execute `git status`."""
+233        git.status()
+234
+235    def do_merge(self, branch_name: str):
+236        """Merge supplied `branch_name` with the currently active branch."""
+237        git.merge(branch_name)
+238
+239    def do_tag(self, tag_id: str):
+240        """Tag current commit with `tag_id`."""
+241        git.tag(tag_id)
+242
+243    @with_parser(amend_files_parser, [files_postparser])
+244    def do_amend(self, args: Namespace):
+245        """Stage files and add to previous commit."""
+246        git.amend(args.files)
+247
+248    @with_parser(delete_branch_parser)
+249    def do_delete_branch(self, args: Namespace):
+250        """Delete branch."""
+251        git.delete_branch(args.branch, not args.remote)
+252
+253    def do_pull_branch(self, branch: str):
+254        """Pull this branch from the origin."""
+255        git.pull_branch(branch)
+256
+257    def do_ignore(self, patterns: str):
+258        """Add the list of patterns to `.gitignore`."""
+259        patterns = "\n".join(patterns.split())
+260        path = Pathier(".gitignore")
+261        path.append("\n")
+262        path.append(patterns, False)
+263
+264    def do_make_private(self, owner: str):
+265        """Make the GitHub remote for this repo private.
+266
+267        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-269
-270        This repo must exist and GitHub CLI must be installed and
+268
+269        This repo must exist and GitHub CLI must be installed and
 configured."""
-271        git.make_private(owner, Pathier.cwd().stem)
-272
-273    def do_make_public(self, owner: str):
-274        """Make the GitHub remote for this repo public.
-275
-276        Expects an argument for the repo owner, i.e. the `OWNER` in
+270        git.make_private(owner, Pathier.cwd().stem)
+271
+272    def do_make_public(self, owner: str):
+273        """Make the GitHub remote for this repo public.
+274
+275        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-277
-278        This repo must exist and GitHub CLI must be installed and
+276
+277        This repo must exist and GitHub CLI must be installed and
 configured."""
-279        git.make_public(owner, Pathier.cwd().stem)
-280
-281    def do_delete_gh_repo(self, owner: str):
-282        """Delete this repo from GitHub.
-283
-284        Expects an argument for the repo owner, i.e. the `OWNER` in
+278        git.make_public(owner, Pathier.cwd().stem)
+279
+280    def do_delete_gh_repo(self, owner: str):
+281        """Delete this repo from GitHub.
+282
+283        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-285
-286        GitHub CLI must be installed and configured.
-287
-288        May require you to reauthorize and rerun command."""
-289        git.delete_remote(owner, Pathier.cwd().stem)
+284
+285        GitHub CLI must be installed and configured.
+286
+287        May require you to reauthorize and rerun command."""
+288        git.delete_remote(owner, Pathier.cwd().stem)
+289
 290
-291
-292def main():
-293    GitBetter().cmdloop()
+291def main():
+292    GitBetter().cmdloop()
+293
 294
-295
-296if __name__ == "__main__":
-297    main()
+295if __name__ == "__main__":
+296    main()
   ⁰
 def new_remote_parser() -> argshell.argshell.ArgShellParser: View Source
 10def new_remote_parser() -> ArgShellParser:
 11    parser = ArgShellParser()
 12    parser.add_argument(
 13        "--public",
 14        action="store_true",
@@ -493,16 +493,17 @@
 120                    "^Essentially makes this shell function as a super-shell
 of whatever shell you launched gitbetter from.^"
 121                )
 122        print()
 123
 124    @property
 125    def unrecognized_command_behavior_status(self):
-126        return f"Unrecognized command behavior: {'Execute with os.system()'
-if self.execute_in_terminal_if_unrecognized else 'Print unknown syntax error'}"
+126        return f"Unrecognized command behavior: {'Execute in shell with
+os.system()' if self.execute_in_terminal_if_unrecognized else 'Print unknown
+syntax error'}"
 127
 128    def do_toggle_unrecognized_command_behavior(self, arg: str):
 129        """Toggle whether the shell will attempt to execute unrecognized
 commands as system commands in the terminal.
 130        When on (the default), `GitBetter` will treat unrecognized commands
 as if you added the `sys` command in front of the input, i.e. `os.system
 (your_input)`.
@@ -534,149 +535,148 @@
 154        git.create_new_branch(name)
 155
 156    @with_parser(new_remote_parser)
 157    def do_new_gh_remote(self, args: Namespace):
 158        """Create a remote GitHub repository for this repo.
 159
 160        GitHub CLI must be installed and configured for this to work."""
-161        name = Pathier.cwd().stem
-162        git.create_remote(name, args.public)
-163
-164    def do_initcommit(self, _: str):
-165        """Stage and commit all files with message "Initial Commit"."""
-166        git.initcommit()
-167
-168    def do_undo(self, _: str):
-169        """Undo all uncommitted changes."""
-170        git.undo()
-171
-172    @with_parser(amend_files_parser, [files_postparser])
-173    def do_add(self, args: Namespace):
-174        """Stage a list of files.
-175        If no files are given, all files will be added."""
-176        git.add(None if not args.files else args.files)
-177
-178    def do_commit(self, message: str):
-179        """Commit staged files with this message."""
-180        if not message.startswith('"'):
-181            message = '"' + message
-182        if not message.endswith('"'):
-183            message += '"'
-184        git.commit(f"-m {message}")
-185
-186    @with_parser(commit_files_parser, [files_postparser])
-187    def do_commitf(self, args: Namespace):
-188        """Stage and commit a list of files."""
-189        git.commit_files(args.files, args.message)
-190
-191    def do_commitall(self, message: str):
-192        """Stage and commit all files with this message."""
-193        if not message.startswith('"'):
-194            message = '"' + message
-195        if not message.endswith('"'):
-196            message += '"'
-197        git.add()
-198        git.commit(f"-m {message}")
-199
-200    def do_switch(self, branch_name: str):
-201        """Switch to this branch."""
-202        git.switch_branch(branch_name)
-203
-204    def do_add_url(self, url: str):
-205        """Add remote url for repo and push repo."""
-206        git.add_remote_url(url)
-207        git.push("-u origin main")
-208
-209    def do_push_new(self, branch_name: str):
-210        """Push this new branch to origin with -u flag."""
-211        git.push_new_branch(branch_name)
-212
-213    def do_push(self, args: str):
-214        """Execute `git push`.
-215
-216        `args` can be any additional args that `git push` accepts."""
-217        git.push(args)
-218
-219    def do_pull(self, args: str):
-220        """Execute `git pull`.
-221
-222        `args` can be any additional args that `git pull` accepts."""
-223        git.pull(args)
-224
-225    def do_list_branches(self, _: str):
-226        """Show local and remote branches."""
-227        git.list_branches()
-228
-229    def do_loggy(self, _: str):
-230        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
-231        git.loggy()
-232
-233    def do_status(self, _: str):
-234        """Execute `git status`."""
-235        git.status()
-236
-237    def do_merge(self, branch_name: str):
-238        """Merge supplied `branch_name` with the currently active branch."""
-239        git.merge(branch_name)
-240
-241    def do_tag(self, tag_id: str):
-242        """Tag current commit with `tag_id`."""
-243        git.tag(tag_id)
-244
-245    @with_parser(amend_files_parser, [files_postparser])
-246    def do_amend(self, args: Namespace):
-247        """Stage files and add to previous commit."""
-248        git.amend(args.files)
-249
-250    @with_parser(delete_branch_parser)
-251    def do_delete_branch(self, args: Namespace):
-252        """Delete branch."""
-253        git.delete_branch(args.branch, not args.remote)
-254
-255    def do_pull_branch(self, branch: str):
-256        """Pull this branch from the origin."""
-257        git.pull_branch(branch)
-258
-259    def do_ignore(self, patterns: str):
-260        """Add the list of patterns to `.gitignore`."""
-261        patterns = "\n".join(patterns.split())
-262        path = Pathier(".gitignore")
-263        path.append("\n")
-264        path.append(patterns, False)
-265
-266    def do_make_private(self, owner: str):
-267        """Make the GitHub remote for this repo private.
-268
-269        Expects an argument for the repo owner, i.e. the `OWNER` in
+161        git.create_remote_from_cwd(args.public)
+162
+163    def do_initcommit(self, _: str):
+164        """Stage and commit all files with message "Initial Commit"."""
+165        git.initcommit()
+166
+167    def do_undo(self, _: str):
+168        """Undo all uncommitted changes."""
+169        git.undo()
+170
+171    @with_parser(amend_files_parser, [files_postparser])
+172    def do_add(self, args: Namespace):
+173        """Stage a list of files.
+174        If no files are given, all files will be added."""
+175        git.add(None if not args.files else args.files)
+176
+177    def do_commit(self, message: str):
+178        """Commit staged files with this message."""
+179        if not message.startswith('"'):
+180            message = '"' + message
+181        if not message.endswith('"'):
+182            message += '"'
+183        git.commit(f"-m {message}")
+184
+185    @with_parser(commit_files_parser, [files_postparser])
+186    def do_commitf(self, args: Namespace):
+187        """Stage and commit a list of files."""
+188        git.commit_files(args.files, args.message)
+189
+190    def do_commitall(self, message: str):
+191        """Stage and commit all files with this message."""
+192        if not message.startswith('"'):
+193            message = '"' + message
+194        if not message.endswith('"'):
+195            message += '"'
+196        git.add()
+197        git.commit(f"-m {message}")
+198
+199    def do_switch(self, branch_name: str):
+200        """Switch to this branch."""
+201        git.switch_branch(branch_name)
+202
+203    def do_add_url(self, url: str):
+204        """Add remote origin url for repo and push repo."""
+205        git.add_remote_url(url)
+206        git.push("-u origin main")
+207
+208    def do_push_new(self, branch_name: str):
+209        """Push this new branch to origin with -u flag."""
+210        git.push_new_branch(branch_name)
+211
+212    def do_push(self, args: str):
+213        """Execute `git push`.
+214
+215        `args` can be any additional args that `git push` accepts."""
+216        git.push(args)
+217
+218    def do_pull(self, args: str):
+219        """Execute `git pull`.
+220
+221        `args` can be any additional args that `git pull` accepts."""
+222        git.pull(args)
+223
+224    def do_branches(self, _: str):
+225        """Show local and remote branches."""
+226        git.list_branches()
+227
+228    def do_loggy(self, _: str):
+229        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
+230        git.loggy()
+231
+232    def do_status(self, _: str):
+233        """Execute `git status`."""
+234        git.status()
+235
+236    def do_merge(self, branch_name: str):
+237        """Merge supplied `branch_name` with the currently active branch."""
+238        git.merge(branch_name)
+239
+240    def do_tag(self, tag_id: str):
+241        """Tag current commit with `tag_id`."""
+242        git.tag(tag_id)
+243
+244    @with_parser(amend_files_parser, [files_postparser])
+245    def do_amend(self, args: Namespace):
+246        """Stage files and add to previous commit."""
+247        git.amend(args.files)
+248
+249    @with_parser(delete_branch_parser)
+250    def do_delete_branch(self, args: Namespace):
+251        """Delete branch."""
+252        git.delete_branch(args.branch, not args.remote)
+253
+254    def do_pull_branch(self, branch: str):
+255        """Pull this branch from the origin."""
+256        git.pull_branch(branch)
+257
+258    def do_ignore(self, patterns: str):
+259        """Add the list of patterns to `.gitignore`."""
+260        patterns = "\n".join(patterns.split())
+261        path = Pathier(".gitignore")
+262        path.append("\n")
+263        path.append(patterns, False)
+264
+265    def do_make_private(self, owner: str):
+266        """Make the GitHub remote for this repo private.
+267
+268        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-270
-271        This repo must exist and GitHub CLI must be installed and
+269
+270        This repo must exist and GitHub CLI must be installed and
 configured."""
-272        git.make_private(owner, Pathier.cwd().stem)
-273
-274    def do_make_public(self, owner: str):
-275        """Make the GitHub remote for this repo public.
-276
-277        Expects an argument for the repo owner, i.e. the `OWNER` in
+271        git.make_private(owner, Pathier.cwd().stem)
+272
+273    def do_make_public(self, owner: str):
+274        """Make the GitHub remote for this repo public.
+275
+276        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-278
-279        This repo must exist and GitHub CLI must be installed and
+277
+278        This repo must exist and GitHub CLI must be installed and
 configured."""
-280        git.make_public(owner, Pathier.cwd().stem)
-281
-282    def do_delete_gh_repo(self, owner: str):
-283        """Delete this repo from GitHub.
-284
-285        Expects an argument for the repo owner, i.e. the `OWNER` in
+279        git.make_public(owner, Pathier.cwd().stem)
+280
+281    def do_delete_gh_repo(self, owner: str):
+282        """Delete this repo from GitHub.
+283
+284        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-286
-287        GitHub CLI must be installed and configured.
-288
-289        May require you to reauthorize and rerun command."""
-290        git.delete_remote(owner, Pathier.cwd().stem)
+285
+286        GitHub CLI must be installed and configured.
+287
+288        May require you to reauthorize and rerun command."""
+289        git.delete_remote(owner, Pathier.cwd().stem)
 GitBetter Shell.
 ⁰
 def default(self, line: str): View Source
 107    def default(self, line: str):
 108        if self.execute_in_terminal_if_unrecognized:
 109            os.system(line)
 110        else:
@@ -750,212 +750,211 @@
 @with_parser(new_remote_parser)
 def do_new_gh_remote(self, args: argshell.argshell.Namespace): View Source
 156    @with_parser(new_remote_parser)
 157    def do_new_gh_remote(self, args: Namespace):
 158        """Create a remote GitHub repository for this repo.
 159
 160        GitHub CLI must be installed and configured for this to work."""
-161        name = Pathier.cwd().stem
-162        git.create_remote(name, args.public)
+161        git.create_remote_from_cwd(args.public)
 Create a remote GitHub repository for this repo.
 GitHub CLI must be installed and configured for this to work.
 ⁰
 def do_initcommit(self, _: str): View Source
-164    def do_initcommit(self, _: str):
-165        """Stage and commit all files with message "Initial Commit"."""
-166        git.initcommit()
+163    def do_initcommit(self, _: str):
+164        """Stage and commit all files with message "Initial Commit"."""
+165        git.initcommit()
 Stage and commit all files with message "Initial Commit".
 ⁰
 def do_undo(self, _: str): View Source
-168    def do_undo(self, _: str):
-169        """Undo all uncommitted changes."""
-170        git.undo()
+167    def do_undo(self, _: str):
+168        """Undo all uncommitted changes."""
+169        git.undo()
 Undo all uncommitted changes.
 ⁰
 @with_parser(amend_files_parser, [files_postparser])
 def do_add(self, args: argshell.argshell.Namespace): View Source
-172    @with_parser(amend_files_parser, [files_postparser])
-173    def do_add(self, args: Namespace):
-174        """Stage a list of files.
-175        If no files are given, all files will be added."""
-176        git.add(None if not args.files else args.files)
+171    @with_parser(amend_files_parser, [files_postparser])
+172    def do_add(self, args: Namespace):
+173        """Stage a list of files.
+174        If no files are given, all files will be added."""
+175        git.add(None if not args.files else args.files)
 Stage a list of files. If no files are given, all files will be added.
 ⁰
 def do_commit(self, message: str): View Source
-178    def do_commit(self, message: str):
-179        """Commit staged files with this message."""
-180        if not message.startswith('"'):
-181            message = '"' + message
-182        if not message.endswith('"'):
-183            message += '"'
-184        git.commit(f"-m {message}")
+177    def do_commit(self, message: str):
+178        """Commit staged files with this message."""
+179        if not message.startswith('"'):
+180            message = '"' + message
+181        if not message.endswith('"'):
+182            message += '"'
+183        git.commit(f"-m {message}")
 Commit staged files with this message.
 ⁰
 @with_parser(commit_files_parser, [files_postparser])
 def do_commitf(self, args: argshell.argshell.Namespace): View Source
-186    @with_parser(commit_files_parser, [files_postparser])
-187    def do_commitf(self, args: Namespace):
-188        """Stage and commit a list of files."""
-189        git.commit_files(args.files, args.message)
+185    @with_parser(commit_files_parser, [files_postparser])
+186    def do_commitf(self, args: Namespace):
+187        """Stage and commit a list of files."""
+188        git.commit_files(args.files, args.message)
 Stage and commit a list of files.
 ⁰
 def do_commitall(self, message: str): View Source
-191    def do_commitall(self, message: str):
-192        """Stage and commit all files with this message."""
-193        if not message.startswith('"'):
-194            message = '"' + message
-195        if not message.endswith('"'):
-196            message += '"'
-197        git.add()
-198        git.commit(f"-m {message}")
+190    def do_commitall(self, message: str):
+191        """Stage and commit all files with this message."""
+192        if not message.startswith('"'):
+193            message = '"' + message
+194        if not message.endswith('"'):
+195            message += '"'
+196        git.add()
+197        git.commit(f"-m {message}")
 Stage and commit all files with this message.
 ⁰
 def do_switch(self, branch_name: str): View Source
-200    def do_switch(self, branch_name: str):
-201        """Switch to this branch."""
-202        git.switch_branch(branch_name)
+199    def do_switch(self, branch_name: str):
+200        """Switch to this branch."""
+201        git.switch_branch(branch_name)
 Switch to this branch.
 ⁰
 def do_add_url(self, url: str): View Source
-204    def do_add_url(self, url: str):
-205        """Add remote url for repo and push repo."""
-206        git.add_remote_url(url)
-207        git.push("-u origin main")
-Add remote url for repo and push repo.
+203    def do_add_url(self, url: str):
+204        """Add remote origin url for repo and push repo."""
+205        git.add_remote_url(url)
+206        git.push("-u origin main")
+Add remote origin url for repo and push repo.
 ⁰
 def do_push_new(self, branch_name: str): View Source
-209    def do_push_new(self, branch_name: str):
-210        """Push this new branch to origin with -u flag."""
-211        git.push_new_branch(branch_name)
+208    def do_push_new(self, branch_name: str):
+209        """Push this new branch to origin with -u flag."""
+210        git.push_new_branch(branch_name)
 Push this new branch to origin with -u flag.
 ⁰
 def do_push(self, args: str): View Source
-213    def do_push(self, args: str):
-214        """Execute `git push`.
-215
-216        `args` can be any additional args that `git push` accepts."""
-217        git.push(args)
+212    def do_push(self, args: str):
+213        """Execute `git push`.
+214
+215        `args` can be any additional args that `git push` accepts."""
+216        git.push(args)
 Execute git push.
 args can be any additional args that git push accepts.
 ⁰
 def do_pull(self, args: str): View Source
-219    def do_pull(self, args: str):
-220        """Execute `git pull`.
-221
-222        `args` can be any additional args that `git pull` accepts."""
-223        git.pull(args)
+218    def do_pull(self, args: str):
+219        """Execute `git pull`.
+220
+221        `args` can be any additional args that `git pull` accepts."""
+222        git.pull(args)
 Execute git pull.
 args can be any additional args that git pull accepts.
 ⁰
-def do_list_branches(self, _: str): View Source
-225    def do_list_branches(self, _: str):
-226        """Show local and remote branches."""
-227        git.list_branches()
+def do_branches(self, _: str): View Source
+224    def do_branches(self, _: str):
+225        """Show local and remote branches."""
+226        git.list_branches()
 Show local and remote branches.
 ⁰
 def do_loggy(self, _: str): View Source
-229    def do_loggy(self, _: str):
-230        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
-231        git.loggy()
+228    def do_loggy(self, _: str):
+229        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
+230        git.loggy()
 Execute git --oneline --name-only --abbrev-commit --graph.
 ⁰
 def do_status(self, _: str): View Source
-233    def do_status(self, _: str):
-234        """Execute `git status`."""
-235        git.status()
+232    def do_status(self, _: str):
+233        """Execute `git status`."""
+234        git.status()
 Execute git status.
 ⁰
 def do_merge(self, branch_name: str): View Source
-237    def do_merge(self, branch_name: str):
-238        """Merge supplied `branch_name` with the currently active branch."""
-239        git.merge(branch_name)
+236    def do_merge(self, branch_name: str):
+237        """Merge supplied `branch_name` with the currently active branch."""
+238        git.merge(branch_name)
 Merge supplied branch_name with the currently active branch.
 ⁰
 def do_tag(self, tag_id: str): View Source
-241    def do_tag(self, tag_id: str):
-242        """Tag current commit with `tag_id`."""
-243        git.tag(tag_id)
+240    def do_tag(self, tag_id: str):
+241        """Tag current commit with `tag_id`."""
+242        git.tag(tag_id)
 Tag current commit with tag_id.
 ⁰
 @with_parser(amend_files_parser, [files_postparser])
 def do_amend(self, args: argshell.argshell.Namespace): View Source
-245    @with_parser(amend_files_parser, [files_postparser])
-246    def do_amend(self, args: Namespace):
-247        """Stage files and add to previous commit."""
-248        git.amend(args.files)
+244    @with_parser(amend_files_parser, [files_postparser])
+245    def do_amend(self, args: Namespace):
+246        """Stage files and add to previous commit."""
+247        git.amend(args.files)
 Stage files and add to previous commit.
 ⁰
 @with_parser(delete_branch_parser)
 def do_delete_branch(self, args: argshell.argshell.Namespace): View Source
-250    @with_parser(delete_branch_parser)
-251    def do_delete_branch(self, args: Namespace):
-252        """Delete branch."""
-253        git.delete_branch(args.branch, not args.remote)
+249    @with_parser(delete_branch_parser)
+250    def do_delete_branch(self, args: Namespace):
+251        """Delete branch."""
+252        git.delete_branch(args.branch, not args.remote)
 Delete branch.
 ⁰
 def do_pull_branch(self, branch: str): View Source
-255    def do_pull_branch(self, branch: str):
-256        """Pull this branch from the origin."""
-257        git.pull_branch(branch)
+254    def do_pull_branch(self, branch: str):
+255        """Pull this branch from the origin."""
+256        git.pull_branch(branch)
 Pull this branch from the origin.
 ⁰
 def do_ignore(self, patterns: str): View Source
-259    def do_ignore(self, patterns: str):
-260        """Add the list of patterns to `.gitignore`."""
-261        patterns = "\n".join(patterns.split())
-262        path = Pathier(".gitignore")
-263        path.append("\n")
-264        path.append(patterns, False)
+258    def do_ignore(self, patterns: str):
+259        """Add the list of patterns to `.gitignore`."""
+260        patterns = "\n".join(patterns.split())
+261        path = Pathier(".gitignore")
+262        path.append("\n")
+263        path.append(patterns, False)
 Add the list of patterns to .gitignore.
 ⁰
 def do_make_private(self, owner: str): View Source
-266    def do_make_private(self, owner: str):
-267        """Make the GitHub remote for this repo private.
-268
-269        Expects an argument for the repo owner, i.e. the `OWNER` in
+265    def do_make_private(self, owner: str):
+266        """Make the GitHub remote for this repo private.
+267
+268        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-270
-271        This repo must exist and GitHub CLI must be installed and
+269
+270        This repo must exist and GitHub CLI must be installed and
 configured."""
-272        git.make_private(owner, Pathier.cwd().stem)
+271        git.make_private(owner, Pathier.cwd().stem)
 Make the GitHub remote for this repo private.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 This repo must exist and GitHub CLI must be installed and configured.
 ⁰
 def do_make_public(self, owner: str): View Source
-274    def do_make_public(self, owner: str):
-275        """Make the GitHub remote for this repo public.
-276
-277        Expects an argument for the repo owner, i.e. the `OWNER` in
+273    def do_make_public(self, owner: str):
+274        """Make the GitHub remote for this repo public.
+275
+276        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-278
-279        This repo must exist and GitHub CLI must be installed and
+277
+278        This repo must exist and GitHub CLI must be installed and
 configured."""
-280        git.make_public(owner, Pathier.cwd().stem)
+279        git.make_public(owner, Pathier.cwd().stem)
 Make the GitHub remote for this repo public.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 This repo must exist and GitHub CLI must be installed and configured.
 ⁰
 def do_delete_gh_repo(self, owner: str): View Source
-282    def do_delete_gh_repo(self, owner: str):
-283        """Delete this repo from GitHub.
-284
-285        Expects an argument for the repo owner, i.e. the `OWNER` in
+281    def do_delete_gh_repo(self, owner: str):
+282        """Delete this repo from GitHub.
+283
+284        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-286
-287        GitHub CLI must be installed and configured.
-288
-289        May require you to reauthorize and rerun command."""
-290        git.delete_remote(owner, Pathier.cwd().stem)
+285
+286        GitHub CLI must be installed and configured.
+287
+288        May require you to reauthorize and rerun command."""
+289        git.delete_remote(owner, Pathier.cwd().stem)
 Delete this repo from GitHub.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 GitHub CLI must be installed and configured.
 May require you to reauthorize and rerun command.
 ** Inherited Members **
   ⁰
 def main(): View Source
-293def main():
-294    GitBetter().cmdloop()
+292def main():
+293    GitBetter().cmdloop()
```

### Comparing `gitbetter-0.4.0/src/gitbetter/git.py` & `gitbetter-0.5.0/src/gitbetter/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,25 @@
     `name`: The name for the repo.
 
     `public`: Set to `True` to create the repo as public, otherwise it'll be created as private."""
     visibility = "--public" if public else "--private"
     os.system(f"gh repo create {name} {visibility}")
 
 
+def create_remote_from_cwd(public: bool = False):
+    """Use GitHub CLI (must be installed and configured) to create a remote GitHub repo from
+    the current working directory repo and add its url as this repo's remote origin.
+
+    #### :params:
+
+    `public`: Create the GitHub repo as a public repo, default is to create it as private."""
+    visibility = "public" if public else "private"
+    os.system(f"gh repo create --source . --{visibility}")
+
+
 def make_private(owner: str, name: str):
     """Uses GitHub CLI (must be installed and configured) to set the repo's visibility to private.
 
     #### :params:
 
     `owner`: The repo owner.
```

### Comparing `gitbetter-0.4.0/src/gitbetter/gitbetter.py` & `gitbetter-0.5.0/src/gitbetter/gitbetter.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                 print(
                     "^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^"
                 )
         print()
 
     @property
     def unrecognized_command_behavior_status(self):
-        return f"Unrecognized command behavior: {'Execute with os.system()' if self.execute_in_terminal_if_unrecognized else 'Print unknown syntax error'}"
+        return f"Unrecognized command behavior: {'Execute in shell with os.system()' if self.execute_in_terminal_if_unrecognized else 'Print unknown syntax error'}"
 
     def do_toggle_unrecognized_command_behavior(self, arg: str):
         """Toggle whether the shell will attempt to execute unrecognized commands as system commands in the terminal.
         When on (the default), `GitBetter` will treat unrecognized commands as if you added the `sys` command in front of the input, i.e. `os.system(your_input)`.
         When off, an `unknown syntax` message will be printed and no commands will be executed."""
         self.execute_in_terminal_if_unrecognized = (
             not self.execute_in_terminal_if_unrecognized
@@ -153,16 +153,15 @@
         git.create_new_branch(name)
 
     @with_parser(new_remote_parser)
     def do_new_gh_remote(self, args: Namespace):
         """Create a remote GitHub repository for this repo.
 
         GitHub CLI must be installed and configured for this to work."""
-        name = Pathier.cwd().stem
-        git.create_remote(name, args.public)
+        git.create_remote_from_cwd(args.public)
 
     def do_initcommit(self, _: str):
         """Stage and commit all files with message "Initial Commit"."""
         git.initcommit()
 
     def do_undo(self, _: str):
         """Undo all uncommitted changes."""
@@ -197,15 +196,15 @@
         git.commit(f"-m {message}")
 
     def do_switch(self, branch_name: str):
         """Switch to this branch."""
         git.switch_branch(branch_name)
 
     def do_add_url(self, url: str):
-        """Add remote url for repo and push repo."""
+        """Add remote origin url for repo and push repo."""
         git.add_remote_url(url)
         git.push("-u origin main")
 
     def do_push_new(self, branch_name: str):
         """Push this new branch to origin with -u flag."""
         git.push_new_branch(branch_name)
 
@@ -217,15 +216,15 @@
 
     def do_pull(self, args: str):
         """Execute `git pull`.
 
         `args` can be any additional args that `git pull` accepts."""
         git.pull(args)
 
-    def do_list_branches(self, _: str):
+    def do_branches(self, _: str):
         """Show local and remote branches."""
         git.list_branches()
 
     def do_loggy(self, _: str):
         """Execute `git --oneline --name-only --abbrev-commit --graph`."""
         git.loggy()
```

### Comparing `gitbetter-0.4.0/LICENSE.txt` & `gitbetter-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitbetter-0.4.0/README.md` & `gitbetter-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,26 +25,27 @@
 C:\gitbetter>gitbetter
 Starting gitbetter...
 Enter 'help' or '?' for command help.
 gitbetter::C:\gitbetter>help
 
 Documented commands (type help <topic>):
 ========================================
-add             help           new_repo                              undo
-add_url         ignore         pull
-amend           initcommit     pull_branch
-cd              list_branches  push
-commit          loggy          push_new
-commitall       make_private   quit
-commitf         make_public    switch
-delete_branch   merge          sys
-delete_gh_repo  new_branch     tag
-git             new_gh_remote  toggle_unrecognized_command_behavior
+add             ignore         pull_branch
+add_url         initcommit     push
+amend           list_branches  push_new
+cd              loggy          quit
+commit          make_private   status
+commitall       make_public    switch
+commitf         merge          sys
+delete_branch   new_branch     tag
+delete_gh_repo  new_gh_remote  toggle_unrecognized_command_behavior
+git             new_repo       undo
+help            pull
 
-Unrecognized command behavior: Execute with os.system()
+Unrecognized command behavior: Execute in shell with os.system()
 ^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^
 
 gitbetter::C:\gitbetter>help commitf
 Stage and commit a list of files.
 Parser help for commitf:
 usage: gitbetter [-h] -m MESSAGE [-r] [files ...]
 
@@ -114,9 +115,8 @@
   test.txt
 >>> git.list_branches()
 * main                3e780ec [origin/main: ahead 3] Merge branch 'my-feature'
   remotes/origin/main fc6b7ac docs: update readme
 </pre>
 
 ### Future Features
-* Redirect the output of git commands so the bindings return the output instead of only being able to print.
-* Make pushing to remote after creating it smoother (make it so you don't manually have to add the url).
+* Redirect the output of git commands so the bindings return the output instead of only being able to print.
```

### Comparing `gitbetter-0.4.0/pyproject.toml` & `gitbetter-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6769 7462 6574 7465 7222 0d0a 6465   "gitbetter"..de
 00000070: 7363 7269 7074 696f 6e20 3d20 2243 7573  scription = "Cus
 00000080: 746f 6d20 6769 7420 7368 656c 6c20 746f  tom git shell to
 00000090: 2074 7970 6520 6c65 7373 2061 6e64 2063   type less and c
 000000a0: 6f6d 6d69 7420 6d6f 7265 2e22 0d0a 7665  ommit more."..ve
-000000b0: 7273 696f 6e20 3d20 2230 2e34 2e30 220d  rsion = "0.4.0".
+000000b0: 7273 696f 6e20 3d20 2230 2e35 2e30 220d  rsion = "0.5.0".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6172  endencies = ["ar
 000000f0: 6773 6865 6c6c 222c 2022 7061 7468 6965  gshell", "pathie
 00000100: 7222 2c20 2270 7974 6573 7422 5d0d 0a72  r", "pytest"]..r
 00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
 00000120: 6d64 220d 0a6b 6579 776f 7264 7320 3d20  md"..keywords =
```

### Comparing `gitbetter-0.4.0/PKG-INFO` & `gitbetter-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitbetter
-Version: 0.4.0
+Version: 0.5.0
 Summary: Custom git shell to type less and commit more.
 Project-URL: Homepage, https://github.com/matt-manes/gitbetter
 Project-URL: Documentation, https://github.com/matt-manes/gitbetter/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gitbetter/tree/main/src/gitbetter
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,commit,git,shell,terminal
@@ -44,26 +44,27 @@
 C:\gitbetter>gitbetter
 Starting gitbetter...
 Enter 'help' or '?' for command help.
 gitbetter::C:\gitbetter>help
 
 Documented commands (type help <topic>):
 ========================================
-add             help           new_repo                              undo
-add_url         ignore         pull
-amend           initcommit     pull_branch
-cd              list_branches  push
-commit          loggy          push_new
-commitall       make_private   quit
-commitf         make_public    switch
-delete_branch   merge          sys
-delete_gh_repo  new_branch     tag
-git             new_gh_remote  toggle_unrecognized_command_behavior
+add             ignore         pull_branch
+add_url         initcommit     push
+amend           list_branches  push_new
+cd              loggy          quit
+commit          make_private   status
+commitall       make_public    switch
+commitf         merge          sys
+delete_branch   new_branch     tag
+delete_gh_repo  new_gh_remote  toggle_unrecognized_command_behavior
+git             new_repo       undo
+help            pull
 
-Unrecognized command behavior: Execute with os.system()
+Unrecognized command behavior: Execute in shell with os.system()
 ^Essentially makes this shell function as a super-shell of whatever shell you launched gitbetter from.^
 
 gitbetter::C:\gitbetter>help commitf
 Stage and commit a list of files.
 Parser help for commitf:
 usage: gitbetter [-h] -m MESSAGE [-r] [files ...]
 
@@ -133,9 +134,8 @@
   test.txt
 >>> git.list_branches()
 * main                3e780ec [origin/main: ahead 3] Merge branch 'my-feature'
   remotes/origin/main fc6b7ac docs: update readme
 </pre>
 
 ### Future Features
-* Redirect the output of git commands so the bindings return the output instead of only being able to print.
-* Make pushing to remote after creating it smoother (make it so you don't manually have to add the url).
+* Redirect the output of git commands so the bindings return the output instead of only being able to print.
```

