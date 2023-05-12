# Comparing `tmp/sphinxawesome_theme-4.1.0.tar.gz` & `tmp/sphinxawesome_theme-5.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxawesome_theme-4.1.0.tar", max compression
+gzip compressed data, was "sphinxawesome_theme-5.0.0b1.tar", max compression
```

## Comparing `sphinxawesome_theme-4.1.0.tar` & `sphinxawesome_theme-5.0.0b1.tar`

### file list

```diff
@@ -1,59 +1,51 @@
--rw-r--r--   0        0        0     1066 2023-05-12 07:27:52.906417 sphinxawesome_theme-4.1.0/LICENSE
--rw-r--r--   0        0        0     2663 2023-05-12 07:27:52.906417 sphinxawesome_theme-4.1.0/README.md
--rw-r--r--   0        0        0     2368 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/pyproject.toml
--rw-r--r--   0        0        0      172 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/README.rst
--rw-r--r--   0        0        0     2814 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/__init__.py
--rw-r--r--   0        0        0      671 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/breadcrumbs.html
--rw-r--r--   0        0        0     3129 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/docsearch.py
--rw-r--r--   0        0        0      959 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/footer.html
--rw-r--r--   0        0        0     2658 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/header.html
--rw-r--r--   0        0        0    12304 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/highlighting.py
--rw-r--r--   0        0        0     1191 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/html_translator.py
--rw-r--r--   0        0        0      825 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/icons.py
--rw-r--r--   0        0        0     3085 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/jinja_functions.py
--rw-r--r--   0        0        0     1158 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/jsonimpl.py
--rw-r--r--   0        0        0     2852 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/layout.html
--rw-r--r--   0        0        0     1396 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/menu.html
--rw-r--r--   0        0        0      622 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/modals.html
--rw-r--r--   0        0        0      311 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/page.html
--rw-r--r--   0        0        0     7438 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/postprocess.py
--rw-r--r--   0        0        0      836 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/prev_next.html
--rw-r--r--   0        0        0      613 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/scrolltop.html
--rw-r--r--   0        0        0      808 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/search.html
--rw-r--r--   0        0        0     1344 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/searchbox.html
--rw-r--r--   0        0        0     1055 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/sidebar.html
--rw-r--r--   0        0        0      432 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/skip.html
--rw-r--r--   0        0        0    28348 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff
--rw-r--r--   0        0        0    28288 2023-05-12 07:27:52.910417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/0ffeb7a552b36437b54c.woff
--rw-r--r--   0        0        0    22192 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2
--rw-r--r--   0        0        0    17336 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/3a43b67e5bbdfb3ab0a6.woff2
--rw-r--r--   0        0        0    26760 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/44fd0da18fe361a5cc7f.woff
--rw-r--r--   0        0        0    26680 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff
--rw-r--r--   0        0        0    20544 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/48af7707fe9e6494d6a5.woff
--rw-r--r--   0        0        0    25940 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff
--rw-r--r--   0        0        0    22092 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/9ac5da2442b734abc516.woff
--rw-r--r--   0        0        0    27532 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff
--rw-r--r--   0        0        0        0 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/awesome-sphinx-design.31d6cfe0d16ae931b73c.js
--rw-r--r--   0        0        0      798 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/awesome-sphinx-design.4ff695238f641b0a2852.css
--rw-r--r--   0        0        0    15744 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/b009a76ad6afe4ebd301.woff2
--rw-r--r--   0        0        0    22228 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/c3b5f43fe4c8f3f1fa21.woff2
--rw-r--r--   0        0        0    21080 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/cfdd43ce3499ca7f900a.woff2
--rw-r--r--   0        0        0    22048 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/d037cb4792991826de7d.woff
--rw-r--r--   0        0        0    20388 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2
--rw-r--r--   0        0        0   108012 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch.f1a1a5835ed7a6ab0c85.js
--rw-r--r--   0        0        0      109 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch.f1a1a5835ed7a6ab0c85.js.LICENSE.txt
--rw-r--r--   0        0        0    16727 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch.f30f8b0589fd2b6fd39c.css
--rw-r--r--   0        0        0      795 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch_config.js_t
--rw-r--r--   0        0        0    17368 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/e10742dbb1d4a0864ba8.woff2
--rw-r--r--   0        0        0    20932 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2
--rw-r--r--   0        0        0    20344 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/f1e2a76794cb86b2aa8e.woff
--rw-r--r--   0        0        0    15920 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/f25d774ecfe0996f8eb5.woff2
--rw-r--r--   0        0        0    21412 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2
--rw-r--r--   0        0        0     2230 2023-05-12 07:27:52.914417 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/manifest.json
--rw-r--r--   0        0        0    57949 2023-05-12 07:27:52.918418 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/theme.c8991bd7bb6e57cbeea8.js
--rw-r--r--   0        0        0       93 2023-05-12 07:27:52.918418 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/theme.c8991bd7bb6e57cbeea8.js.LICENSE.txt
--rw-r--r--   0        0        0    42667 2023-05-12 07:27:52.918418 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/theme.c973b470ab69573097f3.css
--rw-r--r--   0        0        0      275 2023-05-12 07:27:52.918418 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/theme.conf
--rw-r--r--   0        0        0     1333 2023-05-12 07:27:52.918418 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/with-sidebar.html
--rw-r--r--   0        0        0     1157 2023-05-12 07:27:52.918418 sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/without-sidebar.html
--rw-r--r--   0        0        0     3754 1970-01-01 00:00:00.000000 sphinxawesome_theme-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-12 16:19:07.291156 sphinxawesome_theme-5.0.0b1/LICENSE
+-rw-r--r--   0        0        0     2628 2023-05-12 16:19:07.291156 sphinxawesome_theme-5.0.0b1/README.md
+-rw-r--r--   0        0        0     2375 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/README.rst
+-rw-r--r--   0        0        0     7050 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/__init__.py
+-rw-r--r--   0        0        0     1194 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/breadcrumbs.html
+-rw-r--r--   0        0        0     5522 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/deprecated.py
+-rw-r--r--   0        0        0     6185 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/docsearch.py
+-rw-r--r--   0        0        0     1394 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/footer.html
+-rw-r--r--   0        0        0     7631 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/header.html
+-rw-r--r--   0        0        0    12730 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/highlighting.py
+-rw-r--r--   0        0        0      820 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/icons.py
+-rw-r--r--   0        0        0     2133 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/jinja_functions.py
+-rw-r--r--   0        0        0     1191 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/jsonimpl.py
+-rw-r--r--   0        0        0     5307 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/layout.html
+-rw-r--r--   0        0        0     3241 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/logos.py
+-rw-r--r--   0        0        0      895 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/page.html
+-rw-r--r--   0        0        0     7375 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/postprocess.py
+-rw-r--r--   0        0        0     1603 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/prev_next.html
+-rw-r--r--   0        0        0      656 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/scrolltop.html
+-rw-r--r--   0        0        0      920 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/search.html
+-rw-r--r--   0        0        0     1370 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/searchbox.html
+-rw-r--r--   0        0        0     2462 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/sidebar.html
+-rw-r--r--   0        0        0      416 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/sidebar_main_nav_links.html
+-rw-r--r--   0        0        0      256 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/sidebar_toc.html
+-rw-r--r--   0        0        0    28348 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff
+-rw-r--r--   0        0        0    28288 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/0ffeb7a552b36437b54c.woff
+-rw-r--r--   0        0        0    22192 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2
+-rw-r--r--   0        0        0    26760 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/44fd0da18fe361a5cc7f.woff
+-rw-r--r--   0        0        0    26680 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff
+-rw-r--r--   0        0        0    25940 2023-05-12 16:19:07.295156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff
+-rw-r--r--   0        0        0    27532 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff
+-rw-r--r--   0        0        0        0 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/awesome-sphinx-design.31d6cfe0d16ae931b73c.js
+-rw-r--r--   0        0        0     1278 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/awesome-sphinx-design.f3507627e0af8330cfa7.css
+-rw-r--r--   0        0        0    22228 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/c3b5f43fe4c8f3f1fa21.woff2
+-rw-r--r--   0        0        0    21080 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/cfdd43ce3499ca7f900a.woff2
+-rw-r--r--   0        0        0    20388 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2
+-rw-r--r--   0        0        0    19886 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch.445222223e83896718c6.css
+-rw-r--r--   0        0        0   108012 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch.f1a1a5835ed7a6ab0c85.js
+-rw-r--r--   0        0        0      109 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch.f1a1a5835ed7a6ab0c85.js.LICENSE.txt
+-rw-r--r--   0        0        0      704 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch_config.js_t
+-rw-r--r--   0        0        0    20932 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2
+-rw-r--r--   0        0        0    21412 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2
+-rw-r--r--   0        0        0     1590 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/manifest.json
+-rw-r--r--   0        0        0    48804 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/theme.a16405b310edf0713aee.css
+-rw-r--r--   0        0        0    52713 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/theme.ad172c0f1249198ea036.js
+-rw-r--r--   0        0        0       93 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/theme.ad172c0f1249198ea036.js.LICENSE.txt
+-rw-r--r--   0        0        0      470 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/theme.conf
+-rw-r--r--   0        0        0      357 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/toc.html
+-rw-r--r--   0        0        0     2086 2023-05-12 16:19:07.299156 sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/toc.py
+-rw-r--r--   0        0        0     3678 1970-01-01 00:00:00.000000 sphinxawesome_theme-5.0.0b1/PKG-INFO
```

### Comparing `sphinxawesome_theme-4.1.0/LICENSE` & `sphinxawesome_theme-5.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/README.md` & `sphinxawesome_theme-5.0.0b1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -10,56 +10,64 @@
 <p align="center">
    Create beautiful and awesome documentation websites with <a href="https://www.sphinx-doc.org/en/master/">Sphinx</a>.
    See how the theme looks like on <a href="https://sphinxawesome.xyz">sphinxawesome.xyz</a>.
 </p>
 
 ## Get started
 
-To use this theme in your project,
-install it via `pip` and add it to your Sphinx configuration.
-
 1. Install the theme as a Python package:
 
    ```console
    pip install sphinxawesome-theme
    ```
 
