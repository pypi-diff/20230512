# Comparing `tmp/sphinx_lv2_theme-1.2.2.tar.gz` & `tmp/sphinx_lv2_theme-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_lv2_theme-1.2.2.tar", last modified: Sat Dec  3 22:29:18 2022, max compression
+gzip compressed data, was "sphinx_lv2_theme-1.4.0.tar", last modified: Fri May 12 03:22:33 2023, max compression
```

## Comparing `sphinx_lv2_theme-1.2.2.tar` & `sphinx_lv2_theme-1.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 drobilla  (1000) drobilla  (1000)        0 2022-12-03 22:29:18.646555 sphinx_lv2_theme-1.2.2/
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)      751 2022-07-10 19:14:34.000000 sphinx_lv2_theme-1.2.2/LICENSE
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)      129 2021-01-06 20:15:37.000000 sphinx_lv2_theme-1.2.2/MANIFEST.in
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)      670 2022-12-03 22:25:30.000000 sphinx_lv2_theme-1.2.2/NEWS
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)     5340 2022-12-03 22:29:18.646555 sphinx_lv2_theme-1.2.2/PKG-INFO
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)     4557 2021-01-06 20:05:51.000000 sphinx_lv2_theme-1.2.2/README.md
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)       38 2022-12-03 22:29:18.646555 sphinx_lv2_theme-1.2.2/setup.cfg
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)     1250 2022-12-03 22:26:07.000000 sphinx_lv2_theme-1.2.2/setup.py
-drwxr-xr-x   0 drobilla  (1000) drobilla  (1000)        0 2022-12-03 22:29:18.643221 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)      388 2022-12-03 22:26:07.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/__init__.py
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)     1123 2021-01-06 20:05:51.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/domainindex.html
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)     1440 2021-01-06 20:05:51.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/genindex.html
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)      254 2021-01-06 20:05:51.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/globaltoc.html
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)     7018 2021-01-06 23:15:36.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/layout.html
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)      179 2021-01-06 20:05:51.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/localtoc.html
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)       99 2021-01-06 20:05:51.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/page.html
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)      462 2022-12-03 21:32:51.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/search.html
-drwxr-xr-x   0 drobilla  (1000) drobilla  (1000)        0 2022-12-03 22:29:18.646555 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/static/
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)     5287 2022-12-03 21:37:37.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/static/pygments.css
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)    13295 2022-12-03 21:54:45.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/static/sphinx_lv2_theme.css_t
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)      425 2021-01-06 20:05:51.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/theme.conf
-drwxr-xr-x   0 drobilla  (1000) drobilla  (1000)        0 2022-12-03 22:29:18.646555 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme.egg-info/
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)     5340 2022-12-03 22:29:18.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme.egg-info/PKG-INFO
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)      639 2022-12-03 22:29:18.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme.egg-info/SOURCES.txt
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)        1 2022-12-03 22:29:18.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme.egg-info/dependency_links.txt
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)       57 2022-12-03 22:29:18.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme.egg-info/entry_points.txt
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)        7 2022-12-03 22:29:18.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme.egg-info/requires.txt
--rw-r--r--   0 drobilla  (1000) drobilla  (1000)       17 2022-12-03 22:29:18.000000 sphinx_lv2_theme-1.2.2/sphinx_lv2_theme.egg-info/top_level.txt
+drwxr-xr-x   0 drobilla  (1000) drobilla  (1000)        0 2023-05-12 03:22:33.934102 sphinx_lv2_theme-1.4.0/
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)      751 2023-05-05 22:05:57.000000 sphinx_lv2_theme-1.4.0/LICENSE
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)      129 2021-01-06 20:15:37.000000 sphinx_lv2_theme-1.4.0/MANIFEST.in
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)      920 2023-05-12 03:20:05.000000 sphinx_lv2_theme-1.4.0/NEWS
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)     5491 2023-05-12 03:22:33.934102 sphinx_lv2_theme-1.4.0/PKG-INFO
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)     4708 2023-05-12 03:15:41.000000 sphinx_lv2_theme-1.4.0/README.md
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)       38 2023-05-12 03:22:33.934102 sphinx_lv2_theme-1.4.0/setup.cfg
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)     1250 2023-05-12 03:20:13.000000 sphinx_lv2_theme-1.4.0/setup.py
+drwxr-xr-x   0 drobilla  (1000) drobilla  (1000)        0 2023-05-12 03:22:33.934102 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)      388 2023-05-12 03:20:18.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/__init__.py
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)     1123 2021-01-06 20:05:51.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/domainindex.html
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)     1671 2023-05-05 22:52:24.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/genindex.html
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)      254 2021-01-06 20:05:51.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/globaltoc.html
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)     6872 2023-05-12 02:00:31.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/layout.html
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)      179 2021-01-06 20:05:51.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/localtoc.html
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)       99 2021-01-06 20:05:51.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/page.html
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)      463 2023-05-05 22:40:05.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/search.html
+drwxr-xr-x   0 drobilla  (1000) drobilla  (1000)        0 2023-05-12 03:22:33.934102 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/static/
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)     6695 2023-05-10 20:26:01.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/static/pygments.css
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)    13339 2023-05-12 02:04:05.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/static/sphinx_lv2_theme.css_t
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)      449 2023-05-12 01:59:42.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/theme.conf
+drwxr-xr-x   0 drobilla  (1000) drobilla  (1000)        0 2023-05-12 03:22:33.934102 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme.egg-info/
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)     5491 2023-05-12 03:22:33.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme.egg-info/PKG-INFO
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)      639 2023-05-12 03:22:33.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)        1 2023-05-12 03:22:33.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)       57 2023-05-12 03:22:33.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme.egg-info/entry_points.txt
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)        7 2023-05-12 03:22:33.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme.egg-info/requires.txt
+-rw-r--r--   0 drobilla  (1000) drobilla  (1000)       17 2023-05-12 03:22:33.000000 sphinx_lv2_theme-1.4.0/sphinx_lv2_theme.egg-info/top_level.txt
```

### Comparing `sphinx_lv2_theme-1.2.2/LICENSE` & `sphinx_lv2_theme-1.4.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2020-2022 David Robillard <d@drobilla.net>
+Copyright 2020-2023 David Robillard <d@drobilla.net>
 
 Permission to use, copy, modify, and/or distribute this software for any
 purpose with or without fee is hereby granted, provided that the above
 copyright notice and this permission notice appear in all copies.
 
 THIS SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
 WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
