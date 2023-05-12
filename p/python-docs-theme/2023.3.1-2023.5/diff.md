# Comparing `tmp/python-docs-theme-2023.3.1.tar.gz` & `tmp/python-docs-theme-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-docs-theme-2023.3.1.tar", last modified: Mon Mar 13 10:58:02 2023, max compression
+gzip compressed data, was "python-docs-theme-2023.5.tar", last modified: Fri May 12 15:44:48 2023, max compression
```

## Comparing `python-docs-theme-2023.3.1.tar` & `python-docs-theme-2023.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0      858 2021-04-12 15:38:41.686720 python-docs-theme-2023.3.1/README.rst
--rw-r--r--   0        0        0     1481 2023-03-13 10:34:44.276018 python-docs-theme-2023.3.1/pyproject.toml
--rw-r--r--   0        0        0     1790 2023-03-13 10:33:15.343954 python-docs-theme-2023.3.1/python_docs_theme/__init__.py
--rw-r--r--   0        0        0      184 2020-01-14 19:47:11.946027 python-docs-theme-2023.3.1/python_docs_theme/footerdonate.html
--rw-r--r--   0        0        0     6726 2023-03-10 08:32:16.256459 python-docs-theme-2023.3.1/python_docs_theme/layout.html
--rw-r--r--   0        0        0      245 2021-05-10 07:47:02.636520 python-docs-theme-2023.3.1/python_docs_theme/static/caret-down.svg
--rw-r--r--   0        0        0     2868 2021-04-12 15:38:45.486683 python-docs-theme-2023.3.1/python_docs_theme/static/copybutton.js
--rw-r--r--   0        0        0     2132 2021-05-10 07:47:02.636520 python-docs-theme-2023.3.1/python_docs_theme/static/menu.js
--rw-r--r--   0        0        0      695 2020-01-14 19:47:11.946027 python-docs-theme-2023.3.1/python_docs_theme/static/py.png
--rw-r--r--   0        0        0     2041 2021-05-10 07:47:02.636520 python-docs-theme-2023.3.1/python_docs_theme/static/py.svg
--rw-r--r--   0        0        0    11058 2023-03-10 08:32:16.260459 python-docs-theme-2023.3.1/python_docs_theme/static/pydoctheme.css
--rw-r--r--   0        0        0     4353 2023-03-10 08:32:16.260459 python-docs-theme-2023.3.1/python_docs_theme/static/sidebar.js
--rw-r--r--   0        0        0      721 2023-03-10 08:32:16.260459 python-docs-theme-2023.3.1/python_docs_theme/theme.conf
--rw-r--r--   0        0        0     2024 1970-01-01 00:00:00.000000 python-docs-theme-2023.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2460 2020-01-14 19:47:11.942027 python-docs-theme-2023.5/LICENSE
+-rw-r--r--   0        0        0      858 2021-04-12 15:38:41.686720 python-docs-theme-2023.5/README.rst
+-rw-r--r--   0        0        0     1479 2023-05-12 15:09:09.313631 python-docs-theme-2023.5/pyproject.toml
+-rw-r--r--   0        0        0     1781 2023-04-17 09:18:59.310725 python-docs-theme-2023.5/python_docs_theme/__init__.py
+-rw-r--r--   0        0        0      184 2020-01-14 19:47:11.946027 python-docs-theme-2023.5/python_docs_theme/footerdonate.html
+-rw-r--r--   0        0        0     7465 2023-04-17 09:18:59.314725 python-docs-theme-2023.5/python_docs_theme/layout.html
+-rw-r--r--   0        0        0     3508 2023-04-17 09:18:59.314725 python-docs-theme-2023.5/python_docs_theme/static/copybutton.js
+-rw-r--r--   0        0        0     2136 2023-04-17 09:18:59.314725 python-docs-theme-2023.5/python_docs_theme/static/menu.js
+-rw-r--r--   0        0        0      695 2020-01-14 19:47:11.946027 python-docs-theme-2023.5/python_docs_theme/static/py.png
+-rw-r--r--   0        0        0     2041 2021-05-10 07:47:02.636520 python-docs-theme-2023.5/python_docs_theme/static/py.svg
+-rw-r--r--   0        0        0    10971 2023-05-12 15:09:09.321631 python-docs-theme-2023.5/python_docs_theme/static/pydoctheme.css
+-rw-r--r--   0        0        0     1889 2023-05-12 15:09:09.321631 python-docs-theme-2023.5/python_docs_theme/static/pydoctheme_dark.css
+-rw-r--r--   0        0        0     3350 2023-05-12 15:09:09.321631 python-docs-theme-2023.5/python_docs_theme/static/sidebar.js_t
+-rw-r--r--   0        0        0      779 2023-04-17 09:18:59.314725 python-docs-theme-2023.5/python_docs_theme/static/themetoggle.js
+-rw-r--r--   0        0        0      777 2023-04-17 09:18:59.314725 python-docs-theme-2023.5/python_docs_theme/theme.conf
+-rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 python-docs-theme-2023.5/PKG-INFO
```

### Comparing `python-docs-theme-2023.3.1/README.rst` & `python-docs-theme-2023.5/README.rst`

 * *Files identical despite different names*

### Comparing `python-docs-theme-2023.3.1/pyproject.toml` & `python-docs-theme-2023.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["flit_core>=3.7"]
 build-backend = "flit_core.buildapi"
 
 # project metadata
 [project]
 name = "python-docs-theme"