-   For more information, see [How to install the theme](https://sphinxawesome.xyz/how-to/install/).
+   For more information, see [Install the theme](https://sphinxawesome.xyz/how-to/install/).
 
-1. Add `sphinxawesome_theme` as an extension and HTML theme in your Sphinx configuration file `conf.py`:
+1. Add `sphinxawesome_theme` as an HTML theme in your Sphinx configuration file `conf.py`:
 
    ```python
    html_theme = "sphinxawesome_theme"
-   extensions = ["sphinxawesome_theme"]
    ```
 
-   For more information, see [How to load the theme](https://sphinxawesome.xyz/how-to/load/) for more information.
+   For more information, see [Add your theme](https://sphinxawesome.xyz/how-to/add/).
+
+1. Optional:
+
+   - If you want to use Algolia DocSearch with this theme,
+     load the bundled extension:
+
+     ```python
+     # conf.py
+     extensions += ["sphinxawesome_theme.docsearch"]
+     ```
+
+   - If you want to use awesome features for highlighting code,
+     load the bundled extension:
+
+     ```python
+     # conf.py
+     extensions += ["sphinxawesome_theme.highlighting"]
+     ```
 
 ## Features
 
 With the Awesome Theme, you can build readable, functional, and beautiful documentation websites.
-These features make your documentation awesome:
 
 ### Awesome code blocks
 
-Code blocks show the language of the code in a header.
-Each code block has a **Copy** button for easy copying.
-This theme enhances Sphinx's `code-block` directive with these options:
-
-- `emphasize-added`. Highlight lines that should be added to code
-- `emphasize-removed`. Highlight lines that should be removed from the code
-- `emphasize-text: TEXT`. Highlight `TEXT` in the code block to emphasize placeholder text the user should replace.
+- Code block have a **Copy** button for copying the code.
+- If you load the bundled `sphinxawesome_theme.highlighting`,
+  you can use these additional options in your ``code-block`` directives:
+
+  - `emphasize-added`. Highlight lines that should be added to code
+  - `emphasize-removed`. Highlight lines that should be removed from the code
+  - `emphasize-text: TEXT`. Highlight _`TEXT`_ in the code block to emphasize placeholder text.
 
 ### Better headerlinks
 
 Clicking the link icon after headers or captions automatically copies the URL to the clipboard.
 
 ### DocSearch
 
 If you have an Algolia DocSearch account for your documentation,
 you can use DocSearch for a search-as-you-type experience with autocomplete.
 Algolia DocSearch is free for open source documentation projects.
-
-### Better keyboard navigation
-
-Use the `Tab` key to skip through all sections on the page.
-Use the `Space` key to expand or collapse items in the navigation menu or in code definitions.
```

#### html2text {}

```diff
@@ -1,27 +1,26 @@
                       ****** Sphinx awesome theme ******
     [MIT license] [PyPI version] [Netlify Deploy] [GitHub Workflow Status]
  Create beautiful and awesome documentation websites with Sphinx. See how the
                     theme looks like on sphinxawesome.xyz.
-## Get started To use this theme in your project, install it via `pip` and add
-it to your Sphinx configuration. 1. Install the theme as a Python package:
-```console pip install sphinxawesome-theme ``` For more information, see [How
-to install the theme](https://sphinxawesome.xyz/how-to/install/). 1. Add
-`sphinxawesome_theme` as an extension and HTML theme in your Sphinx
-configuration file `conf.py`: ```python html_theme = "sphinxawesome_theme"
-extensions = ["sphinxawesome_theme"] ``` For more information, see [How to load
-the theme](https://sphinxawesome.xyz/how-to/load/) for more information. ##
-Features With the Awesome Theme, you can build readable, functional, and
-beautiful documentation websites. These features make your documentation
-awesome: ### Awesome code blocks Code blocks show the language of the code in a
-header. Each code block has a **Copy** button for easy copying. This theme
-enhances Sphinx's `code-block` directive with these options: - `emphasize-
-added`. Highlight lines that should be added to code - `emphasize-removed`.
-Highlight lines that should be removed from the code - `emphasize-text: TEXT`.
-Highlight `TEXT` in the code block to emphasize placeholder text the user
-should replace. ### Better headerlinks Clicking the link icon after headers or
-captions automatically copies the URL to the clipboard. ### DocSearch If you
-have an Algolia DocSearch account for your documentation, you can use DocSearch
-for a search-as-you-type experience with autocomplete. Algolia DocSearch is
-free for open source documentation projects. ### Better keyboard navigation Use
-the `Tab` key to skip through all sections on the page. Use the `Space` key to
-expand or collapse items in the navigation menu or in code definitions.
+## Get started 1. Install the theme as a Python package: ```console pip install
+sphinxawesome-theme ``` For more information, see [Install the theme](https://
+sphinxawesome.xyz/how-to/install/). 1. Add `sphinxawesome_theme` as an HTML
+theme in your Sphinx configuration file `conf.py`: ```python html_theme =
+"sphinxawesome_theme" ``` For more information, see [Add your theme](https://
+sphinxawesome.xyz/how-to/add/). 1. Optional: - If you want to use Algolia
+DocSearch with this theme, load the bundled extension: ```python # conf.py
+extensions += ["sphinxawesome_theme.docsearch"] ``` - If you want to use
+awesome features for highlighting code, load the bundled extension: ```python #
+conf.py extensions += ["sphinxawesome_theme.highlighting"] ``` ## Features With
+the Awesome Theme, you can build readable, functional, and beautiful
+documentation websites. ### Awesome code blocks - Code block have a **Copy**
+button for copying the code. - If you load the bundled
+`sphinxawesome_theme.highlighting`, you can use these additional options in
+your ``code-block`` directives: - `emphasize-added`. Highlight lines that
+should be added to code - `emphasize-removed`. Highlight lines that should be
+removed from the code - `emphasize-text: TEXT`. Highlight _`TEXT`_ in the code
+block to emphasize placeholder text. ### Better headerlinks Clicking the link
+icon after headers or captions automatically copies the URL to the clipboard.
+### DocSearch If you have an Algolia DocSearch account for your documentation,
+you can use DocSearch for a search-as-you-type experience with autocomplete.
+Algolia DocSearch is free for open source documentation projects.
```

### Comparing `sphinxawesome_theme-4.1.0/pyproject.toml` & `sphinxawesome_theme-5.0.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sphinxawesome-theme"
-version = "4.1.0"
+version = "5.0.0-beta.1"
 description = "An awesome theme for the Sphinx documentation generator"
 readme = "README.md"
 authors = ["Kai Welke <kai687@pm.me>"]
 homepage = "https://sphinxawesome.xyz"
 documentation = "https://sphinxawesome.xyz"
 repository = "https://github.com/kai687/sphinxawesome-theme"
 license = "MIT"
@@ -20,20 +20,20 @@
   { include = "sphinxawesome_theme", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 sphinx = ">4"
 beautifulsoup4 = "^4.9.1"
-python-dotenv = ">=0.19,<1.1"
 
 [tool.poetry.group.docs.dependencies]
 sphinx-autobuild = "^2021.3.14"
 sphinx-sitemap = "^2.2.0"
 sphinx-design = "^0.4.1"
+python-dotenv = ">=0.19,<1.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2"
 pytest-cov = "^4.0"
 coverage = { extras = ["toml"], version = "^7.2" }
 types-docutils = "^0.19.1.6"
 mypy = "^1.0"
```

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/highlighting.py` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/highlighting.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,61 @@
-"""Add more line highlighting options to Pygments.
+"""Add more highlighting options to Pygments.
 
-The theme uses a custom pygments HTML formatter,
-that adds the ability to highlight added/removed
-lines in code.
+This extension extends the Sphinx ``code-block``
+directive with new options:
 
-To make use of this new function, this theme also
-extends the default Sphinx ``code-block`` directive.
+- ``:emphasize-added:``: highlight added lines
+- ``:emphasize-removed:``: highlight removed lines
+- ``:emphasize-text:``: highlight a single word, such as, a placeholder
+
+To achieve this, this extension must make a few larger changes:
+
+1. Provide a custom Sphinx translator to parse the new code block options.
+2. Provide a new Sphinx directive to pass along these new options to Pygments.
+3. Write a new Pygments HTML formatter and a custom filter to handle these options.
+
+It's entirely possible that there's a simpler way of doing this,
+but I haven't found it.
+
+To load this extension, add:
+
+.. code-block:: python
+   :caption: |conf|
+
+   extensions += ["sphinxawesome_theme.highlighting"]
 
 :copyright: Copyright Kai Welke.
 :license: MIT, see LICENSE for details.
 """
+from __future__ import annotations
+
 import re
-from typing import Any, Dict, Generator, List, Optional, Pattern, Tuple, Union
+from typing import Any, Generator, Pattern, Tuple, Union
 
 from docutils import nodes
 from docutils.nodes import Element, Node
 from docutils.parsers.rst import directives
 from pygments import highlight
 from pygments.filter import Filter
 from pygments.filters import ErrorToken
 from pygments.formatters import HtmlFormatter
-from pygments.lexers.shell import BashSessionLexer
 from pygments.token import Generic, _TokenType
 from pygments.util import get_list_opt
 from sphinx.application import Sphinx
 from sphinx.directives.code import CodeBlock, container_wrapper, dedent_lines
 from sphinx.highlighting import PygmentsBridge
 from sphinx.locale import __
 from sphinx.util import logging, parselinenos, texescape
 
 from . import __version__
 
 logger = logging.getLogger(__name__)
 
 # type alias
-TokenType = Union[_TokenType, int]
+TokenType = Union[_TokenType, int]  # For Python 3.8
 TokenStream = Generator[Tuple[TokenType, str], None, None]
 
 
 def _replace_placeholders(
     ttype: _TokenType, value: str, regex: Pattern[str]
 ) -> TokenStream:
     """Replace every occurence of `regex` with `Generic.Emph` token."""
@@ -49,27 +66,31 @@
             yield ttype, value[last:start]
         yield Generic.Emph, value[start:end]
         last = end
     if last != len(value):
         yield ttype, value[last:]
 
 
+# Without the comment, `mypy` throws a fit:
+# Cannot subclass Filter, is type `Any`
+
+
 class AwesomePlaceholders(Filter):  # type: ignore[misc]
     """A Pygments filter for marking up placeholder text."""
 
-    def __init__(self: "AwesomePlaceholders", **options: Any) -> None:
+    def __init__(self: AwesomePlaceholders, **options: str) -> None:
         """Create an instance of the `AwesomePlaceholders` filter."""
         Filter.__init__(self, **options)
         placeholders = get_list_opt(options, "hl_text", [])
         self.placeholders_re = re.compile(
             r"|".join([re.escape(x) for x in placeholders if x])
         )
 
     def filter(
-        self: "AwesomePlaceholders", _lexer: Any, stream: TokenStream
+        self: AwesomePlaceholders, _lexer: Any, stream: TokenStream
     ) -> TokenStream:
         """Filter on all tokens.
 
         The `lexer` is required by the parent class.
         """
         regex = self.placeholders_re
         for ttype, value in stream:
@@ -81,15 +102,15 @@
 
     Allow highlighting added or removed lines.
     Similar to emphasizing lines.
 
     In contrast to Pygments, this formatter returns `<mark>` for higlighted lines.
     """
 
-    def __init__(self: "AwesomeHtmlFormatter", **options: Any) -> None:
+    def __init__(self: AwesomeHtmlFormatter, **options: Any) -> None:
         """Implement `hl_added` and `hl_removed` options."""
         self.added_lines = set()
         self.removed_lines = set()
 
         for lineno in get_list_opt(options, "hl_added", []):
             try:
                 self.added_lines.add(int(lineno))
@@ -100,21 +121,21 @@
             try:
                 self.removed_lines.add(int(lineno))
             except ValueError:
                 pass
 
         # These options aren't compatible with `sphinx.ext.autodoc`
         # options["lineanchors"] = "code"
-        # options["linespans"] = "code-line"
+        options["linespans"] = "line"
         options["wrapcode"] = True
 
         super().__init__(**options)
 
     def _highlight_lines(
-        self: "AwesomeHtmlFormatter", tokensource: TokenStream
+        self: AwesomeHtmlFormatter, tokensource: TokenStream
     ) -> TokenStream:
         """Highlight added, removed, and emphasized lines.
 
         In contrast to Pygments, use `<mark>`, `<ins>`, and `<del>` elements.
         """
         for i, (t, value) in enumerate(tokensource):
             if t != 1:
@@ -125,15 +146,15 @@
                 yield 1, "<ins>%s</ins>" % value
             elif i + 1 in self.removed_lines:
                 yield 1, "<del>%s</del>" % value
             else:
                 yield 1, value
 
     def format_unencoded(
-        self: "AwesomeHtmlFormatter",
+        self: AwesomeHtmlFormatter,
         tokensource: TokenStream,
         outfile: Any,
     ) -> None:
         """Overwrite method to handle emphasized, added, and removed lines.
 
         Unfortunately, the method doesn't extend easily, so I copy it from Pygments.
         """
@@ -160,15 +181,15 @@
             if self.full:
                 source = self._wrap_full(source, outfile)
 
         for _, piece in source:
             outfile.write(piece)
 
 
-def _get_parsed_line_numbers(linespec: str, nlines: int, location: str) -> List[int]:
+def _get_parsed_line_numbers(linespec: str, nlines: int, location: str) -> list[int]:
     """Get the parsed line numbers for the `emphasize-*` options."""
     line_numbers = parselinenos(linespec, nlines)
     if any(i >= nlines for i in line_numbers):
         logger.warning(
             __("line number spec is out of range(1-%d): %r") % (nlines, linespec),
             location=location,
         )
@@ -183,15 +204,15 @@
         "emphasize-removed": directives.unchanged_required,
         "emphasize-text": directives.unchanged_required,
     }
 
     option_spec = CodeBlock.option_spec
     option_spec.update(new_options)
 
-    def run(self: "AwesomeCodeBlock") -> List[Node]:  # noqa
+    def run(self: AwesomeCodeBlock) -> list[Node]:  # noqa
         """Overwrite method from Sphinx.
 
         Add ability to highlight added and removed lines.
         This passes the options to the highlighter.
         You need a custom pygments formatter.
 
         Unfortunately, the original method doesn't lend itself to being extended,
@@ -275,18 +296,18 @@
 class AwesomePygmentsBridge(PygmentsBridge):
     """Class for monkeypatching."""
 
     def highlight_block(
         self: PygmentsBridge,
         source: str,
         lang: str,
-        opts: Optional[Dict[str, Any]] = None,
+        opts: dict[str, Any] | None = None,
         force: bool = False,
         location: Any = None,
-        **kwargs: Any
+        **kwargs: Any,
     ) -> str:
         """Repeat this method."""
         if not isinstance(source, str):
             source = source.decode()  # type: ignore[unreachable]
 
         lexer = self.get_lexer(source, lang, opts, force, location)
         hl_text = get_list_opt(kwargs, "hl_text", [])
@@ -316,22 +337,18 @@
         if self.dest == "html":
             return hlsource
         else:
             # MEMO: this is done to escape Unicode chars with non-Unicode engines
             return texescape.hlescape(hlsource, self.latex_engine)
 
 
-def setup(app: "Sphinx") -> Dict[str, Any]:
+def setup(app: Sphinx) -> dict[str, Any]:
     """Set up this internal extension."""
     PygmentsBridge.html_formatter = AwesomeHtmlFormatter
     PygmentsBridge.highlight_block = AwesomePygmentsBridge.highlight_block  # type: ignore[method-assign]  # noqa
     directives.register_directive("code-block", AwesomeCodeBlock)
 
-    # Allow using `terminal` in addition to `shell-session` and `console`
-    # for interactive command-line sessions
-    app.add_lexer("terminal", BashSessionLexer)
-
     return {
         "version": __version__,
         "parallel_read_safe": True,
         "parallel_write_safe": True,
     }
```

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/jinja_functions.py` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/jinja_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,23 @@
 """Define custom filters for Jinja2 templates.
 
 :copyright: Copyright, Kai Welke.
 :license: MIT, see LICENSE for details.
 """
+from __future__ import annotations
 
 import json
 import posixpath
 from functools import partial
 from os import path
-from typing import Any, Dict
+from typing import Any
 
-from docutils.nodes import Node, make_id
+from docutils.nodes import Node
 from sphinx.application import Sphinx
 
-from . import __version__
-
-
-def _make_id_from_title(title: str) -> Any:
-    """Use the ``docutils.nodes.make_id`` function to create an ID from a title.
-
-    This can be used for creating link targets from headlines.
-    E.g. transform "Code, Figures, and Tables" into "code-figures-and-tables",
-    which can then be used like this:
-    ``<a href=#{{ title|sanitize }}>{{ title }}</a>``
-
-    Note: `docutils.nodes.make_id` returns Any. Setting the return type to `str`
-    here results in a mypy error in strict mode because of that.
-    """
-    return make_id(title)
-
 
 def _get_manifest_json(app: Sphinx) -> Any:
     """Read the ``manifest.json`` file.
 
     Webpack writes a file ``manifest.json`` in the theme's static directory.
     This file has the mapping between hashed and unhashed filenames.
     Returns a dictionary with this mapping.
@@ -67,28 +52,15 @@
     return canonical
 
 
 def setup_jinja(
     app: Sphinx,
     pagename: str,
     templatename: str,
-    context: Dict[str, Any],
+    context: dict[str, Any],
     doctree: Node,
 ) -> None:
     """Register a function as a Jinja2 filter."""
-    if app.builder is not None:
-        app.builder.templates.environment.filters["sanitize"] = _make_id_from_title
-        context["asset"] = partial(_make_asset_url, app)
-        # must override `pageurl` for directory builder
-        if app.builder.name == "dirhtml" and app.config.html_baseurl:
-            context["pageurl"] = _make_canonical(app, pagename)
-
-
-def setup(app: Sphinx) -> Dict[str, Any]:
-    """Register this jinja filter as extension."""
-    app.connect("html-page-context", setup_jinja)
-
-    return {
-        "version": __version__,
-        "parallel_read_safe": True,
-        "parallel_write_safe": True,
-    }
+    context["asset"] = partial(_make_asset_url, app)
+    # must override `pageurl` for directory builder
+    if app.builder.name == "dirhtml" and app.config.html_baseurl:
+        context["pageurl"] = _make_canonical(app, pagename)
```

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/jsonimpl.py` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/jsonimpl.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 The awesome theme uses custom jinja2 helper functions which are
 non-serializable by default. Hence, I need to use a custom JSON
 serializer.
 
 :copyright: Copyright Kai Welke.
 :license: MIT, see LICENSE for details.
 """
+from __future__ import annotations
 
 import json
 from typing import IO, Any
 
 
 class AwesomeJSONEncoder(json.JSONEncoder):
     """Custom JSON encoder for everything in the `context`."""
 
-    def default(self: "AwesomeJSONEncoder", obj: Any) -> str:
+    def default(self: AwesomeJSONEncoder, obj: Any) -> str:
         """Return an empty string for anything that's not serializable by default."""
         return ""
 
 
 def dump(obj: Any, fp: IO[str], *args: Any, **kwargs: Any) -> None:
     """Dump JSON into file."""
     kwargs["cls"] = AwesomeJSONEncoder
```

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/postprocess.py` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/postprocess.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,76 +13,65 @@
 
 Note: This file is not processed by Webpack; don't use Tailwind utility classes.
 They might not show up in the final CSS.
 
 :copyright: Copyright Kai Welke.
 :license: MIT, see LICENSE.
 """
+from __future__ import annotations
 
 import os
 import re
-from typing import Any, Dict, List, Optional
 
 from bs4 import BeautifulSoup, Comment
 from sphinx.application import Sphinx
-from sphinx.util import logging
 
-from . import __version__
-from .icons import ICONS
+from . import icons, logos
 
-logger = logging.getLogger(__name__)
 
-
-def _get_html_files(outdir: str) -> List[str]:
+def _get_html_files(outdir: str) -> list[str]:
     """Get a list of HTML files."""
     html_list = []
     for root, _, files in os.walk(outdir):
         html_list.extend(
             [os.path.join(root, file) for file in files if file.endswith(".html")]
         )
     return html_list
 
 
 def _collapsible_nav(tree: BeautifulSoup) -> None:
-    """Restructure the navigation links to make them collapsible.
-
-    First, all links in the navigation sidebar are wrapped in a ``div``.
-    This allows them to be 'block' and 'position relative' for the
-    'expand' icon to be positioned against.
-
-    Second, an icon is inserted right before the link.
-    Adding the icon as separate DOM element allows click events to be
-    captured separately between the icon and the link.
-    """
-    for link in tree.select(".nav-toc a"):
-        link["data-action"] = "click->sidebar#close"
-        # Don't add the nav-link class twice (#166)
-        if "nav-link" not in link.parent.get("class", []):
-            # First, all links should be wrapped in a div.nav-link
-            link.wrap(tree.new_tag("div", attrs={"class": "nav-link"}))
-            # Next, insert a span.expand before the link, if the #nav-link
-            # has any sibling elements (a ``ul`` in the navigation menu)
-            if link.parent.next_sibling:
-                # create the icon
-                svg = BeautifulSoup(ICONS["chevron_right"], "html.parser").svg
-                svg["tabindex"] = "0"
-                svg["height"] = "1.2rem"
-                svg["class"] = ["expand"]
-                svg["style"] = ["display: inline;"]
-                svg[
-                    "data-action"
-                ] = "click->sidebar#expand keydown->sidebar#expandKeyPressed"
-                link.insert_before(svg)
-
-
-def _expand_current(tree: BeautifulSoup) -> None:
-    """Add the ``.expanded`` class to li.current elements."""
-    for li in tree("li", class_="current"):
-        if "expanded" not in li.get("class", []):
-            li["class"] += ["expanded"]
+    """Make navigation links with children collapsible."""
+    for link in tree.select("#left-sidebar a"):
+        # Check if the link has "children"
+        children = link.next_sibling
+        if children and children.name == "ul":
+            # State must be available in the link and the list
+            li = link.parent
+            li[
+                "x-data"
+            ] = "{ expanded: $el.classList.contains('current') ? true : false }"
+            link["@click"] = "expanded = !expanded"
+            # The expandable class is a hack because we can't use Tailwind
+            # I want to have _only_ expandable links with `justify-between`
+            link["class"].append("expandable")
+            link[":class"] = "{ 'expanded' : expanded }"
+            children["x-show"] = "expanded"
+
+            # Create a button with an icon inside to get focus behavior
+            button = tree.new_tag(
+                "button",
+                attrs={"type": "button", "@click.prevent.stop": "expanded = !expanded"},
+            )
+            label = tree.new_tag("span", attrs={"class": "sr-only"})
+            button.append(label)
+
+            # create the icon
+            svg = BeautifulSoup(icons.ICONS["chevron_right"], "html.parser").svg
+            button.append(svg)
+            link.append(button)
 
 
 def _remove_empty_toctree(tree: BeautifulSoup) -> None:
     """Remove empty toctree divs.
 
     If you include a `toctree` with the `hidden` option,
     an empty `div` is inserted. Remove them.
@@ -91,37 +80,50 @@
     for div in tree("div", class_="toctree-wrapper"):
         children = list(div.children)
         if len(children) == 1 and not children[0].strip():
             div.extract()
 
 
 def _headerlinks(tree: BeautifulSoup) -> None:
-    """Enhance the headerlink experience."""
+    """Make headerlinks copy their URL on click."""
     for link in tree("a", class_="headerlink"):
-        link["data-controller"] = "clipboard"
-        link["data-action"] = "click->clipboard#copyHeaderLink"
-        link["aria-label"] = "Click to copy this link"
+        link[
+            "@click.prevent"
+        ] = "window.navigator.clipboard.writeText($el.href); $el.setAttribute('data-tooltip', 'Copied!'); setTimeout(() => $el.setAttribute('data-tooltip', 'Copy link to this element'), 2000)"
         del link["title"]
-        link["class"].extend(["tooltipped", "tooltipped-ne"])
+        link["aria-label"] = "Copy link to this element"
+        link["data-tooltip"] = "Copy link to this element"
 
 
-def _code_controller(tree: BeautifulSoup) -> None:
-    """Add the controller attribute to code blocks."""
-    for block in tree("div", class_="highlight"):
-        block["data-controller"] = "code"
+def _scrollspy(tree: BeautifulSoup) -> None:
+    """Add an active class to current TOC links in the right sidebar."""
+    for link in tree("a", class_="headerlink"):
+        if link.parent.name in ["h2", "h3"] or (
+            link.parent.name == "dt" and "sig" in link.parent["class"]
+        ):
+            active_link = link["href"]
+            link[
+                "x-intersect.margin.0%.0%.-70%.0%"
+            ] = f"activeSection = '{active_link}'"
+
+    for link in tree.select("#right-sidebar a"):
+        active_link = link["href"]
+        link[":data-current"] = f"activeSection === '{active_link}'"
 
 
 def _external_links(tree: BeautifulSoup) -> None:
     """Add `rel="nofollow noopener"` to external links.
 
     The alternative was to copy `visit_reference` in the HTMLTranslator
     and change literally one line.
     """
     for link in tree("a", class_="reference external"):
         link["rel"] = "nofollow noopener"
+        # append icon
+        link.append(BeautifulSoup(icons.ICONS["external_link"], "html.parser").svg)
 
 
 def _strip_comments(tree: BeautifulSoup) -> None:
     """Remove HTML comments from documents."""
     comments = tree.find_all(string=lambda text: isinstance(text, Comment))
     for c in comments:
         c.extract()
@@ -166,48 +168,38 @@
     2. The modifications are performed in order and in place.
     3. After these modifications, the HTML is written into a file,
     overwriting the original file.
     """
     with open(html_filename, encoding="utf-8") as html:
         tree = BeautifulSoup(html, "html.parser")
 
-    _expand_current(tree)
+    theme_options = logos.get_theme_options(app)
+
     _collapsible_nav(tree)
-    _external_links(tree)
+    if theme_options.get("awesome_external_links"):
+        _external_links(tree)
     _remove_empty_toctree(tree)
-    if app.config.html_awesome_headerlinks:
+    _scrollspy(tree)
+    if theme_options.get("awesome_headerlinks"):
         _headerlinks(tree)
-    _code_controller(tree)
-    if app.config.html_awesome_code_headers:
-        _code_headers(tree)
+    # _code_headers(tree)
     _strip_comments(tree)
 
     with open(html_filename, "w", encoding="utf-8") as out_file:
         out_file.write(str(tree))
 
 
-def post_process_html(app: Sphinx, exc: Optional[Exception]) -> None:
+def post_process_html(app: Sphinx, exc: Exception | None) -> None:
     """Perform modifications on the HTML after building.
 
     This is an extra function, that gets a list from all HTML
     files in the output directory, then runs the ``_modify_html``
     function on each of them.
     """
     if app.builder is not None and app.builder.name not in ["html", "dirhtml"]:
         return
 
     if exc is None:
         html_files = _get_html_files(app.outdir)
 
         for doc in html_files:
             _modify_html(doc, app)
-
-
-def setup(app: "Sphinx") -> Dict[str, Any]:
-    """Set this up as internal extension."""
-    app.connect("build-finished", post_process_html)
-
-    return {
-        "version": __version__,
-        "parallel_read_safe": True,
-        "parallel_write_safe": True,
-    }
```

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/scrolltop.html` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/scrolltop.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 {#-
 A `scroll to top` button. Is shown at the bottom right if `show_scrolltop` is true.
 -#}
-
-
-<button data-scroll-to-top-target="scrollToTop" data-action="scroll-to-top#scroll"
-  class="fixed bottom-8 right-8 p-2 z-10 rounded-sm bg-gray-700 text-xs text-white invisible opacity-0 transition-all duration-1000 hover:bg-gray-950 focus:bg-gray-950">
-  <svg xmlns="http://www.w3.org/2000/svg" height="14" viewBox="0 96 960 960" width="14"
-    class="inline fill-current mb-[2px]" aria-hidden="true">
+<button data-scroll-to-top-target="scrollToTop"
+        data-action="scroll-to-top#scroll"
+        class="fixed bottom-8 right-8 p-2 z-10 rounded-sm bg-gray-700 text-xs text-white invisible opacity-0 transition-all duration-1000 hover:bg-gray-950 focus:bg-gray-950">
+  <svg xmlns="http://www.w3.org/2000/svg"
+       height="14"
+       viewBox="0 96 960 960"
+       width="14"
+       class="inline fill-current mb-[2px]"
+       aria-hidden="true">
     <path d="M450 896V370L202 618l-42-42 320-320 320 320-42 42-248-248v526h-60Z" />
   </svg>
   Back to top
 </button>
```

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/09be83022f2ac2ce16b0.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/0ffeb7a552b36437b54c.woff` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/0ffeb7a552b36437b54c.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/31f64b9c465158bd6066.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/44fd0da18fe361a5cc7f.woff` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/44fd0da18fe361a5cc7f.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/46830c334f8112fa510a.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/6f04107ce68d524ebe69.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/ad463ea60cc8b68792f4.woff`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/c3b5f43fe4c8f3f1fa21.woff2` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/c3b5f43fe4c8f3f1fa21.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/cfdd43ce3499ca7f900a.woff2` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/cfdd43ce3499ca7f900a.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/d0b41bd1d599bc0a52b7.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch.f1a1a5835ed7a6ab0c85.js` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch.f1a1a5835ed7a6ab0c85.js`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch.f30f8b0589fd2b6fd39c.css` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch.445222223e83896718c6.css`

 * *Files 12% similar despite different names*

```diff
@@ -1,2 +1,2 @@
 /*! @docsearch/css 3.3.4 | MIT License | © Algolia, Inc. and contributors | https://docsearch.algolia.com */:root{--docsearch-primary-color:#5468ff;--docsearch-text-color:#1c1e21;--docsearch-spacing:12px;--docsearch-icon-stroke-width:1.4;--docsearch-highlight-color:var(--docsearch-primary-color);--docsearch-muted-color:#969faf;--docsearch-container-background:rgba(101,108,133,.8);--docsearch-logo-color:#5468ff;--docsearch-modal-width:560px;--docsearch-modal-height:600px;--docsearch-modal-background:#f5f6f7;--docsearch-modal-shadow:inset 1px 1px 0 0 hsla(0,0%,100%,.5),0 3px 8px 0 #555a64;--docsearch-searchbox-height:56px;--docsearch-searchbox-background:#ebedf0;--docsearch-searchbox-focus-background:#fff;--docsearch-searchbox-shadow:inset 0 0 0 2px var(--docsearch-primary-color);--docsearch-hit-height:56px;--docsearch-hit-color:#444950;--docsearch-hit-active-color:#fff;--docsearch-hit-background:#fff;--docsearch-hit-shadow:0 1px 3px 0 #d4d9e1;--docsearch-key-gradient:linear-gradient(-225deg,#d5dbe4,#f8f8f8);--docsearch-key-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);--docsearch-footer-height:44px;--docsearch-footer-background:#fff;--docsearch-footer-shadow:0 -1px 0 0 #e0e3e8,0 -3px 6px 0 rgba(69,98,155,.12)}html[data-theme=dark]{--docsearch-text-color:#f5f6f7;--docsearch-container-background:rgba(9,10,17,.8);--docsearch-modal-background:#15172a;--docsearch-modal-shadow:inset 1px 1px 0 0 #2c2e40,0 3px 8px 0 #000309;--docsearch-searchbox-background:#090a11;--docsearch-searchbox-focus-background:#000;--docsearch-hit-color:#bec3c9;--docsearch-hit-shadow:none;--docsearch-hit-background:#090a11;--docsearch-key-gradient:linear-gradient(-26.5deg,#565872,#31355b);--docsearch-key-shadow:inset 0 -2px 0 0 #282d55,inset 0 0 1px 1px #51577d,0 2px 2px 0 rgba(3,4,9,.3);--docsearch-footer-background:#1e2136;--docsearch-footer-shadow:inset 0 1px 0 0 rgba(73,76,106,.5),0 -4px 8px 0 rgba(0,0,0,.2);--docsearch-logo-color:#fff;--docsearch-muted-color:#7f8497}.DocSearch-Button{align-items:center;background:#ebedf0;background:var(--docsearch-searchbox-background);border:0;border-radius:40px;color:#969faf;color:var(--docsearch-muted-color);cursor:pointer;display:flex;font-weight:500;height:36px;justify-content:space-between;margin:0 0 0 16px;padding:0 8px;-webkit-user-select:none;-moz-user-select:none;user-select:none}.DocSearch-Button:active,.DocSearch-Button:focus,.DocSearch-Button:hover{background:#fff;background:var(--docsearch-searchbox-focus-background);box-shadow:inset 0 0 0 2px #5468ff;box-shadow:var(--docsearch-searchbox-shadow);color:#1c1e21;color:var(--docsearch-text-color);outline:none}.DocSearch-Button-Container{align-items:center;display:flex}.DocSearch-Search-Icon{stroke-width:1.6}.DocSearch-Button .DocSearch-Search-Icon{color:#1c1e21;color:var(--docsearch-text-color)}.DocSearch-Button-Placeholder{font-size:1rem;padding:0 12px 0 6px}.DocSearch-Button-Keys{display:flex;min-width:calc(40px + .8em)}.DocSearch-Button-Key{align-items:center;background:linear-gradient(-225deg,#d5dbe4,#f8f8f8);background:var(--docsearch-key-gradient);border:0;border-radius:3px;box-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);box-shadow:var(--docsearch-key-shadow);color:#969faf;color:var(--docsearch-muted-color);display:flex;height:18px;justify-content:center;margin-right:.4em;padding:0 0 2px;position:relative;top:-1px;width:20px}@media (max-width:768px){.DocSearch-Button-Keys,.DocSearch-Button-Placeholder{display:none}}.DocSearch--active{overflow:hidden!important}.DocSearch-Container,.DocSearch-Container *{box-sizing:border-box}.DocSearch-Container{background-color:rgba(101,108,133,.8);background-color:var(--docsearch-container-background);height:100vh;left:0;position:fixed;top:0;width:100vw;z-index:200}.DocSearch-Container a{-webkit-text-decoration:none;text-decoration:none}.DocSearch-Link{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;font:inherit;margin:0;padding:0}.DocSearch-Modal{background:#f5f6f7;background:var(--docsearch-modal-background);border-radius:6px;box-shadow:inset 1px 1px 0 0 hsla(0,0%,100%,.5),0 3px 8px 0 #555a64;box-shadow:var(--docsearch-modal-shadow);flex-direction:column;margin:60px auto auto;max-width:560px;max-width:var(--docsearch-modal-width);position:relative}.DocSearch-SearchBar{display:flex;padding:12px 12px 0;padding:var(--docsearch-spacing) var(--docsearch-spacing) 0}.DocSearch-Form{align-items:center;background:#fff;background:var(--docsearch-searchbox-focus-background);border-radius:4px;box-shadow:inset 0 0 0 2px #5468ff;box-shadow:var(--docsearch-searchbox-shadow);display:flex;height:56px;height:var(--docsearch-searchbox-height);margin:0;padding:0 12px;padding:0 var(--docsearch-spacing);position:relative;width:100%}.DocSearch-Input{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:transparent;border:0;color:#1c1e21;color:var(--docsearch-text-color);flex:1;font:inherit;font-size:1.2em;height:100%;outline:none;padding:0 0 0 8px;width:80%}.DocSearch-Input::-moz-placeholder{color:#969faf;color:var(--docsearch-muted-color);opacity:1}.DocSearch-Input::placeholder{color:#969faf;color:var(--docsearch-muted-color);opacity:1}.DocSearch-Input::-webkit-search-cancel-button,.DocSearch-Input::-webkit-search-decoration,.DocSearch-Input::-webkit-search-results-button,.DocSearch-Input::-webkit-search-results-decoration{display:none}.DocSearch-LoadingIndicator,.DocSearch-MagnifierLabel,.DocSearch-Reset{margin:0;padding:0}.DocSearch-MagnifierLabel,.DocSearch-Reset{align-items:center;color:#5468ff;color:var(--docsearch-highlight-color);display:flex;justify-content:center}.DocSearch-Container--Stalled .DocSearch-MagnifierLabel,.DocSearch-LoadingIndicator{display:none}.DocSearch-Container--Stalled .DocSearch-LoadingIndicator{align-items:center;color:#5468ff;color:var(--docsearch-highlight-color);display:flex;justify-content:center}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Reset{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);animation:none;-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;right:0}}.DocSearch-Reset{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);animation:fade-in .1s ease-in forwards;-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:var(--docsearch-icon-color);cursor:pointer;padding:2px;right:0}.DocSearch-Reset[hidden]{display:none}.DocSearch-Reset:hover{color:#5468ff;color:var(--docsearch-highlight-color)}.DocSearch-LoadingIndicator svg,.DocSearch-MagnifierLabel svg{height:24px;width:24px}.DocSearch-Cancel{display:none}.DocSearch-Dropdown{max-height:488px;max-height:calc(var(--docsearch-modal-height) - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height));min-height:12px;min-height:var(--docsearch-spacing);overflow-y:auto;overflow-y:overlay;padding:0 12px;padding:0 var(--docsearch-spacing);scrollbar-color:#969faf #f5f6f7;scrollbar-color:var(--docsearch-muted-color) var(--docsearch-modal-background);scrollbar-width:thin}.DocSearch-Dropdown::-webkit-scrollbar{width:12px}.DocSearch-Dropdown::-webkit-scrollbar-track{background:transparent}.DocSearch-Dropdown::-webkit-scrollbar-thumb{background-color:#969faf;background-color:var(--docsearch-muted-color);border:3px solid #f5f6f7;border:3px solid var(--docsearch-modal-background);border-radius:20px}.DocSearch-Dropdown ul{list-style:none;margin:0;padding:0}.DocSearch-Label{font-size:.75em;line-height:1.6em}.DocSearch-Help,.DocSearch-Label{color:#969faf;color:var(--docsearch-muted-color)}.DocSearch-Help{font-size:.9em;margin:0;-webkit-user-select:none;-moz-user-select:none;user-select:none}.DocSearch-Title{font-size:1.2em}.DocSearch-Logo a{display:flex}.DocSearch-Logo svg{color:#5468ff;color:var(--docsearch-logo-color);margin-left:8px}.DocSearch-Hits:last-of-type{margin-bottom:24px}.DocSearch-Hits mark{background:none;color:#5468ff;color:var(--docsearch-highlight-color)}.DocSearch-HitsFooter{color:#969faf;color:var(--docsearch-muted-color);display:flex;font-size:.85em;justify-content:center;margin-bottom:12px;margin-bottom:var(--docsearch-spacing);padding:12px;padding:var(--docsearch-spacing)}.DocSearch-HitsFooter a{border-bottom:1px solid;color:inherit}.DocSearch-Hit{border-radius:4px;display:flex;padding-bottom:4px;position:relative}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--deleting{transition:none}}.DocSearch-Hit--deleting{opacity:0;transition:all .25s linear}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit--favoriting{transition:none}}.DocSearch-Hit--favoriting{transform:scale(0);transform-origin:top center;transition:all .25s linear;transition-delay:.25s}.DocSearch-Hit a{background:#fff;background:var(--docsearch-hit-background);border-radius:4px;box-shadow:0 1px 3px 0 #d4d9e1;box-shadow:var(--docsearch-hit-shadow);display:block;padding-left:12px;padding-left:var(--docsearch-spacing);width:100%}.DocSearch-Hit-source{background:#f5f6f7;background:var(--docsearch-modal-background);color:#5468ff;color:var(--docsearch-highlight-color);font-size:.85em;font-weight:600;line-height:32px;margin:0 -4px;padding:8px 4px 0;position:sticky;top:0;z-index:10}.DocSearch-Hit-Tree{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);color:#969faf;color:var(--docsearch-muted-color);height:56px;height:var(--docsearch-hit-height);opacity:.5;width:24px}.DocSearch-Hit[aria-selected=true] a{background-color:#5468ff;background-color:var(--docsearch-highlight-color)}.DocSearch-Hit[aria-selected=true] mark{-webkit-text-decoration:underline;text-decoration:underline}.DocSearch-Hit-Container{align-items:center;color:#444950;color:var(--docsearch-hit-color);display:flex;flex-direction:row;height:56px;height:var(--docsearch-hit-height);padding:0 12px 0 0;padding:0 var(--docsearch-spacing) 0 0}.DocSearch-Hit-icon{height:20px;width:20px}.DocSearch-Hit-action,.DocSearch-Hit-icon{stroke-width:1.4;stroke-width:var(--docsearch-icon-stroke-width);color:#969faf;color:var(--docsearch-muted-color)}.DocSearch-Hit-action{align-items:center;display:flex;height:22px;width:22px}.DocSearch-Hit-action svg{display:block;height:18px;width:18px}.DocSearch-Hit-action+.DocSearch-Hit-action{margin-left:6px}.DocSearch-Hit-action-button{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:50%;color:inherit;cursor:pointer;padding:2px}svg.DocSearch-Hit-Select-Icon{display:none}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Select-Icon{display:block}.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:background-color .1s ease-in}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{transition:none}}.DocSearch-Hit-action-button:focus path,.DocSearch-Hit-action-button:hover path{fill:#fff}.DocSearch-Hit-content-wrapper{display:flex;flex:1 1 auto;flex-direction:column;font-weight:500;justify-content:center;line-height:1.2em;margin:0 8px;overflow-x:hidden;position:relative;text-overflow:ellipsis;white-space:nowrap;width:80%}.DocSearch-Hit-title{font-size:.9em}.DocSearch-Hit-path{color:#969faf;color:var(--docsearch-muted-color);font-size:.75em}.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-Tree,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-action,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-icon,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-path,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-text,.DocSearch-Hit[aria-selected=true] .DocSearch-Hit-title,.DocSearch-Hit[aria-selected=true] mark{color:#fff!important;color:var(--docsearch-hit-active-color)!important}@media screen and (prefers-reduced-motion:reduce){.DocSearch-Hit-action-button:focus,.DocSearch-Hit-action-button:hover{background:rgba(0,0,0,.2);transition:none}}.DocSearch-ErrorScreen,.DocSearch-NoResults,.DocSearch-StartScreen{font-size:.9em;margin:0 auto;padding:36px 0;text-align:center;width:80%}.DocSearch-Screen-Icon{color:#969faf;color:var(--docsearch-muted-color);padding-bottom:12px}.DocSearch-NoResults-Prefill-List{display:inline-block;padding-bottom:24px;text-align:left}.DocSearch-NoResults-Prefill-List ul{display:inline-block;padding:8px 0 0}.DocSearch-NoResults-Prefill-List li{list-style-position:inside;list-style-type:"» "}.DocSearch-Prefill{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;border-radius:1em;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;font-size:1em;font-weight:700;padding:0}.DocSearch-Prefill:focus,.DocSearch-Prefill:hover{outline:none;-webkit-text-decoration:underline;text-decoration:underline}.DocSearch-Footer{align-items:center;background:#fff;background:var(--docsearch-footer-background);border-radius:0 0 8px 8px;box-shadow:0 -1px 0 0 #e0e3e8,0 -3px 6px 0 rgba(69,98,155,.12);box-shadow:var(--docsearch-footer-shadow);display:flex;flex-direction:row-reverse;flex-shrink:0;height:44px;height:var(--docsearch-footer-height);justify-content:space-between;padding:0 12px;padding:0 var(--docsearch-spacing);position:relative;-webkit-user-select:none;-moz-user-select:none;user-select:none;width:100%;z-index:300}.DocSearch-Commands{color:#969faf;color:var(--docsearch-muted-color);display:flex;list-style:none;margin:0;padding:0}.DocSearch-Commands li{align-items:center;display:flex}.DocSearch-Commands li:not(:last-of-type){margin-right:.8em}.DocSearch-Commands-Key{align-items:center;background:linear-gradient(-225deg,#d5dbe4,#f8f8f8);background:var(--docsearch-key-gradient);border:0;border-radius:2px;box-shadow:inset 0 -2px 0 0 #cdcde6,inset 0 0 1px 1px #fff,0 1px 2px 1px rgba(30,35,90,.4);box-shadow:var(--docsearch-key-shadow);color:#969faf;color:var(--docsearch-muted-color);display:flex;height:18px;justify-content:center;margin-right:.4em;padding:0 0 1px;width:20px}@media (max-width:768px){:root{--docsearch-spacing:10px;--docsearch-footer-height:40px}.DocSearch-Dropdown{height:100%}.DocSearch-Container{height:-webkit-fill-available;height:100vh;height:calc(var(--docsearch-vh, 1vh)*100);position:absolute}.DocSearch-Footer{border-radius:0;bottom:0;position:absolute}.DocSearch-Hit-content-wrapper{display:flex;position:relative;width:80%}.DocSearch-Modal{border-radius:0;box-shadow:none;height:-webkit-fill-available;height:100vh;height:calc(var(--docsearch-vh, 1vh)*100);margin:0;max-width:100%;width:100%}.DocSearch-Dropdown{max-height:calc(100vh - 112px);max-height:calc(var(--docsearch-vh, 1vh)*100 - var(--docsearch-searchbox-height) - var(--docsearch-spacing) - var(--docsearch-footer-height))}.DocSearch-Cancel{-webkit-appearance:none;-moz-appearance:none;appearance:none;background:none;border:0;color:#5468ff;color:var(--docsearch-highlight-color);cursor:pointer;display:inline-block;flex:none;font:inherit;font-size:1em;font-weight:500;margin-left:12px;margin-left:var(--docsearch-spacing);outline:none;overflow:hidden;padding:0;-webkit-user-select:none;-moz-user-select:none;user-select:none;white-space:nowrap}.DocSearch-Commands,.DocSearch-Hit-Tree{display:none}}@keyframes fade-in{0%{opacity:0}to{opacity:1}}
-:root{--docsearch-searchbox-background:transparent;--docsearch-searchbox-shadow:inset 0 0 0 2px var(--color-brand);--docsearch-key-gradient:transparent;--docsearch-primary-color:var(--color-brand);--docsearch-modal-width:960px;--docsearch-modal-background:#fff}.DocSearch-Button{border-radius:0;height:3.5rem;line-height:3.5rem;padding-right:1rem}.DocSearch-Button-Key{font-family:Roboto,sans-serif;font-size:.875rem;height:1.25rem;padding:1rem}.DocSearch-Button:hover .DocSearch-Button-Key{border-color:var(--color-gray-dark);color:var(--color-gray-dark)}.DocSearch-Button .DocSearch-Search-Icon{--tw-text-opacity:1;stroke-width:2.5;color:#f3f4f6;color:rgb(243 244 246/var(--tw-text-opacity))}.DocSearch-Button:hover .DocSearch-Search-Icon{color:var(--docsearch-text-color)}.DocSearch-Button-Placeholder{padding-left:.75rem}.DocSearch-Hit-source{color:var(--color-gray-dark)}.DocSearch-Hit a{--tw-border-opacity:1;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;border-color:#f3f4f6;border-color:rgb(243 244 246/var(--tw-border-opacity));border-radius:.125rem;border-width:1px;box-shadow:0 0 transparent,0 0 transparent,0 0 transparent;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.DocSearch-Modal{border-radius:.125rem}
+:root{--docsearch-primary-color:hsl(var(--primary));--docsearch-key-gradient:transparent;--docsearch-key-shadow:transparent;--docsearch-text-color:hsl(var(--popover-foreground));--docsearch-modal-width:760px;--docsearch-modal-background:hsl(var(--popover));--docsearch-footer-background:hsl(var(--popover));--docsearch-searchbox-focus-background:hsl(var(--popover));--docsearch-container-background:hsl(var(--background)/0.8);--docsearch-spacing:0.5rem;--docsearch-hit-active-color:hsl(var(--accent-foreground));--docsearch-hit-background:transparent;--docsearch-searchbox-shadow:none;--docsearch-hit-shadow:none;--docsearch-modal-shadow:none;--docsearch-footer-shadow:none}.DocSearch-Button{--tw-ring-offset-color:hsl(var(--background));border-color:hsl(var(--input));border-radius:.5em;border-style:solid;border-width:1px;display:flex;font-size:.875rem;line-height:1.25rem;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1);width:90%}.DocSearch-Button:hover{--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;box-shadow:0 0 transparent,0 0 transparent,0 0 transparent;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.DocSearch-Button:focus,.DocSearch-Button:hover{background-color:hsl(var(--accent));color:hsl(var(--accent-foreground))}.DocSearch-Button:focus-visible{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);--tw-ring-color:hsl(var(--ring));--tw-ring-offset-width:2px;box-shadow:var(--tw-ring-inset) 0 0 0 2px var(--tw-ring-offset-color),var(--tw-ring-inset) 0 0 0 4px hsl(var(--ring)),0 0 transparent;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 #0000);outline:2px solid transparent;outline-offset:2px}.DocSearch-Button-Placeholder{display:block;font-size:.875rem;font-weight:500;line-height:1.25rem}.DocSearch-Button-Key{background-color:hsl(var(--muted));border-color:hsl(var(--border));border-radius:.25rem;border-style:solid;border-width:1px;color:hsl(var(--muted-foreground));font-size:12px}.DocSearch-Container{--tw-backdrop-blur:blur(4px);-webkit-backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);position:fixed}.DocSearch-Modal{border-color:hsl(var(--border));border-radius:var(--radius);border-width:1px}.DocSearch-SearchBar{border-bottom-left-radius:0;border-bottom-right-radius:0;border-bottom-width:1px;border-color:hsl(var(--input));border-top-left-radius:var(--radius);border-top-right-radius:var(--radius);padding:0}.DocSearch-Form{border-bottom-left-radius:0;border-bottom-right-radius:0;border-top-left-radius:var(--radius);border-top-right-radius:var(--radius)}.DocSearch-Cancel{color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;padding-left:.5rem;padding-right:.5rem}.DocSearch-MagnifierLabel,.DocSearch-Search-Icon{stroke-width:2;opacity:.5}.DocSearch-Hit-source{color:hsl(var(--muted-foreground))}.DocSearch-Hit,.DocSearch-Hit a{border-radius:calc(var(--radius) - 4px)}.DocSearch-Hit a:focus-visible{outline-offset:-2px}.DocSearch-Hit[aria-selected=true] a{background-color:hsl(var(--accent));color:hsl(var(--accent-foreground))}.DocSearch-Commands{display:none}.DocSearch-Footer{border-color:hsl(var(--border));border-top-width:1px}
```

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/docsearch_config.js_t` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/docsearch_config.js_t`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-{%- if docsearch_config %}
+{%- if docsearch %}
 docsearch({
-  container: "{{ docsearch_config.container|default('#docsearch') }}",
-  appId: "{{ docsearch_config.app_id }}",
-  apiKey: "{{ docsearch_config.api_key }}",
-  indexName: "{{ docsearch_config.index_name }}",
-  {%- if docsearch_config.initial_query %}
-  initialQuery: "{{ docsearch_config.initial_query }}",
+  container: "{{ docsearch_container|default('#docsearch') }}",
+  appId: "{{ docsearch_app_id }}",
+  apiKey: "{{ docsearch_api_key }}",
+  indexName: "{{ docsearch_index_name }}",
+  {%- if docsearch_initial_query %}
+  initialQuery: "{{ docsearch_initial_query }}",
   {%- endif %}
-  {%- if docsearch_config.placeholder %}
-  placeholder: "{{ docsearch_config.placeholder|default('Search docs') }}",
+  {%- if docsearch_placeholder %}
+  placeholder: "{{ docsearch_placeholder|default('Search docs') }}",
   {%- endif %}
-  {%- if docsearch_config.search_parameters %}
-  searchParameters: "{{ docsearch_config.search_parameters }}",
+  {%- if docsearch_search_parameters %}
+  searchParameters: "{{ docsearch_search_parameters }}",
   {%- endif %}
-  {%- if docsearch_config.missing_results_url %}
+  {%- if docsearch_missing_results_url %}
   getMissingResultsUrl({ query }) {
-    return `{{ docsearch_config.missing_results_url }}`
+    return `{{ docsearch_missing_results_url }}`
   }
   {%- endif %}
 });
 {%- endif %}
```

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/ec416b97881f4a422686.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/ff058b7e238adc5cba09.woff2`

 * *Files identical despite different names*

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/manifest.json` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/manifest.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6296296296296297%*

 * *Differences: {"'_static/awesome-sphinx-design.css'": "'_static/awesome-sphinx-design.f3507627e0af8330cfa7.css'",*

 * * "'_static/docsearch.css'": "'_static/docsearch.445222223e83896718c6.css'",*

 * * "'_static/theme.css'": "'_static/theme.a16405b310edf0713aee.css'",*

 * * "'_static/theme.js'": "'_static/theme.ad172c0f1249198ea036.js'",*

 * * 'delete': "['_static/roboto-latin-500-italic.woff', '_static/roboto-latin-400-italic.woff', "*

 * *           "'_static/roboto-latin-500-normal.woff', '_static/roboto-latin-400-normal.woff', "*

 * *           "' […]*

```diff
@@ -1,29 +1,21 @@
 {
-    "_static/awesome-sphinx-design.css": "_static/awesome-sphinx-design.4ff695238f641b0a2852.css",
+    "_static/awesome-sphinx-design.css": "_static/awesome-sphinx-design.f3507627e0af8330cfa7.css",
     "_static/awesome-sphinx-design.js": "_static/awesome-sphinx-design.31d6cfe0d16ae931b73c.js",
-    "_static/docsearch.css": "_static/docsearch.f30f8b0589fd2b6fd39c.css",
+    "_static/docsearch.css": "_static/docsearch.445222223e83896718c6.css",
     "_static/docsearch.js": "_static/docsearch.f1a1a5835ed7a6ab0c85.js",
     "_static/docsearch_config.js_t": "_static/docsearch_config.js_t",
     "_static/jetbrains-mono-latin-400-italic.woff": "_static/ad463ea60cc8b68792f4.woff",
     "_static/jetbrains-mono-latin-400-italic.woff2": "_static/ff058b7e238adc5cba09.woff2",
     "_static/jetbrains-mono-latin-400-normal.woff": "_static/6f04107ce68d524ebe69.woff",
     "_static/jetbrains-mono-latin-400-normal.woff2": "_static/d0b41bd1d599bc0a52b7.woff2",
     "_static/jetbrains-mono-latin-500-italic.woff": "_static/09be83022f2ac2ce16b0.woff",
     "_static/jetbrains-mono-latin-500-italic.woff2": "_static/31f64b9c465158bd6066.woff2",
     "_static/jetbrains-mono-latin-500-normal.woff": "_static/46830c334f8112fa510a.woff",
     "_static/jetbrains-mono-latin-500-normal.woff2": "_static/ec416b97881f4a422686.woff2",
     "_static/jetbrains-mono-latin-700-italic.woff": "_static/0ffeb7a552b36437b54c.woff",
     "_static/jetbrains-mono-latin-700-italic.woff2": "_static/c3b5f43fe4c8f3f1fa21.woff2",
     "_static/jetbrains-mono-latin-700-normal.woff": "_static/44fd0da18fe361a5cc7f.woff",
     "_static/jetbrains-mono-latin-700-normal.woff2": "_static/cfdd43ce3499ca7f900a.woff2",
-    "_static/roboto-latin-400-italic.woff": "_static/d037cb4792991826de7d.woff",
-    "_static/roboto-latin-400-italic.woff2": "_static/e10742dbb1d4a0864ba8.woff2",
-    "_static/roboto-latin-400-normal.woff": "_static/f1e2a76794cb86b2aa8e.woff",
-    "_static/roboto-latin-400-normal.woff2": "_static/b009a76ad6afe4ebd301.woff2",
-    "_static/roboto-latin-500-italic.woff": "_static/9ac5da2442b734abc516.woff",
-    "_static/roboto-latin-500-italic.woff2": "_static/3a43b67e5bbdfb3ab0a6.woff2",
-    "_static/roboto-latin-500-normal.woff": "_static/48af7707fe9e6494d6a5.woff",
-    "_static/roboto-latin-500-normal.woff2": "_static/f25d774ecfe0996f8eb5.woff2",
-    "_static/theme.css": "_static/theme.c973b470ab69573097f3.css",
-    "_static/theme.js": "_static/theme.c8991bd7bb6e57cbeea8.js"
+    "_static/theme.css": "_static/theme.a16405b310edf0713aee.css",
+    "_static/theme.js": "_static/theme.ad172c0f1249198ea036.js"
 }
```

### Comparing `sphinxawesome_theme-4.1.0/src/sphinxawesome_theme/static/theme.c973b470ab69573097f3.css` & `sphinxawesome_theme-5.0.0b1/src/sphinxawesome_theme/static/theme.a16405b310edf0713aee.css`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-/*! tailwindcss v3.3.2 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-feature-settings:normal;font-family:Roboto,sans-serif;font-variation-settings:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){text-decoration:underline;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:JetBrains\ Mono,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.prose{color:var(--tw-prose-body);max-width:760px}.prose :where(p):not(:where([class~=not-prose] *)){margin-bottom:1.25em;margin-top:1.25em}.prose :where([class~=lead]):not(:where([class~=not-prose] *)){color:var(--tw-prose-lead);font-size:1.25em;line-height:1.6;margin-bottom:1.2em;margin-top:1.2em}.prose :where(a):not(:where([class~=not-prose] *)){color:var(--tw-prose-links);font-weight:400;-webkit-text-decoration:none;text-decoration:none}.prose :where(strong):not(:where([class~=not-prose] *)){color:var(--tw-prose-bold);font-weight:500}.prose :where(a strong):not(:where([class~=not-prose] *)){color:inherit}.prose :where(blockquote strong):not(:where([class~=not-prose] *)){color:inherit}.prose :where(thead th strong):not(:where([class~=not-prose] *)){color:inherit}.prose :where(ol):not(:where([class~=not-prose] *)){list-style-type:decimal;margin-bottom:1.25em;margin-top:1.25em;padding-left:1.625em}.prose :where(ol[type=A]):not(:where([class~=not-prose] *)){list-style-type:upper-alpha}.prose :where(ol[type=a]):not(:where([class~=not-prose] *)){list-style-type:lower-alpha}.prose :where(ol[type=A s]):not(:where([class~=not-prose] *)){list-style-type:upper-alpha}.prose :where(ol[type=a s]):not(:where([class~=not-prose] *)){list-style-type:lower-alpha}.prose :where(ol[type=I]):not(:where([class~=not-prose] *)){list-style-type:upper-roman}.prose :where(ol[type=i]):not(:where([class~=not-prose] *)){list-style-type:lower-roman}.prose :where(ol[type=I s]):not(:where([class~=not-prose] *)){list-style-type:upper-roman}.prose :where(ol[type=i s]):not(:where([class~=not-prose] *)){list-style-type:lower-roman}.prose :where(ol[type="1"]):not(:where([class~=not-prose] *)){list-style-type:decimal}.prose :where(ul):not(:where([class~=not-prose] *)){list-style-type:disc;margin-bottom:1.25em;margin-top:1.25em;padding-left:1.625em}.prose :where(ol>li):not(:where([class~=not-prose] *))::marker{color:var(--tw-prose-counters);font-weight:500}.prose :where(ul>li):not(:where([class~=not-prose] *))::marker{color:var(--tw-prose-bullets)}.prose :where(hr):not(:where([class~=not-prose] *)){border-color:var(--tw-prose-hr);border-top-width:1px;margin-bottom:3em;margin-top:3em}.prose :where(blockquote):not(:where([class~=not-prose] *)){border-left-color:var(--tw-prose-quote-borders);border-left-width:4px;box-shadow:0 1px 3px 0 rgba(0,0,0,.1),0 1px 2px -1px rgba(0,0,0,.1);color:inherit;font-size:.875rem;font-style:normal;font-weight:400;margin-bottom:1.5rem;margin-top:1.5rem;padding:1rem;quotes:"\201C""\201D""\2018""\2019"}.prose :where(h1):not(:where([class~=not-prose] *)){color:var(--tw-prose-headings);font-size:2.5rem;font-weight:400;letter-spacing:-.025em;line-height:1.1111111;margin-bottom:.8888889em;margin-top:5rem}.prose :where(h1 strong):not(:where([class~=not-prose] *)){color:inherit;font-weight:900}.prose :where(h2):not(:where([class~=not-prose] *)){color:var(--tw-prose-headings);font-size:1.75rem;font-weight:400;letter-spacing:-.025em;line-height:1.3333333;margin-bottom:1em;margin-top:2em}.prose :where(h2 strong):not(:where([class~=not-prose] *)){color:inherit;font-weight:800}.prose :where(h3):not(:where([class~=not-prose] *)){color:var(--tw-prose-headings);font-size:1.375rem;font-weight:400;line-height:1.6;margin-bottom:.6em;margin-top:1.6em}.prose :where(h3 strong):not(:where([class~=not-prose] *)){color:inherit;font-weight:700}.prose :where(h4):not(:where([class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:500;line-height:1.5;margin-bottom:.5em;margin-top:1.5em}.prose :where(h4 strong):not(:where([class~=not-prose] *)){color:inherit;font-weight:700}.prose :where(img):not(:where([class~=not-prose] *)){margin-bottom:2em;margin-top:2em}.prose :where(figure>*):not(:where([class~=not-prose] *)){margin-bottom:0;margin-top:0}.prose :where(figcaption):not(:where([class~=not-prose] *)){color:var(--tw-prose-captions);font-size:.875em;line-height:1.4285714;margin-top:.8571429em}.prose :where(code):not(:where([class~=not-prose] *)){background-color:#f3f4f6;border-radius:.125rem;color:var(--tw-prose-code);font-size:.9375em;font-weight:500;padding:1px 4px}.prose :where(a code):not(:where([class~=not-prose] *)){color:inherit}.prose :where(h1 code):not(:where([class~=not-prose] *)){color:inherit}.prose :where(h2 code):not(:where([class~=not-prose] *)){color:inherit;font-size:.875em}.prose :where(h3 code):not(:where([class~=not-prose] *)){color:inherit;font-size:.9em}.prose :where(h4 code):not(:where([class~=not-prose] *)){color:inherit}.prose :where(blockquote code):not(:where([class~=not-prose] *)){color:inherit}.prose :where(thead th code):not(:where([class~=not-prose] *)){color:inherit}.prose :where(pre):not(:where([class~=not-prose] *)){background-color:inherit;border-radius:.125rem;border-width:1px;color:var(--tw-prose-pre-code);font-size:.9375em;font-weight:400;line-height:1.7142857;margin-bottom:0;margin-top:0;overflow-x:auto;padding:.8571429em 1.1428571em}.prose :where(pre code):not(:where([class~=not-prose] *)){background-color:transparent;border-radius:0;border-width:0;color:inherit;font-family:inherit;font-size:inherit;font-weight:inherit;line-height:inherit;padding:0}.prose :where(pre code):not(:where([class~=not-prose] *)):before{content:none}.prose :where(pre code):not(:where([class~=not-prose] *)):after{content:none}.prose :where(table):not(:where([class~=not-prose] *)){font-size:.875em;line-height:1.7142857;margin-bottom:2em;margin-top:2em;table-layout:auto;text-align:left;width:100%}.prose :where(thead):not(:where([class~=not-prose] *)){border-bottom-color:var(--tw-prose-th-borders);border-bottom-width:1px}.prose :where(thead th):not(:where([class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:500;padding-bottom:.5714286em;padding-left:.5714286em;padding-right:.5714286em;vertical-align:bottom}.prose :where(tbody tr):not(:where([class~=not-prose] *)){border-bottom-color:var(--tw-prose-td-borders);border-bottom-width:1px}.prose :where(tbody tr:last-child):not(:where([class~=not-prose] *)){border-bottom-width:0}.prose :where(tbody td):not(:where([class~=not-prose] *)){vertical-align:baseline}.prose :where(tfoot):not(:where([class~=not-prose] *)){border-top-color:var(--tw-prose-th-borders);border-top-width:1px}.prose :where(tfoot td):not(:where([class~=not-prose] *)){vertical-align:top}.prose{--tw-prose-body:var(--color-gray);--tw-prose-headings:var(--color-gray-dark);--tw-prose-lead:var(--color-gray-dark);--tw-prose-links:var(--color-link);--tw-prose-bold:#111827;--tw-prose-counters:var(--color-gray-dark);--tw-prose-bullets:var(--color-gray-light);--tw-prose-hr:#e5e7eb;--tw-prose-quotes:#111827;--tw-prose-quote-borders:#e5e7eb;--tw-prose-captions:var(--color-gray-light);--tw-prose-code:#111827;--tw-prose-pre-code:inherit;--tw-prose-pre-bg:inherit;--tw-prose-th-borders:#d1d5db;--tw-prose-td-borders:#e5e7eb;--tw-prose-invert-body:#d1d5db;--tw-prose-invert-headings:#fff;--tw-prose-invert-lead:#9ca3af;--tw-prose-invert-links:#fff;--tw-prose-invert-bold:#fff;--tw-prose-invert-counters:#9ca3af;--tw-prose-invert-bullets:#4b5563;--tw-prose-invert-hr:#374151;--tw-prose-invert-quotes:#f3f4f6;--tw-prose-invert-quote-borders:#374151;--tw-prose-invert-captions:#9ca3af;--tw-prose-invert-code:#fff;--tw-prose-invert-pre-code:#d1d5db;--tw-prose-invert-pre-bg:rgba(0,0,0,.5);--tw-prose-invert-th-borders:#4b5563;--tw-prose-invert-td-borders:#374151;font-size:1rem;line-height:inherit}.prose :where(video):not(:where([class~=not-prose] *)){margin-bottom:2em;margin-top:2em}.prose :where(figure):not(:where([class~=not-prose] *)){margin-bottom:2em;margin-top:2em}.prose :where(li):not(:where([class~=not-prose] *)){margin-bottom:.5em;margin-top:.5em}.prose :where(ol>li):not(:where([class~=not-prose] *)){padding-left:.375em}.prose :where(ul>li):not(:where([class~=not-prose] *)){padding-left:.375em}.prose :where(.prose>ul>li p):not(:where([class~=not-prose] *)){margin-bottom:.75em;margin-top:.75em}.prose :where(.prose>ul>li>:first-child):not(:where([class~=not-prose] *)){margin-top:1.25em}.prose :where(.prose>ul>li>:last-child):not(:where([class~=not-prose] *)){margin-bottom:1.25em}.prose :where(.prose>ol>li>:first-child):not(:where([class~=not-prose] *)){margin-top:1.25em}.prose :where(.prose>ol>li>:last-child):not(:where([class~=not-prose] *)){margin-bottom:1.25em}.prose :where(ul ul,ul ol,ol ul,ol ol):not(:where([class~=not-prose] *)){margin-bottom:.75em;margin-top:.75em}.prose :where(hr+*):not(:where([class~=not-prose] *)){margin-top:0}.prose :where(h2+*):not(:where([class~=not-prose] *)){margin-top:0}.prose :where(h3+*):not(:where([class~=not-prose] *)){margin-top:0}.prose :where(h4+*):not(:where([class~=not-prose] *)){margin-top:0}.prose :where(thead th:first-child):not(:where([class~=not-prose] *)){padding-left:0}.prose :where(thead th:last-child):not(:where([class~=not-prose] *)){padding-right:0}.prose :where(tbody td,tfoot td):not(:where([class~=not-prose] *)){padding:.5714286em}.prose :where(tbody td:first-child,tfoot td:first-child):not(:where([class~=not-prose] *)){padding-left:0}.prose :where(tbody td:last-child,tfoot td:last-child):not(:where([class~=not-prose] *)){padding-right:0}.prose :where(.prose>:first-child):not(:where([class~=not-prose] *)){margin-top:0}.prose :where(.prose>:last-child):not(:where([class~=not-prose] *)){margin-bottom:0}.prose{--awsm-prose-placeholders:#6b21a8}.prose :where(svg):not(:where([class~=not-prose] *)){display:inline}.prose :where(.rubric):not(:where([class~=not-prose] *)){color:var(--tw-prose-headings);font-weight:500;margin-bottom:.5em}.prose :where(.centered):not(:where([class~=not-prose] *)){text-align:center}.prose :where(.lead+*):not(:where([class~=not-prose] *)){margin-top:3rem}.prose :where(a.toc-backref):not(:where([class~=not-prose] *)){color:inherit}.prose :where(a:hover):not(:where([class~=not-prose] *)){color:#0ea5e9;color:var(--color-brand);-webkit-text-decoration:underline;text-decoration:underline}.prose :where(a:focus):not(:where([class~=not-prose] *)){color:#0ea5e9;color:var(--color-brand);-webkit-text-decoration:underline;text-decoration:underline}.prose :where(ol ol):not(:where([class~=not-prose] *)){list-style:lower-latin}.prose :where(var):not(:where([class~=not-prose] *)){color:var(--awsm-prose-placeholders)}.prose :where(.samp em):not(:where([class~=not-prose] *)){color:var(--awsm-prose-placeholders)}.prose :where(.file em):not(:where([class~=not-prose] *)){color:var(--awsm-prose-placeholders)}.prose :where(.highlight .ge):not(:where([class~=not-prose] *)){color:var(--awsm-prose-placeholders);font-style:italic;font-weight:500}.prose :where(blockquote .attribution):not(:where([class~=not-prose] *)){font-style:italic}.prose :where(blockquote p:last-child):not(:where([class~=not-prose] *)){margin-bottom:0}.prose :where(blockquote p:first-child):not(:where([class~=not-prose] *)){margin-top:0}.prose :where(dl):not(:where([class~=not-prose] *)){margin-bottom:1.25rem;margin-top:1.25rem}.prose :where(dt):not(:where([class~=not-prose] *)){font-weight:500}.prose :where(dd):not(:where([class~=not-prose] *)){padding-left:1.25rem}.prose :where(kbd:not(.compound)):not(:where([class~=not-prose] *)){border-color:#212121;border-color:var(--color-gray-dark);border-radius:.125rem;border-width:1px;box-shadow:1px 1px;display:inline-block;font-size:.75rem;font-weight:500;padding:1px 4px}.prose :where(.option-list kbd):not(:where([class~=not-prose] *)){border-width:0;box-shadow:none;font-size:inherit;font-weight:700}.prose :where(.guilabel):not(:where([class~=not-prose] *)){color:#212121;color:var(--color-gray-dark);font-weight:500;letter-spacing:.025em}.prose :where(.menuselection):not(:where([class~=not-prose] *)){color:#212121;color:var(--color-gray-dark);font-weight:500;letter-spacing:.025em}.prose :where(figure img):not(:where([class~=not-prose] *)){display:inline-block}.prose :where(.align-center):not(:where([class~=not-prose] *)){margin-left:auto;margin-right:auto;text-align:center}.prose :where(.align-right):not(:where([class~=not-prose] *)){margin-left:auto;text-align:right}.prose :where(caption):not(:where([class~=not-prose] *)){margin-bottom:1.5rem;text-align:left}.prose :where(table p:first-child):not(:where([class~=not-prose] *)){margin-top:0}.prose :where(table p:last-child):not(:where([class~=not-prose] *)){margin-bottom:0}.prose :where(.highlight):not(:where([class~=not-prose] *)){position:relative}.prose :where(pre mark):not(:where([class~=not-prose] *)){background-color:#f0f9ff;display:block}.prose :where(pre ins):not(:where([class~=not-prose] *)){background-color:#f0fdf4;display:block;-webkit-text-decoration:none;text-decoration:none}.prose :where(.highlight-diff .gi):not(:where([class~=not-prose] *)){background-color:#f0fdf4;display:inline-block;width:100%}.prose :where(pre del):not(:where([class~=not-prose] *)){background-color:#fef2f2;display:block;-webkit-text-decoration:none;text-decoration:none}.prose :where(.highlight-diff .gd):not(:where([class~=not-prose] *)){background-color:#fef2f2;display:inline-block;width:100%}.prose :where(.highlight .gp):not(:where([class~=not-prose] *)){font-weight:500;pointer-events:none;-webkit-user-select:none;-moz-user-select:none;user-select:none}.prose :where(.highlight .linenos):not(:where([class~=not-prose] *)){padding-right:1rem;-webkit-user-select:none;-moz-user-select:none;user-select:none}.prose :where(.literal-block-wrapper):not(:where([class~=not-prose] *)){border-radius:.125rem;border-width:1px}.prose :where(.literal-block-wrapper pre):not(:where([class~=not-prose] *)){border:none}.prose :where(.pre):not(:where([class~=not-prose] *)){-webkit-hyphens:none;hyphens:none;white-space:nowrap}.prose :where(.code-block-caption):not(:where([class~=not-prose] *)){background-color:#f9fafb;border-bottom-width:1px;border-top-left-radius:.125rem;border-top-right-radius:.125rem;color:var(--tw-prose-captions);display:flex;font-size:.875rem;justify-content:flex-end;letter-spacing:.025em;padding:.25rem}.prose :where(.sig):not(:where([class~=not-prose] *)){font-family:JetBrains\ Mono;font-weight:700}.prose :where(.sig-name):not(:where([class~=not-prose] *)){color:#000}.prose :where(.default_value):not(:where([class~=not-prose] *)){color:var(--awsm-prose-placeholders)}.prose :where(em.property):not(:where([class~=not-prose] *)){color:var(--awsm-prose-placeholders)}.prose :where(.option .sig-prename):not(:where([class~=not-prose] *)){color:var(--awsm-prose-placeholders);font-style:italic}.prose :where(.viewcode-link):not(:where([class~=not-prose] *)){float:right}.prose :where(.font-size-inherit):not(:where([class~=not-prose] *)){font-size:inherit!important}.prose :where(.footnote>.label):not(:where([class~=not-prose] *)){float:left;padding-right:.5rem}.prose :where(.footnote>:not(.label)):not(:where([class~=not-prose] *)){margin-left:2rem}:root{--sidebar-width:300px;--fluid-margin:7.5vw;--color-brand:#0ea5e9;--color-link:#0369a1;--color-gray:#424242;--color-gray-light:#616161;--color-gray-dark:#212121}.admonition,div.deprecated,div.versionadded,div.versionchanged{--tw-shadow:0 1px 3px 0 rgba(0,0,0,.1),0 1px 2px -1px rgba(0,0,0,.1);--tw-shadow-colored:0 1px 3px 0 var(--tw-shadow-color),0 1px 2px -1px var(--tw-shadow-color);border-left-width:4px;border-radius:.125rem;box-shadow:0 0 transparent,0 0 transparent,0 1px 3px 0 rgba(0,0,0,.1),0 1px 2px -1px rgba(0,0,0,.1);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);font-size:.875rem;margin-bottom:1.5rem;margin-top:1.5rem;padding:1rem}.admonition>:last-child,div.deprecated>:last-child,div.versionadded>:last-child,div.versionchanged>:last-child{margin-bottom:0;margin-top:0}.note,[class^=admonition-]:not(.admonition-title){--tw-border-opacity:1;--tw-text-opacity:1;background-color:rgba(56,189,248,.02);border-color:#38bdf8;border-color:rgb(56 189 248/var(--tw-border-opacity));color:#0c4a6e;color:rgb(12 74 110/var(--tw-text-opacity))}.note .headerlink,[class^=admonition-]:not(.admonition-title) .headerlink{color:currentColor}.hint,.tip,div.versionadded{--tw-border-opacity:1;--tw-text-opacity:1;background-color:rgba(74,222,128,.02);border-color:#4ade80;border-color:rgb(74 222 128/var(--tw-border-opacity));color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity))}.danger,.error,div.deprecated{--tw-border-opacity:1;--tw-text-opacity:1;background-color:hsla(0,91%,71%,.02);border-color:#f87171;border-color:rgb(248 113 113/var(--tw-border-opacity));color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity))}.attention,.caution,.important,.warning,div.versionchanged{--tw-border-opacity:1;--tw-text-opacity:1;background-color:rgba(250,204,21,.02);border-color:#facc15;border-color:rgb(250 204 21/var(--tw-border-opacity));color:#713f12;color:rgb(113 63 18/var(--tw-text-opacity))}div.deprecated .versionmodified,div.versionadded .versionmodified,div.versionchanged .versionmodified{font-style:italic;font-weight:500}.admonition-title{font-weight:500;letter-spacing:.025em;margin-bottom:1rem;margin-top:0}@media print{.contents,.toctree-wrapper{display:none}}.contents .caption,.contents .topic-title,.toctree-wrapper .caption,.toctree-wrapper .topic-title{color:#616161;color:var(--color-gray-light);font-family:JetBrains\ Mono,monospace;font-size:.875rem;font-weight:500;letter-spacing:.025em;text-transform:uppercase}.contents ul,.toctree-wrapper ul{list-style-type:none;padding-left:0}.contents ul li,.toctree-wrapper ul li{padding-left:0}.contents ul ul,.toctree-wrapper ul ul{margin-left:1rem}.nav-toc .caption{color:#424242;color:var(--color-gray);font-size:1.125rem;font-weight:500;letter-spacing:.025em;padding-bottom:.75rem;padding-top:2.5rem}.nav-toc p:first-of-type,.nav-toc>ul:first-child{padding-top:1rem}.nav-toc .expand{fill:currentColor;cursor:pointer;display:inline;height:1.2rem;margin-left:-.4rem;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.15s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-timing-function:cubic-bezier(0,0,.2,1);-webkit-user-select:none;-moz-user-select:none;user-select:none}.nav-toc .expand:focus,.nav-toc .expand:hover{color:#0ea5e9;color:var(--color-brand)}.nav-toc li>ul{max-height:0;overflow-y:hidden;padding-left:1rem}.nav-toc .expanded>div>.expand{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.nav-toc .expanded>ul{max-height:100%}.nav-toc .expanded>ul a.current{color:#0ea5e9;color:var(--color-brand)}.nav-toc a{color:#616161;color:var(--color-gray-light);display:inline-block;padding-bottom:.25rem;padding-top:.25rem}.nav-toc a:focus,.nav-toc a:hover{color:#0ea5e9;color:var(--color-brand)}.nav-toc a.current{color:#212121;color:var(--color-gray-dark);font-weight:500}.nav-toc ul+ul{margin-top:2rem}.nav-link{font-size:.95rem;letter-spacing:.2px}.tooltipped{position:relative}.tooltipped:after{-webkit-font-smoothing:subpixel-antialiased;word-wrap:break-word;--tw-bg-opacity:0.75;--tw-text-opacity:1;background-color:rgba(31,41,55,.75);background-color:rgb(31 41 55/var(--tw-bg-opacity));border-radius:.125rem;color:#fff;color:rgb(255 255 255/var(--tw-text-opacity));content:attr(aria-label);display:none;font-size:.75rem;font-weight:400;letter-spacing:normal;letter-spacing:.025em;opacity:0;padding:.25rem .5rem;pointer-events:none;position:absolute;text-align:center;text-decoration-line:none;text-shadow:none;text-transform:none;white-space:pre;z-index:1000000}@keyframes tooltip-appear{0%{opacity:0}to{opacity:1}}.tooltipped:focus:after,.tooltipped:focus:before,.tooltipped:hover:after,.tooltipped:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.tooltipped-no-delay:focus:after,.tooltipped-no-delay:focus:before,.tooltipped-no-delay:hover:after,.tooltipped-no-delay:hover:before{animation-delay:0s}.tooltipped-multiline:focus:after,.tooltipped-multiline:hover:after{display:table-cell}.tooltipped-s:after,.tooltipped-se:after,.tooltipped-sw:after{margin-top:6px;right:50%;top:100%}.tooltipped-s:before,.tooltipped-se:before,.tooltipped-sw:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.tooltipped-se:after{left:50%;margin-left:-16px;right:auto}.tooltipped-sw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-ne:after,.tooltipped-nw:after{bottom:100%;margin-bottom:6px;right:50%}.tooltipped-n:before,.tooltipped-ne:before,.tooltipped-nw:before{border-top-color:#1a202c;bottom:auto;margin-right:-6px;right:50%;top:-7px}.tooltipped-ne:after{left:50%;margin-left:-16px;right:auto}.tooltipped-nw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-s:after{transform:translateX(50%)}.tooltipped-w:after{bottom:50%;margin-right:6px;right:100%;transform:translateY(50%)}.tooltipped-w:before{border-left-color:#1a202c;bottom:50%;left:-7px;margin-top:-6px;top:50%}.tooltipped-e:after{bottom:50%;left:100%;margin-left:6px;transform:translateY(50%)}.tooltipped-e:before{border-right-color:#1a202c;bottom:50%;margin-top:-6px;right:-7px;top:50%}.tooltipped-align-right-1:after,.tooltipped-align-right-2:after{margin-right:0;right:0}.tooltipped-align-right-1:before{right:10px}.tooltipped-align-right-2:before{right:15px}.tooltipped-align-left-1:after,.tooltipped-align-left-2:after{left:0;margin-left:0}.tooltipped-align-left-1:before{left:5px}.tooltipped-align-left-2:before{left:10px}.tooltipped-multiline:after{word-wrap:break-word;border-collapse:separate;max-width:250px;white-space:pre-line;width:-moz-max-content;width:max-content}.tooltipped-multiline.tooltipped-n:after,.tooltipped-multiline.tooltipped-s:after{left:50%;right:auto;transform:translateX(-50%)}.tooltipped-multiline.tooltipped-e:after,.tooltipped-multiline.tooltipped-w:after{right:100%}@media screen and (min-width:0\0){.tooltipped-multiline:after{width:250px}}.tooltipped-sticky:after,.tooltipped-sticky:before{display:inline-block}.tooltipped-sticky.tooltipped-multiline:after{display:table-cell}pre del:before{--tw-text-opacity:1;--tw-content:"\2212";color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity));content:"\2212";content:var(--tw-content);left:2px;position:absolute}pre ins:before{--tw-text-opacity:1;--tw-content:"\002b";color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity));content:"\002b";content:var(--tw-content);left:2px}.highlight .copy,pre ins:before{position:absolute}.highlight .copy{--tw-bg-opacity:1;--tw-text-opacity:1;background-color:#fff;background-color:rgb(255 255 255/var(--tw-bg-opacity));border-radius:.125rem;border-width:1px;color:#374151;color:rgb(55 65 81/var(--tw-text-opacity));font-size:.75rem;letter-spacing:.025em;opacity:0;padding:.25rem;right:.375rem;text-transform:uppercase;top:.75rem;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.5s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);-webkit-user-select:none;-moz-user-select:none;user-select:none}.highlight .copy:focus{opacity:1}.highlight .copy:active{--tw-translate-x:0.125rem;--tw-translate-y:0.125rem;transform:translate(.125rem,.125rem) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.highlight:hover .copy{opacity:1}.code-lang{color:#212121;color:var(--color-gray-dark);display:inline-block;font-family:JetBrains\ Mono,monospace;letter-spacing:.05em;margin-left:.5rem;margin-right:auto;text-transform:uppercase}.sr-only{clip:rect(0,0,0,0);border-width:0;height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;white-space:nowrap;width:1px}.visible{visibility:visible}.invisible{visibility:hidden}.collapse{visibility:collapse}.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.inset-0{left:0;right:0}.inset-0,.inset-y-0{bottom:0;top:0}.bottom-0{bottom:0}.bottom-8{bottom:2rem}.left-0{left:0}.right-0{right:0}.right-8{right:2rem}.top-0{top:0}.z-10{z-index:10}.z-20{z-index:20}.m-4{margin:1rem}.mx-0{margin-left:0;margin-right:0}.mx-5{margin-left:1.25rem;margin-right:1.25rem}.my-8{margin-bottom:2rem;margin-top:2rem}.mb-2{margin-bottom:.5rem}.mb-4{margin-bottom:1rem}.mb-\[2px\]{margin-bottom:2px}.ml-auto{margin-left:auto}.mr-1{margin-right:.25rem}.mr-auto{margin-right:auto}.mt-12{margin-top:3rem}.mt-16{margin-top:4rem}.mt-20{margin-top:5rem}.block{display:block}.inline-block{display:inline-block}.inline{display:inline}.flex{display:flex}.hidden{display:none}.h-14{height:3.5rem}.h-6{height:1.5rem}.h-8{height:2rem}.h-full{height:100%}.min-h-screen{min-height:100vh}.w-0{width:0}.w-14{width:3.5rem}.w-6{width:1.5rem}.w-8{width:2rem}.w-full{width:100%}.max-w-prose{max-width:760px}.flex-1{flex:1 1 0%}.shrink-0{flex-shrink:0}.-translate-x-full{--tw-translate-x:-100%;transform:translate(-100%,var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-y-full{--tw-translate-y:100%;transform:translate(var(--tw-translate-x),100%) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.transform,.translate-y-full{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.transform-gpu{transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.flex-col{flex-direction:column}.items-center{align-items:center}.justify-end{justify-content:flex-end}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.self-center{align-self:center}.overflow-y-auto{overflow-y:auto}.scroll-smooth{scroll-behavior:smooth}.rounded-sm{border-radius:.125rem}.border-b-4{border-bottom-width:4px}.border-brand{border-color:#0ea5e9;border-color:var(--color-brand)}.bg-black{--tw-bg-opacity:1;background-color:#000;background-color:rgb(0 0 0/var(--tw-bg-opacity))}.bg-gray-700{--tw-bg-opacity:1;background-color:#374151;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.bg-gray-900{--tw-bg-opacity:1;background-color:#111827;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.bg-gray-dark{background-color:#212121;background-color:var(--color-gray-dark)}.bg-transparent{background-color:transparent}.bg-white{--tw-bg-opacity:1;background-color:#fff;background-color:rgb(255 255 255/var(--tw-bg-opacity))}.bg-opacity-50{--tw-bg-opacity:0.5}.fill-current{fill:currentColor}.stroke-current{stroke:currentColor}.p-2{padding:.5rem}.p-3{padding:.75rem}.p-4{padding:1rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-4{padding-left:1rem;padding-right:1rem}.pl-2{padding-left:.5rem}.pl-6{padding-left:1.5rem}.pr-2{padding-right:.5rem}.pr-4{padding-right:1rem}.pt-14{padding-top:3.5rem}.pt-4{padding-top:1rem}.pt-8{padding-top:2rem}.text-right{text-align:right}.text-3xl{font-size:2.5rem}.text-4xl{font-size:3rem}.text-sm{font-size:.875rem}.text-xl{font-size:1.5rem}.text-xs{font-size:.75rem}.font-medium{font-weight:500}.uppercase{text-transform:uppercase}.leading-14{line-height:3.5rem}.tracking-wide{letter-spacing:.025em}.tracking-wider{letter-spacing:.05em}.text-gray{color:#424242;color:var(--color-gray)}.text-gray-100{--tw-text-opacity:1;color:#f3f4f6;color:rgb(243 244 246/var(--tw-text-opacity))}.text-gray-300{--tw-text-opacity:1;color:#d1d5db;color:rgb(209 213 219/var(--tw-text-opacity))}.text-gray-600{--tw-text-opacity:1;color:#4b5563;color:rgb(75 85 99/var(--tw-text-opacity))}.text-gray-700{--tw-text-opacity:1;color:#374151;color:rgb(55 65 81/var(--tw-text-opacity))}.text-gray-800{--tw-text-opacity:1;color:#1f2937;color:rgb(31 41 55/var(--tw-text-opacity))}.text-gray-light{color:#616161;color:var(--color-gray-light)}.text-inherit{color:inherit}.text-link{color:#0369a1;color:var(--color-link)}.text-red-700{--tw-text-opacity:1;color:#b91c1c;color:rgb(185 28 28/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:#fff;color:rgb(255 255 255/var(--tw-text-opacity))}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.opacity-0{opacity:0}.shadow-md{--tw-shadow:0 4px 6px -1px rgba(0,0,0,.1),0 2px 4px -2px rgba(0,0,0,.1);--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color),0 2px 4px -2px var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,0 4px 6px -1px rgba(0,0,0,.1),0 2px 4px -2px rgba(0,0,0,.1);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.blur{--tw-blur:blur(8px);filter:blur(8px) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.transition{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-all{transition-duration:.15s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}.duration-100{transition-duration:.1s}.duration-1000{transition-duration:1s}.duration-300{transition-duration:.3s}.duration-500{transition-duration:.5s}.grid-area-header{grid-area:header}.grid-area-sidebar{grid-area:sidebar}.grid-area-main{grid-area:main}.headerlink{--tw-text-opacity:1;align-items:center;color:#9ca3af;color:rgb(156 163 175/var(--tw-text-opacity));display:inline-flex;font-family:Roboto,sans-serif;margin-left:.25rem;vertical-align:middle}.headerlink:focus,.headerlink:hover{color:#0ea5e9;color:var(--color-brand)}.headerlink>*{fill:currentColor;visibility:hidden}.admonition-title:hover .headerlink,.admonition-title:hover .headerlink>*,.code-block-caption:hover .headerlink,.code-block-caption:hover .headerlink>*,.headerlink:focus>*,dt:not(.does-not-exist):hover .headerlink,dt:not(.does-not-exist):hover .headerlink>*,figure:not(.does-not-exist):hover .headerlink,figure:not(.does-not-exist):hover .headerlink>*,h1:not(.does-not-exist):hover .headerlink,h1:not(.does-not-exist):hover .headerlink>*,h2:not(.does-not-exist):hover .headerlink,h2:not(.does-not-exist):hover .headerlink>*,h3:not(.does-not-exist):hover .headerlink,h3:not(.does-not-exist):hover .headerlink>*,h4:not(.does-not-exist):hover .headerlink,h4:not(.does-not-exist):hover .headerlink>*,table:not(.does-not-exist):hover .headerlink,table:not(.does-not-exist):hover .headerlink>*{visibility:visible}#page.isShown{overflow:hidden}[data-sidebar-target=sidebar].isShown{--tw-translate-x:0px;max-width:90%;opacity:1;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));width:100%}[data-scroll-to-top-target=scrollToTop].isShown{opacity:1;visibility:visible}[data-sidebar-target=screen].isShown{display:block}[data-search-target=snackbar].isShown{--tw-translate-y:0px;opacity:1;transform:translate(var(--tw-translate-x)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.5s;transition-timing-function:cubic-bezier(0,0,.2,1)}.focus-within\:absolute:focus-within{position:absolute}.focus-within\:inset-x-0:focus-within{left:0;right:0}.focus-within\:top-0:focus-within{top:0}.focus-within\:bg-gray-50:focus-within{--tw-bg-opacity:1;background-color:#f9fafb;background-color:rgb(249 250 251/var(--tw-bg-opacity))}.focus-within\:text-gray-800:focus-within{--tw-text-opacity:1;color:#1f2937;color:rgb(31 41 55/var(--tw-text-opacity))}.hover\:bg-gray-700:hover{--tw-bg-opacity:1;background-color:#374151;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.hover\:bg-gray-950:hover{--tw-bg-opacity:1;background-color:#030712;background-color:rgb(3 7 18/var(--tw-bg-opacity))}.hover\:text-brand:hover{color:#0ea5e9;color:var(--color-brand)}.hover\:text-gray-dark:hover{color:#212121;color:var(--color-gray-dark)}.hover\:underline:hover{text-decoration-line:underline}.hover\:no-underline:hover{text-decoration-line:none}.focus\:w-full:focus{width:100%}.focus\:translate-x-0:focus{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.focus\:bg-gray-200:focus{--tw-bg-opacity:1;background-color:#e5e7eb;background-color:rgb(229 231 235/var(--tw-bg-opacity))}.focus\:bg-gray-700:focus{--tw-bg-opacity:1;background-color:#374151;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.focus\:bg-gray-950:focus{--tw-bg-opacity:1;background-color:#030712;background-color:rgb(3 7 18/var(--tw-bg-opacity))}.focus\:text-brand:focus{color:#0ea5e9;color:var(--color-brand)}.focus\:text-gray-dark:focus{color:#212121;color:var(--color-gray-dark)}.focus\:underline:focus{text-decoration-line:underline}.focus\:opacity-100:focus{opacity:1}.focus\:outline-none:focus{outline:2px solid transparent;outline-offset:2px}@media (min-width:640px){.sm\:px-4{padding-left:1rem;padding-right:1rem}}@media (min-width:768px){.md\:mx-auto{margin-left:auto;margin-right:auto}.md\:ml-4{margin-left:1rem}.md\:w-auto{width:auto}.md\:focus-within\:static:focus-within{position:static}.md\:focus-within\:w-full:focus-within{width:100%}}@media (min-width:1024px){.lg\:inline-block{display:inline-block}}@media (min-width:1280px){.xl\:relative{position:relative}.xl\:z-0{z-index:0}.xl\:ml-fluid{margin-left:7.5vw;margin-left:var(--fluid-margin)}.xl\:mr-0{margin-right:0}.xl\:grid{display:grid}.xl\:hidden{display:none}.xl\:h-screen{height:100vh}.xl\:translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.xl\:px-2{padding-left:.5rem;padding-right:.5rem}.xl\:opacity-100{opacity:1}.xl\:grid-layout{grid-template-areas:"header header" "sidebar main";grid-template-columns:max(300px,17%) 1fr;grid-template-columns:max(var(--sidebar-width),17%) 1fr;grid-template-rows:min-content 1fr}}@media print{.print\:mt-4{margin-top:1rem}.print\:block{display:block}.print\:hidden{display:none}.print\:h-auto{height:auto}}
-@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:400;src:url(b009a76ad6afe4ebd301.woff2) format("woff2"),url(f1e2a76794cb86b2aa8e.woff) format("woff")}
-@font-face{font-display:swap;font-family:Roboto;font-style:italic;font-weight:400;src:url(e10742dbb1d4a0864ba8.woff2) format("woff2"),url(d037cb4792991826de7d.woff) format("woff")}
-@font-face{font-display:swap;font-family:Roboto;font-style:normal;font-weight:500;src:url(f25d774ecfe0996f8eb5.woff2) format("woff2"),url(48af7707fe9e6494d6a5.woff) format("woff")}
-@font-face{font-display:swap;font-family:Roboto;font-style:italic;font-weight:500;src:url(3a43b67e5bbdfb3ab0a6.woff2) format("woff2"),url(9ac5da2442b734abc516.woff) format("woff")}
+/*! tailwindcss v3.3.2 | MIT License | https://tailwindcss.com*/*,:after,:before{border:0 solid #e5e7eb;box-sizing:border-box}:after,:before{--tw-content:""}html{-webkit-text-size-adjust:100%;font-feature-settings:normal;font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,BlinkMacSystemFont,Helvetica Neue,Arial,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-variation-settings:normal;line-height:1.5;-moz-tab-size:4;-o-tab-size:4;tab-size:4}body{line-height:inherit;margin:0}hr{border-top-width:1px;color:inherit;height:0}abbr:where([title]){text-decoration:underline;-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{border-collapse:collapse;border-color:inherit;text-indent:0}button,input,optgroup,select,textarea{color:inherit;font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{color:#9ca3af;opacity:1}input::placeholder,textarea::placeholder{color:#9ca3af;opacity:1}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{height:auto;max-width:100%}[hidden]{display:none}:root{--background:0 0% 100%;--foreground:222.2 47.4% 11.2%;--muted:210 40% 96.1%;--muted-foreground:215.4 16.3% 46.9%;--popover:0 0% 100%;--popover-foreground:222.2 47.4% 11.2%;--border:214.3 31.8% 91.4%;--input:214.3 31.8% 91.4%;--card:0 0% 100%;--card-foreground:222.2 47.4% 11.2%;--primary:222.2 47.4% 11.2%;--primary-foreground:210 40% 98%;--secondary:210 40% 96.1%;--secondary-foreground:222.2 47.4% 11.2%;--accent:210 40% 96.1%;--accent-foreground:222.2 47.4% 11.2%;--destructive:0 100% 50%;--destructive-foreground:210 40% 98%;--ring:215 20.2% 65.1%;--radius:0.5rem}.dark{--background:224 71% 4%;--foreground:213 31% 91%;--muted:223 47% 11%;--muted-foreground:215.4 16.3% 56.9%;--accent:216 34% 17%;--accent-foreground:210 40% 98%;--popover:224 71% 4%;--popover-foreground:215 20.2% 65.1%;--border:216 34% 17%;--input:216 34% 17%;--card:224 71% 4%;--card-foreground:213 31% 91%;--primary:210 40% 98%;--primary-foreground:222.2 47.4% 1.2%;--secondary:222.2 47.4% 11.2%;--secondary-foreground:210 40% 98%;--destructive:0 63% 31%;--destructive-foreground:210 40% 98%;--ring:216 34% 17%;--radius:0.5rem}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgba(59,130,246,.5);--tw-ring-offset-shadow:0 0 transparent;--tw-ring-shadow:0 0 transparent;--tw-shadow:0 0 transparent;--tw-shadow-colored:0 0 transparent;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.container{margin-left:auto;margin-right:auto;padding-left:2rem;padding-right:2rem;width:100%}@media (min-width:1400px){.container{max-width:1400px}}#content svg{display:inline}#content hr{border-color:#e2e8f0;border-color:hsl(var(--border));margin-bottom:1rem;margin-top:1rem}@media (min-width:768px){#content hr{margin-bottom:1.5rem;margin-top:1.5rem}}#content h1{font-size:2.25rem;font-weight:700;line-height:2.5rem;margin-bottom:.5rem}#content h2{border-bottom-width:1px;border-color:#e2e8f0;border-color:hsl(var(--border));font-size:1.875rem;font-weight:600;line-height:2.25rem;margin-top:3rem;padding-bottom:.5rem}#content h3{font-size:1.5rem;font-weight:600;line-height:2rem;margin-top:2rem}#content .rubric,#content h4{font-size:1.25rem;font-weight:600;line-height:1.75rem;margin-top:2rem}#content section{scroll-margin:5rem}#content section>p{line-height:1.75rem;margin-top:1.5rem}#content section>p.rubric,#content section>p:first-child{margin-top:0}#content section>p.lead{color:#64748b;color:hsl(var(--muted-foreground));font-size:1.125rem;line-height:1.75rem}#content .centered{text-align:center}#content a:not(.toc-backref){color:#0f172a;color:hsl(var(--primary));font-weight:500;text-decoration-line:underline;text-decoration-thickness:from-font;text-underline-offset:4px}#content ul:not(.search){list-style-type:disc;margin-left:1.5rem;margin-top:1.5rem}#content ul:not(.search) p,#content ul:not(.search)>li{margin-top:1.5rem}#content ul:not(.search) ul{margin-top:0}#content ol{list-style-type:decimal;margin-left:1.5rem;margin-top:1.5rem}#content ol ::marker{font-weight:500}#content ol::marker{font-weight:500}#content ol p,#content ol>li{margin-top:1.5rem}#content ol ol{margin-top:0}#content dl{margin-top:1.5rem}#content dl dt:not(.sig){font-weight:500;margin-top:1.5rem}#content dl dt:not(.sig):first-child{margin-bottom:0;margin-top:0}#content dl dd{margin-left:1.5rem}#content dl p{margin-bottom:.5rem;margin-top:.5rem}#content .align-center{margin-left:auto;margin-right:auto;text-align:center}#content .align-right{margin-left:auto;text-align:right}#content img{margin-top:1.5rem}#content figure img{display:inline-block}#content figcaption{color:#64748b;color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;margin-bottom:3rem}#content figcaption>*{margin-top:1rem}blockquote{border-left-width:2px;font-style:italic;margin-bottom:1.5rem;margin-top:1.5rem;padding-left:1.5rem}blockquote .attribution{font-style:normal;margin-top:.5rem}table{font-size:.875rem;line-height:1.25rem;margin-bottom:1.5rem;margin-top:1.5rem;width:100%}table caption{color:#64748b;color:hsl(var(--muted-foreground));margin-bottom:1.5rem;text-align:left}table thead{border-bottom-width:1px;border-color:#e2e8f0;border-color:hsl(var(--border))}table th{font-weight:500;padding-bottom:.5rem;padding-left:.5rem;text-align:left}table th:first-child{padding-left:0}.dark table th{font-weight:600}table tbody tr{border-bottom-width:1px;border-color:#e2e8f0;border-color:hsl(var(--border))}table tbody td{padding:.5rem}table tbody td:first-child{padding-left:0}.footnote>.label{float:left;padding-right:.5rem}.footnote>:not(.label){margin-bottom:1.5rem;margin-left:2rem;margin-top:1.5rem}.footnote .footnote-reference,.footnote [role=doc-backlink]{text-decoration-line:none!important}.admonition{background-color:#fff;background-color:hsl(var(--background));border-color:#e2e8f0;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;color:#0f172a;color:hsl(var(--foreground));font-size:.875rem;line-height:1.25rem;margin-bottom:1.5rem;margin-top:1.5rem;padding:1rem}.admonition p:not(.admonition-title){margin-top:.5rem}.admonition .admonition-title{margin-top:0!important}.admonition-title{font-weight:500}.dark .admonition-title{font-weight:600;letter-spacing:.025em}.note{--tw-border-opacity:1;--tw-bg-opacity:1;--tw-text-opacity:1;background-color:#f0f9ff;background-color:rgb(240 249 255/var(--tw-bg-opacity));border-color:#0284c7;border-color:rgb(2 132 199/var(--tw-border-opacity));color:#0c4a6e;color:rgb(12 74 110/var(--tw-text-opacity))}.dark .note{--tw-text-opacity:1;background-color:rgba(96,165,250,.15);color:#e0f2fe;color:rgb(224 242 254/var(--tw-text-opacity))}.hint,.tip{--tw-border-opacity:1;--tw-bg-opacity:1;--tw-text-opacity:1;background-color:#f0fdf4;background-color:rgb(240 253 244/var(--tw-bg-opacity));border-color:#16a34a;border-color:rgb(22 163 74/var(--tw-border-opacity));color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity))}.dark .hint,.dark .tip{--tw-text-opacity:1;background-color:rgba(74,222,128,.15);color:#dcfce7;color:rgb(220 252 231/var(--tw-text-opacity))}.danger,.error{--tw-border-opacity:1;--tw-bg-opacity:1;--tw-text-opacity:1;background-color:#fef2f2;background-color:rgb(254 242 242/var(--tw-bg-opacity));border-color:#dc2626;border-color:rgb(220 38 38/var(--tw-border-opacity));color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity))}.dark .danger,.dark .error{--tw-text-opacity:1;background-color:hsla(0,91%,71%,.15);color:#fee2e2;color:rgb(254 226 226/var(--tw-text-opacity))}.attention,.caution,.important,.warning{--tw-border-opacity:1;--tw-bg-opacity:1;--tw-text-opacity:1;background-color:#fefce8;background-color:rgb(254 252 232/var(--tw-bg-opacity));border-color:#ca8a04;border-color:rgb(202 138 4/var(--tw-border-opacity));color:#713f12;color:rgb(113 63 18/var(--tw-text-opacity))}.dark .attention,.dark .caution,.dark .important,.dark .warning{--tw-text-opacity:1;background-color:rgba(250,204,21,.15);color:#fef9c3;color:rgb(254 249 195/var(--tw-text-opacity))}div.versionadded{--tw-border-opacity:1;border-color:#16a34a;border-color:rgb(22 163 74/var(--tw-border-opacity));border-left-width:3px;font-size:.875rem;line-height:1.25rem;margin-top:1rem;padding:.25rem 1rem}div.versionadded p{margin-top:0!important}div.versionadded p:last-child{margin-bottom:0!important}div.versionadded .versionmodified{--tw-text-opacity:1;color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity));font-weight:500}.dark div.versionadded .versionmodified{--tw-text-opacity:1;color:#22c55e;color:rgb(34 197 94/var(--tw-text-opacity));letter-spacing:.025em}div.versionchanged{--tw-border-opacity:1;border-color:#ca8a04;border-color:rgb(202 138 4/var(--tw-border-opacity));border-left-width:3px;font-size:.875rem;line-height:1.25rem;margin-top:1rem;padding:.25rem 1rem}div.versionchanged p{margin-top:0!important}div.versionchanged p:last-child{margin-bottom:0!important}div.versionchanged .versionmodified{--tw-text-opacity:1;color:#713f12;color:rgb(113 63 18/var(--tw-text-opacity));font-weight:500}.dark div.versionchanged .versionmodified{--tw-text-opacity:1;color:#eab308;color:rgb(234 179 8/var(--tw-text-opacity));letter-spacing:.025em}div.deprecated{--tw-border-opacity:1;border-color:#dc2626;border-color:rgb(220 38 38/var(--tw-border-opacity));border-left-width:3px;font-size:.875rem;line-height:1.25rem;margin-top:1rem;padding:.25rem 1rem}div.deprecated p{margin-top:0!important}div.deprecated p:last-child{margin-bottom:0!important}div.deprecated .versionmodified{--tw-text-opacity:1;color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity));font-weight:500}.dark div.deprecated .versionmodified{--tw-text-opacity:1;color:#f87171;color:rgb(248 113 113/var(--tw-text-opacity));letter-spacing:.025em}.highlight{background-color:transparent;position:relative}.highlight:hover .copy{opacity:1}.literal-block-wrapper{border-color:#e2e8f0;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;margin-left:0;margin-right:0;margin-top:1.5rem;max-width:none;padding-left:0;padding-right:0}.literal-block-wrapper pre{border-radius:0;border-style:none;margin-top:0}.literal-block-wrapper .code-block-caption{border-bottom-width:1px;border-color:#e2e8f0;border-color:hsl(var(--border));border-top-left-radius:.5rem;border-top-left-radius:var(--radius);border-top-right-radius:.5rem;border-top-right-radius:var(--radius);color:#64748b;color:hsl(var(--muted-foreground));font-size:.875rem;letter-spacing:.025em;line-height:1.25rem;padding:.5rem 1rem}code{background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:.25rem;font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:.875rem;line-height:1.25rem;padding:.2rem .3rem;position:relative;white-space:nowrap}code .ge,code em{color:#0f172a;color:hsl(var(--accent-foreground));font-weight:700;letter-spacing:.025em}pre{border-color:#e2e8f0;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;font-size:.875rem;line-height:1.25rem;margin-top:1.5rem;overflow-x:auto;padding-bottom:1rem;padding-top:1rem}pre[data-theme=dark]{background-color:#fff;background-color:hsl(var(--background))}pre[data-theme=light]{--tw-bg-opacity:1;background-color:#fff;background-color:rgb(255 255 255/var(--tw-bg-opacity))}pre.literal-block{padding-left:1rem;padding-right:1rem}pre code{background-color:transparent;padding:0;white-space:pre}pre code>[id^=line-]{display:block;padding-left:1rem;padding-right:1rem}pre code [id^=line-]:has(.gd),pre code [id^=line-]:has(.gi),pre code [id^=line-]:has(del),pre code [id^=line-]:has(ins),pre code [id^=line-]:has(mark){padding-left:0;padding-right:0}pre code [id^=line-] del,pre code [id^=line-] ins,pre code [id^=line-] mark{display:block;padding-left:1rem;padding-right:1rem;position:relative}pre code [id^=line-] mark{--tw-shadow:2px 0 currentColor inset;--tw-shadow-colored:inset 2px 0 var(--tw-shadow-color);background-color:#f1f5f9;background-color:hsl(var(--muted));box-shadow:0 0 transparent,0 0 transparent,inset 2px 0 currentColor;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);color:inherit}.dark pre code [id^=line-] mark{--tw-bg-opacity:1;--tw-shadow:3px 0 currentColor inset;--tw-shadow-colored:inset 3px 0 var(--tw-shadow-color);background-color:#334155;background-color:rgb(51 65 85/var(--tw-bg-opacity));box-shadow:0 0 transparent,0 0 transparent,inset 3px 0 currentColor;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}pre code [id^=line-] ins{--tw-text-opacity:1;background-color:rgba(34,197,94,.3);color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity));text-decoration-line:none}pre code [id^=line-] ins:before{--tw-content:"\002b";content:"\002b";content:var(--tw-content);left:2px;position:absolute}.dark pre code [id^=line-] ins{--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgb(187 247 208/var(--tw-text-opacity))}pre code [id^=line-] del{--tw-text-opacity:1;background-color:rgba(239,68,68,.3);color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity));text-decoration-line:none}pre code [id^=line-] del:before{--tw-content:"\2212";content:"\2212";content:var(--tw-content);left:2px;position:absolute}.dark pre code [id^=line-] del{--tw-bg-opacity:1;--tw-text-opacity:1;color:#fecaca;color:rgb(254 202 202/var(--tw-text-opacity))}pre .linenos{padding-left:0;padding-right:1rem;-webkit-user-select:none;-moz-user-select:none;user-select:none}.highlight-diff .gi{--tw-text-opacity:1;background-color:rgba(34,197,94,.3);color:#14532d;color:rgb(20 83 45/var(--tw-text-opacity));display:inline-block;padding-left:1rem;padding-right:1rem;width:100%}.dark .highlight-diff .gi{--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgb(187 247 208/var(--tw-text-opacity))}.highlight-diff .gd{--tw-text-opacity:1;background-color:rgba(239,68,68,.3);color:#7f1d1d;color:rgb(127 29 29/var(--tw-text-opacity));display:inline-block;padding-left:1rem;padding-right:1rem;width:100%}.dark .highlight-diff .gd{--tw-bg-opacity:1;--tw-text-opacity:1;color:#bbf7d0;color:rgb(187 247 208/var(--tw-text-opacity))}.guilabel,.menuselection{border-color:#e2e8f0;border-color:hsl(var(--border));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);border-width:1px;color:#0f172a;color:hsl(var(--accent-foreground));font-weight:500;padding:1px .5rem}#content kbd:not(.compound){background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:.25rem;border-width:1px;font-size:.875rem;font-weight:500;letter-spacing:.025em;line-height:1.25rem;padding:1px .25rem}.sig{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-weight:700;scroll-margin:5rem}.sig-name{color:#0f172a;color:hsl(var(--accent-foreground))}em.property{color:#64748b;color:hsl(var(--muted-foreground))}.option .sig-prename{font-style:italic}.viewcode-link{color:#64748b;color:hsl(var(--muted-foreground));float:right}.option-list kbd{background-color:transparent!important;border-style:none!important;font-size:1em!important;font-weight:700!important}.headerlink{align-items:center;display:inline-flex;margin-left:.25rem;position:relative;vertical-align:middle}.headerlink:after{-webkit-font-smoothing:subpixel-antialiased;word-wrap:break-word;--tw-bg-opacity:0.75;background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);color:#64748b;color:hsl(var(--muted-foreground));content:attr(data-tooltip);display:none;font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,BlinkMacSystemFont,Helvetica Neue,Arial,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-size:.75rem;font-weight:400;letter-spacing:normal;line-height:1rem;opacity:0;padding:.25rem;pointer-events:none;position:absolute;text-align:center;text-decoration-line:none;text-shadow:none;text-transform:none;white-space:pre;z-index:1000000}.headerlink:focus:after,.headerlink:focus:before,.headerlink:hover:after,.headerlink:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.headerlink:after{margin-top:6px;right:50%;top:100%}.headerlink:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.headerlink:after{margin-right:-16px}.headerlink>*{fill:currentColor;color:#64748b;color:hsl(var(--muted-foreground));visibility:hidden}.admonition-title:hover .headerlink,.admonition-title:hover .headerlink>*,.code-block-caption:hover .headerlink,.code-block-caption:hover .headerlink>*,.headerlink:focus>*,dt:not(.does-not-exist):hover .headerlink,dt:not(.does-not-exist):hover .headerlink>*,figure:not(.does-not-exist):hover .headerlink,figure:not(.does-not-exist):hover .headerlink>*,h1:not(.does-not-exist):hover .headerlink,h1:not(.does-not-exist):hover .headerlink>*,h2:not(.does-not-exist):hover .headerlink,h2:not(.does-not-exist):hover .headerlink>*,h3:not(.does-not-exist):hover .headerlink,h3:not(.does-not-exist):hover .headerlink>*,h4:not(.does-not-exist):hover .headerlink,h4:not(.does-not-exist):hover .headerlink>*,table:not(.does-not-exist):hover .headerlink,table:not(.does-not-exist):hover .headerlink>*{visibility:visible}#left-sidebar .caption{border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px);font-size:.875rem;font-weight:600;line-height:1.25rem;margin-bottom:.25rem;padding:1.5rem .5rem .25rem}#left-sidebar .caption:first-child{padding-top:0}#left-sidebar ul{display:grid;font-size:.875rem;grid-auto-flow:row;grid-auto-rows:max-content;line-height:1.25rem;overflow:hidden;transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transition-duration:.3s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}@media (prefers-reduced-motion:reduce){#left-sidebar ul{transition-property:none}}#left-sidebar ul ul{margin-left:.75rem;opacity:1;padding:.5rem 0 .5rem .75rem;position:relative;transition-duration:.5s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}#left-sidebar ul ul:before{--tw-bg-opacity:1;--tw-content:"";background-color:#e5e7eb;background-color:rgb(229 231 235/var(--tw-bg-opacity));bottom:.25rem;content:"";content:var(--tw-content);left:0;position:absolute;top:.25rem;width:1px}.dark #left-sidebar ul ul:before{--tw-bg-opacity:1;background-color:#262626;background-color:rgb(38 38 38/var(--tw-bg-opacity));content:var(--tw-content)}#left-sidebar a{align-items:center;border-color:transparent;border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px);border-width:1px;display:flex;padding:.375rem .5rem;width:100%}#left-sidebar a:hover{text-decoration-line:underline}#left-sidebar a:focus-visible{outline-offset:-1px}#left-sidebar a>button{border-radius:.25rem;color:#64748b;color:hsl(var(--muted-foreground))}#left-sidebar a>button:hover{background-color:rgba(15,23,42,.1);background-color:hsl(var(--primary)/.1)}#left-sidebar a>button>svg{transform:translate3d(var(--tw-translate-x),var(--tw-translate-y),0) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform-origin:center;transition-duration:.15s;transition-property:transform;transition-timing-function:cubic-bezier(.4,0,.2,1)}#left-sidebar a.current{background-color:#f1f5f9;background-color:hsl(var(--accent));border-color:#e2e8f0;border-color:hsl(var(--border));border-width:1px;color:#0f172a;color:hsl(var(--accent-foreground));font-weight:500}#left-sidebar a.expandable{justify-content:space-between}#left-sidebar a.expandable.expanded>button>svg{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}#right-sidebar ul{margin:0}#right-sidebar ul li{margin-top:0;padding-top:.5rem}#right-sidebar ul li a{color:#64748b;color:hsl(var(--muted-foreground));display:inline-block;text-decoration-line:none;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}#right-sidebar ul li a:hover{color:#0f172a;color:hsl(var(--foreground))}#right-sidebar ul li a:focus-visible{outline-offset:-1px}#right-sidebar ul li a[data-current=true]{color:#0f172a;color:hsl(var(--foreground));font-weight:500}#right-sidebar ul li ul{padding-left:1rem}#right-sidebar ul:not(:last-child){padding-bottom:.5rem}.contents>:not([hidden])~:not([hidden]),.toctree-wrapper>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:0;margin-bottom:calc(.5rem*var(--tw-space-y-reverse));margin-top:.5rem;margin-top:calc(.5rem*(1 - var(--tw-space-y-reverse)))}.contents,.toctree-wrapper{font-size:.875rem;line-height:1.25rem}.contents .caption,.contents .topic-title,.toctree-wrapper .caption,.toctree-wrapper .topic-title{font-weight:500;padding-top:1.5rem}.contents ul,.toctree-wrapper ul{list-style-type:none!important;margin:0!important}.contents ul li a.reference,.toctree-wrapper ul li a.reference{color:#64748b!important;color:hsl(var(--muted-foreground))!important;display:inline-block;font-weight:400!important;text-decoration-line:none!important;transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.contents ul li a.reference:hover,.toctree-wrapper ul li a.reference:hover{color:#0f172a;color:hsl(var(--foreground))}.contents ul li ul,.toctree-wrapper ul li ul{padding-left:1rem}.contents ul:not(:last-child),.toctree-wrapper ul:not(:last-child){padding-bottom:.5rem}#search-results .search-summary{color:#64748b;color:hsl(var(--muted-foreground));font-size:1.25rem;line-height:1.75rem;margin-top:1.5rem}#search-results ul.search,#search-results ul.search li{margin-top:1.5rem}#search-results ul.search .context{color:#64748b;color:hsl(var(--muted-foreground));font-size:.875rem;line-height:1.25rem;margin-top:.5rem}.highlighted{background-color:#f1f5f9;background-color:hsl(var(--accent));text-decoration-line:underline;text-decoration-thickness:2px}.highlight-link{border-color:#e2e8f0;border-color:hsl(var(--border));border-radius:.5rem;border-radius:var(--radius);border-width:1px;font-size:.875rem;line-height:1.25rem;padding:.5rem 1rem;position:fixed;right:.5rem;top:4rem}.highlight-link:hover{background-color:#f1f5f9;background-color:hsl(var(--accent))}@media (min-width:1024px){.highlight-link{right:4rem}}.tooltipped{position:relative}.tooltipped:after{-webkit-font-smoothing:subpixel-antialiased;word-wrap:break-word;--tw-bg-opacity:0.75;background-color:#f1f5f9;background-color:hsl(var(--muted));border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px);color:#64748b;color:hsl(var(--muted-foreground));content:attr(data-tooltip);display:none;font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,BlinkMacSystemFont,Helvetica Neue,Arial,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-size:.75rem;font-weight:400;letter-spacing:normal;line-height:1rem;opacity:0;padding:.25rem;pointer-events:none;position:absolute;text-align:center;text-decoration-line:none;text-shadow:none;text-transform:none;white-space:pre;z-index:1000000}@keyframes tooltip-appear{0%{opacity:0}to{opacity:1}}.tooltipped:focus:after,.tooltipped:focus:before,.tooltipped:hover:after,.tooltipped:hover:before{animation-delay:.2s;animation-duration:.4s;animation-fill-mode:forwards;animation-name:tooltip-appear;animation-timing-function:ease-in;display:inline-block;-webkit-text-decoration:none;text-decoration:none}.tooltipped-no-delay:focus:after,.tooltipped-no-delay:focus:before,.tooltipped-no-delay:hover:after,.tooltipped-no-delay:hover:before{animation-delay:0s}.tooltipped-multiline:focus:after,.tooltipped-multiline:hover:after{display:table-cell}.tooltipped-s:after,.tooltipped-se:after,.tooltipped-sw:after{margin-top:6px;right:50%;top:100%}.tooltipped-s:before,.tooltipped-se:before,.tooltipped-sw:before{border-bottom-color:#1a202c;bottom:-7px;margin-right:-6px;right:50%;top:auto}.tooltipped-se:after{left:50%;margin-left:-16px;right:auto}.tooltipped-sw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-ne:after,.tooltipped-nw:after{bottom:100%;margin-bottom:6px;right:50%}.tooltipped-n:before,.tooltipped-ne:before,.tooltipped-nw:before{border-top-color:#1a202c;bottom:auto;margin-right:-6px;right:50%;top:-7px}.tooltipped-ne:after{left:50%;margin-left:-16px;right:auto}.tooltipped-nw:after{margin-right:-16px}.tooltipped-n:after,.tooltipped-s:after{transform:translateX(50%)}.tooltipped-w:after{bottom:50%;margin-right:6px;right:100%;transform:translateY(50%)}.tooltipped-w:before{border-left-color:#1a202c;bottom:50%;left:-7px;margin-top:-6px;top:50%}.tooltipped-e:after{bottom:50%;left:100%;margin-left:6px;transform:translateY(50%)}.tooltipped-e:before{border-right-color:#1a202c;bottom:50%;margin-top:-6px;right:-7px;top:50%}.sr-only{clip:rect(0,0,0,0);border-width:0;height:1px;margin:-1px;overflow:hidden;padding:0;position:absolute;white-space:nowrap;width:1px}.pointer-events-none{pointer-events:none}.invisible{visibility:hidden}.collapse{visibility:collapse}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.inset-0{left:0;right:0}.inset-0,.inset-y-0{bottom:0;top:0}.bottom-8{bottom:2rem}.left-0{left:0}.right-1{right:.25rem}.right-1\.5{right:.375rem}.right-4{right:1rem}.right-8{right:2rem}.top-0{top:0}.top-16{top:4rem}.top-2{top:.5rem}.top-4{top:1rem}.z-10{z-index:10}.z-20{z-index:20}.z-40{z-index:40}.z-50{z-index:50}.z-\[100\]{z-index:100}.mx-auto{margin-left:auto;margin-right:auto}.my-4{margin-bottom:1rem;margin-top:1rem}.my-6{margin-bottom:1.5rem;margin-top:1.5rem}.my-8{margin-bottom:2rem;margin-top:2rem}.-mt-10{margin-top:-2.5rem}.mb-4{margin-bottom:1rem}.mb-\[2px\]{margin-bottom:2px}.ml-0{margin-left:0}.ml-2{margin-left:.5rem}.ml-auto{margin-left:auto}.mr-1{margin-right:.25rem}.mr-2{margin-right:.5rem}.mr-4{margin-right:1rem}.mr-6{margin-right:1.5rem}.mr-auto{margin-right:auto}.mt-12{margin-top:3rem}.mt-4{margin-top:1rem}.block{display:block}.inline{display:inline}.flex{display:flex}.inline-flex{display:inline-flex}.table{display:table}.hidden{display:none}.h-10{height:2.5rem}.h-14{height:3.5rem}.h-4{height:1rem}.h-5{height:1.25rem}.h-6{height:1.5rem}.h-9{height:2.25rem}.h-\[14px\]{height:14px}.h-\[calc\(100vh-8rem\)\]{height:calc(100vh - 8rem)}.h-full{height:100%}.max-h-\[calc\(var\(--vh\)-4rem\)\]{max-height:calc(var(--vh) - 4rem)}.min-h-screen{min-height:100vh}.w-4{width:1rem}.w-5\/6{width:83.333333%}.w-6{width:1.5rem}.w-9{width:2.25rem}.w-\[14px\]{width:14px}.w-full{width:100%}.min-w-0{min-width:0}.min-w-full{min-width:100%}.max-w-prose{max-width:65ch}.flex-1{flex:1 1 0%}.shrink-0{flex-shrink:0}.-translate-x-full{--tw-translate-x:-100%;transform:translate(-100%,var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.rotate-0{--tw-rotate:0deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.rotate-90{--tw-rotate:90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.scale-0{--tw-scale-x:0;--tw-scale-y:0;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(0) scaleY(0);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.scale-100{--tw-scale-x:1;--tw-scale-y:1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(1) scaleY(1)}.scale-100,.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.select-none{-webkit-user-select:none;-moz-user-select:none;user-select:none}.flex-col{flex-direction:column}.items-start{align-items:flex-start}.items-center{align-items:center}.\!justify-start{justify-content:flex-start!important}.justify-start{justify-content:flex-start}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-1{gap:.25rem}.gap-4{gap:1rem}.space-x-1>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:.25rem;margin-left:calc(.25rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(.25rem*var(--tw-space-x-reverse))}.space-x-2>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:.5rem;margin-left:calc(.5rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(.5rem*var(--tw-space-x-reverse))}.space-x-6>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:1.5rem;margin-left:calc(1.5rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(1.5rem*var(--tw-space-x-reverse))}.space-y-2>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-bottom:0;margin-bottom:calc(.5rem*var(--tw-space-y-reverse));margin-top:.5rem;margin-top:calc(.5rem*(1 - var(--tw-space-y-reverse)))}.overflow-hidden{overflow:hidden}.overflow-y-auto{overflow-y:auto}.scroll-smooth{scroll-behavior:smooth}.text-ellipsis{text-overflow:ellipsis}.text-clip{text-overflow:clip}.whitespace-nowrap{white-space:nowrap}.rounded{border-radius:.25rem}.rounded-\[0\.5rem\]{border-radius:.5rem}.rounded-md{border-radius:calc(.5rem - 2px);border-radius:calc(var(--radius) - 2px)}.rounded-sm{border-radius:calc(.5rem - 4px);border-radius:calc(var(--radius) - 4px)}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-r{border-right-width:1px}.border-t{border-top-width:1px}.border-border{border-color:#e2e8f0;border-color:hsl(var(--border))}.border-input{border-color:#e2e8f0;border-color:hsl(var(--input))}.bg-background{background-color:#fff;background-color:hsl(var(--background))}.bg-background\/80{background-color:hsla(0,0%,100%,.8);background-color:hsl(var(--background)/.8)}.bg-background\/95{background-color:hsla(0,0%,100%,.95);background-color:hsl(var(--background)/.95)}.bg-gray-700{--tw-bg-opacity:1;background-color:#374151;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.bg-muted{background-color:#f1f5f9;background-color:hsl(var(--muted))}.bg-transparent{background-color:transparent}.fill-current{fill:currentColor}.p-2{padding:.5rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.px-0{padding-left:0;padding-right:0}.px-1{padding-left:.25rem;padding-right:.25rem}.px-1\.5{padding-left:.375rem;padding-right:.375rem}.px-4{padding-left:1rem;padding-right:1rem}.px-8{padding-left:2rem;padding-right:2rem}.py-2{padding-bottom:.5rem;padding-top:.5rem}.py-6{padding-bottom:1.5rem;padding-top:1.5rem}.pr-6{padding-right:1.5rem}.pt-6{padding-top:1.5rem}.text-center{text-align:center}.font-mono{font-family:JetBrains\ Mono,ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace}.font-sans{font-family:ui-sans-serif,system-ui,-apple-system,Segoe UI,Roboto,Ubuntu,Cantarell,Noto Sans,sans-serif,BlinkMacSystemFont,Helvetica Neue,Arial,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji}.text-\[10px\]{font-size:10px}.text-base{font-size:1rem;line-height:1.5rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:.75rem;line-height:1rem}.font-bold{font-weight:700}.font-medium{font-weight:500}.leading-loose{line-height:2}.text-foreground{color:#0f172a;color:hsl(var(--foreground))}.text-foreground\/60{color:rgba(15,23,42,.6);color:hsl(var(--foreground)/.6)}.text-muted-foreground{color:#64748b;color:hsl(var(--muted-foreground))}.text-red-700{--tw-text-opacity:1;color:#b91c1c;color:rgb(185 28 28/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:#fff;color:rgb(255 255 255/var(--tw-text-opacity))}.underline{text-decoration-line:underline}.underline-offset-4{text-underline-offset:4px}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.opacity-0{opacity:0}.opacity-100{opacity:1}.opacity-70{opacity:.7}.shadow-sm{--tw-shadow:0 1px 2px 0 rgba(0,0,0,.05);--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:0 0 transparent,0 0 transparent,0 1px 2px 0 rgba(0,0,0,.05);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.ring-offset-background{--tw-ring-offset-color:hsl(var(--background))}.backdrop-blur{--tw-backdrop-blur:blur(8px);-webkit-backdrop-filter:blur(8px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(8px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.backdrop-blur-sm{--tw-backdrop-blur:blur(4px);-webkit-backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:blur(4px) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-all{transition-duration:.15s;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-colors{transition-duration:.15s;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-timing-function:cubic-bezier(.4,0,.2,1)}.transition-opacity{transition-duration:.15s;transition-property:opacity;transition-timing-function:cubic-bezier(.4,0,.2,1)}.duration-100{transition-duration:.1s}.duration-1000{transition-duration:1s}[x-cloak]{display:none!important}@media (max-width:640px){.container{padding-left:1rem;padding-right:1rem}}.hover\:bg-accent:hover{background-color:#f1f5f9;background-color:hsl(var(--accent))}.hover\:bg-gray-950:hover{--tw-bg-opacity:1;background-color:#030712;background-color:rgb(3 7 18/var(--tw-bg-opacity))}.hover\:bg-muted:hover{background-color:#f1f5f9;background-color:hsl(var(--muted))}.hover\:bg-transparent:hover{background-color:transparent}.hover\:text-accent-foreground:hover{color:#0f172a;color:hsl(var(--accent-foreground))}.hover\:text-foreground:hover{color:#0f172a;color:hsl(var(--foreground))}.hover\:text-foreground\/80:hover{color:rgba(15,23,42,.8);color:hsl(var(--foreground)/.8)}.hover\:placeholder-accent-foreground:hover::-moz-placeholder{color:#0f172a;color:hsl(var(--accent-foreground))}.hover\:placeholder-accent-foreground:hover::placeholder{color:#0f172a;color:hsl(var(--accent-foreground))}.hover\:opacity-100:hover{opacity:1}.focus\:translate-x-0:focus{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.focus\:bg-accent:focus{background-color:#f1f5f9;background-color:hsl(var(--accent))}.focus\:bg-gray-950:focus{--tw-bg-opacity:1;background-color:#030712;background-color:rgb(3 7 18/var(--tw-bg-opacity))}.focus\:text-accent-foreground:focus{color:#0f172a;color:hsl(var(--accent-foreground))}.focus\:opacity-100:focus{opacity:1}.focus-visible\:outline-none:focus-visible{outline:2px solid transparent;outline-offset:2px}.focus-visible\:ring-2:focus-visible{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color),var(--tw-ring-inset) 0 0 0 calc(2px + var(--tw-ring-offset-width)) var(--tw-ring-color),0 0 transparent;box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 #0000)}.focus-visible\:ring-ring:focus-visible{--tw-ring-color:hsl(var(--ring))}.focus-visible\:ring-offset-2:focus-visible{--tw-ring-offset-width:2px}.disabled\:pointer-events-none:disabled{pointer-events:none}.disabled\:opacity-50:disabled{opacity:.5}.group:hover .group-hover\:bg-accent{background-color:#f1f5f9;background-color:hsl(var(--accent))}.group:hover .group-hover\:text-accent-foreground{color:#0f172a;color:hsl(var(--accent-foreground))}.dark .dark\:block{display:block}.dark .dark\:hidden{display:none}.dark .dark\:-rotate-90{--tw-rotate:-90deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(-90deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:rotate-0{--tw-rotate:0deg;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(0deg) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:scale-0{--tw-scale-x:0;--tw-scale-y:0;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(0) scaleY(0);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:scale-100{--tw-scale-x:1;--tw-scale-y:1;transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(1) scaleY(1);transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.dark .dark\:invert{--tw-invert:invert(100%);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) invert(100%) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow);filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}@media (min-width:640px){.sm\:inline-block{display:inline-block}.sm\:flex{display:flex}.sm\:space-x-4>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-left:1rem;margin-left:calc(1rem*(1 - var(--tw-space-x-reverse)));margin-right:0;margin-right:calc(1rem*var(--tw-space-x-reverse))}.sm\:pr-12{padding-right:3rem}}@media (min-width:768px){.md\:sticky{position:sticky}.md\:top-14{top:3.5rem}.md\:z-30{z-index:30}.md\:my-0{margin-bottom:0;margin-top:0}.md\:-ml-2{margin-left:-.5rem}.md\:inline{display:inline}.md\:flex{display:flex}.md\:grid{display:grid}.md\:\!hidden{display:none!important}.md\:hidden{display:none}.md\:h-24{height:6rem}.md\:h-\[calc\(100vh-3\.5rem\)\]{height:calc(100vh - 3.5rem)}.md\:h-auto{height:auto}.md\:w-40{width:10rem}.md\:w-auto{width:auto}.md\:w-full{width:100%}.md\:flex-none{flex:none}.md\:translate-x-0{--tw-translate-x:0px;transform:translateY(var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.md\:grid-cols-\[220px_minmax\(0\2c 1fr\)\]{grid-template-columns:220px minmax(0,1fr)}.md\:flex-row{flex-direction:row}.md\:justify-end{justify-content:flex-end}.md\:gap-2{gap:.5rem}.md\:gap-6{gap:1.5rem}.md\:overflow-auto{overflow:auto}.md\:bg-transparent{background-color:transparent}.md\:p-0{padding:0}.md\:px-0{padding-left:0;padding-right:0}.md\:py-0{padding-bottom:0;padding-top:0}.md\:text-left{text-align:left}}@media (min-width:1024px){.lg\:my-8{margin-bottom:2rem;margin-top:2rem}.lg\:w-64{width:16rem}.lg\:grid-cols-\[240px_minmax\(0\2c 1fr\)\]{grid-template-columns:240px minmax(0,1fr)}.lg\:gap-10{gap:2.5rem}.lg\:py-8{padding-bottom:2rem;padding-top:2rem}}@media (min-width:1280px){.xl\:block{display:block}.xl\:grid{display:grid}.xl\:grid-cols-\[1fr_300px\]{grid-template-columns:1fr 300px}}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:400;src:url(d0b41bd1d599bc0a52b7.woff2) format("woff2"),url(6f04107ce68d524ebe69.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:400;src:url(ff058b7e238adc5cba09.woff2) format("woff2"),url(ad463ea60cc8b68792f4.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:500;src:url(ec416b97881f4a422686.woff2) format("woff2"),url(46830c334f8112fa510a.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:500;src:url(31f64b9c465158bd6066.woff2) format("woff2"),url(09be83022f2ac2ce16b0.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:normal;font-weight:700;src:url(cfdd43ce3499ca7f900a.woff2) format("woff2"),url(44fd0da18fe361a5cc7f.woff) format("woff")}
 @font-face{font-display:swap;font-family:JetBrains Mono;font-style:italic;font-weight:700;src:url(c3b5f43fe4c8f3f1fa21.woff2) format("woff2"),url(0ffeb7a552b36437b54c.woff) format("woff")}
```

### Comparing `sphinxawesome_theme-4.1.0/PKG-INFO` & `sphinxawesome_theme-5.0.0b1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxawesome-theme
-Version: 4.1.0
+Version: 5.0.0b1
 Summary: An awesome theme for the Sphinx documentation generator
 Home-page: https://sphinxawesome.xyz
 License: MIT
 Author: Kai Welke
 Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Framework :: Sphinx
@@ -16,15 +16,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Documentation
 Requires-Dist: beautifulsoup4 (>=4.9.1,<5.0.0)
-Requires-Dist: python-dotenv (>=0.19,<1.1)
 Requires-Dist: sphinx (>4)
 Project-URL: Documentation, https://sphinxawesome.xyz
 Project-URL: Repository, https://github.com/kai687/sphinxawesome-theme
 Description-Content-Type: text/markdown
 
 <h1 align="center">Sphinx awesome theme</h1>
 
@@ -38,57 +37,65 @@
 <p align="center">
    Create beautiful and awesome documentation websites with <a href="https://www.sphinx-doc.org/en/master/">Sphinx</a>.
    See how the theme looks like on <a href="https://sphinxawesome.xyz">sphinxawesome.xyz</a>.
 </p>
 
 ## Get started
 
-To use this theme in your project,
-install it via `pip` and add it to your Sphinx configuration.
-
 1. Install the theme as a Python package:
 
    ```console
    pip install sphinxawesome-theme
    ```
 
-   For more information, see [How to install the theme](https://sphinxawesome.xyz/how-to/install/).
+   For more information, see [Install the theme](https://sphinxawesome.xyz/how-to/install/).
 
-1. Add `sphinxawesome_theme` as an extension and HTML theme in your Sphinx configuration file `conf.py`:
+1. Add `sphinxawesome_theme` as an HTML theme in your Sphinx configuration file `conf.py`:
 
    ```python
    html_theme = "sphinxawesome_theme"
-   extensions = ["sphinxawesome_theme"]
    ```
 
-   For more information, see [How to load the theme](https://sphinxawesome.xyz/how-to/load/) for more information.
+   For more information, see [Add your theme](https://sphinxawesome.xyz/how-to/add/).
+
+1. Optional:
+
+   - If you want to use Algolia DocSearch with this theme,
+     load the bundled extension:
+
+     ```python
+     # conf.py
+     extensions += ["sphinxawesome_theme.docsearch"]
+     ```
+
+   - If you want to use awesome features for highlighting code,
+     load the bundled extension:
+
+     ```python
+     # conf.py
+     extensions += ["sphinxawesome_theme.highlighting"]
+     ```
 
 ## Features
 
 With the Awesome Theme, you can build readable, functional, and beautiful documentation websites.
-These features make your documentation awesome:
 
 ### Awesome code blocks
 
-Code blocks show the language of the code in a header.
-Each code block has a **Copy** button for easy copying.
-This theme enhances Sphinx's `code-block` directive with these options:
-
-- `emphasize-added`. Highlight lines that should be added to code
-- `emphasize-removed`. Highlight lines that should be removed from the code
-- `emphasize-text: TEXT`. Highlight `TEXT` in the code block to emphasize placeholder text the user should replace.
+- Code block have a **Copy** button for copying the code.
+- If you load the bundled `sphinxawesome_theme.highlighting`,
+  you can use these additional options in your ``code-block`` directives:
+
+  - `emphasize-added`. Highlight lines that should be added to code
+  - `emphasize-removed`. Highlight lines that should be removed from the code
+  - `emphasize-text: TEXT`. Highlight _`TEXT`_ in the code block to emphasize placeholder text.
 
 ### Better headerlinks
 
 Clicking the link icon after headers or captions automatically copies the URL to the clipboard.
 
 ### DocSearch
 
 If you have an Algolia DocSearch account for your documentation,
 you can use DocSearch for a search-as-you-type experience with autocomplete.
 Algolia DocSearch is free for open source documentation projects.
 
-### Better keyboard navigation
-
-Use the `Tab` key to skip through all sections on the page.
-Use the `Space` key to expand or collapse items in the navigation menu or in code definitions.
-
```

#### html2text {}

```diff
@@ -1,42 +1,40 @@
-Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 4.1.0 Summary: An
+Metadata-Version: 2.1 Name: sphinxawesome-theme Version: 5.0.0b1 Summary: An
 awesome theme for the Sphinx documentation generator Home-page: https://
 sphinxawesome.xyz License: MIT Author: Kai Welke Author-email: kai687@pm.me
 Requires-Python: >=3.8,<4.0 Classifier: Framework :: Sphinx Classifier:
 Framework :: Sphinx :: Theme Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Documentation Classifier: Topic :: Documentation :: Sphinx Classifier:
 Topic :: Software Development :: Documentation Requires-Dist: beautifulsoup4
-(>=4.9.1,<5.0.0) Requires-Dist: python-dotenv (>=0.19,<1.1) Requires-Dist:
-sphinx (>4) Project-URL: Documentation, https://sphinxawesome.xyz Project-URL:
-Repository, https://github.com/kai687/sphinxawesome-theme Description-Content-
-Type: text/markdown
+(>=4.9.1,<5.0.0) Requires-Dist: sphinx (>4) Project-URL: Documentation, https:/
+/sphinxawesome.xyz Project-URL: Repository, https://github.com/kai687/
+sphinxawesome-theme Description-Content-Type: text/markdown
                       ****** Sphinx awesome theme ******
     [MIT license] [PyPI version] [Netlify Deploy] [GitHub Workflow Status]
  Create beautiful and awesome documentation websites with Sphinx. See how the
                     theme looks like on sphinxawesome.xyz.
-## Get started To use this theme in your project, install it via `pip` and add
-it to your Sphinx configuration. 1. Install the theme as a Python package:
-```console pip install sphinxawesome-theme ``` For more information, see [How
-to install the theme](https://sphinxawesome.xyz/how-to/install/). 1. Add
-`sphinxawesome_theme` as an extension and HTML theme in your Sphinx
-configuration file `conf.py`: ```python html_theme = "sphinxawesome_theme"
-extensions = ["sphinxawesome_theme"] ``` For more information, see [How to load
-the theme](https://sphinxawesome.xyz/how-to/load/) for more information. ##
-Features With the Awesome Theme, you can build readable, functional, and
-beautiful documentation websites. These features make your documentation
-awesome: ### Awesome code blocks Code blocks show the language of the code in a
-header. Each code block has a **Copy** button for easy copying. This theme
-enhances Sphinx's `code-block` directive with these options: - `emphasize-
-added`. Highlight lines that should be added to code - `emphasize-removed`.
-Highlight lines that should be removed from the code - `emphasize-text: TEXT`.
-Highlight `TEXT` in the code block to emphasize placeholder text the user
-should replace. ### Better headerlinks Clicking the link icon after headers or
-captions automatically copies the URL to the clipboard. ### DocSearch If you
-have an Algolia DocSearch account for your documentation, you can use DocSearch
-for a search-as-you-type experience with autocomplete. Algolia DocSearch is
-free for open source documentation projects. ### Better keyboard navigation Use
-the `Tab` key to skip through all sections on the page. Use the `Space` key to
-expand or collapse items in the navigation menu or in code definitions.
+## Get started 1. Install the theme as a Python package: ```console pip install
+sphinxawesome-theme ``` For more information, see [Install the theme](https://
+sphinxawesome.xyz/how-to/install/). 1. Add `sphinxawesome_theme` as an HTML
+theme in your Sphinx configuration file `conf.py`: ```python html_theme =
+"sphinxawesome_theme" ``` For more information, see [Add your theme](https://
+sphinxawesome.xyz/how-to/add/). 1. Optional: - If you want to use Algolia
+DocSearch with this theme, load the bundled extension: ```python # conf.py
+extensions += ["sphinxawesome_theme.docsearch"] ``` - If you want to use
+awesome features for highlighting code, load the bundled extension: ```python #
+conf.py extensions += ["sphinxawesome_theme.highlighting"] ``` ## Features With
+the Awesome Theme, you can build readable, functional, and beautiful
+documentation websites. ### Awesome code blocks - Code block have a **Copy**
+button for copying the code. - If you load the bundled
+`sphinxawesome_theme.highlighting`, you can use these additional options in
+your ``code-block`` directives: - `emphasize-added`. Highlight lines that
+should be added to code - `emphasize-removed`. Highlight lines that should be
+removed from the code - `emphasize-text: TEXT`. Highlight _`TEXT`_ in the code
+block to emphasize placeholder text. ### Better headerlinks Clicking the link
+icon after headers or captions automatically copies the URL to the clipboard.
+### DocSearch If you have an Algolia DocSearch account for your documentation,
+you can use DocSearch for a search-as-you-type experience with autocomplete.
+Algolia DocSearch is free for open source documentation projects.
```