```

### Comparing `sphinx_lv2_theme-1.2.2/NEWS` & `sphinx_lv2_theme-1.4.0/NEWS`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+sphinx_lv2_theme (1.4.0) stable; urgency=medium
+
+  * Add show_nav_version option
+  * Clean up HTML link tags
+  * Clean up whitespace in output
+  * Fix show_footer_version option
+
+ -- David Robillard <d@drobilla.net>  Fri, 12 May 2023 03:19:58 +0000
+
 sphinx_lv2_theme (1.2.2) stable; urgency=medium
 
   * Add missing style for unions and variables
   * Condense field headings
   * Fix double colons in fields
   * Fix syntax highlighting
   * Fix various minor CSS issues
```

### Comparing `sphinx_lv2_theme-1.2.2/PKG-INFO` & `sphinx_lv2_theme-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_lv2_theme
-Version: 1.2.2
+Version: 1.4.0
 Summary: A minimal static theme for Sphinx
 Home-page: https://gitlab.com/lv2/sphinx_lv2_theme
 Author: David Robillard
 Author-email: d@drobilla.net
 License: ISC
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
@@ -123,14 +123,18 @@
 : Boolean, default `true`.  If true then the project name and version is
   included in the footer.
 
 `show_logo_version`
 : Boolean, default `false`.  If true then the version is added to the logo
   text.
 
+`show_nav_version`
+: Boolean, default `true`.  If true then the version added to the root link on
+  the navigation bar.
+
 `sidebar_width`
 : CSS size, default `20em`.  The width of the sidebar.  This plus
   `body_max_width` should be less than `page_width`.
 
 Usage
 -----
 
@@ -151,14 +155,15 @@
     "logo": "myawesomeproject.svg",
     "logo_name": True,
     "logo_width": "8em",
     "nosidebar": False,
     "page_width": "80em",
     "show_footer_version": True,
     "show_logo_version": False,
