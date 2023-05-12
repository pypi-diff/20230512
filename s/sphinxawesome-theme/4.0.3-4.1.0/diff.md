# Comparing `tmp/sphinxawesome_theme-4.0.3.tar.gz` & `tmp/sphinxawesome_theme-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxawesome_theme-4.0.3.tar", max compression
+gzip compressed data, was "sphinxawesome_theme-4.1.0.tar", max compression
```

## Comparing `sphinxawesome_theme-4.0.3.tar` & `sphinxawesome_theme-4.1.0.tar`

### file list

```diff
@@ -1,55 +1,59 @@
--rw-r--r--   0        0        0     1066 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/LICENSE
--rw-r--r--   0        0        0     2857 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/README.md
--rw-r--r--   0        0        0     2189 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/pyproject.toml
--rw-r--r--   0        0        0      172 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/README.rst
--rw-r--r--   0        0        0     2733 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/__init__.py
--rw-r--r--   0        0        0      671 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/breadcrumbs.html
--rw-r--r--   0        0        0     2255 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/docsearch.py
--rw-r--r--   0        0        0      875 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/footer.html
--rw-r--r--   0        0        0     2726 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/header.html
--rw-r--r--   0        0        0    12023 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/highlighting.py
--rw-r--r--   0        0        0    11203 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/html_translator.py
--rw-r--r--   0        0        0     1668 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/icons.py
--rw-r--r--   0        0        0     3085 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/jinja_functions.py
--rw-r--r--   0        0        0     1239 2023-04-16 05:34:13.172649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/jsonimpl.py
--rw-r--r--   0        0        0     2770 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/layout.html
--rw-r--r--   0        0        0     1396 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/menu.html
--rw-r--r--   0        0        0      622 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/modals.html
--rw-r--r--   0        0        0      311 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/page.html
--rw-r--r--   0        0        0     5817 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/postprocess.py
--rw-r--r--   0        0        0      836 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/prev_next.html
--rw-r--r--   0        0        0      692 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/scrolltop.html
--rw-r--r--   0        0        0      808 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/search.html
--rw-r--r--   0        0        0     1344 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/searchbox.html
--rw-r--r--   0        0        0     1055 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/sidebar.html
--rw-r--r--   0        0        0      432 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/skip.html
--rw-r--r--   0        0        0    28348 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff
--rw-r--r--   0        0        0    22192 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2
--rw-r--r--   0        0        0    17336 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/3a43b67e5bbdfb3ab0a6.woff2
--rw-r--r--   0        0        0    26732 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/42ba3027499c19034257.woff
--rw-r--r--   0        0        0    26680 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff
--rw-r--r--   0        0        0    20544 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/48af7707fe9e6494d6a5.woff
--rw-r--r--   0        0        0    25940 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff
--rw-r--r--   0        0        0    22092 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/9ac5da2442b734abc516.woff
--rw-r--r--   0        0        0    21184 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/a49e53c029ef019e7422.woff2
--rw-r--r--   0        0        0    27532 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff
--rw-r--r--   0        0        0    15744 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/b009a76ad6afe4ebd301.woff2
--rw-r--r--   0        0        0    22048 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/d037cb4792991826de7d.woff
--rw-r--r--   0        0        0    20388 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2
--rw-r--r--   0        0        0   106899 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/docsearch.53303c497cdefb581f6f.js
--rw-r--r--   0        0        0      109 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/docsearch.53303c497cdefb581f6f.js.LICENSE.txt
--rw-r--r--   0        0        0    15435 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/docsearch.70ebcfe862b41f7a90b7.css
--rw-r--r--   0        0        0      263 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/docsearch_config.js_t
--rw-r--r--   0        0        0    17368 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/e10742dbb1d4a0864ba8.woff2
--rw-r--r--   0        0        0    20932 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2
--rw-r--r--   0        0        0    20344 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/f1e2a76794cb86b2aa8e.woff
--rw-r--r--   0        0        0    15920 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/f25d774ecfe0996f8eb5.woff2
--rw-r--r--   0        0        0    21412 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2
--rw-r--r--   0        0        0     1862 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/manifest.json
--rw-r--r--   0        0        0    43174 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/theme.2e8060a090e1247124e3.css
--rw-r--r--   0        0        0    57350 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/theme.b62e1ded0c8c099a2d47.js
--rw-r--r--   0        0        0       93 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/theme.b62e1ded0c8c099a2d47.js.LICENSE.txt
--rw-r--r--   0        0        0      275 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/theme.conf
--rw-r--r--   0        0        0     1269 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/with-sidebar.html
--rw-r--r--   0        0        0     1101 2023-04-16 05:34:13.176649 sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/without-sidebar.html
--rw-r--r--   0        0        0     4167 1970-01-01 00:00:00.000000 sphinxawesome_theme-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-12 07:27:52.906417 sphinxawesome_theme-4.1.0/LICENSE
+-rw-r--r--   0        0        0     2663 2023-05-12 07:27:52.906417 sphinxawesome_theme-4.1.0/README.md
+-rw-r--r--   0        0        0     2368 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/README.rst
+-rw-r--r--   0        0        0     2814 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/__init__.py
+-rw-r--r--   0        0        0      671 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/breadcrumbs.html
+-rw-r--r--   0        0        0     3129 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/docsearch.py
+-rw-r--r--   0        0        0      959 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/footer.html
+-rw-r--r--   0        0        0     2658 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/header.html
+-rw-r--r--   0        0        0    12304 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/highlighting.py
+-rw-r--r--   0        0        0     1191 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/html_translator.py
+-rw-r--r--   0        0        0      825 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/icons.py
+-rw-r--r--   0        0        0     3085 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/jinja_functions.py
+-rw-r--r--   0        0        0     1158 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/jsonimpl.py
+-rw-r--r--   0        0        0     2852 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/layout.html
+-rw-r--r--   0        0        0     1396 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/menu.html
+-rw-r--r--   0        0        0      622 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/modals.html
+-rw-r--r--   0        0        0      311 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/page.html
+-rw-r--r--   0        0        0     7438 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/postprocess.py
+-rw-r--r--   0        0        0      836 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/prev_next.html
+-rw-r--r--   0        0        0      613 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/scrolltop.html
+-rw-r--r--   0        0        0      808 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/search.html
+-rw-r--r--   0        0        0     1344 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/searchbox.html
+-rw-r--r--   0        0        0     1055 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/sidebar.html
+-rw-r--r--   0        0        0      432 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/skip.html
+-rw-r--r--   0        0        0    28348 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff
+-rw-r--r--   0        0        0    28288 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/0ffeb7a552b36437b54c.woff
+-rw-r--r--   0        0        0    22192 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2
+-rw-r--r--   0        0        0    17336 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/3a43b67e5bbdfb3ab0a6.woff2
+-rw-r--r--   0        0        0    26760 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/44fd0da18fe361a5cc7f.woff
+-rw-r--r--   0        0        0    26680 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff
+-rw-r--r--   0        0        0    20544 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/48af7707fe9e6494d6a5.woff
+-rw-r--r--   0        0        0    25940 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff
+-rw-r--r--   0        0        0    22092 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/9ac5da2442b734abc516.woff
+-rw-r--r--   0        0        0    27532 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff
+-rw-r--r--   0        0        0        0 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/awesome-sphinx-design.31d6cfe0d16ae931b73c.js
+-rw-r--r--   0        0        0      798 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/awesome-sphinx-design.4ff695238f641b0a2852.css
+-rw-r--r--   0        0        0    15744 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/b009a76ad6afe4ebd301.woff2
+-rw-r--r--   0        0        0    22228 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/c3b5f43fe4c8f3f1fa21.woff2
+-rw-r--r--   0        0        0    21080 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/cfdd43ce3499ca7f900a.woff2
+-rw-r--r--   0        0        0    22048 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/d037cb4792991826de7d.woff
+-rw-r--r--   0        0        0    20388 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2
+-rw-r--r--   0        0        0   108012 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch.f1a1a5835ed7a6ab0c85.js
+-rw-r--r--   0        0        0      109 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch.f1a1a5835ed7a6ab0c85.js.LICENSE.txt
+-rw-r--r--   0        0        0    16727 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch.f30f8b0589fd2b6fd39c.css
+-rw-r--r--   0        0        0      795 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch_config.js_t
+-rw-r--r--   0        0        0    17368 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/e10742dbb1d4a0864ba8.woff2
+-rw-r--r--   0        0        0    20932 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2
+-rw-r--r--   0        0        0    20344 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/f1e2a76794cb86b2aa8e.woff
+-rw-r--r--   0        0        0    15920 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/f25d774ecfe0996f8eb5.woff2
+-rw-r--r--   0        0        0    21412 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2
+-rw-r--r--   0        0        0     2230 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/manifest.json
+-rw-r--r--   0        0        0    57949 2023-05-12 07:27:52.918418 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/theme.c8991bd7bb6e57cbeea8.js
+-rw-r--r--   0        0        0       93 2023-05-12 07:27:52.918418 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/theme.c8991bd7bb6e57cbeea8.js.LICENSE.txt
+-rw-r--r--   0        0        0    42667 2023-05-12 07:27:52.918418 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/theme.c973b470ab69573097f3.css
+-rw-r--r--   0        0        0      275 2023-05-12 07:27:52.918418 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/theme.conf
+-rw-r--r--   0        0        0     1333 2023-05-12 07:27:52.918418 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/with-sidebar.html
+-rw-r--r--   0        0        0     1157 2023-05-12 07:27:52.918418 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/without-sidebar.html
+-rw-r--r--   0        0        0     3754 1970-01-01 00:00:00.000000 sphinxawesome_theme-4.1.0/PKG-INFO
```

### Comparing `sphinxawesome_theme-4.0.3/LICENSE` & `sphinxawesome_theme-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/README.md` & `sphinxawesome_theme-4.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -45,19 +45,14 @@
 Each code block has a **Copy** button for easy copying.
 This theme enhances Sphinx's `code-block` directive with these options:
 
 - `emphasize-added`. Highlight lines that should be added to code
 - `emphasize-removed`. Highlight lines that should be removed from the code
 - `emphasize-text: TEXT`. Highlight `TEXT` in the code block to emphasize placeholder text the user should replace.
 
-### Collapsible elements
-
-Nested navigation links allow you to reach all pages from all other pages.
-You can make code object definitions like methods, classes, or modules collapsible as well.
-
 ### Better headerlinks
 
 Clicking the link icon after headers or captions automatically copies the URL to the clipboard.
 
 ### DocSearch
 
 If you have an Algolia DocSearch account for your documentation,
```

#### html2text {}

```diff
@@ -14,17 +14,14 @@
 beautiful documentation websites. These features make your documentation
 awesome: ### Awesome code blocks Code blocks show the language of the code in a
 header. Each code block has a **Copy** button for easy copying. This theme
 enhances Sphinx's `code-block` directive with these options: - `emphasize-
 added`. Highlight lines that should be added to code - `emphasize-removed`.
 Highlight lines that should be removed from the code - `emphasize-text: TEXT`.
 Highlight `TEXT` in the code block to emphasize placeholder text the user
-should replace. ### Collapsible elements Nested navigation links allow you to
-reach all pages from all other pages. You can make code object definitions like
-methods, classes, or modules collapsible as well. ### Better headerlinks
-Clicking the link icon after headers or captions automatically copies the URL
-to the clipboard. ### DocSearch If you have an Algolia DocSearch account for
-your documentation, you can use DocSearch for a search-as-you-type experience
-with autocomplete. Algolia DocSearch is free for open source documentation
-projects. ### Better keyboard navigation Use the `Tab` key to skip through all
-sections on the page. Use the `Space` key to expand or collapse items in the
-navigation menu or in code definitions.
+should replace. ### Better headerlinks Clicking the link icon after headers or
+captions automatically copies the URL to the clipboard. ### DocSearch If you
+have an Algolia DocSearch account for your documentation, you can use DocSearch
+for a search-as-you-type experience with autocomplete. Algolia DocSearch is
+free for open source documentation projects. ### Better keyboard navigation Use
+the `Tab` key to skip through all sections on the page. Use the `Space` key to
+expand or collapse items in the navigation menu or in code definitions.
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/__init__.py` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 """The Sphinx awesome theme as a Python package.
 
 :copyright: Copyright Kai Welke.
-:license: MIT, see LICENSE_ for details
-
-.. _LICENSE: https://github.com/kai687/sphinxawesome-theme/blob/master/LICENSE
+:license: MIT, see LICENSE for details
 """
 
 from importlib.metadata import PackageNotFoundError, version
 from os import path
 from typing import Any, Dict
 
 from sphinx.application import Sphinx
@@ -24,48 +22,50 @@
 
 
 def post_config_setup(app: Sphinx, config: Config) -> None:
     """Set up extensions if configuration is ready."""
     if config.html_awesome_highlighting:
         app.setup_extension("sphinxawesome_theme.highlighting")
 
-    if config.html_awesome_html_translator:
+    if config.html_awesome_external_links:
         app.setup_extension("sphinxawesome_theme.html_translator")
 
-    if config.html_awesome_postprocessing:
+    # The awesome code headers are handled in `postprocessing`
+    if config.html_awesome_postprocessing or config.html_awesome_code_headers:
         app.setup_extension("sphinxawesome_theme.postprocess")
 
     if config.html_awesome_docsearch:
         app.setup_extension("sphinxawesome_theme.docsearch")
 
+    # Add the CSS overrides if we're using the `sphinx-design` extension
+    if "sphinx_design" in app.extensions:
+        app.add_css_file("awesome-sphinx-design.css", priority=900)
+
 
 def setup(app: "Sphinx") -> Dict[str, Any]:
     """Register the theme and its extensions wih Sphinx."""
     app.add_html_theme(
         name="sphinxawesome_theme", theme_path=path.abspath(path.dirname(__file__))
     )
     app.add_config_value(
         name="html_awesome_postprocessing", default=True, rebuild="html", types=(bool)
     )
     app.add_config_value(
         name="html_awesome_highlighting", default=True, rebuild="html", types=(bool)
     )
     app.add_config_value(
-        name="html_awesome_html_translator", default=True, rebuild="html", types=(bool)
+        name="html_awesome_external_links", default=False, rebuild="html", types=(bool)
     )
     app.add_config_value(
         name="html_awesome_docsearch", default=False, rebuild="html", types=(bool)
     )
     app.add_config_value(
         name="docsearch_config", default={}, rebuild="html", types=(dict)
     )
     app.add_config_value(
-        name="html_collapsible_definitions", default=False, rebuild="html", types=(str)
-    )
-    app.add_config_value(
         name="html_awesome_headerlinks", default=True, rebuild="html", types=(str)
     )
     app.add_config_value(
         name="html_awesome_code_headers", default=True, rebuild="html", types=(str)
     )
 
     app.setup_extension("sphinxawesome_theme.jinja_functions")
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/breadcrumbs.html` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/docsearch.py` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/docsearch.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import os
 from pathlib import Path
 from typing import Any, Dict
 
 from docutils.nodes import Node
 from dotenv import load_dotenv
 from sphinx.application import Sphinx
+from sphinx.builders.dirhtml import DirectoryHTMLBuilder
+from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.util.display import progress_message
 
 from . import __version__
 
 
 @progress_message("Set up DocSearch")
 def setup_docsearch(
@@ -44,28 +46,46 @@
         "api_key": (
             os.getenv("DOCSEARCH_API_KEY") or app.config.docsearch_config.get("api_key")
         ),
         "index_name": (
             os.getenv("DOCSEARCH_INDEX_NAME")
             or app.config.docsearch_config.get("index_name")
         ),
+        "initial_query": (
+            os.getenv("DOCSEARCH_INITIAL_QUERY")
+            or app.config.docsearch_config.get("initial_query", "")
+        ),
+        "placeholder": (
+            os.getenv("DOCSEARCH_PLACEHOLDER")
+            or app.config.docsearch_config.get("placeholder", "")
+        ),
+        "missing_results_url": (
+            os.getenv("DOCSEARCH_MISSING_RESULTS_URL")
+            or app.config.docsearch_config.get("missing_results_url", "")
+        ),
     }
-    # If we want to use `docsearch` we don't need any other JS file from Sphinx
-    context["script_files"] = []
+    # If we want to use `docsearch` we don't need these default files
+    context["script_files"].remove("_static/sphinx_highlight.js")
+    context["script_files"].remove("_static/documentation_options.js")
+    context["script_files"].remove("_static/doctools.js")
     # Even if we're not using DocSearch, these things MUST be in the context
     context["docsearch"] = app.config.html_awesome_docsearch
     # update local context for rendering the `layout.html` templates for every page
     context["docsearch_config"] = docsearch_config
     # update the global context for writing the `docsearch_config.js` file
     app.builder.globalcontext["docsearch_config"] = docsearch_config  # type: ignore [attr-defined] # noqa: B950,E501
 
 
 def setup(app: Sphinx) -> Dict[str, Any]:
     """Register the extension."""
     app.add_css_file("docsearch.css", priority=150)
     app.connect("html-page-context", setup_docsearch)
 
