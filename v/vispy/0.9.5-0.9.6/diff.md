# Comparing `tmp/vispy-0.9.5.tar.gz` & `tmp/vispy-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/vispy/vispy/dist/tmpnzme9voq/vispy-0.9.5.tar", last modified: Fri Feb  4 16:44:04 2022, max compression
+gzip compressed data, was "/home/runner/work/vispy/vispy/dist/tmpdwipy3lr/vispy-0.9.6.tar", last modified: Fri Feb  4 22:14:17 2022, max compression
```

## Comparing `vispy-0.9.5.tar` & `vispy-0.9.6.tar`

### file list

```diff
@@ -1,902 +1,902 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-02-04 16:43:35.000000 vispy-0.9.5/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-04 16:43:35.000000 vispy-0.9.5/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-02-04 16:43:35.000000 vispy-0.9.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)    10126 2022-02-04 16:43:35.000000 vispy-0.9.5/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-02-04 16:43:35.000000 vispy-0.9.5/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-02-04 16:43:35.000000 vispy-0.9.5/.github_changelog_generator
--rw-r--r--   0 runner    (1001) docker     (121)      375 2022-02-04 16:43:35.000000 vispy-0.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)    29160 2022-02-04 16:43:35.000000 vispy-0.9.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-02-04 16:43:35.000000 vispy-0.9.5/CITATION.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5491 2022-02-04 16:43:35.000000 vispy-0.9.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-02-04 16:43:35.000000 vispy-0.9.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-02-04 16:43:35.000000 vispy-0.9.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-02-04 16:43:35.000000 vispy-0.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6540 2022-02-04 16:44:04.000000 vispy-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5141 2022-02-04 16:43:35.000000 vispy-0.9.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/ci/
--rwxr-xr-x   0 runner    (1001) docker     (121)      399 2022-02-04 16:43:35.000000 vispy-0.9.5/ci/build_website.sh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-02-04 16:43:35.000000 vispy-0.9.5/ci/requirements/linux_full_deps_apt.txt
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-02-04 16:43:35.000000 vispy-0.9.5/ci/requirements/linux_full_deps_conda.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-04 16:43:35.000000 vispy-0.9.5/ci/requirements/linux_full_deps_pip.txt
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-02-04 16:43:35.000000 vispy-0.9.5/ci/requirements/linux_full_newqtdeps_apt.txt
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-02-04 16:43:35.000000 vispy-0.9.5/ci/requirements/linux_full_newqtdeps_conda.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-04 16:43:35.000000 vispy-0.9.5/ci/requirements/linux_full_newqtdeps_pip.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 16:43:35.000000 vispy-0.9.5/ci/requirements/linux_min_deps_conda.txt
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-02-04 16:43:35.000000 vispy-0.9.5/ci/requirements/linux_osmesa_deps_conda.txt
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-02-04 16:43:35.000000 vispy-0.9.5/ci/requirements/linux_website_deps_pip.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-04 16:43:35.000000 vispy-0.9.5/ci/requirements/py37.yml
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-04 16:43:35.000000 vispy-0.9.5/ci/requirements/py39.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/doc/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/CNAME
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (121)   154714 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/ViewFrustum.png
--rw-r--r--   0 runner    (1001) docker     (121)    84235 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/ViewFrustum.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/doc/_static/carousel/
--rw-r--r--   0 runner    (1001) docker     (121)   317728 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/carousel/galaxy.png
--rw-r--r--   0 runner    (1001) docker     (121)    57799 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/carousel/high-frequency.png
--rw-r--r--   0 runner    (1001) docker     (121)    76838 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/carousel/mandelbrot.png
--rw-r--r--   0 runner    (1001) docker     (121)   176107 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/carousel/signals.png
--rw-r--r--   0 runner    (1001) docker     (121)    59110 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)    10073 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/frustum-matrix.png
--rw-r--r--   0 runner    (1001) docker     (121)    41660 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/gl-history.png
--rw-r--r--   0 runner    (1001) docker     (121)    22485 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/gl-pipeline.png
--rw-r--r--   0 runner    (1001) docker     (121)    44757 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/gl-pipeline.svg
--rw-r--r--   0 runner    (1001) docker     (121)     9583 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/ortho-matrix.png
--rw-r--r--   0 runner    (1001) docker     (121)     8828 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/perspective-matrix.png
--rw-r--r--   0 runner    (1001) docker     (121)      755 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/style.css
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/vispy-logo-V.png
--rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/vispy-logo-V.svg
--rw-r--r--   0 runner    (1001) docker     (121)     7398 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/vispy-teaser-short.png
--rw-r--r--   0 runner    (1001) docker     (121)   172644 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/vispy-teaser-short.svg
--rw-r--r--   0 runner    (1001) docker     (121)     8772 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/vispy-teaser.png
--rw-r--r--   0 runner    (1001) docker     (121)   175454 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/vispy-teaser.svg
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/vispy-text-white.png
--rw-r--r--   0 runner    (1001) docker     (121)   171862 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/_static/vispy-text-white.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/doc/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/api/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/community.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12429 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/doc/dev_guide/
--rw-r--r--   0 runner    (1001) docker     (121)    11542 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/dev_guide/contributor_guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/dev_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4716 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/dev_guide/writing_examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6954 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/faq.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/doc/gallery/
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/gallery/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/doc/getting_started/
--rw-r--r--   0 runner    (1001) docker     (121)     3051 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/getting_started/_canvas_app.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12840 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/getting_started/gloo.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/getting_started/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    12434 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/getting_started/modern-gl.rst
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/getting_started/plot.rst
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/getting_started/scene.rst
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/getting_started/visuals.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9770 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/news.rst
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/overview.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3616 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/raspberry.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4989 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/resources.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7990 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/roadmap.rst
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-02-04 16:43:35.000000 vispy-0.9.5/doc/thirdparty.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/basics/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/basics/scene/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/basics/scene/modular_shaders/
--rw-r--r--   0 runner    (1001) docker     (121)     7047 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/scene/modular_shaders/editor.py
--rw-r--r--   0 runner    (1001) docker     (121)    14616 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/scene/modular_shaders/sandbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/scene/shared_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/scene/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/basics/visuals/
--rw-r--r--   0 runner    (1001) docker     (121)     2434 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/arcball.py
--rw-r--r--   0 runner    (1001) docker     (121)     3212 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/arrows.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2757 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/arrows_quiver.py
--rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/axially_symmetric_surfaces.py
--rw-r--r--   0 runner    (1001) docker     (121)     2517 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/bezier.py
--rw-r--r--   0 runner    (1001) docker     (121)     2139 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/box.py
--rw-r--r--   0 runner    (1001) docker     (121)     4597 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/colorbar_visual.py
--rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/colorbar_visual_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4375 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/custom_visual.py
--rw-r--r--   0 runner    (1001) docker     (121)     4329 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/dynamic_polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)     1797 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/grid_mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     4391 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/image_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/image_visual.py
--rw-r--r--   0 runner    (1001) docker     (121)     3899 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/line.py
--rw-r--r--   0 runner    (1001) docker     (121)     6863 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/line_draw.py
--rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/line_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/line_plot3d.py
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/line_plot_axes.py
--rw-r--r--   0 runner    (1001) docker     (121)     9955 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/line_prototype.py
--rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/line_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/markers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4601 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/networkx_layout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/plane.py
--rw-r--r--   0 runner    (1001) docker     (121)     3615 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/polygon_visual.py
--rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/rescalingmarkers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/rotating_box.py
--rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/text_scatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     6161 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/text_visual.py
--rw-r--r--   0 runner    (1001) docker     (121)     2293 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/tube.py
--rw-r--r--   0 runner    (1001) docker     (121)     3395 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/visual_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/basics/visuals/windbarb_quiver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/benchmark/
--rw-r--r--   0 runner    (1001) docker     (121)    10795 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/benchmark/scene_test_1.py
--rw-r--r--   0 runner    (1001) docker     (121)     6012 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/benchmark/scene_test_2.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1378 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/benchmark/simple_glut.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      834 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/benchmark/simple_vispy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/collections/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2133 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/collections/chloropleth.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1197 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/collections/path_collection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      926 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/collections/point_collection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1286 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/collections/polygon_collection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1017 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/collections/segment_collection.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2454 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/collections/tiger.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1718 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/collections/triangle_collection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/demo/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/demo/gloo/
--rw-r--r--   0 runner    (1001) docker     (121)     5269 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/atom.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5748 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/boids.py
--rw-r--r--   0 runner    (1001) docker     (121)     4568 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/brain.py
--rw-r--r--   0 runner    (1001) docker     (121)     2228 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/camera.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7679 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     5725 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/donut.py
--rw-r--r--   0 runner    (1001) docker     (121)     4036 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/fireworks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/demo/gloo/galaxy/
--rwxr-xr-x   0 runner    (1001) docker     (121)     6043 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/galaxy/galaxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     7679 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/galaxy/galaxy_simulation.py
--rw-r--r--   0 runner    (1001) docker     (121)    13768 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/galaxy/galaxy_specrend.py
--rw-r--r--   0 runner    (1001) docker     (121)     5938 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/galaxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5759 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/game_of_life.py
--rw-r--r--   0 runner    (1001) docker     (121)     5000 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/glsl_sandbox_cube.py
--rw-r--r--   0 runner    (1001) docker     (121)     4899 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     7375 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/grayscott.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3392 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/high_frequency.py
--rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/imshow.py
--rw-r--r--   0 runner    (1001) docker     (121)     5308 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/imshow_cuts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/demo/gloo/jfa/
--rwxr-xr-x   0 runner    (1001) docker     (121)      701 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/jfa/fragment_display.glsl
--rwxr-xr-x   0 runner    (1001) docker     (121)     5690 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/jfa/fragment_flood.glsl
--rwxr-xr-x   0 runner    (1001) docker     (121)      655 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/jfa/fragment_seed.glsl
--rw-r--r--   0 runner    (1001) docker     (121)    10260 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/jfa/jfa_translation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/jfa/jfa_vispy.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      672 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/jfa/vertex.glsl
--rwxr-xr-x   0 runner    (1001) docker     (121)      726 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/jfa/vertex_vispy.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     5551 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/mandelbrot.py
--rw-r--r--   0 runner    (1001) docker     (121)     8913 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/mandelbrot_double.py
--rw-r--r--   0 runner    (1001) docker     (121)     5961 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/molecular_viewer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4318 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/ndscatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4233 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/offscreen.py
--rw-r--r--   0 runner    (1001) docker     (121)    13632 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/primitive_mesh_viewer_qt.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2368 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/quiver.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4084 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/rain.py
--rw-r--r--   0 runner    (1001) docker     (121)     7178 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/raytracing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4575 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/realtime_signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     3780 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     5418 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/skybox.py
--rw-r--r--   0 runner    (1001) docker     (121)     4985 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/spacy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6734 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/terrain.py
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/two_qt_widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)     7365 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/unstructured_2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     3309 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/gloo/voronoi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/demo/plot/
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/plot/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/demo/scene/
--rw-r--r--   0 runner    (1001) docker     (121)     6673 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/scene/flow_lines.py
--rw-r--r--   0 runner    (1001) docker     (121)     3285 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/scene/force_directed_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/scene/klein.py
--rw-r--r--   0 runner    (1001) docker     (121)    10222 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/scene/oscilloscope.py
--rw-r--r--   0 runner    (1001) docker     (121)     2977 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/scene/picking.py
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/scene/scrolling_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/demo/visuals/
--rw-r--r--   0 runner    (1001) docker     (121)    34342 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/demo/visuals/wiggly_bar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/gloo/
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3038 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/animate_images.py
--rw-r--r--   0 runner    (1001) docker     (121)     4279 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/animate_images_slice.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3072 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/animate_shape.py
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/colored_quad.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3843 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/display_lines.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2519 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/display_points.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1325 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/display_shape.py
--rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/geometry_shader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3304 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/gpuimage.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3449 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/hello_fbo.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2164 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/multi_texture.py
--rw-r--r--   0 runner    (1001) docker     (121)     4873 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/post_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5317 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/rotate_cube.py
--rw-r--r--   0 runner    (1001) docker     (121)     2226 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/rotating_quad.py
--rw-r--r--   0 runner    (1001) docker     (121)     3354 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/spatial_filters.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      395 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/start.py
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/gloo/start_shaders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/jupyter/
--rw-r--r--   0 runner    (1001) docker     (121)     3614 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/jupyter/Rotating Cube.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     3851 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/jupyter/colormaps.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     7023 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/jupyter/gloo_display_lines.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     9521 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/jupyter/gloo_molecular_viewer.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/offscreen/
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/offscreen/simple_egl.py
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/offscreen/simple_osmesa.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/plotting/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/plotting/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/plotting/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/plotting/export.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      592 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/plotting/ipython_fig_playground.py
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/plotting/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/plotting/plot_colorbars.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1127 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/plotting/scatter_histogram.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/plotting/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/plotting/volume_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/scene/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/axes_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)      948 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/background_borders.py
--rw-r--r--   0 runner    (1001) docker     (121)     2693 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/clipping_planes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/colorbar_widget.py
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/colored_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/console.py
--rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/contour.py
--rw-r--r--   0 runner    (1001) docker     (121)     7041 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/example..gif
--rw-r--r--   0 runner    (1001) docker     (121)     2778 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/example.png
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/flipped_axis.py
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/scene/grid_layout/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/grid_layout/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/grid_layout/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/grid_layout/grid_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/grid_layout/grid_holed.py
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/grid_layout/grid_large.py
--rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/grid_layout/grid_uneven_col.py
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/grid_layout/grid_x_y_viewbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/infinite_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/isocurve.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/isocurve_for_trisurface.py
--rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/isocurve_for_trisurface_qt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4549 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/isocurve_updates.py
--rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/isosurface.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/line.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/line_update.py
--rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/linear_region.py
--rw-r--r--   0 runner    (1001) docker     (121)     3377 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/magnify.py
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/marker_spheres.py
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/mesh_normals.py
--rw-r--r--   0 runner    (1001) docker     (121)     3824 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/mesh_shading.py
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/mesh_texture.py
--rw-r--r--   0 runner    (1001) docker     (121)     4539 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/nested_viewbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/one_cam_two_scenes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/one_scene_four_cams.py
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/point_cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)     1717 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/save_animation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (121)    13158 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/shape_draw.py
--rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/sphere.py
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/surface_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/text.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/turntable_box.py
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/viewbox.py
--rw-r--r--   0 runner    (1001) docker     (121)     4994 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/volume.py
--rw-r--r--   0 runner    (1001) docker     (121)     4293 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/scene/volume_plane.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/tutorial/app/
--rw-r--r--   0 runner    (1001) docker     (121)     1846 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/app/app_events.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/app/fps.py
--rw-r--r--   0 runner    (1001) docker     (121)     2905 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/app/shared_context.py
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/app/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/app/simple_wx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/tutorial/gl/
--rw-r--r--   0 runner    (1001) docker     (121)     8364 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/gl/cube.py
--rw-r--r--   0 runner    (1001) docker     (121)     5538 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/gl/fireworks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3639 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/gl/quad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/tutorial/gloo/
--rw-r--r--   0 runner    (1001) docker     (121)     2641 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/gloo/colored_cube.py
--rw-r--r--   0 runner    (1001) docker     (121)     5020 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/gloo/lighted_cube.py
--rw-r--r--   0 runner    (1001) docker     (121)     3457 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/gloo/outlined_cube.py
--rw-r--r--   0 runner    (1001) docker     (121)     4053 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/gloo/texture_precision.py
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/gloo/textured_cube.py
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/gloo/textured_quad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/examples/tutorial/visuals/
--rw-r--r--   0 runner    (1001) docker     (121)     6494 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/visuals/T01_basic_visual.py
--rw-r--r--   0 runner    (1001) docker     (121)     8240 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/visuals/T02_measurements.py
--rw-r--r--   0 runner    (1001) docker     (121)     8118 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/visuals/T03_antialiasing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2438 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/visuals/T04_fragment_programs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-02-04 16:43:35.000000 vispy-0.9.5/examples/tutorial/visuals/T05_viewer_location.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-02-04 16:43:35.000000 vispy-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-02-04 16:43:35.000000 vispy-0.9.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      296 2022-02-04 16:44:04.000000 vispy-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5062 2022-02-04 16:43:35.000000 vispy-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/app/
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/_default_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     6474 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/_detect_eventloop.py
--rw-r--r--   0 runner    (1001) docker     (121)    10631 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/application.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/app/backends/
--rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8478 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_egl.py
--rw-r--r--   0 runner    (1001) docker     (121)    17018 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_glfw.py
--rw-r--r--   0 runner    (1001) docker     (121)     8805 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_jupyter_rfb.py
--rw-r--r--   0 runner    (1001) docker     (121)     3697 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_offscreen_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     7602 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_osmesa.py
--rw-r--r--   0 runner    (1001) docker     (121)    14963 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_pyglet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_pyqt4.py
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_pyqt5.py
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_pyqt6.py
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_pyside.py
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_pyside2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_pyside6.py
--rw-r--r--   0 runner    (1001) docker     (121)    34839 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_qt.py
--rw-r--r--   0 runner    (1001) docker     (121)    15100 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_sdl2.py
--rw-r--r--   0 runner    (1001) docker     (121)     7953 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_template.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    26111 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_tk.py
--rw-r--r--   0 runner    (1001) docker     (121)    14864 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/_wx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/app/backends/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/tests/test_offscreen_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/backends/tests/test_rfb.py
--rw-r--r--   0 runner    (1001) docker     (121)    10799 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    28638 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/canvas.py
--rw-r--r--   0 runner    (1001) docker     (121)     3411 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/qt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/app/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/tests/qt-designer.ui
--rw-r--r--   0 runner    (1001) docker     (121)    15781 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     6394 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/tests/test_canvas.py
--rw-r--r--   0 runner    (1001) docker     (121)     3579 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (121)     4527 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/tests/test_simultaneous.py
--rw-r--r--   0 runner    (1001) docker     (121)     5754 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/app/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/color/
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5224 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/color/_color_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)    14194 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/color/color_array.py
--rw-r--r--   0 runner    (1001) docker     (121)     6051 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/color/color_space.py
--rw-r--r--   0 runner    (1001) docker     (121)    43616 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/color/colormap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/color/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/color/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12919 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/color/tests/test_color.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/ext/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    54240 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/ext/cocoapy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5340 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/ext/cubehelix.py
--rw-r--r--   0 runner    (1001) docker     (121)    12160 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/ext/egl.py
--rw-r--r--   0 runner    (1001) docker     (121)     4236 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/ext/fontconfig.py
--rw-r--r--   0 runner    (1001) docker     (121)     6617 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/ext/gdi32plus.py
--rw-r--r--   0 runner    (1001) docker     (121)     3411 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/ext/osmesa.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/geometry/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5130 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/_triangulation_debugger.py
--rw-r--r--   0 runner    (1001) docker     (121)     4245 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/calculations.py
--rw-r--r--   0 runner    (1001) docker     (121)    13145 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/curves.py
--rw-r--r--   0 runner    (1001) docker     (121)    20941 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/generation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5796 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/isocurve.py
--rw-r--r--   0 runner    (1001) docker     (121)    20651 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/isosurface.py
--rw-r--r--   0 runner    (1001) docker     (121)    25329 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/meshdata.py
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/normals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/parametric.py
--rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)     5481 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/rect.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/geometry/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/tests/test_calculations.py
--rw-r--r--   0 runner    (1001) docker     (121)     2110 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/tests/test_generation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/tests/test_meshdata.py
--rw-r--r--   0 runner    (1001) docker     (121)    12700 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/tests/test_triangulation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4262 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/torusknot.py
--rw-r--r--   0 runner    (1001) docker     (121)    31968 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/geometry/triangulation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/gloo/
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16454 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/buffer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8640 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     9350 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/framebuffer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/gloo/gl/
--rw-r--r--   0 runner    (1001) docker     (121)     7952 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16615 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/_constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    38247 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/_es2.py
--rw-r--r--   0 runner    (1001) docker     (121)    54470 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/_gl2.py
--rw-r--r--   0 runner    (1001) docker     (121)    14644 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)    11646 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/_pyopengl2.py
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/dummy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/es2.py
--rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/gl2.py
--rw-r--r--   0 runner    (1001) docker     (121)     9274 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/glplus.py
--rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/pyopengl2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/gloo/gl/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9223 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (121)    17340 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/tests/test_functionality.py
--rw-r--r--   0 runner    (1001) docker     (121)    11101 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/tests/test_names.py
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/gl/tests/test_use.py
--rw-r--r--   0 runner    (1001) docker     (121)    65293 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/glir.py
--rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/globject.py
--rw-r--r--   0 runner    (1001) docker     (121)     2291 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (121)    21335 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/program.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/gloo/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19819 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/tests/test_buffer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     5482 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/tests/test_framebuffer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9644 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/tests/test_glir.py
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/tests/test_globject.py
--rw-r--r--   0 runner    (1001) docker     (121)    11414 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/tests/test_program.py
--rw-r--r--   0 runner    (1001) docker     (121)    23993 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/tests/test_texture.py
--rw-r--r--   0 runner    (1001) docker     (121)     6495 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/tests/test_use_gloo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     8689 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/tests/test_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)    37450 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/texture.py
--rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    26390 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/gloo/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/glsl/
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/glsl/antialias/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/antialias/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/antialias/antialias.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/antialias/cap-butt.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/antialias/cap-round.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/antialias/cap-square.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/antialias/cap-triangle-in.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/antialias/cap-triangle-out.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/antialias/cap.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/antialias/caps.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/antialias/filled.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/antialias/outline.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/antialias/stroke.glsl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/glsl/arrowheads/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrowheads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrowheads/angle.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrowheads/arrowheads.frag
--rw-r--r--   0 runner    (1001) docker     (121)      477 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrowheads/arrowheads.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrowheads/arrowheads.vert
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrowheads/curved.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrowheads/inhibitor.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrowheads/stealth.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrowheads/triangle.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrowheads/util.glsl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/glsl/arrows/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/angle-30.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/angle-60.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/angle-90.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/arrow.frag
--rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/arrow.vert
--rw-r--r--   0 runner    (1001) docker     (121)      562 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/arrows.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     6397 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/common.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/curved.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/stealth.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/triangle-30.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/triangle-60.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/triangle-90.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/arrows/util.glsl
--rw-r--r--   0 runner    (1001) docker     (121)    20717 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/build_spatial_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/glsl/collections/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/agg-fast-path.frag
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/agg-fast-path.vert
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/agg-glyph.frag
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/agg-glyph.vert
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/agg-marker.frag
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/agg-marker.vert
--rw-r--r--   0 runner    (1001) docker     (121)     1846 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/agg-path.frag
--rw-r--r--   0 runner    (1001) docker     (121)     4987 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/agg-path.vert
--rw-r--r--   0 runner    (1001) docker     (121)      707 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/agg-point.frag
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/agg-point.vert
--rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/agg-segment.frag
--rw-r--r--   0 runner    (1001) docker     (121)     2075 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/agg-segment.vert
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/marker.frag
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/marker.vert
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/raw-path.frag
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/raw-path.vert
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/raw-point.frag
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/raw-point.vert
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/raw-segment.frag
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/raw-segment.vert
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/raw-triangle.frag
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/raw-triangle.vert
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/sdf-glyph-ticks.vert
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/sdf-glyph.frag
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/sdf-glyph.vert
--rw-r--r--   0 runner    (1001) docker     (121)     2344 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/collections/tick-labels.vert
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/glsl/colormaps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/autumn.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/blues.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      553 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/color-space.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      781 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/colormaps.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      641 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/cool.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      688 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/fire.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/gray.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      639 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/greens.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      721 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/hot.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/ice.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/icefire.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/reds.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/spring.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/summer.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      652 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/user.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/util.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/wheel.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/colormaps/winter.glsl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/glsl/lines/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/lines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9887 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/lines/agg.frag
--rw-r--r--   0 runner    (1001) docker     (121)     7620 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/lines/agg.vert
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/glsl/markers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/arrow.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      695 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/asterisk.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      601 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/chevron.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/clover.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/club.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/cross.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/diamond.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/disc.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/ellipse.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/hbar.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/heart.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/infinity.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     2936 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/marker-sdf.frag
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/marker-sdf.vert
--rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/marker.frag
--rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/marker.vert
--rw-r--r--   0 runner    (1001) docker     (121)      849 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/markers.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/pin.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/ring.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/spade.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/square.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/tag.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/triangle.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      369 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/markers/vbar.glsl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/glsl/math/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/math/circle-through-2-points.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/math/constants.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     3045 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/math/double.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/math/functions.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/math/point-to-line-distance.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/math/point-to-line-projection.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      812 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/math/signed-line-distance.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/math/signed-segment-distance.glsl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/glsl/misc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6828 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/misc/regular-grid.frag
--rw-r--r--   0 runner    (1001) docker     (121)    15813 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/misc/spatial-filters.frag
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/misc/viewport-NDC.glsl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/glsl/transforms/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/azimuthal-equal-area.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/azimuthal-equidistant.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/hammer.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/identity.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/identity_forward.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/identity_inverse.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/linear-scale.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/log-scale.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/mercator-transverse-forward.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/mercator-transverse-inverse.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/panzoom.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/polar.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/position.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/power-scale.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/projection.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/pvm.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/rotate.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/trackball.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/translate.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/transverse_mercator.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/viewport-clipping.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/viewport-transform.glsl
--rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/viewport.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/x.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/y.glsl
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/glsl/transforms/z.glsl
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/io/
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/io/_data/
--rw-r--r--   0 runner    (1001) docker     (121)    65616 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/io/_data/spatial-filters.npy
--rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/io/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     6180 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/io/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     3559 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/io/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     5942 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/io/stl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/io/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/io/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     4223 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/io/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)    12285 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/io/wavefront.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/plot/
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/plot/fig.py
--rw-r--r--   0 runner    (1001) docker     (121)    18595 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/plot/plotwidget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/plot/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/plot/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/plot/tests/test_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/scene/
--rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/scene/cameras/
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/cameras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/cameras/_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/cameras/arcball.py
--rw-r--r--   0 runner    (1001) docker     (121)    18614 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/cameras/base_camera.py
--rw-r--r--   0 runner    (1001) docker     (121)    16343 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/cameras/fly.py
--rw-r--r--   0 runner    (1001) docker     (121)     5387 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/cameras/magnify.py
--rw-r--r--   0 runner    (1001) docker     (121)    10917 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/cameras/panzoom.py
--rw-r--r--   0 runner    (1001) docker     (121)    11617 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/cameras/perspective.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/scene/cameras/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/cameras/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/cameras/tests/test_link.py
--rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/cameras/tests/test_perspective.py
--rw-r--r--   0 runner    (1001) docker     (121)     5351 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/cameras/turntable.py
--rw-r--r--   0 runner    (1001) docker     (121)    22619 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/canvas.py
--rw-r--r--   0 runner    (1001) docker     (121)     2185 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/events.py
--rw-r--r--   0 runner    (1001) docker     (121)    19029 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/node.py
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/subscene.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/scene/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3292 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/tests/test_canvas.py
--rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/tests/test_visuals.py
--rw-r--r--   0 runner    (1001) docker     (121)     9741 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/visuals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/scene/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/widgets/anchor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/widgets/axis.py
--rw-r--r--   0 runner    (1001) docker     (121)     6158 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/widgets/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (121)    14013 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/widgets/console.py
--rw-r--r--   0 runner    (1001) docker     (121)    18656 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/widgets/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/widgets/label.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/scene/widgets/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/widgets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/widgets/tests/test_colorbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     6611 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/widgets/viewbox.py
--rw-r--r--   0 runner    (1001) docker     (121)    13863 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/scene/widgets/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/testing/
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15859 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/testing/_runners.py
--rw-r--r--   0 runner    (1001) docker     (121)    12373 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/testing/_testing.py
--rw-r--r--   0 runner    (1001) docker     (121)    17414 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/testing/image_tester.py
--rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/testing/rendered_array_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/testing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/testing/tests/test_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/util/
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/bunch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/check_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)    15457 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/util/dpi/
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/dpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/dpi/_linux.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/dpi/_quartz.py
--rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/dpi/_win32.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/util/dpi/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/dpi/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/dpi/tests/test_dpi.py
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/eq.py
--rw-r--r--   0 runner    (1001) docker     (121)    29211 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/event.py
--rw-r--r--   0 runner    (1001) docker     (121)    10304 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fetching.py
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/util/fonts/
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2636 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fonts/_freetype.py
--rw-r--r--   0 runner    (1001) docker     (121)     8196 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fonts/_quartz.py
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fonts/_triage.py
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fonts/_vispy_fonts.py
--rw-r--r--   0 runner    (1001) docker     (121)     4514 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fonts/_win32.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/util/fonts/data/
--rw-r--r--   0 runner    (1001) docker     (121)   224592 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fonts/data/OpenSans-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   213292 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fonts/data/OpenSans-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   212896 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fonts/data/OpenSans-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (121)   217360 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fonts/data/OpenSans-Regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/util/fonts/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fonts/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fonts/tests/test_font.py
--rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/fourier.py
--rw-r--r--   0 runner    (1001) docker     (121)      891 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/frozen.py
--rw-r--r--   0 runner    (1001) docker     (121)     9387 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/gallery_scraper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/keys.py
--rw-r--r--   0 runner    (1001) docker     (121)    12809 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/logs.py
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/osmesa_gl.py
--rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/profiler.py
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/ptime.py
--rw-r--r--   0 runner    (1001) docker     (121)     6776 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/quaternion.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/util/svg/
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6927 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/color.py
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/element.py
--rw-r--r--   0 runner    (1001) docker     (121)    15753 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/group.py
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/length.py
--rw-r--r--   0 runner    (1001) docker     (121)      676 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/number.py
--rw-r--r--   0 runner    (1001) docker     (121)    10740 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/path.py
--rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/shapes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/style.py
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/svg.py
--rw-r--r--   0 runner    (1001) docker     (121)     6923 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/transformable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/svg/viewport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/util/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     4312 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/test_docstring_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)     7930 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/test_emitter_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    19967 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/test_event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/test_fourier.py
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/test_gallery_scraper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4715 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/test_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/tests/test_vispy.py
--rw-r--r--   0 runner    (1001) docker     (121)     5314 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)     5678 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/util/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-02-04 16:44:03.000000 vispy-0.9.5/vispy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/
--rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19375 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/_scalable_textures.py
--rw-r--r--   0 runner    (1001) docker     (121)    23572 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/axis.py
--rw-r--r--   0 runner    (1001) docker     (121)     6877 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/border.py
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/box.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/collections/
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7644 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/agg_fast_path_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     6702 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/agg_path_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/agg_point_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4710 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/agg_segment_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)    14095 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/array_list.py
--rw-r--r--   0 runner    (1001) docker     (121)    16738 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/base_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     8924 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/collection.py
--rw-r--r--   0 runner    (1001) docker     (121)      992 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/path_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/point_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/polygon_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4126 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/raw_path_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/raw_point_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/raw_polygon_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3506 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/raw_segment_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2604 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/raw_triangle_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)      797 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/segment_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/triangle_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     5223 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/collections/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    23760 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/colorbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/cube.py
--rw-r--r--   0 runner    (1001) docker     (121)     5091 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/ellipse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/filters/
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/filters/base_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/filters/clipper.py
--rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/filters/clipping_planes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5049 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/filters/color.py
--rw-r--r--   0 runner    (1001) docker     (121)    24361 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/filters/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/filters/picking.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/filters/tests/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/filters/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/filters/tests/test_wireframe_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/glsl/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/glsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/glsl/antialiasing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/glsl/color.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/graphs/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7869 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/graphs/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/graphs/layouts/
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/graphs/layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/graphs/layouts/circular.py
--rw-r--r--   0 runner    (1001) docker     (121)     7500 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/graphs/layouts/force_directed.py
--rw-r--r--   0 runner    (1001) docker     (121)     3583 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/graphs/layouts/networkx_layout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/graphs/layouts/random.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/graphs/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/graphs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5203 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/graphs/tests/test_layouts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/graphs/tests/test_networkx_layout.py
--rw-r--r--   0 runner    (1001) docker     (121)     3204 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/graphs/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     3521 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/gridlines.py
--rw-r--r--   0 runner    (1001) docker     (121)     3346 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/gridmesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     2064 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/histogram.py
--rw-r--r--   0 runner    (1001) docker     (121)    23083 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/image.py
--rw-r--r--   0 runner    (1001) docker     (121)     6006 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/infinite_line.py
--rw-r--r--   0 runner    (1001) docker     (121)     7412 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/isocurve.py
--rw-r--r--   0 runner    (1001) docker     (121)     8508 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/isoline.py
--rw-r--r--   0 runner    (1001) docker     (121)     3900 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/isosurface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/line/
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10150 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/line/arrow.py
--rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/line/dash_atlas.py
--rw-r--r--   0 runner    (1001) docker     (121)    18659 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/line/line.py
--rw-r--r--   0 runner    (1001) docker     (121)     4882 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/line_plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     6614 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/linear_region.py
--rw-r--r--   0 runner    (1001) docker     (121)    29487 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/markers.py
--rw-r--r--   0 runner    (1001) docker     (121)    11951 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     6354 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/mesh_normals.py
--rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/plane.py
--rw-r--r--   0 runner    (1001) docker     (121)     4610 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)     6664 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/rectangle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/regular_polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)     7065 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/scrolling_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/shaders/
--rw-r--r--   0 runner    (1001) docker     (121)      674 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7300 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/expression.py
--rw-r--r--   0 runner    (1001) docker     (121)    26309 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/function.py
--rw-r--r--   0 runner    (1001) docker     (121)     4416 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/multiprogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     4600 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5561 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/program.py
--rw-r--r--   0 runner    (1001) docker     (121)     5771 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/shader_object.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/shaders/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13153 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/tests/test_multiprogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/tests/test_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)     9298 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/shaders/variable.py
--rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     3091 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/sphere.py
--rw-r--r--   0 runner    (1001) docker     (121)     7279 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/surface_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_arrows.py
--rw-r--r--   0 runner    (1001) docker     (121)     4303 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_axis.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (121)     5987 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_colorbar.py
--rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_colormap.py
--rw-r--r--   0 runner    (1001) docker     (121)     4945 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_ellipse.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (121)    10753 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_infinite_line.py
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_isosurface.py
--rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_linear_region.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_markers.py
--rw-r--r--   0 runner    (1001) docker     (121)     9699 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (121)     8683 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_mesh_normals.py
--rw-r--r--   0 runner    (1001) docker     (121)     4157 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)     6658 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_rectangle.py
--rw-r--r--   0 runner    (1001) docker     (121)     4831 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_regular_polygon.py
--rw-r--r--   0 runner    (1001) docker     (121)     5121 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_scalable_textures.py
--rw-r--r--   0 runner    (1001) docker     (121)     2937 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_sdf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (121)     2532 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (121)    11194 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_volume.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tests/test_windbarb.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/text/
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3923 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/text/_sdf_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    10480 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/text/_sdf_gpu.py
--rw-r--r--   0 runner    (1001) docker     (121)    24998 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/text/text.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/transforms/
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5579 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/transforms/_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     7482 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/transforms/base_transform.py
--rw-r--r--   0 runner    (1001) docker     (121)     8899 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/transforms/chain.py
--rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/transforms/interactive.py
--rw-r--r--   0 runner    (1001) docker     (121)    15689 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/transforms/linear.py
--rw-r--r--   0 runner    (1001) docker     (121)    12538 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/transforms/nonlinear.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy/visuals/transforms/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/transforms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6871 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/transforms/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (121)    13759 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/transforms/transform_system.py
--rw-r--r--   0 runner    (1001) docker     (121)     5979 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/tube.py
--rw-r--r--   0 runner    (1001) docker     (121)    25116 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/visual.py
--rw-r--r--   0 runner    (1001) docker     (121)    41948 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/volume.py
--rw-r--r--   0 runner    (1001) docker     (121)     9306 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/windbarb.py
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-02-04 16:43:35.000000 vispy-0.9.5/vispy/visuals/xyz_axis.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6540 2022-02-04 16:44:03.000000 vispy-0.9.5/vispy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    25804 2022-02-04 16:44:04.000000 vispy-0.9.5/vispy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 16:44:03.000000 vispy-0.9.5/vispy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 16:44:03.000000 vispy-0.9.5/vispy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-02-04 16:44:03.000000 vispy-0.9.5/vispy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-04 16:44:03.000000 vispy-0.9.5/vispy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-02-04 22:13:52.000000 vispy-0.9.6/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-04 22:13:52.000000 vispy-0.9.6/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-02-04 22:13:52.000000 vispy-0.9.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:16.000000 vispy-0.9.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)    10126 2022-02-04 22:13:52.000000 vispy-0.9.6/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-02-04 22:13:52.000000 vispy-0.9.6/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-02-04 22:13:52.000000 vispy-0.9.6/.github_changelog_generator
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-02-04 22:13:52.000000 vispy-0.9.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)    29160 2022-02-04 22:13:52.000000 vispy-0.9.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)      343 2022-02-04 22:13:52.000000 vispy-0.9.6/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5491 2022-02-04 22:13:52.000000 vispy-0.9.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-02-04 22:13:52.000000 vispy-0.9.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1774 2022-02-04 22:13:52.000000 vispy-0.9.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      848 2022-02-04 22:13:52.000000 vispy-0.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6540 2022-02-04 22:14:17.000000 vispy-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5141 2022-02-04 22:13:52.000000 vispy-0.9.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      399 2022-02-04 22:13:52.000000 vispy-0.9.6/ci/build_website.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-02-04 22:13:52.000000 vispy-0.9.6/ci/requirements/linux_full_deps_apt.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      254 2022-02-04 22:13:52.000000 vispy-0.9.6/ci/requirements/linux_full_deps_conda.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-04 22:13:52.000000 vispy-0.9.6/ci/requirements/linux_full_deps_pip.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2022-02-04 22:13:52.000000 vispy-0.9.6/ci/requirements/linux_full_newqtdeps_apt.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      351 2022-02-04 22:13:52.000000 vispy-0.9.6/ci/requirements/linux_full_newqtdeps_conda.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-04 22:13:52.000000 vispy-0.9.6/ci/requirements/linux_full_newqtdeps_pip.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 22:13:52.000000 vispy-0.9.6/ci/requirements/linux_min_deps_conda.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-02-04 22:13:52.000000 vispy-0.9.6/ci/requirements/linux_osmesa_deps_conda.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-02-04 22:13:52.000000 vispy-0.9.6/ci/requirements/linux_website_deps_pip.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-04 22:13:52.000000 vispy-0.9.6/ci/requirements/py37.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-04 22:13:52.000000 vispy-0.9.6/ci/requirements/py39.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)      115 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/CNAME
+-rw-r--r--   0 runner    (1001) docker     (121)     2300 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)   154714 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/ViewFrustum.png
+-rw-r--r--   0 runner    (1001) docker     (121)    84235 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/ViewFrustum.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/doc/_static/carousel/
+-rw-r--r--   0 runner    (1001) docker     (121)   317728 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/carousel/galaxy.png
+-rw-r--r--   0 runner    (1001) docker     (121)    57799 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/carousel/high-frequency.png
+-rw-r--r--   0 runner    (1001) docker     (121)    76838 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/carousel/mandelbrot.png
+-rw-r--r--   0 runner    (1001) docker     (121)   176107 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/carousel/signals.png
+-rw-r--r--   0 runner    (1001) docker     (121)    59110 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)    10073 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/frustum-matrix.png
+-rw-r--r--   0 runner    (1001) docker     (121)    41660 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/gl-history.png
+-rw-r--r--   0 runner    (1001) docker     (121)    22485 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/gl-pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (121)    44757 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/gl-pipeline.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     9583 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/ortho-matrix.png
+-rw-r--r--   0 runner    (1001) docker     (121)     8828 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/perspective-matrix.png
+-rw-r--r--   0 runner    (1001) docker     (121)      755 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/style.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2282 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/vispy-logo-V.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2589 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/vispy-logo-V.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     7398 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/vispy-teaser-short.png
+-rw-r--r--   0 runner    (1001) docker     (121)   172644 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/vispy-teaser-short.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     8772 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/vispy-teaser.png
+-rw-r--r--   0 runner    (1001) docker     (121)   175454 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/vispy-teaser.svg
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/vispy-text-white.png
+-rw-r--r--   0 runner    (1001) docker     (121)   171862 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/_static/vispy-text-white.svg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/doc/api/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/api/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/community.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12429 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/doc/dev_guide/
+-rw-r--r--   0 runner    (1001) docker     (121)    11542 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/dev_guide/contributor_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/dev_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4716 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/dev_guide/writing_examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6954 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/faq.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/doc/gallery/
+-rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/gallery/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/doc/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (121)     3051 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/getting_started/_canvas_app.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12840 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/getting_started/gloo.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/getting_started/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    12434 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/getting_started/modern-gl.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/getting_started/plot.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/getting_started/scene.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/getting_started/visuals.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9770 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/news.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3616 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/raspberry.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4989 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/resources.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7990 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/roadmap.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-02-04 22:13:52.000000 vispy-0.9.6/doc/thirdparty.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:16.000000 vispy-0.9.6/examples/basics/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/basics/scene/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/basics/scene/modular_shaders/
+-rw-r--r--   0 runner    (1001) docker     (121)     7047 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/scene/modular_shaders/editor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14616 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/scene/modular_shaders/sandbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/scene/shared_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1839 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/scene/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/basics/visuals/
+-rw-r--r--   0 runner    (1001) docker     (121)     2434 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/arcball.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3212 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/arrows.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2757 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/arrows_quiver.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3758 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/axially_symmetric_surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2517 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2139 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/box.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4597 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/colorbar_visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2962 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/colorbar_visual_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4375 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/custom_visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4329 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/dynamic_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1797 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1457 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/grid_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4391 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/image_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/image_visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3899 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6863 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/line_draw.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1317 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/line_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/line_plot3d.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/line_plot_axes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9955 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/line_prototype.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3221 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/line_transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2326 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/markers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4601 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/networkx_layout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/plane.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3615 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/polygon_visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2008 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/rescalingmarkers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1769 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/rotating_box.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2471 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/text_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6161 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/text_visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2293 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/tube.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3395 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/visual_filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2944 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/basics/visuals/windbarb_quiver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (121)    10795 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/benchmark/scene_test_1.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6012 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/benchmark/scene_test_2.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1378 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/benchmark/simple_glut.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      834 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/benchmark/simple_vispy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/collections/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2133 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/collections/chloropleth.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1197 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/collections/path_collection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      926 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/collections/point_collection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1286 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/collections/polygon_collection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1017 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/collections/segment_collection.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2454 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/collections/tiger.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1718 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/collections/triangle_collection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:16.000000 vispy-0.9.6/examples/demo/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/demo/gloo/
+-rw-r--r--   0 runner    (1001) docker     (121)     5269 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/atom.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5748 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/boids.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4568 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/brain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2228 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/camera.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     7679 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5725 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/donut.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4036 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/fireworks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/demo/gloo/galaxy/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     6043 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/galaxy/galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7679 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/galaxy/galaxy_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13768 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/galaxy/galaxy_specrend.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5938 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5759 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/game_of_life.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5000 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/glsl_sandbox_cube.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4899 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7375 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/grayscott.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3392 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/high_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/imshow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5308 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/imshow_cuts.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/demo/gloo/jfa/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      701 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/jfa/fragment_display.glsl
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5690 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/jfa/fragment_flood.glsl
+-rwxr-xr-x   0 runner    (1001) docker     (121)      655 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/jfa/fragment_seed.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)    10260 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/jfa/jfa_translation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4685 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/jfa/jfa_vispy.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      672 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/jfa/vertex.glsl
+-rwxr-xr-x   0 runner    (1001) docker     (121)      726 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/jfa/vertex_vispy.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     5551 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/mandelbrot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8913 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/mandelbrot_double.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5961 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/molecular_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4318 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/ndscatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4233 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/offscreen.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13632 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/primitive_mesh_viewer_qt.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2368 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/quiver.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4084 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/rain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7178 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/raytracing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4575 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/realtime_signals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3780 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/signals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5418 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/skybox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4985 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/spacy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6734 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/terrain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/two_qt_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7365 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/unstructured_2d.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3309 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/gloo/voronoi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/demo/plot/
+-rw-r--r--   0 runner    (1001) docker     (121)      789 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/plot/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/demo/scene/
+-rw-r--r--   0 runner    (1001) docker     (121)     6673 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/scene/flow_lines.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3285 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/scene/force_directed_graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/scene/klein.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10222 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/scene/oscilloscope.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2977 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/scene/picking.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/scene/scrolling_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/demo/visuals/
+-rw-r--r--   0 runner    (1001) docker     (121)    34342 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/demo/visuals/wiggly_bar.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/gloo/
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3038 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/animate_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4279 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/animate_images_slice.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3072 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/animate_shape.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/colored_quad.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3843 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/display_lines.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2519 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/display_points.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1325 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/display_shape.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2111 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/geometry_shader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3304 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/gpuimage.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3449 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/hello_fbo.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2164 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/multi_texture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4873 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5317 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/rotate_cube.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2226 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/rotating_quad.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3354 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/spatial_filters.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      395 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/start.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/gloo/start_shaders.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (121)     3614 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/jupyter/Rotating Cube.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     3851 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/jupyter/colormaps.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     7023 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/jupyter/gloo_display_lines.ipynb
+-rw-r--r--   0 runner    (1001) docker     (121)     9521 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/jupyter/gloo_molecular_viewer.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/offscreen/
+-rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/offscreen/simple_egl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/offscreen/simple_osmesa.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/plotting/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/plotting/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/plotting/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/plotting/export.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      592 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/plotting/ipython_fig_playground.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/plotting/plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/plotting/plot_colorbars.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1127 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/plotting/scatter_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/plotting/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1335 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/plotting/volume_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/scene/
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/axes_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)      948 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/background_borders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2693 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/clipping_planes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/colorbar_widget.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/colored_line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/console.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2390 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/contour.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7041 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/example..gif
+-rw-r--r--   0 runner    (1001) docker     (121)     2778 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/example.png
+-rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/flipped_axis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/scene/grid_layout/
+-rw-r--r--   0 runner    (1001) docker     (121)       97 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/grid_layout/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/grid_layout/grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/grid_layout/grid_basic.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/grid_layout/grid_holed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/grid_layout/grid_large.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1005 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/grid_layout/grid_uneven_col.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/grid_layout/grid_x_y_viewbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1883 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/infinite_line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1756 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/isocurve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/isocurve_for_trisurface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4613 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/isocurve_for_trisurface_qt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4549 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/isocurve_updates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1859 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/isosurface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1568 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/line_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2432 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/linear_region.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3377 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/magnify.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/marker_spheres.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/mesh_normals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3824 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/mesh_shading.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/mesh_texture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4539 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/nested_viewbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1712 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/one_cam_two_scenes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/one_scene_four_cams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/point_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1717 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/save_animation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1396 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13158 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/shape_draw.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1365 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/surface_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1739 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/text.py
+-rw-r--r--   0 runner    (1001) docker     (121)      978 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/turntable_box.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/viewbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4994 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/volume.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4293 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/scene/volume_plane.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:16.000000 vispy-0.9.6/examples/tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/tutorial/app/
+-rw-r--r--   0 runner    (1001) docker     (121)     1846 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/app/app_events.py
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/app/fps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2905 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/app/shared_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/app/simple.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/app/simple_wx.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/tutorial/gl/
+-rw-r--r--   0 runner    (1001) docker     (121)     8364 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/gl/cube.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5538 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/gl/fireworks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3639 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/gl/quad.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/tutorial/gloo/
+-rw-r--r--   0 runner    (1001) docker     (121)     2641 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/gloo/colored_cube.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5020 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/gloo/lighted_cube.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3457 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/gloo/outlined_cube.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4053 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/gloo/texture_precision.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/gloo/textured_cube.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/gloo/textured_quad.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/examples/tutorial/visuals/
+-rw-r--r--   0 runner    (1001) docker     (121)     6494 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/visuals/T01_basic_visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8240 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/visuals/T02_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8118 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/visuals/T03_antialiasing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2438 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/visuals/T04_fragment_programs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3008 2022-02-04 22:13:52.000000 vispy-0.9.6/examples/tutorial/visuals/T05_viewer_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-02-04 22:13:52.000000 vispy-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-02-04 22:13:52.000000 vispy-0.9.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      296 2022-02-04 22:14:17.000000 vispy-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     5062 2022-02-04 22:13:52.000000 vispy-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/app/
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/_default_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6474 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/_detect_eventloop.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10631 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/application.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/app/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)     1837 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8478 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_egl.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17018 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_glfw.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8805 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_jupyter_rfb.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3697 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_offscreen_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7602 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_osmesa.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14963 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_pyglet.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_pyqt4.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_pyqt5.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1422 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_pyqt6.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_pyside.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_pyside2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_pyside6.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34845 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_qt.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15100 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_sdl2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7953 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)      251 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26111 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_tk.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14864 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/_wx.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/app/backends/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1234 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/tests/test_offscreen_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2313 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/backends/tests/test_rfb.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10799 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28638 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3411 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/qt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/app/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/tests/qt-designer.ui
+-rw-r--r--   0 runner    (1001) docker     (121)    15781 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6394 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/tests/test_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3579 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1285 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4527 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/tests/test_simultaneous.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5754 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/app/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/color/
+-rw-r--r--   0 runner    (1001) docker     (121)      644 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5224 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/color/_color_dict.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14194 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/color/color_array.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6051 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/color/color_space.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43616 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/color/colormap.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/color/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/color/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12919 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/color/tests/test_color.py
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/ext/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54240 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/ext/cocoapy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5340 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/ext/cubehelix.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12160 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/ext/egl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4236 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/ext/fontconfig.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6617 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/ext/gdi32plus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3411 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/ext/osmesa.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/geometry/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5130 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/_triangulation_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4245 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13145 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/curves.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20941 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/generation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5796 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/isocurve.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20651 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/isosurface.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25329 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/meshdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/normals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/parametric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5481 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/rect.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/geometry/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1038 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/tests/test_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2110 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/tests/test_generation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/tests/test_meshdata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12700 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/tests/test_triangulation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4262 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/torusknot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31968 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/geometry/triangulation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/gloo/
+-rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16454 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8640 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9350 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/framebuffer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/gloo/gl/
+-rw-r--r--   0 runner    (1001) docker     (121)     7952 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16615 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    38247 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/_es2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    54470 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/_gl2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14644 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11646 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/_pyopengl2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      737 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/es2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3144 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/gl2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9274 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/glplus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2667 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/pyopengl2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/gloo/gl/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9223 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17340 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/tests/test_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11101 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/tests/test_names.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/gl/tests/test_use.py
+-rw-r--r--   0 runner    (1001) docker     (121)    65293 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/glir.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3912 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/globject.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2291 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21335 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/program.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/gloo/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19819 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/tests/test_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5482 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/tests/test_framebuffer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9644 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/tests/test_glir.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/tests/test_globject.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11414 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/tests/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23993 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/tests/test_texture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6495 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/tests/test_use_gloo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1913 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8689 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/tests/test_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37450 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/texture.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26390 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/gloo/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/glsl/
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/glsl/antialias/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/antialias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      368 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/antialias/antialias.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      970 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/antialias/cap-butt.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/antialias/cap-round.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      970 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/antialias/cap-square.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/antialias/cap-triangle-in.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/antialias/cap-triangle-out.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/antialias/cap.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/antialias/caps.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1247 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/antialias/filled.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/antialias/outline.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/antialias/stroke.glsl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/glsl/arrowheads/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrowheads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2674 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrowheads/angle.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrowheads/arrowheads.frag
+-rw-r--r--   0 runner    (1001) docker     (121)      477 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrowheads/arrowheads.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrowheads/arrowheads.vert
+-rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrowheads/curved.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      665 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrowheads/inhibitor.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrowheads/stealth.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     2481 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrowheads/triangle.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrowheads/util.glsl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/glsl/arrows/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/angle-30.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/angle-60.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      510 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/angle-90.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1448 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/arrow.frag
+-rw-r--r--   0 runner    (1001) docker     (121)     1400 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/arrow.vert
+-rw-r--r--   0 runner    (1001) docker     (121)      562 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/arrows.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     6397 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/common.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/curved.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1762 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/stealth.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/triangle-30.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/triangle-60.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      522 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/triangle-90.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/arrows/util.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)    20717 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/build_spatial_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/glsl/collections/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/agg-fast-path.frag
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/agg-fast-path.vert
+-rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/agg-glyph.frag
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/agg-glyph.vert
+-rw-r--r--   0 runner    (1001) docker     (121)     1406 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/agg-marker.frag
+-rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/agg-marker.vert
+-rw-r--r--   0 runner    (1001) docker     (121)     1846 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/agg-path.frag
+-rw-r--r--   0 runner    (1001) docker     (121)     4987 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/agg-path.vert
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/agg-point.frag
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/agg-point.vert
+-rw-r--r--   0 runner    (1001) docker     (121)     1083 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/agg-segment.frag
+-rw-r--r--   0 runner    (1001) docker     (121)     2075 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/agg-segment.vert
+-rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/marker.frag
+-rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/marker.vert
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/raw-path.frag
+-rw-r--r--   0 runner    (1001) docker     (121)      682 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/raw-path.vert
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/raw-point.frag
+-rw-r--r--   0 runner    (1001) docker     (121)      735 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/raw-point.vert
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/raw-segment.frag
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/raw-segment.vert
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/raw-triangle.frag
+-rw-r--r--   0 runner    (1001) docker     (121)      658 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/raw-triangle.vert
+-rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/sdf-glyph-ticks.vert
+-rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/sdf-glyph.frag
+-rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/sdf-glyph.vert
+-rw-r--r--   0 runner    (1001) docker     (121)     2344 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/collections/tick-labels.vert
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/glsl/colormaps/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/autumn.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/blues.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      553 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/color-space.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      781 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/colormaps.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      641 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/cool.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      688 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/fire.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/gray.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      639 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/greens.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      721 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/hot.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/ice.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      798 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/icefire.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/parse.py
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/reds.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/spring.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/summer.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      652 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/user.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      998 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/util.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/wheel.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/colormaps/winter.glsl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/glsl/lines/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/lines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9887 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/lines/agg.frag
+-rw-r--r--   0 runner    (1001) docker     (121)     7620 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/lines/agg.vert
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/glsl/markers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      518 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/arrow.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      695 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/asterisk.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      601 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/chevron.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      767 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/clover.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1144 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/club.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/cross.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/diamond.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/disc.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/ellipse.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/hbar.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      648 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/heart.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/infinity.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     2936 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/marker-sdf.frag
+-rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/marker-sdf.vert
+-rw-r--r--   0 runner    (1001) docker     (121)     1438 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/marker.frag
+-rw-r--r--   0 runner    (1001) docker     (121)     1330 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/marker.vert
+-rw-r--r--   0 runner    (1001) docker     (121)      849 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/markers.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/pin.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/ring.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/spade.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/square.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/tag.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/triangle.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/markers/vbar.glsl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/glsl/math/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      945 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/math/circle-through-2-points.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/math/constants.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     3045 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/math/double.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      678 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/math/functions.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/math/point-to-line-distance.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/math/point-to-line-projection.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      812 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/math/signed-line-distance.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      924 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/math/signed-segment-distance.glsl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/glsl/misc/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6828 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/misc/regular-grid.frag
+-rw-r--r--   0 runner    (1001) docker     (121)    15813 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/misc/spatial-filters.frag
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/misc/viewport-NDC.glsl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/glsl/transforms/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/azimuthal-equal-area.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/azimuthal-equidistant.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1627 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/hammer.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/identity.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/identity_forward.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      643 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/identity_inverse.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     3394 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/linear-scale.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/log-scale.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/mercator-transverse-forward.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1156 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/mercator-transverse-inverse.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/panzoom.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/polar.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/position.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     3916 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/power-scale.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      120 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/projection.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      411 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/pvm.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/rotate.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/trackball.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/translate.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/transverse_mercator.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/viewport-clipping.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/viewport-transform.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)     1806 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/viewport.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/x.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/y.glsl
+-rw-r--r--   0 runner    (1001) docker     (121)      360 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/glsl/transforms/z.glsl
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/io/
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/io/_data/
+-rw-r--r--   0 runner    (1001) docker     (121)    65616 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/io/_data/spatial-filters.npy
+-rw-r--r--   0 runner    (1001) docker     (121)     2489 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/io/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6180 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3559 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/io/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5942 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/io/stl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1557 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/io/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4223 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/io/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12285 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/io/wavefront.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/plot/
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1733 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/plot/fig.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18595 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/plot/plotwidget.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/plot/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/plot/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/plot/tests/test_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/scene/
+-rw-r--r--   0 runner    (1001) docker     (121)     1487 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/scene/cameras/
+-rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/cameras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/cameras/_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3606 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/cameras/arcball.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18614 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/cameras/base_camera.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16343 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/cameras/fly.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5387 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/cameras/magnify.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10917 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/cameras/panzoom.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11617 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/cameras/perspective.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/scene/cameras/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/cameras/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1612 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/cameras/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3220 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/cameras/tests/test_perspective.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5351 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/cameras/turntable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22619 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2185 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19029 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/node.py
+-rw-r--r--   0 runner    (1001) docker     (121)      564 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/subscene.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/scene/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3292 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/tests/test_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4936 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/tests/test_visuals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9741 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/visuals.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/scene/widgets/
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/widgets/anchor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2954 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/widgets/axis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6158 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/widgets/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14013 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/widgets/console.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18656 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/widgets/grid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/widgets/label.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/scene/widgets/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/widgets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/widgets/tests/test_colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6611 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/widgets/viewbox.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13863 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/scene/widgets/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/testing/
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15859 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/testing/_runners.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12373 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/testing/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17414 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/testing/image_tester.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/testing/rendered_array_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/testing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/testing/tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/util/
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/bunch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/check_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15457 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/util/dpi/
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/dpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2038 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/dpi/_linux.py
+-rw-r--r--   0 runner    (1001) docker     (121)      829 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/dpi/_quartz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1126 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/dpi/_win32.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/util/dpi/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/dpi/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/dpi/tests/test_dpi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/eq.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29211 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/event.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10304 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fetching.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/util/fonts/
+-rw-r--r--   0 runner    (1001) docker     (121)      570 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2636 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fonts/_freetype.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8196 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fonts/_quartz.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fonts/_triage.py
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fonts/_vispy_fonts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4514 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fonts/_win32.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/util/fonts/data/
+-rw-r--r--   0 runner    (1001) docker     (121)   224592 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fonts/data/OpenSans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   213292 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fonts/data/OpenSans-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   212896 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fonts/data/OpenSans-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (121)   217360 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fonts/data/OpenSans-Regular.ttf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/util/fonts/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fonts/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1405 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fonts/tests/test_font.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1967 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/fourier.py
+-rw-r--r--   0 runner    (1001) docker     (121)      891 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/frozen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9387 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/gallery_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/keys.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12809 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/logs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      597 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/osmesa_gl.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      493 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/ptime.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6776 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/quaternion.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/util/svg/
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      800 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6927 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/color.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1412 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/element.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15753 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/length.py
+-rw-r--r--   0 runner    (1001) docker     (121)      676 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/number.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10740 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/path.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1194 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/style.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/svg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6923 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/transformable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/svg/viewport.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/util/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2194 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4312 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/test_docstring_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7930 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/test_emitter_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19967 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/test_event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/test_fourier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/test_gallery_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4715 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/test_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/tests/test_vispy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5314 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5678 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/util/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-02-04 22:14:16.000000 vispy-0.9.6/vispy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/
+-rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19375 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/_scalable_textures.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23572 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/axis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6877 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/border.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/box.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/collections/
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7644 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/agg_fast_path_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6702 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/agg_path_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1714 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/agg_point_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4710 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/agg_segment_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14095 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/array_list.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16738 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/base_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8924 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)      992 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/path_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)      740 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/point_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/polygon_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4126 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/raw_path_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/raw_point_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/raw_polygon_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3506 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/raw_segment_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2604 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/raw_triangle_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)      797 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/segment_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)      625 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/triangle_collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5223 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/collections/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23760 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1723 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/cube.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5091 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/ellipse.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/filters/
+-rw-r--r--   0 runner    (1001) docker     (121)      430 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3477 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/filters/base_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1741 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/filters/clipper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3897 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/filters/clipping_planes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5049 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/filters/color.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24361 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/filters/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/filters/picking.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/filters/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)      160 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/filters/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/filters/tests/test_wireframe_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/glsl/
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/glsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3195 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/glsl/antialiasing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/glsl/color.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/graphs/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7869 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/graphs/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/graphs/layouts/
+-rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/graphs/layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1559 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/graphs/layouts/circular.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7500 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/graphs/layouts/force_directed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3583 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/graphs/layouts/networkx_layout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1674 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/graphs/layouts/random.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/graphs/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/graphs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5203 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/graphs/tests/test_layouts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/graphs/tests/test_networkx_layout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3204 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/graphs/util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3521 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/gridlines.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3346 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/gridmesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2064 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23083 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6006 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/infinite_line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7412 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/isocurve.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8508 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/isoline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3900 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/isosurface.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/line/
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10150 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/line/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2952 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/line/dash_atlas.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18659 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/line/line.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4882 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/line_plot.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6614 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/linear_region.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29487 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/markers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11951 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6354 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/mesh_normals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2203 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/plane.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4610 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6664 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/regular_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7065 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/scrolling_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/shaders/
+-rw-r--r--   0 runner    (1001) docker     (121)      674 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7300 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2775 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/expression.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26309 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/function.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4416 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/multiprogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4600 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5561 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/program.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5771 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/shader_object.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/shaders/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13153 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2234 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/tests/test_multiprogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1472 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9298 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/shaders/variable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4940 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3091 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7279 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/surface_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3562 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_arrows.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4303 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_axis.py
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5987 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_colorbar.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_colormap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4945 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_ellipse.py
+-rw-r--r--   0 runner    (1001) docker     (121)      814 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10753 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1936 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_infinite_line.py
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_isosurface.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_linear_region.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_markers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9699 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8683 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_mesh_normals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4157 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6658 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_rectangle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4831 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_regular_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5121 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_scalable_textures.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2937 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_sdf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2532 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11194 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_volume.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tests/test_windbarb.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/text/
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3923 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/text/_sdf_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)    10480 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/text/_sdf_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24998 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/text/text.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/transforms/
+-rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5579 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/transforms/_util.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7482 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/transforms/base_transform.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8899 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/transforms/chain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/transforms/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15689 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/transforms/linear.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12538 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/transforms/nonlinear.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy/visuals/transforms/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/transforms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6871 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/transforms/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13759 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/transforms/transform_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5979 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/tube.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25116 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/visual.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41948 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/volume.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9306 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/windbarb.py
+-rw-r--r--   0 runner    (1001) docker     (121)      957 2022-02-04 22:13:52.000000 vispy-0.9.6/vispy/visuals/xyz_axis.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 22:14:17.000000 vispy-0.9.6/vispy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6540 2022-02-04 22:14:16.000000 vispy-0.9.6/vispy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    25804 2022-02-04 22:14:16.000000 vispy-0.9.6/vispy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 22:14:16.000000 vispy-0.9.6/vispy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 22:14:16.000000 vispy-0.9.6/vispy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2022-02-04 22:14:16.000000 vispy-0.9.6/vispy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-02-04 22:14:16.000000 vispy-0.9.6/vispy.egg-info/top_level.txt
```

### Comparing `vispy-0.9.5/.github/workflows/main.yml` & `vispy-0.9.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/.github/workflows/wheels.yml` & `vispy-0.9.6/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/CHANGELOG.md` & `vispy-0.9.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/CODE_OF_CONDUCT.md` & `vispy-0.9.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/LICENSE.txt` & `vispy-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/MANIFEST.in` & `vispy-0.9.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/PKG-INFO` & `vispy-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vispy
-Version: 0.9.5
+Version: 0.9.6
 Summary: Interactive visualization in Python
 Home-page: http://vispy.org
 Download-URL: https://pypi.python.org/pypi/vispy
 Author: Vispy contributors
 Author-email: vispy@googlegroups.com
 License: (new) BSD
 Keywords: visualization,OpenGl,ES,medical,imaging,3D,plotting,numpy,bigdata,ipython,jupyter,widgets