+    "show_nav_version": True,
     "sidebar_width": "18em",
 }
 ```
 
  -- David Robillard <d@drobilla.net>
 
 [Sphinx]: https://www.sphinx-doc.org/
```

### Comparing `sphinx_lv2_theme-1.2.2/README.md` & `sphinx_lv2_theme-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,18 @@
 : Boolean, default `true`.  If true then the project name and version is
   included in the footer.
 
 `show_logo_version`
 : Boolean, default `false`.  If true then the version is added to the logo
   text.
 
+`show_nav_version`
+: Boolean, default `true`.  If true then the version added to the root link on
+  the navigation bar.
+
 `sidebar_width`
 : CSS size, default `20em`.  The width of the sidebar.  This plus
   `body_max_width` should be less than `page_width`.
 
 Usage
 -----
 
@@ -129,14 +133,15 @@
     "logo": "myawesomeproject.svg",
     "logo_name": True,
     "logo_width": "8em",
     "nosidebar": False,
     "page_width": "80em",
     "show_footer_version": True,
     "show_logo_version": False,
+    "show_nav_version": True,
     "sidebar_width": "18em",
 }
 ```
 
  -- David Robillard <d@drobilla.net>
 
 [Sphinx]: https://www.sphinx-doc.org/
```

### Comparing `sphinx_lv2_theme-1.2.2/setup.py` & `sphinx_lv2_theme-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="sphinx_lv2_theme",
-    version="1.2.2",
+    version="1.4.0",
     description="A minimal static theme for Sphinx",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     url="https://gitlab.com/lv2/sphinx_lv2_theme",
     author="David Robillard",
     author_email="d@drobilla.net",
     license="ISC",
