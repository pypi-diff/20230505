# Comparing `tmp/gitbetter-0.3.0.tar.gz` & `tmp/gitbetter-0.4.0.tar.gz`

## Comparing `gitbetter-0.3.0.tar` & `gitbetter-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 gitbetter-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0    34124 2020-02-02 00:00:00.000000 gitbetter-0.3.0/docs/gitbetter.html
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-0.3.0/docs/index.html
--rw-r--r--   0        0        0    56411 2020-02-02 00:00:00.000000 gitbetter-0.3.0/docs/search.js
--rw-r--r--   0        0        0   130318 2020-02-02 00:00:00.000000 gitbetter-0.3.0/docs/gitbetter/git.html
--rw-r--r--   0        0        0   246570 2020-02-02 00:00:00.000000 gitbetter-0.3.0/docs/gitbetter/gitbetter.html
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gitbetter-0.3.0/src/gitbetter/__init__.py
--rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 gitbetter-0.3.0/src/gitbetter/git.py
--rw-r--r--   0        0        0    10135 2020-02-02 00:00:00.000000 gitbetter-0.3.0/src/gitbetter/gitbetter.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-0.3.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 gitbetter-0.3.0/README.md
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 gitbetter-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 gitbetter-0.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34124 2020-02-02 00:00:00.000000 gitbetter-0.4.0/docs/gitbetter.html
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 gitbetter-0.4.0/docs/index.html
+-rw-r--r--   0        0        0    57211 2020-02-02 00:00:00.000000 gitbetter-0.4.0/docs/search.js
+-rw-r--r--   0        0        0   132406 2020-02-02 00:00:00.000000 gitbetter-0.4.0/docs/gitbetter/git.html
+-rw-r--r--   0        0        0   250092 2020-02-02 00:00:00.000000 gitbetter-0.4.0/docs/gitbetter/gitbetter.html
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 gitbetter-0.4.0/src/gitbetter/__init__.py
+-rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 gitbetter-0.4.0/src/gitbetter/git.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 gitbetter-0.4.0/src/gitbetter/gitbetter.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 gitbetter-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gitbetter-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     4284 2020-02-02 00:00:00.000000 gitbetter-0.4.0/README.md
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 gitbetter-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4897 2020-02-02 00:00:00.000000 gitbetter-0.4.0/PKG-INFO
```

### Comparing `gitbetter-0.3.0/CHANGELOG.md` & `gitbetter-0.4.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 # Changelog
 
-## 0.2.0 (2023-05-02)
+## 0.3.0 (2023-05-02)
+
+#### Refactorings
+
+* remove do_cmd as it's now covered by parent class's do_sys
+
+
+## v0.2.0 (2023-05-02)
 
 #### New Features
 
 * override do_help to display unrecognized_command_behavior_status after standard help message
 * add functionality to toggle unrecognized command behavior
-* add default() override to execute line as system command when unrecognized
+* add default override to execute line as system command when unrecognized
 * display current working directory in prompt
 #### Fixes
 
 * set requires-python to >=3.10
 #### Refactorings
 
 * remove cwd command
 #### Docs
 
 * update readme
+#### Others
+
+* build v0.2.0
+* update changelog
 
 
 ## v0.1.1 (2023-04-30)
 
 #### Fixes
 
 * cast Pathier objects to strings in recurse_files()
```

### Comparing `gitbetter-0.3.0/docs/gitbetter.html` & `gitbetter-0.4.0/docs/gitbetter.html`

 * *Files identical despite different names*

### Comparing `gitbetter-0.3.0/docs/search.js` & `gitbetter-0.4.0/docs/search.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -713,14 +713,22 @@
         "modulename": "gitbetter.git",
         "qualname": "loggy",
         "kind": "function",
         "doc": "<p>Equivalent to <code>git log --oneline --name-only --abbrev-commit --graph</code>.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
+        "fullname": "gitbetter.git.status",
+        "modulename": "gitbetter.git",
+        "qualname": "status",
+        "kind": "function",
+        "doc": "<p>Execute <code>git status</code>.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
         "fullname": "gitbetter.git.commit",
         "modulename": "gitbetter.git",
         "qualname": "commit",
         "kind": "function",
         "doc": "<div class=\"pdoc-code codehilite\">\n<pre><span></span><code><span class=\"gp\">&gt;&gt;&gt; </span><span class=\"n\">git</span> <span class=\"n\">commit</span> <span class=\"p\">{</span><span class=\"n\">args</span><span class=\"p\">}</span>\n</code></pre>\n</div>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
@@ -1125,14 +1133,22 @@
         "modulename": "gitbetter.gitbetter",
         "qualname": "GitBetter.do_loggy",
         "kind": "function",
         "doc": "<p>Execute <code>git --oneline --name-only --abbrev-commit --graph</code>.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">_</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }, {
+        "fullname": "gitbetter.gitbetter.GitBetter.do_status",
+        "modulename": "gitbetter.gitbetter",
+        "qualname": "GitBetter.do_status",
+        "kind": "function",
+        "doc": "<p>Execute <code>git status</code>.</p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">_</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
+        "funcdef": "def"
+    }, {
         "fullname": "gitbetter.gitbetter.GitBetter.do_merge",
         "modulename": "gitbetter.gitbetter",
         "qualname": "GitBetter.do_merge",
         "kind": "function",
         "doc": "<p>Merge supplied <code>branch_name</code> with the currently active branch.</p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"bp\">self</span>, </span><span class=\"param\"><span class=\"n\">branch_name</span><span class=\"p\">:</span> <span class=\"nb\">str</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
```

### Comparing `gitbetter-0.3.0/docs/gitbetter/git.html` & `gitbetter-0.4.0/docs/gitbetter/git.html`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,17 @@
             <li>
                     <a class="function" href="#new_repo">new_repo</a>
             </li>
             <li>
                     <a class="function" href="#loggy">loggy</a>
             </li>
             <li>
+                    <a class="function" href="#status">status</a>
+            </li>
+            <li>
                     <a class="function" href="#commit">commit</a>
             </li>
             <li>
                     <a class="function" href="#add">add</a>
             </li>
             <li>
                     <a class="function" href="#commit_files">commit_files</a>
@@ -147,191 +150,196 @@
 </span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>
 </span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>
 </span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a><span class="k">def</span> <span class="nf">loggy</span><span class="p">():</span>
 </span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git log --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
 </span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;log --oneline --name-only --abbrev-commit --graph&quot;</span><span class="p">)</span>
 </span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>
 </span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="c1"># ======================================Staging/Committing======================================</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a><span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a><span class="k">def</span> <span class="nf">status</span><span class="p">():</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>    <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;status&quot;</span><span class="p">)</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
 </span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a><span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a><span class="sd">    If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>        <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>        <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;add </span><span class="si">{</span><span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">files</span><span class="p">)</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a><span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="c1"># ======================================Staging/Committing======================================</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a><span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a><span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>    <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a><span class="sd">    If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;add </span><span class="si">{</span><span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">files</span><span class="p">)</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>
 </span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a><span class="k">def</span> <span class="nf">initcommit</span><span class="p">():</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a><span class="sd">    &gt;&gt;&gt; git add .</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a><span class="sd">    &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>    <span class="n">add</span><span class="p">()</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a><span class="sd">    If `files` is `None`, all files will be staged.</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a><span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a><span class="k">def</span> <span class="nf">initcommit</span><span class="p">():</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="sd">    &gt;&gt;&gt; git add .</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a><span class="sd">    &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>    <span class="n">add</span><span class="p">()</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>
 </span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="sd">    Equivalent to:</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a><span class="sd">    &gt;&gt;&gt; git add {files}</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a><span class="sd">    &gt;&gt;&gt; git commit --amend --no-edit</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="n">id_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="sd">&quot;&quot;&quot;Tag the current commit with `id_`.</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a><span class="sd">    Equivalent to `git tag {id_}`.&quot;&quot;&quot;</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">id_</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a><span class="c1"># ==========================================Push/Pull==========================================</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">):</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a><span class="sd">    If `files` is `None`, all files will be staged.</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a><span class="sd">    Equivalent to:</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a><span class="sd">    &gt;&gt;&gt; git add {files}</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="sd">    &gt;&gt;&gt; git commit --amend --no-edit</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a><span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="n">id_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>    <span class="sd">&quot;&quot;&quot;Tag the current commit with `id_`.</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a><span class="sd">    Equivalent to `git tag {id_}`.&quot;&quot;&quot;</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">id_</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>
 </span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a><span class="c1"># ==========================================Push/Pull==========================================</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">):</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>
 </span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a><span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
 </span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a><span class="sd">    Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>    <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a><span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a><span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="sd">    Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
 </span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a><span class="c1"># ============================================Checkout/Branches============================================</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a><span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a><span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>
 </span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="k">def</span> <span class="nf">list_branches</span><span class="p">():</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>    <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a><span class="c1"># ============================================Checkout/Branches============================================</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a><span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>
 </span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
-</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a><span class="k">def</span> <span class="nf">list_branches</span><span class="p">():</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
+</span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>    <span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
 </span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>
 </span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a><span class="sd">    Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
-</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a><span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>    <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a><span class="sd">    Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a><span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a><span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>
+</span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a><span class="sd">    Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a><span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a><span class="sd">    Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>
 </span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a><span class="sd">    `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>    <span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>        <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a><span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>    <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a><span class="sd">    #### :params:</span>
 </span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a><span class="k">def</span> <span class="nf">undo</span><span class="p">():</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a><span class="sd">    Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a><span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>    <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a><span class="sd">    `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>    <span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>        <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a><span class="k">def</span> <span class="nf">undo</span><span class="p">():</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>    <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="sd">    Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
 </span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>
 </span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="c1"># ===============================Requires GitHub CLI to be installed and configured===============================</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a><span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
-</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>
-</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a><span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a><span class="c1"># ===============================Requires GitHub CLI to be installed and configured===============================</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>
 </span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>
-</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="sd">    `name`: The name for the repo.</span>
-</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>
-</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a><span class="sd">    `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
-</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
-</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a><span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a><span class="sd">    `name`: The name for the repo.</span>
 </span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>
-</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a><span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
-</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>
-</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a><span class="sd">    `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>
 </span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
-</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="sd">    `owner`: The repo owner.</span>
-</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>
-</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility private&quot;</span><span class="p">)</span>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a><span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>
+</span><span id="L-177"><a href="#L-177"><span class="linenos">177</span></a><span class="sd">    #### :params:</span>
 </span><span id="L-178"><a href="#L-178"><span class="linenos">178</span></a>
-</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a>
-</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a><span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
-</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>
-</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-179"><a href="#L-179"><span class="linenos">179</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="L-180"><a href="#L-180"><span class="linenos">180</span></a>
+</span><span id="L-181"><a href="#L-181"><span class="linenos">181</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="L-182"><a href="#L-182"><span class="linenos">182</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility private&quot;</span><span class="p">)</span>
+</span><span id="L-183"><a href="#L-183"><span class="linenos">183</span></a>
 </span><span id="L-184"><a href="#L-184"><span class="linenos">184</span></a>
-</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="sd">    `owner`: The repo owner.</span>
-</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>
-</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility public&quot;</span><span class="p">)</span>
+</span><span id="L-185"><a href="#L-185"><span class="linenos">185</span></a><span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-186"><a href="#L-186"><span class="linenos">186</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
+</span><span id="L-187"><a href="#L-187"><span class="linenos">187</span></a>
+</span><span id="L-188"><a href="#L-188"><span class="linenos">188</span></a><span class="sd">    #### :params:</span>
 </span><span id="L-189"><a href="#L-189"><span class="linenos">189</span></a>
-</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a>
-</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a><span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
-</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>
-</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-190"><a href="#L-190"><span class="linenos">190</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="L-191"><a href="#L-191"><span class="linenos">191</span></a>
+</span><span id="L-192"><a href="#L-192"><span class="linenos">192</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="L-193"><a href="#L-193"><span class="linenos">193</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility public&quot;</span><span class="p">)</span>
+</span><span id="L-194"><a href="#L-194"><span class="linenos">194</span></a>
 </span><span id="L-195"><a href="#L-195"><span class="linenos">195</span></a>
-</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="sd">    `owner`: The repo owner.</span>
-</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>
-</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a><span class="sd">    `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
-</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo delete </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --yes&quot;</span><span class="p">)</span>
+</span><span id="L-196"><a href="#L-196"><span class="linenos">196</span></a><span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-197"><a href="#L-197"><span class="linenos">197</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
+</span><span id="L-198"><a href="#L-198"><span class="linenos">198</span></a>
+</span><span id="L-199"><a href="#L-199"><span class="linenos">199</span></a><span class="sd">    #### :params:</span>
+</span><span id="L-200"><a href="#L-200"><span class="linenos">200</span></a>
+</span><span id="L-201"><a href="#L-201"><span class="linenos">201</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="L-202"><a href="#L-202"><span class="linenos">202</span></a>
+</span><span id="L-203"><a href="#L-203"><span class="linenos">203</span></a><span class="sd">    `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
+</span><span id="L-204"><a href="#L-204"><span class="linenos">204</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo delete </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --yes&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             </section>
                 <section id="execute">
                             <input id="execute-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -405,28 +413,50 @@
 
 
             <div class="docstring"><p>Equivalent to <code>git log --oneline --name-only --abbrev-commit --graph</code>.</p>
 </div>
 
 
                 </section>
+                <section id="status">
+                            <input id="status-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">status</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="status-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#status"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="status-24"><a href="#status-24"><span class="linenos">24</span></a><span class="k">def</span> <span class="nf">status</span><span class="p">():</span>
+</span><span id="status-25"><a href="#status-25"><span class="linenos">25</span></a>    <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="status-26"><a href="#status-26"><span class="linenos">26</span></a>    <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;status&quot;</span><span class="p">)</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Execute <code>git status</code>.</p>
+</div>
+
+
+                </section>
                 <section id="commit">
                             <input id="commit-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">commit</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="commit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#commit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="commit-25"><a href="#commit-25"><span class="linenos">25</span></a><span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="commit-26"><a href="#commit-26"><span class="linenos">26</span></a>    <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
-</span><span id="commit-27"><a href="#commit-27"><span class="linenos">27</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="commit-30"><a href="#commit-30"><span class="linenos">30</span></a><span class="k">def</span> <span class="nf">commit</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="commit-31"><a href="#commit-31"><span class="linenos">31</span></a>    <span class="sd">&quot;&quot;&quot;&gt;&gt;&gt; git commit {args}&quot;&quot;&quot;</span>
+</span><span id="commit-32"><a href="#commit-32"><span class="linenos">32</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;commit </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">git</span> <span class="n">commit</span> <span class="p">{</span><span class="n">args</span><span class="p">}</span>
 </code></pre>
 </div>
@@ -441,22 +471,22 @@
         <span class="def">def</span>
         <span class="name">add</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="add-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#add"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="add-30"><a href="#add-30"><span class="linenos">30</span></a><span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="add-31"><a href="#add-31"><span class="linenos">31</span></a>    <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
-</span><span id="add-32"><a href="#add-32"><span class="linenos">32</span></a>
-</span><span id="add-33"><a href="#add-33"><span class="linenos">33</span></a><span class="sd">    If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
-</span><span id="add-34"><a href="#add-34"><span class="linenos">34</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="add-35"><a href="#add-35"><span class="linenos">35</span></a>        <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
-</span><span id="add-36"><a href="#add-36"><span class="linenos">36</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="add-37"><a href="#add-37"><span class="linenos">37</span></a>        <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;add </span><span class="si">{</span><span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">files</span><span class="p">)</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="add-35"><a href="#add-35"><span class="linenos">35</span></a><span class="k">def</span> <span class="nf">add</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="add-36"><a href="#add-36"><span class="linenos">36</span></a>    <span class="sd">&quot;&quot;&quot;Stage a list of files.</span>
+</span><span id="add-37"><a href="#add-37"><span class="linenos">37</span></a>
+</span><span id="add-38"><a href="#add-38"><span class="linenos">38</span></a><span class="sd">    If no files are given (`files=None`), all files will be staged.&quot;&quot;&quot;</span>
+</span><span id="add-39"><a href="#add-39"><span class="linenos">39</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="add-40"><a href="#add-40"><span class="linenos">40</span></a>        <span class="n">execute</span><span class="p">(</span><span class="s2">&quot;add .&quot;</span><span class="p">)</span>
+</span><span id="add-41"><a href="#add-41"><span class="linenos">41</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="add-42"><a href="#add-42"><span class="linenos">42</span></a>        <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;add </span><span class="si">{</span><span class="s2">&quot; &quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">files</span><span class="p">)</span><span class="si">}</span><span class="s1">&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage a list of files.</p>
 
 <p>If no files are given (<code>files=None</code>), all files will be staged.</p>
 </div>
@@ -470,18 +500,18 @@
         <span class="def">def</span>
         <span class="name">commit_files</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>, </span><span class="param"><span class="n">message</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="commit_files-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#commit_files"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="commit_files-40"><a href="#commit_files-40"><span class="linenos">40</span></a><span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="commit_files-41"><a href="#commit_files-41"><span class="linenos">41</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
-</span><span id="commit_files-42"><a href="#commit_files-42"><span class="linenos">42</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
-</span><span id="commit_files-43"><a href="#commit_files-43"><span class="linenos">43</span></a>    <span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="commit_files-45"><a href="#commit_files-45"><span class="linenos">45</span></a><span class="k">def</span> <span class="nf">commit_files</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">],</span> <span class="n">message</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="commit_files-46"><a href="#commit_files-46"><span class="linenos">46</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit a list of files with commit message `message`.&quot;&quot;&quot;</span>
+</span><span id="commit_files-47"><a href="#commit_files-47"><span class="linenos">47</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
+</span><span id="commit_files-48"><a href="#commit_files-48"><span class="linenos">48</span></a>    <span class="n">commit</span><span class="p">(</span><span class="sa">f</span><span class="s1">&#39;-m &quot;</span><span class="si">{</span><span class="n">message</span><span class="si">}</span><span class="s1">&quot;&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit a list of files with commit message <code>message</code>.</p>
 </div>
 
 
@@ -493,20 +523,20 @@
         <span class="def">def</span>
         <span class="name">initcommit</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="initcommit-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#initcommit"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="initcommit-46"><a href="#initcommit-46"><span class="linenos">46</span></a><span class="k">def</span> <span class="nf">initcommit</span><span class="p">():</span>
-</span><span id="initcommit-47"><a href="#initcommit-47"><span class="linenos">47</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to</span>
-</span><span id="initcommit-48"><a href="#initcommit-48"><span class="linenos">48</span></a><span class="sd">    &gt;&gt;&gt; git add .</span>
-</span><span id="initcommit-49"><a href="#initcommit-49"><span class="linenos">49</span></a><span class="sd">    &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
-</span><span id="initcommit-50"><a href="#initcommit-50"><span class="linenos">50</span></a>    <span class="n">add</span><span class="p">()</span>
-</span><span id="initcommit-51"><a href="#initcommit-51"><span class="linenos">51</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="initcommit-51"><a href="#initcommit-51"><span class="linenos">51</span></a><span class="k">def</span> <span class="nf">initcommit</span><span class="p">():</span>
+</span><span id="initcommit-52"><a href="#initcommit-52"><span class="linenos">52</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to</span>
+</span><span id="initcommit-53"><a href="#initcommit-53"><span class="linenos">53</span></a><span class="sd">    &gt;&gt;&gt; git add .</span>
+</span><span id="initcommit-54"><a href="#initcommit-54"><span class="linenos">54</span></a><span class="sd">    &gt;&gt;&gt; git commit -m &quot;Initial commit&quot; &quot;&quot;&quot;</span>
+</span><span id="initcommit-55"><a href="#initcommit-55"><span class="linenos">55</span></a>    <span class="n">add</span><span class="p">()</span>
+</span><span id="initcommit-56"><a href="#initcommit-56"><span class="linenos">56</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s1">&#39;-m &quot;Initial commit&quot;&#39;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to</p>
 
 <div class="pdoc-code codehilite">
 <pre><span></span><code><span class="gp">&gt;&gt;&gt; </span><span class="n">git</span> <span class="n">add</span> <span class="o">.</span>
@@ -524,25 +554,25 @@
         <span class="def">def</span>
         <span class="name">amend</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="amend-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#amend"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="amend-54"><a href="#amend-54"><span class="linenos">54</span></a><span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="amend-55"><a href="#amend-55"><span class="linenos">55</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
-</span><span id="amend-56"><a href="#amend-56"><span class="linenos">56</span></a>
-</span><span id="amend-57"><a href="#amend-57"><span class="linenos">57</span></a><span class="sd">    If `files` is `None`, all files will be staged.</span>
-</span><span id="amend-58"><a href="#amend-58"><span class="linenos">58</span></a>
-</span><span id="amend-59"><a href="#amend-59"><span class="linenos">59</span></a><span class="sd">    Equivalent to:</span>
-</span><span id="amend-60"><a href="#amend-60"><span class="linenos">60</span></a><span class="sd">    &gt;&gt;&gt; git add {files}</span>
-</span><span id="amend-61"><a href="#amend-61"><span class="linenos">61</span></a><span class="sd">    &gt;&gt;&gt; git commit --amend --no-edit</span>
-</span><span id="amend-62"><a href="#amend-62"><span class="linenos">62</span></a><span class="sd">    &quot;&quot;&quot;</span>
-</span><span id="amend-63"><a href="#amend-63"><span class="linenos">63</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
-</span><span id="amend-64"><a href="#amend-64"><span class="linenos">64</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="amend-59"><a href="#amend-59"><span class="linenos">59</span></a><span class="k">def</span> <span class="nf">amend</span><span class="p">(</span><span class="n">files</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="amend-60"><a href="#amend-60"><span class="linenos">60</span></a>    <span class="sd">&quot;&quot;&quot;Stage and commit changes to the previous commit.</span>
+</span><span id="amend-61"><a href="#amend-61"><span class="linenos">61</span></a>
+</span><span id="amend-62"><a href="#amend-62"><span class="linenos">62</span></a><span class="sd">    If `files` is `None`, all files will be staged.</span>
+</span><span id="amend-63"><a href="#amend-63"><span class="linenos">63</span></a>
+</span><span id="amend-64"><a href="#amend-64"><span class="linenos">64</span></a><span class="sd">    Equivalent to:</span>
+</span><span id="amend-65"><a href="#amend-65"><span class="linenos">65</span></a><span class="sd">    &gt;&gt;&gt; git add {files}</span>
+</span><span id="amend-66"><a href="#amend-66"><span class="linenos">66</span></a><span class="sd">    &gt;&gt;&gt; git commit --amend --no-edit</span>
+</span><span id="amend-67"><a href="#amend-67"><span class="linenos">67</span></a><span class="sd">    &quot;&quot;&quot;</span>
+</span><span id="amend-68"><a href="#amend-68"><span class="linenos">68</span></a>    <span class="n">add</span><span class="p">(</span><span class="n">files</span><span class="p">)</span>
+</span><span id="amend-69"><a href="#amend-69"><span class="linenos">69</span></a>    <span class="n">commit</span><span class="p">(</span><span class="s2">&quot;--amend --no-edit&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage and commit changes to the previous commit.</p>
 
 <p>If <code>files</code> is <code>None</code>, all files will be staged.</p>
 
@@ -564,19 +594,19 @@
         <span class="def">def</span>
         <span class="name">tag</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">id_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="tag-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#tag"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="tag-67"><a href="#tag-67"><span class="linenos">67</span></a><span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="n">id_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="tag-68"><a href="#tag-68"><span class="linenos">68</span></a>    <span class="sd">&quot;&quot;&quot;Tag the current commit with `id_`.</span>
-</span><span id="tag-69"><a href="#tag-69"><span class="linenos">69</span></a>
-</span><span id="tag-70"><a href="#tag-70"><span class="linenos">70</span></a><span class="sd">    Equivalent to `git tag {id_}`.&quot;&quot;&quot;</span>
-</span><span id="tag-71"><a href="#tag-71"><span class="linenos">71</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">id_</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="tag-72"><a href="#tag-72"><span class="linenos">72</span></a><span class="k">def</span> <span class="nf">tag</span><span class="p">(</span><span class="n">id_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="tag-73"><a href="#tag-73"><span class="linenos">73</span></a>    <span class="sd">&quot;&quot;&quot;Tag the current commit with `id_`.</span>
+</span><span id="tag-74"><a href="#tag-74"><span class="linenos">74</span></a>
+</span><span id="tag-75"><a href="#tag-75"><span class="linenos">75</span></a><span class="sd">    Equivalent to `git tag {id_}`.&quot;&quot;&quot;</span>
+</span><span id="tag-76"><a href="#tag-76"><span class="linenos">76</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;tag </span><span class="si">{</span><span class="n">id_</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Tag the current commit with <code>id_</code>.</p>
 
 <p>Equivalent to <code>git tag {id_}</code>.</p>
 </div>
@@ -590,17 +620,17 @@
         <span class="def">def</span>
         <span class="name">add_remote_url</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">url</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;origin&#39;</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="add_remote_url-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#add_remote_url"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="add_remote_url-75"><a href="#add_remote_url-75"><span class="linenos">75</span></a><span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">):</span>
-</span><span id="add_remote_url-76"><a href="#add_remote_url-76"><span class="linenos">76</span></a>    <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
-</span><span id="add_remote_url-77"><a href="#add_remote_url-77"><span class="linenos">77</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="add_remote_url-80"><a href="#add_remote_url-80"><span class="linenos">80</span></a><span class="k">def</span> <span class="nf">add_remote_url</span><span class="p">(</span><span class="n">url</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;origin&quot;</span><span class="p">):</span>
+</span><span id="add_remote_url-81"><a href="#add_remote_url-81"><span class="linenos">81</span></a>    <span class="sd">&quot;&quot;&quot;Add remote url to repo.&quot;&quot;&quot;</span>
+</span><span id="add_remote_url-82"><a href="#add_remote_url-82"><span class="linenos">82</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;remote add </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">url</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add remote url to repo.</p>
 </div>
 
 
@@ -612,17 +642,17 @@
         <span class="def">def</span>
         <span class="name">push</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="push-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#push"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="push-80"><a href="#push-80"><span class="linenos">80</span></a><span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
-</span><span id="push-81"><a href="#push-81"><span class="linenos">81</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
-</span><span id="push-82"><a href="#push-82"><span class="linenos">82</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="push-85"><a href="#push-85"><span class="linenos">85</span></a><span class="k">def</span> <span class="nf">push</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
+</span><span id="push-86"><a href="#push-86"><span class="linenos">86</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git push {args}`.&quot;&quot;&quot;</span>
+</span><span id="push-87"><a href="#push-87"><span class="linenos">87</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;push </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git push {args}</code>.</p>
 </div>
 
 