```

### Comparing `vispy-0.9.5/README.rst` & `vispy-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/Makefile` & `vispy-0.9.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/ViewFrustum.png` & `vispy-0.9.6/doc/_static/ViewFrustum.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/ViewFrustum.svg` & `vispy-0.9.6/doc/_static/ViewFrustum.svg`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/carousel/galaxy.png` & `vispy-0.9.6/doc/_static/carousel/galaxy.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/carousel/high-frequency.png` & `vispy-0.9.6/doc/_static/carousel/high-frequency.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/carousel/mandelbrot.png` & `vispy-0.9.6/doc/_static/carousel/mandelbrot.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/carousel/signals.png` & `vispy-0.9.6/doc/_static/carousel/signals.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/favicon.ico` & `vispy-0.9.6/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/frustum-matrix.png` & `vispy-0.9.6/doc/_static/frustum-matrix.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/gl-history.png` & `vispy-0.9.6/doc/_static/gl-history.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/gl-pipeline.png` & `vispy-0.9.6/doc/_static/gl-pipeline.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/gl-pipeline.svg` & `vispy-0.9.6/doc/_static/gl-pipeline.svg`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/ortho-matrix.png` & `vispy-0.9.6/doc/_static/ortho-matrix.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/perspective-matrix.png` & `vispy-0.9.6/doc/_static/perspective-matrix.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/style.css` & `vispy-0.9.6/doc/_static/style.css`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/vispy-logo-V.png` & `vispy-0.9.6/doc/_static/vispy-logo-V.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/vispy-logo-V.svg` & `vispy-0.9.6/doc/_static/vispy-logo-V.svg`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/vispy-teaser-short.png` & `vispy-0.9.6/doc/_static/vispy-teaser-short.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/vispy-teaser-short.svg` & `vispy-0.9.6/doc/_static/vispy-teaser-short.svg`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/vispy-teaser.png` & `vispy-0.9.6/doc/_static/vispy-teaser.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/vispy-teaser.svg` & `vispy-0.9.6/doc/_static/vispy-teaser.svg`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/vispy-text-white.png` & `vispy-0.9.6/doc/_static/vispy-text-white.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/_static/vispy-text-white.svg` & `vispy-0.9.6/doc/_static/vispy-text-white.svg`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/community.rst` & `vispy-0.9.6/doc/community.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/conf.py` & `vispy-0.9.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/dev_guide/contributor_guide.rst` & `vispy-0.9.6/doc/dev_guide/contributor_guide.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/dev_guide/writing_examples.rst` & `vispy-0.9.6/doc/dev_guide/writing_examples.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/faq.rst` & `vispy-0.9.6/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/gallery/index.rst` & `vispy-0.9.6/doc/gallery/index.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/getting_started/_canvas_app.rst` & `vispy-0.9.6/doc/getting_started/_canvas_app.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/getting_started/gloo.rst` & `vispy-0.9.6/doc/getting_started/gloo.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/getting_started/index.rst` & `vispy-0.9.6/doc/getting_started/index.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/getting_started/modern-gl.rst` & `vispy-0.9.6/doc/getting_started/modern-gl.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/index.rst` & `vispy-0.9.6/doc/index.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/installation.rst` & `vispy-0.9.6/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/news.rst` & `vispy-0.9.6/doc/news.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/overview.rst` & `vispy-0.9.6/doc/overview.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/raspberry.rst` & `vispy-0.9.6/doc/raspberry.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/resources.rst` & `vispy-0.9.6/doc/resources.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/roadmap.rst` & `vispy-0.9.6/doc/roadmap.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/doc/thirdparty.rst` & `vispy-0.9.6/doc/thirdparty.rst`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/scene/modular_shaders/editor.py` & `vispy-0.9.6/examples/basics/scene/modular_shaders/editor.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/scene/modular_shaders/sandbox.py` & `vispy-0.9.6/examples/basics/scene/modular_shaders/sandbox.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/scene/shared_context.py` & `vispy-0.9.6/examples/basics/scene/shared_context.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/scene/stereo.py` & `vispy-0.9.6/examples/basics/scene/stereo.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/arcball.py` & `vispy-0.9.6/examples/basics/visuals/arcball.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/arrows.py` & `vispy-0.9.6/examples/basics/visuals/arrows.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/arrows_quiver.py` & `vispy-0.9.6/examples/basics/visuals/arrows_quiver.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/axially_symmetric_surfaces.py` & `vispy-0.9.6/examples/basics/visuals/axially_symmetric_surfaces.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/bezier.py` & `vispy-0.9.6/examples/basics/visuals/bezier.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/box.py` & `vispy-0.9.6/examples/basics/visuals/box.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/colorbar_visual.py` & `vispy-0.9.6/examples/basics/visuals/colorbar_visual.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/colorbar_visual_types.py` & `vispy-0.9.6/examples/basics/visuals/colorbar_visual_types.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/custom_visual.py` & `vispy-0.9.6/examples/basics/visuals/custom_visual.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/dynamic_polygon.py` & `vispy-0.9.6/examples/basics/visuals/dynamic_polygon.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/graph.py` & `vispy-0.9.6/examples/basics/visuals/graph.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/grid_mesh.py` & `vispy-0.9.6/examples/basics/visuals/grid_mesh.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/image_transforms.py` & `vispy-0.9.6/examples/basics/visuals/image_transforms.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/image_visual.py` & `vispy-0.9.6/examples/basics/visuals/image_visual.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/line.py` & `vispy-0.9.6/examples/basics/visuals/line.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/line_draw.py` & `vispy-0.9.6/examples/basics/visuals/line_draw.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/line_plot.py` & `vispy-0.9.6/examples/basics/visuals/line_plot.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/line_plot3d.py` & `vispy-0.9.6/examples/basics/visuals/line_plot3d.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/line_plot_axes.py` & `vispy-0.9.6/examples/basics/visuals/line_plot_axes.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/line_prototype.py` & `vispy-0.9.6/examples/basics/visuals/line_prototype.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/line_transform.py` & `vispy-0.9.6/examples/basics/visuals/line_transform.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/markers.py` & `vispy-0.9.6/examples/basics/visuals/markers.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/mesh.py` & `vispy-0.9.6/examples/basics/visuals/mesh.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/networkx_layout.py` & `vispy-0.9.6/examples/basics/visuals/networkx_layout.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/plane.py` & `vispy-0.9.6/examples/basics/visuals/plane.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/polygon_visual.py` & `vispy-0.9.6/examples/basics/visuals/polygon_visual.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/rescalingmarkers.py` & `vispy-0.9.6/examples/basics/visuals/rescalingmarkers.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/rotating_box.py` & `vispy-0.9.6/examples/basics/visuals/rotating_box.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/text_scatter.py` & `vispy-0.9.6/examples/basics/visuals/text_scatter.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/text_visual.py` & `vispy-0.9.6/examples/basics/visuals/text_visual.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/tube.py` & `vispy-0.9.6/examples/basics/visuals/tube.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/visual_filters.py` & `vispy-0.9.6/examples/basics/visuals/visual_filters.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/basics/visuals/windbarb_quiver.py` & `vispy-0.9.6/examples/basics/visuals/windbarb_quiver.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/benchmark/scene_test_1.py` & `vispy-0.9.6/examples/benchmark/scene_test_1.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/benchmark/scene_test_2.py` & `vispy-0.9.6/examples/benchmark/scene_test_2.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/benchmark/simple_glut.py` & `vispy-0.9.6/examples/benchmark/simple_glut.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/benchmark/simple_vispy.py` & `vispy-0.9.6/examples/benchmark/simple_vispy.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/collections/chloropleth.py` & `vispy-0.9.6/examples/collections/chloropleth.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/collections/path_collection.py` & `vispy-0.9.6/examples/collections/path_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/collections/point_collection.py` & `vispy-0.9.6/examples/collections/point_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/collections/polygon_collection.py` & `vispy-0.9.6/examples/collections/polygon_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/collections/segment_collection.py` & `vispy-0.9.6/examples/collections/segment_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/collections/tiger.py` & `vispy-0.9.6/examples/collections/tiger.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/collections/triangle_collection.py` & `vispy-0.9.6/examples/collections/triangle_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/atom.py` & `vispy-0.9.6/examples/demo/gloo/atom.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/boids.py` & `vispy-0.9.6/examples/demo/gloo/boids.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/brain.py` & `vispy-0.9.6/examples/demo/gloo/brain.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/camera.py` & `vispy-0.9.6/examples/demo/gloo/camera.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/cloud.py` & `vispy-0.9.6/examples/demo/gloo/cloud.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/donut.py` & `vispy-0.9.6/examples/demo/gloo/donut.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/fireworks.py` & `vispy-0.9.6/examples/demo/gloo/fireworks.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/galaxy/galaxy.py` & `vispy-0.9.6/examples/demo/gloo/galaxy/galaxy.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/galaxy/galaxy_simulation.py` & `vispy-0.9.6/examples/demo/gloo/galaxy/galaxy_simulation.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/galaxy/galaxy_specrend.py` & `vispy-0.9.6/examples/demo/gloo/galaxy/galaxy_specrend.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/galaxy.py` & `vispy-0.9.6/examples/demo/gloo/galaxy.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/game_of_life.py` & `vispy-0.9.6/examples/demo/gloo/game_of_life.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/glsl_sandbox_cube.py` & `vispy-0.9.6/examples/demo/gloo/glsl_sandbox_cube.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/graph.py` & `vispy-0.9.6/examples/demo/gloo/graph.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/grayscott.py` & `vispy-0.9.6/examples/demo/gloo/grayscott.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/high_frequency.py` & `vispy-0.9.6/examples/demo/gloo/high_frequency.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/imshow.py` & `vispy-0.9.6/examples/demo/gloo/imshow.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/imshow_cuts.py` & `vispy-0.9.6/examples/demo/gloo/imshow_cuts.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/jfa/fragment_display.glsl` & `vispy-0.9.6/examples/demo/gloo/jfa/fragment_display.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/jfa/fragment_flood.glsl` & `vispy-0.9.6/examples/demo/gloo/jfa/fragment_flood.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/jfa/fragment_seed.glsl` & `vispy-0.9.6/examples/demo/gloo/jfa/fragment_seed.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/jfa/jfa_translation.py` & `vispy-0.9.6/examples/demo/gloo/jfa/jfa_translation.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/jfa/jfa_vispy.py` & `vispy-0.9.6/examples/demo/gloo/jfa/jfa_vispy.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/jfa/vertex.glsl` & `vispy-0.9.6/examples/demo/gloo/jfa/vertex.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/jfa/vertex_vispy.glsl` & `vispy-0.9.6/examples/demo/gloo/jfa/vertex_vispy.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/mandelbrot.py` & `vispy-0.9.6/examples/demo/gloo/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/mandelbrot_double.py` & `vispy-0.9.6/examples/demo/gloo/mandelbrot_double.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/molecular_viewer.py` & `vispy-0.9.6/examples/demo/gloo/molecular_viewer.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/ndscatter.py` & `vispy-0.9.6/examples/demo/gloo/ndscatter.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/offscreen.py` & `vispy-0.9.6/examples/demo/gloo/offscreen.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/primitive_mesh_viewer_qt.py` & `vispy-0.9.6/examples/demo/gloo/primitive_mesh_viewer_qt.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/quiver.py` & `vispy-0.9.6/examples/demo/gloo/quiver.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/rain.py` & `vispy-0.9.6/examples/demo/gloo/rain.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/raytracing.py` & `vispy-0.9.6/examples/demo/gloo/raytracing.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/realtime_signals.py` & `vispy-0.9.6/examples/demo/gloo/realtime_signals.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/signals.py` & `vispy-0.9.6/examples/demo/gloo/signals.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/skybox.py` & `vispy-0.9.6/examples/demo/gloo/skybox.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/spacy.py` & `vispy-0.9.6/examples/demo/gloo/spacy.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/terrain.py` & `vispy-0.9.6/examples/demo/gloo/terrain.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/two_qt_widgets.py` & `vispy-0.9.6/examples/demo/gloo/two_qt_widgets.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/unstructured_2d.py` & `vispy-0.9.6/examples/demo/gloo/unstructured_2d.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/gloo/voronoi.py` & `vispy-0.9.6/examples/demo/gloo/voronoi.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/plot/plot.py` & `vispy-0.9.6/examples/demo/plot/plot.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/scene/flow_lines.py` & `vispy-0.9.6/examples/demo/scene/flow_lines.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/scene/force_directed_graph.py` & `vispy-0.9.6/examples/demo/scene/force_directed_graph.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/scene/klein.py` & `vispy-0.9.6/examples/demo/scene/klein.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/scene/oscilloscope.py` & `vispy-0.9.6/examples/demo/scene/oscilloscope.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/scene/picking.py` & `vispy-0.9.6/examples/demo/scene/picking.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/scene/scrolling_plots.py` & `vispy-0.9.6/examples/demo/scene/scrolling_plots.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/demo/visuals/wiggly_bar.py` & `vispy-0.9.6/examples/demo/visuals/wiggly_bar.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/animate_images.py` & `vispy-0.9.6/examples/gloo/animate_images.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/animate_images_slice.py` & `vispy-0.9.6/examples/gloo/animate_images_slice.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/animate_shape.py` & `vispy-0.9.6/examples/gloo/animate_shape.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/colored_quad.py` & `vispy-0.9.6/examples/gloo/colored_quad.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/display_lines.py` & `vispy-0.9.6/examples/gloo/display_lines.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/display_points.py` & `vispy-0.9.6/examples/gloo/display_points.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/display_shape.py` & `vispy-0.9.6/examples/gloo/display_shape.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/geometry_shader.py` & `vispy-0.9.6/examples/gloo/geometry_shader.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/gpuimage.py` & `vispy-0.9.6/examples/gloo/gpuimage.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/hello_fbo.py` & `vispy-0.9.6/examples/gloo/hello_fbo.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/multi_texture.py` & `vispy-0.9.6/examples/gloo/multi_texture.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/post_processing.py` & `vispy-0.9.6/examples/gloo/post_processing.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/rotate_cube.py` & `vispy-0.9.6/examples/gloo/rotate_cube.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/rotating_quad.py` & `vispy-0.9.6/examples/gloo/rotating_quad.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/spatial_filters.py` & `vispy-0.9.6/examples/gloo/spatial_filters.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/gloo/start_shaders.py` & `vispy-0.9.6/examples/gloo/start_shaders.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/jupyter/Rotating Cube.ipynb` & `vispy-0.9.6/examples/jupyter/Rotating Cube.ipynb`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/jupyter/colormaps.ipynb` & `vispy-0.9.6/examples/jupyter/colormaps.ipynb`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/jupyter/gloo_display_lines.ipynb` & `vispy-0.9.6/examples/jupyter/gloo_display_lines.ipynb`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/jupyter/gloo_molecular_viewer.ipynb` & `vispy-0.9.6/examples/jupyter/gloo_molecular_viewer.ipynb`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/offscreen/simple_egl.py` & `vispy-0.9.6/examples/offscreen/simple_egl.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/offscreen/simple_osmesa.py` & `vispy-0.9.6/examples/offscreen/simple_osmesa.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/plotting/colorbar.py` & `vispy-0.9.6/examples/plotting/colorbar.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/plotting/export.py` & `vispy-0.9.6/examples/plotting/export.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/plotting/ipython_fig_playground.py` & `vispy-0.9.6/examples/plotting/ipython_fig_playground.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/plotting/plot.py` & `vispy-0.9.6/examples/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/plotting/plot_colorbars.py` & `vispy-0.9.6/examples/plotting/plot_colorbars.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/plotting/scatter_histogram.py` & `vispy-0.9.6/examples/plotting/scatter_histogram.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/plotting/spectrogram.py` & `vispy-0.9.6/examples/plotting/spectrogram.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/plotting/volume_plot.py` & `vispy-0.9.6/examples/plotting/volume_plot.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/axes_plot.py` & `vispy-0.9.6/examples/scene/axes_plot.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/background_borders.py` & `vispy-0.9.6/examples/scene/background_borders.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/clipping_planes.py` & `vispy-0.9.6/examples/scene/clipping_planes.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/colorbar_widget.py` & `vispy-0.9.6/examples/scene/colorbar_widget.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/colored_line.py` & `vispy-0.9.6/examples/scene/colored_line.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/console.py` & `vispy-0.9.6/examples/scene/console.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/contour.py` & `vispy-0.9.6/examples/scene/contour.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/example..gif` & `vispy-0.9.6/examples/scene/example..gif`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/example.png` & `vispy-0.9.6/examples/scene/example.png`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/flipped_axis.py` & `vispy-0.9.6/examples/scene/flipped_axis.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/graph.py` & `vispy-0.9.6/examples/scene/graph.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/grid_layout/grid.py` & `vispy-0.9.6/examples/scene/grid_layout/grid.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/grid_layout/grid_basic.py` & `vispy-0.9.6/examples/scene/grid_layout/grid_basic.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/grid_layout/grid_holed.py` & `vispy-0.9.6/examples/scene/grid_layout/grid_holed.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/grid_layout/grid_large.py` & `vispy-0.9.6/examples/scene/grid_layout/grid_large.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/grid_layout/grid_uneven_col.py` & `vispy-0.9.6/examples/scene/grid_layout/grid_uneven_col.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/grid_layout/grid_x_y_viewbox.py` & `vispy-0.9.6/examples/scene/grid_layout/grid_x_y_viewbox.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/image.py` & `vispy-0.9.6/examples/scene/image.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/infinite_line.py` & `vispy-0.9.6/examples/scene/infinite_line.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/isocurve.py` & `vispy-0.9.6/examples/scene/isocurve.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/isocurve_for_trisurface.py` & `vispy-0.9.6/examples/scene/isocurve_for_trisurface.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/isocurve_for_trisurface_qt.py` & `vispy-0.9.6/examples/scene/isocurve_for_trisurface_qt.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/isocurve_updates.py` & `vispy-0.9.6/examples/scene/isocurve_updates.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/isosurface.py` & `vispy-0.9.6/examples/scene/isosurface.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/line.py` & `vispy-0.9.6/examples/scene/line.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/line_update.py` & `vispy-0.9.6/examples/scene/line_update.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/linear_region.py` & `vispy-0.9.6/examples/scene/linear_region.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/magnify.py` & `vispy-0.9.6/examples/scene/magnify.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/marker_spheres.py` & `vispy-0.9.6/examples/scene/marker_spheres.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/mesh_normals.py` & `vispy-0.9.6/examples/scene/mesh_normals.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/mesh_shading.py` & `vispy-0.9.6/examples/scene/mesh_shading.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/mesh_texture.py` & `vispy-0.9.6/examples/scene/mesh_texture.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/nested_viewbox.py` & `vispy-0.9.6/examples/scene/nested_viewbox.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/one_cam_two_scenes.py` & `vispy-0.9.6/examples/scene/one_cam_two_scenes.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/one_scene_four_cams.py` & `vispy-0.9.6/examples/scene/one_scene_four_cams.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/point_cloud.py` & `vispy-0.9.6/examples/scene/point_cloud.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/polygon.py` & `vispy-0.9.6/examples/scene/polygon.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/save_animation.py` & `vispy-0.9.6/examples/scene/save_animation.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/sensitivity.py` & `vispy-0.9.6/examples/scene/sensitivity.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/shape_draw.py` & `vispy-0.9.6/examples/scene/shape_draw.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/sphere.py` & `vispy-0.9.6/examples/scene/sphere.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/surface_plot.py` & `vispy-0.9.6/examples/scene/surface_plot.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/text.py` & `vispy-0.9.6/examples/scene/text.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/turntable_box.py` & `vispy-0.9.6/examples/scene/turntable_box.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/viewbox.py` & `vispy-0.9.6/examples/scene/viewbox.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/volume.py` & `vispy-0.9.6/examples/scene/volume.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/scene/volume_plane.py` & `vispy-0.9.6/examples/scene/volume_plane.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/app/app_events.py` & `vispy-0.9.6/examples/tutorial/app/app_events.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/app/fps.py` & `vispy-0.9.6/examples/tutorial/app/fps.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/app/shared_context.py` & `vispy-0.9.6/examples/tutorial/app/shared_context.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/app/simple.py` & `vispy-0.9.6/examples/tutorial/app/simple.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/app/simple_wx.py` & `vispy-0.9.6/examples/tutorial/app/simple_wx.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/gl/cube.py` & `vispy-0.9.6/examples/tutorial/gl/cube.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/gl/fireworks.py` & `vispy-0.9.6/examples/tutorial/gl/fireworks.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/gl/quad.py` & `vispy-0.9.6/examples/tutorial/gl/quad.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/gloo/colored_cube.py` & `vispy-0.9.6/examples/tutorial/gloo/colored_cube.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/gloo/lighted_cube.py` & `vispy-0.9.6/examples/tutorial/gloo/lighted_cube.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/gloo/outlined_cube.py` & `vispy-0.9.6/examples/tutorial/gloo/outlined_cube.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/gloo/texture_precision.py` & `vispy-0.9.6/examples/tutorial/gloo/texture_precision.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/gloo/textured_cube.py` & `vispy-0.9.6/examples/tutorial/gloo/textured_cube.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/gloo/textured_quad.py` & `vispy-0.9.6/examples/tutorial/gloo/textured_quad.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/visuals/T01_basic_visual.py` & `vispy-0.9.6/examples/tutorial/visuals/T01_basic_visual.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/visuals/T02_measurements.py` & `vispy-0.9.6/examples/tutorial/visuals/T02_measurements.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/visuals/T03_antialiasing.py` & `vispy-0.9.6/examples/tutorial/visuals/T03_antialiasing.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/visuals/T04_fragment_programs.py` & `vispy-0.9.6/examples/tutorial/visuals/T04_fragment_programs.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/examples/tutorial/visuals/T05_viewer_location.py` & `vispy-0.9.6/examples/tutorial/visuals/T05_viewer_location.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/setup.py` & `vispy-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/__init__.py` & `vispy-0.9.6/vispy/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/__init__.py` & `vispy-0.9.6/vispy/app/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/_default_app.py` & `vispy-0.9.6/vispy/app/_default_app.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/_detect_eventloop.py` & `vispy-0.9.6/vispy/app/_detect_eventloop.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/application.py` & `vispy-0.9.6/vispy/app/application.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/__init__.py` & `vispy-0.9.6/vispy/app/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_egl.py` & `vispy-0.9.6/vispy/app/backends/_egl.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_glfw.py` & `vispy-0.9.6/vispy/app/backends/_glfw.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_jupyter_rfb.py` & `vispy-0.9.6/vispy/app/backends/_jupyter_rfb.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_offscreen_util.py` & `vispy-0.9.6/vispy/app/backends/_offscreen_util.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_osmesa.py` & `vispy-0.9.6/vispy/app/backends/_osmesa.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_pyglet.py` & `vispy-0.9.6/vispy/app/backends/_pyglet.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_pyqt4.py` & `vispy-0.9.6/vispy/app/backends/_pyqt4.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_pyqt5.py` & `vispy-0.9.6/vispy/app/backends/_pyqt5.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_pyqt6.py` & `vispy-0.9.6/vispy/app/backends/_pyqt6.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_pyside.py` & `vispy-0.9.6/vispy/app/backends/_pyside.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_pyside2.py` & `vispy-0.9.6/vispy/app/backends/_pyside2.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_pyside6.py` & `vispy-0.9.6/vispy/app/backends/_pyside6.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_qt.py` & `vispy-0.9.6/vispy/app/backends/_qt.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         if LooseVersion(QT_VERSION_STR) >= '5.4.0':
             from PyQt5.QtWidgets import QOpenGLWidget as QGLWidget
             from PyQt5.QtGui import QSurfaceFormat as QGLFormat
             QT5_NEW_API = True
         else:
             from PyQt5.QtOpenGL import QGLWidget, QGLFormat
     from PyQt5 import QtGui, QtCore, QtWidgets, QtTest
