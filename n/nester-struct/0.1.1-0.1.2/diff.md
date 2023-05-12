# Comparing `tmp/nester-struct-0.1.1.tar.gz` & `tmp/nester-struct-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nester-struct-0.1.1.tar", last modified: Thu May 11 08:09:22 2023, max compression
+gzip compressed data, was "nester-struct-0.1.2.tar", last modified: Fri May 12 15:41:28 2023, max compression
```

## Comparing `nester-struct-0.1.1.tar` & `nester-struct-0.1.2.tar`

### file list

```diff
@@ -1,158 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.759224 nester-struct-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.759224 nester-struct-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.759224 nester-struct-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.github/workflows/increase_version.yml
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.github/workflows/label.yml
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.github/workflows/newsfragment_checker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.github/workflows/packaging.yml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.github/workflows/towncrier.yml
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-11 08:08:58.000000 nester-struct-0.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-11 08:08:58.000000 nester-struct-0.1.1/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-11 08:08:58.000000 nester-struct-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-11 08:08:58.000000 nester-struct-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-11 08:08:58.000000 nester-struct-0.1.1/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 08:08:58.000000 nester-struct-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-11 08:09:22.775225 nester-struct-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-11 08:08:58.000000 nester-struct-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-11 08:08:58.000000 nester-struct-0.1.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.759224 nester-struct-0.1.1/changelog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:08:58.000000 nester-struct-0.1.1/changelog/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.759224 nester-struct-0.1.1/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-11 08:08:58.000000 nester-struct-0.1.1/changelog.d/changelog_template.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.759224 nester-struct-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.755223 nester-struct-0.1.1/docs/_build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.763224 nester-struct-0.1.1/docs/_build/html/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.763224 nester-struct-0.1.1/docs/_build/html/.doctrees/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/.doctrees/dev_docs.doctree
--rw-r--r--   0 runner    (1001) docker     (123)   110815 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/.doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/.doctrees/index.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/.doctrees/installation_guide.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.763224 nester-struct-0.1.1/docs/_build/html/.doctrees/source/
--rw-r--r--   0 runner    (1001) docker     (123)    28309 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/.doctrees/source/utils.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/.doctrees/supported_languages.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    19176 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/.doctrees/usage_guide.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.763224 nester-struct-0.1.1/docs/_build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_sources/dev_docs.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_sources/installation_guide.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.763224 nester-struct-0.1.1/docs/_build/html/_sources/source/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_sources/source/utils.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_sources/supported_languages.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_sources/usage_guide.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.767224 nester-struct-0.1.1/docs/_build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.767224 nester-struct-0.1.1/docs/_build/html/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/badge_only.css
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.771225 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    87624 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    86288 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   323344 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   193308 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   309728 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)   184912 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   328412 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   195704 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   309192 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 runner    (1001) docker     (123)   182708 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   135235 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/file.png
--rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/index_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.771225 nester-struct-0.1.1/docs/_build/html/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/js/badge_only.js
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/_static/sphinx_highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/dev_docs.html
--rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/installation_guide.html
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/searchindex.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.771225 nester-struct-0.1.1/docs/_build/html/source/
--rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/source/utils.html
--rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/supported_languages.html
--rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_build/html/usage_guide.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.771225 nester-struct-0.1.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/_static/index_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/dev_docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/installation_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/source/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/supported_languages.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-11 08:08:58.000000 nester-struct-0.1.1/docs/usage_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/img/
--rw-r--r--   0 runner    (1001) docker     (123)    70052 2023-05-11 08:08:58.000000 nester-struct-0.1.1/img/logo_social_preview.png
--rw-r--r--   0 runner    (1001) docker     (123)    62005 2023-05-11 08:08:58.000000 nester-struct-0.1.1/img/logo_thumbnail.png
--rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-05-11 08:08:58.000000 nester-struct-0.1.1/index_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-11 08:08:58.000000 nester-struct-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-11 08:09:22.775225 nester-struct-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.755223 nester-struct-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/src/nester/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 08:08:58.000000 nester-struct-0.1.1/src/nester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-11 08:08:58.000000 nester-struct-0.1.1/src/nester/nester_commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.755223 nester-struct-0.1.1/src/nester/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/src/nester/templates/c/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:08:58.000000 nester-struct-0.1.1/src/nester/templates/c/c_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/src/nester/templates/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:08:58.000000 nester-struct-0.1.1/src/nester/templates/cpp/cpp_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/src/nester/templates/cs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:08:58.000000 nester-struct-0.1.1/src/nester/templates/cs/cs_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/src/nester/templates/java/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:08:58.000000 nester-struct-0.1.1/src/nester/templates/java/java_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/src/nester/templates/py/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-11 08:08:58.000000 nester-struct-0.1.1/src/nester/templates/py/py_layout.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/src/nester/templates/rb/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-11 08:08:58.000000 nester-struct-0.1.1/src/nester/templates/rb/rb_layout.json
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-11 08:08:58.000000 nester-struct-0.1.1/src/nester/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/src/nester_struct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-11 08:09:22.000000 nester-struct-0.1.1/src/nester_struct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-11 08:09:22.000000 nester-struct-0.1.1/src/nester_struct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:09:22.000000 nester-struct-0.1.1/src/nester_struct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 08:09:22.000000 nester-struct-0.1.1/src/nester_struct.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-11 08:09:22.000000 nester-struct-0.1.1/src/nester_struct.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 08:09:22.000000 nester-struct-0.1.1/src/nester_struct.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 08:09:22.000000 nester-struct-0.1.1/src/nester_struct.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:08:58.000000 nester-struct-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/tests/interation_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:08:58.000000 nester-struct-0.1.1/tests/interation_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-11 08:08:58.000000 nester-struct-0.1.1/tests/interation_tests/test_util_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 08:09:22.775225 nester-struct-0.1.1/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 08:08:58.000000 nester-struct-0.1.1/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-11 08:08:58.000000 nester-struct-0.1.1/tests/unit_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.034017 nester-struct-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.018016 nester-struct-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.018016 nester-struct-0.1.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.018016 nester-struct-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/workflows/increase_version.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/workflows/label.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/workflows/newsfragment_checker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/workflows/packaging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.github/workflows/towncrier.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-12 15:41:11.000000 nester-struct-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-12 15:41:11.000000 nester-struct-0.1.2/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-12 15:41:11.000000 nester-struct-0.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-05-12 15:41:11.000000 nester-struct-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-12 15:41:11.000000 nester-struct-0.1.2/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-12 15:41:11.000000 nester-struct-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-12 15:41:28.034017 nester-struct-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-12 15:41:11.000000 nester-struct-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 15:41:11.000000 nester-struct-0.1.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.018016 nester-struct-0.1.2/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:11.000000 nester-struct-0.1.2/changelog/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.018016 nester-struct-0.1.2/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-12 15:41:11.000000 nester-struct-0.1.2/changelog.d/changelog_template.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.022016 nester-struct-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.014016 nester-struct-0.1.2/docs/_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.022016 nester-struct-0.1.2/docs/_build/html/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.022016 nester-struct-0.1.2/docs/_build/html/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/.doctrees/dev_docs.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)   110815 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/.doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/.doctrees/index.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/.doctrees/installation_guide.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.022016 nester-struct-0.1.2/docs/_build/html/.doctrees/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    28309 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/.doctrees/source/utils.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/.doctrees/supported_languages.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)    19176 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/.doctrees/usage_guide.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.022016 nester-struct-0.1.2/docs/_build/html/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_sources/dev_docs.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_sources/installation_guide.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.022016 nester-struct-0.1.2/docs/_build/html/_sources/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_sources/source/utils.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_sources/supported_languages.rst.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_sources/usage_guide.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.026016 nester-struct-0.1.2/docs/_build/html/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/basic.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.026016 nester-struct-0.1.2/docs/_build/html/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/badge_only.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.030017 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    87624 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    86288 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   323344 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   193308 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   309728 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   184912 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   328412 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   195704 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   309192 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   182708 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   135235 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/css/theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/index_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.030017 nester-struct-0.1.2/docs/_build/html/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/js/badge_only.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/js/html5shiv.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/js/theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/dev_docs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6253 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/installation_guide.html
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/py-modindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.030017 nester-struct-0.1.2/docs/_build/html/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    13389 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/source/utils.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/supported_languages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9821 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_build/html/usage_guide.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.030017 nester-struct-0.1.2/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.030017 nester-struct-0.1.2/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/_static/index_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/dev_docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/installation_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.030017 nester-struct-0.1.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/source/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/supported_languages.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-12 15:41:11.000000 nester-struct-0.1.2/docs/usage_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.030017 nester-struct-0.1.2/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    70052 2023-05-12 15:41:11.000000 nester-struct-0.1.2/img/logo_social_preview.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62005 2023-05-12 15:41:11.000000 nester-struct-0.1.2/img/logo_thumbnail.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86196 2023-05-12 15:41:11.000000 nester-struct-0.1.2/index_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-12 15:41:11.000000 nester-struct-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-12 15:41:28.034017 nester-struct-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.014016 nester-struct-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.034017 nester-struct-0.1.2/src/nester/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 15:41:11.000000 nester-struct-0.1.2/src/nester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-12 15:41:11.000000 nester-struct-0.1.2/src/nester/nester_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.014016 nester-struct-0.1.2/src/nester/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.034017 nester-struct-0.1.2/src/nester/templates/c/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-12 15:41:11.000000 nester-struct-0.1.2/src/nester/templates/c/c_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.034017 nester-struct-0.1.2/src/nester/templates/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-12 15:41:11.000000 nester-struct-0.1.2/src/nester/templates/cpp/cpp_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.034017 nester-struct-0.1.2/src/nester/templates/cs/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-12 15:41:11.000000 nester-struct-0.1.2/src/nester/templates/cs/cs_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.034017 nester-struct-0.1.2/src/nester/templates/java/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-12 15:41:11.000000 nester-struct-0.1.2/src/nester/templates/java/java_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.034017 nester-struct-0.1.2/src/nester/templates/py/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-12 15:41:11.000000 nester-struct-0.1.2/src/nester/templates/py/py_layout.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.034017 nester-struct-0.1.2/src/nester/templates/rb/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-12 15:41:11.000000 nester-struct-0.1.2/src/nester/templates/rb/rb_layout.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-12 15:41:11.000000 nester-struct-0.1.2/src/nester/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.034017 nester-struct-0.1.2/src/nester_struct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-05-12 15:41:27.000000 nester-struct-0.1.2/src/nester_struct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-12 15:41:28.000000 nester-struct-0.1.2/src/nester_struct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:41:27.000000 nester-struct-0.1.2/src/nester_struct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-12 15:41:27.000000 nester-struct-0.1.2/src/nester_struct.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-12 15:41:27.000000 nester-struct-0.1.2/src/nester_struct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 15:41:27.000000 nester-struct-0.1.2/src/nester_struct.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:41:27.000000 nester-struct-0.1.2/src/nester_struct.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.034017 nester-struct-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:11.000000 nester-struct-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.034017 nester-struct-0.1.2/tests/interation_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:11.000000 nester-struct-0.1.2/tests/interation_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-12 15:41:11.000000 nester-struct-0.1.2/tests/interation_tests/test_util_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:28.034017 nester-struct-0.1.2/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:41:11.000000 nester-struct-0.1.2/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-12 15:41:11.000000 nester-struct-0.1.2/tests/unit_tests/test_utils.py
```

### Comparing `nester-struct-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `nester-struct-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `nester-struct-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/.github/PULL_REQUEST_TEMPLATE.md` & `nester-struct-0.1.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/.github/workflows/codeql.yml` & `nester-struct-0.1.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/.github/workflows/increase_version.yml` & `nester-struct-0.1.2/.github/workflows/increase_version.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/.github/workflows/label.yml` & `nester-struct-0.1.2/.github/workflows/label.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/.github/workflows/newsfragment_checker.yml` & `nester-struct-0.1.2/.github/workflows/newsfragment_checker.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/.github/workflows/packaging.yml` & `nester-struct-0.1.2/.github/workflows/packaging.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/.github/workflows/pylint.yml` & `nester-struct-0.1.2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/.github/workflows/towncrier.yml` & `nester-struct-0.1.2/.github/workflows/towncrier.yml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/.pre-commit-config.yaml` & `nester-struct-0.1.2/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -6,18 +6,12 @@
         args: ["--verbose", "--safe"]
         # It is recommended to specify the latest version of Python
         # supported by your project here, or alternatively use
         # pre-commit's default_language_version, see
         # https://pre-commit.com/#top_level-default_language_version
         language_version: python3.10
         additional_dependencies: ['click==8.1.3']