+    # Disable built-in search when using DocSearch
+    StandaloneHTMLBuilder.search = False
+    DirectoryHTMLBuilder.search = False
+
     return {
         "version": __version__,
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/footer.html` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/footer.html`

 * *Files 19% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 {%- if last_updated -%}
   {%- trans last_updated=last_updated|e -%}
     Last updated: {{ last_updated }}.&nbsp;
   {%- endtrans -%}
 {%- endif -%}
 {%- if show_sphinx -%}
   {%- trans sphinx_version=sphinx_version|e -%}
-    Made with <a href="https://www.sphinx-doc.org">Sphinx {{ sphinx_version }}</a>
+    Made with <a class="text-link hover:text-brand focus:text-brand hover:underline focus:underline" href="https://www.sphinx-doc.org">Sphinx {{ sphinx_version }}</a>
   {%- endtrans -%}
 {%- endif -%}
 </div>
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/header.html` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/header.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 {#-
-  Template file for the header.
+Template file for the header.
 -#}
 
 {%- set hamburger -%}
-<button
-    data-action="sidebar#open"
-    data-sidebar-target="hamburger"
-    class="xl:hidden h-14 w-14 leading-14 text-gray-100 hover:bg-gray-700 hover:text-brand focus:outline-none focus:bg-gray-700 focus:text-brand">
+<button data-action="sidebar#open" data-sidebar-target="hamburger"
+  class="xl:hidden h-14 w-14 leading-14 text-gray-100 hover:bg-gray-700 hover:text-brand focus:outline-none focus:bg-gray-700 focus:text-brand">
   <span class="sr-only">Open navigation menu</span>
-  <svg aria-hidden="true" class="fill-current h-8 w-8" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M3 18h18v-2H3v2zm0-5h18v-2H3v2zm0-7v2h18V6H3z"/></svg>
+  <svg aria-hidden="true" class="inline fill-current h-8 w-8" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
+    <path d="M3 18h18v-2H3v2zm0-5h18v-2H3v2zm0-7v2h18V6H3z" />
+  </svg>
 </button>
 {%- endset -%}
 
 {%- macro home_link(logo=false) -%}
-<a class="hover:bg-gray-700 focus:bg-gray-700 focus:outline-none"
-   href="{{ pathto(master_doc) }}"
-   title="{{ _('Back to homepage') }}">
+<a class="hover:bg-gray-700 focus:bg-gray-700 focus:outline-none" href="{{ pathto(master_doc) }}"
+  title="{{ _('Back to homepage') }}">
 
   {%- set _logo_url = logo_url|default(pathto('_static/' + (logo or ""), 1)) %}
   {%- if logo or logo_url %}
-    <img class="h-14 w-14 p-3 inline-block" src="{{ _logo_url }}" alt="Logo" />
+  <img class="h-14 w-14 p-3 inline-block" src="{{ _logo_url }}" alt="Logo" />
   {%- endif -%}
-  <span class="hidden lg:inline-block shrink-0 font-medium text-gray-100 mx-5 leading-14 tracking-wider">{{ docstitle }}</span>
+  <span class="hidden lg:inline-block shrink-0 font-medium text-gray-100 mx-5 leading-14 tracking-wider">{{ docstitle
+    }}</span>
 </a>
 {%- endmacro -%}
 
 {%- macro extra_link(text, url) -%}
-  {% if url is string %}
-    {% set url = url if url.startswith("http") else pathto(url) %}
-    {%- set active = "bg-gray-700 border-b-4 border-brand" if pagename in url else "bg-transparent" -%}
-    <a href="{{ url }}" class="h-14 inline-block leading-14 text-gray-100 {{ active }} tracking-wide font-medium hover:text-brand focus:bg-gray-700 focus:outline-none hover:no-underline focus:text-brand px-2 sm:px-4">{{ text }}</a>
-  {% endif %}
-  {% if url is mapping %}
-    {% set link = url.link if url.link.startswith("http") else pathto(url.link) %}
-    <a href="{{ link }}" aria-label="Visit {{ text }}" class="tooltipped tooltipped-sw h-14 inline-block text-gray-100 leading-14 hover:text-brand focus:bg-gray-700 focus:outline-none hover:no-underline focus:text-brand pl-2 pr-4 sm:px-4">{{ url.icon }}</a>
-  {% endif %}
+{% if url is string %}
+{% set url = url if url.startswith("http") else pathto(url) %}
+{%- set active = "bg-gray-700 border-b-4 border-brand" if pagename in url else "bg-transparent" -%}
+<a href="{{ url }}"
+  class="h-14 inline-block leading-14 text-gray-100 {{ active }} tracking-wide font-medium hover:text-brand focus:bg-gray-700 focus:outline-none hover:no-underline focus:text-brand px-2 sm:px-4">{{
+  text }}</a>
+{% endif %}
+{% if url is mapping %}
+{% set link = url.link if url.link.startswith("http") else pathto(url.link) %}
+<a href="{{ link }}" title="Visit {{ text }}"
+  class="h-14 inline-block text-gray-100 leading-14 hover:text-brand focus:bg-gray-700 focus:outline-none hover:no-underline focus:text-brand pl-2 pr-4 sm:px-4">{{
+  url.icon }}</a>
+{% endif %}
 {%- endmacro -%}
 
 
 <div class="bg-gray-dark shadow-md flex items-center h-full xl:px-2 relative">
   {#- show logo on the left side of the header -#}
   <div class="flex items-center">
     {%- if theme_show_nav|tobool %}
-      {{ hamburger }}
+    {{ hamburger }}
     {%- endif %}
     {%- block logo -%}
-      {{ home_link(logo) }}
+    {{ home_link(logo) }}
     {%- endblock -%}
   </div>
 
   {#- show a search input field on the right side -#}
   <div class="flex justify-end items-center flex-1">
     {%- include "searchbox.html" %}
 
     {%- if theme_extra_header_links|tobool -%}
-      {%- block extra_header_links -%}
-      <div class="shrink-0">
-        {%- for text, url in theme_extra_header_links.items() -%}
-          {{ extra_link(text, url) }}
-        {%- endfor -%}
-      </div>
-      {%- endblock -%}
+    {%- block extra_header_links -%}
+    <div class="shrink-0">
+      {%- for text, url in theme_extra_header_links.items() -%}
+      {{ extra_link(text, url) }}
+      {%- endfor -%}
+    </div>
+    {%- endblock -%}
     {%- endif -%}
   </div>
 </div>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 {#- Template file for the header. -#} {%- set hamburger -%}  Open navigation
-menu   {%- endset -%} {%- macro home_link(logo=false) -%} {%-_set__logo_url_=
+menu     {%- endset -%} {%- macro home_link(logo=false) -%} {%-_set__logo_url_=
 logo_url|default(pathto('_static/'_+_(logo_or_""),_1))_%}_{%-_if_logo_or
 logo_url_%}_[Logo]_{%-_endif_-%}_{{_docstitle_}} {%- endmacro -%} {%- macro
 extra_link(text, url) -%} {% if url is string %} {% set url = url if
 url.startswith("http") else pathto(url) %} {%- set active = "bg-gray-700
 border-b-4 border-brand" if pagename in url else "bg-transparent" -%} {{_text
 }} {% endif %} {% if url is mapping %} {% set link = url.link if
 url.link.startswith("http") else pathto(url.link) %} {{_url.icon_}} {% endif %}
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/highlighting.py` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/highlighting.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,270 +6,234 @@
 
 To make use of this new function, this theme also
 extends the default Sphinx ``code-block`` directive.
 
 :copyright: Copyright Kai Welke.
 :license: MIT, see LICENSE for details.
 """
-import contextlib
-from typing import Any, Dict, Generator, List, Tuple
+import re
+from typing import Any, Dict, Generator, List, Optional, Pattern, Tuple, Union
 
 from docutils import nodes
-from docutils.nodes import Node
+from docutils.nodes import Element, Node
 from docutils.parsers.rst import directives
-from docutils.statemachine import StringList
+from pygments import highlight
+from pygments.filter import Filter
+from pygments.filters import ErrorToken
 from pygments.formatters import HtmlFormatter
 from pygments.lexers.shell import BashSessionLexer
+from pygments.token import Generic, _TokenType
 from pygments.util import get_list_opt
 from sphinx.application import Sphinx
-from sphinx.directives.code import CodeBlock, dedent_lines
+from sphinx.directives.code import CodeBlock, container_wrapper, dedent_lines
 from sphinx.highlighting import PygmentsBridge
 from sphinx.locale import __
-from sphinx.util import logging, parselinenos
-from sphinx.util.docutils import SphinxDirective
+from sphinx.util import logging, parselinenos, texescape
 
 from . import __version__
 
 logger = logging.getLogger(__name__)
 
 # type alias
-TokenStream = Generator[Tuple[int, str], None, None]
+TokenType = Union[_TokenType, int]
+TokenStream = Generator[Tuple[TokenType, str], None, None]
 
 
-def container_wrapper(
-    directive: SphinxDirective, literal_node: Node, caption: str
-) -> nodes.container:
-    """We need the container to have class highlight."""
-    container_node = nodes.container(
-        "",
-        literal_block=True,
-        language=literal_node["language"],  # type: ignore
-        classes=["highlight"],
-    )
-    parsed = nodes.Element()
-    directive.state.nested_parse(
-        StringList([caption], source=""), directive.content_offset, parsed
-    )
-    if isinstance(parsed[0], nodes.system_message):
-        msg = __("Invalid caption: %s" % parsed[0].astext())
-        raise ValueError(msg)
-    elif isinstance(parsed[0], nodes.Element):
-        caption_node = nodes.caption(
-            parsed[0].rawsource,
-            "",
-            *parsed[0].children,
+def _replace_placeholders(
+    ttype: _TokenType, value: str, regex: Pattern[str]
+) -> TokenStream:
+    """Replace every occurence of `regex` with `Generic.Emph` token."""
+    last = 0
+    for match in regex.finditer(value):
+        start, end = match.start(), match.end()
+        if start != last:
+            yield ttype, value[last:start]
+        yield Generic.Emph, value[start:end]
+        last = end
+    if last != len(value):
+        yield ttype, value[last:]
+
+
+class AwesomePlaceholders(Filter):  # type: ignore[misc]
+    """A Pygments filter for marking up placeholder text."""
+
+    def __init__(self: "AwesomePlaceholders", **options: Any) -> None:
+        """Create an instance of the `AwesomePlaceholders` filter."""
+        Filter.__init__(self, **options)
+        placeholders = get_list_opt(options, "hl_text", [])
+        self.placeholders_re = re.compile(
+            r"|".join([re.escape(x) for x in placeholders if x])
         )
-        caption_node.source = literal_node.source
-        caption_node.line = literal_node.line
-        container_node += caption_node
-        container_node += literal_node
-        return container_node
-    else:
-        raise RuntimeError  # never reached
+
+    def filter(
+        self: "AwesomePlaceholders", _lexer: Any, stream: TokenStream
+    ) -> TokenStream:
+        """Filter on all tokens.
+
+        The `lexer` is required by the parent class.
+        """
+        regex = self.placeholders_re
+        for ttype, value in stream:
+            yield from _replace_placeholders(ttype, value, regex)
 
 
 class AwesomeHtmlFormatter(HtmlFormatter):  # type: ignore
     """Custom HTML formatter for Pygments.
 
-    This produces quite different HTML compared to Sphinx.
-    - the code block is wrapped in ``<pre><code>``
-      as recommended by the HTML living standard.
-    - allow highlighting added/removed lines: this is different from
-      using the ``diff`` syntax, as it can be combined with any syntax.
-    - it only uses the inline line number mechanism
-      that's going to be the future. It's much easier to have consistent
-      styling that way.
+    Allow highlighting added or removed lines.
+    Similar to emphasizing lines.
+
+    In contrast to Pygments, this formatter returns `<mark>` for higlighted lines.
     """
 
     def __init__(self: "AwesomeHtmlFormatter", **options: Any) -> None:
         """Implement `hl_added` and `hl_removed` options."""
         self.added_lines = set()
         self.removed_lines = set()
 
         for lineno in get_list_opt(options, "hl_added", []):
-            with contextlib.suppress(ValueError):
+            try:
                 self.added_lines.add(int(lineno))
+            except ValueError:
+                pass
 
         for lineno in get_list_opt(options, "hl_removed", []):
-            with contextlib.suppress(ValueError):
+            try:
                 self.removed_lines.add(int(lineno))
+            except ValueError:
+                pass
+
+        # These options aren't compatible with `sphinx.ext.autodoc`
+        # options["lineanchors"] = "code"
+        # options["linespans"] = "code-line"
+        options["wrapcode"] = True
 
         super().__init__(**options)
 
     def _highlight_lines(
         self: "AwesomeHtmlFormatter", tokensource: TokenStream
     ) -> TokenStream:
-        """Add classes to `hl_added` and `hl_removed` lines.
+        """Highlight added, removed, and emphasized lines.
 
-        Simplification, because we only need to care about class-based styles
-        for this theme.
+        In contrast to Pygments, use `<mark>`, `<ins>`, and `<del>` elements.
         """
         for i, (t, value) in enumerate(tokensource):
             if t != 1:
                 yield t, value
-            if i + 1 in self.hl_lines:  # i + 1 because Python indexes start at 0
+            if i + 1 in self.hl_lines:
                 yield 1, "<mark>%s</mark>" % value
             elif i + 1 in self.added_lines:
                 yield 1, "<ins>%s</ins>" % value
             elif i + 1 in self.removed_lines:
                 yield 1, "<del>%s</del>" % value
             else:
                 yield 1, value
 
-    def wrap(
-        self: "AwesomeHtmlFormatter", source: TokenStream, outfile: Any
-    ) -> TokenStream:
-        """Return a <pre><code> wrapped element.
-
-        Pygments returns the highlighted block wrapped inside a ``div.highlight``.
-        We want to get the <pre> only, and we'll wrap it in a div later, so that
-        we can add the code button, and an optional caption.
-
-        Returning a <pre><code> block follows the HTML5 specification for marking
-        up code blocks.
-        """
-        return self._wrap_div(self._wrap_pre(self._wrap_code(source)))
-
-    def _wrap_div(self: "AwesomeHtmlFormatter", inner: TokenStream) -> TokenStream:
-        """Wrap the highlighted code in a div for easier styling."""
-        yield 0, ('<div class="highlight">')
-        yield from inner
-        yield 0, ("</div>")
-
-    def _wrap_pre(self: "AwesomeHtmlFormatter", inner: TokenStream) -> TokenStream:
-        """Overwrite this method.
-
-        I don't want an empty span in front of every code block.
-        This is a simplification as the theme doesn't use inline styles.
-        """
-        if self.filename:
-            yield 0, ('<span class="filename">' + self.filename + "</span>")
-
-        yield 0, ("<pre>")
-        yield from inner
-        yield 0, ("</pre>")
-
-    def _wrap_linespans(
-        self: "AwesomeHtmlFormatter", inner: TokenStream
-    ) -> TokenStream:
-        """Overwrite as I want a class applied to the linespan."""
-        i = self.linenostart - 1
-        for t, line in inner:
-            if t:
-                i += 1
-                yield 1, f"<span id='line-{i}' class='code-line'>{line}</span>"
-            else:
-                yield 0, line
-
     def format_unencoded(
-        self: "AwesomeHtmlFormatter", tokensource: Tuple[Any, Any], outfile: Any
+        self: "AwesomeHtmlFormatter",
+        tokensource: TokenStream,
+        outfile: Any,
     ) -> None:
-        """Produce the highlighted code block for Sphinx.
+        """Overwrite method to handle emphasized, added, and removed lines.
 
-        First, we add the line numbers, then line spans, then add the emphasized lines.
-        This is to have consistent spacing with and without line numbers.
+        Unfortunately, the method doesn't extend easily, so I copy it from Pygments.
         """
         source = self._format_lines(tokensource)
 
-        # add the line numbers first
-        if self.linenos == 2:
+        # As a special case, we wrap line numbers before line highlighting
+        # so the line numbers get wrapped in the highlighting tag.
+        if not self.nowrap and self.linenos == 2:
             source = self._wrap_inlinelinenos(source)
-            source = self._wrap_linespans(source)
 
-        # then add the highlighted lines
+        # This is the only change I made from the original
         if self.hl_lines or self.added_lines or self.removed_lines:
             source = self._highlight_lines(source)
 
-        # wrap the thing in <code> and <pre>
         if not self.nowrap:
-            source = self.wrap(source, outfile)
+            if self.lineanchors:
+                source = self._wrap_lineanchors(source)
+            if self.linespans:
+                source = self._wrap_linespans(source)
+            source = self.wrap(source)
+            if self.linenos == 1:
+                source = self._wrap_tablelinenos(source)
+            source = self._wrap_div(source)
+            if self.full:
+                source = self._wrap_full(source, outfile)
 
         for _, piece in source:
             outfile.write(piece)
 
 
+def _get_parsed_line_numbers(linespec: str, nlines: int, location: str) -> List[int]:
+    """Get the parsed line numbers for the `emphasize-*` options."""
+    line_numbers = parselinenos(linespec, nlines)
+    if any(i >= nlines for i in line_numbers):
+        logger.warning(
+            __("line number spec is out of range(1-%d): %r") % (nlines, linespec),
+            location=location,
+        )
+    return [x + 1 for x in line_numbers if x < nlines]
+
+
 class AwesomeCodeBlock(CodeBlock):
     """Add options to highlight added and removed lines to `code-block` directives."""
 
     new_options = {
         "emphasize-added": directives.unchanged_required,
         "emphasize-removed": directives.unchanged_required,
         "emphasize-text": directives.unchanged_required,
     }
 
     option_spec = CodeBlock.option_spec
     option_spec.update(new_options)
 
-    def run(self: "AwesomeCodeBlock") -> List[Node]:  # noqa: C901
-        """Implement option method."""
+    def run(self: "AwesomeCodeBlock") -> List[Node]:  # noqa
+        """Overwrite method from Sphinx.
+
+        Add ability to highlight added and removed lines.
+        This passes the options to the highlighter.
+        You need a custom pygments formatter.
+
+        Unfortunately, the original method doesn't lend itself to being extended,
+        so I had to copy it.
+        """
         document = self.state.document
         code = "\n".join(self.content)
         location = self.state_machine.get_source_and_line(self.lineno)
+        nlines = len(self.content)
 
+        hl_lines = hl_added = hl_removed = None
         linespec = self.options.get("emphasize-lines")
         if linespec:
             try:
-                nlines = len(self.content)
-                hl_lines = parselinenos(linespec, nlines)
-                if any(i >= nlines for i in hl_lines):
-                    logger.warning(
-                        __("line number spec is out of range(1-%d): %r")
-                        % (nlines, self.options["emphasize-lines"]),
-                        location=location,
-                    )
-
-                hl_lines = [x + 1 for x in hl_lines if x < nlines]
+                hl_lines = _get_parsed_line_numbers(linespec, nlines, location)
             except ValueError as err:
                 return [document.reporter.warning(err, line=self.lineno)]
-        else:
-            hl_lines = []
 
-        # add parsing for hl_added and hl_removed
         linespec = self.options.get("emphasize-added")
         if linespec:
             try:
-                nlines = len(self.content)
-                hl_added = parselinenos(linespec, nlines)
-                if any(i >= nlines for i in hl_added):
-                    logger.warning(
-                        __("line number spec is out of range(1-%d): %r")
-                        % (nlines, self.options["emphasize-added"]),
-                        location=location,
-                    )
-                hl_added = [x + 1 for x in hl_added if x < nlines]
+                hl_added = _get_parsed_line_numbers(linespec, nlines, location)
             except ValueError as err:
                 return [document.reporter.warning(err, line=self.lineno)]
-        else:
-            hl_added = []
 
-        # add parsing for hl_added and hl_removed
         linespec = self.options.get("emphasize-removed")
         if linespec:
             try:
-                nlines = len(self.content)
-                hl_removed = parselinenos(linespec, nlines)
-                if any(i >= nlines for i in hl_removed):
-                    logger.warning(
-                        __("line number spec is out of range(1-%d): %r")
-                        % (nlines, self.options["emphasize-removed"]),
-                        location=location,
-                    )
-                hl_removed = [x + 1 for x in hl_removed if x < nlines]
+                hl_removed = _get_parsed_line_numbers(linespec, nlines, location)
             except ValueError as err:
                 return [document.reporter.warning(err, line=self.lineno)]
-        else:
-            hl_removed = []
 
         if "dedent" in self.options:
-            location = self.state_machine.get_source_and_line(self.lineno)
-            lines = code.split("\n")
+            lines = code.splitlines(True)
             lines = dedent_lines(lines, self.options["dedent"], location=location)
-            code = "\n".join(lines)
+            code = "".join(lines)
 
-        literal = nodes.literal_block(code, code)
+        literal: Element = nodes.literal_block(code, code)
         if "linenos" in self.options or "lineno-start" in self.options:
             literal["linenos"] = True
         literal["classes"] += self.options.get("class", [])
         literal["force"] = "force" in self.options
         if self.arguments:
             # highlight language specified
             literal["language"] = self.arguments[0]
@@ -277,42 +241,93 @@
             # no highlight language specified.  Then this directive refers the current
             # highlight setting via ``highlight`` directive or ``highlight_language``
             # configuration.
             literal["language"] = self.env.temp_data.get(
                 "highlight_language", self.config.highlight_language
             )
         extra_args = literal["highlight_args"] = {}
-        if hl_lines:
+        if hl_lines is not None:
             extra_args["hl_lines"] = hl_lines
-        if hl_added:
+        if hl_added is not None:
             extra_args["hl_added"] = hl_added
-        if hl_removed:
+        if hl_removed is not None:
             extra_args["hl_removed"] = hl_removed
         if "lineno-start" in self.options:
             extra_args["linenostart"] = self.options["lineno-start"]
         if "emphasize-text" in self.options:
             extra_args["hl_text"] = self.options["emphasize-text"]
+
         self.set_source_info(literal)
 
-        # if there is a caption, we need to wrap this node in a container
         caption = self.options.get("caption")
         if caption:
             try:
                 literal = container_wrapper(self, literal, caption)
             except ValueError as exc:
                 return [document.reporter.warning(exc, line=self.lineno)]
 
+        # literal will be note_implicit_target that is linked from caption and numref.
+        # when options['name'] is provided, it should be primary ID.
         self.add_name(literal)
 
         return [literal]
 
 
+class AwesomePygmentsBridge(PygmentsBridge):
+    """Class for monkeypatching."""
+
+    def highlight_block(
+        self: PygmentsBridge,
+        source: str,
+        lang: str,
+        opts: Optional[Dict[str, Any]] = None,
+        force: bool = False,
+        location: Any = None,
+        **kwargs: Any
+    ) -> str:
+        """Repeat this method."""
+        if not isinstance(source, str):
+            source = source.decode()  # type: ignore[unreachable]
+
+        lexer = self.get_lexer(source, lang, opts, force, location)
+        hl_text = get_list_opt(kwargs, "hl_text", [])
+        if hl_text:
+            lexer.add_filter(AwesomePlaceholders(hl_text=hl_text))
+
+        # highlight via Pygments
+        formatter = self.get_formatter(**kwargs)
+        try:
+            hlsource: str = highlight(source, lexer, formatter)
+        except ErrorToken:
+            # this is most probably not the selected language,
+            # so let it pass unhighlighted
+            if lang == "default":
+                pass  # automatic highlighting failed.
+            else:
+                logger.warning(
+                    __('Could not lex literal_block as "%s". ' "Highlighting skipped."),
+                    lang,
+                    type="misc",
+                    subtype="highlighting_failure",
+                    location=location,
+                )
+            lexer = self.get_lexer(source, "none", opts, force, location)
+            hlsource = highlight(source, lexer, formatter)
+
+        if self.dest == "html":
+            return hlsource
+        else:
+            # MEMO: this is done to escape Unicode chars with non-Unicode engines
+            return texescape.hlescape(hlsource, self.latex_engine)
+
+
 def setup(app: "Sphinx") -> Dict[str, Any]:
     """Set up this internal extension."""
     PygmentsBridge.html_formatter = AwesomeHtmlFormatter
+    PygmentsBridge.highlight_block = AwesomePygmentsBridge.highlight_block  # type: ignore[method-assign]  # noqa
     directives.register_directive("code-block", AwesomeCodeBlock)
 
     # Allow using `terminal` in addition to `shell-session` and `console`
     # for interactive command-line sessions
     app.add_lexer("terminal", BashSessionLexer)
 
     return {
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/jinja_functions.py` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/jinja_functions.py`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/jsonimpl.py` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/jsonimpl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """Custom JSON serializer.
 
 The awesome theme uses custom jinja2 helper functions which are
 non-serializable by default. Hence, I need to use a custom JSON
 serializer.
 
 :copyright: Copyright Kai Welke.
-:license: MIT, see LICENSE_ for details.
-
-.. _LICENSE: https://github.com/kai687/sphinxawesome-theme/blob/master/LICENSE
+:license: MIT, see LICENSE for details.
 """
 
 import json
 from typing import IO, Any
 
 
 class AwesomeJSONEncoder(json.JSONEncoder):
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/layout.html` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/layout.html`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 {%- set titlesuffix = " | "|safe + docstitle|e -%}
 {%- endif -%}
 {%- else -%}
 {%- set titlesuffix = "" -%}
 {%- endif -%}
 
 <!DOCTYPE html>
-<html lang="{{ lang_attr }}">
+<html lang="{{ lang_attr }}" class="scroll-smooth">
 
 <head>
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <meta charset="utf-8" />
   {{ metatags }}
   {%- block htmltitle %}
   <title>{{ title|striptags|e if title else docstitle }}{{ titlesuffix }}</title>
@@ -55,21 +55,23 @@
   {%- if next %}
   <link rel="next" title="{{ next.title|striptags|e }}" href="{{ next.link|e }}" />
   {%- endif %}
   {%- if prev %}
   <link rel="prev" title="{{ prev.title|striptags|e }}" href="{{ prev.link|e }}" />
   {%- endif %}
   {%- endblock %}
+  {%- block extrahead %}{%- endblock %}
 </head>
 
-<body class="antialiased text-gray scroll-smooth">
-  <div id="page" data-controller="sidebar search {{ 'scroll' if theme_show_scrolltop|tobool }}"
-    data-action="keydown@window->search#focus {{ 'scroll@window->scroll#showButton' if theme_show_scrolltop|tobool }}"
-    class="min-h-screen xl:h-screen flex flex-col xl:grid xl:grid-layout print:block print:h-auto">
-    {% include "skip.html" %}
+<body class="antialiased text-gray">
+    <div id="page" data-controller="sidebar search scroll {{ 'scroll-to-top' if theme_show_scrolltop|tobool }}"
+      data-action="keydown@window->search#focus {{ 'scroll@window->scroll-to-top#showButton' if theme_show_scrolltop|tobool }}"
+      class="min-h-screen xl:h-screen flex flex-col xl:grid xl:grid-layout print:block print:h-auto"
+    >
+      {% include "skip.html" %}
 
     <header class="grid-area-header z-10 h-14 fixed w-full top-0 print:hidden">
       {% include "header.html" %}
     </header>
 
     {% block document %}
     {% endblock %}
```

#### html2text {}

```diff
@@ -15,11 +15,11 @@
  {%- endif %} {%- set _favicon_url = favicon_url | default(pathto('_static/' +
 (favicon or ""), 1)) %} {%- if favicon_url or favicon %}
  {%- endif %} {%- block linktags %} {%- if hasdoc('search') and not docsearch
 %}
  {%- endif %} {%- if hasdoc('genindex') %}
  {%- endif %} {%- if next %}
  {%- endif %} {%- if prev %}
- {%- endif %} {%- endblock %}
+ {%- endif %} {%- endblock %} {%- block extrahead %}{%- endblock %}
 {% include "skip.html" %}  {% include "header.html" %}  {% block document %} {%
 endblock %} {% include "modals.html" %}
 {% block scripts %} {{ script() }} {% endblock %}
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/menu.html` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/menu.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/modals.html` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/modals.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/postprocess.py` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/postprocess.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 They might not show up in the final CSS.
 
 :copyright: Copyright Kai Welke.
 :license: MIT, see LICENSE.
 """
 
 import os
+import re
 from typing import Any, Dict, List, Optional
 
 from bs4 import BeautifulSoup, Comment
 from sphinx.application import Sphinx
 from sphinx.util import logging
 
 from . import __version__
@@ -60,38 +61,30 @@
             link.wrap(tree.new_tag("div", attrs={"class": "nav-link"}))
             # Next, insert a span.expand before the link, if the #nav-link
             # has any sibling elements (a ``ul`` in the navigation menu)
             if link.parent.next_sibling:
                 # create the icon
                 svg = BeautifulSoup(ICONS["chevron_right"], "html.parser").svg
                 svg["tabindex"] = "0"
+                svg["height"] = "1.2rem"
                 svg["class"] = ["expand"]
+                svg["style"] = ["display: inline;"]
                 svg[
                     "data-action"
                 ] = "click->sidebar#expand keydown->sidebar#expandKeyPressed"
                 link.insert_before(svg)
 
 
 def _expand_current(tree: BeautifulSoup) -> None:
     """Add the ``.expanded`` class to li.current elements."""
     for li in tree("li", class_="current"):
         if "expanded" not in li.get("class", []):
             li["class"] += ["expanded"]
 
 
-def _remove_span_pre(tree: BeautifulSoup) -> None:
-    """Unwrap unnecessary spans.
-
-    This gets added by visit_Text(). If I overwrite it there,
-    it's 20 lines of code for only 1 line of change.
-    """
-    for span in tree("span", class_="pre"):
-        span.unwrap()
-
-
 def _remove_empty_toctree(tree: BeautifulSoup) -> None:
     """Remove empty toctree divs.
 
     If you include a `toctree` with the `hidden` option,
     an empty `div` is inserted. Remove them.
     The empty `div` contains a single `end-of-line` character.
     """
@@ -107,45 +100,89 @@
         link["data-controller"] = "clipboard"
         link["data-action"] = "click->clipboard#copyHeaderLink"
         link["aria-label"] = "Click to copy this link"
         del link["title"]
         link["class"].extend(["tooltipped", "tooltipped-ne"])
 
 
+def _code_controller(tree: BeautifulSoup) -> None:
+    """Add the controller attribute to code blocks."""
+    for block in tree("div", class_="highlight"):
+        block["data-controller"] = "code"
+
+
 def _external_links(tree: BeautifulSoup) -> None:
-    """Add `rel="nofollow noopener"` to external links."""
+    """Add `rel="nofollow noopener"` to external links.
+
+    The alternative was to copy `visit_reference` in the HTMLTranslator
+    and change literally one line.
+    """
     for link in tree("a", class_="reference external"):
         link["rel"] = "nofollow noopener"
 
 
 def _strip_comments(tree: BeautifulSoup) -> None:
     """Remove HTML comments from documents."""
     comments = tree.find_all(string=lambda text: isinstance(text, Comment))
     for c in comments:
         c.extract()
 
 
+def _code_headers(tree: BeautifulSoup) -> None:
+    """Add the programming language to a code block."""
+    # Find all "<div class="highlight-<LANG> notranslate>" blocks
+    pattern = re.compile("highlight-(.*) ")
+    for code_block in tree.find_all("div", class_=pattern):
+        hl_lang = None
+        # Get the highlight language
+        classes_string = " ".join(code_block.get("class", []))
+        match = pattern.search(classes_string)
+        if match:
+            hl_lang = match.group(1).replace("default", "python")
+
+        parent = code_block.parent
+
+        # Deal with code blocks with captions
+        if "literal-block-wrapper" in parent.get("class", []):
+            caption = parent.select(".code-block-caption")[0]
+            if caption:
+                span = tree.new_tag("span", attrs={"class": "code-lang"})
+                span.append(tree.new_string(hl_lang))
+                caption.insert(0, span)
+        else:
+            # Code block without captions, we need to wrap them first
+            wrapper = tree.new_tag("div", attrs={"class": "literal-block-wrapper"})
+            caption = tree.new_tag("div", attrs={"class": "code-block-caption"})
+            span = tree.new_tag("span", attrs={"class": "code-lang"})
+            span.append(tree.new_string(hl_lang))
+            caption.append(span)
+            code_block.wrap(wrapper)
+            wrapper.insert(0, caption)
+
+
 def _modify_html(html_filename: str, app: Sphinx) -> None:
     """Modify a single HTML document.
 
     1. The HTML document is parsed into a BeautifulSoup tree.
     2. The modifications are performed in order and in place.
     3. After these modifications, the HTML is written into a file,
     overwriting the original file.
     """
     with open(html_filename, encoding="utf-8") as html:
         tree = BeautifulSoup(html, "html.parser")
 
     _expand_current(tree)
     _collapsible_nav(tree)
-    _remove_span_pre(tree)
-    _remove_empty_toctree(tree)
     _external_links(tree)
+    _remove_empty_toctree(tree)
     if app.config.html_awesome_headerlinks:
         _headerlinks(tree)
+    _code_controller(tree)
+    if app.config.html_awesome_code_headers:
+        _code_headers(tree)
     _strip_comments(tree)
 
     with open(html_filename, "w", encoding="utf-8") as out_file:
         out_file.write(str(tree))
 
 
 def post_process_html(app: Sphinx, exc: Optional[Exception]) -> None:
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/prev_next.html` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/prev_next.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/search.html` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/searchbox.html` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/sidebar.html` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/sidebar.html`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/3a43b67e5bbdfb3ab0a6.woff2` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/3a43b67e5bbdfb3ab0a6.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/48af7707fe9e6494d6a5.woff` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/48af7707fe9e6494d6a5.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/9ac5da2442b734abc516.woff` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/9ac5da2442b734abc516.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/b009a76ad6afe4ebd301.woff2` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/b009a76ad6afe4ebd301.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/d037cb4792991826de7d.woff` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/d037cb4792991826de7d.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/docsearch.53303c497cdefb581f6f.js` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch.f1a1a5835ed7a6ab0c85.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see docsearch.53303c497cdefb581f6f.js.LICENSE.txt */ ! function() {
+/*! For license information please see docsearch.f1a1a5835ed7a6ab0c85.js.LICENSE.txt */ ! function() {
     "use strict";
 
     function e(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
@@ -54,45 +54,45 @@
     function c(e, t) {
         return function(e) {
             if (Array.isArray(e)) return e
         }(e) || function(e, t) {
             var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
             if (null != n) {
                 var r, o, c = [],
-                    i = !0,
-                    a = !1;
+                    a = !0,
+                    i = !1;
                 try {
-                    for (n = n.call(e); !(i = (r = n.next()).done) && (c.push(r.value), !t || c.length !== t); i = !0);
+                    for (n = n.call(e); !(a = (r = n.next()).done) && (c.push(r.value), !t || c.length !== t); a = !0);
                 } catch (e) {
-                    a = !0, o = e
+                    i = !0, o = e
                 } finally {
                     try {
-                        i || null == n.return || n.return()
+                        a || null == n.return || n.return()
                     } finally {
-                        if (a) throw o
+                        if (i) throw o
                     }
                 }
                 return c
             }
-        }(e, t) || a(e, t) || function() {
+        }(e, t) || i(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function i(e) {
+    function a(e) {
         return function(e) {
             if (Array.isArray(e)) return u(e)
         }(e) || function(e) {
             if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
-        }(e) || a(e) || function() {
+        }(e) || i(e) || function() {
             throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function a(e, t) {
+    function i(e, t) {
         if (e) {
             if ("string" == typeof e) return u(e, t);
             var n = Object.prototype.toString.call(e).slice(8, -1);
             return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? u(e, t) : void 0
         }
     }
 
@@ -112,22 +112,22 @@
 
     function _(e) {
         var t = e.parentNode;
         t && t.removeChild(e)
     }
 
     function b(e, t, n) {
-        var r, o, c, i = arguments,
-            a = {};
-        for (c in t) "key" == c ? r = t[c] : "ref" == c ? o = t[c] : a[c] = t[c];
+        var r, o, c, a = arguments,
+            i = {};
+        for (c in t) "key" == c ? r = t[c] : "ref" == c ? o = t[c] : i[c] = t[c];
         if (arguments.length > 3)
-            for (n = [n], c = 3; c < arguments.length; c++) n.push(i[c]);
-        if (null != n && (a.children = n), "function" == typeof e && null != e.defaultProps)
-            for (c in e.defaultProps) void 0 === a[c] && (a[c] = e.defaultProps[c]);
-        return g(e, a, r, o, null)
+            for (n = [n], c = 3; c < arguments.length; c++) n.push(a[c]);
+        if (null != n && (i.children = n), "function" == typeof e && null != e.defaultProps)
+            for (c in e.defaultProps) void 0 === i[c] && (i[c] = e.defaultProps[c]);
+        return g(e, i, r, o, null)
     }
 
     function g(e, t, n, r, o) {
         var c = {
             type: e,
             props: t,
             key: n,
@@ -175,20 +175,20 @@
         (!e.__d && (e.__d = !0) && s.push(e) && !P.__r++ || p !== l.debounceRendering) && ((p = l.debounceRendering) || f)(P)
     }
 
     function P() {
         for (var e; P.__r = s.length;) e = s.sort((function(e, t) {
             return e.__v.__b - t.__v.__b
         })), s = [], e.some((function(e) {
-            var t, n, r, o, c, i;
-            e.__d && (c = (o = (t = e).__v).__e, (i = t.__P) && (n = [], (r = y({}, o)).__v = o.__v + 1, T(i, o, r, t.__n, void 0 !== i.ownerSVGElement, null != o.__h ? [c] : null, n, null == c ? E(o) : c, o.__h), L(n, o), o.__e != c && w(o)))
+            var t, n, r, o, c, a;
+            e.__d && (c = (o = (t = e).__v).__e, (a = t.__P) && (n = [], (r = y({}, o)).__v = o.__v + 1, T(a, o, r, t.__n, void 0 !== a.ownerSVGElement, null != o.__h ? [c] : null, n, null == c ? E(o) : c, o.__h), L(n, o), o.__e != c && w(o)))
         }))
     }
 
-    function I(e, t, n, r, o, c, i, a, u, l) {
+    function I(e, t, n, r, o, c, a, i, u, l) {
         var s, f, p, m, v, y, _, b = r && r.__k || h,
             S = b.length;
         for (n.__k = [], s = 0; s < t.length; s++)
             if (null != (m = n.__k[s] = null == (m = t[s]) || "boolean" == typeof m ? null : "string" == typeof m || "number" == typeof m ? g(null, m, null, null, m) : Array.isArray(m) ? g(O, {
                     children: m
                 }, null, null, null) : m.__b > 0 ? g(m.type, m.props, m.key, null, m.__v) : m)) {
                 if (m.__ = n, m.__b = n.__b + 1, null === (p = b[s]) || p && m.key == p.key && m.type === p.type) b[s] = void 0;
@@ -196,15 +196,15 @@
                     for (f = 0; f < S; f++) {
                         if ((p = b[f]) && m.key == p.key && m.type === p.type) {
                             b[f] = void 0;
                             break
                         }
                         p = null
                     }
-                T(e, m, p = p || d, o, c, i, a, u, l), v = m.__e, (f = m.ref) && p.ref != f && (_ || (_ = []), p.ref && _.push(p.ref, null, m), _.push(f, m.__c || v, m)), null != v ? (null == y && (y = v), "function" == typeof m.type && null != m.__k && m.__k === p.__k ? m.__d = u = k(m, u, e) : u = C(e, m, p, b, v, u), l || "option" !== n.type ? "function" == typeof n.type && (n.__d = u) : e.value = "") : u && p.__e == u && u.parentNode != e && (u = E(p))
+                T(e, m, p = p || d, o, c, a, i, u, l), v = m.__e, (f = m.ref) && p.ref != f && (_ || (_ = []), p.ref && _.push(p.ref, null, m), _.push(f, m.__c || v, m)), null != v ? (null == y && (y = v), "function" == typeof m.type && null != m.__k && m.__k === p.__k ? m.__d = u = k(m, u, e) : u = C(e, m, p, b, v, u), l || "option" !== n.type ? "function" == typeof n.type && (n.__d = u) : e.value = "") : u && p.__e == u && u.parentNode != e && (u = E(p))
             } for (n.__e = y, s = S; s--;) null != b[s] && ("function" == typeof n.type && null != b[s].__e && b[s].__e == n.__d && (n.__d = E(r, s + 1)), H(b[s], b[s]));
         if (_)
             for (s = 0; s < _.length; s++) M(_[s], _[++s], _[++s])
     }
 
     function k(e, t, n) {
         var r, o;
@@ -215,38 +215,38 @@
     function D(e, t) {
         return t = t || [], null == e || "boolean" == typeof e || (Array.isArray(e) ? e.some((function(e) {
             D(e, t)
         })) : t.push(e)), t
     }
 
     function C(e, t, n, r, o, c) {
-        var i, a, u;
-        if (void 0 !== t.__d) i = t.__d, t.__d = void 0;
-        else if (null == n || o != c || null == o.parentNode) e: if (null == c || c.parentNode !== e) e.appendChild(o), i = null;
+        var a, i, u;
+        if (void 0 !== t.__d) a = t.__d, t.__d = void 0;
+        else if (null == n || o != c || null == o.parentNode) e: if (null == c || c.parentNode !== e) e.appendChild(o), a = null;
             else {
-                for (a = c, u = 0;
-                    (a = a.nextSibling) && u < r.length; u += 2)
-                    if (a == o) break e;
-                e.insertBefore(o, c), i = c
-            } return void 0 !== i ? i : o.nextSibling
+                for (i = c, u = 0;
+                    (i = i.nextSibling) && u < r.length; u += 2)
+                    if (i == o) break e;
+                e.insertBefore(o, c), a = c
+            } return void 0 !== a ? a : o.nextSibling
     }
 
-    function A(e, t, n) {
+    function x(e, t, n) {
         "-" === t[0] ? e.setProperty(t, n) : e[t] = null == n ? "" : "number" != typeof n || v.test(t) ? n : n + "px"
     }
 
-    function x(e, t, n, r, o) {
+    function A(e, t, n, r, o) {
         var c;
         e: if ("style" === t)
             if ("string" == typeof n) e.style.cssText = n;
             else {
                 if ("string" == typeof r && (e.style.cssText = r = ""), r)
-                    for (t in r) n && t in n || A(e.style, t, "");
+                    for (t in r) n && t in n || x(e.style, t, "");
                 if (n)
-                    for (t in n) r && n[t] === r[t] || A(e.style, t, n[t])
+                    for (t in n) r && n[t] === r[t] || x(e.style, t, n[t])
             }
         else if ("o" === t[0] && "n" === t[1]) c = t !== (t = t.replace(/Capture$/, "")), t = t.toLowerCase() in e ? t.toLowerCase().slice(2) : t.slice(2), e.l || (e.l = {}), e.l[t + c] = n, n ? r || e.addEventListener(t, c ? R : N, c) : e.removeEventListener(t, c ? R : N, c);
         else if ("dangerouslySetInnerHTML" !== t) {
             if (o) t = t.replace(/xlink[H:h]/, "h").replace(/sName$/, "s");
             else if ("href" !== t && "list" !== t && "form" !== t && "download" !== t && t in e) try {
                 e[t] = null == n ? "" : n;
                 break e
@@ -259,36 +259,36 @@
         this.l[e.type + !1](l.event ? l.event(e) : e)
     }
 
     function R(e) {
         this.l[e.type + !0](l.event ? l.event(e) : e)
     }
 
-    function T(e, t, n, r, o, c, i, a, u) {
+    function T(e, t, n, r, o, c, a, i, u) {
         var s, f, p, m, d, h, v, _, b, g, E, w = t.type;
         if (void 0 !== t.constructor) return null;
-        null != n.__h && (u = n.__h, a = t.__e = n.__e, t.__h = null, c = [a]), (s = l.__b) && s(t);
+        null != n.__h && (u = n.__h, i = t.__e = n.__e, t.__h = null, c = [i]), (s = l.__b) && s(t);
         try {
             e: if ("function" == typeof w) {
                 if (_ = t.props, b = (s = w.contextType) && r[s.__c], g = s ? b ? b.props.value : s.__ : r, n.__c ? v = (f = t.__c = n.__c).__ = f.__E : ("prototype" in w && w.prototype.render ? t.__c = f = new w(_, g) : (t.__c = f = new S(_, g), f.constructor = w, f.render = U), b && b.sub(f), f.props = _, f.state || (f.state = {}), f.context = g, f.__n = r, p = f.__d = !0, f.__h = []), null == f.__s && (f.__s = f.state), null != w.getDerivedStateFromProps && (f.__s == f.state && (f.__s = y({}, f.__s)), y(f.__s, w.getDerivedStateFromProps(_, f.__s))), m = f.props, d = f.state, p) null == w.getDerivedStateFromProps && null != f.componentWillMount && f.componentWillMount(), null != f.componentDidMount && f.__h.push(f.componentDidMount);
                 else {
                     if (null == w.getDerivedStateFromProps && _ !== m && null != f.componentWillReceiveProps && f.componentWillReceiveProps(_, g), !f.__e && null != f.shouldComponentUpdate && !1 === f.shouldComponentUpdate(_, f.__s, g) || t.__v === n.__v) {
-                        f.props = _, f.state = f.__s, t.__v !== n.__v && (f.__d = !1), f.__v = t, t.__e = n.__e, t.__k = n.__k, f.__h.length && i.push(f);
+                        f.props = _, f.state = f.__s, t.__v !== n.__v && (f.__d = !1), f.__v = t, t.__e = n.__e, t.__k = n.__k, f.__h.length && a.push(f);
                         break e
                     }
                     null != f.componentWillUpdate && f.componentWillUpdate(_, f.__s, g), null != f.componentDidUpdate && f.__h.push((function() {
                         f.componentDidUpdate(m, d, h)
                     }))
                 }
-                f.context = g, f.props = _, f.state = f.__s, (s = l.__r) && s(t), f.__d = !1, f.__v = t, f.__P = e, s = f.render(f.props, f.state, f.context), f.state = f.__s, null != f.getChildContext && (r = y(y({}, r), f.getChildContext())), p || null == f.getSnapshotBeforeUpdate || (h = f.getSnapshotBeforeUpdate(m, d)), E = null != s && s.type === O && null == s.key ? s.props.children : s, I(e, Array.isArray(E) ? E : [E], t, n, r, o, c, i, a, u), f.base = t.__e, t.__h = null, f.__h.length && i.push(f), v && (f.__E = f.__ = null), f.__e = !1
-            } else null == c && t.__v === n.__v ? (t.__k = n.__k, t.__e = n.__e) : t.__e = q(n.__e, t, n, r, o, c, i, u);
+                f.context = g, f.props = _, f.state = f.__s, (s = l.__r) && s(t), f.__d = !1, f.__v = t, f.__P = e, s = f.render(f.props, f.state, f.context), f.state = f.__s, null != f.getChildContext && (r = y(y({}, r), f.getChildContext())), p || null == f.getSnapshotBeforeUpdate || (h = f.getSnapshotBeforeUpdate(m, d)), E = null != s && s.type === O && null == s.key ? s.props.children : s, I(e, Array.isArray(E) ? E : [E], t, n, r, o, c, a, i, u), f.base = t.__e, t.__h = null, f.__h.length && a.push(f), v && (f.__E = f.__ = null), f.__e = !1
+            } else null == c && t.__v === n.__v ? (t.__k = n.__k, t.__e = n.__e) : t.__e = q(n.__e, t, n, r, o, c, a, u);
             (s = l.diffed) && s(t)
         }
         catch (e) {
-            t.__v = null, (u || null != c) && (t.__e = a, t.__h = !!u, c[c.indexOf(a)] = null), l.__e(e, t, n)
+            t.__v = null, (u || null != c) && (t.__e = i, t.__h = !!u, c[c.indexOf(i)] = null), l.__e(e, t, n)
         }
     }
 
     function L(e, t) {
         l.__c && l.__c(t, e), e.some((function(t) {
             try {
                 e = t.__h, t.__h = [], e.some((function(e) {
@@ -296,43 +296,43 @@
                 }))
             } catch (e) {
                 l.__e(e, t.__v)
             }
         }))
     }
 
-    function q(e, t, n, r, o, c, i, a) {
+    function q(e, t, n, r, o, c, a, i) {
         var u, l, s, f, p = n.props,
             m = t.props,
             v = t.type,
             y = 0;
         if ("svg" === v && (o = !0), null != c)
             for (; y < c.length; y++)
                 if ((u = c[y]) && (u === e || (v ? u.localName == v : 3 == u.nodeType))) {
                     e = u, c[y] = null;
                     break
                 } if (null == e) {
             if (null === v) return document.createTextNode(m);
-            e = o ? document.createElementNS("http://www.w3.org/2000/svg", v) : document.createElement(v, m.is && m), c = null, a = !1
+            e = o ? document.createElementNS("http://www.w3.org/2000/svg", v) : document.createElement(v, m.is && m), c = null, i = !1
         }
-        if (null === v) p === m || a && e.data === m || (e.data = m);
+        if (null === v) p === m || i && e.data === m || (e.data = m);
         else {
-            if (c = c && h.slice.call(e.childNodes), l = (p = n.props || d).dangerouslySetInnerHTML, s = m.dangerouslySetInnerHTML, !a) {
+            if (c = c && h.slice.call(e.childNodes), l = (p = n.props || d).dangerouslySetInnerHTML, s = m.dangerouslySetInnerHTML, !i) {
                 if (null != c)
                     for (p = {}, f = 0; f < e.attributes.length; f++) p[e.attributes[f].name] = e.attributes[f].value;
                 (s || l) && (s && (l && s.__html == l.__html || s.__html === e.innerHTML) || (e.innerHTML = s && s.__html || ""))
             }
             if (function(e, t, n, r, o) {
                     var c;
-                    for (c in n) "children" === c || "key" === c || c in t || x(e, c, null, n[c], r);
-                    for (c in t) o && "function" != typeof t[c] || "children" === c || "key" === c || "value" === c || "checked" === c || n[c] === t[c] || x(e, c, t[c], n[c], r)
-                }(e, m, p, o, a), s) t.__k = [];
-            else if (y = t.props.children, I(e, Array.isArray(y) ? y : [y], t, n, r, o && "foreignObject" !== v, c, i, e.firstChild, a), null != c)
+                    for (c in n) "children" === c || "key" === c || c in t || A(e, c, null, n[c], r);
+                    for (c in t) o && "function" != typeof t[c] || "children" === c || "key" === c || "value" === c || "checked" === c || n[c] === t[c] || A(e, c, t[c], n[c], r)
+                }(e, m, p, o, i), s) t.__k = [];
+            else if (y = t.props.children, I(e, Array.isArray(y) ? y : [y], t, n, r, o && "foreignObject" !== v, c, a, e.firstChild, i), null != c)
                 for (y = c.length; y--;) null != c[y] && _(c[y]);
-            a || ("value" in m && void 0 !== (y = m.value) && (y !== e.value || "progress" === v && !y) && x(e, "value", y, p.value, !1), "checked" in m && void 0 !== (y = m.checked) && y !== e.checked && x(e, "checked", y, p.checked, !1))
+            i || ("value" in m && void 0 !== (y = m.value) && (y !== e.value || "progress" === v && !y) && A(e, "value", y, p.value, !1), "checked" in m && void 0 !== (y = m.checked) && y !== e.checked && A(e, "checked", y, p.checked, !1))
         }
         return e
     }
 
     function M(e, t, n) {
         try {
             "function" == typeof e ? e(t) : e.current = t
@@ -366,20 +366,20 @@
     }
 
     function B(e, t) {
         F(e, t, B)
     }
 
     function V(e, t, n) {
-        var r, o, c, i = arguments,
-            a = y({}, e.props);
-        for (c in t) "key" == c ? r = t[c] : "ref" == c ? o = t[c] : a[c] = t[c];
+        var r, o, c, a = arguments,
+            i = y({}, e.props);
+        for (c in t) "key" == c ? r = t[c] : "ref" == c ? o = t[c] : i[c] = t[c];
         if (arguments.length > 3)
-            for (n = [n], c = 3; c < arguments.length; c++) n.push(i[c]);
-        return null != n && (a.children = n), g(e.type, a, r || e.key, o || e.ref, null)
+            for (n = [n], c = 3; c < arguments.length; c++) n.push(a[c]);
+        return null != n && (i.children = n), g(e.type, i, r || e.key, o || e.ref, null)
     }
     l = {
         __e: function(e, t) {
             for (var n, r, o; t = t.__;)
                 if ((n = t.__c) && !n.__) try {
                     if ((r = n.constructor) && null != r.getDerivedStateFromError && (n.setState(r.getDerivedStateFromError(e)), o = n.__d), null != n.componentDidCatch && (n.componentDidCatch(e), o = n.__d), o) return n.__E = n
                 } catch (t) {
@@ -434,15 +434,15 @@
     }
 
     function ce(e, t) {
         var n = ee(W++, 7);
         return se(n.__H, t) && (n.__ = e(), n.__H = t, n.__h = e), n.__
     }
 
-    function ie() {
+    function ae() {
         $.forEach((function(e) {
             if (e.__P) try {
                 e.__H.__h.forEach(ue), e.__H.__h.forEach(le), e.__H.__h = []
             } catch (t) {
                 e.__H.__h = [], l.__e(t, e.__v)
             }
         })), $ = []
@@ -454,19 +454,19 @@
         var t = (K = e.__c).__H;
         t && (t.__h.forEach(ue), t.__h.forEach(le), t.__h = [])
     }, l.diffed = function(e) {
         Y && Y(e);
         var t = e.__c;
         t && t.__H && t.__H.__h.length && (1 !== $.push(t) && z === l.requestAnimationFrame || ((z = l.requestAnimationFrame) || function(e) {
             var t, n = function() {
-                    clearTimeout(r), ae && cancelAnimationFrame(t), setTimeout(e)
+                    clearTimeout(r), ie && cancelAnimationFrame(t), setTimeout(e)
                 },
                 r = setTimeout(n, 100);
-            ae && (t = requestAnimationFrame(n))
-        })(ie)), K = void 0
+            ie && (t = requestAnimationFrame(n))
+        })(ae)), K = void 0
     }, l.__c = function(e, t) {
         t.some((function(e) {
             try {
                 e.__h.forEach(ue), e.__h = e.__h.filter((function(e) {
                     return !e.__ || le(e)
                 }))
             } catch (n) {
@@ -480,15 +480,15 @@
         var t = e.__c;
         if (t && t.__H) try {
             t.__H.__.forEach(ue)
         } catch (e) {
             l.__e(e, t.__v)
         }
     };
-    var ae = "function" == typeof requestAnimationFrame;
+    var ie = "function" == typeof requestAnimationFrame;
 
     function ue(e) {
         var t = K;
         "function" == typeof e.__c && e.__c(), K = t
     }
 
     function le(e) {
@@ -566,21 +566,21 @@
         be(e, t, n)
     }, (ge.prototype = new S).__c = function(e, t) {
         var n = t.__c,
             r = this;
         null == r.t && (r.t = []), r.t.push(n);
         var o = Oe(r.__v),
             c = !1,
-            i = function() {
-                c || (c = !0, n.componentWillUnmount = n.__c, o ? o(a) : a())
+            a = function() {
+                c || (c = !0, n.componentWillUnmount = n.__c, o ? o(i) : i())
             };
         n.__c = n.componentWillUnmount, n.componentWillUnmount = function() {
-            i(), n.__c && n.__c()
+            a(), n.__c && n.__c()
         };
-        var a = function() {
+        var i = function() {
                 if (!--r.__u) {
                     if (r.state.__e) {
                         var e = r.state.__e;
                         r.__v.__k[0] = function e(t, n, r) {
                             return t && (t.__v = null, t.__k = t.__k && t.__k.map((function(t) {
                                 return e(t, n, r)
                             })), t.__c && t.__c.__P === n && (t.__e && r.insertBefore(t.__e, t.__d), t.__c.__e = !0, t.__c.__P = r)), t
@@ -591,15 +591,15 @@
                             __e: r.__b = null
                         }); t = r.t.pop();) t.forceUpdate()
                 }
             },
             u = !0 === t.__h;
         r.__u++ || u || r.setState({
             __e: r.__b = r.__v.__k[0]
-        }), e.then(i, i)
+        }), e.then(a, a)
     }, ge.prototype.componentWillUnmount = function() {
         this.t = []
     }, ge.prototype.render = function(e, t) {
         if (this.__b) {
             if (this.__v.__k) {
                 var n = document.createElement("div"),
                     r = this.__v.__k[0].__c;
@@ -702,27 +702,27 @@
                     configurable: !0,
                     writable: !0,
                     value: t
                 })
             }
         })
     }));
-    var Ae = l.event;
+    var xe = l.event;
 
-    function xe() {}
+    function Ae() {}
 
     function Ne() {
         return this.cancelBubble
     }
 
     function Re() {
         return this.defaultPrevented
     }
     l.event = function(e) {
-        return Ae && (e = Ae(e)), e.persist = xe, e.isPropagationStopped = Ne, e.isDefaultPrevented = Re, e.nativeEvent = e
+        return xe && (e = xe(e)), e.persist = Ae, e.isPropagationStopped = Ne, e.isDefaultPrevented = Re, e.nativeEvent = e
     };
     var Te, Le = {
             configurable: !0,
             get: function() {
                 return this.class
             }
         },
@@ -949,35 +949,35 @@
                 if (Object.getOwnPropertySymbols) {
                     var c = Object.getOwnPropertySymbols(e);
                     for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
                 }
                 return o
             }(e, We),
             c = r.buttonText,
-            i = void 0 === c ? "Search" : c,
-            a = r.buttonAriaLabel,
-            u = void 0 === a ? "Search" : a,
+            a = void 0 === c ? "Search" : c,
+            i = r.buttonAriaLabel,
+            u = void 0 === i ? "Search" : i,
             l = function(e, t) {
                 return function(e) {
                     if (Array.isArray(e)) return e
                 }(e) || function(e, t) {
                     var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                     if (null != n) {
                         var r, o, c = [],
-                            i = !0,
-                            a = !1;
+                            a = !0,
+                            i = !1;
                         try {
-                            for (n = n.call(e); !(i = (r = n.next()).done) && (c.push(r.value), 2 !== c.length); i = !0);
+                            for (n = n.call(e); !(a = (r = n.next()).done) && (c.push(r.value), 2 !== c.length); a = !0);
                         } catch (e) {
-                            a = !0, o = e
+                            i = !0, o = e
                         } finally {
                             try {
-                                i || null == n.return || n.return()
+                                a || null == n.return || n.return()
                             } finally {
-                                if (a) throw o
+                                if (i) throw o
                             }
                         }
                         return c
                     }
                 }(e) || function(e, t) {
                     if (e) {
                         if ("string" == typeof e) return ze(e, 2);
@@ -998,15 +998,15 @@
             "aria-label": u
         }, o, {
             ref: t
         }), Fe.createElement("span", {
             className: "DocSearch-Button-Container"
         }, Fe.createElement(Ve, null), Fe.createElement("span", {
             className: "DocSearch-Button-Placeholder"
-        }, i)), Fe.createElement("span", {
+        }, a)), Fe.createElement("span", {
             className: "DocSearch-Button-Keys"
         }, null !== s && Fe.createElement(Fe.Fragment, null, Fe.createElement("kbd", {
             className: "DocSearch-Button-Key"
         }, "Ctrl" === s ? Fe.createElement(Be, null) : s), Fe.createElement("kbd", {
             className: "DocSearch-Button-Key"
         }, "K"))))
     }));
@@ -1022,15 +1022,15 @@
         return 0 === e.collections.length ? 0 : e.collections.reduce((function(e, t) {
             return e + t.items.length
         }), 0)
     }
     var Ye = function() {},
         Ge = [{
             segment: "autocomplete-core",
-            version: "1.7.4"
+            version: "1.8.2"
         }];
 
     function Xe(e, t) {
         var n = t;
         return {
             then: function(t, r) {
                 return Xe(e.then(tt(t, n, e), tt(r, n, e)), n)
@@ -1083,44 +1083,56 @@
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function ot(e, t, n) {
+    function ot(e) {
+        for (var t = 1; t < arguments.length; t++) {
+            var n = null != arguments[t] ? arguments[t] : {};
+            t % 2 ? rt(Object(n), !0).forEach((function(t) {
+                ct(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : rt(Object(n)).forEach((function(t) {
+                Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
+            }))
+        }
+        return e
+    }
+
+    function ct(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function ct(e) {
+    function at(e) {
         var t = function(e) {
             var t = e.collections.map((function(e) {
                 return e.items.length
             })).reduce((function(e, t, n) {
                 var r = (e[n - 1] || 0) + t;
                 return e.push(r), e
             }), []).reduce((function(t, n) {
                 return n <= e.activeItemId ? t + 1 : t
             }), 0);
             return e.collections[t]
         }(e);
         if (!t) return null;
         var n = t.items[function(e) {
                 for (var t = e.state, n = e.collection, r = !1, o = 0, c = 0; !1 === r;) {
-                    var i = t.collections[o];
-                    if (i === n) {
+                    var a = t.collections[o];
+                    if (a === n) {
                         r = !0;
                         break
                     }
-                    c += i.items.length, o++
+                    c += a.items.length, o++
                 }
                 return t.activeItemId - c
             }({
                 state: e,
                 collection: t
             })],
             r = t.source;
@@ -1135,174 +1147,168 @@
                 state: e
             }),
             source: r
         }
     }
     var it = /((gt|sm)-|galaxy nexus)|samsung[- ]/i;
 
-    function at(e, t) {
+    function ut(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function ut(e) {
+    function lt(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? at(Object(n), !0).forEach((function(t) {
-                lt(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : at(Object(n)).forEach((function(t) {
+            t % 2 ? ut(Object(n), !0).forEach((function(t) {
+                st(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ut(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function lt(e, t, n) {
+    function st(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function st(e, t) {
+    function ft(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function ft(e, t, n) {
+    function pt(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function pt(e, t) {
+    function mt(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function mt(e) {
+    function dt(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? pt(Object(n), !0).forEach((function(t) {
-                dt(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : pt(Object(n)).forEach((function(t) {
+            t % 2 ? mt(Object(n), !0).forEach((function(t) {
+                ht(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : mt(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function dt(e, t, n) {
+    function ht(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function ht(e, t) {
+    function vt(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function vt(e, t) {
+    function yt(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function yt(e) {
+    function _t(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? vt(Object(n), !0).forEach((function(t) {
-                _t(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : vt(Object(n)).forEach((function(t) {
+            t % 2 ? yt(Object(n), !0).forEach((function(t) {
+                bt(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : yt(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function _t(e, t, n) {
+    function bt(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function bt(e, t) {
+    function gt(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function gt(e) {
+    function Ot(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? bt(Object(n), !0).forEach((function(t) {
-                Ot(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : bt(Object(n)).forEach((function(t) {
+            t % 2 ? gt(Object(n), !0).forEach((function(t) {
+                St(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : gt(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Ot(e, t, n) {
+    function St(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function St(e, t) {
-        (null == t || t > e.length) && (t = e.length);
-        for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
-        return r
-    }
-
     function Et(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
@@ -1328,198 +1334,215 @@
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
     function Pt(e) {
+        return function(e) {
+            if (Array.isArray(e)) return It(e)
+        }(e) || function(e) {
+            if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
+        }(e) || function(e, t) {
+            if (e) {
+                if ("string" == typeof e) return It(e, t);
+                var n = Object.prototype.toString.call(e).slice(8, -1);
+                return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? It(e, t) : void 0
+            }
+        }(e) || function() {
+            throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
+        }()
+    }
+
+    function It(e, t) {
+        (null == t || t > e.length) && (t = e.length);
+        for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
+        return r
+    }
+
+    function kt(e) {
         return Boolean(e.execute)
     }
 
-    function It(e) {
+    function Dt(e) {
         var t = e.reduce((function(e, t) {
-            if (!Pt(t)) return e.push(t), e;
+            if (!kt(t)) return e.push(t), e;
             var n = t.searchClient,
                 r = t.execute,
                 o = t.requesterId,
                 c = t.requests,
-                i = e.find((function(e) {
-                    return Pt(t) && Pt(e) && e.searchClient === n && Boolean(o) && e.requesterId === o
+                a = e.find((function(e) {
+                    return kt(t) && kt(e) && e.searchClient === n && Boolean(o) && e.requesterId === o
                 }));
-            if (i) {
-                var a;
-                (a = i.items).push.apply(a, function(e) {
-                    return function(e) {
-                        if (Array.isArray(e)) return St(e)
-                    }(e) || function(e) {
-                        if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
-                    }(e) || function(e, t) {
-                        if (e) {
-                            if ("string" == typeof e) return St(e, t);
-                            var n = Object.prototype.toString.call(e).slice(8, -1);
-                            return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? St(e, t) : void 0
-                        }
-                    }(e) || function() {
-                        throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
-                    }()
-                }(c))
+            if (a) {
+                var i;
+                (i = a.items).push.apply(i, Pt(c))
             } else {
                 var u = {
                     execute: r,
                     requesterId: o,
                     items: c,
                     searchClient: n
                 };
                 e.push(u)
             }
             return e
         }), []).map((function(e) {
-            if (!Pt(e)) return Promise.resolve(e);
+            if (!kt(e)) return Promise.resolve(e);
             var t = e,
                 n = t.execute,
                 r = t.items;
             return n({
                 searchClient: t.searchClient,
                 requests: r
             })
         }));
         return Promise.all(t).then((function(e) {
             return $e(e)
         }))
     }
-    var kt = ["event", "nextState", "props", "query", "refresh", "store"];
+    var Ct = ["event", "nextState", "props", "query", "refresh", "store"];
 
-    function Dt(e, t) {
+    function xt(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Ct(e) {
+    function At(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Dt(Object(n), !0).forEach((function(t) {
-                At(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Dt(Object(n)).forEach((function(t) {
+            t % 2 ? xt(Object(n), !0).forEach((function(t) {
+                Nt(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : xt(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function At(e, t, n) {
+    function Nt(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
-    var xt, Nt, Rt, Tt = null,
-        Lt = (xt = -1, Nt = -1, Rt = void 0, function(e) {
-            var t = ++xt;
+    var Rt, Tt, Lt, qt = null,
+        Mt = (Rt = -1, Tt = -1, Lt = void 0, function(e) {
+            var t = ++Rt;
             return Promise.resolve(e).then((function(e) {
-                return Rt && t < Nt ? Rt : (Nt = t, Rt = e, e)
+                return Lt && t < Tt ? Lt : (Tt = t, Lt = e, e)
             }))
         });
 
-    function qt(e) {
+    function Ht(e) {
         var t = e.event,
             n = e.nextState,
             r = void 0 === n ? {} : n,
             o = e.props,
             c = e.query,
-            i = e.refresh,
-            a = e.store,
+            a = e.refresh,
+            i = e.store,
             u = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = function(e, t) {
                     if (null == e) return {};
                     var n, r, o = {},
                         c = Object.keys(e);
                     for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                     return o
                 }(e, t);
                 if (Object.getOwnPropertySymbols) {
                     var c = Object.getOwnPropertySymbols(e);
                     for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
                 }
                 return o
-            }(e, kt);
-        Tt && o.environment.clearTimeout(Tt);
+            }(e, Ct);
+        qt && o.environment.clearTimeout(qt);
         var l = u.setCollections,
             s = u.setIsOpen,
             f = u.setQuery,
             p = u.setActiveItemId,
             m = u.setStatus;
         if (f(c), p(o.defaultActiveItemId), !c && !1 === o.openOnFocus) {
-            var d, h = a.getState().collections.map((function(e) {
-                return Ct(Ct({}, e), {}, {
+            var d, h = i.getState().collections.map((function(e) {
+                return At(At({}, e), {}, {
                     items: []
                 })
             }));
             m("idle"), l(h), s(null !== (d = r.isOpen) && void 0 !== d ? d : o.shouldPanelOpen({
-                state: a.getState()
+                state: i.getState()
             }));
-            var v = et(Lt(h).then((function() {
+            var v = et(Mt(h).then((function() {
                 return Promise.resolve()
             })));
-            return a.pendingRequests.add(v)
+            return i.pendingRequests.add(v)
         }
-        m("loading"), Tt = o.environment.setTimeout((function() {
+        m("loading"), qt = o.environment.setTimeout((function() {
             m("stalled")
         }), o.stallThreshold);
-        var y = et(Lt(o.getSources(Ct({
+        var y = et(Mt(o.getSources(At({
             query: c,
-            refresh: i,
-            state: a.getState()
+            refresh: a,
+            state: i.getState()
         }, u)).then((function(e) {
             return Promise.all(e.map((function(e) {
-                return Promise.resolve(e.getItems(Ct({
+                return Promise.resolve(e.getItems(At({
                     query: c,
-                    refresh: i,
-                    state: a.getState()
+                    refresh: a,
+                    state: i.getState()
                 }, u))).then((function(t) {
-                    return function(e, t) {
-                        return n = e, Boolean(null == n ? void 0 : n.execute) ? wt(wt({}, e), {}, {
-                            requests: e.queries.map((function(n) {
-                                return {
-                                    query: n,
-                                    sourceId: t,
-                                    transformResponse: e.transformResponse
-                                }
-                            }))
-                        }) : {
+                    return function(e, t, n) {
+                        if (o = e, Boolean(null == o ? void 0 : o.execute)) {
+                            var r = "algolia" === e.requesterId ? Object.assign.apply(Object, [{}].concat(Pt(Object.keys(n.context).map((function(e) {
+                                var t;
+                                return null === (t = n.context[e]) || void 0 === t ? void 0 : t.__algoliaSearchParameters
+                            }))))) : {};
+                            return wt(wt({}, e), {}, {
+                                requests: e.queries.map((function(n) {
+                                    return {
+                                        query: "algolia" === e.requesterId ? wt(wt({}, n), {}, {
+                                            params: wt(wt({}, r), n.params)
+                                        }) : n,
+                                        sourceId: t,
+                                        transformResponse: e.transformResponse
+                                    }
+                                }))
+                            })
+                        }
+                        var o;
+                        return {
                             items: e,
                             sourceId: t
-                        };
-                        var n
-                    }(t, e.sourceId)
+                        }
+                    }(t, e.sourceId, i.getState())
                 }))
-            }))).then(It).then((function(t) {
-                return function(e, t) {
+            }))).then(Dt).then((function(t) {
+                return function(e, t, n) {
                     return t.map((function(t) {
-                        var n = e.filter((function(e) {
+                        var r = e.filter((function(e) {
                                 return e.sourceId === t.sourceId
                             })),
-                            r = n.map((function(e) {
+                            o = r.map((function(e) {
                                 return e.items
                             })),
-                            o = n[0].transformResponse,
-                            c = o ? o(function(e) {
+                            c = r[0].transformResponse,
+                            a = c ? c(function(e) {
                                 var t = e.map((function(e) {
                                     var t;
-                                    return ut(ut({}, e), {}, {
+                                    return lt(lt({}, e), {}, {
                                         hits: null === (t = e.hits) || void 0 === t ? void 0 : t.map((function(t) {
-                                            return ut(ut({}, t), {}, {
+                                            return lt(lt({}, t), {}, {
                                                 __autocomplete_indexName: e.index,
                                                 __autocomplete_queryID: e.queryID
                                             })
                                         }))
                                     })
                                 }));
                                 return {
@@ -1538,148 +1561,161 @@
                                                         value: e.highlighted
                                                     }
                                                 }
                                             }
                                         }))
                                     })).filter(Boolean)
                                 }
-                            }(r)) : r;
-                        return Array.isArray(c), c.every(Boolean), 'The `getItems` function from source "'.concat(t.sourceId, '" must return an array of items but returned ').concat(JSON.stringify(void 0), ".\n\nDid you forget to return items?\n\nSee: https://www.algolia.com/doc/ui-libraries/autocomplete/core-concepts/sources/#param-getitems"), {
+                            }(o)) : o;
+                        return t.onResolve({
+                            source: t,
+                            results: o,
+                            items: a,
+                            state: n.getState()
+                        }), Array.isArray(a), a.every(Boolean), 'The `getItems` function from source "'.concat(t.sourceId, '" must return an array of items but returned ').concat(JSON.stringify(void 0), ".\n\nDid you forget to return items?\n\nSee: https://www.algolia.com/doc/ui-libraries/autocomplete/core-concepts/sources/#param-getitems"), {
                             source: t,
-                            items: c
+                            items: a
                         }
                     }))
-                }(t, e)
+                }(t, e, i)
             })).then((function(e) {
                 return function(e) {
                     var t = e.props,
                         n = e.state,
                         r = e.collections.reduce((function(e, t) {
-                            return gt(gt({}, e), {}, Ot({}, t.source.sourceId, gt(gt({}, t.source), {}, {
+                            return Ot(Ot({}, e), {}, St({}, t.source.sourceId, Ot(Ot({}, t.source), {}, {
                                 getItems: function() {
                                     return $e(t.items)
                                 }
                             })))
-                        }), {});
+                        }), {}),
+                        o = t.plugins.reduce((function(e, t) {
+                            return t.reshape ? t.reshape(e) : e
+                        }), {
+                            sourcesBySourceId: r,
+                            state: n
+                        }).sourcesBySourceId;
                     return $e(t.reshape({
-                        sources: Object.values(r),
-                        sourcesBySourceId: r,
+                        sourcesBySourceId: o,
+                        sources: Object.values(o),
                         state: n
                     })).filter(Boolean).map((function(e) {
                         return {
                             source: e,
                             items: e.getItems()
                         }
                     }))
                 }({
                     collections: e,
                     props: o,
-                    state: a.getState()
+                    state: i.getState()
                 })
             }))
         })))).then((function(e) {
             var n;
             m("idle"), l(e);
             var f = o.shouldPanelOpen({
-                state: a.getState()
+                state: i.getState()
             });
             s(null !== (n = r.isOpen) && void 0 !== n ? n : o.openOnFocus && !c && f || f);
-            var p = ct(a.getState());
-            if (null !== a.getState().activeItemId && p) {
+            var p = at(i.getState());
+            if (null !== i.getState().activeItemId && p) {
                 var d = p.item,
                     h = p.itemInputValue,
                     v = p.itemUrl,
                     y = p.source;
-                y.onActive(Ct({
+                y.onActive(At({
                     event: t,
                     item: d,
                     itemInputValue: h,
                     itemUrl: v,
-                    refresh: i,
+                    refresh: a,
                     source: y,
-                    state: a.getState()
+                    state: i.getState()
                 }, u))
             }
         })).finally((function() {
-            m("idle"), Tt && o.environment.clearTimeout(Tt)
+            m("idle"), qt && o.environment.clearTimeout(qt)
         }));
-        return a.pendingRequests.add(y)
+        return i.pendingRequests.add(y)
     }
-    var Mt = ["event", "props", "refresh", "store"];
+    var Ut = ["event", "props", "refresh", "store"];
 
-    function Ht(e, t) {
+    function Ft(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Ut(e) {
+    function Bt(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Ht(Object(n), !0).forEach((function(t) {
-                Ft(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ht(Object(n)).forEach((function(t) {
+            t % 2 ? Ft(Object(n), !0).forEach((function(t) {
+                Vt(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Ft(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Ft(e, t, n) {
+    function Vt(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
-    var Bt = ["props", "refresh", "store"],
-        Vt = ["inputElement", "formElement", "panelElement"],
-        Wt = ["inputElement"],
-        Kt = ["inputElement", "maxLength"],
-        zt = ["item", "source"];
+    var Wt = ["props", "refresh", "store"],
+        Kt = ["inputElement", "formElement", "panelElement"],
+        zt = ["inputElement"],
+        Jt = ["inputElement", "maxLength"],
+        $t = ["sourceIndex"],
+        Qt = ["sourceIndex"],
+        Zt = ["item", "source", "sourceIndex"];
 
-    function Jt(e, t) {
+    function Yt(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function $t(e) {
+    function Gt(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Jt(Object(n), !0).forEach((function(t) {
-                Qt(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Jt(Object(n)).forEach((function(t) {
+            t % 2 ? Yt(Object(n), !0).forEach((function(t) {
+                Xt(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Yt(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Qt(e, t, n) {
+    function Xt(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function Zt(e, t) {
+    function en(e, t) {
         if (null == e) return {};
         var n, r, o = function(e, t) {
             if (null == e) return {};
             var n, r, o = {},
                 c = Object.keys(e);
             for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
             return o
@@ -1687,229 +1723,229 @@
         if (Object.getOwnPropertySymbols) {
             var c = Object.getOwnPropertySymbols(e);
             for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
 
-    function Yt(e, t) {
+    function tn(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Gt(e) {
+    function nn(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Yt(Object(n), !0).forEach((function(t) {
-                Xt(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Yt(Object(n)).forEach((function(t) {
+            t % 2 ? tn(Object(n), !0).forEach((function(t) {
+                rn(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : tn(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Xt(e, t, n) {
+    function rn(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function en(e) {
+    function on(e) {
         var t, n, r, o, c = e.plugins,
-            i = e.options,
-            a = null === (t = ((null === (n = i.__autocomplete_metadata) || void 0 === n ? void 0 : n.userAgents) || [])[0]) || void 0 === t ? void 0 : t.segment,
-            u = a ? Xt({}, a, Object.keys((null === (r = i.__autocomplete_metadata) || void 0 === r ? void 0 : r.options) || {})) : {};
+            a = e.options,
+            i = null === (t = ((null === (n = a.__autocomplete_metadata) || void 0 === n ? void 0 : n.userAgents) || [])[0]) || void 0 === t ? void 0 : t.segment,
+            u = i ? rn({}, i, Object.keys((null === (r = a.__autocomplete_metadata) || void 0 === r ? void 0 : r.options) || {})) : {};
         return {
             plugins: c.map((function(e) {
                 return {
                     name: e.name,
                     options: Object.keys(e.__autocomplete_pluginOptions || [])
                 }
             })),
-            options: Gt({
-                "autocomplete-core": Object.keys(i)
+            options: nn({
+                "autocomplete-core": Object.keys(a)
             }, u),
-            ua: Ge.concat((null === (o = i.__autocomplete_metadata) || void 0 === o ? void 0 : o.userAgents) || [])
+            ua: Ge.concat((null === (o = a.__autocomplete_metadata) || void 0 === o ? void 0 : o.userAgents) || [])
         }
     }
 
-    function tn(e) {
+    function cn(e) {
         var t, n = e.state;
-        return !1 === n.isOpen || null === n.activeItemId ? null : (null === (t = ct(n)) || void 0 === t ? void 0 : t.itemInputValue) || null
+        return !1 === n.isOpen || null === n.activeItemId ? null : (null === (t = at(n)) || void 0 === t ? void 0 : t.itemInputValue) || null
     }
 
-    function nn(e, t) {
+    function an(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function rn(e) {
+    function un(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? nn(Object(n), !0).forEach((function(t) {
-                on(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : nn(Object(n)).forEach((function(t) {
+            t % 2 ? an(Object(n), !0).forEach((function(t) {
+                ln(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : an(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function on(e, t, n) {
+    function ln(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
-    var cn = function(e, t) {
+    var sn = function(e, t) {
         switch (t.type) {
             case "setActiveItemId":
             case "mousemove":
-                return rn(rn({}, e), {}, {
+                return un(un({}, e), {}, {
                     activeItemId: t.payload
                 });
             case "setQuery":
-                return rn(rn({}, e), {}, {
+                return un(un({}, e), {}, {
                     query: t.payload,
                     completion: null
                 });
             case "setCollections":
-                return rn(rn({}, e), {}, {
+                return un(un({}, e), {}, {
                     collections: t.payload
                 });
             case "setIsOpen":
-                return rn(rn({}, e), {}, {
+                return un(un({}, e), {}, {
                     isOpen: t.payload
                 });
             case "setStatus":
-                return rn(rn({}, e), {}, {
+                return un(un({}, e), {}, {
                     status: t.payload
                 });
             case "setContext":
-                return rn(rn({}, e), {}, {
-                    context: rn(rn({}, e.context), t.payload)
+                return un(un({}, e), {}, {
+                    context: un(un({}, e.context), t.payload)
                 });
             case "ArrowDown":
-                var n = rn(rn({}, e), {}, {
+                var n = un(un({}, e), {}, {
                     activeItemId: t.payload.hasOwnProperty("nextActiveItemId") ? t.payload.nextActiveItemId : nt(1, e.activeItemId, Ze(e), t.props.defaultActiveItemId)
                 });
-                return rn(rn({}, n), {}, {
-                    completion: tn({
+                return un(un({}, n), {}, {
+                    completion: cn({
                         state: n
                     })
                 });
             case "ArrowUp":
-                var r = rn(rn({}, e), {}, {
+                var r = un(un({}, e), {}, {
                     activeItemId: nt(-1, e.activeItemId, Ze(e), t.props.defaultActiveItemId)
                 });
-                return rn(rn({}, r), {}, {
-                    completion: tn({
+                return un(un({}, r), {}, {
+                    completion: cn({
                         state: r
                     })
                 });
             case "Escape":
-                return e.isOpen ? rn(rn({}, e), {}, {
+                return e.isOpen ? un(un({}, e), {}, {
                     activeItemId: null,
                     isOpen: !1,
                     completion: null
-                }) : rn(rn({}, e), {}, {
+                }) : un(un({}, e), {}, {
                     activeItemId: null,
                     query: "",
                     status: "idle",
                     collections: []
                 });
             case "submit":
-                return rn(rn({}, e), {}, {
+                return un(un({}, e), {}, {
                     activeItemId: null,
                     isOpen: !1,
                     status: "idle"
                 });
             case "reset":
-                return rn(rn({}, e), {}, {
+                return un(un({}, e), {}, {
                     activeItemId: !0 === t.props.openOnFocus ? t.props.defaultActiveItemId : null,
                     status: "idle",
                     query: ""
                 });
             case "focus":
-                return rn(rn({}, e), {}, {
+                return un(un({}, e), {}, {
                     activeItemId: t.props.defaultActiveItemId,
                     isOpen: (t.props.openOnFocus || Boolean(e.query)) && t.props.shouldPanelOpen({
                         state: e
                     })
                 });
             case "blur":
-                return t.props.debug ? e : rn(rn({}, e), {}, {
+                return t.props.debug ? e : un(un({}, e), {}, {
                     isOpen: !1,
                     activeItemId: null
                 });
             case "mouseleave":
-                return rn(rn({}, e), {}, {
+                return un(un({}, e), {}, {
                     activeItemId: t.props.defaultActiveItemId
                 });
             default:
                 return "The reducer action ".concat(JSON.stringify(t.type), " is not supported."), e
         }
     };
 
-    function an(e, t) {
+    function fn(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function un(e) {
+    function pn(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? an(Object(n), !0).forEach((function(t) {
-                ln(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : an(Object(n)).forEach((function(t) {
+            t % 2 ? fn(Object(n), !0).forEach((function(t) {
+                mn(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : fn(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function ln(e, t, n) {
+    function mn(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function sn(e) {
+    function dn(e) {
         var t = [],
             n = function(e, t) {
                 var n, r = "undefined" != typeof window ? window : {},
                     o = e.plugins || [];
-                return yt(yt({
+                return _t(_t({
                     debug: !1,
                     openOnFocus: !1,
                     placeholder: "",
                     autoFocus: !1,
                     defaultActiveItemId: null,
                     stallThreshold: 300,
                     environment: r,
@@ -1918,15 +1954,15 @@
                     },
                     reshape: function(e) {
                         return e.sources
                     }
                 }, e), {}, {
                     id: null !== (n = e.id) && void 0 !== n ? n : "autocomplete-".concat(Qe++),
                     plugins: o,
-                    initialState: yt({
+                    initialState: _t({
                         activeItemId: null,
                         query: "",
                         completion: null,
                         collections: [],
                         isOpen: !1,
                         status: "idle",
                         context: {}
@@ -1951,22 +1987,22 @@
                             var n;
                             return null === (n = e.onReset) || void 0 === n ? void 0 : n.call(e, t)
                         }))
                     },
                     getSources: function(n) {
                         return Promise.all([].concat(function(e) {
                             return function(e) {
-                                if (Array.isArray(e)) return ht(e)
+                                if (Array.isArray(e)) return vt(e)
                             }(e) || function(e) {
                                 if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
                             }(e) || function(e, t) {
                                 if (e) {
-                                    if ("string" == typeof e) return ht(e, t);
+                                    if ("string" == typeof e) return vt(e, t);
                                     var n = Object.prototype.toString.call(e).slice(8, -1);
-                                    return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? ht(e, t) : void 0
+                                    return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? vt(e, t) : void 0
                                 }
                             }(e) || function() {
                                 throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                             }()
                         }(o.map((function(e) {
                             return e.getSources
                         }))), [e.getSources]).filter(Boolean).map((function(e) {
@@ -1974,60 +2010,61 @@
                                 var n = [];
                                 return Promise.resolve(e(t)).then((function(e) {
                                     return Array.isArray(e), Promise.all(e.filter((function(e) {
                                         return Boolean(e)
                                     })).map((function(e) {
                                         if (e.sourceId, n.includes(e.sourceId)) throw new Error("[Autocomplete] The `sourceId` ".concat(JSON.stringify(e.sourceId), " is not unique."));
                                         n.push(e.sourceId);
-                                        var t = function(e) {
-                                            for (var t = 1; t < arguments.length; t++) {
-                                                var n = null != arguments[t] ? arguments[t] : {};
-                                                t % 2 ? rt(Object(n), !0).forEach((function(t) {
-                                                    ot(e, t, n[t])
-                                                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : rt(Object(n)).forEach((function(t) {
-                                                    Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
-                                                }))
-                                            }
-                                            return e
-                                        }({
+                                        var t = {
                                             getItemInputValue: function(e) {
                                                 return e.state.query
                                             },
                                             getItemUrl: function() {},
                                             onSelect: function(e) {
                                                 (0, e.setIsOpen)(!1)
                                             },
-                                            onActive: Ye
-                                        }, e);
-                                        return Promise.resolve(t)
+                                            onActive: Ye,
+                                            onResolve: Ye
+                                        };
+                                        Object.keys(t).forEach((function(e) {
+                                            t[e].__default = !0
+                                        }));
+                                        var r = ot(ot({}, t), e);
+                                        return Promise.resolve(r)
                                     })))
                                 }))
                             }(e, n)
                         }))).then((function(e) {
                             return $e(e)
                         })).then((function(e) {
                             return e.map((function(e) {
-                                return yt(yt({}, e), {}, {
+                                return _t(_t({}, e), {}, {
                                     onSelect: function(n) {
                                         e.onSelect(n), t.forEach((function(e) {
                                             var t;
                                             return null === (t = e.onSelect) || void 0 === t ? void 0 : t.call(e, n)
                                         }))
                                     },
                                     onActive: function(n) {
                                         e.onActive(n), t.forEach((function(e) {
                                             var t;
                                             return null === (t = e.onActive) || void 0 === t ? void 0 : t.call(e, n)
                                         }))
+                                    },
+                                    onResolve: function(n) {
+                                        e.onResolve(n), t.forEach((function(e) {
+                                            var t;
+                                            return null === (t = e.onResolve) || void 0 === t ? void 0 : t.call(e, n)
+                                        }))
                                     }
                                 })
                             }))
                         }))
                     },
-                    navigator: yt({
+                    navigator: _t({
                         navigate: function(e) {
                             var t = e.itemUrl;
                             r.location.assign(t)
                         },
                         navigateNewTab: function(e) {
                             var t = e.itemUrl,
                                 n = r.open(t, "_blank", "noopener");
@@ -2043,32 +2080,32 @@
             r = function(e, t, n) {
                 var r, o = t.initialState;
                 return {
                     getState: function() {
                         return o
                     },
                     dispatch: function(r, c) {
-                        var i = function(e) {
+                        var a = function(e) {
                             for (var t = 1; t < arguments.length; t++) {
                                 var n = null != arguments[t] ? arguments[t] : {};
-                                t % 2 ? st(Object(n), !0).forEach((function(t) {
-                                    ft(e, t, n[t])
-                                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : st(Object(n)).forEach((function(t) {
+                                t % 2 ? ft(Object(n), !0).forEach((function(t) {
+                                    pt(e, t, n[t])
+                                })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : ft(Object(n)).forEach((function(t) {
                                     Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                                 }))
                             }
                             return e
                         }({}, o);
                         o = e(o, {
                             type: r,
                             props: t,
                             payload: c
                         }), n({
                             state: o,
-                            prevState: i
+                            prevState: a
                         })
                     },
                     pendingRequests: (r = [], {
                         add: function(e) {
                             return r.push(e), e.finally((function() {
                                 r = r.filter((function(t) {
                                     return t !== e
@@ -2081,38 +2118,39 @@
                             }))
                         },
                         isEmpty: function() {
                             return 0 === r.length
                         }
                     })
                 }
-            }(cn, n, (function(e) {
+            }(sn, n, (function(e) {
                 var t = e.prevState,
                     r = e.state;
-                n.onStateChange(un({
+                n.onStateChange(pn({
                     prevState: t,
                     state: r,
-                    refresh: i
+                    refresh: a,
+                    navigator: n.navigator
                 }, o))
             })),
             o = function(e) {
                 var t = e.store;
                 return {
                     setActiveItemId: function(e) {
                         t.dispatch("setActiveItemId", e)
                     },
                     setQuery: function(e) {
                         t.dispatch("setQuery", e)
                     },
                     setCollections: function(e) {
                         var n = 0,
                             r = e.map((function(e) {
-                                return mt(mt({}, e), {}, {
+                                return dt(dt({}, e), {}, {
                                     items: $e(e.items).map((function(e) {
-                                        return mt(mt({}, e), {}, {
+                                        return dt(dt({}, e), {}, {
                                             __autocomplete_id: n++
                                         })
                                     }))
                                 })
                             }));
                         t.dispatch("setCollections", r)
                     },
@@ -2129,95 +2167,101 @@
             }({
                 store: r
             }),
             c = function(e) {
                 var t = e.props,
                     n = e.refresh,
                     r = e.store,
-                    o = Zt(e, Bt);
+                    o = en(e, Wt),
+                    c = function(e, t) {
+                        return void 0 !== t ? "".concat(e, "-").concat(t) : e
+                    };
                 return {
                     getEnvironmentProps: function(e) {
                         var n = e.inputElement,
                             o = e.formElement,
                             c = e.panelElement;
 
-                        function i(e) {
+                        function a(e) {
                             !r.getState().isOpen && r.pendingRequests.isEmpty() || e.target === n || !1 === [o, c].some((function(t) {
                                 return (n = t) === (r = e.target) || n.contains(r);
                                 var n, r
                             })) && (r.dispatch("blur", null), t.debug || r.pendingRequests.cancelAll())
                         }
-                        return $t({
-                            onTouchStart: i,
-                            onMouseDown: i,
+                        return Gt({
+                            onTouchStart: a,
+                            onMouseDown: a,
                             onTouchMove: function(e) {
                                 !1 !== r.getState().isOpen && n === t.environment.document.activeElement && e.target !== n && n.blur()
                             }
-                        }, Zt(e, Vt))
+                        }, en(e, Kt))
                     },
                     getRootProps: function(e) {
-                        return $t({
+                        return Gt({
                             role: "combobox",
                             "aria-expanded": r.getState().isOpen,
                             "aria-haspopup": "listbox",
                             "aria-owns": r.getState().isOpen ? "".concat(t.id, "-list") : void 0,
                             "aria-labelledby": "".concat(t.id, "-label")
                         }, e)
                     },
                     getFormProps: function(e) {
-                        return e.inputElement, $t({
+                        return e.inputElement, Gt({
                             action: "",
                             noValidate: !0,
                             role: "search",
                             onSubmit: function(c) {
-                                var i;
-                                c.preventDefault(), t.onSubmit($t({
+                                var a;
+                                c.preventDefault(), t.onSubmit(Gt({
                                     event: c,
                                     refresh: n,
                                     state: r.getState()
-                                }, o)), r.dispatch("submit", null), null === (i = e.inputElement) || void 0 === i || i.blur()
+                                }, o)), r.dispatch("submit", null), null === (a = e.inputElement) || void 0 === a || a.blur()
                             },
                             onReset: function(c) {
-                                var i;
-                                c.preventDefault(), t.onReset($t({
+                                var a;
+                                c.preventDefault(), t.onReset(Gt({
                                     event: c,
                                     refresh: n,
                                     state: r.getState()
-                                }, o)), r.dispatch("reset", null), null === (i = e.inputElement) || void 0 === i || i.focus()
+                                }, o)), r.dispatch("reset", null), null === (a = e.inputElement) || void 0 === a || a.focus()
                             }
-                        }, Zt(e, Wt))
+                        }, en(e, zt))
                     },
                     getLabelProps: function(e) {
-                        return $t({
-                            htmlFor: "".concat(t.id, "-input"),
-                            id: "".concat(t.id, "-label")
-                        }, e)
+                        var n = e || {},
+                            r = n.sourceIndex,
+                            o = en(n, $t);
+                        return Gt({
+                            htmlFor: "".concat(c(t.id, r), "-input"),
+                            id: "".concat(c(t.id, r), "-label")
+                        }, o)
                     },
                     getInputProps: function(e) {
                         var c;
 
-                        function i(e) {
-                            (t.openOnFocus || Boolean(r.getState().query)) && qt($t({
+                        function a(e) {
+                            (t.openOnFocus || Boolean(r.getState().query)) && Ht(Gt({
                                 event: e,
                                 props: t,
                                 query: r.getState().completion || r.getState().query,
                                 refresh: n,
                                 store: r
                             }, o)), r.dispatch("focus", null)
                         }
-                        var a = e || {},
-                            u = (a.inputElement, a.maxLength),
+                        var i = e || {},
+                            u = (i.inputElement, i.maxLength),
                             l = void 0 === u ? 512 : u,
-                            s = Zt(a, Kt),
-                            f = ct(r.getState()),
+                            s = en(i, Jt),
+                            f = at(r.getState()),
                             p = function(e) {
                                 return Boolean(e && e.match(it))
                             }((null === (c = t.environment.navigator) || void 0 === c ? void 0 : c.userAgent) || ""),
                             m = null != f && f.itemUrl && !p ? "go" : "search";
-                        return $t({
+                        return Gt({
                             "aria-autocomplete": "both",
                             "aria-activedescendant": r.getState().isOpen && null !== r.getState().activeItemId ? "".concat(t.id, "-item-").concat(r.getState().activeItemId) : void 0,
                             "aria-controls": r.getState().isOpen ? "".concat(t.id, "-list") : void 0,
                             "aria-labelledby": "".concat(t.id, "-label"),
                             value: r.getState().completion || r.getState().query,
                             id: "".concat(t.id, "-input"),
                             autoComplete: "off",
@@ -2226,15 +2270,15 @@
                             enterKeyHint: m,
                             spellCheck: "false",
                             autoFocus: t.autoFocus,
                             placeholder: t.placeholder,
                             maxLength: l,
                             type: "search",
                             onChange: function(e) {
-                                qt($t({
+                                Ht(Gt({
                                     event: e,
                                     props: t,
                                     query: e.currentTarget.value.slice(0, l),
                                     refresh: n,
                                     store: r
                                 }, o))
                             },
@@ -2254,276 +2298,289 @@
                                                 return o
                                             }(e, t);
                                             if (Object.getOwnPropertySymbols) {
                                                 var c = Object.getOwnPropertySymbols(e);
                                                 for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
                                             }
                                             return o
-                                        }(e, Mt);
+                                        }(e, Ut);
                                     if ("ArrowUp" === t.key || "ArrowDown" === t.key) {
-                                        var i = function() {
+                                        var a = function() {
                                                 var e = n.environment.document.getElementById("".concat(n.id, "-item-").concat(o.getState().activeItemId));
                                                 e && (e.scrollIntoViewIfNeeded ? e.scrollIntoViewIfNeeded(!1) : e.scrollIntoView(!1))
                                             },
-                                            a = function() {
-                                                var e = ct(o.getState());
+                                            i = function() {
+                                                var e = at(o.getState());
                                                 if (null !== o.getState().activeItemId && e) {
                                                     var n = e.item,
-                                                        i = e.itemInputValue,
-                                                        a = e.itemUrl,
+                                                        a = e.itemInputValue,
+                                                        i = e.itemUrl,
                                                         u = e.source;
-                                                    u.onActive(Ut({
+                                                    u.onActive(Bt({
                                                         event: t,
                                                         item: n,
-                                                        itemInputValue: i,
-                                                        itemUrl: a,
+                                                        itemInputValue: a,
+                                                        itemUrl: i,
                                                         refresh: r,
                                                         source: u,
                                                         state: o.getState()
                                                     }, c))
                                                 }
                                             };
-                                        t.preventDefault(), !1 === o.getState().isOpen && (n.openOnFocus || Boolean(o.getState().query)) ? qt(Ut({
+                                        t.preventDefault(), !1 === o.getState().isOpen && (n.openOnFocus || Boolean(o.getState().query)) ? Ht(Bt({
                                             event: t,
                                             props: n,
                                             query: o.getState().query,
                                             refresh: r,
                                             store: o
                                         }, c)).then((function() {
                                             o.dispatch(t.key, {
                                                 nextActiveItemId: n.defaultActiveItemId
-                                            }), a(), setTimeout(i, 0)
-                                        })) : (o.dispatch(t.key, {}), a(), i())
+                                            }), i(), setTimeout(a, 0)
+                                        })) : (o.dispatch(t.key, {}), i(), a())
                                     } else if ("Escape" === t.key) t.preventDefault(), o.dispatch(t.key, null), o.pendingRequests.cancelAll();
                                     else if ("Tab" === t.key) o.dispatch("blur", null), o.pendingRequests.cancelAll();
                                     else if ("Enter" === t.key) {
                                         if (null === o.getState().activeItemId || o.getState().collections.every((function(e) {
                                                 return 0 === e.items.length
                                             }))) return void(n.debug || o.pendingRequests.cancelAll());
                                         t.preventDefault();
-                                        var u = ct(o.getState()),
+                                        var u = at(o.getState()),
                                             l = u.item,
                                             s = u.itemInputValue,
                                             f = u.itemUrl,
                                             p = u.source;
-                                        if (t.metaKey || t.ctrlKey) void 0 !== f && (p.onSelect(Ut({
+                                        if (t.metaKey || t.ctrlKey) void 0 !== f && (p.onSelect(Bt({
                                             event: t,
                                             item: l,
                                             itemInputValue: s,
                                             itemUrl: f,
                                             refresh: r,
                                             source: p,
                                             state: o.getState()
                                         }, c)), n.navigator.navigateNewTab({
                                             itemUrl: f,
                                             item: l,
                                             state: o.getState()
                                         }));
-                                        else if (t.shiftKey) void 0 !== f && (p.onSelect(Ut({
+                                        else if (t.shiftKey) void 0 !== f && (p.onSelect(Bt({
                                             event: t,
                                             item: l,
                                             itemInputValue: s,
                                             itemUrl: f,
                                             refresh: r,
                                             source: p,
                                             state: o.getState()
                                         }, c)), n.navigator.navigateNewWindow({
                                             itemUrl: f,
                                             item: l,
                                             state: o.getState()
                                         }));
                                         else if (t.altKey);
                                         else {
-                                            if (void 0 !== f) return p.onSelect(Ut({
+                                            if (void 0 !== f) return p.onSelect(Bt({
                                                 event: t,
                                                 item: l,
                                                 itemInputValue: s,
                                                 itemUrl: f,
                                                 refresh: r,
                                                 source: p,
                                                 state: o.getState()
                                             }, c)), void n.navigator.navigate({
                                                 itemUrl: f,
                                                 item: l,
                                                 state: o.getState()
                                             });
-                                            qt(Ut({
+                                            Ht(Bt({
                                                 event: t,
                                                 nextState: {
                                                     isOpen: !1
                                                 },
                                                 props: n,
                                                 query: s,
                                                 refresh: r,
                                                 store: o
                                             }, c)).then((function() {
-                                                p.onSelect(Ut({
+                                                p.onSelect(Bt({
                                                     event: t,
                                                     item: l,
                                                     itemInputValue: s,
                                                     itemUrl: f,
                                                     refresh: r,
                                                     source: p,
                                                     state: o.getState()
                                                 }, c))
                                             }))
                                         }
                                     }
-                                }($t({
+                                }(Gt({
                                     event: e,
                                     props: t,
                                     refresh: n,
                                     store: r
                                 }, o))
                             },
-                            onFocus: i,
+                            onFocus: a,
                             onBlur: Ye,
                             onClick: function(n) {
-                                e.inputElement !== t.environment.document.activeElement || r.getState().isOpen || i(n)
+                                e.inputElement !== t.environment.document.activeElement || r.getState().isOpen || a(n)
                             }
                         }, s)
                     },
                     getPanelProps: function(e) {
-                        return $t({
+                        return Gt({
                             onMouseDown: function(e) {
                                 e.preventDefault()
                             },
                             onMouseLeave: function() {
                                 r.dispatch("mouseleave", null)
                             }
                         }, e)
                     },
                     getListProps: function(e) {
-                        return $t({
+                        var n = e || {},
+                            r = n.sourceIndex,
+                            o = en(n, Qt);
+                        return Gt({
                             role: "listbox",
-                            "aria-labelledby": "".concat(t.id, "-label"),
-                            id: "".concat(t.id, "-list")
-                        }, e)
+                            "aria-labelledby": "".concat(c(t.id, r), "-label"),
+                            id: "".concat(c(t.id, r), "-list")
+                        }, o)
                     },
                     getItemProps: function(e) {
-                        var c = e.item,
+                        var a = e.item,
                             i = e.source,
-                            a = Zt(e, zt);
-                        return $t({
-                            id: "".concat(t.id, "-item-").concat(c.__autocomplete_id),
+                            u = e.sourceIndex,
+                            l = en(e, Zt);
+                        return Gt({
+                            id: "".concat(c(t.id, u), "-item-").concat(a.__autocomplete_id),
                             role: "option",
-                            "aria-selected": r.getState().activeItemId === c.__autocomplete_id,
+                            "aria-selected": r.getState().activeItemId === a.__autocomplete_id,
                             onMouseMove: function(e) {
-                                if (c.__autocomplete_id !== r.getState().activeItemId) {
-                                    r.dispatch("mousemove", c.__autocomplete_id);
-                                    var t = ct(r.getState());
+                                if (a.__autocomplete_id !== r.getState().activeItemId) {
+                                    r.dispatch("mousemove", a.__autocomplete_id);
+                                    var t = at(r.getState());
                                     if (null !== r.getState().activeItemId && t) {
-                                        var i = t.item,
-                                            a = t.itemInputValue,
+                                        var c = t.item,
+                                            i = t.itemInputValue,
                                             u = t.itemUrl,
                                             l = t.source;
-                                        l.onActive($t({
+                                        l.onActive(Gt({
                                             event: e,
-                                            item: i,
-                                            itemInputValue: a,
+                                            item: c,
+                                            itemInputValue: i,
                                             itemUrl: u,
                                             refresh: n,
                                             source: l,
                                             state: r.getState()
                                         }, o))
                                     }
                                 }
                             },
                             onMouseDown: function(e) {
                                 e.preventDefault()
                             },
                             onClick: function(e) {
-                                var a = i.getItemInputValue({
-                                        item: c,
+                                var c = i.getItemInputValue({
+                                        item: a,
                                         state: r.getState()
                                     }),
                                     u = i.getItemUrl({
-                                        item: c,
+                                        item: a,
                                         state: r.getState()
                                     });
-                                (u ? Promise.resolve() : qt($t({
+                                (u ? Promise.resolve() : Ht(Gt({
                                     event: e,
                                     nextState: {
                                         isOpen: !1
                                     },
                                     props: t,
-                                    query: a,
+                                    query: c,
                                     refresh: n,
                                     store: r
                                 }, o))).then((function() {
-                                    i.onSelect($t({
+                                    i.onSelect(Gt({
                                         event: e,
-                                        item: c,
-                                        itemInputValue: a,
+                                        item: a,
+                                        itemInputValue: c,
                                         itemUrl: u,
                                         refresh: n,
                                         source: i,
                                         state: r.getState()
                                     }, o))
                                 }))
                             }
-                        }, a)
+                        }, l)
                     }
                 }
-            }(un({
+            }(pn({
                 props: n,
-                refresh: i,
-                store: r
+                refresh: a,
+                store: r,
+                navigator: n.navigator
             }, o));
 
-        function i() {
-            return qt(un({
+        function a() {
+            return Ht(pn({
                 event: new Event("input"),
                 nextState: {
                     isOpen: r.getState().isOpen
                 },
                 props: n,
+                navigator: n.navigator,
                 query: r.getState().query,
-                refresh: i,
+                refresh: a,
                 store: r
             }, o))
         }
         return n.plugins.forEach((function(e) {
-                var n;
-                return null === (n = e.subscribe) || void 0 === n ? void 0 : n.call(e, un(un({}, o), {}, {
-                    refresh: i,
+                var r;
+                return null === (r = e.subscribe) || void 0 === r ? void 0 : r.call(e, pn(pn({}, o), {}, {
+                    navigator: n.navigator,
+                    refresh: a,
                     onSelect: function(e) {
                         t.push({
                             onSelect: e
                         })
                     },
                     onActive: function(e) {
                         t.push({
                             onActive: e
                         })
+                    },
+                    onResolve: function(e) {
+                        t.push({
+                            onResolve: e
+                        })
                     }
                 }))
             })),
             function(e) {
                 var t, n, r = e.metadata,
                     o = e.environment;
                 if (null === (t = o.navigator) || void 0 === t || null === (n = t.userAgent) || void 0 === n ? void 0 : n.includes("Algolia Crawler")) {
                     var c = o.document.createElement("meta"),
-                        i = o.document.querySelector("head");
+                        a = o.document.querySelector("head");
                     c.name = "algolia:metadata", setTimeout((function() {
-                        c.content = JSON.stringify(r), i.appendChild(c)
+                        c.content = JSON.stringify(r), a.appendChild(c)
                     }), 0)
                 }
             }({
-                metadata: en({
+                metadata: on({
                     plugins: n.plugins,
                     options: e
                 }),
                 environment: n.environment
-            }), un(un({
-                refresh: i
+            }), pn(pn({
+                refresh: a,
+                navigator: n.navigator
             }, c), o)
     }
 
-    function fn(e) {
+    function hn(e) {
         var t = e.translations,
             n = (void 0 === t ? {} : t).searchByText,
             r = void 0 === n ? "Search by" : n;
         return Fe.createElement("a", {
             href: "https://www.algolia.com/ref/docsearch/?utm_source=".concat(window.location.hostname, "&utm_medium=referral&utm_content=powered_by&utm_campaign=docsearch"),
             target: "_blank",
             rel: "noopener noreferrer"
@@ -2568,98 +2625,98 @@
             d: "M1314.05,104.73h-49.33c-48.36,0-90.91,25.48-115.75,64.1-11.79,18.34-19.6,39.64-22.11,62.59-.58,5.3-.88,10.68-.88,16.14s.31,11.15,.93,16.59c4.28,38.09,23.14,71.61,50.66,94.52,2.93,2.6,6.05,4.98,9.31,7.14,12.86,8.49,28.11,13.47,44.52,13.47h0c17.99,0,34.61-5.93,48.16-15.97,16.29-11.58,28.88-28.54,34.48-47.75v50.26h-.11v11.08c0,21.84-5.71,38.27-17.34,49.36-11.61,11.08-31.04,16.63-58.25,16.63-11.12,0-28.79-.59-46.6-2.41-2.83-.29-5.46,1.5-6.27,4.22l-12.78,43.11c-1.02,3.46,1.27,7.02,4.83,7.53,21.52,3.08,42.52,4.68,54.65,4.68,48.91,0,85.16-10.75,108.89-32.21,21.48-19.41,33.15-48.89,35.2-88.52V110.63c0-3.26-2.64-5.9-5.9-5.9h-56.32Zm0,64.1s.65,139.13,0,143.36c-12.08,9.77-27.11,13.59-43.49,14.7-.16,.01-.33,.03-.49,.04-1.12,.07-2.24,.1-3.36,.1-1.32,0-2.63-.03-3.94-.1-40.41-2.11-74.52-37.26-74.52-79.38,0-10.25,1.96-20.01,5.42-28.98,11.22-29.12,38.77-49.74,71.06-49.74h49.33Z"
         }), Fe.createElement("path", {
             className: "cls-1",
             d: "M249.83,0C113.3,0,2,110.09,.03,246.16c-2,138.19,110.12,252.7,248.33,253.5,42.68,.25,83.79-10.19,120.3-30.03,3.56-1.93,4.11-6.83,1.08-9.51l-23.38-20.72c-4.75-4.21-11.51-5.4-17.36-2.92-25.48,10.84-53.17,16.38-81.71,16.03-111.68-1.37-201.91-94.29-200.13-205.96,1.76-110.26,92-199.41,202.67-199.41h202.69V407.41l-115-102.18c-3.72-3.31-9.42-2.66-12.42,1.31-18.46,24.44-48.53,39.64-81.93,37.34-46.33-3.2-83.87-40.5-87.34-86.81-4.15-55.24,39.63-101.52,94-101.52,49.18,0,89.68,37.85,93.91,85.95,.38,4.28,2.31,8.27,5.52,11.12l29.95,26.55c3.4,3.01,8.79,1.17,9.63-3.3,2.16-11.55,2.92-23.58,2.07-35.92-4.82-70.34-61.8-126.93-132.17-131.26-80.68-4.97-148.13,58.14-150.27,137.25-2.09,77.1,61.08,143.56,138.19,145.26,32.19,.71,62.03-9.41,86.14-26.95l150.26,133.2c6.44,5.71,16.61,1.14,16.61-7.47V9.48C499.66,4.25,495.42,0,490.18,0H249.83Z"
         })))
     }
 
-    function pn(e) {
+    function vn(e) {
         return Fe.createElement("svg", {
             width: "15",
             height: "15",
             "aria-label": e.ariaLabel,
             role: "img"
         }, Fe.createElement("g", {
             fill: "none",
             stroke: "currentColor",
             strokeLinecap: "round",
             strokeLinejoin: "round",
             strokeWidth: "1.2"
         }, e.children))
     }
 
-    function mn(e) {
+    function yn(e) {
         var t = e.translations,
             n = void 0 === t ? {} : t,
             r = n.selectText,
             o = void 0 === r ? "to select" : r,
             c = n.selectKeyAriaLabel,
-            i = void 0 === c ? "Enter key" : c,
-            a = n.navigateText,
-            u = void 0 === a ? "to navigate" : a,
+            a = void 0 === c ? "Enter key" : c,
+            i = n.navigateText,
+            u = void 0 === i ? "to navigate" : i,
             l = n.navigateUpKeyAriaLabel,
             s = void 0 === l ? "Arrow up" : l,
             f = n.navigateDownKeyAriaLabel,
             p = void 0 === f ? "Arrow down" : f,
             m = n.closeText,
             d = void 0 === m ? "to close" : m,
             h = n.closeKeyAriaLabel,
             v = void 0 === h ? "Escape key" : h,
             y = n.searchByText,
             _ = void 0 === y ? "Search by" : y;
         return Fe.createElement(Fe.Fragment, null, Fe.createElement("div", {
             className: "DocSearch-Logo"
-        }, Fe.createElement(fn, {
+        }, Fe.createElement(hn, {
             translations: {
                 searchByText: _
             }
         })), Fe.createElement("ul", {
             className: "DocSearch-Commands"
         }, Fe.createElement("li", null, Fe.createElement("kbd", {
             className: "DocSearch-Commands-Key"
-        }, Fe.createElement(pn, {
-            ariaLabel: i
+        }, Fe.createElement(vn, {
+            ariaLabel: a
         }, Fe.createElement("path", {
             d: "M12 3.53088v3c0 1-1 2-2 2H4M7 11.53088l-3-3 3-3"
         }))), Fe.createElement("span", {
             className: "DocSearch-Label"
         }, o)), Fe.createElement("li", null, Fe.createElement("kbd", {
             className: "DocSearch-Commands-Key"
-        }, Fe.createElement(pn, {
+        }, Fe.createElement(vn, {
             ariaLabel: p
         }, Fe.createElement("path", {
             d: "M7.5 3.5v8M10.5 8.5l-3 3-3-3"
         }))), Fe.createElement("kbd", {
             className: "DocSearch-Commands-Key"
-        }, Fe.createElement(pn, {
+        }, Fe.createElement(vn, {
             ariaLabel: s
         }, Fe.createElement("path", {
             d: "M7.5 11.5v-8M10.5 6.5l-3-3-3 3"
         }))), Fe.createElement("span", {
             className: "DocSearch-Label"
         }, u)), Fe.createElement("li", null, Fe.createElement("kbd", {
             className: "DocSearch-Commands-Key"
-        }, Fe.createElement(pn, {
+        }, Fe.createElement(vn, {
             ariaLabel: v
         }, Fe.createElement("path", {
             d: "M13.6167 8.936c-.1065.3583-.6883.962-1.4875.962-.7993 0-1.653-.9165-1.653-2.1258v-.5678c0-1.2548.7896-2.1016 1.653-2.1016.8634 0 1.3601.4778 1.4875 1.0724M9 6c-.1352-.4735-.7506-.9219-1.46-.8972-.7092.0246-1.344.57-1.344 1.2166s.4198.8812 1.3445.9805C8.465 7.3992 8.968 7.9337 9 8.5c.032.5663-.454 1.398-1.4595 1.398C6.6593 9.898 6 9 5.963 8.4851m-1.4748.5368c-.2635.5941-.8099.876-1.5443.876s-1.7073-.6248-1.7073-2.204v-.4603c0-1.0416.721-2.131 1.7073-2.131.9864 0 1.6425 1.031 1.5443 2.2492h-2.956"
         }))), Fe.createElement("span", {
             className: "DocSearch-Label"
         }, d))))
     }
 
-    function dn(e) {
+    function _n(e) {
         var t = e.hit,
             n = e.children;
         return Fe.createElement("a", {
             href: t.url
         }, n)
     }
 
-    function hn() {
+    function bn() {
         return Fe.createElement("svg", {
             viewBox: "0 0 38 38",
             stroke: "currentColor",
             strokeOpacity: ".5"
         }, Fe.createElement("g", {
             fill: "none",
             fillRule: "evenodd"
@@ -2679,15 +2736,15 @@
             from: "0 18 18",
             to: "360 18 18",
             dur: "1s",
             repeatCount: "indefinite"
         })))))
     }
 
-    function vn() {
+    function gn() {
         return Fe.createElement("svg", {
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Fe.createElement("g", {
             stroke: "currentColor",
             fill: "none",
@@ -2697,30 +2754,30 @@
         }, Fe.createElement("path", {
             d: "M3.18 6.6a8.23 8.23 0 1112.93 9.94h0a8.23 8.23 0 01-11.63 0"
         }), Fe.createElement("path", {
             d: "M6.44 7.25H2.55V3.36M10.45 6v5.6M10.45 11.6L13 13"
         })))
     }
 
-    function yn() {
+    function On() {
         return Fe.createElement("svg", {
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Fe.createElement("path", {
             d: "M10 10l5.09-5.09L10 10l5.09 5.09L10 10zm0 0L4.91 4.91 10 10l-5.09 5.09L10 10z",
             stroke: "currentColor",
             fill: "none",
             fillRule: "evenodd",
             strokeLinecap: "round",
             strokeLinejoin: "round"
         }))
     }
 
-    function _n() {
+    function Sn() {
         return Fe.createElement("svg", {
             className: "DocSearch-Hit-Select-Icon",
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Fe.createElement("g", {
             stroke: "currentColor",
@@ -2730,138 +2787,138 @@
             strokeLinejoin: "round"
         }, Fe.createElement("path", {
             d: "M18 3v4c0 2-2 4-4 4H2"
         }), Fe.createElement("path", {
             d: "M8 17l-6-6 6-6"
         })))
     }
-    var bn = function() {
+    var En = function() {
         return Fe.createElement("svg", {
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Fe.createElement("path", {
             d: "M17 6v12c0 .52-.2 1-1 1H4c-.7 0-1-.33-1-1V2c0-.55.42-1 1-1h8l5 5zM14 8h-3.13c-.51 0-.87-.34-.87-.87V4",
             stroke: "currentColor",
             fill: "none",
             fillRule: "evenodd",
             strokeLinejoin: "round"
         }))
     };
 
-    function gn(e) {
+    function wn(e) {
         switch (e.type) {
             case "lvl1":
-                return Fe.createElement(bn, null);
+                return Fe.createElement(En, null);
             case "content":
-                return Fe.createElement(Sn, null);
+                return Fe.createElement(Pn, null);
             default:
-                return Fe.createElement(On, null)
+                return Fe.createElement(jn, null)
         }
     }
 
-    function On() {
+    function jn() {
         return Fe.createElement("svg", {
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Fe.createElement("path", {
             d: "M13 13h4-4V8H7v5h6v4-4H7V8H3h4V3v5h6V3v5h4-4v5zm-6 0v4-4H3h4z",
             stroke: "currentColor",
             fill: "none",
             fillRule: "evenodd",
             strokeLinecap: "round",
             strokeLinejoin: "round"
         }))
     }
 
-    function Sn() {
+    function Pn() {
         return Fe.createElement("svg", {
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Fe.createElement("path", {
             d: "M17 5H3h14zm0 5H3h14zm0 5H3h14z",
             stroke: "currentColor",
             fill: "none",
             fillRule: "evenodd",
             strokeLinejoin: "round"
         }))
     }
 
-    function En() {
+    function In() {
         return Fe.createElement("svg", {
             width: "20",
             height: "20",
             viewBox: "0 0 20 20"
         }, Fe.createElement("path", {
             d: "M10 14.2L5 17l1-5.6-4-4 5.5-.7 2.5-5 2.5 5 5.6.8-4 4 .9 5.5z",
             stroke: "currentColor",
             fill: "none",
             fillRule: "evenodd",
             strokeLinejoin: "round"
         }))
     }
 
-    function wn() {
+    function kn() {
         return Fe.createElement("svg", {
             width: "40",
             height: "40",
             viewBox: "0 0 20 20",
             fill: "none",
             fillRule: "evenodd",
             stroke: "currentColor",
             strokeLinecap: "round",
             strokeLinejoin: "round"
         }, Fe.createElement("path", {
             d: "M19 4.8a16 16 0 00-2-1.2m-3.3-1.2A16 16 0 001.1 4.7M16.7 8a12 12 0 00-2.8-1.4M10 6a12 12 0 00-6.7 2M12.3 14.7a4 4 0 00-4.5 0M14.5 11.4A8 8 0 0010 10M3 16L18 2M10 18h0"
         }))
     }
 
-    function jn() {
+    function Dn() {
         return Fe.createElement("svg", {
             width: "40",
             height: "40",
             viewBox: "0 0 20 20",
             fill: "none",
             fillRule: "evenodd",
             stroke: "currentColor",
             strokeLinecap: "round",
             strokeLinejoin: "round"
         }, Fe.createElement("path", {
             d: "M15.5 4.8c2 3 1.7 7-1 9.7h0l4.3 4.3-4.3-4.3a7.8 7.8 0 01-9.8 1m-2.2-2.2A7.8 7.8 0 0113.2 2.4M2 18L18 2"
         }))
     }
 
-    function Pn(e) {
+    function Cn(e) {
         var t = e.translations,
             n = void 0 === t ? {} : t,
             r = n.titleText,
             o = void 0 === r ? "Unable to fetch results" : r,
             c = n.helpText,
-            i = void 0 === c ? "You might want to check your network connection." : c;
+            a = void 0 === c ? "You might want to check your network connection." : c;
         return Fe.createElement("div", {
             className: "DocSearch-ErrorScreen"
         }, Fe.createElement("div", {
             className: "DocSearch-Screen-Icon"
-        }, Fe.createElement(wn, null)), Fe.createElement("p", {
+        }, Fe.createElement(kn, null)), Fe.createElement("p", {
             className: "DocSearch-Title"
         }, o), Fe.createElement("p", {
             className: "DocSearch-Help"
-        }, i))
+        }, a))
     }
-    var In = ["translations"];
+    var xn = ["translations"];
 
-    function kn(e, t) {
+    function An(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function Dn(e) {
+    function Nn(e) {
         var t = e.translations,
             n = void 0 === t ? {} : t,
             r = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = function(e, t) {
                     if (null == e) return {};
                     var n, r, o = {},
@@ -2870,45 +2927,45 @@
                     return o
                 }(e, t);
                 if (Object.getOwnPropertySymbols) {
                     var c = Object.getOwnPropertySymbols(e);
                     for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
                 }
                 return o
-            }(e, In),
+            }(e, xn),
             o = n.noResultsText,
             c = void 0 === o ? "No results for" : o,
-            i = n.suggestedQueryText,
-            a = void 0 === i ? "Try searching for" : i,
+            a = n.suggestedQueryText,
+            i = void 0 === a ? "Try searching for" : a,
             u = n.reportMissingResultsText,
             l = void 0 === u ? "Believe this query should return results?" : u,
             s = n.reportMissingResultsLinkText,
             f = void 0 === s ? "Let us know." : s,
             p = r.state.context.searchSuggestions;
         return Fe.createElement("div", {
             className: "DocSearch-NoResults"
         }, Fe.createElement("div", {
             className: "DocSearch-Screen-Icon"
-        }, Fe.createElement(jn, null)), Fe.createElement("p", {
+        }, Fe.createElement(Dn, null)), Fe.createElement("p", {
             className: "DocSearch-Title"
         }, c, ' "', Fe.createElement("strong", null, r.state.query), '"'), p && p.length > 0 && Fe.createElement("div", {
             className: "DocSearch-NoResults-Prefill-List"
         }, Fe.createElement("p", {
             className: "DocSearch-Help"
-        }, a, ":"), Fe.createElement("ul", null, p.slice(0, 3).reduce((function(e, t) {
+        }, i, ":"), Fe.createElement("ul", null, p.slice(0, 3).reduce((function(e, t) {
             return [].concat(function(e) {
                 return function(e) {
-                    if (Array.isArray(e)) return kn(e)
+                    if (Array.isArray(e)) return An(e)
                 }(e) || function(e) {
                     if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
                 }(e) || function(e, t) {
                     if (e) {
-                        if ("string" == typeof e) return kn(e, t);
+                        if ("string" == typeof e) return An(e, t);
                         var n = Object.prototype.toString.call(e).slice(8, -1);
-                        return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? kn(e, t) : void 0
+                        return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? An(e, t) : void 0
                     }
                 }(e) || function() {
                     throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                 }()
             }(e), [Fe.createElement("li", {
                 key: t
             }, Fe.createElement("button", {
@@ -2925,257 +2982,261 @@
             href: r.getMissingResultsUrl({
                 query: r.state.query
             }),
             target: "_blank",
             rel: "noopener noreferrer"
         }, f)))
     }
-    var Cn = ["hit", "attribute", "tagName"];
+    var Rn = ["hit", "attribute", "tagName"];
 
-    function An(e, t) {
+    function Tn(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function xn(e) {
+    function Ln(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? An(Object(n), !0).forEach((function(t) {
-                Nn(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : An(Object(n)).forEach((function(t) {
+            t % 2 ? Tn(Object(n), !0).forEach((function(t) {
+                qn(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Tn(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Nn(e, t, n) {
+    function qn(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function Rn(e, t) {
+    function Mn(e, t) {
         return t.split(".").reduce((function(e, t) {
             return null != e && e[t] ? e[t] : null
         }), e)
     }
 
-    function Tn(e) {
+    function Hn(e) {
         var t = e.hit,
             n = e.attribute,
             r = e.tagName;
-        return b(void 0 === r ? "span" : r, xn(xn({}, function(e, t) {
+        return b(void 0 === r ? "span" : r, Ln(Ln({}, function(e, t) {
             if (null == e) return {};
             var n, r, o = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = {},
                     c = Object.keys(e);
                 for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                 return o
             }(e, t);
             if (Object.getOwnPropertySymbols) {
                 var c = Object.getOwnPropertySymbols(e);
                 for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
             }
             return o
-        }(e, Cn)), {}, {
+        }(e, Rn)), {}, {
             dangerouslySetInnerHTML: {
-                __html: Rn(t, "_snippetResult.".concat(n, ".value")) || Rn(t, n)
+                __html: Mn(t, "_snippetResult.".concat(n, ".value")) || Mn(t, n)
             }
         }))
     }
 
-    function Ln(e, t) {
+    function Un(e, t) {
         return function(e) {
             if (Array.isArray(e)) return e
         }(e) || function(e, t) {
             var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
             if (null != n) {
                 var r, o, c = [],
-                    i = !0,
-                    a = !1;
+                    a = !0,
+                    i = !1;
                 try {
-                    for (n = n.call(e); !(i = (r = n.next()).done) && (c.push(r.value), !t || c.length !== t); i = !0);
+                    for (n = n.call(e); !(a = (r = n.next()).done) && (c.push(r.value), !t || c.length !== t); a = !0);
                 } catch (e) {
-                    a = !0, o = e
+                    i = !0, o = e
                 } finally {
                     try {
-                        i || null == n.return || n.return()
+                        a || null == n.return || n.return()
                     } finally {
-                        if (a) throw o
+                        if (i) throw o
                     }
                 }
                 return c
             }
         }(e, t) || function(e, t) {
             if (e) {
-                if ("string" == typeof e) return qn(e, t);
+                if ("string" == typeof e) return Fn(e, t);
                 var n = Object.prototype.toString.call(e).slice(8, -1);
-                return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? qn(e, t) : void 0
+                return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Fn(e, t) : void 0
             }
         }(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function qn(e, t) {
+    function Fn(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function Mn() {
-        return Mn = Object.assign || function(e) {
+    function Bn() {
+        return Bn = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, Mn.apply(this, arguments)
+        }, Bn.apply(this, arguments)
     }
 
-    function Hn(e) {
+    function Vn(e) {
         return e.collection && 0 !== e.collection.items.length ? Fe.createElement("section", {
             className: "DocSearch-Hits"
         }, Fe.createElement("div", {
             className: "DocSearch-Hit-source"
         }, e.title), Fe.createElement("ul", e.getListProps(), e.collection.items.map((function(t, n) {
-            return Fe.createElement(Un, Mn({
+            return Fe.createElement(Wn, Bn({
                 key: [e.title, t.objectID].join(":"),
                 item: t,
                 index: n
             }, e))
         })))) : null
     }
 
-    function Un(e) {
+    function Wn(e) {
         var t = e.item,
             n = e.index,
             r = e.renderIcon,
             o = e.renderAction,
             c = e.getItemProps,
-            i = e.onItemClick,
-            a = e.collection,
+            a = e.onItemClick,
+            i = e.collection,
             u = e.hitComponent,
-            l = Ln(Fe.useState(!1), 2),
+            l = Un(Fe.useState(!1), 2),
             s = l[0],
             f = l[1],
-            p = Ln(Fe.useState(!1), 2),
+            p = Un(Fe.useState(!1), 2),
             m = p[0],
             d = p[1],
             h = Fe.useRef(null),
             v = u;
-        return Fe.createElement("li", Mn({
+        return Fe.createElement("li", Bn({
             className: ["DocSearch-Hit", t.__docsearch_parent && "DocSearch-Hit--Child", s && "DocSearch-Hit--deleting", m && "DocSearch-Hit--favoriting"].filter(Boolean).join(" "),
             onTransitionEnd: function() {
                 h.current && h.current()
             }
         }, c({
             item: t,
-            source: a.source,
-            onClick: function() {
-                i(t)
+            source: i.source,
+            onClick: function(e) {
+                a(t, e)
             }
         })), Fe.createElement(v, {
             hit: t
         }, Fe.createElement("div", {
             className: "DocSearch-Hit-Container"
         }, r({
             item: t,
             index: n
         }), t.hierarchy[t.type] && "lvl1" === t.type && Fe.createElement("div", {
             className: "DocSearch-Hit-content-wrapper"
-        }, Fe.createElement(Tn, {
+        }, Fe.createElement(Hn, {
             className: "DocSearch-Hit-title",
             hit: t,
             attribute: "hierarchy.lvl1"
-        }), t.content && Fe.createElement(Tn, {
+        }), t.content && Fe.createElement(Hn, {
             className: "DocSearch-Hit-path",
             hit: t,
             attribute: "content"
         })), t.hierarchy[t.type] && ("lvl2" === t.type || "lvl3" === t.type || "lvl4" === t.type || "lvl5" === t.type || "lvl6" === t.type) && Fe.createElement("div", {
             className: "DocSearch-Hit-content-wrapper"
-        }, Fe.createElement(Tn, {
+        }, Fe.createElement(Hn, {
             className: "DocSearch-Hit-title",
             hit: t,
             attribute: "hierarchy.".concat(t.type)
-        }), Fe.createElement(Tn, {
+        }), Fe.createElement(Hn, {
             className: "DocSearch-Hit-path",
             hit: t,
             attribute: "hierarchy.lvl1"
         })), "content" === t.type && Fe.createElement("div", {
             className: "DocSearch-Hit-content-wrapper"
-        }, Fe.createElement(Tn, {
+        }, Fe.createElement(Hn, {
             className: "DocSearch-Hit-title",
             hit: t,
             attribute: "content"
-        }), Fe.createElement(Tn, {
+        }), Fe.createElement(Hn, {
             className: "DocSearch-Hit-path",
             hit: t,
             attribute: "hierarchy.lvl1"
         })), o({
             item: t,
             runDeleteTransition: function(e) {
                 f(!0), h.current = e
             },
             runFavoriteTransition: function(e) {
                 d(!0), h.current = e
             }
         }))))
     }
 
-    function Fn(e, t) {
+    function Kn(e, t) {
         return e.reduce((function(e, n) {
             var r = t(n);
             return e.hasOwnProperty(r) || (e[r] = []), e[r].length < 5 && e[r].push(n), e
         }), {})
     }
 
-    function Bn(e) {
+    function zn(e) {
         return e
     }
 
-    function Vn() {}
-    var Wn = /(<mark>|<\/mark>)/g,
-        Kn = RegExp(Wn.source);
+    function Jn(e) {
+        return 1 === e.button || e.altKey || e.ctrlKey || e.metaKey || e.shiftKey
+    }
 
-    function zn(e) {
-        var t, n, r, o, c, i = e;
-        if (!i.__docsearch_parent && !e._highlightResult) return e.hierarchy.lvl0;
-        var a = ((i.__docsearch_parent ? null === (t = i.__docsearch_parent) || void 0 === t || null === (n = t._highlightResult) || void 0 === n || null === (r = n.hierarchy) || void 0 === r ? void 0 : r.lvl0 : null === (o = e._highlightResult) || void 0 === o || null === (c = o.hierarchy) || void 0 === c ? void 0 : c.lvl0) || {}).value;
-        return a && Kn.test(a) ? a.replace(Wn, "") : a
+    function $n() {}
+    var Qn = /(<mark>|<\/mark>)/g,
+        Zn = RegExp(Qn.source);
+
+    function Yn(e) {
+        var t, n, r, o, c, a = e;
+        if (!a.__docsearch_parent && !e._highlightResult) return e.hierarchy.lvl0;
+        var i = ((a.__docsearch_parent ? null === (t = a.__docsearch_parent) || void 0 === t || null === (n = t._highlightResult) || void 0 === n || null === (r = n.hierarchy) || void 0 === r ? void 0 : r.lvl0 : null === (o = e._highlightResult) || void 0 === o || null === (c = o.hierarchy) || void 0 === c ? void 0 : c.lvl0) || {}).value;
+        return i && Zn.test(i) ? i.replace(Qn, "") : i
     }
 
-    function Jn() {
-        return Jn = Object.assign || function(e) {
+    function Gn() {
+        return Gn = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, Jn.apply(this, arguments)
+        }, Gn.apply(this, arguments)
     }
 
-    function $n(e) {
+    function Xn(e) {
         return Fe.createElement("div", {
             className: "DocSearch-Dropdown-Container"
         }, e.state.collections.map((function(t) {
             if (0 === t.items.length) return null;
-            var n = zn(t.items[0]);
-            return Fe.createElement(Hn, Jn({}, e, {
+            var n = Yn(t.items[0]);
+            return Fe.createElement(Vn, Gn({}, e, {
                 key: t.source.sourceId,
                 title: n,
                 collection: t,
                 renderIcon: function(e) {
                     var n, r = e.item,
                         o = e.index;
                     return Fe.createElement(Fe.Fragment, null, r.__docsearch_parent && Fe.createElement("svg", {
@@ -3189,43 +3250,43 @@
                         strokeLinejoin: "round"
                     }, r.__docsearch_parent !== (null === (n = t.items[o + 1]) || void 0 === n ? void 0 : n.__docsearch_parent) ? Fe.createElement("path", {
                         d: "M8 6v21M20 27H8.3"
                     }) : Fe.createElement("path", {
                         d: "M8 6v42M20 27H8.3"
                     }))), Fe.createElement("div", {
                         className: "DocSearch-Hit-icon"
-                    }, Fe.createElement(gn, {
+                    }, Fe.createElement(wn, {
                         type: r.type
                     })))
                 },
                 renderAction: function() {
                     return Fe.createElement("div", {
                         className: "DocSearch-Hit-action"
-                    }, Fe.createElement(_n, null))
+                    }, Fe.createElement(Sn, null))
                 }
             }))
         })), e.resultsFooterComponent && Fe.createElement("section", {
             className: "DocSearch-HitsFooter"
         }, Fe.createElement(e.resultsFooterComponent, {
             state: e.state
         })))
     }
-    var Qn = ["translations"];
+    var er = ["translations"];
 
-    function Zn() {
-        return Zn = Object.assign || function(e) {
+    function tr() {
+        return tr = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, Zn.apply(this, arguments)
+        }, tr.apply(this, arguments)
     }
 
-    function Yn(e) {
+    function nr(e) {
         var t = e.translations,
             n = void 0 === t ? {} : t,
             r = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = function(e, t) {
                     if (null == e) return {};
                     var n, r, o = {},
@@ -3234,40 +3295,40 @@
                     return o
                 }(e, t);
                 if (Object.getOwnPropertySymbols) {
                     var c = Object.getOwnPropertySymbols(e);
                     for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
                 }
                 return o
-            }(e, Qn),
+            }(e, er),
             o = n.recentSearchesTitle,
             c = void 0 === o ? "Recent" : o,
-            i = n.noRecentSearchesText,
-            a = void 0 === i ? "No recent searches" : i,
+            a = n.noRecentSearchesText,
+            i = void 0 === a ? "No recent searches" : a,
             u = n.saveRecentSearchButtonTitle,
             l = void 0 === u ? "Save this search" : u,
             s = n.removeRecentSearchButtonTitle,
             f = void 0 === s ? "Remove this search from history" : s,
             p = n.favoriteSearchesTitle,
             m = void 0 === p ? "Favorite" : p,
             d = n.removeFavoriteSearchButtonTitle,
             h = void 0 === d ? "Remove this search from favorites" : d;
         return "idle" === r.state.status && !1 === r.hasCollections ? r.disableUserPersonalization ? null : Fe.createElement("div", {
             className: "DocSearch-StartScreen"
         }, Fe.createElement("p", {
             className: "DocSearch-Help"
-        }, a)) : !1 === r.hasCollections ? null : Fe.createElement("div", {
+        }, i)) : !1 === r.hasCollections ? null : Fe.createElement("div", {
             className: "DocSearch-Dropdown-Container"
-        }, Fe.createElement(Hn, Zn({}, r, {
+        }, Fe.createElement(Vn, tr({}, r, {
             title: c,
             collection: r.state.collections[0],
             renderIcon: function() {
                 return Fe.createElement("div", {
                     className: "DocSearch-Hit-icon"
-                }, Fe.createElement(vn, null))
+                }, Fe.createElement(gn, null))
             },
             renderAction: function(e) {
                 var t = e.item,
                     n = e.runFavoriteTransition,
                     o = e.runDeleteTransition;
                 return Fe.createElement(Fe.Fragment, null, Fe.createElement("div", {
                     className: "DocSearch-Hit-action"
@@ -3276,34 +3337,34 @@
                     title: l,
                     type: "submit",
                     onClick: function(e) {
                         e.preventDefault(), e.stopPropagation(), n((function() {
                             r.favoriteSearches.add(t), r.recentSearches.remove(t), r.refresh()
                         }))
                     }
-                }, Fe.createElement(En, null))), Fe.createElement("div", {
+                }, Fe.createElement(In, null))), Fe.createElement("div", {
                     className: "DocSearch-Hit-action"
                 }, Fe.createElement("button", {
                     className: "DocSearch-Hit-action-button",
                     title: f,
                     type: "submit",
                     onClick: function(e) {
                         e.preventDefault(), e.stopPropagation(), o((function() {
                             r.recentSearches.remove(t), r.refresh()
                         }))
                     }
-                }, Fe.createElement(yn, null))))
+                }, Fe.createElement(On, null))))
             }
-        })), Fe.createElement(Hn, Zn({}, r, {
+        })), Fe.createElement(Vn, tr({}, r, {
             title: m,
             collection: r.state.collections[1],
             renderIcon: function() {
                 return Fe.createElement("div", {
                     className: "DocSearch-Hit-icon"
-                }, Fe.createElement(En, null))
+                }, Fe.createElement(In, null))
             },
             renderAction: function(e) {
                 var t = e.item,
                     n = e.runDeleteTransition;
                 return Fe.createElement("div", {
                     className: "DocSearch-Hit-action"
                 }, Fe.createElement("button", {
@@ -3311,30 +3372,30 @@
                     title: h,
                     type: "submit",
                     onClick: function(e) {
                         e.preventDefault(), e.stopPropagation(), n((function() {
                             r.favoriteSearches.remove(t), r.refresh()
                         }))
                     }
-                }, Fe.createElement(yn, null)))
+                }, Fe.createElement(On, null)))
             }
         })))
     }
-    var Gn = ["translations"];
+    var rr = ["translations"];
 
-    function Xn() {
-        return Xn = Object.assign || function(e) {
+    function or() {
+        return or = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, Xn.apply(this, arguments)
+        }, or.apply(this, arguments)
     }
-    var er = Fe.memo((function(e) {
+    var cr = Fe.memo((function(e) {
             var t = e.translations,
                 n = void 0 === t ? {} : t,
                 r = function(e, t) {
                     if (null == e) return {};
                     var n, r, o = function(e, t) {
                         if (null == e) return {};
                         var n, r, o = {},
@@ -3343,43 +3404,43 @@
                         return o
                     }(e, t);
                     if (Object.getOwnPropertySymbols) {
                         var c = Object.getOwnPropertySymbols(e);
                         for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
                     }
                     return o
-                }(e, Gn);
-            if ("error" === r.state.status) return Fe.createElement(Pn, {
+                }(e, rr);
+            if ("error" === r.state.status) return Fe.createElement(Cn, {
                 translations: null == n ? void 0 : n.errorScreen
             });
             var o = r.state.collections.some((function(e) {
                 return e.items.length > 0
             }));
-            return r.state.query ? !1 === o ? Fe.createElement(Dn, Xn({}, r, {
+            return r.state.query ? !1 === o ? Fe.createElement(Nn, or({}, r, {
                 translations: null == n ? void 0 : n.noResultsScreen
-            })) : Fe.createElement($n, r) : Fe.createElement(Yn, Xn({}, r, {
+            })) : Fe.createElement(Xn, r) : Fe.createElement(nr, or({}, r, {
                 hasCollections: o,
                 translations: null == n ? void 0 : n.startScreen
             }))
         }), (function(e, t) {
             return "loading" === t.state.status || "stalled" === t.state.status
         })),
-        tr = ["translations"];
+        ar = ["translations"];
 
-    function nr() {
-        return nr = Object.assign || function(e) {
+    function ir() {
+        return ir = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, nr.apply(this, arguments)
+        }, ir.apply(this, arguments)
     }
 
-    function rr(e) {
+    function ur(e) {
         var t = e.translations,
             n = void 0 === t ? {} : t,
             r = function(e, t) {
                 if (null == e) return {};
                 var n, r, o = function(e, t) {
                     if (null == e) return {};
                     var n, r, o = {},
@@ -3388,19 +3449,19 @@
                     return o
                 }(e, t);
                 if (Object.getOwnPropertySymbols) {
                     var c = Object.getOwnPropertySymbols(e);
                     for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
                 }
                 return o
-            }(e, tr),
+            }(e, ar),
             o = n.resetButtonTitle,
             c = void 0 === o ? "Clear the query" : o,
-            i = n.resetButtonAriaLabel,
-            a = void 0 === i ? "Clear the query" : i,
+            a = n.resetButtonAriaLabel,
+            i = void 0 === a ? "Clear the query" : a,
             u = n.cancelButtonText,
             l = void 0 === u ? "Cancel" : u,
             s = n.cancelButtonAriaLabel,
             f = void 0 === s ? "Cancel" : s,
             p = r.getFormProps({
                 inputElement: r.inputRef.current
             }).onReset;
@@ -3410,41 +3471,41 @@
             r.isFromSelection && r.inputRef.current && r.inputRef.current.select()
         }), [r.isFromSelection, r.inputRef]), Fe.createElement(Fe.Fragment, null, Fe.createElement("form", {
             className: "DocSearch-Form",
             onSubmit: function(e) {
                 e.preventDefault()
             },
             onReset: p
-        }, Fe.createElement("label", nr({
+        }, Fe.createElement("label", ir({
             className: "DocSearch-MagnifierLabel"
         }, r.getLabelProps()), Fe.createElement(Ve, null)), Fe.createElement("div", {
             className: "DocSearch-LoadingIndicator"
-        }, Fe.createElement(hn, null)), Fe.createElement("input", nr({
+        }, Fe.createElement(bn, null)), Fe.createElement("input", ir({
             className: "DocSearch-Input",
             ref: r.inputRef
         }, r.getInputProps({
             inputElement: r.inputRef.current,
             autoFocus: r.autoFocus,
             maxLength: 64
         }))), Fe.createElement("button", {
             type: "reset",
             title: c,
             className: "DocSearch-Reset",
-            "aria-label": a,
+            "aria-label": i,
             hidden: !r.state.query
-        }, Fe.createElement(yn, null))), Fe.createElement("button", {
+        }, Fe.createElement(On, null))), Fe.createElement("button", {
             className: "DocSearch-Cancel",
             type: "reset",
             "aria-label": f,
             onClick: r.onClose
         }, l))
     }
-    var or = ["_highlightResult", "_snippetResult"];
+    var lr = ["_highlightResult", "_snippetResult"];
 
-    function cr(e) {
+    function sr(e) {
         var t = e.key,
             n = e.limit,
             r = void 0 === n ? 5 : n,
             o = function(e) {
                 return !1 === function() {
                     var e = "__TEST_KEY__";
                     try {
@@ -3481,33 +3542,33 @@
                             return o
                         }(e, t);
                         if (Object.getOwnPropertySymbols) {
                             var c = Object.getOwnPropertySymbols(e);
                             for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
                         }
                         return o
-                    }(t, or)),
-                    i = c.findIndex((function(e) {
+                    }(t, lr)),
+                    a = c.findIndex((function(e) {
                         return e.objectID === n.objectID
                     }));
-                i > -1 && c.splice(i, 1), c.unshift(n), c = c.slice(0, r), o.setItem(c)
+                a > -1 && c.splice(a, 1), c.unshift(n), c = c.slice(0, r), o.setItem(c)
             },
             remove: function(e) {
                 c = c.filter((function(t) {
                     return t.objectID !== e.objectID
                 })), o.setItem(c)
             },
             getAll: function() {
                 return c
             }
         }
     }
-    var ir = ["facetName", "facetQuery"];
+    var fr = ["facetName", "facetQuery"];
 
-    function ar(e) {
+    function pr(e) {
         var t, n = "algoliasearch-client-js-".concat(e.key),
             r = function() {
                 return void 0 === t && (t = e.localStorage || window.localStorage), t
             },
             o = function() {
                 return JSON.parse(r().getItem(n) || "{}")
             };
@@ -3547,16 +3608,16 @@
                 return Promise.resolve().then((function() {
                     r().removeItem(n)
                 }))
             }
         }
     }
 
-    function ur(e) {
-        var t = i(e.caches),
+    function mr(e) {
+        var t = a(e.caches),
             n = t.shift();
         return void 0 === n ? {
             get: function(e, t) {
                 var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {
                     miss: function() {
                         return Promise.resolve()
                     }
@@ -3580,150 +3641,150 @@
             get: function(e, r) {
                 var o = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {
                     miss: function() {
                         return Promise.resolve()
                     }
                 };
                 return n.get(e, r, o).catch((function() {
-                    return ur({
+                    return mr({
                         caches: t
                     }).get(e, r, o)
                 }))
             },
             set: function(e, r) {
                 return n.set(e, r).catch((function() {
-                    return ur({
+                    return mr({
                         caches: t
                     }).set(e, r)
                 }))
             },
             delete: function(e) {
                 return n.delete(e).catch((function() {
-                    return ur({
+                    return mr({
                         caches: t
                     }).delete(e)
                 }))
             },
             clear: function() {
                 return n.clear().catch((function() {
-                    return ur({
+                    return mr({
                         caches: t
                     }).clear()
                 }))
             }
         }
     }
 
-    function lr() {
+    function dr() {
         var e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {
                 serializable: !0
             },
             t = {};
         return {
             get: function(n, r) {
                 var o = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {
                         miss: function() {
                             return Promise.resolve()
                         }
                     },
                     c = JSON.stringify(n);
                 if (c in t) return Promise.resolve(e.serializable ? JSON.parse(t[c]) : t[c]);
-                var i = r(),
-                    a = o && o.miss || function() {
+                var a = r(),
+                    i = o && o.miss || function() {
                         return Promise.resolve()
                     };
-                return i.then((function(e) {
-                    return a(e)
+                return a.then((function(e) {
+                    return i(e)
                 })).then((function() {
-                    return i
+                    return a
                 }))
             },
             set: function(n, r) {
                 return t[JSON.stringify(n)] = e.serializable ? JSON.stringify(r) : r, Promise.resolve(r)
             },
             delete: function(e) {
                 return delete t[JSON.stringify(e)], Promise.resolve()
             },
             clear: function() {
                 return t = {}, Promise.resolve()
             }
         }
     }
 
-    function sr(e) {
+    function hr(e) {
         for (var t = e.length - 1; t > 0; t--) {
             var n = Math.floor(Math.random() * (t + 1)),
                 r = e[t];
             e[t] = e[n], e[n] = r
         }
         return e
     }
 
-    function fr(e, t) {
+    function vr(e, t) {
         return t ? (Object.keys(t).forEach((function(n) {
             e[n] = t[n](e)
         })), e) : e
     }
 
-    function pr(e) {
+    function yr(e) {
         for (var t = arguments.length, n = new Array(t > 1 ? t - 1 : 0), r = 1; r < t; r++) n[r - 1] = arguments[r];
         var o = 0;
         return e.replace(/%s/g, (function() {
             return encodeURIComponent(n[o++])
         }))
     }
-    var mr = {
+    var _r = {
         WithinQueryParameters: 0,
         WithinHeaders: 1
     };
 
-    function dr(e, t) {
+    function br(e, t) {
         var n = e || {},
             r = n.data || {};
         return Object.keys(n).forEach((function(e) {
             -1 === ["timeout", "headers", "queryParameters", "data", "cacheable"].indexOf(e) && (r[e] = n[e])
         })), {
             data: Object.entries(r).length > 0 ? r : void 0,
             timeout: n.timeout || t,
             headers: n.headers || {},
             queryParameters: n.queryParameters || {},
             cacheable: n.cacheable
         }
     }
-    var hr = {
+    var gr = {
             Read: 1,
             Write: 2,
             Any: 3
         },
-        vr = 1;
+        Or = 1;
 
-    function yr(e) {
-        var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : vr;
+    function Sr(e) {
+        var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Or;
         return t(t({}, e), {}, {
             status: n,
             lastUpdate: Date.now()
         })
     }
 
-    function _r(e) {
+    function Er(e) {
         return "string" == typeof e ? {
             protocol: "https",
             url: e,
-            accept: hr.Any
+            accept: gr.Any
         } : {
             protocol: e.protocol || "https",
             url: e.url,
-            accept: e.accept || hr.Any
+            accept: e.accept || gr.Any
         }
     }
-    var br = "POST";
+    var wr = "POST";
 
-    function gr(e, n, r, o) {
+    function jr(e, n, r, o) {
         var c = [],
-            a = function(e, n) {
+            i = function(e, n) {
                 if ("GET" !== e.method && (void 0 !== e.data || void 0 !== n.data)) {
                     var r = Array.isArray(e.data) ? e.data : t(t({}, e.data), n.data);
                     return JSON.stringify(r)
                 }
             }(r, o),
             u = function(e, n) {
                 var r = t(t({}, e.headers), n.headers),
@@ -3735,28 +3796,28 @@
             }(e, o),
             l = r.method,
             s = "GET" !== r.method ? {} : t(t({}, r.data), o.data),
             f = t(t(t({
                 "x-algolia-agent": e.userAgent.value
             }, e.queryParameters), s), o.queryParameters),
             p = 0,
-            m = function t(n, i) {
+            m = function t(n, a) {
                 var s = n.pop();
                 if (void 0 === s) throw {
                     name: "RetryError",
                     message: "Unreachable hosts - your application id may be incorrect. If the error persists, contact support@algolia.com.",
-                    transporterStackTrace: wr(c)
+                    transporterStackTrace: Dr(c)
                 };
                 var m = {
-                        data: a,
+                        data: i,
                         headers: u,
                         method: l,
-                        url: Sr(s, r.path, f),
-                        connectTimeout: i(p, e.timeouts.connect),
-                        responseTimeout: i(p, o.timeout)
+                        url: Ir(s, r.path, f),
+                        connectTimeout: a(p, e.timeouts.connect),
+                        responseTimeout: a(p, o.timeout)
                     },
                     d = function(e) {
                         var t = {
                             request: m,
                             response: e,
                             host: s,
                             triesLeft: n.length
@@ -3777,16 +3838,16 @@
                                         }
                                     }(t.message, e)
                                 }
                             }(e)
                         },
                         onRetry: function(r) {
                             var o = d(r);
-                            return r.isTimedOut && p++, Promise.all([e.logger.info("Retryable failure", jr(o)), e.hostsCache.set(s, yr(s, r.isTimedOut ? 3 : 2))]).then((function() {
-                                return t(n, i)
+                            return r.isTimedOut && p++, Promise.all([e.logger.info("Retryable failure", Cr(o)), e.hostsCache.set(s, Sr(s, r.isTimedOut ? 3 : 2))]).then((function() {
+                                return t(n, a)
                             }))
                         },
                         onFail: function(e) {
                             throw d(e),
                                 function(e, t) {
                                     var n = e.content,
                                         r = e.status,
@@ -3798,15 +3859,15 @@
                                         return {
                                             name: "ApiError",
                                             message: e,
                                             status: t,
                                             transporterStackTrace: n
                                         }
                                     }(o, r, t)
-                                }(e, wr(c))
+                                }(e, Dr(c))
                         }
                     };
                 return e.requester.send(m).then((function(e) {
                     return function(e, t) {
                         return function(e) {
                             var t = e.status;
                             return e.isTimedOut || function(e) {
@@ -3817,126 +3878,126 @@
                         }(e) ? t.onRetry(e) : 2 == ~~(e.status / 100) ? t.onSucess(e) : t.onFail(e)
                     }(e, h)
                 }))
             };
         return function(e, t) {
             return Promise.all(t.map((function(t) {
                 return e.get(t, (function() {
-                    return Promise.resolve(yr(t))
+                    return Promise.resolve(Sr(t))
                 }))
             }))).then((function(e) {
                 var n = e.filter((function(e) {
                         return function(e) {
-                            return e.status === vr || Date.now() - e.lastUpdate > 12e4
+                            return e.status === Or || Date.now() - e.lastUpdate > 12e4
                         }(e)
                     })),
                     r = e.filter((function(e) {
                         return function(e) {
                             return 3 === e.status && Date.now() - e.lastUpdate <= 12e4
                         }(e)
                     })),
-                    o = [].concat(i(n), i(r));
+                    o = [].concat(a(n), a(r));
                 return {
                     getTimeout: function(e, t) {
                         return (0 === r.length && 0 === e ? 1 : r.length + 3 + e) * t
                     },
                     statelessHosts: o.length > 0 ? o.map((function(e) {
-                        return _r(e)
+                        return Er(e)
                     })) : t
                 }
             }))
         }(e.hostsCache, n).then((function(e) {
-            return m(i(e.statelessHosts).reverse(), e.getTimeout)
+            return m(a(e.statelessHosts).reverse(), e.getTimeout)
         }))
     }
 
-    function Or(e) {
+    function Pr(e) {
         var t = {
             value: "Algolia for JavaScript (".concat(e, ")"),
             add: function(e) {
                 var n = "; ".concat(e.segment).concat(void 0 !== e.version ? " (".concat(e.version, ")") : "");
                 return -1 === t.value.indexOf(n) && (t.value = "".concat(t.value).concat(n)), t
             }
         };
         return t
     }
 
-    function Sr(e, t, n) {
-        var r = Er(n),
+    function Ir(e, t, n) {
+        var r = kr(n),
             o = "".concat(e.protocol, "://").concat(e.url, "/").concat("/" === t.charAt(0) ? t.substr(1) : t);
         return r.length && (o += "?".concat(r)), o
     }
 
-    function Er(e) {
+    function kr(e) {
         return Object.keys(e).map((function(t) {
-            return pr("%s=%s", t, (n = e[t], "[object Object]" === Object.prototype.toString.call(n) || "[object Array]" === Object.prototype.toString.call(n) ? JSON.stringify(e[t]) : e[t]));
+            return yr("%s=%s", t, (n = e[t], "[object Object]" === Object.prototype.toString.call(n) || "[object Array]" === Object.prototype.toString.call(n) ? JSON.stringify(e[t]) : e[t]));
             var n
         })).join("&")
     }
 
-    function wr(e) {
+    function Dr(e) {
         return e.map((function(e) {
-            return jr(e)
+            return Cr(e)
         }))
     }
 
-    function jr(e) {
+    function Cr(e) {
         var n = e.request.headers["x-algolia-api-key"] ? {
             "x-algolia-api-key": "*****"
         } : {};
         return t(t({}, e), {}, {
             request: t(t({}, e.request), {}, {
                 headers: t(t({}, e.request.headers), n)
             })
         })
     }
-    var Pr = function(e) {
+    var xr = function(e) {
             var n = e.appId,
                 r = function(e, t, n) {
                     var r = {
                         "x-algolia-api-key": n,
                         "x-algolia-application-id": t
                     };
                     return {
                         headers: function() {
-                            return e === mr.WithinHeaders ? r : {}
+                            return e === _r.WithinHeaders ? r : {}
                         },
                         queryParameters: function() {
-                            return e === mr.WithinQueryParameters ? r : {}
+                            return e === _r.WithinQueryParameters ? r : {}
                         }
                     }
-                }(void 0 !== e.authMode ? e.authMode : mr.WithinHeaders, n, e.apiKey),
+                }(void 0 !== e.authMode ? e.authMode : _r.WithinHeaders, n, e.apiKey),
                 o = function(e) {
                     var t = e.hostsCache,
                         n = e.logger,
                         r = e.requester,
                         o = e.requestsCache,
-                        i = e.responsesCache,
-                        a = e.timeouts,
+                        a = e.responsesCache,
+                        i = e.timeouts,
                         u = e.userAgent,
                         l = e.hosts,
                         s = e.queryParameters,
                         f = {
                             hostsCache: t,
                             logger: n,
                             requester: r,
                             requestsCache: o,
-                            responsesCache: i,
-                            timeouts: a,
+                            responsesCache: a,
+                            timeouts: i,
                             userAgent: u,
                             headers: e.headers,
                             queryParameters: s,
                             hosts: l.map((function(e) {
-                                return _r(e)
+                                return Er(e)
                             })),
                             read: function(e, t) {
-                                var n = dr(t, f.timeouts.read),
+                                var n = br(t, f.timeouts.read),
                                     r = function() {
-                                        return gr(f, f.hosts.filter((function(e) {
-                                            return 0 != (e.accept & hr.Read)
+                                        return jr(f, f.hosts.filter((function(e) {
+                                            return 0 != (e.accept & gr.Read)
                                         })), e, n)
                                     };
                                 if (!0 !== (void 0 !== n.cacheable ? n.cacheable : e.cacheable)) return r();
                                 var o = {
                                     request: e,
                                     mappedRequestOptions: n,
                                     transporter: {
@@ -3958,153 +4019,153 @@
                                 }), {
                                     miss: function(e) {
                                         return f.responsesCache.set(o, e)
                                     }
                                 })
                             },
                             write: function(e, t) {
-                                return gr(f, f.hosts.filter((function(e) {
-                                    return 0 != (e.accept & hr.Write)
-                                })), e, dr(t, f.timeouts.write))
+                                return jr(f, f.hosts.filter((function(e) {
+                                    return 0 != (e.accept & gr.Write)
+                                })), e, br(t, f.timeouts.write))
                             }
                         };
                     return f
                 }(t(t({
                     hosts: [{
                         url: "".concat(n, "-dsn.algolia.net"),
-                        accept: hr.Read
+                        accept: gr.Read
                     }, {
                         url: "".concat(n, ".algolia.net"),
-                        accept: hr.Write
-                    }].concat(sr([{
+                        accept: gr.Write
+                    }].concat(hr([{
                         url: "".concat(n, "-1.algolianet.com")
                     }, {
                         url: "".concat(n, "-2.algolianet.com")
                     }, {
                         url: "".concat(n, "-3.algolianet.com")
                     }]))
                 }, e), {}, {
                     headers: t(t(t({}, r.headers()), {
                         "content-type": "application/x-www-form-urlencoded"
                     }), e.headers),
                     queryParameters: t(t({}, r.queryParameters()), e.queryParameters)
                 })),
-                i = {
+                a = {
                     transporter: o,
                     appId: n,
                     addAlgoliaAgent: function(e, t) {
                         o.userAgent.add({
                             segment: e,
                             version: t
                         })
                     },
                     clearCache: function() {
                         return Promise.all([o.requestsCache.clear(), o.responsesCache.clear()]).then((function() {}))
                     }
                 };
-            return fr(i, e.methods)
+            return vr(a, e.methods)
         },
-        Ir = function(e) {
+        Ar = function(e) {
             return function(t) {
                 var n = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                return fr({
+                return vr({
                     transporter: e.transporter,
                     appId: e.appId,
                     indexName: t
                 }, n.methods)
             }
         },
-        kr = function(e) {
+        Nr = function(e) {
             return function(n, r) {
                 var o = n.map((function(e) {
                     return t(t({}, e), {}, {
-                        params: Er(e.params || {})
+                        params: kr(e.params || {})
                     })
                 }));
                 return e.transporter.read({
-                    method: br,
+                    method: wr,
                     path: "1/indexes/*/queries",
                     data: {
                         requests: o
                     },
                     cacheable: !0
                 }, r)
             }
         },
-        Dr = function(e) {
+        Rr = function(e) {
             return function(n, r) {
                 return Promise.all(n.map((function(n) {
                     var o = n.params,
                         c = o.facetName,
-                        i = o.facetQuery,
-                        a = function(e, t) {
+                        a = o.facetQuery,
+                        i = function(e, t) {
                             if (null == e) return {};
                             var n, r, o = function(e, t) {
                                 if (null == e) return {};
                                 var n, r, o = {},
                                     c = Object.keys(e);
                                 for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || (o[n] = e[n]);
                                 return o
                             }(e, t);
                             if (Object.getOwnPropertySymbols) {
                                 var c = Object.getOwnPropertySymbols(e);
                                 for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
                             }
                             return o
-                        }(o, ir);
-                    return Ir(e)(n.indexName, {
+                        }(o, fr);
+                    return Ar(e)(n.indexName, {
                         methods: {
-                            searchForFacetValues: xr
+                            searchForFacetValues: qr
                         }
-                    }).searchForFacetValues(c, i, t(t({}, r), a))
+                    }).searchForFacetValues(c, a, t(t({}, r), i))
                 })))
             }
         },
-        Cr = function(e) {
+        Tr = function(e) {
             return function(t, n, r) {
                 return e.transporter.read({
-                    method: br,
-                    path: pr("1/answers/%s/prediction", e.indexName),
+                    method: wr,
+                    path: yr("1/answers/%s/prediction", e.indexName),
                     data: {
                         query: t,
                         queryLanguages: n
                     },
                     cacheable: !0
                 }, r)
             }
         },
-        Ar = function(e) {
+        Lr = function(e) {
             return function(t, n) {
                 return e.transporter.read({
-                    method: br,
-                    path: pr("1/indexes/%s/query", e.indexName),
+                    method: wr,
+                    path: yr("1/indexes/%s/query", e.indexName),
                     data: {
                         query: t
                     },
                     cacheable: !0
                 }, n)
             }
         },
-        xr = function(e) {
+        qr = function(e) {
             return function(t, n, r) {
                 return e.transporter.read({
-                    method: br,
-                    path: pr("1/indexes/%s/facets/%s/query", e.indexName, t),
+                    method: wr,
+                    path: yr("1/indexes/%s/facets/%s/query", e.indexName, t),
                     data: {
                         facetQuery: n
                     },
                     cacheable: !0
                 }, r)
             }
         },
-        Nr = 1,
-        Rr = 2,
-        Tr = 3;
+        Mr = 1,
+        Hr = 2,
+        Ur = 3;
 
-    function Lr(e, n, r) {
+    function Fr(e, n, r) {
         var o, c = {
             appId: e,
             apiKey: n,
             timeouts: {
                 connect: 1,
                 read: 2,
                 write: 30
@@ -4140,133 +4201,133 @@
                                 status: n.status,
                                 isTimedOut: !1
                             })
                         }, n.send(e.data)
                     }))
                 }
             },
-            logger: (o = Tr, {
+            logger: (o = Ur, {
                 debug: function(e, t) {
-                    return Nr >= o && console.debug(e, t), Promise.resolve()
+                    return Mr >= o && console.debug(e, t), Promise.resolve()
                 },
                 info: function(e, t) {
-                    return Rr >= o && console.info(e, t), Promise.resolve()
+                    return Hr >= o && console.info(e, t), Promise.resolve()
                 },
                 error: function(e, t) {
                     return console.error(e, t), Promise.resolve()
                 }
             }),
-            responsesCache: lr(),
-            requestsCache: lr({
+            responsesCache: dr(),
+            requestsCache: dr({
                 serializable: !1
             }),
-            hostsCache: ur({
-                caches: [ar({
+            hostsCache: mr({
+                caches: [pr({
                     key: "".concat("4.8.5", "-").concat(e)
-                }), lr()]
+                }), dr()]
             }),
-            userAgent: Or("4.8.5").add({
+            userAgent: Pr("4.8.5").add({
                 segment: "Browser",
                 version: "lite"
             }),
-            authMode: mr.WithinQueryParameters
+            authMode: _r.WithinQueryParameters
         };
-        return Pr(t(t(t({}, c), r), {}, {
+        return xr(t(t(t({}, c), r), {}, {
             methods: {
-                search: kr,
-                searchForFacetValues: Dr,
-                multipleQueries: kr,
-                multipleSearchForFacetValues: Dr,
+                search: Nr,
+                searchForFacetValues: Rr,
+                multipleQueries: Nr,
+                multipleSearchForFacetValues: Rr,
                 initIndex: function(e) {
                     return function(t) {
-                        return Ir(e)(t, {
+                        return Ar(e)(t, {
                             methods: {
-                                search: Ar,
-                                searchForFacetValues: xr,
-                                findAnswers: Cr
+                                search: Lr,
+                                searchForFacetValues: qr,
+                                findAnswers: Tr
                             }
                         })
                     }
                 }
             }
         }))
     }
-    Lr.version = "4.8.5";
-    var qr = ["footer", "searchBox"];
+    Fr.version = "4.8.5";
+    var Br = ["footer", "searchBox"];
 
-    function Mr() {
-        return Mr = Object.assign || function(e) {
+    function Vr() {
+        return Vr = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, Mr.apply(this, arguments)
+        }, Vr.apply(this, arguments)
     }
 
-    function Hr(e, t) {
+    function Wr(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Ur(e) {
+    function Kr(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Hr(Object(n), !0).forEach((function(t) {
-                Fr(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Hr(Object(n)).forEach((function(t) {
+            t % 2 ? Wr(Object(n), !0).forEach((function(t) {
+                zr(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Wr(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Fr(e, t, n) {
+    function zr(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function Br(e, t) {
+    function Jr(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function Vr(e) {
+    function $r(e) {
         var t = e.appId,
             n = e.apiKey,
             r = e.indexName,
             o = e.placeholder,
             c = void 0 === o ? "Search docs" : o,
-            i = e.searchParameters,
-            a = e.onClose,
-            u = void 0 === a ? Vn : a,
+            a = e.searchParameters,
+            i = e.onClose,
+            u = void 0 === i ? $n : i,
             l = e.transformItems,
-            s = void 0 === l ? Bn : l,
+            s = void 0 === l ? zn : l,
             f = e.hitComponent,
-            p = void 0 === f ? dn : f,
+            p = void 0 === f ? _n : f,
             m = e.resultsFooterComponent,
             d = void 0 === m ? function() {
                 return null
             } : m,
             h = e.navigator,
             v = e.initialScrollY,
             y = void 0 === v ? 0 : v,
             _ = e.transformSearchClient,
-            b = void 0 === _ ? Bn : _,
+            b = void 0 === _ ? zn : _,
             g = e.disableUserPersonalization,
             O = void 0 !== g && g,
             S = e.initialQuery,
             E = void 0 === S ? "" : S,
             w = e.translations,
             j = void 0 === w ? {} : w,
             P = e.getMissingResultsUrl,
@@ -4282,188 +4343,188 @@
                     return o
                 }(e, t);
                 if (Object.getOwnPropertySymbols) {
                     var c = Object.getOwnPropertySymbols(e);
                     for (r = 0; r < c.length; r++) n = c[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
                 }
                 return o
-            }(j, qr),
+            }(j, Br),
             C = function(e, t) {
                 return function(e) {
                     if (Array.isArray(e)) return e
                 }(e) || function(e, t) {
                     var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                     if (null != n) {
                         var r, o, c = [],
-                            i = !0,
-                            a = !1;
+                            a = !0,
+                            i = !1;
                         try {
-                            for (n = n.call(e); !(i = (r = n.next()).done) && (c.push(r.value), 2 !== c.length); i = !0);
+                            for (n = n.call(e); !(a = (r = n.next()).done) && (c.push(r.value), 2 !== c.length); a = !0);
                         } catch (e) {
-                            a = !0, o = e
+                            i = !0, o = e
                         } finally {
                             try {
-                                i || null == n.return || n.return()
+                                a || null == n.return || n.return()
                             } finally {
-                                if (a) throw o
+                                if (i) throw o
                             }
                         }
                         return c
                     }
                 }(e) || function(e, t) {
                     if (e) {
-                        if ("string" == typeof e) return Br(e, 2);
+                        if ("string" == typeof e) return Jr(e, 2);
                         var n = Object.prototype.toString.call(e).slice(8, -1);
-                        return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Br(e, 2) : void 0
+                        return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Jr(e, 2) : void 0
                     }
                 }(e) || function() {
                     throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                 }()
             }(Fe.useState({
                 query: "",
                 collections: [],
                 completion: null,
                 context: {},
                 isOpen: !1,
                 activeItemId: null,
                 status: "idle"
             })),
-            A = C[0],
-            x = C[1],
+            x = C[0],
+            A = C[1],
             N = Fe.useRef(null),
             R = Fe.useRef(null),
             T = Fe.useRef(null),
             L = Fe.useRef(null),
             q = Fe.useRef(null),
             M = Fe.useRef(10),
             H = Fe.useRef("undefined" != typeof window ? window.getSelection().toString().slice(0, 64) : "").current,
             U = Fe.useRef(E || H).current,
             F = function(e, t, n) {
                 return Fe.useMemo((function() {
-                    var r = Lr(e, t);
-                    return r.addAlgoliaAgent("docsearch", "3.3.3"), !1 === /docsearch.js \(.*\)/.test(r.transporter.userAgent.value) && r.addAlgoliaAgent("docsearch-react", "3.3.3"), n(r)
+                    var r = Fr(e, t);
+                    return r.addAlgoliaAgent("docsearch", "3.3.4"), !1 === /docsearch.js \(.*\)/.test(r.transporter.userAgent.value) && r.addAlgoliaAgent("docsearch-react", "3.3.4"), n(r)
                 }), [e, t, n])
             }(t, n, b),
-            B = Fe.useRef(cr({
+            B = Fe.useRef(sr({
                 key: "__DOCSEARCH_FAVORITE_SEARCHES__".concat(r),
                 limit: 10
             })).current,
-            V = Fe.useRef(cr({
+            V = Fe.useRef(sr({
                 key: "__DOCSEARCH_RECENT_SEARCHES__".concat(r),
                 limit: 0 === B.getAll().length ? 7 : 4
             })).current,
             W = Fe.useCallback((function(e) {
                 if (!O) {
                     var t = "content" === e.type ? e.__docsearch_parent : e;
                     t && -1 === B.getAll().findIndex((function(e) {
                         return e.objectID === t.objectID
                     })) && V.add(t)
                 }
             }), [B, V, O]),
             K = Fe.useMemo((function() {
-                return sn({
+                return dn({
                     id: "docsearch",
                     defaultActiveItemId: 0,
                     placeholder: c,
                     openOnFocus: !0,
                     initialState: {
                         query: U,
                         context: {
                             searchSuggestions: []
                         }
                     },
                     navigator: h,
                     onStateChange: function(e) {
-                        x(e.state)
+                        A(e.state)
                     },
                     getSources: function(e) {
                         var t = e.query,
                             n = e.state,
                             o = e.setContext,
                             c = e.setStatus;
                         return t ? F.search([{
                             query: t,
                             indexName: r,
-                            params: Ur({
+                            params: Kr({
                                 attributesToRetrieve: ["hierarchy.lvl0", "hierarchy.lvl1", "hierarchy.lvl2", "hierarchy.lvl3", "hierarchy.lvl4", "hierarchy.lvl5", "hierarchy.lvl6", "content", "type", "url"],
                                 attributesToSnippet: ["hierarchy.lvl1:".concat(M.current), "hierarchy.lvl2:".concat(M.current), "hierarchy.lvl3:".concat(M.current), "hierarchy.lvl4:".concat(M.current), "hierarchy.lvl5:".concat(M.current), "hierarchy.lvl6:".concat(M.current), "content:".concat(M.current)],
                                 snippetEllipsisText: "…",
                                 highlightPreTag: "<mark>",
                                 highlightPostTag: "</mark>",
                                 hitsPerPage: 20
-                            }, i)
+                            }, a)
                         }]).catch((function(e) {
                             throw "RetryError" === e.name && c("error"), e
                         })).then((function(e) {
                             var t = e.results[0],
                                 r = t.hits,
                                 c = t.nbHits,
-                                i = Fn(r, (function(e) {
-                                    return zn(e)
+                                a = Kn(r, (function(e) {
+                                    return Yn(e)
                                 }));
-                            return n.context.searchSuggestions.length < Object.keys(i).length && o({
-                                searchSuggestions: Object.keys(i)
+                            return n.context.searchSuggestions.length < Object.keys(a).length && o({
+                                searchSuggestions: Object.keys(a)
                             }), o({
                                 nbHits: c
-                            }), Object.values(i).map((function(e, t) {
+                            }), Object.values(a).map((function(e, t) {
                                 return {
                                     sourceId: "hits".concat(t),
                                     onSelect: function(e) {
                                         var t = e.item,
                                             n = e.event;
-                                        W(t), n.shiftKey || n.ctrlKey || n.metaKey || u()
+                                        W(t), Jn(n) || u()
                                     },
                                     getItemUrl: function(e) {
                                         return e.item.url
                                     },
                                     getItems: function() {
-                                        return Object.values(Fn(e, (function(e) {
+                                        return Object.values(Kn(e, (function(e) {
                                             return e.hierarchy.lvl1
                                         }))).map(s).map((function(e) {
                                             return e.map((function(t) {
-                                                return Ur(Ur({}, t), {}, {
+                                                return Kr(Kr({}, t), {}, {
                                                     __docsearch_parent: "lvl1" !== t.type && e.find((function(e) {
                                                         return "lvl1" === e.type && e.hierarchy.lvl1 === t.hierarchy.lvl1
                                                     }))
                                                 })
                                             }))
                                         })).flat()
                                     }
                                 }
                             }))
                         })) : O ? [] : [{
                             sourceId: "recentSearches",
                             onSelect: function(e) {
                                 var t = e.item,
                                     n = e.event;
-                                W(t), n.shiftKey || n.ctrlKey || n.metaKey || u()
+                                W(t), Jn(n) || u()
                             },
                             getItemUrl: function(e) {
                                 return e.item.url
                             },
                             getItems: function() {
                                 return V.getAll()
                             }
                         }, {
                             sourceId: "favoriteSearches",
                             onSelect: function(e) {
                                 var t = e.item,
                                     n = e.event;
-                                W(t), n.shiftKey || n.ctrlKey || n.metaKey || u()
+                                W(t), Jn(n) || u()
                             },
                             getItemUrl: function(e) {
                                 return e.item.url
                             },
                             getItems: function() {
                                 return B.getAll()
                             }
                         }]
                     }
                 })
-            }), [r, i, F, u, V, B, W, U, c, h, s, O]),
+            }), [r, a, F, u, V, B, W, U, c, h, s, O]),
             z = K.getEnvironmentProps,
             J = K.getRootProps,
             $ = K.refresh;
         return function(e) {
                 var t = e.getEnvironmentProps,
                     n = e.panelElement,
                     r = e.formElement,
@@ -4472,18 +4533,18 @@
                     if (n && r && o) {
                         var e = t({
                                 panelElement: n,
                                 formElement: r,
                                 inputElement: o
                             }),
                             c = e.onTouchStart,
-                            i = e.onTouchMove;
-                        return window.addEventListener("touchstart", c), window.addEventListener("touchmove", i),
+                            a = e.onTouchMove;
+                        return window.addEventListener("touchstart", c), window.addEventListener("touchmove", a),
                             function() {
-                                window.removeEventListener("touchstart", c), window.removeEventListener("touchmove", i)
+                                window.removeEventListener("touchstart", c), window.removeEventListener("touchmove", a)
                             }
                     }
                 }), [t, n, r, o])
             }({
                 getEnvironmentProps: z,
                 panelElement: L.current,
                 formElement: T.current,
@@ -4514,138 +4575,138 @@
                         var e, t;
                         document.body.classList.remove("DocSearch--active"), null === (e = (t = window).scrollTo) || void 0 === e || e.call(t, 0, y)
                     }
             }), []), Fe.useEffect((function() {
                 window.matchMedia("(max-width: 768px)").matches && (M.current = 5)
             }), []), Fe.useEffect((function() {
                 L.current && (L.current.scrollTop = 0)
-            }), [A.query]), Fe.useEffect((function() {
+            }), [x.query]), Fe.useEffect((function() {
                 U.length > 0 && ($(), q.current && q.current.focus())
             }), [U, $]), Fe.useEffect((function() {
                 function e() {
                     if (R.current) {
                         var e = .01 * window.innerHeight;
                         R.current.style.setProperty("--docsearch-vh", "".concat(e, "px"))
                     }
                 }
                 return e(), window.addEventListener("resize", e),
                     function() {
                         window.removeEventListener("resize", e)
                     }
-            }), []), Fe.createElement("div", Mr({
+            }), []), Fe.createElement("div", Vr({
                 ref: N
             }, J({
                 "aria-expanded": !0
             }), {
-                className: ["DocSearch", "DocSearch-Container", "stalled" === A.status && "DocSearch-Container--Stalled", "error" === A.status && "DocSearch-Container--Errored"].filter(Boolean).join(" "),
+                className: ["DocSearch", "DocSearch-Container", "stalled" === x.status && "DocSearch-Container--Stalled", "error" === x.status && "DocSearch-Container--Errored"].filter(Boolean).join(" "),
                 role: "button",
                 tabIndex: 0,
                 onMouseDown: function(e) {
                     e.target === e.currentTarget && u()
                 }
             }), Fe.createElement("div", {
                 className: "DocSearch-Modal",
                 ref: R
             }, Fe.createElement("header", {
                 className: "DocSearch-SearchBar",
                 ref: T
-            }, Fe.createElement(rr, Mr({}, K, {
-                state: A,
+            }, Fe.createElement(ur, Vr({}, K, {
+                state: x,
                 autoFocus: 0 === U.length,
                 inputRef: q,
                 isFromSelection: Boolean(U) && U === H,
                 translations: k,
                 onClose: u
             }))), Fe.createElement("div", {
                 className: "DocSearch-Dropdown",
                 ref: L
-            }, Fe.createElement(er, Mr({}, K, {
+            }, Fe.createElement(cr, Vr({}, K, {
                 indexName: r,
-                state: A,
+                state: x,
                 hitComponent: p,
                 resultsFooterComponent: d,
                 disableUserPersonalization: O,
                 recentSearches: V,
                 favoriteSearches: B,
                 inputRef: q,
                 translations: D,
                 getMissingResultsUrl: P,
-                onItemClick: function(e) {
-                    W(e), u()
+                onItemClick: function(e, t) {
+                    W(e), Jn(t) || u()
                 }
             }))), Fe.createElement("footer", {
                 className: "DocSearch-Footer"
-            }, Fe.createElement(mn, {
+            }, Fe.createElement(yn, {
                 translations: I
             }))))
     }
 
-    function Wr() {
-        return Wr = Object.assign || function(e) {
+    function Qr() {
+        return Qr = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
-        }, Wr.apply(this, arguments)
+        }, Qr.apply(this, arguments)
     }
 
-    function Kr(e, t) {
+    function Zr(e, t) {
         return function(e) {
             if (Array.isArray(e)) return e
         }(e) || function(e, t) {
             var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
             if (null != n) {
                 var r, o, c = [],
-                    i = !0,
-                    a = !1;
+                    a = !0,
+                    i = !1;
                 try {
-                    for (n = n.call(e); !(i = (r = n.next()).done) && (c.push(r.value), !t || c.length !== t); i = !0);
+                    for (n = n.call(e); !(a = (r = n.next()).done) && (c.push(r.value), !t || c.length !== t); a = !0);
                 } catch (e) {
-                    a = !0, o = e
+                    i = !0, o = e
                 } finally {
                     try {
-                        i || null == n.return || n.return()
+                        a || null == n.return || n.return()
                     } finally {
-                        if (a) throw o
+                        if (i) throw o
                     }
                 }
                 return c
             }
         }(e, t) || function(e, t) {
             if (e) {
-                if ("string" == typeof e) return zr(e, t);
+                if ("string" == typeof e) return Yr(e, t);
                 var n = Object.prototype.toString.call(e).slice(8, -1);
-                return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? zr(e, t) : void 0
+                return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Yr(e, t) : void 0
             }
         }(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
 
-    function zr(e, t) {
+    function Yr(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
 
-    function Jr(e) {
+    function Gr(e) {
         var t, n, r = Fe.useRef(null),
-            o = Kr(Fe.useState(!1), 2),
+            o = Zr(Fe.useState(!1), 2),
             c = o[0],
-            i = o[1],
-            a = Kr(Fe.useState((null == e ? void 0 : e.initialQuery) || void 0), 2),
-            u = a[0],
-            l = a[1],
+            a = o[1],
+            i = Zr(Fe.useState((null == e ? void 0 : e.initialQuery) || void 0), 2),
+            u = i[0],
+            l = i[1],
             s = Fe.useCallback((function() {
-                i(!0)
-            }), [i]),
+                a(!0)
+            }), [a]),
             f = Fe.useCallback((function() {
-                i(!1)
-            }), [i]);
+                a(!1)
+            }), [a]);
         return function(e) {
             var t = e.isOpen,
                 n = e.onOpen,
                 r = e.onClose,
                 o = e.onInput,
                 c = e.searchButtonRef;
             Fe.useEffect((function() {
@@ -4662,32 +4723,32 @@
                     }
             }), [t, n, r, o, c])
         }({
             isOpen: c,
             onOpen: s,
             onClose: f,
             onInput: Fe.useCallback((function(e) {
-                i(!0), l(e.key)
-            }), [i, l]),
+                a(!0), l(e.key)
+            }), [a, l]),
             searchButtonRef: r
         }), Fe.createElement(Fe.Fragment, null, Fe.createElement(Je, {
             ref: r,
             translations: null == e || null === (t = e.translations) || void 0 === t ? void 0 : t.button,
             onClick: s
-        }), c && Pe(Fe.createElement(Vr, Wr({}, e, {
+        }), c && Pe(Fe.createElement($r, Qr({}, e, {
             initialScrollY: window.scrollY,
             initialQuery: u,
             translations: null == e || null === (n = e.translations) || void 0 === n ? void 0 : n.modal,
             onClose: f
         })), document.body))
     }
     window.docsearch = function(e) {
-        Ce(Fe.createElement(Jr, o({}, e, {
+        Ce(Fe.createElement(Gr, o({}, e, {
             transformSearchClient: function(t) {
-                return t.addAlgoliaAgent("docsearch.js", "3.3.3"), e.transformSearchClient ? e.transformSearchClient(t) : t
+                return t.addAlgoliaAgent("docsearch.js", "3.3.4"), e.transformSearchClient ? e.transformSearchClient(t) : t
             }
         })), function(e) {
             var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : window;
             return "string" == typeof e ? t.document.querySelector(e) : e
         }(e.container, e.environment))
     }
 }();
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/docsearch.70ebcfe862b41f7a90b7.css` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch.f30f8b0589fd2b6fd39c.css`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1,2 @@
-/*! @docsearch/css 3.3.3 | MIT License | © Algolia, Inc. and contributors | https://docsearch.algolia.com */:root{--docsearch-primary-color:#5468ff;--docsearch-text-color:#1c1e21;--docsearch-spacing:12px;--docsearch-icon-stroke-width:1.4;--docsearch-highlight-color:var(--docsearch-primary-color);--docsearch-muted-color:#969faf;--docsearch-container-background:rgba(101,108,133,.8);--docsearch-logo-color:#5468ff;--docsearch-modal-width:560px;--docsearch-modal-height:600px;--docsearch-modal-background:#f5f6f7;--docsearch-modal-shadow:inset 1px 1px 0 0 hsla(0,0%,100%,.5),0 3px 8px 0 #555a64;--docsearch-searchbox-height:56px;--docsearch-searchbox-background:#ebedf0;--docsearch-searchbox-focus-background:#fff;--docsearch-searchbox-shadow:inset 0 0 0 2px var(--docsearch-primary-color);--docsearch-hit-height:56px;--docsearch-hit-color:#444950;--docsearch-hit-active-color:#fff;--docsearch-hit-background:#fff;--docsearch-hit-shadow:0 1px 3px 0 #d4d9e1;--docsearch-key-gradient:linear-gradient(-225deg,#d5dbe4,#f8f8f8);--docsearch-key-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);--docsearch-footer-height:44px;--docsearch-footer-background:#fff;--docsearch-footer-shadow:0 -1px 0 0 #e0e3e8,0 -3px 6px 0 rgba(69,98,155,.12)}html[data-theme=dark]{--docsearch-text-color:#f5f6f7;--docsearch-container-background:rgba(9,10,17,.8);--docsearch-modal-background:#15172a;--docsearch-modal-shadow:inset 1px 1px 0 0 #2c2e40,0 3px 8px 0 #000309;--docsearch-searchbox-background:#090a11;--docsearch-searchbox-focus-background:#000;--docsearch-hit-color:#bec3c9;--docsearch-hit-shadow:none;--docsearch-hit-background:#090a11;--docsearch-key-gradient:linear-gradient(-26.5deg,#565872,#31355b);--docsearch-key-shadow:inset 0 -2px 0 0 #282d55,inset 0 0 1px 1px #51577d,0 2px 2px 0 rgba(3,4,9,.3);--docsearch-footer-background:#1e2136;--docsearch-footer-shadow:inset 0 1px 0 0 rgba(73,76,106,.5),0 -4px 8px 0 rgba(0,0,0,.2);--docsearch-logo-color:#fff;--docsearch-muted-color:#7f8497}.DocSearch-Button{align-items:center;background:#ebedf0;background:var(--docsearch-searchbox-background);border:0;border-radius:40px;color:#969faf;color:var(--docsearch-muted-color);cursor:pointer;display:flex;font-weight:500;height:36px;justify-content:space-between;margin:0 0 0 16px;padding:0 8px;-webkit-user-select:none;-moz-user-select:none;user-select:none}.DocSearch-Button:active,.DocSearch-Button:focus,.DocSearch-Button:hover{background:#fff;background:var(--docsearch-searchbox-focus-background);box-shadow:inset 0 0 0 2px #5468ff;box-shadow:var(--docsearch-searchbox-shadow);color:#1c1e21;color:var(--docsearch-text-color);outline:none}.DocSearch-Button-Container{align-items:center;display:flex}.DocSearch-Search-Icon{stroke-width:1.6}.DocSearch-Button .DocSearch-Search-Icon{color:#1c1e21;color:var(--docsearch-text-color)}.DocSearch-Button-Placeholder{font-size:1rem;padding:0 12px 0 6px}.DocSearch-Button-Keys{display:flex;min-width:calc(40px + .8em)}.DocSearch-Button-Key{align-items:center;background:linear-gradient(-225deg,#d5dbe4,#f8f8f8);background:var(--docsearch-key-gradient);border:0;border-radius:3px;box-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);box-shadow:var(--docsearch-key-shadow);color:#969faf;color:var(--docsearch-muted-color);display:flex;height:18px;justify-content:center;margin-right:.4em;padding:0 0 2px;position:relative;top:-1px;width:20px}@media (max-width:768px){.DocSearch-Button-Keys,.DocSearch-Button-Placeholder{display:none}}.DocSearch--active{overflow:hidden!important}.DocSearch-Container,.DocSearch-Container *{box-sizing:border-box}.DocSearch-Container{background-color:rgba(101,108,133,.8);background-color:var(--docsearch-container-background);height:100vh;left:0;position:fixed;top:0;width:100vw;z-index:200}.DocSearch-Container a{-webkit-text-decoration:none;text-decoration:none}.DocSearch-Link{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;font:inherit;margin:0;padding:0}.DocSearch-Modal{background:#f5f6f7;background:var(--docsearch-modal-background);border-radius:6px;box-shadow:inset 1px 1px 0 0 hsla(0,0%,100%,.5),0 3px 8px 0 #555a64;box-shadow:var(--docsearch-modal-shadow);flex-direction:column;margin:60px auto auto;max-width:560px;max-width:var(--docsearch-modal-width);position:relative}.DocSearch-SearchBar{display:flex;padding:12px 12px 0;padding:var(--docsearch-spacing) var(--docsearch-spacing) 0}.DocSearch-Form{align-items:center;background:#fff;background:var(--docsearch-searchbox-focus-background);border-radius:4px;box-shadow:inset 0 0 0 2px #5468ff;box-shadow:var(--docsearch-searchbox-shadow);display:flex;height:56px;height:var(--docsearch-searchbox-height);margin:0;padding:0 12px;padding:0 var(--docsearch-spacing);position:relative;width:100%}.DocSearch-Input{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:transparent;border:0;color:#1c1e21;color:var(--docsearch-text-color);flex:1;font:inherit;font-size:1.2em;height:100%;outline:none;padding:0 0 0 8px;width:80%}.DocSearch-Input::-moz-placeholder{color:#969faf;color:var(--docsearch-muted-color);opacity:1}.DocSearch-Input::placeholder{color:#969faf;color:var(--docsearch-muted-color);opacity:1}.DocSearch-Input::-webkit-search-cancel-button,.DocSearch-Input::-webkit-search-decoration,.DocSearch-Input::-webkit-search-results-button,.DocSearch-Input::-webkit-search-results-decoration{display:none}.DocSearch-LoadingIndicator,.DocSearch-MagnifierLabel,.DocSearch-Reset{margin:0;padding:0}.DocSearch-MagnifierLabel,.DocSearch-Reset{align-items:center;color:#5468ff;color:var(--docsearch-highlight-color);display:flex;justify-content:center}.DocSearch-Container--Stalled .DocSearch-MagnifierLabel,.DocSearch-LoadingIndicator{display:none}.DocSearch-Container--Stalled .DocSearch-LoadingIndicator{align-items:center;color:#5468ff;color:var(--docsearch-highlight-color);display:flex;justify-content:center}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Reset{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);animation:none;-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;right:0}}.DocSearch-Reset{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);animation:fade-in .1s ease-in forwards;-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;padding:2px;right:0}.DocSearch-Reset[hidden]{display:none}.DocSearch-Reset:hover{color:#5468ff;color:var(--docsearch-highlight-color)}.DocSearch-LoadingIndicator svg,.DocSearch-MagnifierLabel svg{height:24px;width:24px}.DocSearch-Cancel{display:none}.DocSearch-Dropdown{max-height:488px;max-height:calc(var(--docsearch-modal-height) - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height));min-height:12px;min-height:var(--docsearch-spacing);overflow-y:auto;overflow-y:overlay;padding:0 12px;padding:0 var(--docsearch-spacing);scrollbar-color:#969faf #f5f6f7;scrollbar-color:var(--docsearch-muted-color) var(--docsearch-modal-background);scrollbar-width:thin}.DocSearch-Dropdown::-webkit-scrollbar{width:12px}.DocSearch-Dropdown::-webkit-scrollbar-track{background:transparent}.DocSearch-Dropdown::-webkit-scrollbar-thumb{background-color:#969faf;background-color:var(--docsearch-muted-color);border:3px solid #f5f6f7;border:3px solid var(--docsearch-modal-background);border-radius:20px}.DocSearch-Dropdown ul{list-style:none;margin:0;padding:0}.DocSearch-Label{font-size:.75em;line-height:1.6em}.DocSearch-Help,.DocSearch-Label{color:#969faf;color:var(--docsearch-muted-color)}.DocSearch-Help{font-size:.9em;margin:0;-webkit-user-select:none;-moz-user-select:none;user-select:none}.DocSearch-Title{font-size:1.2em}.DocSearch-Logo a{display:flex}.DocSearch-Logo svg{color:#5468ff;color:var(--docsearch-logo-color);margin-left:8px}.DocSearch-Hits:last-of-type{margin-bottom:24px}.DocSearch-Hits mark{background:none;color:#5468ff;color:var(--docsearch-highlight-color)}.DocSearch-HitsFooter{color:#969faf;color:var(--docsearch-muted-color);display:flex;font-size:.85em;justify-content:center;margin-bottom:12px;margin-bottom:var(--docsearch-spacing);padding:12px;padding:var(--docsearch-spacing)}.DocSearch-HitsFooter a{border-bottom:1px solid;color:inherit}.DocSearch-Hit{border-radius:4px;display:flex;padding-bottom:4px;position:relative}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--deleting{transition:none}}.DocSearch-Hit--deleting{opacity:0;transition:all .25s linear}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--favoriting{transition:none}}.DocSearch-Hit--favoriting{transform:scale(0);transform-origin:top center;transition:all .25s linear;transition-delay:.25s}.DocSearch-Hit a{background:#fff;background:var(--docsearch-hit-background);border-radius:4px;box-shadow:0 1px 3px 0 #d4d9e1;box-shadow:var(--docsearch-hit-shadow);display:block;padding-left:12px;padding-left:var(--docsearch-spacing);width:100%}.DocSearch-Hit-source{background:#f5f6f7;background:var(--docsearch-modal-background);color:#5468ff;color:var(--docsearch-highlight-color);font-size:.85em;font-weight:600;line-height:32px;margin:0 -4px;padding:8px 4px 0;position:sticky;top:0;z-index:10}.DocSearch-Hit-Tree{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);color:#969faf;color:var(--docsearch-muted-color);height:56px;height:var(--docsearch-hit-height);opacity:.5;width:24px}.DocSearch-Hit[aria-selected=true] a{background-color:#5468ff;background-color:var(--docsearch-highlight-color)}.DocSearch-Hit[aria-selected=true] mark{-webkit-text-decoration:underline;text-decoration:underline}.DocSearch-Hit-Container{align-items:center;color:#444950;color:var(--docsearch-hit-color);display:flex;flex-direction:row;height:56px;height:var(--docsearch-hit-height);padding:0 12px 0 0;padding:0 var(--docsearch-spacing) 0 0}.DocSearch-Hit-icon{height:20px;width:20px}.DocSearch-Hit-action,.DocSearch-Hit-icon{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);color:#969faf;color:var(--docsearch-muted-color)}.DocSearch-Hit-action{align-items:center;display:flex;height:22px;width:22px}.DocSearch-Hit-action svg{display:block;height:18px;width:18px}.DocSearch-Hit-action+.DocSearch-Hit-action{margin-left:6px}.DocSearch-Hit-action-button{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:inherit;cursor:pointer;padding:2px}svg.DocSearch-Hit-Select-Icon{display:none}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Select-Icon{display:block}.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:background-color .1s ease-in}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{transition:none}}.DocSearch-Hit-action-button:focus path,.DocSearch-Hit-action-button:hover path{fill:#fff}.DocSearch-Hit-content-wrapper{display:flex;flex:1 1 auto;flex-direction:column;font-weight:500;justify-content:center;line-height:1.2em;margin:0 8px;overflow-x:hidden;position:relative;text-overflow:ellipsis;white-space:nowrap;width:80%}.DocSearch-Hit-title{font-size:.9em}.DocSearch-Hit-path{color:#969faf;color:var(--docsearch-muted-color);font-size:.75em}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Tree,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-action,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-icon,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-path,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-text,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-title,.DocSearch-Hit[aria-selected=true] mark{color:#fff!important;color:var(--docsearch-hit-active-color)!important}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:none}}.DocSearch-ErrorScreen,.DocSearch-NoResults,.DocSearch-StartScreen{font-size:.9em;margin:0 auto;padding:36px 0;text-align:center;width:80%}.DocSearch-Screen-Icon{color:#969faf;color:var(--docsearch-muted-color);padding-bottom:12px}.DocSearch-NoResults-Prefill-List{display:inline-block;padding-bottom:24px;text-align:left}.DocSearch-NoResults-Prefill-List ul{display:inline-block;padding:8px 0 0}.DocSearch-NoResults-Prefill-List li{list-style-position:inside;list-style-type:"» "}.DocSearch-Prefill{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:1em;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;font-size:1em;font-weight:700;padding:0}.DocSearch-Prefill:focus,.DocSearch-Prefill:hover{outline:none;-webkit-text-decoration:underline;text-decoration:underline}.DocSearch-Footer{align-items:center;background:#fff;background:var(--docsearch-footer-background);border-radius:0 0 8px 8px;box-shadow:0 -1px 0 0 #e0e3e8,0 -3px 6px 0 rgba(69,98,155,.12);box-shadow:var(--docsearch-footer-shadow);display:flex;flex-direction:row-reverse;flex-shrink:0;height:44px;height:var(--docsearch-footer-height);justify-content:space-between;padding:0 12px;padding:0 var(--docsearch-spacing);position:relative;-webkit-user-select:none;-moz-user-select:none;user-select:none;width:100%;z-index:300}.DocSearch-Commands{color:#969faf;color:var(--docsearch-muted-color);display:flex;list-style:none;margin:0;padding:0}.DocSearch-Commands li{align-items:center;display:flex}.DocSearch-Commands li:not(:last-of-type){margin-right:.8em}.DocSearch-Commands-Key{align-items:center;background:linear-gradient(-225deg,#d5dbe4,#f8f8f8);background:var(--docsearch-key-gradient);border:0;border-radius:2px;box-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);box-shadow:var(--docsearch-key-shadow);color:#969faf;color:var(--docsearch-muted-color);display:flex;height:18px;justify-content:center;margin-right:.4em;padding:0 0 1px;width:20px}@media (max-width:768px){:root{--docsearch-spacing:10px;--docsearch-footer-height:40px}.DocSearch-Dropdown{height:100%}.DocSearch-Container{height:-webkit-fill-available;height:100vh;height:calc(var(--docsearch-vh, 1vh)*100);position:absolute}.DocSearch-Footer{border-radius:0;bottom:0;position:absolute}.DocSearch-Hit-content-wrapper{display:flex;position:relative;width:80%}.DocSearch-Modal{border-radius:0;box-shadow:none;height:-webkit-fill-available;height:100vh;height:calc(var(--docsearch-vh, 1vh)*100);margin:0;max-width:100%;width:100%}.DocSearch-Dropdown{max-height:calc(100vh - 112px);max-height:calc(var(--docsearch-vh, 1vh)*100 - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height))}.DocSearch-Cancel{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;flex:none;font:inherit;font-size:1em;font-weight:500;margin-left:12px;margin-left:var(--docsearch-spacing);outline:none;overflow:hidden;padding:0;-webkit-user-select:none;-moz-user-select:none;user-select:none;white-space:nowrap}.DocSearch-Commands,.DocSearch-Hit-Tree{display:none}}@keyframes fade-in{0%{opacity:0}to{opacity:1}}
+/*! @docsearch/css 3.3.4 | MIT License | © Algolia, Inc. and contributors | https://docsearch.algolia.com */:root{--docsearch-primary-color:#5468ff;--docsearch-text-color:#1c1e21;--docsearch-spacing:12px;--docsearch-icon-stroke-width:1.4;--docsearch-highlight-color:var(--docsearch-primary-color);--docsearch-muted-color:#969faf;--docsearch-container-background:rgba(101,108,133,.8);--docsearch-logo-color:#5468ff;--docsearch-modal-width:560px;--docsearch-modal-height:600px;--docsearch-modal-background:#f5f6f7;--docsearch-modal-shadow:inset 1px 1px 0 0 hsla(0,0%,100%,.5),0 3px 8px 0 #555a64;--docsearch-searchbox-height:56px;--docsearch-searchbox-background:#ebedf0;--docsearch-searchbox-focus-background:#fff;--docsearch-searchbox-shadow:inset 0 0 0 2px var(--docsearch-primary-color);--docsearch-hit-height:56px;--docsearch-hit-color:#444950;--docsearch-hit-active-color:#fff;--docsearch-hit-background:#fff;--docsearch-hit-shadow:0 1px 3px 0 #d4d9e1;--docsearch-key-gradient:linear-gradient(-225deg,#d5dbe4,#f8f8f8);--docsearch-key-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);--docsearch-footer-height:44px;--docsearch-footer-background:#fff;--docsearch-footer-shadow:0 -1px 0 0 #e0e3e8,0 -3px 6px 0 rgba(69,98,155,.12)}html[data-theme=dark]{--docsearch-text-color:#f5f6f7;--docsearch-container-background:rgba(9,10,17,.8);--docsearch-modal-background:#15172a;--docsearch-modal-shadow:inset 1px 1px 0 0 #2c2e40,0 3px 8px 0 #000309;--docsearch-searchbox-background:#090a11;--docsearch-searchbox-focus-background:#000;--docsearch-hit-color:#bec3c9;--docsearch-hit-shadow:none;--docsearch-hit-background:#090a11;--docsearch-key-gradient:linear-gradient(-26.5deg,#565872,#31355b);--docsearch-key-shadow:inset 0 -2px 0 0 #282d55,inset 0 0 1px 1px #51577d,0 2px 2px 0 rgba(3,4,9,.3);--docsearch-footer-background:#1e2136;--docsearch-footer-shadow:inset 0 1px 0 0 rgba(73,76,106,.5),0 -4px 8px 0 rgba(0,0,0,.2);--docsearch-logo-color:#fff;--docsearch-muted-color:#7f8497}.DocSearch-Button{align-items:center;background:#ebedf0;background:var(--docsearch-searchbox-background);border:0;border-radius:40px;color:#969faf;color:var(--docsearch-muted-color);cursor:pointer;display:flex;font-weight:500;height:36px;justify-content:space-between;margin:0 0 0 16px;padding:0 8px;-webkit-user-select:none;-moz-user-select:none;user-select:none}.DocSearch-Button:active,.DocSearch-Button:focus,.DocSearch-Button:hover{background:#fff;background:var(--docsearch-searchbox-focus-background);box-shadow:inset 0 0 0 2px #5468ff;box-shadow:var(--docsearch-searchbox-shadow);color:#1c1e21;color:var(--docsearch-text-color);outline:none}.DocSearch-Button-Container{align-items:center;display:flex}.DocSearch-Search-Icon{stroke-width:1.6}.DocSearch-Button .DocSearch-Search-Icon{color:#1c1e21;color:var(--docsearch-text-color)}.DocSearch-Button-Placeholder{font-size:1rem;padding:0 12px 0 6px}.DocSearch-Button-Keys{display:flex;min-width:calc(40px + .8em)}.DocSearch-Button-Key{align-items:center;background:linear-gradient(-225deg,#d5dbe4,#f8f8f8);background:var(--docsearch-key-gradient);border:0;border-radius:3px;box-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);box-shadow:var(--docsearch-key-shadow);color:#969faf;color:var(--docsearch-muted-color);display:flex;height:18px;justify-content:center;margin-right:.4em;padding:0 0 2px;position:relative;top:-1px;width:20px}@media (max-width:768px){.DocSearch-Button-Keys,.DocSearch-Button-Placeholder{display:none}}.DocSearch--active{overflow:hidden!important}.DocSearch-Container,.DocSearch-Container *{box-sizing:border-box}.DocSearch-Container{background-color:rgba(101,108,133,.8);background-color:var(--docsearch-container-background);height:100vh;left:0;position:fixed;top:0;width:100vw;z-index:200}.DocSearch-Container a{-webkit-text-decoration:none;text-decoration:none}.DocSearch-Link{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;font:inherit;margin:0;padding:0}.DocSearch-Modal{background:#f5f6f7;background:var(--docsearch-modal-background);border-radius:6px;box-shadow:inset 1px 1px 0 0 hsla(0,0%,100%,.5),0 3px 8px 0 #555a64;box-shadow:var(--docsearch-modal-shadow);flex-direction:column;margin:60px auto auto;max-width:560px;max-width:var(--docsearch-modal-width);position:relative}.DocSearch-SearchBar{display:flex;padding:12px 12px 0;padding:var(--docsearch-spacing) var(--docsearch-spacing) 0}.DocSearch-Form{align-items:center;background:#fff;background:var(--docsearch-searchbox-focus-background);border-radius:4px;box-shadow:inset 0 0 0 2px #5468ff;box-shadow:var(--docsearch-searchbox-shadow);display:flex;height:56px;height:var(--docsearch-searchbox-height);margin:0;padding:0 12px;padding:0 var(--docsearch-spacing);position:relative;width:100%}.DocSearch-Input{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:transparent;border:0;color:#1c1e21;color:var(--docsearch-text-color);flex:1;font:inherit;font-size:1.2em;height:100%;outline:none;padding:0 0 0 8px;width:80%}.DocSearch-Input::-moz-placeholder{color:#969faf;color:var(--docsearch-muted-color);opacity:1}.DocSearch-Input::placeholder{color:#969faf;color:var(--docsearch-muted-color);opacity:1}.DocSearch-Input::-webkit-search-cancel-button,.DocSearch-Input::-webkit-search-decoration,.DocSearch-Input::-webkit-search-results-button,.DocSearch-Input::-webkit-search-results-decoration{display:none}.DocSearch-LoadingIndicator,.DocSearch-MagnifierLabel,.DocSearch-Reset{margin:0;padding:0}.DocSearch-MagnifierLabel,.DocSearch-Reset{align-items:center;color:#5468ff;color:var(--docsearch-highlight-color);display:flex;justify-content:center}.DocSearch-Container--Stalled .DocSearch-MagnifierLabel,.DocSearch-LoadingIndicator{display:none}.DocSearch-Container--Stalled .DocSearch-LoadingIndicator{align-items:center;color:#5468ff;color:var(--docsearch-highlight-color);display:flex;justify-content:center}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Reset{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);animation:none;-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;right:0}}.DocSearch-Reset{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);animation:fade-in .1s ease-in forwards;-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;padding:2px;right:0}.DocSearch-Reset[hidden]{display:none}.DocSearch-Reset:hover{color:#5468ff;color:var(--docsearch-highlight-color)}.DocSearch-LoadingIndicator svg,.DocSearch-MagnifierLabel svg{height:24px;width:24px}.DocSearch-Cancel{display:none}.DocSearch-Dropdown{max-height:488px;max-height:calc(var(--docsearch-modal-height) - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height));min-height:12px;min-height:var(--docsearch-spacing);overflow-y:auto;overflow-y:overlay;padding:0 12px;padding:0 var(--docsearch-spacing);scrollbar-color:#969faf #f5f6f7;scrollbar-color:var(--docsearch-muted-color) var(--docsearch-modal-background);scrollbar-width:thin}.DocSearch-Dropdown::-webkit-scrollbar{width:12px}.DocSearch-Dropdown::-webkit-scrollbar-track{background:transparent}.DocSearch-Dropdown::-webkit-scrollbar-thumb{background-color:#969faf;background-color:var(--docsearch-muted-color);border:3px solid #f5f6f7;border:3px solid var(--docsearch-modal-background);border-radius:20px}.DocSearch-Dropdown ul{list-style:none;margin:0;padding:0}.DocSearch-Label{font-size:.75em;line-height:1.6em}.DocSearch-Help,.DocSearch-Label{color:#969faf;color:var(--docsearch-muted-color)}.DocSearch-Help{font-size:.9em;margin:0;-webkit-user-select:none;-moz-user-select:none;user-select:none}.DocSearch-Title{font-size:1.2em}.DocSearch-Logo a{display:flex}.DocSearch-Logo svg{color:#5468ff;color:var(--docsearch-logo-color);margin-left:8px}.DocSearch-Hits:last-of-type{margin-bottom:24px}.DocSearch-Hits mark{background:none;color:#5468ff;color:var(--docsearch-highlight-color)}.DocSearch-HitsFooter{color:#969faf;color:var(--docsearch-muted-color);display:flex;font-size:.85em;justify-content:center;margin-bottom:12px;margin-bottom:var(--docsearch-spacing);padding:12px;padding:var(--docsearch-spacing)}.DocSearch-HitsFooter a{border-bottom:1px solid;color:inherit}.DocSearch-Hit{border-radius:4px;display:flex;padding-bottom:4px;position:relative}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--deleting{transition:none}}.DocSearch-Hit--deleting{opacity:0;transition:all .25s linear}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--favoriting{transition:none}}.DocSearch-Hit--favoriting{transform:scale(0);transform-origin:top center;transition:all .25s linear;transition-delay:.25s}.DocSearch-Hit a{background:#fff;background:var(--docsearch-hit-background);border-radius:4px;box-shadow:0 1px 3px 0 #d4d9e1;box-shadow:var(--docsearch-hit-shadow);display:block;padding-left:12px;padding-left:var(--docsearch-spacing);width:100%}.DocSearch-Hit-source{background:#f5f6f7;background:var(--docsearch-modal-background);color:#5468ff;color:var(--docsearch-highlight-color);font-size:.85em;font-weight:600;line-height:32px;margin:0 -4px;padding:8px 4px 0;position:sticky;top:0;z-index:10}.DocSearch-Hit-Tree{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);color:#969faf;color:var(--docsearch-muted-color);height:56px;height:var(--docsearch-hit-height);opacity:.5;width:24px}.DocSearch-Hit[aria-selected=true] a{background-color:#5468ff;background-color:var(--docsearch-highlight-color)}.DocSearch-Hit[aria-selected=true] mark{-webkit-text-decoration:underline;text-decoration:underline}.DocSearch-Hit-Container{align-items:center;color:#444950;color:var(--docsearch-hit-color);display:flex;flex-direction:row;height:56px;height:var(--docsearch-hit-height);padding:0 12px 0 0;padding:0 var(--docsearch-spacing) 0 0}.DocSearch-Hit-icon{height:20px;width:20px}.DocSearch-Hit-action,.DocSearch-Hit-icon{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);color:#969faf;color:var(--docsearch-muted-color)}.DocSearch-Hit-action{align-items:center;display:flex;height:22px;width:22px}.DocSearch-Hit-action svg{display:block;height:18px;width:18px}.DocSearch-Hit-action+.DocSearch-Hit-action{margin-left:6px}.DocSearch-Hit-action-button{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:inherit;cursor:pointer;padding:2px}svg.DocSearch-Hit-Select-Icon{display:none}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Select-Icon{display:block}.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:background-color .1s ease-in}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{transition:none}}.DocSearch-Hit-action-button:focus path,.DocSearch-Hit-action-button:hover path{fill:#fff}.DocSearch-Hit-content-wrapper{display:flex;flex:1 1 auto;flex-direction:column;font-weight:500;justify-content:center;line-height:1.2em;margin:0 8px;overflow-x:hidden;position:relative;text-overflow:ellipsis;white-space:nowrap;width:80%}.DocSearch-Hit-title{font-size:.9em}.DocSearch-Hit-path{color:#969faf;color:var(--docsearch-muted-color);font-size:.75em}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Tree,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-action,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-icon,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-path,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-text,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-title,.DocSearch-Hit[aria-selected=true] mark{color:#fff!important;color:var(--docsearch-hit-active-color)!important}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:none}}.DocSearch-ErrorScreen,.DocSearch-NoResults,.DocSearch-StartScreen{font-size:.9em;margin:0 auto;padding:36px 0;text-align:center;width:80%}.DocSearch-Screen-Icon{color:#969faf;color:var(--docsearch-muted-color);padding-bottom:12px}.DocSearch-NoResults-Prefill-List{display:inline-block;padding-bottom:24px;text-align:left}.DocSearch-NoResults-Prefill-List ul{display:inline-block;padding:8px 0 0}.DocSearch-NoResults-Prefill-List li{list-style-position:inside;list-style-type:"» "}.DocSearch-Prefill{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:1em;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;font-size:1em;font-weight:700;padding:0}.DocSearch-Prefill:focus,.DocSearch-Prefill:hover{outline:none;-webkit-text-decoration:underline;text-decoration:underline}.DocSearch-Footer{align-items:center;background:#fff;background:var(--docsearch-footer-background);border-radius:0 0 8px 8px;box-shadow:0 -1px 0 0 #e0e3e8,0 -3px 6px 0 rgba(69,98,155,.12);box-shadow:var(--docsearch-footer-shadow);display:flex;flex-direction:row-reverse;flex-shrink:0;height:44px;height:var(--docsearch-footer-height);justify-content:space-between;padding:0 12px;padding:0 var(--docsearch-spacing);position:relative;-webkit-user-select:none;-moz-user-select:none;user-select:none;width:100%;z-index:300}.DocSearch-Commands{color:#969faf;color:var(--docsearch-muted-color);display:flex;list-style:none;margin:0;padding:0}.DocSearch-Commands li{align-items:center;display:flex}.DocSearch-Commands li:not(:last-of-type){margin-right:.8em}.DocSearch-Commands-Key{align-items:center;background:linear-gradient(-225deg,#d5dbe4,#f8f8f8);background:var(--docsearch-key-gradient);border:0;border-radius:2px;box-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);box-shadow:var(--docsearch-key-shadow);color:#969faf;color:var(--docsearch-muted-color);display:flex;height:18px;justify-content:center;margin-right:.4em;padding:0 0 1px;width:20px}@media (max-width:768px){:root{--docsearch-spacing:10px;--docsearch-footer-height:40px}.DocSearch-Dropdown{height:100%}.DocSearch-Container{height:-webkit-fill-available;height:100vh;height:calc(var(--docsearch-vh, 1vh)*100);position:absolute}.DocSearch-Footer{border-radius:0;bottom:0;position:absolute}.DocSearch-Hit-content-wrapper{display:flex;position:relative;width:80%}.DocSearch-Modal{border-radius:0;box-shadow:none;height:-webkit-fill-available;height:100vh;height:calc(var(--docsearch-vh, 1vh)*100);margin:0;max-width:100%;width:100%}.DocSearch-Dropdown{max-height:calc(100vh - 112px);max-height:calc(var(--docsearch-vh, 1vh)*100 - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height))}.DocSearch-Cancel{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;flex:none;font:inherit;font-size:1em;font-weight:500;margin-left:12px;margin-left:var(--docsearch-spacing);outline:none;overflow:hidden;padding:0;-webkit-user-select:none;-moz-user-select:none;user-select:none;white-space:nowrap}.DocSearch-Commands,.DocSearch-Hit-Tree{display:none}}@keyframes fade-in{0%{opacity:0}to{opacity:1}}
+:root{--docsearch-searchbox-background:transparent;--docsearch-searchbox-shadow:inset 0 0 0 2px var(--color-brand);--docsearch-key-gradient:transparent;--docsearch-primary-color:var(--color-brand);--docsearch-modal-width:960px;--docsearch-modal-background:#fff}.DocSearch-Button{border-radius:0;height:3.5rem;line-height:3.5rem;padding-right:1rem}.DocSearch-Button-Key{font-family:Roboto,sans-serif;font-size:.875rem;height:1.25rem;padding:1rem}.DocSearch-Button:hover .DocSearch-Button-Key{border-color:var(--color-gray-dark);color:var(--color-gray-dark)}.DocSearch-Button .DocSearch-Search-Icon{--tw-text-opacity:1;stroke-width:2.5;color:#f3f4f6;color:rgb(243 244 246/var(--tw-text-opacity))}.DocSearch-Button:hover .DocSearch-Search-Icon{color:var(--docsearch-text-color)}.DocSearch-Button-Placeholder{padding-left:.75rem}.DocSearch-Hit-source{color:var(--color-gray-dark)}.DocSearch-Hit a{--tw-border-opacity:1;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;border-color:#f3f4f6;border-color:rgb(243 244 246/var(--tw-border-opacity));border-radius:.125rem;border-width:1px;box-shadow:0 0 transparent,0 0 transparent,0 0 transparent;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.DocSearch-Modal{border-radius:.125rem}
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/e10742dbb1d4a0864ba8.woff2` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/e10742dbb1d4a0864ba8.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/f1e2a76794cb86b2aa8e.woff` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/f1e2a76794cb86b2aa8e.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/f25d774ecfe0996f8eb5.woff2` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/f25d774ecfe0996f8eb5.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/manifest.json` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/manifest.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6551724137931034%*

 * *Differences: {"'_static/awesome-sphinx-design.css'": "'_static/awesome-sphinx-design.4ff695238f641b0a2852.css'",*

 * * "'_static/awesome-sphinx-design.js'": "'_static/awesome-sphinx-design.31d6cfe0d16ae931b73c.js'",*

 * * "'_static/docsearch.css'": "'_static/docsearch.f30f8b0589fd2b6fd39c.css'",*

 * * "'_static/docsearch.js'": "'_static/docsearch.f1a1a5835ed7a6ab0c85.js'",*

 * * "'_static/jetbrains-mono-latin-700-italic.woff'": "'_static/0ffeb7a552b36437b54c.woff'",*

 * * "'_static/jetbrains-mono-latin-700-italic.woff2'": "'_static/c3b5f43fe4c8 […]*

```diff
@@ -1,25 +1,29 @@
 {
-    "_static/docsearch.css": "_static/docsearch.70ebcfe862b41f7a90b7.css",
-    "_static/docsearch.js": "_static/docsearch.53303c497cdefb581f6f.js",
+    "_static/awesome-sphinx-design.css": "_static/awesome-sphinx-design.4ff695238f641b0a2852.css",
+    "_static/awesome-sphinx-design.js": "_static/awesome-sphinx-design.31d6cfe0d16ae931b73c.js",
+    "_static/docsearch.css": "_static/docsearch.f30f8b0589fd2b6fd39c.css",
+    "_static/docsearch.js": "_static/docsearch.f1a1a5835ed7a6ab0c85.js",
     "_static/docsearch_config.js_t": "_static/docsearch_config.js_t",
     "_static/jetbrains-mono-latin-400-italic.woff": "_static/ad463ea60cc8b68792f4.woff",
     "_static/jetbrains-mono-latin-400-italic.woff2": "_static/ff058b7e238adc5cba09.woff2",
     "_static/jetbrains-mono-latin-400-normal.woff": "_static/6f04107ce68d524ebe69.woff",
     "_static/jetbrains-mono-latin-400-normal.woff2": "_static/d0b41bd1d599bc0a52b7.woff2",
     "_static/jetbrains-mono-latin-500-italic.woff": "_static/09be83022f2ac2ce16b0.woff",
     "_static/jetbrains-mono-latin-500-italic.woff2": "_static/31f64b9c465158bd6066.woff2",
     "_static/jetbrains-mono-latin-500-normal.woff": "_static/46830c334f8112fa510a.woff",
     "_static/jetbrains-mono-latin-500-normal.woff2": "_static/ec416b97881f4a422686.woff2",
-    "_static/jetbrains-mono-latin-600-normal.woff": "_static/42ba3027499c19034257.woff",
-    "_static/jetbrains-mono-latin-600-normal.woff2": "_static/a49e53c029ef019e7422.woff2",
+    "_static/jetbrains-mono-latin-700-italic.woff": "_static/0ffeb7a552b36437b54c.woff",
+    "_static/jetbrains-mono-latin-700-italic.woff2": "_static/c3b5f43fe4c8f3f1fa21.woff2",
+    "_static/jetbrains-mono-latin-700-normal.woff": "_static/44fd0da18fe361a5cc7f.woff",
+    "_static/jetbrains-mono-latin-700-normal.woff2": "_static/cfdd43ce3499ca7f900a.woff2",
     "_static/roboto-latin-400-italic.woff": "_static/d037cb4792991826de7d.woff",
     "_static/roboto-latin-400-italic.woff2": "_static/e10742dbb1d4a0864ba8.woff2",
     "_static/roboto-latin-400-normal.woff": "_static/f1e2a76794cb86b2aa8e.woff",
     "_static/roboto-latin-400-normal.woff2": "_static/b009a76ad6afe4ebd301.woff2",
     "_static/roboto-latin-500-italic.woff": "_static/9ac5da2442b734abc516.woff",
     "_static/roboto-latin-500-italic.woff2": "_static/3a43b67e5bbdfb3ab0a6.woff2",
     "_static/roboto-latin-500-normal.woff": "_static/48af7707fe9e6494d6a5.woff",
     "_static/roboto-latin-500-normal.woff2": "_static/f25d774ecfe0996f8eb5.woff2",
-    "_static/theme.css": "_static/theme.2e8060a090e1247124e3.css",
-    "_static/theme.js": "_static/theme.b62e1ded0c8c099a2d47.js"
+    "_static/theme.css": "_static/theme.c973b470ab69573097f3.css",
+    "_static/theme.js": "_static/theme.c8991bd7bb6e57cbeea8.js"
 }
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/static/theme.b62e1ded0c8c099a2d47.js` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/theme.c8991bd7bb6e57cbeea8.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,16 @@
-/*! For license information please see theme.b62e1ded0c8c099a2d47.js.LICENSE.txt */ ! function() {
+/*! For license information please see theme.c8991bd7bb6e57cbeea8.js.LICENSE.txt */ ! function() {
     var e = {
             798: function(e, t, r) {
                 var n = {
                     "./clipboard-controller.js": 890,
                     "./code-controller.js": 606,
                     "./collapsible-controller.js": 635,
                     "./scroll-controller.js": 850,
+                    "./scroll-to-top-controller.js": 625,
                     "./search-controller.js": 935,
                     "./sidebar-controller.js": 214
                 };
 
                 function s(e) {
                     var t = i(e);
                     return r(t)
@@ -567,15 +568,15 @@
                     selectorMatched(e) {
                         this.delegate.selectorMatched && (this.delegate.selectorMatched(e, this.selector, this.details), this.matchesByElement.add(this.selector, e))
                     }
                     selectorUnmatched(e) {
                         this.delegate.selectorUnmatched(e, this.selector, this.details), this.matchesByElement.delete(this.selector, e)
                     }
                 }
-                class A {
+                class w {
                     constructor(e, t) {
                         this.element = e, this.delegate = t, this.started = !1, this.stringMap = new Map, this.mutationObserver = new MutationObserver((e => this.processMutations(e)))
                     }
                     start() {
                         this.started || (this.started = !0, this.mutationObserver.observe(this.element, {
                             attributes: !0,
                             attributeOldValue: !0
@@ -622,15 +623,15 @@
                     get currentAttributeNames() {
                         return Array.from(this.element.attributes).map((e => e.name))
                     }
                     get recordedAttributeNames() {
                         return Array.from(this.stringMap.keys())
                     }
                 }
-                class O {
+                class A {
                     constructor(e, t, r) {
                         this.attributeObserver = new v(e, t, this), this.delegate = r, this.tokensByElement = new b
                     }
                     get started() {
                         return this.attributeObserver.started
                     }
                     start() {
@@ -698,17 +699,17 @@
                                 attributeName: r,
                                 content: e,
                                 index: n
                             })))
                         }(e.getAttribute(t) || "", e, t)
                     }
                 }
-                class w {
+                class O {
                     constructor(e, t, r) {
-                        this.tokenListObserver = new O(e, t, this), this.delegate = r, this.parseResultsByToken = new WeakMap, this.valuesByTokenByElement = new WeakMap
+                        this.tokenListObserver = new A(e, t, this), this.delegate = r, this.parseResultsByToken = new WeakMap, this.valuesByTokenByElement = new WeakMap
                     }
                     get started() {
                         return this.tokenListObserver.started
                     }
                     start() {
                         this.tokenListObserver.start()
                     }
@@ -761,15 +762,15 @@
                     }
                 }
                 class k {
                     constructor(e, t) {
                         this.context = e, this.delegate = t, this.bindingsByAction = new Map
                     }
                     start() {
-                        this.valueListObserver || (this.valueListObserver = new w(this.element, this.actionAttribute, this), this.valueListObserver.start())
+                        this.valueListObserver || (this.valueListObserver = new O(this.element, this.actionAttribute, this), this.valueListObserver.start())
                     }
                     stop() {
                         this.valueListObserver && (this.valueListObserver.stop(), delete this.valueListObserver, this.disconnectAllActions())
                     }
                     get element() {
                         return this.context.element
                     }
@@ -805,15 +806,15 @@
                     }
                     elementUnmatchedValue(e, t) {
                         this.disconnectAction(t)
                     }
                 }
                 class T {
                     constructor(e, t) {
-                        this.context = e, this.receiver = t, this.stringMapObserver = new A(this.element, this), this.valueDescriptorMap = this.controller.valueDescriptorMap
+                        this.context = e, this.receiver = t, this.stringMapObserver = new w(this.element, this), this.valueDescriptorMap = this.controller.valueDescriptorMap
                     }
                     start() {
                         this.stringMapObserver.start(), this.invokeChangedCallbacksForDefaultValues()
                     }
                     stop() {
                         this.stringMapObserver.stop()
                     }
@@ -880,15 +881,15 @@
                     }
                 }
                 class M {
                     constructor(e, t) {
                         this.context = e, this.delegate = t, this.targetsByName = new b
                     }
                     start() {
-                        this.tokenListObserver || (this.tokenListObserver = new O(this.element, this.attributeName, this), this.tokenListObserver.start())
+                        this.tokenListObserver || (this.tokenListObserver = new A(this.element, this.attributeName, this), this.tokenListObserver.start())
                     }
                     stop() {
                         this.tokenListObserver && (this.disconnectAllTargets(), this.tokenListObserver.stop(), delete this.tokenListObserver)
                     }
                     tokenMatched({
                         element: e,
                         content: t
@@ -1387,15 +1388,15 @@
                     }
                     get documentScope() {
                         return this.isDocumentScope ? this : new P(this.schema, document.documentElement, this.identifier, this.guide.logger)
                     }
                 }
                 class R {
                     constructor(e, t, r) {
-                        this.element = e, this.schema = t, this.delegate = r, this.valueListObserver = new w(this.element, this.controllerAttribute, this), this.scopesByIdentifierByElement = new WeakMap, this.scopeReferenceCounts = new WeakMap
+                        this.element = e, this.schema = t, this.delegate = r, this.valueListObserver = new O(this.element, this.controllerAttribute, this), this.scopesByIdentifierByElement = new WeakMap, this.scopeReferenceCounts = new WeakMap
                     }
                     start() {
                         this.valueListObserver.start()
                     }
                     stop() {
                         this.valueListObserver.stop()
                     }
@@ -1568,109 +1569,109 @@
                 }
 
                 function W([e, t], r) {
                     return function(e) {
                         const t = `${h(e.token)}-value`,
                             r = function(e) {
                                 const t = function(e) {
-                                        const t = H(e.typeObject.type);
+                                        const t = Q(e.typeObject.type);
                                         if (!t) return;
-                                        const r = Q(e.typeObject.default);
+                                        const r = H(e.typeObject.default);
                                         if (t !== r) {
                                             throw new Error(`The specified default value for the Stimulus Value "${e.controller?`${e.controller}.${e.token}`:e.token}" must match the defined type "${t}". The provided default value of "${e.typeObject.default}" is of type "${r}".`)
                                         }
                                         return t
                                     }({
                                         controller: e.controller,
                                         token: e.token,
                                         typeObject: e.typeDefinition
                                     }),
-                                    r = Q(e.typeDefinition),
-                                    n = H(e.typeDefinition),
+                                    r = H(e.typeDefinition),
+                                    n = Q(e.typeDefinition),
                                     s = t || r || n;
                                 if (s) return s;
                                 throw new Error(`Unknown value type "${e.controller?`${e.controller}.${e.typeDefinition}`:e.token}" for "${e.token}" value`)
                             }(e);
                         return {
                             type: r,
                             key: t,
                             name: a(t),
                             get defaultValue() {
                                 return function(e) {
-                                    const t = H(e);
-                                    if (t) return J[t];
+                                    const t = Q(e);
+                                    if (t) return Y[t];
                                     const r = e.default;
                                     return void 0 !== r ? r : e
                                 }(e.typeDefinition)
                             },
                             get hasCustomDefaultValue() {
-                                return void 0 !== Q(e.typeDefinition)
+                                return void 0 !== H(e.typeDefinition)
                             },
-                            reader: Y[r],
+                            reader: J[r],
                             writer: X[r] || X.default
                         }
                     }({
                         controller: r,
                         token: e,
                         typeDefinition: t
                     })
                 }
 
-                function H(e) {
+                function Q(e) {
                     switch (e) {
                         case Array:
                             return "array";
                         case Boolean:
                             return "boolean";
                         case Number:
                             return "number";
                         case Object:
                             return "object";
                         case String:
                             return "string"
                     }
                 }
 
-                function Q(e) {
+                function H(e) {
                     switch (typeof e) {
                         case "boolean":
                             return "boolean";
                         case "number":
                             return "number";
                         case "string":
                             return "string"
                     }
                     return Array.isArray(e) ? "array" : "[object Object]" === Object.prototype.toString.call(e) ? "object" : void 0
                 }
-                const J = {
+                const Y = {
                         get array() {
                             return []
                         },
                         boolean: !1,
                         number: 0,
                         get object() {
                             return {}
                         },
                         string: ""
                     },
-                    Y = {
+                    J = {
                         array(e) {
                             const t = JSON.parse(e);
-                            if (!Array.isArray(t)) throw new TypeError(`expected value of type "array" but instead got value "${e}" of type "${Q(t)}"`);
+                            if (!Array.isArray(t)) throw new TypeError(`expected value of type "array" but instead got value "${e}" of type "${H(t)}"`);
                             return t
                         },
                         boolean(e) {
                             return !("0" == e || "false" == String(e).toLowerCase())
                         },
                         number(e) {
                             return Number(e)
                         },
                         object(e) {
                             const t = JSON.parse(e);
-                            if (null === t || "object" != typeof t || Array.isArray(t)) throw new TypeError(`expected value of type "object" but instead got value "${e}" of type "${Q(t)}"`);
+                            if (null === t || "object" != typeof t || Array.isArray(t)) throw new TypeError(`expected value of type "object" but instead got value "${e}" of type "${H(t)}"`);
                             return t
                         },
                         string(e) {
                             return e
                         }
                     },
                     X = {
@@ -1912,30 +1913,27 @@
                             t.classList.add("copy"), t.setAttribute("data-code-target", "button"), t.setAttribute("data-action", "code#copy"), t.textContent = this.label, e.appendChild(t)
                         }
                     }
                     copy() {
                         const e = new(i())(this.pre, {
                             target: () => this.pre
                         });
-                        e.on("success", (e => {
+                        e.on("success", (() => {
                             this.hasButtonTarget && (this.buttonTarget.textContent = "copied!", setTimeout((() => this.buttonTarget.textContent = this.label), 1500))
                         })), e.on("error", (e => {
                             console.error(e.action), console.error(e.trigger)
                         }))
                     }
                 }
             },
             635: function(e, t, r) {
                 "use strict";
                 r.r(t);
                 var n = r(599);
                 t.default = class extends n.Qr {
-                    expandAccordion(e) {
-                        this.expand(e.target)
-                    }
                     expandMore(e) {
                         this.expand(e.target.parentNode)
                     }
                     expand(e) {
                         e.classList.toggle("active");
                         const t = e.querySelector("button.expand-more");
                         e.classList.contains("active") ? (t.setAttribute("aria-expanded", "true"), t.setAttribute("aria-label", "Collapse this section")) : (t.setAttribute("aria-expanded", "false"), t.setAttribute("aria-label", "Expand this section"))
@@ -1943,40 +1941,64 @@
                 }
             },
             850: function(e, t, r) {
                 "use strict";
                 r.r(t);
                 var n = r(599);
                 t.default = class extends n.Qr {
-                    static targets = ["scrollToTop", "main"];
-                    initialize() {
+                    connect() {
                         const e = document.querySelectorAll("article section"),
                             t = {
                                 root: this.element,
                                 rootMargin: "0px 0px -95% 0px"
                             },
-                            r = new IntersectionObserver((e => {
-                                e.forEach((e => {
-                                    const t = document.querySelector(`.nav-toc a[href*=${e.target.id}]`);
-                                    e.isIntersecting && t ? t.classList.add("current") : t && t.classList.remove("current")
-                                }))
-                            }), t);
+                            r = new IntersectionObserver(this._highlightCurrentSection, t);
                         e.forEach((e => {
                             r.observe(e)
                         }))
                     }
-                    scrollToTop() {
-                        this.mainTarget.scrollTop = 0, window.scrollTo(0, 0), this.scrollToTopTarget.blur()
+                    _highlightCurrentSection(e) {
+                        e.forEach((e => {
+                            const t = document.querySelector(`.nav-toc a[href*=${e.target.id}]`);
+                            e.isIntersecting && t ? t.classList.add("current") : t && t.classList.remove("current")
+                        }))
+                    }
+                }
+            },
+            625: function(e, t, r) {
+                "use strict";
+                r.r(t);
+                var n = r(599);
+                t.default = class extends n.Qr {
+                    static targets = ["scrollToTop", "main"];
+                    connect() {
+                        this.lastPosition = 0, this.offset = 200
+                    }
+                    scroll() {
+                        this.scrollWindow.scrollTop = 0, window.scrollTo({
+                            top: 0,
+                            left: 0,
+                            behavior: "smooth"
+                        }), this.scrollToTopTarget.blur()
                     }
                     showButton() {
-                        if (this.hasScrollToTopTarget) {
-                            const e = this.scrollToTopTarget;
-                            this.mainTarget.scrollTop > 100 || window.scrollY > 100 ? e.classList.add("isShown") : e.classList.remove("isShown")
+                        if (this.hasScrollToTopTarget && this.hasMainTarget) {
+                            const e = this.mainTarget.scrollTop > this.offset || window.scrollY > this.offset;
+                            if (this.mainTarget.scrollTop > 0 && 0 === window.scrollY) {
+                                const t = this.mainTarget.scrollTop < this.lastPosition;
+                                this.toggleClass(e && t), this.lastPosition = this.mainTarget.scrollTop
+                            } else if (window.scrollY > 0 && 0 === this.mainTarget.scrollTop) {
+                                const t = window.scrollY < this.lastPosition;
+                                this.toggleClass(e && t), this.lastPosition = window.scrollY
+                            }
                         }
                     }
+                    toggleClass(e) {
+                        e ? this.scrollToTopTarget.classList.add("isShown") : this.scrollToTopTarget.classList.remove("isShown")
+                    }
                 }
             },
             935: function(e, t, r) {
                 "use strict";
                 r.r(t);
                 var n = r(599);
                 t.default = class extends n.Qr {
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/with-sidebar.html` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/with-sidebar.html`

 * *Files 12% similar despite different names*

```diff
@@ -9,35 +9,37 @@
 {% block document %}
 <aside data-sidebar-target="sidebar" class="grid-area-sidebar h-full fixed pt-14 xl:relative inset-y-0 left-0 z-20 xl:z-0 print:hidden overflow-y-auto transition-all transform transform-gpu -translate-x-full opacity-0 duration-300 xl:translate-x-0 xl:opacity-100">
   {% include "sidebar.html" %}
 </aside>
 
 <main
   {%- if theme_show_scrolltop|tobool %}
-  data-action="scroll->scroll#showButton"
-  data-scroll-target="main"
+  data-action="scroll->scroll-to-top#showButton"
+  data-scroll-to-top-target="main"
   {%- endif %}
   class="px-4 pt-14 xl:ml-fluid grid-area-main overflow-y-auto flex flex-col flex-1 h-full mx-0 md:mx-auto xl:mr-0"
 >
   {%- if pagename != master_doc and theme_show_breadcrumbs|tobool %}
     {%- include "breadcrumbs.html" %}
-  {% endif -%}
+  {%- endif %}
 
-  <article role="main" class="flex-1">
+  <article role="main" class="flex-1 prose">
     {% block body %}{% endblock %}
   </article>
 
   {%- if theme_show_prev_next|tobool %}
     {%- include "prev_next.html" %}
   {%- endif %}
 
+  {%- block extrabody %}{%- endblock %}
+
   <footer>
-    {% block footer %}
-      {% include "footer.html" %}
-    {% endblock %}
+    {%- block footer %}
+      {%- include "footer.html" %}
+    {%- endblock %}
   </footer>
 
   {#- scroll to top button -#}
   {%- if theme_show_scrolltop|tobool -%}
     {%- include "scrolltop.html" %}
   {%- endif -%}
 </main>
```

### Comparing `sphinxawesome_theme-4.0.3/src/sphinxawesome_theme/without-sidebar.html` & `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/without-sidebar.html`

 * *Files 14% similar despite different names*

```diff
@@ -6,32 +6,34 @@
 
 {% extends "layout.html" %}
 
 
 {% block document %}
 <main
   {%- if theme_show_scrolltop|tobool %}
-  data-action="scroll->scroll#showButton"
-  data-scroll-target="main"
+  data-action="scroll->scroll-to-top#showButton"
+  data-scroll-to-top-target="main"
   {%- endif %}
-  class="px-4 pt-14 col-span-full overflow-y-auto flex flex-col flex-1 h-full w-full"
+  class="px-4 pt-14 grid-area-main overflow-y-auto flex flex-col flex-1 h-full w-full"
   >
-  <div class="flex flex-col h-full mx-auto max-w-prose">
+  <div class="flex flex-col h-full max-w-prose">
     {%- if pagename != master_doc and theme_show_breadcrumbs|tobool %}
       {%- include "breadcrumbs.html" %}
     {%- endif %}
 
-    <article role="main" class="flex-1">
+    <article role="main" class="flex-1 prose">
       {% block body %}{% endblock %}
     </article>
 
     {%- if theme_show_prev_next|tobool %}
       {%- include "prev_next.html" %}
     {%- endif %}
 
+    {%- block extrabody %}{%- endblock %}
+
     <footer>
       {%- block footer %}
         {%- include "footer.html" %}
       {%- endblock %}
     </footer>
 
     {#- scroll to top button -#}
```

### Comparing `sphinxawesome_theme-4.0.3/PKG-INFO` & `sphinxawesome_theme-4.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxawesome-theme
-Version: 4.0.3
+Version: 4.1.0
 Summary: An awesome theme for the Sphinx documentation generator
 Home-page: https://sphinxawesome.xyz
 License: MIT
 Author: Kai Welke
 Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
@@ -15,21 +15,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
-Provides-Extra: docs
 Requires-Dist: beautifulsoup4 (>=4.9.1,<5.0.0)
-Requires-Dist: myst-parser (>=0.19,<1.1) ; extra == "docs"
 Requires-Dist: python-dotenv (>=0.19,<1.1)
 Requires-Dist: sphinx (>4)
-Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; extra == "docs"
-Requires-Dist: sphinx-sitemap (>=2.2.0,<3.0.0) ; extra == "docs"
 Project-URL: Documentation, https://sphinxawesome.xyz
 Project-URL: Repository, https://github.com/kai687/sphinxawesome-theme
 Description-Content-Type: text/markdown
 
 <h1 align="center">Sphinx awesome theme</h1>
 
 <p align="center">
@@ -77,19 +73,14 @@
 Each code block has a **Copy** button for easy copying.
 This theme enhances Sphinx's `code-block` directive with these options:
 
 - `emphasize-added`. Highlight lines that should be added to code
 - `emphasize-removed`. Highlight lines that should be removed from the code
 - `emphasize-text: TEXT`. Highlight `TEXT` in the code block to emphasize placeholder text the user should replace.
 
-### Collapsible elements
-
-Nested navigation links allow you to reach all pages from all other pages.
-You can make code object definitions like methods, classes, or modules collapsible as well.
-
 ### Better headerlinks
 
 Clicking the link icon after headers or captions automatically copies the URL to the clipboard.
 
 ### DocSearch
 
 If you have an Algolia DocSearch account for your documentation,
```

#### html2text {}

```diff
@@ -1,25 +1,22 @@
-Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 4.0.3 Summary: An
+Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 4.1.0 Summary: An
 awesome theme for the Sphinx documentation generator Home-page: https://
 sphinxawesome.xyz License: MIT Author: Kai Welke Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0 Classifier: Framework :: Sphinx Classifier:
 Framework :: Sphinx :: Theme Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Documentation Classifier: Topic :: Documentation :: Sphinx Classifier:
-Topic :: Software Development :: Documentation Provides-Extra: docs Requires-
-Dist: beautifulsoup4 (>=4.9.1,<5.0.0) Requires-Dist: myst-parser (>=0.19,<1.1)
-; extra == "docs" Requires-Dist: python-dotenv (>=0.19,<1.1) Requires-Dist:
-sphinx (>4) Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; extra ==
-"docs" Requires-Dist: sphinx-sitemap (>=2.2.0,<3.0.0) ; extra == "docs"
-Project-URL: Documentation, https://sphinxawesome.xyz Project-URL: Repository,
-https://github.com/kai687/sphinxawesome-theme Description-Content-Type: text/
-markdown
+Topic :: Software Development :: Documentation Requires-Dist: beautifulsoup4
+(>=4.9.1,<5.0.0) Requires-Dist: python-dotenv (>=0.19,<1.1) Requires-Dist:
+sphinx (>4) Project-URL: Documentation, https://sphinxawesome.xyz Project-URL:
+Repository, https://github.com/kai687/sphinxawesome-theme Description-Content-
+Type: text/markdown
                       ****** Sphinx awesome theme ******
     [MIT license] [PyPI version] [Netlify Deploy] [GitHub Workflow Status]
  Create beautiful and awesome documentation websites with Sphinx. See how the
                     theme looks like on sphinxawesome.xyz.
 ## Get started To use this theme in your project, install it via `pip` and add
 it to your Sphinx configuration. 1. Install the theme as a Python package:
 ```console pip install sphinxawesome-theme ``` For more information, see [How
@@ -32,17 +29,14 @@
 beautiful documentation websites. These features make your documentation
 awesome: ### Awesome code blocks Code blocks show the language of the code in a
 header. Each code block has a **Copy** button for easy copying. This theme
 enhances Sphinx's `code-block` directive with these options: - `emphasize-
 added`. Highlight lines that should be added to code - `emphasize-removed`.
 Highlight lines that should be removed from the code - `emphasize-text: TEXT`.
 Highlight `TEXT` in the code block to emphasize placeholder text the user
-should replace. ### Collapsible elements Nested navigation links allow you to
-reach all pages from all other pages. You can make code object definitions like
-methods, classes, or modules collapsible as well. ### Better headerlinks
-Clicking the link icon after headers or captions automatically copies the URL
-to the clipboard. ### DocSearch If you have an Algolia DocSearch account for
-your documentation, you can use DocSearch for a search-as-you-type experience
-with autocomplete. Algolia DocSearch is free for open source documentation
-projects. ### Better keyboard navigation Use the `Tab` key to skip through all
-sections on the page. Use the `Space` key to expand or collapse items in the
-navigation menu or in code definitions.
+should replace. ### Better headerlinks Clicking the link icon after headers or
+captions automatically copies the URL to the clipboard. ### DocSearch If you
+have an Algolia DocSearch account for your documentation, you can use DocSearch
+for a search-as-you-type experience with autocomplete. Algolia DocSearch is
+free for open source documentation projects. ### Better keyboard navigation Use
+the `Tab` key to skip through all sections on the page. Use the `Space` key to
+expand or collapse items in the navigation menu or in code definitions.
```