-    QWidget, QApplication = QtWidgets.QWidget, QtWidgets.QApplication  # 
+    QWidget, QApplication = QtWidgets.QWidget, QtWidgets.QApplication  # Compat
 elif qt_lib == 'pyqt6':
     _check_imports('PyQt6')
     if not USE_EGL:
         from PyQt6.QtCore import QT_VERSION_STR
         if LooseVersion(QT_VERSION_STR) >= '6.0.0':
             from PyQt6.QtOpenGLWidgets import QOpenGLWidget as QGLWidget
             from PyQt6.QtGui import QSurfaceFormat as QGLFormat
@@ -626,15 +626,15 @@
         mod = ()
         qtmod = event.modifiers()
         qt_keyboard_modifiers = QtCore.Qt.KeyboardModifier if PYQT6_API else QtCore.Qt
         for q, v in ([qt_keyboard_modifiers.ShiftModifier, keys.SHIFT],
                      [qt_keyboard_modifiers.ControlModifier, keys.CONTROL],
                      [qt_keyboard_modifiers.AltModifier, keys.ALT],
                      [qt_keyboard_modifiers.MetaModifier, keys.META]):
-            if q & qtmod:
+            if qtmod & q:
                 mod += (v,)
         return mod
 
 
 _EGL_DISPLAY = None
 egl = None