@@ -634,17 +664,17 @@
         <span class="def">def</span>
         <span class="name">pull</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s1">&#39;&#39;</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="pull-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#pull"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="pull-85"><a href="#pull-85"><span class="linenos">85</span></a><span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
-</span><span id="pull-86"><a href="#pull-86"><span class="linenos">86</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
-</span><span id="pull-87"><a href="#pull-87"><span class="linenos">87</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="pull-90"><a href="#pull-90"><span class="linenos">90</span></a><span class="k">def</span> <span class="nf">pull</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span> <span class="o">=</span> <span class="s2">&quot;&quot;</span><span class="p">):</span>
+</span><span id="pull-91"><a href="#pull-91"><span class="linenos">91</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git pull {args}`.&quot;&quot;&quot;</span>
+</span><span id="pull-92"><a href="#pull-92"><span class="linenos">92</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;pull </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git pull {args}</code>.</p>
 </div>
 
 
@@ -656,19 +686,19 @@
         <span class="def">def</span>
         <span class="name">push_new_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="push_new_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#push_new_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="push_new_branch-90"><a href="#push_new_branch-90"><span class="linenos">90</span></a><span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="push_new_branch-91"><a href="#push_new_branch-91"><span class="linenos">91</span></a>    <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
-</span><span id="push_new_branch-92"><a href="#push_new_branch-92"><span class="linenos">92</span></a>
-</span><span id="push_new_branch-93"><a href="#push_new_branch-93"><span class="linenos">93</span></a><span class="sd">    Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
-</span><span id="push_new_branch-94"><a href="#push_new_branch-94"><span class="linenos">94</span></a>    <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="push_new_branch-95"><a href="#push_new_branch-95"><span class="linenos">95</span></a><span class="k">def</span> <span class="nf">push_new_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="push_new_branch-96"><a href="#push_new_branch-96"><span class="linenos">96</span></a>    <span class="sd">&quot;&quot;&quot;Push a new branch to origin with tracking.</span>
+</span><span id="push_new_branch-97"><a href="#push_new_branch-97"><span class="linenos">97</span></a>
+</span><span id="push_new_branch-98"><a href="#push_new_branch-98"><span class="linenos">98</span></a><span class="sd">    Equivalent to `git push -u origin {branch}`.&quot;&quot;&quot;</span>
+</span><span id="push_new_branch-99"><a href="#push_new_branch-99"><span class="linenos">99</span></a>    <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-u origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Push a new branch to origin with tracking.</p>
 
 <p>Equivalent to <code>git push -u origin {branch}</code>.</p>
 </div>
@@ -682,17 +712,17 @@
         <span class="def">def</span>
         <span class="name">pull_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="pull_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#pull_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="pull_branch-97"><a href="#pull_branch-97"><span class="linenos">97</span></a><span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="pull_branch-98"><a href="#pull_branch-98"><span class="linenos">98</span></a>    <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
-</span><span id="pull_branch-99"><a href="#pull_branch-99"><span class="linenos">99</span></a>    <span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="pull_branch-102"><a href="#pull_branch-102"><span class="linenos">102</span></a><span class="k">def</span> <span class="nf">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="pull_branch-103"><a href="#pull_branch-103"><span class="linenos">103</span></a>    <span class="sd">&quot;&quot;&quot;Pull `branch` from origin.&quot;&quot;&quot;</span>
+</span><span id="pull_branch-104"><a href="#pull_branch-104"><span class="linenos">104</span></a>    <span class="n">pull</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin </span><span class="si">{</span><span class="n">branch</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Pull <code><a href="#branch">branch</a></code> from origin.</p>
 </div>
 
 
@@ -704,17 +734,17 @@
         <span class="def">def</span>
         <span class="name">branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="branch-103"><a href="#branch-103"><span class="linenos">103</span></a><span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="branch-104"><a href="#branch-104"><span class="linenos">104</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
-</span><span id="branch-105"><a href="#branch-105"><span class="linenos">105</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="branch-108"><a href="#branch-108"><span class="linenos">108</span></a><span class="k">def</span> <span class="nf">branch</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="branch-109"><a href="#branch-109"><span class="linenos">109</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git branch {args}`.&quot;&quot;&quot;</span>
+</span><span id="branch-110"><a href="#branch-110"><span class="linenos">110</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;branch </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git branch {args}</code>.</p>
 </div>
 
 
@@ -726,17 +756,17 @@
         <span class="def">def</span>
         <span class="name">list_branches</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="list_branches-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#list_branches"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="list_branches-108"><a href="#list_branches-108"><span class="linenos">108</span></a><span class="k">def</span> <span class="nf">list_branches</span><span class="p">():</span>