-version = "2023.3.1"
+version = "2023.5"
 description = "The Sphinx theme for the CPython docs and related projects"
 readme = "README.rst"
 urls.Code = "https://github.com/python/python-docs-theme"
 urls.Download = "https://pypi.org/project/python-docs-theme/"
 urls.Homepage = "https://github.com/python/python-docs-theme/"
 urls."Issue tracker" = "https://github.com/python/python-docs-theme/issues"
-license.text = "PSF-2.0"
+license.file = "LICENSE"
 requires-python = ">=3.8"
 
 # Classifiers list: https://pypi.org/classifiers/
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Sphinx :: Theme",
     "Intended Audience :: Developers",
```

### Comparing `python-docs-theme-2023.3.1/python_docs_theme/__init__.py` & `python-docs-theme-2023.5/python_docs_theme/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,16 +48,15 @@
             context["css_files"],
             ["_static/pydoctheme.css"],
         )
 
 
 def setup(app):
     current_dir = os.path.abspath(os.path.dirname(__file__))
-    app.add_html_theme(
-        'python_docs_theme', current_dir)
+    app.add_html_theme("python_docs_theme", current_dir)
 
     app.connect("html-page-context", _html_page_context)
 
     return {
-        'parallel_read_safe': True,
-        'parallel_write_safe': True,
+        "parallel_read_safe": True,
+        "parallel_write_safe": True,
     }
```

### Comparing `python-docs-theme-2023.3.1/python_docs_theme/layout.html` & `python-docs-theme-2023.5/python_docs_theme/layout.html`

 * *Files 10% similar despite different names*

```diff
@@ -33,43 +33,54 @@
             {% block relbaritems %}
             {%- if pagename != "search" and builder != "singlehtml" and builder != "htmlhelp" %}
                 <li class="right">
                     {{ searchbox() }}
                     {{ reldelim2 }}
                 </li>
             {%- endif %}