```

### Comparing `vispy-0.9.5/vispy/app/backends/_sdl2.py` & `vispy-0.9.6/vispy/app/backends/_sdl2.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_template.py` & `vispy-0.9.6/vispy/app/backends/_template.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_tk.py` & `vispy-0.9.6/vispy/app/backends/_tk.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/_wx.py` & `vispy-0.9.6/vispy/app/backends/_wx.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/tests/test_offscreen_util.py` & `vispy-0.9.6/vispy/app/backends/tests/test_offscreen_util.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/backends/tests/test_rfb.py` & `vispy-0.9.6/vispy/app/backends/tests/test_rfb.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/base.py` & `vispy-0.9.6/vispy/app/base.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/canvas.py` & `vispy-0.9.6/vispy/app/canvas.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/qt.py` & `vispy-0.9.6/vispy/app/qt.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/tests/qt-designer.ui` & `vispy-0.9.6/vispy/app/tests/qt-designer.ui`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/tests/test_app.py` & `vispy-0.9.6/vispy/app/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/tests/test_backends.py` & `vispy-0.9.6/vispy/app/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/tests/test_canvas.py` & `vispy-0.9.6/vispy/app/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/tests/test_context.py` & `vispy-0.9.6/vispy/app/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/tests/test_qt.py` & `vispy-0.9.6/vispy/app/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/tests/test_simultaneous.py` & `vispy-0.9.6/vispy/app/tests/test_simultaneous.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/app/timer.py` & `vispy-0.9.6/vispy/app/timer.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/color/__init__.py` & `vispy-0.9.6/vispy/color/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/color/_color_dict.py` & `vispy-0.9.6/vispy/color/_color_dict.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/color/color_array.py` & `vispy-0.9.6/vispy/color/color_array.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/color/color_space.py` & `vispy-0.9.6/vispy/color/color_space.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/color/colormap.py` & `vispy-0.9.6/vispy/color/colormap.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/color/tests/test_color.py` & `vispy-0.9.6/vispy/color/tests/test_color.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/ext/cocoapy.py` & `vispy-0.9.6/vispy/ext/cocoapy.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/ext/cubehelix.py` & `vispy-0.9.6/vispy/ext/cubehelix.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/ext/egl.py` & `vispy-0.9.6/vispy/ext/egl.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/ext/fontconfig.py` & `vispy-0.9.6/vispy/ext/fontconfig.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/ext/gdi32plus.py` & `vispy-0.9.6/vispy/ext/gdi32plus.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/ext/osmesa.py` & `vispy-0.9.6/vispy/ext/osmesa.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/__init__.py` & `vispy-0.9.6/vispy/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/_triangulation_debugger.py` & `vispy-0.9.6/vispy/geometry/_triangulation_debugger.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/calculations.py` & `vispy-0.9.6/vispy/geometry/calculations.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/curves.py` & `vispy-0.9.6/vispy/geometry/curves.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/generation.py` & `vispy-0.9.6/vispy/geometry/generation.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/isocurve.py` & `vispy-0.9.6/vispy/geometry/isocurve.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/isosurface.py` & `vispy-0.9.6/vispy/geometry/isosurface.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/meshdata.py` & `vispy-0.9.6/vispy/geometry/meshdata.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/normals.py` & `vispy-0.9.6/vispy/geometry/normals.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/parametric.py` & `vispy-0.9.6/vispy/geometry/parametric.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/polygon.py` & `vispy-0.9.6/vispy/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/rect.py` & `vispy-0.9.6/vispy/geometry/rect.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/tests/test_calculations.py` & `vispy-0.9.6/vispy/geometry/tests/test_calculations.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/tests/test_generation.py` & `vispy-0.9.6/vispy/geometry/tests/test_generation.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/tests/test_meshdata.py` & `vispy-0.9.6/vispy/geometry/tests/test_meshdata.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/tests/test_triangulation.py` & `vispy-0.9.6/vispy/geometry/tests/test_triangulation.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/torusknot.py` & `vispy-0.9.6/vispy/geometry/torusknot.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/geometry/triangulation.py` & `vispy-0.9.6/vispy/geometry/triangulation.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/__init__.py` & `vispy-0.9.6/vispy/gloo/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/buffer.py` & `vispy-0.9.6/vispy/gloo/buffer.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/context.py` & `vispy-0.9.6/vispy/gloo/context.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/framebuffer.py` & `vispy-0.9.6/vispy/gloo/framebuffer.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/__init__.py` & `vispy-0.9.6/vispy/gloo/gl/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/_constants.py` & `vispy-0.9.6/vispy/gloo/gl/_constants.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/_es2.py` & `vispy-0.9.6/vispy/gloo/gl/_es2.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/_gl2.py` & `vispy-0.9.6/vispy/gloo/gl/_gl2.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/_proxy.py` & `vispy-0.9.6/vispy/gloo/gl/_proxy.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/_pyopengl2.py` & `vispy-0.9.6/vispy/gloo/gl/_pyopengl2.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/dummy.py` & `vispy-0.9.6/vispy/gloo/gl/dummy.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/es2.py` & `vispy-0.9.6/vispy/gloo/gl/es2.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/gl2.py` & `vispy-0.9.6/vispy/gloo/gl/gl2.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/glplus.py` & `vispy-0.9.6/vispy/gloo/gl/glplus.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/pyopengl2.py` & `vispy-0.9.6/vispy/gloo/gl/pyopengl2.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/tests/test_basics.py` & `vispy-0.9.6/vispy/gloo/gl/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/tests/test_functionality.py` & `vispy-0.9.6/vispy/gloo/gl/tests/test_functionality.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/tests/test_names.py` & `vispy-0.9.6/vispy/gloo/gl/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/gl/tests/test_use.py` & `vispy-0.9.6/vispy/gloo/gl/tests/test_use.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/glir.py` & `vispy-0.9.6/vispy/gloo/glir.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/globject.py` & `vispy-0.9.6/vispy/gloo/globject.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/preprocessor.py` & `vispy-0.9.6/vispy/gloo/preprocessor.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/program.py` & `vispy-0.9.6/vispy/gloo/program.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/tests/test_buffer.py` & `vispy-0.9.6/vispy/gloo/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/tests/test_context.py` & `vispy-0.9.6/vispy/gloo/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/tests/test_framebuffer.py` & `vispy-0.9.6/vispy/gloo/tests/test_framebuffer.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/tests/test_glir.py` & `vispy-0.9.6/vispy/gloo/tests/test_glir.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/tests/test_globject.py` & `vispy-0.9.6/vispy/gloo/tests/test_globject.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/tests/test_program.py` & `vispy-0.9.6/vispy/gloo/tests/test_program.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/tests/test_texture.py` & `vispy-0.9.6/vispy/gloo/tests/test_texture.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/tests/test_use_gloo.py` & `vispy-0.9.6/vispy/gloo/tests/test_use_gloo.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/tests/test_util.py` & `vispy-0.9.6/vispy/gloo/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/tests/test_wrappers.py` & `vispy-0.9.6/vispy/gloo/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/texture.py` & `vispy-0.9.6/vispy/gloo/texture.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/util.py` & `vispy-0.9.6/vispy/gloo/util.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/gloo/wrappers.py` & `vispy-0.9.6/vispy/gloo/wrappers.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/__init__.py` & `vispy-0.9.6/vispy/glsl/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/antialias/cap-butt.glsl` & `vispy-0.9.6/vispy/glsl/antialias/cap-butt.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/antialias/cap-round.glsl` & `vispy-0.9.6/vispy/glsl/antialias/cap-round.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/antialias/cap-square.glsl` & `vispy-0.9.6/vispy/glsl/antialias/cap-square.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/antialias/cap-triangle-in.glsl` & `vispy-0.9.6/vispy/glsl/antialias/cap-triangle-in.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/antialias/cap-triangle-out.glsl` & `vispy-0.9.6/vispy/glsl/antialias/cap-triangle-out.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/antialias/cap.glsl` & `vispy-0.9.6/vispy/glsl/antialias/cap.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/antialias/caps.glsl` & `vispy-0.9.6/vispy/glsl/antialias/caps.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/antialias/filled.glsl` & `vispy-0.9.6/vispy/glsl/antialias/filled.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/antialias/outline.glsl` & `vispy-0.9.6/vispy/glsl/antialias/outline.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/antialias/stroke.glsl` & `vispy-0.9.6/vispy/glsl/antialias/stroke.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrowheads/angle.glsl` & `vispy-0.9.6/vispy/glsl/arrowheads/angle.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrowheads/arrowheads.frag` & `vispy-0.9.6/vispy/glsl/arrowheads/arrowheads.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrowheads/arrowheads.vert` & `vispy-0.9.6/vispy/glsl/arrowheads/arrowheads.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrowheads/curved.glsl` & `vispy-0.9.6/vispy/glsl/arrowheads/curved.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrowheads/inhibitor.glsl` & `vispy-0.9.6/vispy/glsl/arrowheads/inhibitor.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrowheads/stealth.glsl` & `vispy-0.9.6/vispy/glsl/arrowheads/stealth.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrowheads/triangle.glsl` & `vispy-0.9.6/vispy/glsl/arrowheads/triangle.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrows/arrow.frag` & `vispy-0.9.6/vispy/glsl/arrows/arrow.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrows/arrow.vert` & `vispy-0.9.6/vispy/glsl/arrows/arrow.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrows/arrows.glsl` & `vispy-0.9.6/vispy/glsl/arrows/arrows.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrows/common.glsl` & `vispy-0.9.6/vispy/glsl/arrows/common.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrows/curved.glsl` & `vispy-0.9.6/vispy/glsl/arrows/curved.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrows/stealth.glsl` & `vispy-0.9.6/vispy/glsl/arrows/stealth.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrows/triangle-30.glsl` & `vispy-0.9.6/vispy/glsl/arrows/triangle-30.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrows/triangle-60.glsl` & `vispy-0.9.6/vispy/glsl/arrows/triangle-60.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrows/triangle-90.glsl` & `vispy-0.9.6/vispy/glsl/arrows/triangle-90.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/arrows/util.glsl` & `vispy-0.9.6/vispy/glsl/arrows/util.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/build_spatial_filters.py` & `vispy-0.9.6/vispy/glsl/build_spatial_filters.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/agg-fast-path.frag` & `vispy-0.9.6/vispy/glsl/collections/agg-fast-path.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/agg-fast-path.vert` & `vispy-0.9.6/vispy/glsl/collections/agg-fast-path.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/agg-glyph.frag` & `vispy-0.9.6/vispy/glsl/collections/agg-glyph.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/agg-glyph.vert` & `vispy-0.9.6/vispy/glsl/collections/agg-glyph.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/agg-marker.frag` & `vispy-0.9.6/vispy/glsl/collections/agg-marker.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/agg-marker.vert` & `vispy-0.9.6/vispy/glsl/collections/agg-marker.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/agg-path.frag` & `vispy-0.9.6/vispy/glsl/collections/agg-path.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/agg-path.vert` & `vispy-0.9.6/vispy/glsl/collections/agg-path.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/agg-point.frag` & `vispy-0.9.6/vispy/glsl/collections/agg-point.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/agg-point.vert` & `vispy-0.9.6/vispy/glsl/collections/agg-point.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/agg-segment.frag` & `vispy-0.9.6/vispy/glsl/collections/agg-segment.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/agg-segment.vert` & `vispy-0.9.6/vispy/glsl/collections/agg-segment.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/marker.frag` & `vispy-0.9.6/vispy/glsl/collections/marker.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/marker.vert` & `vispy-0.9.6/vispy/glsl/collections/marker.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/raw-path.vert` & `vispy-0.9.6/vispy/glsl/collections/raw-path.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/raw-point.vert` & `vispy-0.9.6/vispy/glsl/collections/raw-point.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/raw-segment.vert` & `vispy-0.9.6/vispy/glsl/collections/raw-segment.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/raw-triangle.vert` & `vispy-0.9.6/vispy/glsl/collections/raw-triangle.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/sdf-glyph-ticks.vert` & `vispy-0.9.6/vispy/glsl/collections/sdf-glyph-ticks.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/sdf-glyph.frag` & `vispy-0.9.6/vispy/glsl/collections/sdf-glyph.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/sdf-glyph.vert` & `vispy-0.9.6/vispy/glsl/collections/sdf-glyph.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/collections/tick-labels.vert` & `vispy-0.9.6/vispy/glsl/collections/tick-labels.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/autumn.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/autumn.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/blues.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/blues.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/color-space.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/color-space.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/colormaps.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/colormaps.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/cool.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/cool.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/fire.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/fire.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/gray.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/gray.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/greens.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/greens.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/hot.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/hot.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/ice.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/ice.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/icefire.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/icefire.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/parse.py` & `vispy-0.9.6/vispy/glsl/colormaps/parse.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/reds.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/reds.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/spring.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/spring.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/summer.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/summer.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/user.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/user.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/util.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/util.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/wheel.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/wheel.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/colormaps/winter.glsl` & `vispy-0.9.6/vispy/glsl/colormaps/winter.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/lines/agg.frag` & `vispy-0.9.6/vispy/glsl/lines/agg.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/lines/agg.vert` & `vispy-0.9.6/vispy/glsl/lines/agg.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/arrow.glsl` & `vispy-0.9.6/vispy/glsl/markers/arrow.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/asterisk.glsl` & `vispy-0.9.6/vispy/glsl/markers/asterisk.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/chevron.glsl` & `vispy-0.9.6/vispy/glsl/markers/chevron.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/clover.glsl` & `vispy-0.9.6/vispy/glsl/markers/clover.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/club.glsl` & `vispy-0.9.6/vispy/glsl/markers/club.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/cross.glsl` & `vispy-0.9.6/vispy/glsl/markers/cross.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/ellipse.glsl` & `vispy-0.9.6/vispy/glsl/markers/ellipse.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/heart.glsl` & `vispy-0.9.6/vispy/glsl/markers/heart.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/infinity.glsl` & `vispy-0.9.6/vispy/glsl/markers/infinity.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/marker-sdf.frag` & `vispy-0.9.6/vispy/glsl/markers/marker-sdf.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/marker-sdf.vert` & `vispy-0.9.6/vispy/glsl/markers/marker-sdf.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/marker.frag` & `vispy-0.9.6/vispy/glsl/markers/marker.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/marker.vert` & `vispy-0.9.6/vispy/glsl/markers/marker.vert`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/markers.glsl` & `vispy-0.9.6/vispy/glsl/markers/markers.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/pin.glsl` & `vispy-0.9.6/vispy/glsl/markers/pin.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/spade.glsl` & `vispy-0.9.6/vispy/glsl/markers/spade.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/markers/triangle.glsl` & `vispy-0.9.6/vispy/glsl/markers/triangle.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/math/circle-through-2-points.glsl` & `vispy-0.9.6/vispy/glsl/math/circle-through-2-points.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/math/constants.glsl` & `vispy-0.9.6/vispy/glsl/math/constants.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/math/double.glsl` & `vispy-0.9.6/vispy/glsl/math/double.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/math/functions.glsl` & `vispy-0.9.6/vispy/glsl/math/functions.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/math/point-to-line-distance.glsl` & `vispy-0.9.6/vispy/glsl/math/point-to-line-distance.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/math/point-to-line-projection.glsl` & `vispy-0.9.6/vispy/glsl/math/point-to-line-projection.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/math/signed-line-distance.glsl` & `vispy-0.9.6/vispy/glsl/math/signed-line-distance.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/math/signed-segment-distance.glsl` & `vispy-0.9.6/vispy/glsl/math/signed-segment-distance.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/misc/regular-grid.frag` & `vispy-0.9.6/vispy/glsl/misc/regular-grid.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/misc/spatial-filters.frag` & `vispy-0.9.6/vispy/glsl/misc/spatial-filters.frag`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/misc/viewport-NDC.glsl` & `vispy-0.9.6/vispy/glsl/misc/viewport-NDC.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/azimuthal-equal-area.glsl` & `vispy-0.9.6/vispy/glsl/transforms/azimuthal-equal-area.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/azimuthal-equidistant.glsl` & `vispy-0.9.6/vispy/glsl/transforms/azimuthal-equidistant.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/hammer.glsl` & `vispy-0.9.6/vispy/glsl/transforms/hammer.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/identity_forward.glsl` & `vispy-0.9.6/vispy/glsl/transforms/identity_forward.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/identity_inverse.glsl` & `vispy-0.9.6/vispy/glsl/transforms/identity_inverse.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/linear-scale.glsl` & `vispy-0.9.6/vispy/glsl/transforms/linear-scale.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/log-scale.glsl` & `vispy-0.9.6/vispy/glsl/transforms/log-scale.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/mercator-transverse-forward.glsl` & `vispy-0.9.6/vispy/glsl/transforms/mercator-transverse-forward.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/mercator-transverse-inverse.glsl` & `vispy-0.9.6/vispy/glsl/transforms/mercator-transverse-inverse.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/polar.glsl` & `vispy-0.9.6/vispy/glsl/transforms/polar.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/position.glsl` & `vispy-0.9.6/vispy/glsl/transforms/position.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/power-scale.glsl` & `vispy-0.9.6/vispy/glsl/transforms/power-scale.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/rotate.glsl` & `vispy-0.9.6/vispy/glsl/transforms/rotate.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/translate.glsl` & `vispy-0.9.6/vispy/glsl/transforms/translate.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/transverse_mercator.glsl` & `vispy-0.9.6/vispy/glsl/transforms/transverse_mercator.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/viewport-clipping.glsl` & `vispy-0.9.6/vispy/glsl/transforms/viewport-clipping.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/viewport-transform.glsl` & `vispy-0.9.6/vispy/glsl/transforms/viewport-transform.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/glsl/transforms/viewport.glsl` & `vispy-0.9.6/vispy/glsl/transforms/viewport.glsl`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/io/__init__.py` & `vispy-0.9.6/vispy/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/io/_data/spatial-filters.npy` & `vispy-0.9.6/vispy/io/_data/spatial-filters.npy`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/io/datasets.py` & `vispy-0.9.6/vispy/io/datasets.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/io/image.py` & `vispy-0.9.6/vispy/io/image.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/io/mesh.py` & `vispy-0.9.6/vispy/io/mesh.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/io/stl.py` & `vispy-0.9.6/vispy/io/stl.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/io/tests/test_image.py` & `vispy-0.9.6/vispy/io/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/io/tests/test_io.py` & `vispy-0.9.6/vispy/io/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/io/wavefront.py` & `vispy-0.9.6/vispy/io/wavefront.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/plot/__init__.py` & `vispy-0.9.6/vispy/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/plot/fig.py` & `vispy-0.9.6/vispy/plot/fig.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/plot/plotwidget.py` & `vispy-0.9.6/vispy/plot/plotwidget.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/plot/tests/test_plot.py` & `vispy-0.9.6/vispy/plot/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/__init__.py` & `vispy-0.9.6/vispy/scene/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/cameras/__init__.py` & `vispy-0.9.6/vispy/scene/cameras/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/cameras/_base.py` & `vispy-0.9.6/vispy/scene/cameras/_base.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/cameras/arcball.py` & `vispy-0.9.6/vispy/scene/cameras/arcball.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/cameras/base_camera.py` & `vispy-0.9.6/vispy/scene/cameras/base_camera.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/cameras/fly.py` & `vispy-0.9.6/vispy/scene/cameras/fly.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/cameras/magnify.py` & `vispy-0.9.6/vispy/scene/cameras/magnify.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/cameras/panzoom.py` & `vispy-0.9.6/vispy/scene/cameras/panzoom.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/cameras/perspective.py` & `vispy-0.9.6/vispy/scene/cameras/perspective.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/cameras/tests/test_link.py` & `vispy-0.9.6/vispy/scene/cameras/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/cameras/tests/test_perspective.py` & `vispy-0.9.6/vispy/scene/cameras/tests/test_perspective.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/cameras/turntable.py` & `vispy-0.9.6/vispy/scene/cameras/turntable.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/canvas.py` & `vispy-0.9.6/vispy/scene/canvas.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/events.py` & `vispy-0.9.6/vispy/scene/events.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/node.py` & `vispy-0.9.6/vispy/scene/node.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/subscene.py` & `vispy-0.9.6/vispy/scene/subscene.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/tests/test_canvas.py` & `vispy-0.9.6/vispy/scene/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/tests/test_node.py` & `vispy-0.9.6/vispy/scene/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/tests/test_visuals.py` & `vispy-0.9.6/vispy/scene/tests/test_visuals.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/visuals.py` & `vispy-0.9.6/vispy/scene/visuals.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/widgets/__init__.py` & `vispy-0.9.6/vispy/scene/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/widgets/anchor.py` & `vispy-0.9.6/vispy/scene/widgets/anchor.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/widgets/axis.py` & `vispy-0.9.6/vispy/scene/widgets/axis.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/widgets/colorbar.py` & `vispy-0.9.6/vispy/scene/widgets/colorbar.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/widgets/console.py` & `vispy-0.9.6/vispy/scene/widgets/console.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/widgets/grid.py` & `vispy-0.9.6/vispy/scene/widgets/grid.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/widgets/label.py` & `vispy-0.9.6/vispy/scene/widgets/label.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/widgets/tests/test_colorbar.py` & `vispy-0.9.6/vispy/scene/widgets/tests/test_colorbar.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/widgets/viewbox.py` & `vispy-0.9.6/vispy/scene/widgets/viewbox.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/scene/widgets/widget.py` & `vispy-0.9.6/vispy/scene/widgets/widget.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/testing/__init__.py` & `vispy-0.9.6/vispy/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/testing/_runners.py` & `vispy-0.9.6/vispy/testing/_runners.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/testing/_testing.py` & `vispy-0.9.6/vispy/testing/_testing.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/testing/image_tester.py` & `vispy-0.9.6/vispy/testing/image_tester.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/testing/rendered_array_tester.py` & `vispy-0.9.6/vispy/testing/rendered_array_tester.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/testing/tests/test_testing.py` & `vispy-0.9.6/vispy/testing/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/__init__.py` & `vispy-0.9.6/vispy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/check_environment.py` & `vispy-0.9.6/vispy/util/check_environment.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/config.py` & `vispy-0.9.6/vispy/util/config.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/dpi/__init__.py` & `vispy-0.9.6/vispy/util/dpi/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/dpi/_linux.py` & `vispy-0.9.6/vispy/util/dpi/_linux.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/dpi/_quartz.py` & `vispy-0.9.6/vispy/util/dpi/_quartz.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/dpi/_win32.py` & `vispy-0.9.6/vispy/util/dpi/_win32.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/eq.py` & `vispy-0.9.6/vispy/util/eq.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/event.py` & `vispy-0.9.6/vispy/util/event.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fetching.py` & `vispy-0.9.6/vispy/util/fetching.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/filter.py` & `vispy-0.9.6/vispy/util/filter.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fonts/__init__.py` & `vispy-0.9.6/vispy/util/fonts/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fonts/_freetype.py` & `vispy-0.9.6/vispy/util/fonts/_freetype.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fonts/_quartz.py` & `vispy-0.9.6/vispy/util/fonts/_quartz.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fonts/_triage.py` & `vispy-0.9.6/vispy/util/fonts/_triage.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fonts/_vispy_fonts.py` & `vispy-0.9.6/vispy/util/fonts/_vispy_fonts.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fonts/_win32.py` & `vispy-0.9.6/vispy/util/fonts/_win32.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fonts/data/OpenSans-Bold.ttf` & `vispy-0.9.6/vispy/util/fonts/data/OpenSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fonts/data/OpenSans-BoldItalic.ttf` & `vispy-0.9.6/vispy/util/fonts/data/OpenSans-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fonts/data/OpenSans-Italic.ttf` & `vispy-0.9.6/vispy/util/fonts/data/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fonts/data/OpenSans-Regular.ttf` & `vispy-0.9.6/vispy/util/fonts/data/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fonts/tests/test_font.py` & `vispy-0.9.6/vispy/util/fonts/tests/test_font.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/fourier.py` & `vispy-0.9.6/vispy/util/fourier.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/frozen.py` & `vispy-0.9.6/vispy/util/frozen.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/gallery_scraper.py` & `vispy-0.9.6/vispy/util/gallery_scraper.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/keys.py` & `vispy-0.9.6/vispy/util/keys.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/logs.py` & `vispy-0.9.6/vispy/util/logs.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/osmesa_gl.py` & `vispy-0.9.6/vispy/util/osmesa_gl.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/profiler.py` & `vispy-0.9.6/vispy/util/profiler.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/quaternion.py` & `vispy-0.9.6/vispy/util/quaternion.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/__init__.py` & `vispy-0.9.6/vispy/util/svg/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/base.py` & `vispy-0.9.6/vispy/util/svg/base.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/color.py` & `vispy-0.9.6/vispy/util/svg/color.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/element.py` & `vispy-0.9.6/vispy/util/svg/element.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/geometry.py` & `vispy-0.9.6/vispy/util/svg/geometry.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/group.py` & `vispy-0.9.6/vispy/util/svg/group.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/length.py` & `vispy-0.9.6/vispy/util/svg/length.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/number.py` & `vispy-0.9.6/vispy/util/svg/number.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/path.py` & `vispy-0.9.6/vispy/util/svg/path.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/shapes.py` & `vispy-0.9.6/vispy/util/svg/shapes.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/style.py` & `vispy-0.9.6/vispy/util/svg/style.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/svg.py` & `vispy-0.9.6/vispy/util/svg/svg.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/transform.py` & `vispy-0.9.6/vispy/util/svg/transform.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/transformable.py` & `vispy-0.9.6/vispy/util/svg/transformable.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/svg/viewport.py` & `vispy-0.9.6/vispy/util/svg/viewport.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/tests/test_config.py` & `vispy-0.9.6/vispy/util/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/tests/test_docstring_parameters.py` & `vispy-0.9.6/vispy/util/tests/test_docstring_parameters.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/tests/test_emitter_group.py` & `vispy-0.9.6/vispy/util/tests/test_emitter_group.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/tests/test_event_emitter.py` & `vispy-0.9.6/vispy/util/tests/test_event_emitter.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/tests/test_fourier.py` & `vispy-0.9.6/vispy/util/tests/test_fourier.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/tests/test_gallery_scraper.py` & `vispy-0.9.6/vispy/util/tests/test_gallery_scraper.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/tests/test_import.py` & `vispy-0.9.6/vispy/util/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/tests/test_key.py` & `vispy-0.9.6/vispy/util/tests/test_key.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/tests/test_logging.py` & `vispy-0.9.6/vispy/util/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/tests/test_transforms.py` & `vispy-0.9.6/vispy/util/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/tests/test_vispy.py` & `vispy-0.9.6/vispy/util/tests/test_vispy.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/transforms.py` & `vispy-0.9.6/vispy/util/transforms.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/util/wrappers.py` & `vispy-0.9.6/vispy/util/wrappers.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/__init__.py` & `vispy-0.9.6/vispy/visuals/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/_scalable_textures.py` & `vispy-0.9.6/vispy/visuals/_scalable_textures.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/axis.py` & `vispy-0.9.6/vispy/visuals/axis.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/border.py` & `vispy-0.9.6/vispy/visuals/border.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/box.py` & `vispy-0.9.6/vispy/visuals/box.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/__init__.py` & `vispy-0.9.6/vispy/visuals/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/agg_fast_path_collection.py` & `vispy-0.9.6/vispy/visuals/collections/agg_fast_path_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/agg_path_collection.py` & `vispy-0.9.6/vispy/visuals/collections/agg_path_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/agg_point_collection.py` & `vispy-0.9.6/vispy/visuals/collections/agg_point_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/agg_segment_collection.py` & `vispy-0.9.6/vispy/visuals/collections/agg_segment_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/array_list.py` & `vispy-0.9.6/vispy/visuals/collections/array_list.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/base_collection.py` & `vispy-0.9.6/vispy/visuals/collections/base_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/collection.py` & `vispy-0.9.6/vispy/visuals/collections/collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/path_collection.py` & `vispy-0.9.6/vispy/visuals/collections/path_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/point_collection.py` & `vispy-0.9.6/vispy/visuals/collections/point_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/polygon_collection.py` & `vispy-0.9.6/vispy/visuals/collections/polygon_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/raw_path_collection.py` & `vispy-0.9.6/vispy/visuals/collections/raw_path_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/raw_point_collection.py` & `vispy-0.9.6/vispy/visuals/collections/raw_point_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/raw_polygon_collection.py` & `vispy-0.9.6/vispy/visuals/collections/raw_polygon_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/raw_segment_collection.py` & `vispy-0.9.6/vispy/visuals/collections/raw_segment_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/raw_triangle_collection.py` & `vispy-0.9.6/vispy/visuals/collections/raw_triangle_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/segment_collection.py` & `vispy-0.9.6/vispy/visuals/collections/segment_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/triangle_collection.py` & `vispy-0.9.6/vispy/visuals/collections/triangle_collection.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/collections/util.py` & `vispy-0.9.6/vispy/visuals/collections/util.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/colorbar.py` & `vispy-0.9.6/vispy/visuals/colorbar.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/cube.py` & `vispy-0.9.6/vispy/visuals/cube.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/ellipse.py` & `vispy-0.9.6/vispy/visuals/ellipse.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/filters/base_filter.py` & `vispy-0.9.6/vispy/visuals/filters/base_filter.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/filters/clipper.py` & `vispy-0.9.6/vispy/visuals/filters/clipper.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/filters/clipping_planes.py` & `vispy-0.9.6/vispy/visuals/filters/clipping_planes.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/filters/color.py` & `vispy-0.9.6/vispy/visuals/filters/color.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/filters/mesh.py` & `vispy-0.9.6/vispy/visuals/filters/mesh.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/filters/picking.py` & `vispy-0.9.6/vispy/visuals/filters/picking.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/glsl/antialiasing.py` & `vispy-0.9.6/vispy/visuals/glsl/antialiasing.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/glsl/color.py` & `vispy-0.9.6/vispy/visuals/glsl/color.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/graphs/graph.py` & `vispy-0.9.6/vispy/visuals/graphs/graph.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/graphs/layouts/__init__.py` & `vispy-0.9.6/vispy/visuals/graphs/layouts/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/graphs/layouts/circular.py` & `vispy-0.9.6/vispy/visuals/graphs/layouts/circular.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/graphs/layouts/force_directed.py` & `vispy-0.9.6/vispy/visuals/graphs/layouts/force_directed.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/graphs/layouts/networkx_layout.py` & `vispy-0.9.6/vispy/visuals/graphs/layouts/networkx_layout.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/graphs/layouts/random.py` & `vispy-0.9.6/vispy/visuals/graphs/layouts/random.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/graphs/tests/test_layouts.py` & `vispy-0.9.6/vispy/visuals/graphs/tests/test_layouts.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/graphs/tests/test_networkx_layout.py` & `vispy-0.9.6/vispy/visuals/graphs/tests/test_networkx_layout.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/graphs/util.py` & `vispy-0.9.6/vispy/visuals/graphs/util.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/gridlines.py` & `vispy-0.9.6/vispy/visuals/gridlines.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/gridmesh.py` & `vispy-0.9.6/vispy/visuals/gridmesh.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/histogram.py` & `vispy-0.9.6/vispy/visuals/histogram.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/image.py` & `vispy-0.9.6/vispy/visuals/image.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/infinite_line.py` & `vispy-0.9.6/vispy/visuals/infinite_line.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/isocurve.py` & `vispy-0.9.6/vispy/visuals/isocurve.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/isoline.py` & `vispy-0.9.6/vispy/visuals/isoline.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/isosurface.py` & `vispy-0.9.6/vispy/visuals/isosurface.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/line/arrow.py` & `vispy-0.9.6/vispy/visuals/line/arrow.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/line/dash_atlas.py` & `vispy-0.9.6/vispy/visuals/line/dash_atlas.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/line/line.py` & `vispy-0.9.6/vispy/visuals/line/line.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/line_plot.py` & `vispy-0.9.6/vispy/visuals/line_plot.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/linear_region.py` & `vispy-0.9.6/vispy/visuals/linear_region.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/markers.py` & `vispy-0.9.6/vispy/visuals/markers.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/mesh.py` & `vispy-0.9.6/vispy/visuals/mesh.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/mesh_normals.py` & `vispy-0.9.6/vispy/visuals/mesh_normals.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/plane.py` & `vispy-0.9.6/vispy/visuals/plane.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/polygon.py` & `vispy-0.9.6/vispy/visuals/polygon.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/rectangle.py` & `vispy-0.9.6/vispy/visuals/rectangle.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/regular_polygon.py` & `vispy-0.9.6/vispy/visuals/regular_polygon.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/scrolling_lines.py` & `vispy-0.9.6/vispy/visuals/scrolling_lines.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/shaders/__init__.py` & `vispy-0.9.6/vispy/visuals/shaders/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/shaders/compiler.py` & `vispy-0.9.6/vispy/visuals/shaders/compiler.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/shaders/expression.py` & `vispy-0.9.6/vispy/visuals/shaders/expression.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/shaders/function.py` & `vispy-0.9.6/vispy/visuals/shaders/function.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/shaders/multiprogram.py` & `vispy-0.9.6/vispy/visuals/shaders/multiprogram.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/shaders/parsing.py` & `vispy-0.9.6/vispy/visuals/shaders/parsing.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/shaders/program.py` & `vispy-0.9.6/vispy/visuals/shaders/program.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/shaders/shader_object.py` & `vispy-0.9.6/vispy/visuals/shaders/shader_object.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/shaders/tests/test_function.py` & `vispy-0.9.6/vispy/visuals/shaders/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/shaders/tests/test_multiprogram.py` & `vispy-0.9.6/vispy/visuals/shaders/tests/test_multiprogram.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/shaders/tests/test_parsing.py` & `vispy-0.9.6/vispy/visuals/shaders/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/shaders/variable.py` & `vispy-0.9.6/vispy/visuals/shaders/variable.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/spectrogram.py` & `vispy-0.9.6/vispy/visuals/spectrogram.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/sphere.py` & `vispy-0.9.6/vispy/visuals/sphere.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/surface_plot.py` & `vispy-0.9.6/vispy/visuals/surface_plot.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_arrows.py` & `vispy-0.9.6/vispy/visuals/tests/test_arrows.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_axis.py` & `vispy-0.9.6/vispy/visuals/tests/test_axis.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_collections.py` & `vispy-0.9.6/vispy/visuals/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_colorbar.py` & `vispy-0.9.6/vispy/visuals/tests/test_colorbar.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_colormap.py` & `vispy-0.9.6/vispy/visuals/tests/test_colormap.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_ellipse.py` & `vispy-0.9.6/vispy/visuals/tests/test_ellipse.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_histogram.py` & `vispy-0.9.6/vispy/visuals/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_image.py` & `vispy-0.9.6/vispy/visuals/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_infinite_line.py` & `vispy-0.9.6/vispy/visuals/tests/test_infinite_line.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_linear_region.py` & `vispy-0.9.6/vispy/visuals/tests/test_linear_region.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_markers.py` & `vispy-0.9.6/vispy/visuals/tests/test_markers.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_mesh.py` & `vispy-0.9.6/vispy/visuals/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_mesh_normals.py` & `vispy-0.9.6/vispy/visuals/tests/test_mesh_normals.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_polygon.py` & `vispy-0.9.6/vispy/visuals/tests/test_polygon.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_rectangle.py` & `vispy-0.9.6/vispy/visuals/tests/test_rectangle.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_regular_polygon.py` & `vispy-0.9.6/vispy/visuals/tests/test_regular_polygon.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_scalable_textures.py` & `vispy-0.9.6/vispy/visuals/tests/test_scalable_textures.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_sdf.py` & `vispy-0.9.6/vispy/visuals/tests/test_sdf.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_spectrogram.py` & `vispy-0.9.6/vispy/visuals/tests/test_spectrogram.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_text.py` & `vispy-0.9.6/vispy/visuals/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_volume.py` & `vispy-0.9.6/vispy/visuals/tests/test_volume.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tests/test_windbarb.py` & `vispy-0.9.6/vispy/visuals/tests/test_windbarb.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/text/_sdf_cpu.pyx` & `vispy-0.9.6/vispy/visuals/text/_sdf_cpu.pyx`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/text/_sdf_gpu.py` & `vispy-0.9.6/vispy/visuals/text/_sdf_gpu.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/text/text.py` & `vispy-0.9.6/vispy/visuals/text/text.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/transforms/__init__.py` & `vispy-0.9.6/vispy/visuals/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/transforms/_util.py` & `vispy-0.9.6/vispy/visuals/transforms/_util.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/transforms/base_transform.py` & `vispy-0.9.6/vispy/visuals/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/transforms/chain.py` & `vispy-0.9.6/vispy/visuals/transforms/chain.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/transforms/interactive.py` & `vispy-0.9.6/vispy/visuals/transforms/interactive.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/transforms/linear.py` & `vispy-0.9.6/vispy/visuals/transforms/linear.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/transforms/nonlinear.py` & `vispy-0.9.6/vispy/visuals/transforms/nonlinear.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/transforms/tests/test_transforms.py` & `vispy-0.9.6/vispy/visuals/transforms/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/transforms/transform_system.py` & `vispy-0.9.6/vispy/visuals/transforms/transform_system.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/tube.py` & `vispy-0.9.6/vispy/visuals/tube.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/visual.py` & `vispy-0.9.6/vispy/visuals/visual.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/volume.py` & `vispy-0.9.6/vispy/visuals/volume.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/windbarb.py` & `vispy-0.9.6/vispy/visuals/windbarb.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy/visuals/xyz_axis.py` & `vispy-0.9.6/vispy/visuals/xyz_axis.py`

 * *Files identical despite different names*

### Comparing `vispy-0.9.5/vispy.egg-info/PKG-INFO` & `vispy-0.9.6/vispy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vispy
-Version: 0.9.5
+Version: 0.9.6
 Summary: Interactive visualization in Python
 Home-page: http://vispy.org
 Download-URL: https://pypi.python.org/pypi/vispy
 Author: Vispy contributors
 Author-email: vispy@googlegroups.com
 License: (new) BSD
 Keywords: visualization,OpenGl,ES,medical,imaging,3D,plotting,numpy,bigdata,ipython,jupyter,widgets
```

### Comparing `vispy-0.9.5/vispy.egg-info/SOURCES.txt` & `vispy-0.9.6/vispy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