-  # condlict with pre-commit. Will stay deactivated for now.
-  # Run isort manually like this :
-  #
-  # isort --profile black .
-  #
-  # while in the project's root directory.
-  # - repo: https://github.com/pycqa/isort
-  #   rev: 5.6.4
-  #   hooks:
-  #     - id: isort
-  #       args: ["--profile", "black", "--filter-files"]
+  - repo: https://github.com/pycqa/isort
+    rev: 5.12.0
+    hooks:
+      - id: isort
+        args: ["--profile", "black", "--filter-files"]
```

### Comparing `nester-struct-0.1.1/CODE_OF_CONDUCT.md` & `nester-struct-0.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/CONTRIBUTING.md` & `nester-struct-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/INSTALL.md` & `nester-struct-0.1.2/INSTALL.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/LICENSE` & `nester-struct-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/PKG-INFO` & `nester-struct-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nester-struct
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automated creation of project structure
 Home-page: https://github.com/ByteOtter/nester
 Author: Christopher Hock
 Author-email: christopher-hock@protonmail.com
 License: GPLv3.0
 Keywords: automation,project_structure,python
 Classifier: Natural Language :: English
```

### Comparing `nester-struct-0.1.1/README.md` & `nester-struct-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/Makefile` & `nester-struct-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/.doctrees/dev_docs.doctree` & `nester-struct-0.1.2/docs/_build/html/.doctrees/dev_docs.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/.doctrees/environment.pickle` & `nester-struct-0.1.2/docs/_build/html/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/.doctrees/index.doctree` & `nester-struct-0.1.2/docs/_build/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/.doctrees/installation_guide.doctree` & `nester-struct-0.1.2/docs/_build/html/.doctrees/installation_guide.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/.doctrees/source/utils.doctree` & `nester-struct-0.1.2/docs/_build/html/.doctrees/source/utils.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/.doctrees/supported_languages.doctree` & `nester-struct-0.1.2/docs/_build/html/.doctrees/supported_languages.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/.doctrees/usage_guide.doctree` & `nester-struct-0.1.2/docs/_build/html/.doctrees/usage_guide.doctree`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_sources/index.rst.txt` & `nester-struct-0.1.2/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_sources/installation_guide.rst.txt` & `nester-struct-0.1.2/docs/_build/html/_sources/installation_guide.rst.txt`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_sources/supported_languages.rst.txt` & `nester-struct-0.1.2/docs/_build/html/_sources/supported_languages.rst.txt`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_sources/usage_guide.rst.txt` & `nester-struct-0.1.2/docs/_build/html/_sources/usage_guide.rst.txt`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/basic.css` & `nester-struct-0.1.2/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/badge_only.css` & `nester-struct-0.1.2/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/custom.css` & `nester-struct-0.1.2/docs/_build/html/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-bold.woff` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-normal.woff` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `nester-struct-0.1.2/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/css/theme.css` & `nester-struct-0.1.2/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/doctools.js` & `nester-struct-0.1.2/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/index_logo.png` & `nester-struct-0.1.2/docs/_build/html/_static/index_logo.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/js/badge_only.js` & `nester-struct-0.1.2/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `nester-struct-0.1.2/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/js/html5shiv.min.js` & `nester-struct-0.1.2/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/js/theme.js` & `nester-struct-0.1.2/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/language_data.js` & `nester-struct-0.1.2/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/pygments.css` & `nester-struct-0.1.2/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/searchtools.js` & `nester-struct-0.1.2/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/_static/sphinx_highlight.js` & `nester-struct-0.1.2/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/dev_docs.html` & `nester-struct-0.1.2/docs/_build/html/dev_docs.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/genindex.html` & `nester-struct-0.1.2/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/index.html` & `nester-struct-0.1.2/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/installation_guide.html` & `nester-struct-0.1.2/docs/_build/html/installation_guide.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/py-modindex.html` & `nester-struct-0.1.2/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/search.html` & `nester-struct-0.1.2/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/searchindex.js` & `nester-struct-0.1.2/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/source/utils.html` & `nester-struct-0.1.2/docs/_build/html/source/utils.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/supported_languages.html` & `nester-struct-0.1.2/docs/_build/html/supported_languages.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_build/html/usage_guide.html` & `nester-struct-0.1.2/docs/_build/html/usage_guide.html`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_static/css/custom.css` & `nester-struct-0.1.2/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/_static/index_logo.png` & `nester-struct-0.1.2/docs/_static/index_logo.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/conf.py` & `nester-struct-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/index.rst` & `nester-struct-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/installation_guide.rst` & `nester-struct-0.1.2/docs/installation_guide.rst`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/supported_languages.rst` & `nester-struct-0.1.2/docs/supported_languages.rst`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/docs/usage_guide.rst` & `nester-struct-0.1.2/docs/usage_guide.rst`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/img/logo_social_preview.png` & `nester-struct-0.1.2/img/logo_social_preview.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/img/logo_thumbnail.png` & `nester-struct-0.1.2/img/logo_thumbnail.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/index_logo.png` & `nester-struct-0.1.2/index_logo.png`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/pyproject.toml` & `nester-struct-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/setup.cfg` & `nester-struct-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/src/nester/nester_commands.py` & `nester-struct-0.1.2/src/nester/nester_commands.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/src/nester/utils.py` & `nester-struct-0.1.2/src/nester/utils.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/src/nester_struct.egg-info/PKG-INFO` & `nester-struct-0.1.2/src/nester_struct.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nester-struct
-Version: 0.1.1
+Version: 0.1.2
 Summary: Automated creation of project structure
 Home-page: https://github.com/ByteOtter/nester
 Author: Christopher Hock
 Author-email: christopher-hock@protonmail.com
 License: GPLv3.0
 Keywords: automation,project_structure,python
 Classifier: Natural Language :: English
```

### Comparing `nester-struct-0.1.1/src/nester_struct.egg-info/SOURCES.txt` & `nester-struct-0.1.2/src/nester_struct.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 .github/workflows/black.yml
 .github/workflows/codeql.yml
 .github/workflows/increase_version.yml
 .github/workflows/label.yml
 .github/workflows/newsfragment_checker.yml
 .github/workflows/packaging.yml
 .github/workflows/pylint.yml
+.github/workflows/tests.yml
 .github/workflows/towncrier.yml
 changelog/.gitkeep
 changelog.d/changelog_template.jinja
 docs/Makefile
 docs/conf.py
 docs/dev_docs.rst
 docs/index.rst
```

### Comparing `nester-struct-0.1.1/tests/interation_tests/test_util_integration.py` & `nester-struct-0.1.2/tests/interation_tests/test_util_integration.py`

 * *Files identical despite different names*

### Comparing `nester-struct-0.1.1/tests/unit_tests/test_utils.py` & `nester-struct-0.1.2/tests/unit_tests/test_utils.py`

 * *Files identical despite different names*