+            <li class="right">{{ themeselector() }}{{ reldelim2 }}</li>
             {% endblock %}
       </ul>
     </div>
 {%- endmacro %}
 
 {%- macro searchbox() %}
 {# modified from sphinx/themes/basic/searchbox.html #}
     {%- if builder != "htmlhelp" %}
     <div class="inline-search" role="search">
         <form class="inline-search" action="{{ pathto('search') }}" method="get">
-          <input placeholder="{{ _('Quick search') }}" aria-label="{{ _('Quick search') }}" type="text" name="q" />
+          <input placeholder="{{ _('Quick search') }}" aria-label="{{ _('Quick search') }}" type="search" name="q" />
           <input type="submit" value="{{ _('Go') }}" />
-          <input type="hidden" name="check_keywords" value="yes" />
-          <input type="hidden" name="area" value="default" />
         </form>
     </div>
     {%- endif %}
 {%- endmacro %}
 
+{%- macro themeselector() %}
+<label class="theme-selector-label">
+    {{ _('Theme') }}
+    <select class="theme-selector" oninput="activateTheme(this.value)">
+        <option value="auto" selected>{{ _('Auto') }}</option>
+        <option value="light">{{ _('Light') }}</option>
+        <option value="dark">{{ _('Dark') }}</option>
+    </select>
+</label>
+{%- endmacro %}
+
 {% block relbar1 %} {% if builder != 'qthelp' %} {{ relbar() }} {% endif %} {% endblock %}
 {% block relbar2 %} {% if builder != 'qthelp' %} {{ relbar() }} {% endif %} {% endblock %}
 
-
 {%- block extrahead -%}
+    <link rel="stylesheet" href="{{ pathto('_static/pydoctheme_dark.css', 1) }}" media="(prefers-color-scheme: dark)" id="pydoctheme_dark_css">
     <link rel="shortcut icon" type="image/png" href="{{ pathto('_static/' + theme_root_icon, 1) }}" />
     {%- if builder != "htmlhelp" %}
         {%- if not embedded %}
             <script type="text/javascript" src="{{ pathto('_static/copybutton.js', 1) }}"></script>
             <script type="text/javascript" src="{{ pathto('_static/menu.js', 1) }}"></script>
+            <script type="text/javascript" src="{{ pathto('_static/themetoggle.js', 1) }}"></script>
         {%- endif -%}
     {%- endif -%}
     {{ super() }}
 {%- endblock -%}
 
 {%- block css -%}
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
@@ -78,36 +89,38 @@
 
 {%- block body_tag %}
 {{ super() }}
 {%- if builder != 'htmlhelp' %}
 <div class="mobile-nav">
     <input type="checkbox" id="menuToggler" class="toggler__input" aria-controls="navigation"
            aria-pressed="false" aria-expanded="false" role="button" aria-label="{{ _('Menu')}}" />
-    <label for="menuToggler" class="toggler__label">
-        <span></span>
-    </label>
     <nav class="nav-content" role="navigation">
-         <a href="{{ theme_root_url }}" class="nav-logo">
-             <img src="{{ pathto('_static/py.svg', 1) }}" alt="Logo"/>
-         </a>
-        <div class="version_switcher_placeholder"></div>
-        {%- if pagename != "search" and builder != "singlehtml" %}
-        <form role="search" class="search" action="{{ pathto('search') }}" method="get">
-            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" class="search-icon">
-                <path fill-rule="nonzero"
-                        d="M15.5 14h-.79l-.28-.27a6.5 6.5 0 001.48-5.34c-.47-2.78-2.79-5-5.59-5.34a6.505 6.505 0 00-7.27 7.27c.34 2.8 2.56 5.12 5.34 5.59a6.5 6.5 0 005.34-1.48l.27.28v.79l4.25 4.25c.41.41 1.08.41 1.49 0 .41-.41.41-1.08 0-1.49L15.5 14zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z" fill="#444"></path>
-            </svg>
-            <input type="text" name="q" aria-label="{{ _('Quick search') }}"/>
-            <input type="submit" value="{{ _('Go') }}"/>
-        </form>
-        {%- endif %}
+        <label for="menuToggler" class="toggler__label">
+            <span></span>
+        </label>
+        <span class="nav-items-wrapper">
+            <a href="{{ theme_root_url }}" class="nav-logo">
+                <img src="{{ pathto('_static/py.svg', 1) }}" alt="Logo"/>
+            </a>
+            <span class="version_switcher_placeholder"></span>
+            {%- if pagename != "search" and builder != "singlehtml" %}
+            <form role="search" class="search" action="{{ pathto('search') }}" method="get">
+                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" class="search-icon">
+                    <path fill-rule="nonzero" fill="currentColor" d="M15.5 14h-.79l-.28-.27a6.5 6.5 0 001.48-5.34c-.47-2.78-2.79-5-5.59-5.34a6.505 6.505 0 00-7.27 7.27c.34 2.8 2.56 5.12 5.34 5.59a6.5 6.5 0 005.34-1.48l.27.28v.79l4.25 4.25c.41.41 1.08.41 1.49 0 .41-.41.41-1.08 0-1.49L15.5 14zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"></path>
+                </svg>
+                <input placeholder="{{ _('Quick search') }}" aria-label="{{ _('Quick search') }}" type="search" name="q" />
+                <input type="submit" value="{{ _('Go') }}"/>
+            </form>
+            {%- endif %}
+        </span>
     </nav>
     <div class="menu-wrapper">
         <nav class="menu" role="navigation" aria-label="main navigation">
             <div class="language_switcher_placeholder"></div>
+            {{ themeselector() }}
             {%- if logo %}
             <p class="logo">
                 <a href="{{ pathto('index') }}">
                 <img class="logo" src="{{ pathto('_static/' + logo, 1)|e }}" alt="Logo"/>
                 </a>
             </p>
             {%- endif %}
```

#### html2text {}

```diff
@@ -13,30 +13,34 @@
 % if loop.last %}{{ accesskey("U") }}{% endif %}>{{ parent.title }}
 {{ reldelim1 }}
 {%- endfor %}
 {{_title_}}
 {% block relbaritems %} {%- if pagename != "search" and builder != "singlehtml"
 and builder != "htmlhelp" %}
 {{ searchbox() }} {{ reldelim2 }}