-</span><span id="list_branches-109"><a href="#list_branches-109"><span class="linenos">109</span></a>    <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
-</span><span id="list_branches-110"><a href="#list_branches-110"><span class="linenos">110</span></a>    <span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="list_branches-113"><a href="#list_branches-113"><span class="linenos">113</span></a><span class="k">def</span> <span class="nf">list_branches</span><span class="p">():</span>
+</span><span id="list_branches-114"><a href="#list_branches-114"><span class="linenos">114</span></a>    <span class="sd">&quot;&quot;&quot;Print a list of branches.&quot;&quot;&quot;</span>
+</span><span id="list_branches-115"><a href="#list_branches-115"><span class="linenos">115</span></a>    <span class="n">branch</span><span class="p">(</span><span class="s2">&quot;-vva&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Print a list of branches.</p>
 </div>
 
 
@@ -748,17 +778,17 @@
         <span class="def">def</span>
         <span class="name">checkout</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="checkout-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#checkout"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="checkout-113"><a href="#checkout-113"><span class="linenos">113</span></a><span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="checkout-114"><a href="#checkout-114"><span class="linenos">114</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
-</span><span id="checkout-115"><a href="#checkout-115"><span class="linenos">115</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="checkout-118"><a href="#checkout-118"><span class="linenos">118</span></a><span class="k">def</span> <span class="nf">checkout</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="checkout-119"><a href="#checkout-119"><span class="linenos">119</span></a>    <span class="sd">&quot;&quot;&quot;Equivalent to `git checkout {args}`.&quot;&quot;&quot;</span>
+</span><span id="checkout-120"><a href="#checkout-120"><span class="linenos">120</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;checkout </span><span class="si">{</span><span class="n">args</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Equivalent to <code>git checkout {args}</code>.</p>
 </div>
 
 
@@ -770,19 +800,19 @@
         <span class="def">def</span>
         <span class="name">switch_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="switch_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#switch_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="switch_branch-118"><a href="#switch_branch-118"><span class="linenos">118</span></a><span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="switch_branch-119"><a href="#switch_branch-119"><span class="linenos">119</span></a>    <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
-</span><span id="switch_branch-120"><a href="#switch_branch-120"><span class="linenos">120</span></a>
-</span><span id="switch_branch-121"><a href="#switch_branch-121"><span class="linenos">121</span></a><span class="sd">    Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
-</span><span id="switch_branch-122"><a href="#switch_branch-122"><span class="linenos">122</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="switch_branch-123"><a href="#switch_branch-123"><span class="linenos">123</span></a><span class="k">def</span> <span class="nf">switch_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="switch_branch-124"><a href="#switch_branch-124"><span class="linenos">124</span></a>    <span class="sd">&quot;&quot;&quot;Switch to the branch specified by `branch_name`.</span>
+</span><span id="switch_branch-125"><a href="#switch_branch-125"><span class="linenos">125</span></a>
+</span><span id="switch_branch-126"><a href="#switch_branch-126"><span class="linenos">126</span></a><span class="sd">    Equivalent to `git checkout {branch_name}`.&quot;&quot;&quot;</span>
+</span><span id="switch_branch-127"><a href="#switch_branch-127"><span class="linenos">127</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Switch to the branch specified by <code>branch_name</code>.</p>
 
 <p>Equivalent to <code>git checkout {branch_name}</code>.</p>
 </div>
@@ -796,19 +826,19 @@
         <span class="def">def</span>
         <span class="name">create_new_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_new_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_new_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_new_branch-125"><a href="#create_new_branch-125"><span class="linenos">125</span></a><span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="create_new_branch-126"><a href="#create_new_branch-126"><span class="linenos">126</span></a>    <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
-</span><span id="create_new_branch-127"><a href="#create_new_branch-127"><span class="linenos">127</span></a>
-</span><span id="create_new_branch-128"><a href="#create_new_branch-128"><span class="linenos">128</span></a><span class="sd">    Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
-</span><span id="create_new_branch-129"><a href="#create_new_branch-129"><span class="linenos">129</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_new_branch-130"><a href="#create_new_branch-130"><span class="linenos">130</span></a><span class="k">def</span> <span class="nf">create_new_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="create_new_branch-131"><a href="#create_new_branch-131"><span class="linenos">131</span></a>    <span class="sd">&quot;&quot;&quot;Create and switch to a new branch named with `branch_name`.</span>
+</span><span id="create_new_branch-132"><a href="#create_new_branch-132"><span class="linenos">132</span></a>
+</span><span id="create_new_branch-133"><a href="#create_new_branch-133"><span class="linenos">133</span></a><span class="sd">    Equivalent to `git checkout -b {branch_name} --track`.&quot;&quot;&quot;</span>
+</span><span id="create_new_branch-134"><a href="#create_new_branch-134"><span class="linenos">134</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;-b </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2"> --track&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Create and switch to a new branch named with <code>branch_name</code>.</p>
 
 <p>Equivalent to <code>git checkout -b {branch_name} --track</code>.</p>
 </div>
@@ -822,23 +852,23 @@
         <span class="def">def</span>
         <span class="name">delete_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="delete_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#delete_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_branch-132"><a href="#delete_branch-132"><span class="linenos">132</span></a><span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
-</span><span id="delete_branch-133"><a href="#delete_branch-133"><span class="linenos">133</span></a>    <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
-</span><span id="delete_branch-134"><a href="#delete_branch-134"><span class="linenos">134</span></a>
-</span><span id="delete_branch-135"><a href="#delete_branch-135"><span class="linenos">135</span></a><span class="sd">    #### :params:</span>
-</span><span id="delete_branch-136"><a href="#delete_branch-136"><span class="linenos">136</span></a>
-</span><span id="delete_branch-137"><a href="#delete_branch-137"><span class="linenos">137</span></a><span class="sd">    `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
-</span><span id="delete_branch-138"><a href="#delete_branch-138"><span class="linenos">138</span></a>    <span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="delete_branch-139"><a href="#delete_branch-139"><span class="linenos">139</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
-</span><span id="delete_branch-140"><a href="#delete_branch-140"><span class="linenos">140</span></a>        <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_branch-137"><a href="#delete_branch-137"><span class="linenos">137</span></a><span class="k">def</span> <span class="nf">delete_branch</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">local_only</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">True</span><span class="p">):</span>
+</span><span id="delete_branch-138"><a href="#delete_branch-138"><span class="linenos">138</span></a>    <span class="sd">&quot;&quot;&quot;Delete `branch_name` from repo.</span>
+</span><span id="delete_branch-139"><a href="#delete_branch-139"><span class="linenos">139</span></a>
+</span><span id="delete_branch-140"><a href="#delete_branch-140"><span class="linenos">140</span></a><span class="sd">    #### :params:</span>
+</span><span id="delete_branch-141"><a href="#delete_branch-141"><span class="linenos">141</span></a>
+</span><span id="delete_branch-142"><a href="#delete_branch-142"><span class="linenos">142</span></a><span class="sd">    `local_only`: Only delete the local copy of `branch`, otherwise also delete the remote branch on origin and remote-tracking branch.&quot;&quot;&quot;</span>
+</span><span id="delete_branch-143"><a href="#delete_branch-143"><span class="linenos">143</span></a>    <span class="n">branch</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;--delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="delete_branch-144"><a href="#delete_branch-144"><span class="linenos">144</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">local_only</span><span class="p">:</span>
+</span><span id="delete_branch-145"><a href="#delete_branch-145"><span class="linenos">145</span></a>        <span class="n">push</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;origin --delete </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete <code>branch_name</code> from repo.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -854,19 +884,19 @@
         <span class="def">def</span>
         <span class="name">undo</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="undo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#undo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="undo-143"><a href="#undo-143"><span class="linenos">143</span></a><span class="k">def</span> <span class="nf">undo</span><span class="p">():</span>
-</span><span id="undo-144"><a href="#undo-144"><span class="linenos">144</span></a>    <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
-</span><span id="undo-145"><a href="#undo-145"><span class="linenos">145</span></a>
-</span><span id="undo-146"><a href="#undo-146"><span class="linenos">146</span></a><span class="sd">    Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
-</span><span id="undo-147"><a href="#undo-147"><span class="linenos">147</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="undo-148"><a href="#undo-148"><span class="linenos">148</span></a><span class="k">def</span> <span class="nf">undo</span><span class="p">():</span>
+</span><span id="undo-149"><a href="#undo-149"><span class="linenos">149</span></a>    <span class="sd">&quot;&quot;&quot;Undo uncommitted changes.</span>
+</span><span id="undo-150"><a href="#undo-150"><span class="linenos">150</span></a>
+</span><span id="undo-151"><a href="#undo-151"><span class="linenos">151</span></a><span class="sd">    Equivalent to `git checkout .`.&quot;&quot;&quot;</span>
+</span><span id="undo-152"><a href="#undo-152"><span class="linenos">152</span></a>    <span class="n">checkout</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Undo uncommitted changes.</p>
 
 <p>Equivalent to <code>git checkout .</code>.</p>
 </div>
@@ -880,17 +910,17 @@
         <span class="def">def</span>
         <span class="name">merge</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="merge-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#merge"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="merge-150"><a href="#merge-150"><span class="linenos">150</span></a><span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="merge-151"><a href="#merge-151"><span class="linenos">151</span></a>    <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
-</span><span id="merge-152"><a href="#merge-152"><span class="linenos">152</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="merge-155"><a href="#merge-155"><span class="linenos">155</span></a><span class="k">def</span> <span class="nf">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="merge-156"><a href="#merge-156"><span class="linenos">156</span></a>    <span class="sd">&quot;&quot;&quot;Merge branch `branch_name` with currently active branch.&quot;&quot;&quot;</span>
+</span><span id="merge-157"><a href="#merge-157"><span class="linenos">157</span></a>    <span class="n">execute</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;merge </span><span class="si">{</span><span class="n">branch_name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Merge branch <code>branch_name</code> with currently active branch.</p>
 </div>
 
 
@@ -902,24 +932,24 @@
         <span class="def">def</span>
         <span class="name">create_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="create_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#create_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="create_remote-158"><a href="#create_remote-158"><span class="linenos">158</span></a><span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
-</span><span id="create_remote-159"><a href="#create_remote-159"><span class="linenos">159</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
-</span><span id="create_remote-160"><a href="#create_remote-160"><span class="linenos">160</span></a>
-</span><span id="create_remote-161"><a href="#create_remote-161"><span class="linenos">161</span></a><span class="sd">    #### :params:</span>
-</span><span id="create_remote-162"><a href="#create_remote-162"><span class="linenos">162</span></a>
-</span><span id="create_remote-163"><a href="#create_remote-163"><span class="linenos">163</span></a><span class="sd">    `name`: The name for the repo.</span>
-</span><span id="create_remote-164"><a href="#create_remote-164"><span class="linenos">164</span></a>
-</span><span id="create_remote-165"><a href="#create_remote-165"><span class="linenos">165</span></a><span class="sd">    `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
-</span><span id="create_remote-166"><a href="#create_remote-166"><span class="linenos">166</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
-</span><span id="create_remote-167"><a href="#create_remote-167"><span class="linenos">167</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="create_remote-163"><a href="#create_remote-163"><span class="linenos">163</span></a><span class="k">def</span> <span class="nf">create_remote</span><span class="p">(</span><span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">public</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
+</span><span id="create_remote-164"><a href="#create_remote-164"><span class="linenos">164</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</span>
+</span><span id="create_remote-165"><a href="#create_remote-165"><span class="linenos">165</span></a>
+</span><span id="create_remote-166"><a href="#create_remote-166"><span class="linenos">166</span></a><span class="sd">    #### :params:</span>
+</span><span id="create_remote-167"><a href="#create_remote-167"><span class="linenos">167</span></a>
+</span><span id="create_remote-168"><a href="#create_remote-168"><span class="linenos">168</span></a><span class="sd">    `name`: The name for the repo.</span>
+</span><span id="create_remote-169"><a href="#create_remote-169"><span class="linenos">169</span></a>
+</span><span id="create_remote-170"><a href="#create_remote-170"><span class="linenos">170</span></a><span class="sd">    `public`: Set to `True` to create the repo as public, otherwise it&#39;ll be created as private.&quot;&quot;&quot;</span>
+</span><span id="create_remote-171"><a href="#create_remote-171"><span class="linenos">171</span></a>    <span class="n">visibility</span> <span class="o">=</span> <span class="s2">&quot;--public&quot;</span> <span class="k">if</span> <span class="n">public</span> <span class="k">else</span> <span class="s2">&quot;--private&quot;</span>
+</span><span id="create_remote-172"><a href="#create_remote-172"><span class="linenos">172</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo create </span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> </span><span class="si">{</span><span class="n">visibility</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to create a remote GitHub repo.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -937,23 +967,23 @@
         <span class="def">def</span>
         <span class="name">make_private</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="make_private-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#make_private"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="make_private-170"><a href="#make_private-170"><span class="linenos">170</span></a><span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="make_private-171"><a href="#make_private-171"><span class="linenos">171</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
-</span><span id="make_private-172"><a href="#make_private-172"><span class="linenos">172</span></a>
-</span><span id="make_private-173"><a href="#make_private-173"><span class="linenos">173</span></a><span class="sd">    #### :params:</span>
-</span><span id="make_private-174"><a href="#make_private-174"><span class="linenos">174</span></a>
-</span><span id="make_private-175"><a href="#make_private-175"><span class="linenos">175</span></a><span class="sd">    `owner`: The repo owner.</span>
-</span><span id="make_private-176"><a href="#make_private-176"><span class="linenos">176</span></a>
-</span><span id="make_private-177"><a href="#make_private-177"><span class="linenos">177</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="make_private-178"><a href="#make_private-178"><span class="linenos">178</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility private&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="make_private-175"><a href="#make_private-175"><span class="linenos">175</span></a><span class="k">def</span> <span class="nf">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="make_private-176"><a href="#make_private-176"><span class="linenos">176</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to private.</span>
+</span><span id="make_private-177"><a href="#make_private-177"><span class="linenos">177</span></a>
+</span><span id="make_private-178"><a href="#make_private-178"><span class="linenos">178</span></a><span class="sd">    #### :params:</span>
+</span><span id="make_private-179"><a href="#make_private-179"><span class="linenos">179</span></a>
+</span><span id="make_private-180"><a href="#make_private-180"><span class="linenos">180</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="make_private-181"><a href="#make_private-181"><span class="linenos">181</span></a>
+</span><span id="make_private-182"><a href="#make_private-182"><span class="linenos">182</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="make_private-183"><a href="#make_private-183"><span class="linenos">183</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility private&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to private.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -971,23 +1001,23 @@
         <span class="def">def</span>
         <span class="name">make_public</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="make_public-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#make_public"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="make_public-181"><a href="#make_public-181"><span class="linenos">181</span></a><span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="make_public-182"><a href="#make_public-182"><span class="linenos">182</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
-</span><span id="make_public-183"><a href="#make_public-183"><span class="linenos">183</span></a>
-</span><span id="make_public-184"><a href="#make_public-184"><span class="linenos">184</span></a><span class="sd">    #### :params:</span>
-</span><span id="make_public-185"><a href="#make_public-185"><span class="linenos">185</span></a>
-</span><span id="make_public-186"><a href="#make_public-186"><span class="linenos">186</span></a><span class="sd">    `owner`: The repo owner.</span>
-</span><span id="make_public-187"><a href="#make_public-187"><span class="linenos">187</span></a>
-</span><span id="make_public-188"><a href="#make_public-188"><span class="linenos">188</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
-</span><span id="make_public-189"><a href="#make_public-189"><span class="linenos">189</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility public&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="make_public-186"><a href="#make_public-186"><span class="linenos">186</span></a><span class="k">def</span> <span class="nf">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="make_public-187"><a href="#make_public-187"><span class="linenos">187</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be installed and configured) to set the repo&#39;s visibility to public.</span>
+</span><span id="make_public-188"><a href="#make_public-188"><span class="linenos">188</span></a>
+</span><span id="make_public-189"><a href="#make_public-189"><span class="linenos">189</span></a><span class="sd">    #### :params:</span>
+</span><span id="make_public-190"><a href="#make_public-190"><span class="linenos">190</span></a>
+</span><span id="make_public-191"><a href="#make_public-191"><span class="linenos">191</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="make_public-192"><a href="#make_public-192"><span class="linenos">192</span></a>
+</span><span id="make_public-193"><a href="#make_public-193"><span class="linenos">193</span></a><span class="sd">    `name`: The name of the repo to edit.&quot;&quot;&quot;</span>
+</span><span id="make_public-194"><a href="#make_public-194"><span class="linenos">194</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo edit </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --visibility public&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be installed and configured) to set the repo's visibility to public.</p>
 
 <h4 id="params">:params:</h4>
 
@@ -1005,23 +1035,23 @@
         <span class="def">def</span>
         <span class="name">delete_remote</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span>, </span><span class="param"><span class="n">name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="delete_remote-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#delete_remote"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_remote-192"><a href="#delete_remote-192"><span class="linenos">192</span></a><span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="delete_remote-193"><a href="#delete_remote-193"><span class="linenos">193</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
-</span><span id="delete_remote-194"><a href="#delete_remote-194"><span class="linenos">194</span></a>
-</span><span id="delete_remote-195"><a href="#delete_remote-195"><span class="linenos">195</span></a><span class="sd">    #### :params:</span>
-</span><span id="delete_remote-196"><a href="#delete_remote-196"><span class="linenos">196</span></a>
-</span><span id="delete_remote-197"><a href="#delete_remote-197"><span class="linenos">197</span></a><span class="sd">    `owner`: The repo owner.</span>
-</span><span id="delete_remote-198"><a href="#delete_remote-198"><span class="linenos">198</span></a>
-</span><span id="delete_remote-199"><a href="#delete_remote-199"><span class="linenos">199</span></a><span class="sd">    `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
-</span><span id="delete_remote-200"><a href="#delete_remote-200"><span class="linenos">200</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo delete </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --yes&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_remote-197"><a href="#delete_remote-197"><span class="linenos">197</span></a><span class="k">def</span> <span class="nf">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">,</span> <span class="n">name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="delete_remote-198"><a href="#delete_remote-198"><span class="linenos">198</span></a>    <span class="sd">&quot;&quot;&quot;Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</span>
+</span><span id="delete_remote-199"><a href="#delete_remote-199"><span class="linenos">199</span></a>
+</span><span id="delete_remote-200"><a href="#delete_remote-200"><span class="linenos">200</span></a><span class="sd">    #### :params:</span>
+</span><span id="delete_remote-201"><a href="#delete_remote-201"><span class="linenos">201</span></a>
+</span><span id="delete_remote-202"><a href="#delete_remote-202"><span class="linenos">202</span></a><span class="sd">    `owner`: The repo owner.</span>
+</span><span id="delete_remote-203"><a href="#delete_remote-203"><span class="linenos">203</span></a>
+</span><span id="delete_remote-204"><a href="#delete_remote-204"><span class="linenos">204</span></a><span class="sd">    `name`: The name of the remote repo to delete.&quot;&quot;&quot;</span>
+</span><span id="delete_remote-205"><a href="#delete_remote-205"><span class="linenos">205</span></a>    <span class="n">os</span><span class="o">.</span><span class="n">system</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;gh repo delete </span><span class="si">{</span><span class="n">owner</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="n">name</span><span class="si">}</span><span class="s2"> --yes&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Uses GitHub CLI (must be isntalled and configured) to delete the remote for this repo.</p>
 
 <h4 id="params">:params:</h4>
```

#### html2text {}

```diff
@@ -2,14 +2,15 @@
 
   ⁰
 ____ gitbetter [Unknown INPUT type]
 ***** API Documentation *****
     * execute
     * new_repo
     * loggy
+    * status
     * commit
     * add
     * commit_files
     * initcommit
     * amend
     * tag
     * add_remote_url
@@ -52,201 +53,206 @@
 _17
 _18def loggy():
 _19    """Equivalent to `git log --oneline --name-only --abbrev-commit --
 graph`."""
 _20    execute("log --oneline --name-only --abbrev-commit --graph")
 _21
 _22
-_23# ======================================Staging/
-Committing======================================
-_24def commit(args: str):
-_25    """>>> git commit {args}"""
-_26    execute(f"commit {args}")
+_23def status():
+_24    """Execute `git status`."""
+_25    execute("status")
+_26
 _27
-_28
-_29def add(files: list[str] | None = None):
-_30    """Stage a list of files.
-_31
-_32    If no files are given (`files=None`), all files will be staged."""
-_33    if not files:
-_34        execute("add .")
-_35    else:
-_36        execute(f'add {" ".join(files)}')
-_37
-_38
-_39def commit_files(files: list[str], message: str):
-_40    """Stage and commit a list of files with commit message `message`."""
-_41    add(files)
-_42    commit(f'-m "{message}"')
+_28# ======================================Staging/
+Committing======================================
+_29def commit(args: str):
+_30    """>>> git commit {args}"""
+_31    execute(f"commit {args}")
+_32
+_33
+_34def add(files: list[str] | None = None):
+_35    """Stage a list of files.
+_36
+_37    If no files are given (`files=None`), all files will be staged."""
+_38    if not files:
+_39        execute("add .")
+_40    else:
+_41        execute(f'add {" ".join(files)}')
+_42
 _43
-_44
-_45def initcommit():
-_46    """Equivalent to
-_47    >>> git add .
-_48    >>> git commit -m "Initial commit" """
-_49    add()
-_50    commit('-m "Initial commit"')
-_51
-_52
-_53def amend(files: list[str] | None = None):
-_54    """Stage and commit changes to the previous commit.
-_55
-_56    If `files` is `None`, all files will be staged.
+_44def commit_files(files: list[str], message: str):
+_45    """Stage and commit a list of files with commit message `message`."""
+_46    add(files)
+_47    commit(f'-m "{message}"')
+_48
+_49
+_50def initcommit():
+_51    """Equivalent to
+_52    >>> git add .
+_53    >>> git commit -m "Initial commit" """
+_54    add()
+_55    commit('-m "Initial commit"')
+_56
 _57
-_58    Equivalent to:
-_59    >>> git add {files}
-_60    >>> git commit --amend --no-edit
-_61    """
-_62    add(files)
-_63    commit("--amend --no-edit")
-_64
-_65
-_66def tag(id_: str):
-_67    """Tag the current commit with `id_`.
-_68
-_69    Equivalent to `git tag {id_}`."""
-_70    execute(f"tag {id_}")
-_71
-_72
-_73# ==========================================Push/
-Pull==========================================
-_74def add_remote_url(url: str, name: str = "origin"):
-_75    """Add remote url to repo."""
-_76    execute(f"remote add {name} {url}")
+_58def amend(files: list[str] | None = None):
+_59    """Stage and commit changes to the previous commit.
+_60
+_61    If `files` is `None`, all files will be staged.
+_62
+_63    Equivalent to:
+_64    >>> git add {files}
+_65    >>> git commit --amend --no-edit
+_66    """
+_67    add(files)
+_68    commit("--amend --no-edit")
+_69
+_70
+_71def tag(id_: str):
+_72    """Tag the current commit with `id_`.
+_73
+_74    Equivalent to `git tag {id_}`."""
+_75    execute(f"tag {id_}")
+_76
 _77
-_78
-_79def push(args: str = ""):
-_80    """Equivalent to `git push {args}`."""
-_81    execute(f"push {args}")
+_78# ==========================================Push/
+Pull==========================================
+_79def add_remote_url(url: str, name: str = "origin"):
+_80    """Add remote url to repo."""
+_81    execute(f"remote add {name} {url}")
 _82
 _83
-_84def pull(args: str = ""):
-_85    """Equivalent to `git pull {args}`."""
-_86    execute(f"pull {args}")
+_84def push(args: str = ""):
+_85    """Equivalent to `git push {args}`."""
+_86    execute(f"push {args}")
 _87
 _88
-_89def push_new_branch(branch: str):
-_90    """Push a new branch to origin with tracking.
-_91
-_92    Equivalent to `git push -u origin {branch}`."""
-_93    push(f"-u origin {branch}")
-_94
-_95
-_96def pull_branch(branch: str):
-_97    """Pull `branch` from origin."""
-_98    pull(f"origin {branch}")
+_89def pull(args: str = ""):
+_90    """Equivalent to `git pull {args}`."""
+_91    execute(f"pull {args}")
+_92
+_93
+_94def push_new_branch(branch: str):
+_95    """Push a new branch to origin with tracking.
+_96
+_97    Equivalent to `git push -u origin {branch}`."""
+_98    push(f"-u origin {branch}")
 _99
 100
-101# ============================================Checkout/
-Branches============================================
-102def branch(args: str):
-103    """Equivalent to `git branch {args}`."""
-104    execute(f"branch {args}")
+101def pull_branch(branch: str):
+102    """Pull `branch` from origin."""
+103    pull(f"origin {branch}")
+104
 105
-106
-107def list_branches():
-108    """Print a list of branches."""
-109    branch("-vva")
+106# ============================================Checkout/
+Branches============================================
+107def branch(args: str):
+108    """Equivalent to `git branch {args}`."""
+109    execute(f"branch {args}")
 110
 111
-112def checkout(args: str):
-113    """Equivalent to `git checkout {args}`."""
-114    execute(f"checkout {args}")
+112def list_branches():
+113    """Print a list of branches."""
+114    branch("-vva")
 115
 116
-117def switch_branch(branch_name: str):
-118    """Switch to the branch specified by `branch_name`.
-119
-120    Equivalent to `git checkout {branch_name}`."""
-121    checkout(branch_name)
-122
-123
-124def create_new_branch(branch_name: str):
-125    """Create and switch to a new branch named with `branch_name`.
-126
-127    Equivalent to `git checkout -b {branch_name} --track`."""
-128    checkout(f"-b {branch_name} --track")
-129
-130
-131def delete_branch(branch_name: str, local_only: bool = True):
-132    """Delete `branch_name` from repo.
-133
-134    #### :params:
+117def checkout(args: str):
+118    """Equivalent to `git checkout {args}`."""
+119    execute(f"checkout {args}")
+120
+121
+122def switch_branch(branch_name: str):
+123    """Switch to the branch specified by `branch_name`.
+124
+125    Equivalent to `git checkout {branch_name}`."""
+126    checkout(branch_name)
+127
+128
+129def create_new_branch(branch_name: str):
+130    """Create and switch to a new branch named with `branch_name`.
+131
+132    Equivalent to `git checkout -b {branch_name} --track`."""
+133    checkout(f"-b {branch_name} --track")
+134
 135
-136    `local_only`: Only delete the local copy of `branch`, otherwise also
-delete the remote branch on origin and remote-tracking branch."""
-137    branch(f"--delete {branch_name}")
-138    if not local_only:
-139        push(f"origin --delete {branch_name}")
+136def delete_branch(branch_name: str, local_only: bool = True):
+137    """Delete `branch_name` from repo.
+138
+139    #### :params:
 140
-141
-142def undo():
-143    """Undo uncommitted changes.
-144
-145    Equivalent to `git checkout .`."""
-146    checkout(".")
-147
-148
-149def merge(branch_name: str):
-150    """Merge branch `branch_name` with currently active branch."""
-151    execute(f"merge {branch_name}")
+141    `local_only`: Only delete the local copy of `branch`, otherwise also
+delete the remote branch on origin and remote-tracking branch."""
+142    branch(f"--delete {branch_name}")
+143    if not local_only:
+144        push(f"origin --delete {branch_name}")
+145
+146
+147def undo():
+148    """Undo uncommitted changes.
+149
+150    Equivalent to `git checkout .`."""
+151    checkout(".")
 152
 153
-154# ===============================Requires GitHub CLI to be installed and
+154def merge(branch_name: str):
+155    """Merge branch `branch_name` with currently active branch."""
+156    execute(f"merge {branch_name}")
+157
+158
+159# ===============================Requires GitHub CLI to be installed and
 configured===============================
-155
-156
-157def create_remote(name: str, public: bool = False):
-158    """Uses GitHub CLI (must be installed and configured) to create a remote
-GitHub repo.
-159
-160    #### :params:
+160
 161
-162    `name`: The name for the repo.
-163
-164    `public`: Set to `True` to create the repo as public, otherwise it'll be
-created as private."""
-165    visibility = "--public" if public else "--private"
-166    os.system(f"gh repo create {name} {visibility}")
-167
+162def create_remote(name: str, public: bool = False):
+163    """Uses GitHub CLI (must be installed and configured) to create a remote
+GitHub repo.
+164
+165    #### :params:
+166
+167    `name`: The name for the repo.
 168
-169def make_private(owner: str, name: str):
-170    """Uses GitHub CLI (must be installed and configured) to set the repo's
-visibility to private.
-171
-172    #### :params:
+169    `public`: Set to `True` to create the repo as public, otherwise it'll be
+created as private."""
+170    visibility = "--public" if public else "--private"
+171    os.system(f"gh repo create {name} {visibility}")
+172
 173
-174    `owner`: The repo owner.
-175
-176    `name`: The name of the repo to edit."""
-177    os.system(f"gh repo edit {owner}/{name} --visibility private")
+174def make_private(owner: str, name: str):
+175    """Uses GitHub CLI (must be installed and configured) to set the repo's
+visibility to private.
+176
+177    #### :params:
 178
-179
-180def make_public(owner: str, name: str):
-181    """Uses GitHub CLI (must be installed and configured) to set the repo's
-visibility to public.
-182
-183    #### :params:
+179    `owner`: The repo owner.
+180
+181    `name`: The name of the repo to edit."""
+182    os.system(f"gh repo edit {owner}/{name} --visibility private")
+183
 184
-185    `owner`: The repo owner.
-186
-187    `name`: The name of the repo to edit."""
-188    os.system(f"gh repo edit {owner}/{name} --visibility public")
+185def make_public(owner: str, name: str):
+186    """Uses GitHub CLI (must be installed and configured) to set the repo's
+visibility to public.
+187
+188    #### :params:
 189
-190
-191def delete_remote(owner: str, name: str):
-192    """Uses GitHub CLI (must be isntalled and configured) to delete the
-remote for this repo.
-193
-194    #### :params:
+190    `owner`: The repo owner.
+191
+192    `name`: The name of the repo to edit."""
+193    os.system(f"gh repo edit {owner}/{name} --visibility public")
+194
 195
-196    `owner`: The repo owner.
-197
-198    `name`: The name of the remote repo to delete."""
-199    os.system(f"gh repo delete {owner}/{name} --yes")
+196def delete_remote(owner: str, name: str):
+197    """Uses GitHub CLI (must be isntalled and configured) to delete the
+remote for this repo.
+198
+199    #### :params:
+200
+201    `owner`: The repo owner.
+202
+203    `name`: The name of the remote repo to delete."""
+204    os.system(f"gh repo delete {owner}/{name} --yes")
   ⁰
 def execute(command: str) -> int: View Source
 _5def execute(command: str) -> int:
 _6    """Execute git command.
 _7
 _8    Equivalent to `os.system(f"git {command}")`
 _9
@@ -265,241 +271,247 @@
 def loggy(): View Source
 19def loggy():
 20    """Equivalent to `git log --oneline --name-only --abbrev-commit --
 graph`."""
 21    execute("log --oneline --name-only --abbrev-commit --graph")
 Equivalent to git log --oneline --name-only --abbrev-commit --graph.
   ⁰
+def status(): View Source
+24def status():
+25    """Execute `git status`."""
+26    execute("status")
+Execute git status.
+  ⁰
 def commit(args: str): View Source
-25def commit(args: str):
-26    """>>> git commit {args}"""
-27    execute(f"commit {args}")
+30def commit(args: str):
+31    """>>> git commit {args}"""
+32    execute(f"commit {args}")
 >>> git commit {args}
   ⁰
 def add(files: list[str] | None = None): View Source
-30def add(files: list[str] | None = None):
-31    """Stage a list of files.
-32
-33    If no files are given (`files=None`), all files will be staged."""
-34    if not files:
-35        execute("add .")
-36    else:
-37        execute(f'add {" ".join(files)}')
+35def add(files: list[str] | None = None):
+36    """Stage a list of files.
+37
+38    If no files are given (`files=None`), all files will be staged."""
+39    if not files:
+40        execute("add .")
+41    else:
+42        execute(f'add {" ".join(files)}')
 Stage a list of files.
 If no files are given (files=None), all files will be staged.
   ⁰
 def commit_files(files: list[str], message: str): View Source
-40def commit_files(files: list[str], message: str):
-41    """Stage and commit a list of files with commit message `message`."""
-42    add(files)
-43    commit(f'-m "{message}"')
+45def commit_files(files: list[str], message: str):
+46    """Stage and commit a list of files with commit message `message`."""
+47    add(files)
+48    commit(f'-m "{message}"')
 Stage and commit a list of files with commit message message.
   ⁰
 def initcommit(): View Source
-46def initcommit():
-47    """Equivalent to
-48    >>> git add .
-49    >>> git commit -m "Initial commit" """
-50    add()
-51    commit('-m "Initial commit"')
+51def initcommit():
+52    """Equivalent to
+53    >>> git add .
+54    >>> git commit -m "Initial commit" """
+55    add()
+56    commit('-m "Initial commit"')
 Equivalent to
 >>> git add .
 >>> git commit -m "Initial commit"
   ⁰
 def amend(files: list[str] | None = None): View Source
-54def amend(files: list[str] | None = None):
-55    """Stage and commit changes to the previous commit.
-56
-57    If `files` is `None`, all files will be staged.
-58
-59    Equivalent to:
-60    >>> git add {files}
-61    >>> git commit --amend --no-edit
-62    """
-63    add(files)
-64    commit("--amend --no-edit")
+59def amend(files: list[str] | None = None):
+60    """Stage and commit changes to the previous commit.
+61
+62    If `files` is `None`, all files will be staged.
+63
+64    Equivalent to:
+65    >>> git add {files}
+66    >>> git commit --amend --no-edit
+67    """
+68    add(files)
+69    commit("--amend --no-edit")
 Stage and commit changes to the previous commit.
 If files is None, all files will be staged.
 Equivalent to:
 >>> git add {files}
 >>> git commit --amend --no-edit
   ⁰
 def tag(id_: str): View Source
-67def tag(id_: str):
-68    """Tag the current commit with `id_`.
-69
-70    Equivalent to `git tag {id_}`."""
-71    execute(f"tag {id_}")
+72def tag(id_: str):
+73    """Tag the current commit with `id_`.
+74
+75    Equivalent to `git tag {id_}`."""
+76    execute(f"tag {id_}")
 Tag the current commit with id_.
 Equivalent to git tag {id_}.
   ⁰
 def add_remote_url(url: str, name: str = 'origin'): View Source
-75def add_remote_url(url: str, name: str = "origin"):
-76    """Add remote url to repo."""
-77    execute(f"remote add {name} {url}")
+80def add_remote_url(url: str, name: str = "origin"):
+81    """Add remote url to repo."""
+82    execute(f"remote add {name} {url}")
 Add remote url to repo.
   ⁰
 def push(args: str = ''): View Source
-80def push(args: str = ""):
-81    """Equivalent to `git push {args}`."""
-82    execute(f"push {args}")
+85def push(args: str = ""):
+86    """Equivalent to `git push {args}`."""
+87    execute(f"push {args}")
 Equivalent to git push {args}.
   ⁰
 def pull(args: str = ''): View Source
-85def pull(args: str = ""):
-86    """Equivalent to `git pull {args}`."""
-87    execute(f"pull {args}")
+90def pull(args: str = ""):
+91    """Equivalent to `git pull {args}`."""
+92    execute(f"pull {args}")
 Equivalent to git pull {args}.
   ⁰
 def push_new_branch(branch: str): View Source
-90def push_new_branch(branch: str):
-91    """Push a new branch to origin with tracking.
-92
-93    Equivalent to `git push -u origin {branch}`."""
-94    push(f"-u origin {branch}")
+95def push_new_branch(branch: str):
+96    """Push a new branch to origin with tracking.
+97
+98    Equivalent to `git push -u origin {branch}`."""
+99    push(f"-u origin {branch}")
 Push a new branch to origin with tracking.
 Equivalent to git push -u origin {branch}.
   ⁰
 def pull_branch(branch: str): View Source
-97def pull_branch(branch: str):
-98    """Pull `branch` from origin."""
-99    pull(f"origin {branch}")
+102def pull_branch(branch: str):
+103    """Pull `branch` from origin."""
+104    pull(f"origin {branch}")
 Pull branch from origin.
   ⁰
 def branch(args: str): View Source
-103def branch(args: str):
-104    """Equivalent to `git branch {args}`."""
-105    execute(f"branch {args}")
+108def branch(args: str):
+109    """Equivalent to `git branch {args}`."""
+110    execute(f"branch {args}")
 Equivalent to git branch {args}.
   ⁰
 def list_branches(): View Source
-108def list_branches():
-109    """Print a list of branches."""
-110    branch("-vva")
+113def list_branches():
+114    """Print a list of branches."""
+115    branch("-vva")
 Print a list of branches.
   ⁰
 def checkout(args: str): View Source
-113def checkout(args: str):
-114    """Equivalent to `git checkout {args}`."""
-115    execute(f"checkout {args}")
+118def checkout(args: str):
+119    """Equivalent to `git checkout {args}`."""
+120    execute(f"checkout {args}")
 Equivalent to git checkout {args}.
   ⁰
 def switch_branch(branch_name: str): View Source
-118def switch_branch(branch_name: str):
-119    """Switch to the branch specified by `branch_name`.
-120
-121    Equivalent to `git checkout {branch_name}`."""
-122    checkout(branch_name)
+123def switch_branch(branch_name: str):
+124    """Switch to the branch specified by `branch_name`.
+125
+126    Equivalent to `git checkout {branch_name}`."""
+127    checkout(branch_name)
 Switch to the branch specified by branch_name.
 Equivalent to git checkout {branch_name}.
   ⁰
 def create_new_branch(branch_name: str): View Source
-125def create_new_branch(branch_name: str):
-126    """Create and switch to a new branch named with `branch_name`.
-127
-128    Equivalent to `git checkout -b {branch_name} --track`."""
-129    checkout(f"-b {branch_name} --track")
+130def create_new_branch(branch_name: str):
+131    """Create and switch to a new branch named with `branch_name`.
+132
+133    Equivalent to `git checkout -b {branch_name} --track`."""
+134    checkout(f"-b {branch_name} --track")
 Create and switch to a new branch named with branch_name.
 Equivalent to git checkout -b {branch_name} --track.
   ⁰
 def delete_branch(branch_name: str, local_only: bool = True): View Source
-132def delete_branch(branch_name: str, local_only: bool = True):
-133    """Delete `branch_name` from repo.
-134
-135    #### :params:
-136
-137    `local_only`: Only delete the local copy of `branch`, otherwise also
+137def delete_branch(branch_name: str, local_only: bool = True):
+138    """Delete `branch_name` from repo.
+139
+140    #### :params:
+141
+142    `local_only`: Only delete the local copy of `branch`, otherwise also
 delete the remote branch on origin and remote-tracking branch."""
-138    branch(f"--delete {branch_name}")
-139    if not local_only:
-140        push(f"origin --delete {branch_name}")
+143    branch(f"--delete {branch_name}")
+144    if not local_only:
+145        push(f"origin --delete {branch_name}")
 Delete branch_name from repo.
 *** :params: ***
 local_only: Only delete the local copy of branch, otherwise also delete the
 remote branch on origin and remote-tracking branch.
   ⁰
 def undo(): View Source
-143def undo():
-144    """Undo uncommitted changes.
-145
-146    Equivalent to `git checkout .`."""
-147    checkout(".")
+148def undo():
+149    """Undo uncommitted changes.
+150
+151    Equivalent to `git checkout .`."""
+152    checkout(".")
 Undo uncommitted changes.
 Equivalent to git checkout ..
   ⁰
 def merge(branch_name: str): View Source
-150def merge(branch_name: str):
-151    """Merge branch `branch_name` with currently active branch."""
-152    execute(f"merge {branch_name}")
+155def merge(branch_name: str):
+156    """Merge branch `branch_name` with currently active branch."""
+157    execute(f"merge {branch_name}")
 Merge branch branch_name with currently active branch.
   ⁰
 def create_remote(name: str, public: bool = False): View Source
-158def create_remote(name: str, public: bool = False):
-159    """Uses GitHub CLI (must be installed and configured) to create a remote
+163def create_remote(name: str, public: bool = False):
+164    """Uses GitHub CLI (must be installed and configured) to create a remote
 GitHub repo.
-160
-161    #### :params:
-162
-163    `name`: The name for the repo.
-164
-165    `public`: Set to `True` to create the repo as public, otherwise it'll be
+165
+166    #### :params:
+167
+168    `name`: The name for the repo.
+169
+170    `public`: Set to `True` to create the repo as public, otherwise it'll be
 created as private."""
-166    visibility = "--public" if public else "--private"
-167    os.system(f"gh repo create {name} {visibility}")
+171    visibility = "--public" if public else "--private"
+172    os.system(f"gh repo create {name} {visibility}")
 Uses GitHub CLI (must be installed and configured) to create a remote GitHub
 repo.
 *** :params: ***
 name: The name for the repo.
 public: Set to True to create the repo as public, otherwise it'll be created as
 private.
   ⁰
 def make_private(owner: str, name: str): View Source
-170def make_private(owner: str, name: str):
-171    """Uses GitHub CLI (must be installed and configured) to set the repo's
+175def make_private(owner: str, name: str):
+176    """Uses GitHub CLI (must be installed and configured) to set the repo's
 visibility to private.
-172
-173    #### :params:
-174
-175    `owner`: The repo owner.
-176
-177    `name`: The name of the repo to edit."""
-178    os.system(f"gh repo edit {owner}/{name} --visibility private")
+177
+178    #### :params:
+179
+180    `owner`: The repo owner.
+181
+182    `name`: The name of the repo to edit."""
+183    os.system(f"gh repo edit {owner}/{name} --visibility private")
 Uses GitHub CLI (must be installed and configured) to set the repo's visibility
 to private.
 *** :params: ***
 owner: The repo owner.
 name: The name of the repo to edit.
   ⁰
 def make_public(owner: str, name: str): View Source
-181def make_public(owner: str, name: str):
-182    """Uses GitHub CLI (must be installed and configured) to set the repo's
+186def make_public(owner: str, name: str):
+187    """Uses GitHub CLI (must be installed and configured) to set the repo's
 visibility to public.
-183
-184    #### :params:
-185
-186    `owner`: The repo owner.
-187
-188    `name`: The name of the repo to edit."""
-189    os.system(f"gh repo edit {owner}/{name} --visibility public")
+188
+189    #### :params:
+190
+191    `owner`: The repo owner.
+192
+193    `name`: The name of the repo to edit."""
+194    os.system(f"gh repo edit {owner}/{name} --visibility public")
 Uses GitHub CLI (must be installed and configured) to set the repo's visibility
 to public.
 *** :params: ***
 owner: The repo owner.
 name: The name of the repo to edit.
   ⁰
 def delete_remote(owner: str, name: str): View Source
-192def delete_remote(owner: str, name: str):
-193    """Uses GitHub CLI (must be isntalled and configured) to delete the
+197def delete_remote(owner: str, name: str):
+198    """Uses GitHub CLI (must be isntalled and configured) to delete the
 remote for this repo.
-194
-195    #### :params:
-196
-197    `owner`: The repo owner.
-198
-199    `name`: The name of the remote repo to delete."""
-200    os.system(f"gh repo delete {owner}/{name} --yes")
+199
+200    #### :params:
+201
+202    `owner`: The repo owner.
+203
+204    `name`: The name of the remote repo to delete."""
+205    os.system(f"gh repo delete {owner}/{name} --yes")
 Uses GitHub CLI (must be isntalled and configured) to delete the remote for
 this repo.
 *** :params: ***
 owner: The repo owner.
 name: The name of the remote repo to delete.
```

### Comparing `gitbetter-0.3.0/docs/gitbetter/gitbetter.html` & `gitbetter-0.4.0/docs/gitbetter/gitbetter.html`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,17 @@
                         <li>
                                 <a class="function" href="#GitBetter.do_list_branches">do_list_branches</a>
                         </li>
                         <li>
                                 <a class="function" href="#GitBetter.do_loggy">do_loggy</a>
                         </li>
                         <li>
+                                <a class="function" href="#GitBetter.do_status">do_status</a>
+                        </li>
+                        <li>
                                 <a class="function" href="#GitBetter.do_merge">do_merge</a>
                         </li>
                         <li>
                                 <a class="function" href="#GitBetter.do_tag">do_tag</a>
                         </li>
                         <li>
                                 <a class="function" href="#GitBetter.do_amend">do_amend</a>
@@ -395,76 +398,80 @@
 </span><span id="L-225"><a href="#L-225"><span class="linenos">225</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
 </span><span id="L-226"><a href="#L-226"><span class="linenos">226</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
 </span><span id="L-227"><a href="#L-227"><span class="linenos">227</span></a>
 </span><span id="L-228"><a href="#L-228"><span class="linenos">228</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="L-229"><a href="#L-229"><span class="linenos">229</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
 </span><span id="L-230"><a href="#L-230"><span class="linenos">230</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
 </span><span id="L-231"><a href="#L-231"><span class="linenos">231</span></a>
-</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="L-232"><a href="#L-232"><span class="linenos">232</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-233"><a href="#L-233"><span class="linenos">233</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="L-234"><a href="#L-234"><span class="linenos">234</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
 </span><span id="L-235"><a href="#L-235"><span class="linenos">235</span></a>
-</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="L-236"><a href="#L-236"><span class="linenos">236</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-237"><a href="#L-237"><span class="linenos">237</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="L-238"><a href="#L-238"><span class="linenos">238</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span><span id="L-239"><a href="#L-239"><span class="linenos">239</span></a>
-</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>
-</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
-</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>
-</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+</span><span id="L-240"><a href="#L-240"><span class="linenos">240</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-241"><a href="#L-241"><span class="linenos">241</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="L-242"><a href="#L-242"><span class="linenos">242</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="L-243"><a href="#L-243"><span class="linenos">243</span></a>
+</span><span id="L-244"><a href="#L-244"><span class="linenos">244</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="L-245"><a href="#L-245"><span class="linenos">245</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-246"><a href="#L-246"><span class="linenos">246</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="L-247"><a href="#L-247"><span class="linenos">247</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="L-248"><a href="#L-248"><span class="linenos">248</span></a>
+</span><span id="L-249"><a href="#L-249"><span class="linenos">249</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="L-250"><a href="#L-250"><span class="linenos">250</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="L-251"><a href="#L-251"><span class="linenos">251</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="L-252"><a href="#L-252"><span class="linenos">252</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
 </span><span id="L-253"><a href="#L-253"><span class="linenos">253</span></a>
-</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
-</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>
-</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>
-</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>
-</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a>
-</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>
-</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>
-</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a>
-</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>
-</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>
-</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="L-254"><a href="#L-254"><span class="linenos">254</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-255"><a href="#L-255"><span class="linenos">255</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="L-256"><a href="#L-256"><span class="linenos">256</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+</span><span id="L-257"><a href="#L-257"><span class="linenos">257</span></a>
+</span><span id="L-258"><a href="#L-258"><span class="linenos">258</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-259"><a href="#L-259"><span class="linenos">259</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="L-260"><a href="#L-260"><span class="linenos">260</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="L-261"><a href="#L-261"><span class="linenos">261</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="L-262"><a href="#L-262"><span class="linenos">262</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-263"><a href="#L-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+</span><span id="L-264"><a href="#L-264"><span class="linenos">264</span></a>
+</span><span id="L-265"><a href="#L-265"><span class="linenos">265</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-266"><a href="#L-266"><span class="linenos">266</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="L-267"><a href="#L-267"><span class="linenos">267</span></a>
+</span><span id="L-268"><a href="#L-268"><span class="linenos">268</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-269"><a href="#L-269"><span class="linenos">269</span></a>
+</span><span id="L-270"><a href="#L-270"><span class="linenos">270</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="L-271"><a href="#L-271"><span class="linenos">271</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-272"><a href="#L-272"><span class="linenos">272</span></a>
+</span><span id="L-273"><a href="#L-273"><span class="linenos">273</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-274"><a href="#L-274"><span class="linenos">274</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="L-275"><a href="#L-275"><span class="linenos">275</span></a>
+</span><span id="L-276"><a href="#L-276"><span class="linenos">276</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-277"><a href="#L-277"><span class="linenos">277</span></a>
+</span><span id="L-278"><a href="#L-278"><span class="linenos">278</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="L-279"><a href="#L-279"><span class="linenos">279</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="L-280"><a href="#L-280"><span class="linenos">280</span></a>
+</span><span id="L-281"><a href="#L-281"><span class="linenos">281</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="L-282"><a href="#L-282"><span class="linenos">282</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
 </span><span id="L-283"><a href="#L-283"><span class="linenos">283</span></a>
-</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a>
+</span><span id="L-284"><a href="#L-284"><span class="linenos">284</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="L-285"><a href="#L-285"><span class="linenos">285</span></a>
+</span><span id="L-286"><a href="#L-286"><span class="linenos">286</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
 </span><span id="L-287"><a href="#L-287"><span class="linenos">287</span></a>
-</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+</span><span id="L-288"><a href="#L-288"><span class="linenos">288</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="L-289"><a href="#L-289"><span class="linenos">289</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span><span id="L-290"><a href="#L-290"><span class="linenos">290</span></a>
 </span><span id="L-291"><a href="#L-291"><span class="linenos">291</span></a>
-</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>    <span class="n">main</span><span class="p">()</span>
+</span><span id="L-292"><a href="#L-292"><span class="linenos">292</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="L-293"><a href="#L-293"><span class="linenos">293</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+</span><span id="L-294"><a href="#L-294"><span class="linenos">294</span></a>
+</span><span id="L-295"><a href="#L-295"><span class="linenos">295</span></a>
+</span><span id="L-296"><a href="#L-296"><span class="linenos">296</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-297"><a href="#L-297"><span class="linenos">297</span></a>    <span class="n">main</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
                 <section id="new_remote_parser">
                             <input id="new_remote_parser-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -785,68 +792,72 @@
 </span><span id="GitBetter-226"><a href="#GitBetter-226"><span class="linenos">226</span></a>        <span class="sd">&quot;&quot;&quot;Show local and remote branches.&quot;&quot;&quot;</span>
 </span><span id="GitBetter-227"><a href="#GitBetter-227"><span class="linenos">227</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">list_branches</span><span class="p">()</span>
 </span><span id="GitBetter-228"><a href="#GitBetter-228"><span class="linenos">228</span></a>
 </span><span id="GitBetter-229"><a href="#GitBetter-229"><span class="linenos">229</span></a>    <span class="k">def</span> <span class="nf">do_loggy</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
 </span><span id="GitBetter-230"><a href="#GitBetter-230"><span class="linenos">230</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git --oneline --name-only --abbrev-commit --graph`.&quot;&quot;&quot;</span>
 </span><span id="GitBetter-231"><a href="#GitBetter-231"><span class="linenos">231</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">loggy</span><span class="p">()</span>
 </span><span id="GitBetter-232"><a href="#GitBetter-232"><span class="linenos">232</span></a>
-</span><span id="GitBetter-233"><a href="#GitBetter-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-234"><a href="#GitBetter-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-235"><a href="#GitBetter-235"><span class="linenos">235</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+</span><span id="GitBetter-233"><a href="#GitBetter-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-234"><a href="#GitBetter-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-235"><a href="#GitBetter-235"><span class="linenos">235</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
 </span><span id="GitBetter-236"><a href="#GitBetter-236"><span class="linenos">236</span></a>
-</span><span id="GitBetter-237"><a href="#GitBetter-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-238"><a href="#GitBetter-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-239"><a href="#GitBetter-239"><span class="linenos">239</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="GitBetter-237"><a href="#GitBetter-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-238"><a href="#GitBetter-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-239"><a href="#GitBetter-239"><span class="linenos">239</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span><span id="GitBetter-240"><a href="#GitBetter-240"><span class="linenos">240</span></a>
-</span><span id="GitBetter-241"><a href="#GitBetter-241"><span class="linenos">241</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter-242"><a href="#GitBetter-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-243"><a href="#GitBetter-243"><span class="linenos">243</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-244"><a href="#GitBetter-244"><span class="linenos">244</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
-</span><span id="GitBetter-245"><a href="#GitBetter-245"><span class="linenos">245</span></a>
-</span><span id="GitBetter-246"><a href="#GitBetter-246"><span class="linenos">246</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="GitBetter-247"><a href="#GitBetter-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter-248"><a href="#GitBetter-248"><span class="linenos">248</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-249"><a href="#GitBetter-249"><span class="linenos">249</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
-</span><span id="GitBetter-250"><a href="#GitBetter-250"><span class="linenos">250</span></a>
-</span><span id="GitBetter-251"><a href="#GitBetter-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-252"><a href="#GitBetter-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-253"><a href="#GitBetter-253"><span class="linenos">253</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+</span><span id="GitBetter-241"><a href="#GitBetter-241"><span class="linenos">241</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-242"><a href="#GitBetter-242"><span class="linenos">242</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-243"><a href="#GitBetter-243"><span class="linenos">243</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+</span><span id="GitBetter-244"><a href="#GitBetter-244"><span class="linenos">244</span></a>
+</span><span id="GitBetter-245"><a href="#GitBetter-245"><span class="linenos">245</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter-246"><a href="#GitBetter-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-247"><a href="#GitBetter-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-248"><a href="#GitBetter-248"><span class="linenos">248</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+</span><span id="GitBetter-249"><a href="#GitBetter-249"><span class="linenos">249</span></a>
+</span><span id="GitBetter-250"><a href="#GitBetter-250"><span class="linenos">250</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="GitBetter-251"><a href="#GitBetter-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter-252"><a href="#GitBetter-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-253"><a href="#GitBetter-253"><span class="linenos">253</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
 </span><span id="GitBetter-254"><a href="#GitBetter-254"><span class="linenos">254</span></a>
-</span><span id="GitBetter-255"><a href="#GitBetter-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-256"><a href="#GitBetter-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-257"><a href="#GitBetter-257"><span class="linenos">257</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="GitBetter-258"><a href="#GitBetter-258"><span class="linenos">258</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-259"><a href="#GitBetter-259"><span class="linenos">259</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter-260"><a href="#GitBetter-260"><span class="linenos">260</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
-</span><span id="GitBetter-261"><a href="#GitBetter-261"><span class="linenos">261</span></a>
-</span><span id="GitBetter-262"><a href="#GitBetter-262"><span class="linenos">262</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-263"><a href="#GitBetter-263"><span class="linenos">263</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="GitBetter-264"><a href="#GitBetter-264"><span class="linenos">264</span></a>
-</span><span id="GitBetter-265"><a href="#GitBetter-265"><span class="linenos">265</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter-266"><a href="#GitBetter-266"><span class="linenos">266</span></a>
-</span><span id="GitBetter-267"><a href="#GitBetter-267"><span class="linenos">267</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-268"><a href="#GitBetter-268"><span class="linenos">268</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="GitBetter-269"><a href="#GitBetter-269"><span class="linenos">269</span></a>
-</span><span id="GitBetter-270"><a href="#GitBetter-270"><span class="linenos">270</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-271"><a href="#GitBetter-271"><span class="linenos">271</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="GitBetter-272"><a href="#GitBetter-272"><span class="linenos">272</span></a>
-</span><span id="GitBetter-273"><a href="#GitBetter-273"><span class="linenos">273</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter-274"><a href="#GitBetter-274"><span class="linenos">274</span></a>
-</span><span id="GitBetter-275"><a href="#GitBetter-275"><span class="linenos">275</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-276"><a href="#GitBetter-276"><span class="linenos">276</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
-</span><span id="GitBetter-277"><a href="#GitBetter-277"><span class="linenos">277</span></a>
-</span><span id="GitBetter-278"><a href="#GitBetter-278"><span class="linenos">278</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter-279"><a href="#GitBetter-279"><span class="linenos">279</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="GitBetter-280"><a href="#GitBetter-280"><span class="linenos">280</span></a>
-</span><span id="GitBetter-281"><a href="#GitBetter-281"><span class="linenos">281</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter-282"><a href="#GitBetter-282"><span class="linenos">282</span></a>
-</span><span id="GitBetter-283"><a href="#GitBetter-283"><span class="linenos">283</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="GitBetter-255"><a href="#GitBetter-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-256"><a href="#GitBetter-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-257"><a href="#GitBetter-257"><span class="linenos">257</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+</span><span id="GitBetter-258"><a href="#GitBetter-258"><span class="linenos">258</span></a>
+</span><span id="GitBetter-259"><a href="#GitBetter-259"><span class="linenos">259</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-260"><a href="#GitBetter-260"><span class="linenos">260</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-261"><a href="#GitBetter-261"><span class="linenos">261</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="GitBetter-262"><a href="#GitBetter-262"><span class="linenos">262</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-263"><a href="#GitBetter-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter-264"><a href="#GitBetter-264"><span class="linenos">264</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+</span><span id="GitBetter-265"><a href="#GitBetter-265"><span class="linenos">265</span></a>
+</span><span id="GitBetter-266"><a href="#GitBetter-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-267"><a href="#GitBetter-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="GitBetter-268"><a href="#GitBetter-268"><span class="linenos">268</span></a>
+</span><span id="GitBetter-269"><a href="#GitBetter-269"><span class="linenos">269</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-270"><a href="#GitBetter-270"><span class="linenos">270</span></a>
+</span><span id="GitBetter-271"><a href="#GitBetter-271"><span class="linenos">271</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-272"><a href="#GitBetter-272"><span class="linenos">272</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-273"><a href="#GitBetter-273"><span class="linenos">273</span></a>
+</span><span id="GitBetter-274"><a href="#GitBetter-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-275"><a href="#GitBetter-275"><span class="linenos">275</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="GitBetter-276"><a href="#GitBetter-276"><span class="linenos">276</span></a>
+</span><span id="GitBetter-277"><a href="#GitBetter-277"><span class="linenos">277</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-278"><a href="#GitBetter-278"><span class="linenos">278</span></a>
+</span><span id="GitBetter-279"><a href="#GitBetter-279"><span class="linenos">279</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-280"><a href="#GitBetter-280"><span class="linenos">280</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-281"><a href="#GitBetter-281"><span class="linenos">281</span></a>
+</span><span id="GitBetter-282"><a href="#GitBetter-282"><span class="linenos">282</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter-283"><a href="#GitBetter-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
 </span><span id="GitBetter-284"><a href="#GitBetter-284"><span class="linenos">284</span></a>
-</span><span id="GitBetter-285"><a href="#GitBetter-285"><span class="linenos">285</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="GitBetter-286"><a href="#GitBetter-286"><span class="linenos">286</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter-285"><a href="#GitBetter-285"><span class="linenos">285</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter-286"><a href="#GitBetter-286"><span class="linenos">286</span></a>
+</span><span id="GitBetter-287"><a href="#GitBetter-287"><span class="linenos">287</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="GitBetter-288"><a href="#GitBetter-288"><span class="linenos">288</span></a>
+</span><span id="GitBetter-289"><a href="#GitBetter-289"><span class="linenos">289</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="GitBetter-290"><a href="#GitBetter-290"><span class="linenos">290</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>GitBetter Shell.</p>
 </div>
 
 
@@ -1363,28 +1374,50 @@
 
 
             <div class="docstring"><p>Execute <code>git --oneline --name-only --abbrev-commit --graph</code>.</p>
 </div>
 
 
                             </div>
+                            <div id="GitBetter.do_status" class="classattr">
+                                        <input id="GitBetter.do_status-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">do_status</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">_</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="GitBetter.do_status-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#GitBetter.do_status"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_status-233"><a href="#GitBetter.do_status-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_status</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">_</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_status-234"><a href="#GitBetter.do_status-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Execute `git status`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_status-235"><a href="#GitBetter.do_status-235"><span class="linenos">235</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">status</span><span class="p">()</span>
+</span></pre></div>
+
+
+            <div class="docstring"><p>Execute <code>git status</code>.</p>
+</div>
+
+
+                            </div>
                             <div id="GitBetter.do_merge" class="classattr">
                                         <input id="GitBetter.do_merge-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">do_merge</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_merge-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_merge"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_merge-233"><a href="#GitBetter.do_merge-233"><span class="linenos">233</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_merge-234"><a href="#GitBetter.do_merge-234"><span class="linenos">234</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_merge-235"><a href="#GitBetter.do_merge-235"><span class="linenos">235</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_merge-237"><a href="#GitBetter.do_merge-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_merge</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch_name</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_merge-238"><a href="#GitBetter.do_merge-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Merge supplied `branch_name` with the currently active branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_merge-239"><a href="#GitBetter.do_merge-239"><span class="linenos">239</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">merge</span><span class="p">(</span><span class="n">branch_name</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Merge supplied <code>branch_name</code> with the currently active branch.</p>
 </div>
 
 
@@ -1396,17 +1429,17 @@
         <span class="def">def</span>
         <span class="name">do_tag</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_tag-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_tag"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_tag-237"><a href="#GitBetter.do_tag-237"><span class="linenos">237</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_tag-238"><a href="#GitBetter.do_tag-238"><span class="linenos">238</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_tag-239"><a href="#GitBetter.do_tag-239"><span class="linenos">239</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_tag-241"><a href="#GitBetter.do_tag-241"><span class="linenos">241</span></a>    <span class="k">def</span> <span class="nf">do_tag</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">tag_id</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_tag-242"><a href="#GitBetter.do_tag-242"><span class="linenos">242</span></a>        <span class="sd">&quot;&quot;&quot;Tag current commit with `tag_id`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_tag-243"><a href="#GitBetter.do_tag-243"><span class="linenos">243</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">tag</span><span class="p">(</span><span class="n">tag_id</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Tag current commit with <code>tag_id</code>.</p>
 </div>
 
 
@@ -1419,18 +1452,18 @@
         <span class="def">def</span>
         <span class="name">do_amend</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_amend-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_amend"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_amend-241"><a href="#GitBetter.do_amend-241"><span class="linenos">241</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
-</span><span id="GitBetter.do_amend-242"><a href="#GitBetter.do_amend-242"><span class="linenos">242</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_amend-243"><a href="#GitBetter.do_amend-243"><span class="linenos">243</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_amend-244"><a href="#GitBetter.do_amend-244"><span class="linenos">244</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_amend-245"><a href="#GitBetter.do_amend-245"><span class="linenos">245</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">amend_files_parser</span><span class="p">,</span> <span class="p">[</span><span class="n">files_postparser</span><span class="p">])</span>
+</span><span id="GitBetter.do_amend-246"><a href="#GitBetter.do_amend-246"><span class="linenos">246</span></a>    <span class="k">def</span> <span class="nf">do_amend</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_amend-247"><a href="#GitBetter.do_amend-247"><span class="linenos">247</span></a>        <span class="sd">&quot;&quot;&quot;Stage files and add to previous commit.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_amend-248"><a href="#GitBetter.do_amend-248"><span class="linenos">248</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">amend</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">files</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Stage files and add to previous commit.</p>
 </div>
 
 
@@ -1443,18 +1476,18 @@
         <span class="def">def</span>
         <span class="name">do_delete_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argshell</span><span class="o">.</span><span class="n">argshell</span><span class="o">.</span><span class="n">Namespace</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_delete_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_delete_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_branch-246"><a href="#GitBetter.do_delete_branch-246"><span class="linenos">246</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
-</span><span id="GitBetter.do_delete_branch-247"><a href="#GitBetter.do_delete_branch-247"><span class="linenos">247</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
-</span><span id="GitBetter.do_delete_branch-248"><a href="#GitBetter.do_delete_branch-248"><span class="linenos">248</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_delete_branch-249"><a href="#GitBetter.do_delete_branch-249"><span class="linenos">249</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_branch-250"><a href="#GitBetter.do_delete_branch-250"><span class="linenos">250</span></a>    <span class="nd">@with_parser</span><span class="p">(</span><span class="n">delete_branch_parser</span><span class="p">)</span>
+</span><span id="GitBetter.do_delete_branch-251"><a href="#GitBetter.do_delete_branch-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_delete_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">args</span><span class="p">:</span> <span class="n">Namespace</span><span class="p">):</span>
+</span><span id="GitBetter.do_delete_branch-252"><a href="#GitBetter.do_delete_branch-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Delete branch.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_delete_branch-253"><a href="#GitBetter.do_delete_branch-253"><span class="linenos">253</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_branch</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">branch</span><span class="p">,</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">remote</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete branch.</p>
 </div>
 
 
@@ -1466,17 +1499,17 @@
         <span class="def">def</span>
         <span class="name">do_pull_branch</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">branch</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_pull_branch-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_pull_branch"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull_branch-251"><a href="#GitBetter.do_pull_branch-251"><span class="linenos">251</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_pull_branch-252"><a href="#GitBetter.do_pull_branch-252"><span class="linenos">252</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_pull_branch-253"><a href="#GitBetter.do_pull_branch-253"><span class="linenos">253</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_pull_branch-255"><a href="#GitBetter.do_pull_branch-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_pull_branch</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">branch</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_pull_branch-256"><a href="#GitBetter.do_pull_branch-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Pull this branch from the origin.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_pull_branch-257"><a href="#GitBetter.do_pull_branch-257"><span class="linenos">257</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">pull_branch</span><span class="p">(</span><span class="n">branch</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Pull this branch from the origin.</p>
 </div>
 
 
@@ -1488,20 +1521,20 @@
         <span class="def">def</span>
         <span class="name">do_ignore</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_ignore-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_ignore"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_ignore-255"><a href="#GitBetter.do_ignore-255"><span class="linenos">255</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_ignore-256"><a href="#GitBetter.do_ignore-256"><span class="linenos">256</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_ignore-257"><a href="#GitBetter.do_ignore-257"><span class="linenos">257</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
-</span><span id="GitBetter.do_ignore-258"><a href="#GitBetter.do_ignore-258"><span class="linenos">258</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
-</span><span id="GitBetter.do_ignore-259"><a href="#GitBetter.do_ignore-259"><span class="linenos">259</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="GitBetter.do_ignore-260"><a href="#GitBetter.do_ignore-260"><span class="linenos">260</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_ignore-259"><a href="#GitBetter.do_ignore-259"><span class="linenos">259</span></a>    <span class="k">def</span> <span class="nf">do_ignore</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">patterns</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_ignore-260"><a href="#GitBetter.do_ignore-260"><span class="linenos">260</span></a>        <span class="sd">&quot;&quot;&quot;Add the list of patterns to `.gitignore`.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_ignore-261"><a href="#GitBetter.do_ignore-261"><span class="linenos">261</span></a>        <span class="n">patterns</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">patterns</span><span class="o">.</span><span class="n">split</span><span class="p">())</span>
+</span><span id="GitBetter.do_ignore-262"><a href="#GitBetter.do_ignore-262"><span class="linenos">262</span></a>        <span class="n">path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="s2">&quot;.gitignore&quot;</span><span class="p">)</span>
+</span><span id="GitBetter.do_ignore-263"><a href="#GitBetter.do_ignore-263"><span class="linenos">263</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="GitBetter.do_ignore-264"><a href="#GitBetter.do_ignore-264"><span class="linenos">264</span></a>        <span class="n">path</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">patterns</span><span class="p">,</span> <span class="kc">False</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Add the list of patterns to <code>.gitignore</code>.</p>
 </div>
 
 
@@ -1513,21 +1546,21 @@
         <span class="def">def</span>
         <span class="name">do_make_private</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_make_private-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_make_private"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_private-262"><a href="#GitBetter.do_make_private-262"><span class="linenos">262</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_make_private-263"><a href="#GitBetter.do_make_private-263"><span class="linenos">263</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
-</span><span id="GitBetter.do_make_private-264"><a href="#GitBetter.do_make_private-264"><span class="linenos">264</span></a>
-</span><span id="GitBetter.do_make_private-265"><a href="#GitBetter.do_make_private-265"><span class="linenos">265</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_make_private-266"><a href="#GitBetter.do_make_private-266"><span class="linenos">266</span></a>
-</span><span id="GitBetter.do_make_private-267"><a href="#GitBetter.do_make_private-267"><span class="linenos">267</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_make_private-268"><a href="#GitBetter.do_make_private-268"><span class="linenos">268</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_private-266"><a href="#GitBetter.do_make_private-266"><span class="linenos">266</span></a>    <span class="k">def</span> <span class="nf">do_make_private</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_make_private-267"><a href="#GitBetter.do_make_private-267"><span class="linenos">267</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo private.</span>
+</span><span id="GitBetter.do_make_private-268"><a href="#GitBetter.do_make_private-268"><span class="linenos">268</span></a>
+</span><span id="GitBetter.do_make_private-269"><a href="#GitBetter.do_make_private-269"><span class="linenos">269</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_make_private-270"><a href="#GitBetter.do_make_private-270"><span class="linenos">270</span></a>
+</span><span id="GitBetter.do_make_private-271"><a href="#GitBetter.do_make_private-271"><span class="linenos">271</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_make_private-272"><a href="#GitBetter.do_make_private-272"><span class="linenos">272</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_private</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make the GitHub remote for this repo private.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1543,21 +1576,21 @@
         <span class="def">def</span>
         <span class="name">do_make_public</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_make_public-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_make_public"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_public-270"><a href="#GitBetter.do_make_public-270"><span class="linenos">270</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_make_public-271"><a href="#GitBetter.do_make_public-271"><span class="linenos">271</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
-</span><span id="GitBetter.do_make_public-272"><a href="#GitBetter.do_make_public-272"><span class="linenos">272</span></a>
-</span><span id="GitBetter.do_make_public-273"><a href="#GitBetter.do_make_public-273"><span class="linenos">273</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_make_public-274"><a href="#GitBetter.do_make_public-274"><span class="linenos">274</span></a>
-</span><span id="GitBetter.do_make_public-275"><a href="#GitBetter.do_make_public-275"><span class="linenos">275</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_make_public-276"><a href="#GitBetter.do_make_public-276"><span class="linenos">276</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_make_public-274"><a href="#GitBetter.do_make_public-274"><span class="linenos">274</span></a>    <span class="k">def</span> <span class="nf">do_make_public</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_make_public-275"><a href="#GitBetter.do_make_public-275"><span class="linenos">275</span></a>        <span class="sd">&quot;&quot;&quot;Make the GitHub remote for this repo public.</span>
+</span><span id="GitBetter.do_make_public-276"><a href="#GitBetter.do_make_public-276"><span class="linenos">276</span></a>
+</span><span id="GitBetter.do_make_public-277"><a href="#GitBetter.do_make_public-277"><span class="linenos">277</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_make_public-278"><a href="#GitBetter.do_make_public-278"><span class="linenos">278</span></a>
+</span><span id="GitBetter.do_make_public-279"><a href="#GitBetter.do_make_public-279"><span class="linenos">279</span></a><span class="sd">        This repo must exist and GitHub CLI must be installed and configured.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_make_public-280"><a href="#GitBetter.do_make_public-280"><span class="linenos">280</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">make_public</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Make the GitHub remote for this repo public.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1573,23 +1606,23 @@
         <span class="def">def</span>
         <span class="name">do_delete_gh_repo</span><span class="signature pdoc-code condensed">(<span class="param"><span class="bp">self</span>, </span><span class="param"><span class="n">owner</span><span class="p">:</span> <span class="nb">str</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="GitBetter.do_delete_gh_repo-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#GitBetter.do_delete_gh_repo"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_gh_repo-278"><a href="#GitBetter.do_delete_gh_repo-278"><span class="linenos">278</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
-</span><span id="GitBetter.do_delete_gh_repo-279"><a href="#GitBetter.do_delete_gh_repo-279"><span class="linenos">279</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
-</span><span id="GitBetter.do_delete_gh_repo-280"><a href="#GitBetter.do_delete_gh_repo-280"><span class="linenos">280</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-281"><a href="#GitBetter.do_delete_gh_repo-281"><span class="linenos">281</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
-</span><span id="GitBetter.do_delete_gh_repo-282"><a href="#GitBetter.do_delete_gh_repo-282"><span class="linenos">282</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-283"><a href="#GitBetter.do_delete_gh_repo-283"><span class="linenos">283</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="GitBetter.do_delete_gh_repo-282"><a href="#GitBetter.do_delete_gh_repo-282"><span class="linenos">282</span></a>    <span class="k">def</span> <span class="nf">do_delete_gh_repo</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">owner</span><span class="p">:</span> <span class="nb">str</span><span class="p">):</span>
+</span><span id="GitBetter.do_delete_gh_repo-283"><a href="#GitBetter.do_delete_gh_repo-283"><span class="linenos">283</span></a>        <span class="sd">&quot;&quot;&quot;Delete this repo from GitHub.</span>
 </span><span id="GitBetter.do_delete_gh_repo-284"><a href="#GitBetter.do_delete_gh_repo-284"><span class="linenos">284</span></a>
-</span><span id="GitBetter.do_delete_gh_repo-285"><a href="#GitBetter.do_delete_gh_repo-285"><span class="linenos">285</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
-</span><span id="GitBetter.do_delete_gh_repo-286"><a href="#GitBetter.do_delete_gh_repo-286"><span class="linenos">286</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
+</span><span id="GitBetter.do_delete_gh_repo-285"><a href="#GitBetter.do_delete_gh_repo-285"><span class="linenos">285</span></a><span class="sd">        Expects an argument for the repo owner, i.e. the `OWNER` in `github.com/{OWNER}/{repo-name}`</span>
+</span><span id="GitBetter.do_delete_gh_repo-286"><a href="#GitBetter.do_delete_gh_repo-286"><span class="linenos">286</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-287"><a href="#GitBetter.do_delete_gh_repo-287"><span class="linenos">287</span></a><span class="sd">        GitHub CLI must be installed and configured.</span>
+</span><span id="GitBetter.do_delete_gh_repo-288"><a href="#GitBetter.do_delete_gh_repo-288"><span class="linenos">288</span></a>
+</span><span id="GitBetter.do_delete_gh_repo-289"><a href="#GitBetter.do_delete_gh_repo-289"><span class="linenos">289</span></a><span class="sd">        May require you to reauthorize and rerun command.&quot;&quot;&quot;</span>
+</span><span id="GitBetter.do_delete_gh_repo-290"><a href="#GitBetter.do_delete_gh_repo-290"><span class="linenos">290</span></a>        <span class="n">git</span><span class="o">.</span><span class="n">delete_remote</span><span class="p">(</span><span class="n">owner</span><span class="p">,</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span><span class="o">.</span><span class="n">stem</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Delete this repo from GitHub.</p>
 
 <p>Expects an argument for the repo owner, i.e. the <code>OWNER</code> in <code>github.com/{OWNER}/{repo-name}</code></p>
 
@@ -1607,28 +1640,28 @@
                                 <dd id="GitBetter.__init__" class="function">Cmd</dd>
                 <dd id="GitBetter.precmd" class="function">precmd</dd>
                 <dd id="GitBetter.postcmd" class="function">postcmd</dd>
                 <dd id="GitBetter.preloop" class="function">preloop</dd>
                 <dd id="GitBetter.postloop" class="function">postloop</dd>
                 <dd id="GitBetter.parseline" class="function">parseline</dd>
                 <dd id="GitBetter.onecmd" class="function">onecmd</dd>
-                <dd id="GitBetter.emptyline" class="function">emptyline</dd>
                 <dd id="GitBetter.completedefault" class="function">completedefault</dd>
                 <dd id="GitBetter.completenames" class="function">completenames</dd>
                 <dd id="GitBetter.complete" class="function">complete</dd>
                 <dd id="GitBetter.get_names" class="function">get_names</dd>
                 <dd id="GitBetter.complete_help" class="function">complete_help</dd>
                 <dd id="GitBetter.print_topics" class="function">print_topics</dd>
                 <dd id="GitBetter.columnize" class="function">columnize</dd>
 
             </div>
             <div><dt>argshell.argshell.ArgShell</dt>
                                 <dd id="GitBetter.do_quit" class="function">do_quit</dd>
                 <dd id="GitBetter.do_sys" class="function">do_sys</dd>
                 <dd id="GitBetter.cmdloop" class="function">cmdloop</dd>
+                <dd id="GitBetter.emptyline" class="function">emptyline</dd>
 
             </div>
                                 </dl>
                             </div>
                 </section>
                 <section id="main">
                             <input id="main-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
@@ -1637,16 +1670,16 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-289"><a href="#main-289"><span class="linenos">289</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="main-290"><a href="#main-290"><span class="linenos">290</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-293"><a href="#main-293"><span class="linenos">293</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="main-294"><a href="#main-294"><span class="linenos">294</span></a>    <span class="n">GitBetter</span><span class="p">()</span><span class="o">.</span><span class="n">cmdloop</span><span class="p">()</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -27,14 +27,15 @@
           o do_switch
           o do_add_url
           o do_push_new
           o do_push
           o do_pull
           o do_list_branches
           o do_loggy
+          o do_status
           o do_merge
           o do_tag
           o do_amend
           o do_delete_branch
           o do_pull_branch
           o do_ignore
           o do_make_private
@@ -290,81 +291,85 @@
 225        """Show local and remote branches."""
 226        git.list_branches()
 227
 228    def do_loggy(self, _: str):
 229        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
 230        git.loggy()
 231
-232    def do_merge(self, branch_name: str):
-233        """Merge supplied `branch_name` with the currently active branch."""
-234        git.merge(branch_name)
+232    def do_status(self, _: str):
+233        """Execute `git status`."""
+234        git.status()
 235
-236    def do_tag(self, tag_id: str):
-237        """Tag current commit with `tag_id`."""
-238        git.tag(tag_id)
+236    def do_merge(self, branch_name: str):
+237        """Merge supplied `branch_name` with the currently active branch."""
+238        git.merge(branch_name)
 239
-240    @with_parser(amend_files_parser, [files_postparser])
-241    def do_amend(self, args: Namespace):
-242        """Stage files and add to previous commit."""
-243        git.amend(args.files)
-244
-245    @with_parser(delete_branch_parser)
-246    def do_delete_branch(self, args: Namespace):
-247        """Delete branch."""
-248        git.delete_branch(args.branch, not args.remote)
-249
-250    def do_pull_branch(self, branch: str):
-251        """Pull this branch from the origin."""
-252        git.pull_branch(branch)
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
 253
-254    def do_ignore(self, patterns: str):
-255        """Add the list of patterns to `.gitignore`."""
-256        patterns = "\n".join(patterns.split())
-257        path = Pathier(".gitignore")
-258        path.append("\n")
-259        path.append(patterns, False)
-260
-261    def do_make_private(self, owner: str):
-262        """Make the GitHub remote for this repo private.
-263
-264        Expects an argument for the repo owner, i.e. the `OWNER` in
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
-265
-266        This repo must exist and GitHub CLI must be installed and
+269
+270        This repo must exist and GitHub CLI must be installed and
 configured."""
-267        git.make_private(owner, Pathier.cwd().stem)
-268
-269    def do_make_public(self, owner: str):
-270        """Make the GitHub remote for this repo public.
-271
-272        Expects an argument for the repo owner, i.e. the `OWNER` in
+271        git.make_private(owner, Pathier.cwd().stem)
+272
+273    def do_make_public(self, owner: str):
+274        """Make the GitHub remote for this repo public.
+275
+276        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-273
-274        This repo must exist and GitHub CLI must be installed and
+277
+278        This repo must exist and GitHub CLI must be installed and
 configured."""
-275        git.make_public(owner, Pathier.cwd().stem)
-276
-277    def do_delete_gh_repo(self, owner: str):
-278        """Delete this repo from GitHub.
-279
-280        Expects an argument for the repo owner, i.e. the `OWNER` in
-`github.com/{OWNER}/{repo-name}`
-281
-282        GitHub CLI must be installed and configured.
+279        git.make_public(owner, Pathier.cwd().stem)
+280
+281    def do_delete_gh_repo(self, owner: str):
+282        """Delete this repo from GitHub.
 283
-284        May require you to reauthorize and rerun command."""
-285        git.delete_remote(owner, Pathier.cwd().stem)
-286
+284        Expects an argument for the repo owner, i.e. the `OWNER` in
+`github.com/{OWNER}/{repo-name}`
+285
+286        GitHub CLI must be installed and configured.
 287
-288def main():
-289    GitBetter().cmdloop()
+288        May require you to reauthorize and rerun command."""
+289        git.delete_remote(owner, Pathier.cwd().stem)
 290
 291
-292if __name__ == "__main__":
-293    main()
+292def main():
+293    GitBetter().cmdloop()
+294
+295
+296if __name__ == "__main__":
+297    main()
   ⁰
 def new_remote_parser() -> argshell.argshell.ArgShellParser: View Source
 10def new_remote_parser() -> ArgShellParser:
 11    parser = ArgShellParser()
 12    parser.add_argument(
 13        "--public",
 14        action="store_true",
@@ -601,73 +606,77 @@
 226        """Show local and remote branches."""
 227        git.list_branches()
 228
 229    def do_loggy(self, _: str):
 230        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
 231        git.loggy()
 232
-233    def do_merge(self, branch_name: str):
-234        """Merge supplied `branch_name` with the currently active branch."""
-235        git.merge(branch_name)
+233    def do_status(self, _: str):
+234        """Execute `git status`."""
+235        git.status()
 236
-237    def do_tag(self, tag_id: str):
-238        """Tag current commit with `tag_id`."""
-239        git.tag(tag_id)
+237    def do_merge(self, branch_name: str):
+238        """Merge supplied `branch_name` with the currently active branch."""
+239        git.merge(branch_name)
 240
-241    @with_parser(amend_files_parser, [files_postparser])
-242    def do_amend(self, args: Namespace):
-243        """Stage files and add to previous commit."""
-244        git.amend(args.files)
-245
-246    @with_parser(delete_branch_parser)
-247    def do_delete_branch(self, args: Namespace):
-248        """Delete branch."""
-249        git.delete_branch(args.branch, not args.remote)
-250
-251    def do_pull_branch(self, branch: str):
-252        """Pull this branch from the origin."""
-253        git.pull_branch(branch)
+241    def do_tag(self, tag_id: str):
+242        """Tag current commit with `tag_id`."""
+243        git.tag(tag_id)
+244
+245    @with_parser(amend_files_parser, [files_postparser])
+246    def do_amend(self, args: Namespace):
+247        """Stage files and add to previous commit."""
+248        git.amend(args.files)
+249
+250    @with_parser(delete_branch_parser)
+251    def do_delete_branch(self, args: Namespace):
+252        """Delete branch."""
+253        git.delete_branch(args.branch, not args.remote)
 254
-255    def do_ignore(self, patterns: str):
-256        """Add the list of patterns to `.gitignore`."""
-257        patterns = "\n".join(patterns.split())
-258        path = Pathier(".gitignore")
-259        path.append("\n")
-260        path.append(patterns, False)
-261
-262    def do_make_private(self, owner: str):
-263        """Make the GitHub remote for this repo private.
-264
-265        Expects an argument for the repo owner, i.e. the `OWNER` in
+255    def do_pull_branch(self, branch: str):
+256        """Pull this branch from the origin."""
+257        git.pull_branch(branch)
+258
+259    def do_ignore(self, patterns: str):
+260        """Add the list of patterns to `.gitignore`."""
+261        patterns = "\n".join(patterns.split())
+262        path = Pathier(".gitignore")
+263        path.append("\n")
+264        path.append(patterns, False)
+265
+266    def do_make_private(self, owner: str):
+267        """Make the GitHub remote for this repo private.
+268
+269        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-266
-267        This repo must exist and GitHub CLI must be installed and
+270
+271        This repo must exist and GitHub CLI must be installed and
 configured."""
-268        git.make_private(owner, Pathier.cwd().stem)
-269
-270    def do_make_public(self, owner: str):
-271        """Make the GitHub remote for this repo public.
-272
-273        Expects an argument for the repo owner, i.e. the `OWNER` in
+272        git.make_private(owner, Pathier.cwd().stem)
+273
+274    def do_make_public(self, owner: str):
+275        """Make the GitHub remote for this repo public.
+276
+277        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-274
-275        This repo must exist and GitHub CLI must be installed and
+278
+279        This repo must exist and GitHub CLI must be installed and
 configured."""
-276        git.make_public(owner, Pathier.cwd().stem)
-277
-278    def do_delete_gh_repo(self, owner: str):
-279        """Delete this repo from GitHub.
-280
-281        Expects an argument for the repo owner, i.e. the `OWNER` in
-`github.com/{OWNER}/{repo-name}`
-282
-283        GitHub CLI must be installed and configured.
+280        git.make_public(owner, Pathier.cwd().stem)
+281
+282    def do_delete_gh_repo(self, owner: str):
+283        """Delete this repo from GitHub.
 284
-285        May require you to reauthorize and rerun command."""
-286        git.delete_remote(owner, Pathier.cwd().stem)
+285        Expects an argument for the repo owner, i.e. the `OWNER` in
+`github.com/{OWNER}/{repo-name}`
+286
+287        GitHub CLI must be installed and configured.
+288
+289        May require you to reauthorize and rerun command."""
+290        git.delete_remote(owner, Pathier.cwd().stem)
 GitBetter Shell.
 ⁰
 def default(self, line: str): View Source
 107    def default(self, line: str):
 108        if self.execute_in_terminal_if_unrecognized:
 109            os.system(line)
 110        else:
@@ -845,102 +854,108 @@
 ⁰
 def do_loggy(self, _: str): View Source
 229    def do_loggy(self, _: str):
 230        """Execute `git --oneline --name-only --abbrev-commit --graph`."""
 231        git.loggy()
 Execute git --oneline --name-only --abbrev-commit --graph.
 ⁰
+def do_status(self, _: str): View Source
+233    def do_status(self, _: str):
+234        """Execute `git status`."""
+235        git.status()
+Execute git status.
+⁰
 def do_merge(self, branch_name: str): View Source
-233    def do_merge(self, branch_name: str):
-234        """Merge supplied `branch_name` with the currently active branch."""
-235        git.merge(branch_name)
+237    def do_merge(self, branch_name: str):
+238        """Merge supplied `branch_name` with the currently active branch."""
+239        git.merge(branch_name)
 Merge supplied branch_name with the currently active branch.
 ⁰
 def do_tag(self, tag_id: str): View Source
-237    def do_tag(self, tag_id: str):
-238        """Tag current commit with `tag_id`."""
-239        git.tag(tag_id)
+241    def do_tag(self, tag_id: str):
+242        """Tag current commit with `tag_id`."""
+243        git.tag(tag_id)
 Tag current commit with tag_id.
 ⁰
 @with_parser(amend_files_parser, [files_postparser])
 def do_amend(self, args: argshell.argshell.Namespace): View Source
-241    @with_parser(amend_files_parser, [files_postparser])
-242    def do_amend(self, args: Namespace):
-243        """Stage files and add to previous commit."""
-244        git.amend(args.files)
+245    @with_parser(amend_files_parser, [files_postparser])
+246    def do_amend(self, args: Namespace):
+247        """Stage files and add to previous commit."""
+248        git.amend(args.files)
 Stage files and add to previous commit.
 ⁰
 @with_parser(delete_branch_parser)
 def do_delete_branch(self, args: argshell.argshell.Namespace): View Source
-246    @with_parser(delete_branch_parser)
-247    def do_delete_branch(self, args: Namespace):
-248        """Delete branch."""
-249        git.delete_branch(args.branch, not args.remote)
+250    @with_parser(delete_branch_parser)
+251    def do_delete_branch(self, args: Namespace):
+252        """Delete branch."""
+253        git.delete_branch(args.branch, not args.remote)
 Delete branch.
 ⁰
 def do_pull_branch(self, branch: str): View Source
-251    def do_pull_branch(self, branch: str):
-252        """Pull this branch from the origin."""
-253        git.pull_branch(branch)
+255    def do_pull_branch(self, branch: str):
+256        """Pull this branch from the origin."""
+257        git.pull_branch(branch)
 Pull this branch from the origin.
 ⁰
 def do_ignore(self, patterns: str): View Source
-255    def do_ignore(self, patterns: str):
-256        """Add the list of patterns to `.gitignore`."""
-257        patterns = "\n".join(patterns.split())
-258        path = Pathier(".gitignore")
-259        path.append("\n")
-260        path.append(patterns, False)
+259    def do_ignore(self, patterns: str):
+260        """Add the list of patterns to `.gitignore`."""
+261        patterns = "\n".join(patterns.split())
+262        path = Pathier(".gitignore")
+263        path.append("\n")
+264        path.append(patterns, False)
 Add the list of patterns to .gitignore.
 ⁰
 def do_make_private(self, owner: str): View Source
-262    def do_make_private(self, owner: str):
-263        """Make the GitHub remote for this repo private.
-264
-265        Expects an argument for the repo owner, i.e. the `OWNER` in
+266    def do_make_private(self, owner: str):
+267        """Make the GitHub remote for this repo private.
+268
+269        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-266
-267        This repo must exist and GitHub CLI must be installed and
+270
+271        This repo must exist and GitHub CLI must be installed and
 configured."""
-268        git.make_private(owner, Pathier.cwd().stem)
+272        git.make_private(owner, Pathier.cwd().stem)
 Make the GitHub remote for this repo private.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 This repo must exist and GitHub CLI must be installed and configured.
 ⁰
 def do_make_public(self, owner: str): View Source
-270    def do_make_public(self, owner: str):
-271        """Make the GitHub remote for this repo public.
-272
-273        Expects an argument for the repo owner, i.e. the `OWNER` in
+274    def do_make_public(self, owner: str):
+275        """Make the GitHub remote for this repo public.
+276
+277        Expects an argument for the repo owner, i.e. the `OWNER` in
 `github.com/{OWNER}/{repo-name}`
-274
-275        This repo must exist and GitHub CLI must be installed and
+278
+279        This repo must exist and GitHub CLI must be installed and
 configured."""
-276        git.make_public(owner, Pathier.cwd().stem)
+280        git.make_public(owner, Pathier.cwd().stem)
 Make the GitHub remote for this repo public.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 This repo must exist and GitHub CLI must be installed and configured.
 ⁰
 def do_delete_gh_repo(self, owner: str): View Source
-278    def do_delete_gh_repo(self, owner: str):
-279        """Delete this repo from GitHub.
-280
-281        Expects an argument for the repo owner, i.e. the `OWNER` in
-`github.com/{OWNER}/{repo-name}`
-282
-283        GitHub CLI must be installed and configured.
+282    def do_delete_gh_repo(self, owner: str):
+283        """Delete this repo from GitHub.
 284
-285        May require you to reauthorize and rerun command."""
-286        git.delete_remote(owner, Pathier.cwd().stem)
+285        Expects an argument for the repo owner, i.e. the `OWNER` in
+`github.com/{OWNER}/{repo-name}`
+286
+287        GitHub CLI must be installed and configured.
+288
+289        May require you to reauthorize and rerun command."""
+290        git.delete_remote(owner, Pathier.cwd().stem)
 Delete this repo from GitHub.
 Expects an argument for the repo owner, i.e. the OWNER in github.com/{OWNER}/
 {repo-name}
 GitHub CLI must be installed and configured.
 May require you to reauthorize and rerun command.
 ** Inherited Members **
   ⁰
 def main(): View Source
-289def main():
-290    GitBetter().cmdloop()
+293def main():
+294    GitBetter().cmdloop()
```

### Comparing `gitbetter-0.3.0/src/gitbetter/git.py` & `gitbetter-0.4.0/src/gitbetter/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,19 @@
 
 
 def loggy():
     """Equivalent to `git log --oneline --name-only --abbrev-commit --graph`."""
     execute("log --oneline --name-only --abbrev-commit --graph")
 
 
+def status():
+    """Execute `git status`."""
+    execute("status")
+
+
 # ======================================Staging/Committing======================================
 def commit(args: str):
     """>>> git commit {args}"""
     execute(f"commit {args}")
 
 
 def add(files: list[str] | None = None):
```

### Comparing `gitbetter-0.3.0/src/gitbetter/gitbetter.py` & `gitbetter-0.4.0/src/gitbetter/gitbetter.py`

 * *Files 3% similar despite different names*

```diff
@@ -225,14 +225,18 @@
         """Show local and remote branches."""
         git.list_branches()
 
     def do_loggy(self, _: str):
         """Execute `git --oneline --name-only --abbrev-commit --graph`."""
         git.loggy()
 
+    def do_status(self, _: str):
+        """Execute `git status`."""
+        git.status()
+
     def do_merge(self, branch_name: str):
         """Merge supplied `branch_name` with the currently active branch."""
         git.merge(branch_name)
 
     def do_tag(self, tag_id: str):
         """Tag current commit with `tag_id`."""
         git.tag(tag_id)
```

### Comparing `gitbetter-0.3.0/LICENSE.txt` & `gitbetter-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gitbetter-0.3.0/README.md` & `gitbetter-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gitbetter-0.3.0/pyproject.toml` & `gitbetter-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 6c69 6e67 2e62 7569 6c64 220d 0a0d 0a5b  ling.build"....[
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6769 7462 6574 7465 7222 0d0a 6465   "gitbetter"..de
 00000070: 7363 7269 7074 696f 6e20 3d20 2243 7573  scription = "Cus
 00000080: 746f 6d20 6769 7420 7368 656c 6c20 746f  tom git shell to
 00000090: 2074 7970 6520 6c65 7373 2061 6e64 2063   type less and c
 000000a0: 6f6d 6d69 7420 6d6f 7265 2e22 0d0a 7665  ommit more."..ve
-000000b0: 7273 696f 6e20 3d20 2230 2e33 2e30 220d  rsion = "0.3.0".
+000000b0: 7273 696f 6e20 3d20 2230 2e34 2e30 220d  rsion = "0.4.0".
 000000c0: 0a72 6571 7569 7265 732d 7079 7468 6f6e  .requires-python
 000000d0: 203d 2022 3e3d 332e 3130 220d 0a64 6570   = ">=3.10"..dep
 000000e0: 656e 6465 6e63 6965 7320 3d20 5b22 6172  endencies = ["ar
 000000f0: 6773 6865 6c6c 222c 2022 7061 7468 6965  gshell", "pathie
 00000100: 7222 2c20 2270 7974 6573 7422 5d0d 0a72  r", "pytest"]..r
 00000110: 6561 646d 6520 3d20 2252 4541 444d 452e  eadme = "README.
 00000120: 6d64 220d 0a6b 6579 776f 7264 7320 3d20  md"..keywords =
```

### Comparing `gitbetter-0.3.0/PKG-INFO` & `gitbetter-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitbetter
-Version: 0.3.0
+Version: 0.4.0
 Summary: Custom git shell to type less and commit more.
 Project-URL: Homepage, https://github.com/matt-manes/gitbetter
 Project-URL: Documentation, https://github.com/matt-manes/gitbetter/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gitbetter/tree/main/src/gitbetter
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,commit,git,shell,terminal
```