```

### Comparing `sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/domainindex.html` & `sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/domainindex.html`

 * *Files identical despite different names*

### Comparing `sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/layout.html` & `sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/layout.html`

 * *Files 12% similar despite different names*

```diff
@@ -14,66 +14,62 @@
   {%- set titlesuffix = " &#8212; "|safe + docstitle|e -%}
 {%- else -%}
   {%- set titlesuffix = "" -%}
 {%- endif -%}
 
 {# Related navigation bar #}
 {%- macro relbar() -%}
-  <ul>
-    {%- if next -%}
-      <li class="right last">
-        <a href="{{ next.link|e }}">&rarr;</a>
-      </li>
+      <ul>
+    {%- if next %}
+        <li class="right last"><a href="{{ next.link|e }}">&rarr;</a></li>
     {%- endif -%}
 
-    {%- if prev -%}
-      <li class="right">
-        <a href="{{ prev.link|e }}">&larr;</a>
-      </li>
+    {%- if prev %}
+        <li class="right"><a href="{{ prev.link|e }}">&larr;</a></li>
     {%- endif -%}
 
-    {# Other related links #}
-    {# Note that "first" and "last" are flipped here because of the right float #}
+    {#- Other related links -#}
+    {#- Note that "first" and "last" are flipped here because of the right float -#}
     {%- set first = False -%}
     {%- for rellink in rellinks -%}
       {%- if
         not (prev and pathto(rellink[0]) == prev.link) and
-        not (next and pathto(rellink[0]) == next.link) -%}
-        <li class="right">
-          <a href="{{ pathto(rellink[0])|e }}"
-             title="{{ rellink[1]|striptags|e }}"
-             {{ accesskey(rellink[2]) }}>
-             {{ rellink[3] }}</a>
-        </li>
+        not (next and pathto(rellink[0]) == next.link) %}
+        <li class="right"><a href="{{ pathto(rellink[0])|e }}" title="{{ rellink[1]|striptags|e }}" {{ accesskey(rellink[2]) }}> {{ rellink[3] }}</a></li>
         {%- set first = True -%}
       {%- endif -%}
     {%- endfor -%}
 
-    {%- block rootrellink -%}
-      <li class="nav-item nav-item-0">
-        <a href="{{ pathto(master_doc)|e }}">
-          {{ shorttitle|e }}</a>
-      </li>
+    {%- block rootrellink %}
+        <li class="nav-item nav-item-0">
+          <a href="{{ pathto(master_doc)|e }}">
+            {{ shorttitle|e }}
+            {%- if theme_show_nav_version %}
+              {{ release }}
+            {%- endif %}
+          </a>
+        </li>
     {%- endblock -%}
 
     {%- for parent in parents -%}
       <li class="nav-item nav-item-{{ loop.index }}">
         {{ reldelim1 }}
         <a href="{{ parent.link|e }}" {% if loop.last %}{{ accesskey("U") }}{% endif %}>
           {{ parent.title }}
         </a>
       </li>
-    {%- endfor -%}
+    {%- endfor %}
 
-    <li class="nav-item nav-item-this">
-      {{ reldelim1 }}
-      <a href="{{ link|e }}">{{ title }}</a>
-    </li>
-    {%- block relbaritems %}{% endblock -%}
-  </ul>
+    {%- block thisrellink %}
+        <li class="nav-item nav-item-this">{{ reldelim1 }} <a href="{{ link|e }}">{{ title }}</a></li>
+    {%- endblock -%}
+    {%- block relbaritems -%}
+    {%- endblock -%}
+    {# #}
+      </ul>
 {%- endmacro -%}
 
 {# Sidebar #}
 {%- macro sidebar() -%}
   {%- if render_sidebar -%}
     <div class="sidebar" role="navigation" aria-label="main navigation">
       {%- block sidebarlogo -%}
@@ -101,22 +97,20 @@
       {%- endfor -%}
     </div>
   {%- endif -%}
 {%- endmacro -%}
 
 {# CSS links #}
 {%- macro css() -%}
-  <link rel="stylesheet" href="{{ pathto('_static/pygments.css', 1) }}" type="text/css" />
-  <link rel="stylesheet" href="{{ pathto('_static/' + style, 1)|e }}" type="text/css" />
   {%- for css in css_files -%}
-    {%- if css|attr("filename") -%}
-      {{ css_tag(css) }}
-    {%- else -%}
-      <link rel="stylesheet" href="{{ pathto(css, 1)|e }}" type="text/css" />
-    {%- endif -%}
+    {%- if css|attr("filename") %}
+    {{ css_tag(css) }}
+    {%- else %}
+    <link rel="stylesheet" href="{{ pathto(css, 1)|e }}" type="text/css" />
+    {% endif %}
   {%- endfor -%}
 {%- endmacro -%}
 
 {# HTML tag #}
 {%- if html_tag %}
   {{ html_tag }}
 {% else -%}
@@ -124,41 +118,41 @@
 {% endif -%}
 
 {# HTML head #}
 {%- block html_head %}
   <head>
     <meta charset="{{ encoding }}" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    {{- metatags }}
+    {{ metatags -}}
     {%- block htmltitle %}
-      <title>{{ title|striptags|e }}{{ titlesuffix }}</title>
+    <title>{{ title|striptags|e }}{{ titlesuffix }}</title>
     {%- endblock %}
     {%- block css %}
       {{- css() }}
     {%- endblock %}
     {%- if not embedded %}
       {%- if pageurl %}
-        <link rel="canonical" href="{{ pageurl|e }}" />
+    <link rel="canonical" href="{{ pageurl|e }}" />
       {%- endif %}
       {%- if favicon %}
-        <link rel="shortcut icon" href="{{ pathto('_static/' + favicon, 1)|e }}"/>
+    <link rel="shortcut icon" href="{{ pathto('_static/' + favicon, 1)|e }}"/>
       {%- endif %}
     {%- endif %}
     {%- block linktags %}
       {%- if hasdoc('about') %}
-        <link rel="author" title="{{ _('About these documents') }}" href="{{ pathto('about') }}" />
+    <link rel="author" title="{{ _('About these documents') }}" href="{{ pathto('about') }}" />
       {%- endif %}
       {%- if hasdoc('copyright') %}
-        <link rel="copyright" title="{{ _('Copyright') }}" href="{{ pathto('copyright') }}" />
+    <link rel="copyright" title="{{ _('Copyright') }}" href="{{ pathto('copyright') }}" />
       {%- endif %}
       {%- if next %}
-        <link rel="next" title="{{ next.title|striptags|e }}" href="{{ next.link|e }}" />
+    <link rel="next" title="{{ next.title|striptags|e }}" href="{{ next.link|e }}" />
       {%- endif %}
       {%- if prev %}
-        <link rel="prev" title="{{ prev.title|striptags|e }}" href="{{ prev.link|e }}" />
+    <link rel="prev" title="{{ prev.title|striptags|e }}" href="{{ prev.link|e }}" />
       {%- endif %}
     {%- endblock %}
     {%- block extrahead %}{% endblock %}
   </head>
 {% endblock -%}
 
 {# HTML body #}
@@ -167,76 +161,75 @@
 {% endblock %}
 
 {%- block header %}{% endblock %}
 
 {%- block content %}
   {%- if builder != "singlehtml" %}
     {%- block relbar1 %}
-      <div class="related topnav" role="navigation" aria-label="related navigation">
-        {{ relbar() }}
-      </div>
-    {% endblock %}
+    <div class="related topnav" role="navigation" aria-label="related navigation">
+      {{ relbar() }}
+    </div>
+    {%- endblock -%}
   {%- endif %}
 
-  {%- block sidebar1 %}
+  {%- block sidebar1 -%}
     {{ sidebar() }}
-  {% endblock %}
+  {%- endblock %}
 
-  <div class="document">
+    <div class="document">
     {%- block document %}
       <div class="documentwrapper">
         <div class="body" role="main">
-          {% block body %}{% endblock %}
-          <div class="clearer"></div>
+
+        {% block body -%}{%- endblock -%}
+        {# #}
         </div>
       </div>
     {%- endblock %}
-
-    <div class="clearer"></div>
-  </div>
+    </div>
 {%- endblock %}
 
-<div class="clearer"></div>
+    <div class="clearer"></div>
 
 {%- block footer %}
-  <div class="footer" role="contentinfo">
+    <div class="footer" role="contentinfo">
 
-    {%- if show_copyright %}
-      {%- if hasdoc('copyright') %}
-        {% trans path=pathto('copyright'), copyright=copyright|e %}
-          <a class="copyright" href="{{ path }}">Copyright</a> {{ copyright }}.
-        {% endtrans %}
-      {%- else %}
-        {% trans copyright=copyright|e %}
-          <span class="copyright">Copyright {{ copyright }}.</span>
-        {% endtrans %}
-      {%- endif %}
-    {%- endif %}
-    {%- if theme_display_version %}
+    {%- if show_copyright -%}
+      {%- if hasdoc('copyright') -%}
+        {%- trans path=pathto('copyright'), copyright=copyright|e %}
+      <a class="copyright" href="{{ path }}">Copyright</a> {{ copyright }}.
+        {%- endtrans -%}
+      {%- else -%}
+        {%- trans copyright=copyright|e %}
+      <span class="copyright">Copyright {{ copyright }}.</span>
+        {%- endtrans -%}
+      {%- endif -%}
+    {%- endif -%}
+    {%- if theme_show_footer_version %}
       <span class="meta">
         Generated for {{shorttitle|e}} {{ release }}
         {%- if show_sphinx %}
           using <a href="https://www.sphinx-doc.org/">Sphinx</a> {{ sphinx_version }}
         {%- endif %}.
       </span>
     {%- elif show_sphinx %}
       <span class="meta">
         Generated using
         <a href="https://www.sphinx-doc.org/">Sphinx</a> {{ sphinx_version }}.
       </span>
-    {%- endif %}
-
-  </div>
+    {%- endif -%}
+    {# #}
+    </div>
 {%- endblock %}
 
-<div class="clearer"></div>
+    <div class="clearer"></div>
 
 {%- if builder != "singlehtml" %}
   {%- block relbar2 %}
     <div class="related bottomnav" role="navigation" aria-label="related navigation">
       {{ relbar() }}
     </div>
-  {% endblock %}
+  {%- endblock -%}
 {%- endif %}
 
   </body>
   </html>
```

#### html2text {}

```diff
@@ -3,74 +3,73 @@
 reldelim1 is not defined and '»' or reldelim1 -%} {%- set reldelim2 = reldelim2
 is not defined and ',' or reldelim2 -%} {%- set render_sidebar = (not embedded)
 and (not theme_nosidebar|tobool) and (sidebars != []) -%} {%- set url_root =
 pathto('', 1) -%} {%- if url_root == '#' -%}{% set url_root = '' -%}{% endif -
 %} {%- if not embedded and docstitle -%} {%- set titlesuffix = " — "|safe +
 docstitle|e -%} {%- else -%} {%- set titlesuffix = "" -%} {%- endif -%} {#
 Related navigation bar #} {%- macro relbar() -%}
-    * {%- if next -%}
+    * {%- if next %}
     * →
-    * {%- endif -%} {%- if prev -%}
+    * {%- endif -%} {%- if prev %}
     * ←
-    * {%- endif -%} {# Other related links #} {# Note that "first" and "last"
-      are flipped here because of the right float #} {%- set first = False -%}
-      {%- for rellink in rellinks -%} {%- if not (prev and pathto(rellink[0])
-      == prev.link) and not (next and pathto(rellink[0]) == next.link) -%}
+    * {%- endif -%} {#- Other related links -#} {#- Note that "first" and
+      "last" are flipped here because of the right float -#} {%- set first =
+      False -%} {%- for rellink in rellinks -%} {%- if not (prev and pathto
+      (rellink[0]) == prev.link) and not (next and pathto(rellink[0]) ==
+      next.link) %}
     * { accesskey(rellink[2]) }}> {{ rellink[3] }}
-{%- set first = True -%} {%- endif -%} {%- endfor -%} {%- block rootrellink -%}
-{{_shorttitle|e_}}
+{%- set first = True -%} {%- endif -%} {%- endfor -%} {%- block rootrellink %}
+{{_shorttitle|e_}}_{%-_if_theme_show_nav_version_%}_{{_release_}}_{%-_endif_%}
 {%- endblock -%} {%- for parent in parents -%}
 {{ reldelim1 }}
 % if loop.last %}{{ accesskey("U") }}{% endif %}> {{ parent.title }}
-{%- endfor -%}
+{%- endfor %} {%- block thisrellink %}
 {{ reldelim1 }} {{_title_}}
-{%- block relbaritems %}{% endblock -%}
+{%- endblock -%} {%- block relbaritems -%} {%- endblock -%} {# #}
 {%- endmacro -%} {# Sidebar #} {%- macro sidebar() -%} {%- if render_sidebar -
 %}
 {%- block sidebarlogo -%} {%- if theme_logo -%}
 [Logo]
 {%- endif -%} {%- if theme_logo_name|lower == 'true' -%}
 {{ project }} {%- if theme_show_logo_version %} {{ release }} {%- endif %}
 {%- endif -%} {%- if theme_description -%}
 {{ theme_description }}
 {%- endif -%} {%- endblock -%} {%- for sidebartemplate in sidebars -%} {%-
 include sidebartemplate -%} {%- endfor -%}
-{%- endif -%} {%- endmacro -%} {# CSS links #} {%- macro css() -%}
-
- {%- for css in css_files -%} {%- if css|attr("filename") -%} {{ css_tag(css)
-}} {%- else -%}
- {%- endif -%} {%- endfor -%} {%- endmacro -%} {# HTML tag #} {%- if html_tag
-%} {{ html_tag }} {% else -%}
+{%- endif -%} {%- endmacro -%} {# CSS links #} {%- macro css() -%} {%- for css
+in css_files -%} {%- if css|attr("filename") %} {{ css_tag(css) }} {%- else %}
+ {% endif %} {%- endfor -%} {%- endmacro -%} {# HTML tag #} {%- if html_tag %}
+{{ html_tag }} {% else -%}
 % if language is not none %} lang="{{ language }}"{% endif %}> {% endif -%} {#
 HTML head #} {%- block html_head %}
 
- {{- metatags }} {%- block htmltitle %}
+ {{ metatags -}} {%- block htmltitle %}
 {%- endblock %} {%- block css %} {{- css() }} {%- endblock %} {%- if not
 embedded %} {%- if pageurl %}
  {%- endif %} {%- if favicon %}
  {%- endif %} {%- endif %} {%- block linktags %} {%- if hasdoc('about') %}
  {%- endif %} {%- if hasdoc('copyright') %}
  {%- endif %} {%- if next %}
  {%- endif %} {%- if prev %}
  {%- endif %} {%- endblock %} {%- block extrahead %}{% endblock %}
 {% endblock -%} {# HTML body #} {%- block body_tag %}
 {% endblock %} {%- block header %}{% endblock %} {%- block content %} {%- if
 builder != "singlehtml" %} {%- block relbar1 %}
 {{ relbar() }}
-{% endblock %} {%- endif %} {%- block sidebar1 %} {{ sidebar() }} {% endblock
-%}
+{%- endblock -%} {%- endif %} {%- block sidebar1 -%} {{ sidebar() }} {%-
+endblock %}
 {%- block document %}
-{% block body %}{% endblock %}
+{% block body -%}{%- endblock -%} {# #}
 {%- endblock %}
 {%- endblock %}
 {%- block footer %}
-{%- if show_copyright %} {%- if hasdoc('copyright') %} {% trans path=pathto
-('copyright'), copyright=copyright|e %} Copyright {{ copyright }}. {% endtrans
-%} {%- else %} {% trans copyright=copyright|e %} Copyright {{ copyright }}. {%
-endtrans %} {%- endif %} {%- endif %} {%- if theme_display_version %}
-Generated for {{shorttitle|e}} {{ release }} {%- if show_sphinx %} using Sphinx
-{{ sphinx_version }} {%- endif %}.  {%- elif show_sphinx %}  Generated using
-Sphinx {{ sphinx_version }}.  {%- endif %}
+{%- if show_copyright -%} {%- if hasdoc('copyright') -%} {%- trans path=pathto
+('copyright'), copyright=copyright|e %} Copyright {{ copyright }}. {%- endtrans
+-%} {%- else -%} {%- trans copyright=copyright|e %} Copyright {{ copyright }}.
+{%- endtrans -%} {%- endif -%} {%- endif -%} {%- if theme_show_footer_version
+%}  Generated for {{shorttitle|e}} {{ release }} {%- if show_sphinx %} using
+Sphinx {{ sphinx_version }} {%- endif %}.  {%- elif show_sphinx %}  Generated
+using Sphinx {{ sphinx_version }}.  {%- endif -%} {# #}
 {%- endblock %}
 {%- if builder != "singlehtml" %} {%- block relbar2 %}
 {{ relbar() }}
-{% endblock %} {%- endif %}
+{%- endblock -%} {%- endif %}
```

### Comparing `sphinx_lv2_theme-1.2.2/sphinx_lv2_theme/static/sphinx_lv2_theme.css_t` & `sphinx_lv2_theme-1.4.0/sphinx_lv2_theme/static/sphinx_lv2_theme.css_t`

 * *Files 3% similar despite different names*

```diff
@@ -178,25 +178,22 @@
   border-bottom: 1px solid #EEE;
   border-left: 1px solid #EEE;
   border-right: 1px solid #EEE;
   margin: 0;
 }
 
 .bottomnav {
-  border-left: 1px solid #EEE;
-  border-right: 1px solid #EEE;
   border-top-left-radius: 0.271em;
   border-top-right-radius: 0.271em;
-  border-top: 1px solid #EEE;
+  border: 1px solid #EEE;
   margin: 0.438em 0 0;
 }
 
 .related {
   background: #FAFAFA;
-  border: 1px solid #EEE;
   box-sizing: border-box;
   clear: both;
   font-size: 0.708em;
   line-height: 2.618em;
   width: 100%;
 }
 
@@ -543,23 +540,31 @@
 .method > dt:first-of-type,
 .struct > dt:first-of-type,
 .type > dt:first-of-type,
 .union > dt:first-of-type,
 .var > dt:first-of-type {
   font-family: "SF Mono", Menlo, Consolas, "DejaVu Sans Mono", monospace, fixed;
   font-size: 1.146em;
+}
+
+span.sig-name,
+span.desc-name, {
   font-weight: 600;
 }
 
+.highlight span.k {
+  color: #586E75;
+}
+
 section > dl, .section > dl {
-  margin-top: 2.618em;
+  margin-top: 3em;
 }
 
 dl.method {
-  margin-top: 1.146em;
+  margin-top: 1.618em;
 }
 
 .struct > dd > dl.member > dt,
 .enum > dd > dl.member > dt,
 .enum-class > dd > dl.member > dt {
   padding: 0.382em 0 0;
 }
@@ -606,15 +611,15 @@
 @media screen {
   a {
     color: #546E00;
   }
 }
 
 /* Squash as much as reasonable on super narrow screens like mobile */
-@media (max-width: {{ theme_body_min_width|todim }}) {
+@media (width <= {{ theme_body_min_width|todim }}) {
   div.logo, .logo-name, .description, .sidebarlogo {
     display: none;
   }
 
   .sidebar {
     border-top-left-radius: 0;
     border-top-right-radius: 0;
@@ -638,15 +643,15 @@
 
   .highlight-c, .highlight-cpp, .highlight-py {
     font-size: 0.708em;
   }
 }
 
 /* Make the sidebar a topbar on narrow screens */
-@media (min-width: {{ theme_body_min_width|todim }}) and (max-width: {{ theme_page_width|todim }}) {
+@media (width >= {{ theme_body_min_width|todim }}) and (width <= {{ theme_page_width|todim }}) {
   div.logo, .logo-name, .description, .sidebarlogo {
     display: none;
   }
 
   .sidebar {
     border-top-left-radius: 0;
     border-top-right-radius: 0;
@@ -666,15 +671,15 @@
     max-width: none;
     min-width: unset;
     padding: 0 1.854em;
   }
 }
 
 /* Sidebar on wide screens */
-@media (min-width: {{ theme_page_width|todim }}) {
+@media (width >= {{ theme_page_width|todim }}) {
   .sidebar {
     clear: left;
     float: left;
     margin: 1em 3em 1em 0;
     width: {{ theme_sidebar_width|todim }};
   }
 
@@ -768,21 +773,24 @@
     background-color: #282828;
   }
 
   td, th {
     border: 1px solid #383838;
   }
 
+  .topnav, .bottomnav {
+    border-color: #333;
+  }
+
   .related {
     background: #1A1A1A;
-    border: 1px solid #333;
   }
 
   .related ul {
-    color: #444;
+    color: #666;
   }
 
   .related .right {
     border-bottom: 1px solid #333;
     border-left: 1px solid #333;
   }
 
@@ -814,14 +822,19 @@
     color: #444;
   }
 
   .function em.property,
   .method em.property {
     color: #999;
   }
+
+  span.k,
+  span.kt {
+    color: #93A1A1;
+  }
 }
 
 /* Hard black for dark mode on mobile (since it's likely to be an OLED screen) */
 @media only screen and (hover: none) and (pointer: coarse) and (prefers-color-scheme: dark) {
   html {
     background: #000;
     color: #CCC;
```

### Comparing `sphinx_lv2_theme-1.2.2/sphinx_lv2_theme.egg-info/PKG-INFO` & `sphinx_lv2_theme-1.4.0/sphinx_lv2_theme.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-lv2-theme
-Version: 1.2.2
+Version: 1.4.0
 Summary: A minimal static theme for Sphinx
 Home-page: https://gitlab.com/lv2/sphinx_lv2_theme
 Author: David Robillard
 Author-email: d@drobilla.net
 License: ISC
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
@@ -123,14 +123,18 @@
 : Boolean, default `true`.  If true then the project name and version is
   included in the footer.
 
 `show_logo_version`
 : Boolean, default `false`.  If true then the version is added to the logo
   text.
 
+`show_nav_version`
+: Boolean, default `true`.  If true then the version added to the root link on
+  the navigation bar.
+
 `sidebar_width`
 : CSS size, default `20em`.  The width of the sidebar.  This plus
   `body_max_width` should be less than `page_width`.
 
 Usage
 -----
 
@@ -151,14 +155,15 @@
     "logo": "myawesomeproject.svg",
     "logo_name": True,
     "logo_width": "8em",
     "nosidebar": False,
     "page_width": "80em",
     "show_footer_version": True,
     "show_logo_version": False,
+    "show_nav_version": True,
     "sidebar_width": "18em",
 }
 ```
 
  -- David Robillard <d@drobilla.net>
 
 [Sphinx]: https://www.sphinx-doc.org/
```

### Comparing `sphinx_lv2_theme-1.2.2/sphinx_lv2_theme.egg-info/SOURCES.txt` & `sphinx_lv2_theme-1.4.0/sphinx_lv2_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