-{%- endif %} {% endblock %}
+{%- endif %}
+{{ themeselector() }}{{ reldelim2 }}
+{% endblock %}
 {%- endmacro %} {%- macro searchbox() %} {# modified from sphinx/themes/basic/
 searchbox.html #} {%- if builder != "htmlhelp" %}
-[q                   ] [{{ _('Go') }}]
-{%- endif %} {%- endmacro %} {% block relbar1 %} {% if builder != 'qthelp' %} {
-{ relbar() }} {% endif %} {% endblock %} {% block relbar2 %} {% if builder !=
-'qthelp' %} {{ relbar() }} {% endif %} {% endblock %} {%- block extrahead -%}
+[Unknown INPUT type] [{{ _('Go') }}]
+{%- endif %} {%- endmacro %} {%- macro themeselector() %}  {{ _('Theme') }}
+[One of: {{ _('Auto') }}/{{ _('Light') }}/{{ _('Dark') }}]  {%- endmacro %} {%
+block relbar1 %} {% if builder != 'qthelp' %} {{ relbar() }} {% endif %} {%
+endblock %} {% block relbar2 %} {% if builder != 'qthelp' %} {{ relbar() }} {%
+endif %} {% endblock %} {%- block extrahead -%}
+
  {%- if builder != "htmlhelp" %} {%- if not embedded %}
  {%- endif -%} {%- endif -%} {{ super() }} {%- endblock -%} {%- block css -%}
  {{ super() }} {%- endblock -%} {%- block body_tag %} {{ super() }} {%- if
 builder != 'htmlhelp' %}
-⁰     [Logo]
-{%- if pagename != "search" and builder != "singlehtml" %}
-   [q                   ] [{{ _('Go') }}]
+⁰      [Logo]  {%- if pagename != "search" and builder != "singlehtml" %}
+   [Unknown INPUT type] [{{ _('Go') }}]
 {%- endif %}
-{%- if logo %}
+{{ themeselector() }} {%- if logo %}
 [Logo]
 {%- endif %} {%- for sidebartemplate in sidebars %} {%- include sidebartemplate
 %} {%- endfor %}
 {% endif -%} {% endblock %} {% block footer %}
 © {% if theme_copyright_url or hasdoc('copyright') %}{%_endif_%}{%_trans
 %}Copyright{%_endtrans_%}{%_if_theme_copyright_url_or_hasdoc('copyright')_%}{%
 endif %} {{ copyright|e }}.
```

### Comparing `python-docs-theme-2023.3.1/python_docs_theme/static/menu.js` & `python-docs-theme-2023.5/python_docs_theme/static/menu.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,56 +1,58 @@
-document.addEventListener('DOMContentLoaded', function() {
+document.addEventListener("DOMContentLoaded", function() {
 
     // Make tables responsive by wrapping them in a div and making them scrollable
-    const tables = document.querySelectorAll('table.docutils');
+    const tables = document.querySelectorAll("table.docutils")
     tables.forEach(function(table) {
-        table.outerHTML = '<div class="responsive-table__container">' + table.outerHTML + '</div>'
-    });
+        table.outerHTML = '<div class="responsive-table__container">' + table.outerHTML + "</div>"
+    })
 
-    const togglerInput = document.querySelector('.toggler__input');
-    const togglerLabel = document.querySelector('.toggler__label');
-    const sideMenu = document.querySelector('.menu-wrapper');
-    const menuItems = document.querySelectorAll('.menu')
-    const doc = document.querySelector('.document');
-    const body = document.querySelector('body');
+    const togglerInput = document.querySelector(".toggler__input")
+    const togglerLabel = document.querySelector(".toggler__label")
+    const sideMenu = document.querySelector(".menu-wrapper")
+    const menuItems = document.querySelectorAll(".menu")
+    const doc = document.querySelector(".document")
+    const body = document.querySelector("body")
 
     function closeMenu() {
-        togglerInput.checked = false;
-        sideMenu.setAttribute("aria-expanded", 'false');
-        sideMenu.setAttribute('aria-hidden', 'true');
-        togglerLabel.setAttribute('aria-pressed', 'false');
-        body.style.overflow = 'visible';
+        togglerInput.checked = false
+        sideMenu.setAttribute("aria-expanded", "false")
+        sideMenu.setAttribute("aria-hidden", "true")
+        togglerLabel.setAttribute("aria-pressed", "false")
+        body.style.overflow = "visible"
     }
 
     function openMenu() {
-        togglerInput.checked = true;
-        sideMenu.setAttribute("aria-expanded", 'true');
-        sideMenu.setAttribute('aria-hidden', 'false');
-        togglerLabel.setAttribute('aria-pressed', 'true');
-        body.style.overflow = 'hidden';
+        togglerInput.checked = true
+        sideMenu.setAttribute("aria-expanded", "true")
+        sideMenu.setAttribute("aria-hidden", "false")
+        togglerLabel.setAttribute("aria-pressed", "true")
+        body.style.overflow = "hidden"
     }
 
     // Close menu when link on the sideMenu is clicked
-    sideMenu.addEventListener('click', function(event) {
-        let target = event.target;
-        if (target.tagName.toLowerCase() !== 'a') return;
-        closeMenu();
+    sideMenu.addEventListener("click", function(event) {
+        let target = event.target
+        if (target.tagName.toLowerCase() !== "a") {
+            return
+        }
+        closeMenu()
     })
     // Add accessibility data when sideMenu is opened/closed
-    togglerInput.addEventListener('change', function(e) {
-        togglerInput.checked ? openMenu() : closeMenu();
-    });
+    togglerInput.addEventListener("change", function(_event) {
+        togglerInput.checked ? openMenu() : closeMenu()
+    })
     // Make sideMenu links tabbable only when visible
     for (let menuItem of menuItems) {
         if (togglerInput.checked) {
-            menuItem.setAttribute('tabindex', '0');
+            menuItem.setAttribute("tabindex", "0")
         } else {
-            menuItem.setAttribute('tabindex', '-1');
+            menuItem.setAttribute("tabindex", "-1")
         }
     }
     // Close sideMenu when document body is clicked
-    doc.addEventListener('click', function() {
+    doc.addEventListener("click", function() {
         if (togglerInput.checked) {
-            closeMenu();
+            closeMenu()
         }
     })
 })
```

### Comparing `python-docs-theme-2023.3.1/python_docs_theme/static/py.png` & `python-docs-theme-2023.5/python_docs_theme/static/py.png`

 * *Files identical despite different names*

### Comparing `python-docs-theme-2023.3.1/python_docs_theme/static/py.svg` & `python-docs-theme-2023.5/python_docs_theme/static/py.svg`

 * *Files identical despite different names*

### Comparing `python-docs-theme-2023.3.1/python_docs_theme/static/pydoctheme.css` & `python-docs-theme-2023.5/python_docs_theme/static/pydoctheme.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,110 +1,173 @@
-@import url("default.css");
+@import url('classic.css');
+
+/* unset some styles from the classic stylesheet */
+div.document,
+div.body,
+div.related,
+div.body h1,
+div.body h2,
+div.body h3,
+div.body h4,
+div.body h5,
+div.body h6,
+div.sphinxsidebar a,
+div.sphinxsidebar p,
+div.sphinxsidebar ul,
+div.sphinxsidebar h3,
+div.sphinxsidebar h3 a,
+div.sphinxsidebar h4,
+.menu a,
+.menu p,
+.menu ul,
+.menu h3,
+.menu h3 a,
+.menu h4,
+table.docutils td,
+table.indextable tr.cap,
+pre {
+    background-color: inherit;
+    color: inherit;
+}
 
 body {
-    background-color: white;
     margin-left: 1em;
     margin-right: 1em;
 }
 
 .mobile-nav,
 .menu-wrapper {
     display: none;
 }
 
 div.related {
+    margin-top: 0.5em;
     margin-bottom: 1.2em;
     padding: 0.5em 0;
-    border-bottom: 1px solid #ccc;
-    margin-top: 0.5em;
+    border-width: 1px;
+    border-color: #ccc;
 }
 
-div.related a:hover {
-    color: #0095C4;
+.mobile-nav + div.related {
+    border-bottom-style: solid;
 }
 
-div.related ~ div.related {
-    border-top: 1px solid #ccc;
-    border-bottom: none;
+.document + div.related {
+    border-top-style: solid;
+}
+
+div.related a:hover {
+    color: #0095c4;
 }
 
 .related .switchers {
     display: inline-flex;
 }
 
 .switchers > div {
     margin-right: 5px;
 }
 
-.version_switcher_placeholder,
-.language_switcher_placeholder {
-    padding-left: 5px;
-    background-color: white;
+div.related ul::after {
+    content: '';
+    clear: both;
+    display: block;
 }
 
-.inline-search {
-    display: inline;
-}
+.inline-search,
 form.inline-search input {
     display: inline;
 }
-form.inline-search input[type="submit"] {
+
+form.inline-search input[type='submit'] {
     width: 40px;
 }
 
 div.document {
     display: flex;
 }
 
 div.sphinxsidebar {
     float: none;
     position: sticky;
     top: 0;
     max-height: 100vh;
-    background-color: #eeeeee;
+    color: #444;
+    background-color: #eee;
     border-radius: 5px;
     line-height: 130%;
     font-size: smaller;
 }
 
-div.sphinxsidebar h3, div.sphinxsidebar h4 {
+div.sphinxsidebar h3,
+div.sphinxsidebar h4 {
     margin-top: 1.5em;
 }
 
 div.sphinxsidebarwrapper {
+    width: 217px;
     box-sizing: border-box;
     height: 100%;
     overflow-x: hidden;
     overflow-y: auto;
+    float: left;
 }
 
 div.sphinxsidebarwrapper > h3:first-child {
     margin-top: 0.2em;
 }
 
 div.sphinxsidebarwrapper > ul > li > ul > li {
     margin-bottom: 0.4em;
 }
 
 div.sphinxsidebar a:hover {
-    color: #0095C4;
+    color: #0095c4;
 }
 
 form.inline-search input,
-div.sphinxsidebar input {
-    font-family: 'Lucida Grande',Arial,sans-serif;
+div.sphinxsidebar input,
+div.related input {
+    font-family: 'Lucida Grande', Arial, sans-serif;
     border: 1px solid #999999;
     font-size: smaller;
     border-radius: 3px;
 }
 
-div.sphinxsidebar input[type=text] {
+div.sphinxsidebar input[type='text'] {
     max-width: 150px;
 }
 
+#sidebarbutton {
+    /* Sphinx 4.x and earlier compat */
+    height: 100%;
+    background-color: #CCCCCC;
+    margin-left: 0;
+    color: #444444;
+    font-size: 1.2em;
+    cursor: pointer;
+    padding-top: 1px;
+    float: right;
+    display: table;
+    /* after Sphinx 4.x and earlier is dropped, only the below is needed */
+    width: 12px;
+    border-radius: 0 5px 5px 0;
+    border-left: none;
+}
+
+#sidebarbutton span {
+    /* Sphinx 4.x and earlier compat */
+    display: table-cell;
+    vertical-align: middle;
+}
+
+#sidebarbutton:hover {
+    background-color: #AAAAAA;
+}
+
 div.body {
     padding: 0 0 0 1.2em;
 }
 
 div.body p, div.body dd, div.body li, div.body blockquote {
     text-align: left;
     line-height: 1.4;
@@ -122,15 +185,16 @@
 }
 
 div.body pre {
     border-radius: 3px;
     border: 1px solid #ac9;
 }
 
-div.body div.admonition, div.body div.impl-detail {
+div.body div.admonition,
+div.body div.impl-detail {
     border-radius: 3px;
 }
 
 div.body div.impl-detail > p {
     margin: 0;
 }
 
@@ -143,108 +207,132 @@
 }
 
 div.body a:visited {
     color: #6363bb;
 }
 
 div.body a:hover {
-    color: #00B0E4;
+    color: #00b0e4;
 }
 
 tt, code, pre {
     font-family: ui-monospace, "Cascadia Mono", "Segoe UI Mono", "Liberation Mono", Menlo, Monaco, Consolas, monospace;
     font-size: 96.5%;
 }
 
-div.body tt, div.body code {
+div.body tt,
+div.body code {
     border-radius: 3px;
 }
 
-div.body tt.descname, div.body code.descname {
+div.body tt.descname,
+div.body code.descname {
     font-size: 120%;
 }
 
-div.body tt.xref, div.body a tt, div.body code.xref, div.body a code {
+div.body tt.xref,
+div.body a tt,
+div.body code.xref,
+div.body a code {
     font-weight: normal;
 }
 
 table.docutils {
     border: 1px solid #ddd;
     min-width: 20%;
     border-radius: 3px;
     margin-top: 10px;
     margin-bottom: 10px;
 }
 
-table.docutils td, table.docutils th {
+table.docutils td,
+table.docutils th {
     border: 1px solid #ddd !important;
     border-radius: 3px;
+    padding: 0.3em 0.5em;
 }
 
-table p, table li {
+table p,
+table li {
     text-align: left !important;
 }
 
 table.docutils th {
     background-color: #eee;
-    padding: 0.3em 0.5em;
 }
 
-table.docutils td {
-    background-color: white;
-    padding: 0.3em 0.5em;
-}
-
-table.footnote, table.footnote td {
+table.footnote,
+table.footnote td {
     border: 0 !important;
 }
 
 div.footer {
     line-height: 150%;
     text-align: right;
     width: auto;
     margin-right: 10px;
 }
 
 div.footer a:hover {
-    color: #0095C4;
+    color: #0095c4;
 }
 
 .refcount {
     color: #060;
 }
 
 .stableabi {
     color: #229;
 }
 
-.highlight {
-    background: none !important;
-}
-
-dl > dt span ~ em {
+dl > dt span ~ em,
+.sig {
     font-family: ui-monospace, "Cascadia Mono", "Segoe UI Mono", "Liberation Mono", Menlo, Monaco, Consolas, monospace;
 }
 
 .toctree-wrapper ul {
     padding-left: 20px;
 }
 
+.theme-selector {
+    margin-left: .5em;
+}
+
 div.genindex-jumpbox,
 div.genindex-jumpbox > p {
     display: inline-flex;
     flex-wrap: wrap;
 }
 
 div.genindex-jumpbox a {
     margin: 0 5px;
     min-width: 30px;
     text-align: center;
 }
 
+.copybutton {
+    cursor: pointer;
+    position: absolute;
+    top: 0;
+    right: 0;
+    text-size: 75%;
+    font-family: monospace;
+    padding-left: 0.2em;
+    padding-right: 0.2em;
+    border-radius: 0 3px 0 0;
+    color: #ac9; /* follows div.body pre */
+    border-color: #ac9; /* follows div.body pre */
+    border-style: solid; /* follows div.body pre */
+    border-width: 1px; /* follows div.body pre */
+}
+
+.copybutton[data-hidden='true'] {
+    text-decoration: line-through;
+}
+
 @media (max-width: 1023px) {
     /* Body layout */
     div.body {
         min-width: 100%;
         padding: 0;
         font-size: 0.875rem;
     }
@@ -285,128 +373,95 @@
     .mobile-nav {
         display: block;
         height: 40px;
         width: 100%;
         position: fixed;
         top: 0;
         left: 0;
-        background-color: white;
         box-shadow: rgba(0, 0, 0, 0.25) 0 0 2px 0;
         z-index: 1;
     }
     .mobile-nav * {
         box-sizing: border-box;
     }
     .nav-content {
         position: absolute;
-        z-index: 2;
-        left: 0;
-        top: 0;
+        z-index: 1;
         height: 40px;
         width: 100%;
-        max-width: 100vw;
-        padding: 0 1rem 0 45px;
         display: flex;
-        align-items: center;
         background-color: white;
     }
-    .nav-logo {
-        margin-right: 0.7rem;
+    .nav-items-wrapper {
         display: flex;
-        flex: 0 0 auto;
+        flex: auto;
+        padding: .25rem;
+        align-items: stretch;
+    }
+    .nav-logo {
+        margin-right: 1rem;
+        flex-shrink: 0;
+        align-self: center;
     }
     .nav-content img {
+        display: block;
         width: 20px;
-        height: auto;
     }
     .version_switcher_placeholder {
-        flex: 0 1 0;
         margin-right: 1rem;
     }
+    .version_switcher_placeholder > select {
+        height: 100%;
+    }
     .nav-content .search {
         display: flex;
-        flex: 1 1 auto;
-        align-items: center;
-        padding: 0 0 0 2px;
+        flex: auto;
         border: 1px solid #a9a9a9;
-        height: 30px;
-        overflow: hidden;
-    }
-    .nav-content .search:hover {
-        box-shadow: 0 1px 6px 0 rgba(32,33,36,0.28);
-        border-color: rgba(223,225,229,0);
+        align-items: stretch;
     }
-    .nav-content .search input[type=text] {
+    .nav-content .search input[type=search] {
         border: 0;
-        outline: 0;
-        box-shadow: none;
-        width: 40px;
-        height: 28px;
-        flex: 1 1 auto;
+        padding-left: 24px;
+        width: 100%;
+        flex: 1;
     }
     .nav-content .search input[type=submit] {
         height: 100%;
-        appearance: none;
-        -webkit-appearance: none;
-        border: 1px solid transparent;
-        border-left-color: #a9a9a9;
         box-shadow: none;
+        border: 0;
+        border-left: 1px solid #a9a9a9;
         cursor: pointer;
-        background-color: #f0f0f0;
         margin-right: 0;
     }
-    .nav-content .search input[type=submit]:hover {
-        border-color: #a9a9a9;
-    }
     .nav-content .search svg {
-        flex: 0 0 20px;
-        fill: #333;
+        position: absolute;
+        align-self: center;
+        padding-left: 4px;
     }
     .toggler__input {
-        width: 40px;
-        height: 40px;
-        left: 0;
-        opacity: 0;
-        position: absolute;
-        z-index: 3;
-        margin: 0;
+        display: none;
     }
     .toggler__label {
         width: 40px;
-        height: 40px;
-        margin: 0;
-        position: absolute;
         cursor: pointer;
-        top: 0;
-        left: 0;
-        background-color: transparent;
-        border: 1px solid white;
-        box-shadow: none;
-        z-index: 3;
         display: flex;
         align-items: center;
         justify-content: center;
-        padding: 0 8px;
+        padding: 8px;
+        flex-shrink: 0;
     }
-    .toggler__label:focus {
-        background-color: #eee;
-        border: 1px solid #ededed;
-        box-shadow: rgba(0, 0, 0, 0.25) 1px 0 2px 0;
-    }
-    .toggler__label:hover {
-        background-color: #eee;
-        border: 1px solid #ededed;
-        box-shadow: rgba(0, 0, 0, 0.25) 1px 0 2px 0;
+    .toggler__label:hover, .toggler__label:focus {
+        background-color: rgba(127 127 127 / 50%);
     }
     .toggler__label > span {
         position: relative;
         flex: none;
         height: 2px;
         width: 100%;
-        background: #444;
+        background: currentColor;
         transition: all 400ms ease;
     }
     .toggler__label > span::before,
     .toggler__label > span::after {
         content: '';
         height: 2px;
         width: 100%;
@@ -414,25 +469,25 @@
         position: absolute;
         left: 0;
         top: -8px;
     }
     .toggler__label > span::after {
         top: 8px;
     }
-    .toggler__input:checked ~ .toggler__label span {
+    .toggler__input:checked ~ nav > .toggler__label span {
         transform: rotate(135deg);
     }
-    .toggler__input:checked ~ .toggler__label span::before {
+    .toggler__input:checked ~ nav > .toggler__label span::before {
         transform: rotate(90deg);
     }
-    .toggler__input:checked ~ .toggler__label span::before,
-    .toggler__input:checked ~ .toggler__label span::after {
+    .toggler__input:checked ~ nav > .toggler__label span::before,
+    .toggler__input:checked ~ nav > .toggler__label span::after {
         top: 0;
     }
-    .toggler__input:checked:hover ~ .toggler__label span {
+    .toggler__input:checked:hover ~ nav > .toggler__label span {
         transform: rotate(315deg);
     }
     .toggler__input:checked ~ .menu-wrapper {
         visibility: visible;
         left: 0;
     }
 
@@ -442,14 +497,15 @@
         position: fixed;
         top: 0;
         transition: left 400ms ease;
         left: -310px;
         width: 300px;
         height: 100%;
         background-color: #eee;
+        color: #444444;
         box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
         overflow-y: auto;
     }
     .menu-wrapper.open {
         visibility: visible;
         left: 0;
     }
@@ -461,24 +517,22 @@
         margin-bottom: 0;
         font-weight: normal;
     }
     .menu-wrapper h4 {
         font-size: 1.3em;
     }
     .menu-wrapper h3 {
-        color: #444444;
         font-size: 1.4em;
     }
     .menu-wrapper h3 + p,
     .menu-wrapper h4 + p {
         margin-top: 0.5rem;
     }
     .menu a {
         font-size: smaller;
-        color: #444444;
         text-decoration: none;
     }
     .menu ul {
         list-style: none;
         line-height: 1.4;
         overflow-wrap: break-word;
         padding-left: 0;
@@ -486,58 +540,39 @@
     .menu ul ul {
         margin-left: 20px;
         list-style: square;
     }
     .menu ul li {
         margin-bottom: 0.5rem;
     }
-    .language_switcher_placeholder,
-    .version_switcher_placeholder {
-        position: relative;
-        border: 1px solid #a8a8a8;
-        height: 30px;
-        padding-right: 7px;
-    }
     .language_switcher_placeholder {
         margin-top: 2rem;
     }
-    .language_switcher_placeholder::after,
-    .version_switcher_placeholder::after {
-        content: url('../_static/caret-down.svg');
-        position: absolute;
-        top: 7px;
-        width: 15px;
-        height: 15px;
-        right: 0;
-        pointer-events: none;
-    }
-    .language_switcher_placeholder select,
-    .version_switcher_placeholder select {
-        -webkit-appearance: none;
-        appearance: none;
-        border: 0;
-        height: 100%;
-        background-color: white;
-    }
-    .language_switcher_placeholder:focus-visible,
-    .version_switcher_placeholder:focus-visible {
-        outline-offset: 5px;
-    }
     .language_switcher_placeholder select {
         width: 100%;
     }
     .document {
         position: relative;
         z-index: 0;
     }
     /*Responsive tables*/
     .responsive-table__container {
         width: 100%;
         overflow-x: auto;
     }
+
+    .menu .theme-selector-label {
+        margin-top: .5em;
+        display: flex;
+        width: 100%;
+    }
+
+    .menu .theme-selector {
+        flex: auto;
+    }
 }
 
 @media (min-width: 1024px) {
     div.footer {
         margin-top: -2em;
     }
 }
```

### Comparing `python-docs-theme-2023.3.1/python_docs_theme/theme.conf` & `python-docs-theme-2023.5/python_docs_theme/theme.conf`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [theme]
 inherit = default
 stylesheet = pydoctheme.css
 pygments_style = default
+pygments_dark_style = monokai
 
 [options]
 bodyfont = 'Lucida Grande', Arial, sans-serif
 headfont = 'Lucida Grande', Arial, sans-serif
 footerbgcolor = white
 footertextcolor = #555555
 relbarbgcolor = white
 relbartextcolor = #666666
 relbarlinkcolor = #444444
 sidebarbgcolor = white
 sidebartextcolor = #444444
 sidebarlinkcolor = #444444
+sidebarbtncolor = #cccccc
 bgcolor = white
 textcolor = #222222
 linkcolor = #0090c0
 visitedlinkcolor = #00608f
 headtextcolor = #1a1a1a
 headbgcolor = white
 headlinkcolor = #aaaaaa
```

### Comparing `python-docs-theme-2023.3.1/PKG-INFO` & `python-docs-theme-2023.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-docs-theme
-Version: 2023.3.1
+Version: 2023.5
 Summary: The Sphinx theme for the CPython docs and related projects
 Author-email: PyPA <distutils-sig@python.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Sphinx :: Theme
 Classifier: Intended Audience :: Developers
```

