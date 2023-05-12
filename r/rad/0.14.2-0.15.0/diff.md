# Comparing `tmp/rad-0.14.2.tar.gz` & `tmp/rad-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rad-0.14.2.tar", last modified: Fri Mar 31 14:47:00 2023, max compression
+gzip compressed data, was "rad-0.15.0.tar", last modified: Fri May 12 21:12:44 2023, max compression
```

## Comparing `rad-0.14.2.tar` & `rad-0.15.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.288744 rad-0.14.2/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-31 14:46:46.000000 rad-0.14.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.268742 rad-0.14.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-31 14:46:46.000000 rad-0.14.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-31 14:46:46.000000 rad-0.14.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.268742 rad-0.14.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-31 14:46:46.000000 rad-0.14.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-31 14:46:46.000000 rad-0.14.2/.github/workflows/ci_cron.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-03-31 14:46:46.000000 rad-0.14.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-03-31 14:46:46.000000 rad-0.14.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-03-31 14:46:46.000000 rad-0.14.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-31 14:46:46.000000 rad-0.14.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-31 14:46:46.000000 rad-0.14.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-03-31 14:46:46.000000 rad-0.14.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-03-31 14:46:46.000000 rad-0.14.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-31 14:46:46.000000 rad-0.14.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-31 14:46:46.000000 rad-0.14.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 14:46:46.000000 rad-0.14.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-03-31 14:47:00.288744 rad-0.14.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-31 14:46:46.000000 rad-0.14.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.272743 rad-0.14.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-03-31 14:46:46.000000 rad-0.14.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.272743 rad-0.14.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-31 14:46:46.000000 rad-0.14.2/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    59966 2023-03-31 14:46:46.000000 rad-0.14.2/docs/_static/stsci_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.264742 rad-0.14.2/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.272743 rad-0.14.2/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-31 14:46:46.000000 rad-0.14.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-31 14:46:46.000000 rad-0.14.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-31 14:46:46.000000 rad-0.14.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-31 14:46:46.000000 rad-0.14.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2023-03-31 14:46:46.000000 rad-0.14.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-31 14:46:46.000000 rad-0.14.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-31 14:46:46.000000 rad-0.14.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-03-31 14:46:46.000000 rad-0.14.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-31 14:46:46.000000 rad-0.14.2/docs/manifests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-31 14:46:46.000000 rad-0.14.2/docs/reference_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-03-31 14:46:46.000000 rad-0.14.2/docs/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-03-31 14:46:46.000000 rad-0.14.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.272743 rad-0.14.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-03-31 14:46:46.000000 rad-0.14.2/scripts/insert_next_release.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      954 2023-03-31 14:46:46.000000 rad-0.14.2/scripts/set_release_date.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 14:47:00.288744 rad-0.14.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.264742 rad-0.14.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.272743 rad-0.14.2/src/rad/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-31 14:47:00.000000 rad-0.14.2/src/rad/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/integration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.276743 rad-0.14.2/src/rad/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.276743 rad-0.14.2/src/rad/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (123)    11736 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/manifests/datamodels-1.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.280743 rad-0.14.2/src/rad/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/aperture-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/associations-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/basic-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/cal_logs-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/cal_step-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/coordinates-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/ephemeris-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/exposure-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/guidestar-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/guidewindow-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/observation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/photometry-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/pixelarea-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/pointing-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/program-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/rad_schema-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/ramp-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/ref_file-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.284743 rad-0.14.2/src/rad/resources/schemas/reference_files/
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/inverse_linearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/source_detection-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.288744 rad-0.14.2/src/rad/resources/schemas/tagged_scalars/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/target-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.288744 rad-0.14.2/src/rad/resources/schemas/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/unit/unit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/variance-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/visit-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/wfi_image-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-31 14:46:46.000000 rad-0.14.2/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.276743 rad-0.14.2/src/rad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-03-31 14:47:00.000000 rad-0.14.2/src/rad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-03-31 14:47:00.000000 rad-0.14.2/src/rad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 14:47:00.000000 rad-0.14.2/src/rad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 14:47:00.000000 rad-0.14.2/src/rad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-31 14:47:00.000000 rad-0.14.2/src/rad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-31 14:47:00.000000 rad-0.14.2/src/rad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 14:47:00.288744 rad-0.14.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-31 14:46:46.000000 rad-0.14.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-31 14:46:46.000000 rad-0.14.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-31 14:46:46.000000 rad-0.14.2/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-03-31 14:46:46.000000 rad-0.14.2/tests/test_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-31 14:46:46.000000 rad-0.14.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.595994 rad-0.15.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-12 21:12:33.000000 rad-0.15.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.583994 rad-0.15.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-12 21:12:33.000000 rad-0.15.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-12 21:12:33.000000 rad-0.15.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.583994 rad-0.15.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-12 21:12:33.000000 rad-0.15.0/.github/workflows/changelog.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-12 21:12:33.000000 rad-0.15.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-12 21:12:33.000000 rad-0.15.0/.github/workflows/ci_cron.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-12 21:12:33.000000 rad-0.15.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-12 21:12:33.000000 rad-0.15.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-12 21:12:33.000000 rad-0.15.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-12 21:12:33.000000 rad-0.15.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-12 21:12:33.000000 rad-0.15.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-05-12 21:12:33.000000 rad-0.15.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-05-12 21:12:33.000000 rad-0.15.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-12 21:12:33.000000 rad-0.15.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-12 21:12:33.000000 rad-0.15.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:33.000000 rad-0.15.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-12 21:12:44.595994 rad-0.15.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-12 21:12:33.000000 rad-0.15.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.583994 rad-0.15.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-12 21:12:33.000000 rad-0.15.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.583994 rad-0.15.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-12 21:12:33.000000 rad-0.15.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)    59966 2023-05-12 21:12:33.000000 rad-0.15.0/docs/_static/stsci_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.579994 rad-0.15.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.583994 rad-0.15.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-12 21:12:33.000000 rad-0.15.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-12 21:12:33.000000 rad-0.15.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-12 21:12:33.000000 rad-0.15.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 21:12:33.000000 rad-0.15.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6688 2023-05-12 21:12:33.000000 rad-0.15.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-12 21:12:33.000000 rad-0.15.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-12 21:12:33.000000 rad-0.15.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-05-12 21:12:33.000000 rad-0.15.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-12 21:12:33.000000 rad-0.15.0/docs/manifests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-12 21:12:33.000000 rad-0.15.0/docs/reference_files.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-12 21:12:33.000000 rad-0.15.0/docs/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-12 21:12:33.000000 rad-0.15.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.583994 rad-0.15.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-05-12 21:12:33.000000 rad-0.15.0/scripts/insert_next_release.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      954 2023-05-12 21:12:33.000000 rad-0.15.0/scripts/set_release_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 21:12:44.595994 rad-0.15.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.579994 rad-0.15.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.587994 rad-0.15.0/src/rad/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.587994 rad-0.15.0/src/rad/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.587994 rad-0.15.0/src/rad/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/manifests/datamodels-1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.591994 rad-0.15.0/src/rad/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/aperture-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/associations-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/basic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/cal_logs-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/cal_step-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/coordinates-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/exposure-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/guidestar-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9255 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/observation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/photometry-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/pointing-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/program-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/ramp-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/ref_file-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.595994 rad-0.15.0/src/rad/resources/schemas/reference_files/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/inverse_linearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/ref_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/resample-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/source_detection-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.595994 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/calibration_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/target-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/variance-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/visit-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wfi_detector-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-12 21:12:33.000000 rad-0.15.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.587994 rad-0.15.0/src/rad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 21:12:44.000000 rad-0.15.0/src/rad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 21:12:44.595994 rad-0.15.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-12 21:12:33.000000 rad-0.15.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-12 21:12:33.000000 rad-0.15.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-12 21:12:33.000000 rad-0.15.0/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-12 21:12:33.000000 rad-0.15.0/tests/test_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-12 21:12:33.000000 rad-0.15.0/tox.ini
```

### Comparing `rad-0.14.2/.github/pull_request_template.md` & `rad-0.15.0/.github/pull_request_template.md`

 * *Files 14% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 <!-- describe the changes comprising this PR here -->
 This PR addresses ...
 
 **Checklist**
 - [ ] Schema changes discussed at RAD Review Board meeting
 - [ ] Added entry in `CHANGES.rst` under the corresponding subsection
 - [ ] Updated relevant roman_datamodels utilities and tests
+- [ ] Passed romancal regression testing on Jenkins / PLWishMaster. Link: https://plwishmaster.stsci.edu:8081/job/RT/job/romancal/XXX/
```

### Comparing `rad-0.14.2/.github/workflows/ci.yml` & `rad-0.15.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/.github/workflows/publish-to-pypi.yml` & `rad-0.15.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/.github/workflows/release.yml` & `rad-0.15.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/.gitignore` & `rad-0.15.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/.pre-commit-config.yaml` & `rad-0.15.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -13,50 +13,50 @@
     - id: check-symlinks
     - id: debug-statements
     - id: detect-private-key
     - id: end-of-file-fixer
     - id: trailing-whitespace
 
 - repo: https://github.com/pre-commit/pygrep-hooks
-  rev: v1.9.0
+  rev: v1.10.0
   hooks:
     - id: python-check-blanket-noqa
     - id: python-check-mock-methods
     - id: rst-directive-colons
     - id: rst-inline-touching-normal
     - id: text-unicode-replacement-char
 
 - repo: https://github.com/codespell-project/codespell
-  rev: v2.2.2
+  rev: v2.2.4
   hooks:
     - id: codespell
       args: ["--write-changes"]
       additional_dependencies:
         - tomli
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: 'v3.3.1'
+  rev: 'v3.4.0'
   hooks:
     - id: pyupgrade
       args: ["--py38-plus"]
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: 'v0.0.207'
+  rev: 'v0.0.265'
   hooks:
     - id: ruff
-      args: ["--fix", "--force-exclude"]
+      args: ["--fix"]
 
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
     - id: isort
 
 - repo: https://github.com/psf/black
-  rev: 22.12.0
+  rev: 23.3.0
   hooks:
     - id: black
 
 - repo: https://github.com/PyCQA/bandit
-  rev: 1.7.4
+  rev: 1.7.5
   hooks:
     - id: bandit
       args: ["-r", "-ll"]
```

### Comparing `rad-0.14.2/CHANGES.rst` & `rad-0.15.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+0.15.0 (2023-05-12)
+-------------------
+
+- Update program to be a string to match association code [#255]
+
+- Add gw_science_file_source to GW file, update size of the filename [#258]
+
+- Update program to be a string to match association code [#255]
+
+- Update guide star id, add catalog version, and add science file name [#258]
+
+- Add gw_science_file_source to GW file, update size of the filename [#258]
+
+- Remove use of deprecated ``pytest-openfiles`` ``pytest`` plugin. This has been replaced by
+  catching ``ResourceWarning`` s. [#231]
+
+- Add read pattern to the exposure group. [#233]
+
+- Add ``distortion`` keyword option to the list of reference files, so that the ``distortion``
+  reference file can be properly allowed in by the ``ref_file-1.0.0`` schema. [#237]
+
+- Changelog CI workflow has been added. [#240]
+
+- Clarifying database tables for guidewindows and guidestar." [#250]
+
+- Remove the ``unit-1.0.0`` schema, because it is no-longer needed. [#248]
+
+- Remove the unused ``pixelarea-1.0.0`` schema, which was replaced by the
+  ``reference_files/pixelarea-1.0.0`` schema. [#245]
+
+- Added support for level 3 mosaic model. [#241]
+
+- Add further restrictions to the ``patternProperties`` keywords in the
+  ``wfi_img_photom`` schema. [#254]
+
+
 0.14.2 (2023-03-31)
 -------------------
 
 - Format the code with ``isort`` and ``black``. [#200]
 
 - Switch linting from ``flake8`` to ``ruff``. [#201]
 
@@ -17,14 +53,15 @@
 
 - Add schema for source detection. [#215]
 
 - Temporarily make source detection optional in cal_logs. [#224]
 
 - Add database team to Code Owners file [#227]
 
+- Update CodeOwners file [#230]
 
 
 0.14.1 (2023-01-31)
 -------------------
 
 - Update guidwindow titles and descriptions. [#193]
```

### Comparing `rad-0.14.2/CODE_OF_CONDUCT.md` & `rad-0.15.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/LICENSE` & `rad-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/PKG-INFO` & `rad-0.15.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.14.2
+Version: 0.15.0
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.14.2/README.md` & `rad-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/docs/Makefile` & `rad-0.15.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/docs/_static/custom.css` & `rad-0.15.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/docs/_static/stsci_logo.png` & `rad-0.15.0/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/docs/conf.py` & `rad-0.15.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,20 @@
 import os
 import sys
 from pathlib import Path
 
 # Ensure documentation examples are deterministically random.
 import numpy
 import stsci_rtd_theme
-import tomli
+
+if sys.version_info < (3, 11):
+    import tomli as tomllib
+else:
+    import tomllib
+
 from importlib_metadata import distribution
 
 try:
     numpy.random.seed(int(os.environ["SOURCE_DATE_EPOCH"]))
 except KeyError:
     pass
 
@@ -42,15 +47,15 @@
     from sphinx_astropy.conf.v1 import *  # noqa: F403
 except ImportError:
     print("ERROR: the documentation requires the sphinx-astropy package to be installed")
     sys.exit(1)
 
 # Get configuration information from pyproject.toml
 with open(Path(__file__).parent.parent / "pyproject.toml", "rb") as configuration_file:
-    conf = tomli.load(configuration_file)
+    conf = tomllib.load(configuration_file)
 configuration = conf["project"]
 
 
 # -- General configuration ----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 # needs_sphinx = '1.2'
```

### Comparing `rad-0.14.2/docs/index.rst` & `rad-0.15.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/docs/make.bat` & `rad-0.15.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/docs/schemas.rst` & `rad-0.15.0/docs/schemas.rst`

 * *Files 20% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     exposure_type-1.0.0
     exposure-1.0.0
     guidestar-1.0.0
     guidewindow_modes-1.0.0
     guidewindow-1.0.0
     observation-1.0.0
     photometry-1.0.0
-    pixelarea-1.0.0
     pointing-1.0.0
     program-1.0.0
     rad_schema-1.0.0
     ramp_fit_output-1.0.0
     ramp-1.0.0
     ref_file-1.0.0
     target-1.0.0
```

### Comparing `rad-0.14.2/pyproject.toml` & `rad-0.15.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     'asdf-astropy >=0.4.0',
 ]
 dynamic = ['version']
 
 [project.optional-dependencies]
 test = [
     'pytest>=4.6.0',
-    'pytest-openfiles>=0.5.0',
     'pytest-doctestplus>=0.11.1',
 ]
 docs = [
     'sphinx',
     'sphinx-asdf>=0.1.3',
     'sphinx-astropy',
     'astropy>=5.0.4',
@@ -61,19 +60,22 @@
 ]
 
 [tool.pytest.ini_options]
 minversion = 4.6
 doctest_plus = true
 doctest_rst = true
 text_file_format = 'rst'
-addopts = '--show-capture=no --open-files'
+addopts = '--show-capture=no'
 testpaths = [
     'tests',
     'src/rad/resources/schemas',
 ]
+filterwarnings = [
+    "error::ResourceWarning",
+]
 asdf_schema_tests_enabled = 'true'
 asdf_schema_skip_tests = 'src/rad/resources/schemas/rad_schema-1.0.0.yaml'
 asdf_schema_root = 'src/rad/resources/schemas'
 
 [tool.isort]
 profile = "black"
 filter_files = true
```

### Comparing `rad-0.14.2/scripts/insert_next_release.py` & `rad-0.15.0/scripts/insert_next_release.py`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/scripts/set_release_date.py` & `rad-0.15.0/scripts/set_release_date.py`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/integration.py` & `rad-0.15.0/src/rad/integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/manifests/datamodels-1.0.yaml` & `rad-0.15.0/src/rad/resources/manifests/datamodels-1.0.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -30,35 +30,35 @@
   description: |-
     Basic Roman Raw Science
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/wfi_image-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/wfi_image-1.0.0
   title: Wfi level 2 image information
   description: |-
     Wfi level 2 image information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/wfi_mosaic-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/wfi_mosaic-1.0.0
+  title: Wfi level 3 mosiac information
+  description: |-
+    Wfi level 3 mosaic information
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/wfi_mode-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/wfi_mode-1.0.0
   title: Roman WFI Instrument Mode
   description: |-
     Roman WFI Instrument
-- tag_uri: asdf://stsci.edu/datamodels/roman/tags/pixelarea-1.0.0
-  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/pixelarea-1.0.0
-  title: Pixel area array
-  description: |-
-    The schema for the pixel area array
 # Metadata Modules
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/exposure-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/exposure-1.0.0
   title: Exposure information
   description: |-
     Exposure information
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/program-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/program-1.0.0
-  title: Xprogram information
+  title: Program information
   description: |-
-    Xprogram information
+    Program information
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/observation-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/observation-1.0.0
   title: Observation information
   description: |-
     Observation information
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/ephemeris-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/ephemeris-1.0.0
@@ -116,14 +116,19 @@
   description: |-
     Guidestar information
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/cal_step-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/cal_step-1.0.0
   title: Calibration Step status information
   description: |-
     Calibration Step status information
+- tag_uri: asdf://stsci.edu/datamodels/roman/tags/resample-1.0.0
+  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/resample-1.0.0
+  title: Resample information
+  description: |-
+    Resample information
 # Reference Modules
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/dark-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/reference_files/dark-1.0.0
   title: Dark reference schema
   description: |-
     Dark reference schema
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/reference_files/distortion-1.0.0
@@ -239,17 +244,8 @@
   description: |-
     SDF software version number
 - tag_uri: asdf://stsci.edu/datamodels/roman/tags/telescope-1.0.0
   schema_uri: asdf://stsci.edu/datamodels/roman/schemas/tagged_scalars/telescope-1.0.0
   title: Telescope used to acquire the data
   description: |-
     Telescope used to acquire the data
-- tag_uri: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-  schema_uri: asdf://stsci.edu/datamodels/roman/schemas/unit/unit-1.0.0
-  title: Special Units used by Roman
-  description: |-
-    This represents the units used by Roman which are not part of
-    [VOUnit syntax, Version 1.0](http://www.ivoa.net/documents/VOUnits/index.html).
-
-    The specific non-VOUnit units used by Roman will be checked/enforced by the
-    converter.
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/aperture-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/aperture-1.0.0.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -18,22 +18,22 @@
            'CGI_CEN', 'WFI_CEN']
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:aperture.AperName
     archive_catalog:
       datatype: nvarchar(40)
-      destination: [ScienceCommon.aperture_name]
+      destination: [ScienceCommon.aperture_name, GuideWindow.aperture_name]
   position_angle:
     title: "[deg] Position angle of aperture used"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD #v3_position_angle in baseline_prime_visits or spacecraft_parameters
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.position_angle]
+      destination: [ScienceCommon.position_angle, GuideWindow.position_angle]
 propertyOrder: [name, position_angle]
 flowStyle: block
 required: [name, position_angle]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/associations-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/associations-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/basic-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/basic-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/cal_step-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/cal_step-1.0.0.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -8,76 +8,76 @@
 properties:
   assign_wcs:
     title: Assign World Coordinate System
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.assign_wcs]
+      destination: [ScienceRefData.assign_wcs, GuideWindow.assign_wcs]
   flat_field:
     title: Flat Field Step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.flat_field]
+      destination: [ScienceRefData.flat_field, GuideWindow.flat_field]
   dark:
     title: Dark Subtraction
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.dark]
+      destination: [ScienceRefData.dark, GuideWindow.dark]
   dq_init:
     title: Data Quality Mask Step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.dq_init]
+      destination: [ScienceRefData.dq_init, GuideWindow.dq_init]
   jump:
     title: Jump Detection Step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.jump]
+      destination: [ScienceRefData.jump, GuideWindow.jump]
   linearity:
     title: Linearity Correction
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.linearity]
+      destination: [ScienceRefData.linearity, GuideWindow.linearity]
   photom:
     title: Photometry Step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.photom]
+      destination: [ScienceRefData.photom, GuideWindow.photom]
   source_detection:
     title: Source Detection Step
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.source_detection]
+      destination: [ScienceRefData.source_detection, GuideWindow.source_detection]
   ramp_fit:
     title: Ramp Fitting
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.ramp_fit]
+      destination: [ScienceRefData.ramp_fit, GuideWindow.ramp_fit]
   saturation:
     title: Saturation Checking
     type: string
     enum: ['N/A', 'COMPLETE', 'SKIPPED', 'INCOMPLETE']
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceRefData.saturation]
+      destination: [ScienceRefData.saturation, GuideWindow.saturation]
 propertyOrder: [assign_wcs, flat_field, dark, dq_init, jump, linearity, photom, source_detection, ramp_fit, saturation]
 flowStyle: block
-required: [assign_wcs, flat_field, dark, dq_init, jump, linearity, photom, ramp_fit, saturation]
+required: [assign_wcs, flat_field, dark, dq_init, jump, linearity, photom, source_detection, ramp_fit, saturation]
 additionalProperties: true
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/common-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/ephemeris-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/ephemeris-1.0.0.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -11,126 +11,126 @@
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.earth_angle]
+      destination: [ScienceCommon.earth_angle, GuideWindow.earth_angle]
   moon_angle:
     title: "[radians] Moon Angle"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.moon_angle]
+      destination: [ScienceCommon.moon_angle, GuideWindow.moon_angle]
   ephemeris_reference_frame:
     title: Ephemeris reference frame
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(10)
-      destination: [ScienceCommon.ephemeris_reference_frame]
+      destination: [ScienceCommon.ephemeris_reference_frame, GuideWindow.ephemeris_reference_frame]
   sun_angle:
     title: "[radians] Sun Angle"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.sun_angle]
+      destination: [ScienceCommon.sun_angle, GuideWindow.sun_angle]
   type:
     title: Type of ephemeris
     type: string
     enum: [DEFINITIVE, PREDICTED]
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(10)
-      destination: [ScienceCommon.ephemeris_type]
+      destination: [ScienceCommon.ephemeris_type, GuideWindow.ephemeris_type]
   time:
     title: UTC time of position and velocity vectors in ephemeris (MJD)
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Roman Science Data Processing (RSDP)
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ephemeris_time]
+      destination: [ScienceCommon.ephemeris_time, GuideWindow.ephemeris_time]
   spatial_x:
     title: "[km] X spatial coordinate of Roman"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Roman Science Data Processing (RSDP)
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.spatial_x]
+      destination: [ScienceCommon.spatial_x, GuideWindow.spatial_x]
   spatial_y:
     title: "[km] Y spatial coordinate of Roman"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Roman Science Data Processing (RSDP)
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.spatial_y]
+      destination: [ScienceCommon.spatial_y, GuideWindow.spatial_y]
   spatial_z:
     title: "[km] Z spatial coordinate of Roman"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Roman Science Data Processing (RSDP)
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.spatial_z]
+      destination: [ScienceCommon.spatial_z, GuideWindow.spatial_z]
   velocity_x:
     title: "[km/s] X component of Roman velocity"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Roman Science Data Processing (RSDP)
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.velocity_x]
+      destination: [ScienceCommon.velocity_x, GuideWindow.velocity_x]
   velocity_y:
     title: "[km/s] Y component of Roman velocity"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Roman Science Data Processing (RSDP)
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.velocity_y]
+      destination: [ScienceCommon.velocity_y, GuideWindow.velocity_y]
   velocity_z:
     title: "[km/s] Z component of Roman velocity"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: Roman Science Data Processing (RSDP)
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.velocity_z]
+      destination: [ScienceCommon.velocity_z, GuideWindow.velocity_z]
 propertyOrder: [earth_angle, moon_angle, sun_angle, type, time,
                 ephemeris_reference_frame, spatial_x, spatial_y,
                 spatial_z, velocity_x, velocity_y, velocity_z]
 flowStyle: block
 required: [earth_angle, moon_angle, sun_angle, type, time,
            ephemeris_reference_frame, spatial_x, spatial_y,
            spatial_z, velocity_x, velocity_y, velocity_z]
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/exposure-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/exposure-1.0.0.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -15,378 +15,397 @@
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [ScienceCommon.exposure_id]
+      destination: [ScienceCommon.exposure_id, GuideWindow.exposure_id]
 
   type:
     $ref: exposure_type-1.0.0
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(25)
-      destination: [ScienceCommon.exposure_type]
+      destination: [ScienceCommon.exposure_type, GuideWindow.exposure_type]
 
   start_time:
     title: UTC exposure start time
     description: |
         This is a python date-time object that records the
         time at the start of the exposure in UTC.
     tag: tag:stsci.edu:asdf/time/time-1.1.0
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: datetime2
-      destination: [ScienceCommon.exposure_start_time]
+      destination: [ScienceCommon.exposure_start_time, GuideWindow.exposure_start_time]
   mid_time:
     title: UTC exposure mid time
     description: |
         This is a python date-time object that records the
         time at the middle of the exposure in UTC.
     tag: tag:stsci.edu:asdf/time/time-1.1.0
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: datetime2
-      destination: [ScienceCommon.exposure_mid_time]
+      destination: [ScienceCommon.exposure_mid_time, GuideWindow.exposure_mid_time]
   end_time:
     title: UTC exposure end time
     description: |
         This is a python date-time object that records the
         time at the end of the exposure in UTC.
     tag: tag:stsci.edu:asdf/time/time-1.1.0
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: datetime2
-      destination: [ScienceCommon.exposure_end_time]
+      destination: [ScienceCommon.exposure_end_time, GuideWindow.exposure_end_time]
   start_time_mjd:
     title: "[d] exposure start time in MJD"
     description: |
          This records the time at the start of the exposure using the
          Modified Julian Date (MJD). This is used in the archive catalog for
          multi-mission matching.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.exposure_start_time_mjd]
+      destination: [ScienceCommon.exposure_start_time_mjd, GuideWindow.exposure_start_time_mjd]
   mid_time_mjd:
     title: "[d] exposure mid time in MJD"
     description: |
         This records the time at the midpoint of the exposure using the
         Modified Julian Date  (MJD). This is used in the archive catalog for
         multi-mission matching.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.exposure_mid_time_mjd]
+      destination: [ScienceCommon.exposure_mid_time_mjd, GuideWindow.exposure_mid_time_mjd]
   end_time_mjd:
     title: "[d] exposure end time in MJD"
     description: |
         This records the time at the end of the exposure using the
         Modified Julian Date  (MJD). This is used in the archive catalog for
         multi-mission matching.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.exposure_end_time_mjd]
+      destination: [ScienceCommon.exposure_end_time_mjd, GuideWindow.exposure_end_time_mjd]
   start_time_tdb:
     title: "[d] TDB time of exposure start in MJD"
     description: |
         This records the time at the start of the exposure using
         the Modified Julian Date for the Barycentric Dynamical Time system
         (TDB, Temps Dynamique Barycentrique), a relativistic coordinate
         time scale.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.exposure_start_time_tdb]
+      destination: [ScienceCommon.exposure_start_time_tdb, GuideWindow.exposure_start_time_tdb]
   mid_time_tdb:
     title: "[d] TDB time of exposure mid in MJD"
     description: |
         This records the time at the midpoint of the exposure using
         the Modified Julian Date for the Barycentric Dynamical Time system
         (TDB, Temps Dynamique Barycentrique), a relativistic coordinate
         time scale.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.exposure_mid_time_tdb]
+      destination: [ScienceCommon.exposure_mid_time_tdb, GuideWindow.exposure_mid_time_tdb]
   end_time_tdb:
     title: "[d] TDB time of exposure end in MJD"
     description: |
         This records the time at the end of the exposure using
         the Modified Julian Date for the Barycentric Dynamical Time system
         (TDB, Temps Dynamique Barycentrique), a relativistic coordinate
         time scale.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.exposure_end_time_tdb]
+      destination: [ScienceCommon.exposure_end_time_tdb, GuideWindow.exposure_end_time_tdb]
   ngroups:
     title: Number of groups in integration
     description: |
         This is the number of resultant frames in the exposure
         that are transmitted to the ground. The WFI data always has the
         number of integrations=1.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [ScienceCommon.exposure_ngroups]
+      destination: [ScienceCommon.exposure_ngroups, GuideWindow.exposure_ngroups]
   nframes:
     title: Number of frames per group
     description: |
         This is the number of science frames that are combined to
         produce a resultant frame.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [ScienceCommon.exposure_nframes]
+      destination: [ScienceCommon.exposure_nframes, GuideWindow.exposure_nframes]
   data_problem:
     title: Science telemetry indicated a problem
     description: |
         This is a flag to indicate that the science telemetry
         experienced a problem.
     type: boolean
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nchar(1)
-      destination: [ScienceCommon.exposure_data_problem]
+      destination: [ScienceCommon.exposure_data_problem, GuideWindow.exposure_data_problem]
   sca_number:
     title: Sensor Chip Assembly number
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [ScienceCommon.exposure_sca_number]
+      destination: [ScienceCommon.exposure_sca_number, GuideWindow.exposure_sca_number]
   gain_factor:
     title: Gain scale factor
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.exposure_gain_factor]
+      destination: [ScienceCommon.exposure_gain_factor, GuideWindow.exposure_gain_factor]
   integration_time:
     title: "[s] Effective integration time"
     description: The effective time that the sensor has been exposed to the sky.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.exposure_integration_time]
+      destination: [ScienceCommon.exposure_integration_time, GuideWindow.exposure_integration_time]
   elapsed_exposure_time:
     title: "[s] Total elapsed exposure time"
     description: |
         The time between the start of the first Reset/Read Science Frame of an Exposure
         and the completion of the final Read Only Science Frame of that Exposure.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.elapsed_exposure_time]
+      destination: [ScienceCommon.elapsed_exposure_time, GuideWindow.elapsed_exposure_time]
   frame_divisor:
     title: Divisor applied to frame-averaged groups
     description: |
         This is the number of reads per resultant. Its use depends upon the definition
         in the MA table.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [ScienceCommon.exposure_frame_divisor]
+      destination: [ScienceCommon.exposure_frame_divisor, GuideWindow.exposure_frame_divisor]
   groupgap:
     title: Number of frames dropped between groups
     description: This is the number of reads that are "dropped" and not used in the resultant.
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [ScienceCommon.exposure_groupgap]
+      destination: [ScienceCommon.exposure_groupgap, GuideWindow.exposure_groupgap]
   frame_time:
     title: "[s] Time between frames"
     description: |
         The time between the end of one read and the start of the next read. This
         depends on the MA table being used.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.exposure_frame_time]
+      destination: [ScienceCommon.exposure_frame_time, GuideWindow.exposure_frame_time]
   group_time:
     title: "[s] Time between groups"
     description: |
         The time that is the sum of the reads that are used to construct a resultant.
         This will depend on the MA table being used.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.exposure_group_time]
+      destination: [ScienceCommon.exposure_group_time, GuideWindow.exposure_group_time]
   exposure_time:
     title: "[s] exposure time"
     description: |
         The time between the start of the first Reset/Read Science Frame of an Exposure
         and the completion of the final Read Only Science Frame of that Exposure.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.exposure_time]
+      destination: [ScienceCommon.exposure_time, GuideWindow.exposure_time]
   effective_exposure_time:
     title: "[s] Effective exposure time"
     description: The time that the detector is collecting photons that are used in the resultants.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.effective_exposure_time]
+      destination: [ScienceCommon.effective_exposure_time, GuideWindow.effective_exposure_time]
   duration:
     title: "[s] Total duration of exposure"
     description: |
         The time that the detector is dedicated to an exposure. This includes any overhead
         and times for dropped frames etc.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.exposure_duration]
+      destination: [ScienceCommon.exposure_duration, GuideWindow.exposure_duration]
   ma_table_name:
     title: Identifier for the multi-accumulation table used
     description: |
         The name of the MA table used for the exposure as defined by the
         PRD (Project Reference Database)
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(50)
-      destination: [ScienceCommon.ma_table_name]
+      destination: [ScienceCommon.ma_table_name, GuideWindow.ma_table_name]
   ma_table_number:
     title: Numerical identifier for the multi-accumulation table used
     description: |
         The number of the MA table used for the exposure as defined by the
         PRD (Project Reference Database). This is used for matching the exposure
         to the appropriate calibration data.
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: smallint
-      destination: [ScienceCommon.ma_table_number]
+      destination: [ScienceCommon.ma_table_number, GuideWindow.ma_table_number]
   level0_compressed:
     title: Level 0 data was compressed
     description: |
         A flag to indicate that the exposure has data that needed to be decompressed by
         the ground system.
     type: boolean
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nchar(1)
-      destination: [ScienceCommon.exposure_level0_compressed]
+      destination: [ScienceCommon.exposure_level0_compressed, GuideWindow.exposure_level0_compressed]
+  read_pattern:
+    title: Pattern of reads
+    description: |
+      Enumeration of detector reads to resultants making up the L1 data downlinked
+      from the observatory
+    type: array
+    items:
+      type: array
+      items:
+        type: integer
+    sdf:
+      special_processing: VALUE_REQUIRED
+      source:
+        origin: TBD
+    archive_catalog:
+      datatype: nvarchar(3500)
+      destination: [ScienceCommon.read_pattern, GuideWindow.read_pattern]
 propertyOrder: [id, type,
            start_time, mid_time, end_time,
            start_time_mjd, mid_time_mjd, end_time_mjd,
            start_time_tdb, mid_time_tdb, end_time_tdb,
            ngroups, nframes, data_problem, sca_number,
            gain_factor, integration_time, elapsed_exposure_time,
            frame_divisor, groupgap,
            frame_time, group_time, exposure_time,
            effective_exposure_time, duration,
-           ma_table_name, ma_table_number, level0_compressed]
+           ma_table_name, ma_table_number, level0_compressed,
+           read_pattern]
 flowStyle: block
 required: [id, type,
            start_time, mid_time, end_time,
            start_time_mjd, mid_time_mjd, end_time_mjd,
            start_time_tdb, mid_time_tdb, end_time_tdb,
            ngroups, nframes, data_problem, sca_number,
            gain_factor, integration_time, elapsed_exposure_time,
            frame_divisor, groupgap,
            frame_time, group_time, exposure_time,
            effective_exposure_time, duration,
-           ma_table_name, ma_table_number, level0_compressed]
+           ma_table_name, ma_table_number, level0_compressed,
+           read_pattern]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/guidestar-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/observation-1.0.0.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,230 +1,184 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/guidestar-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/observation-1.0.0
 
-title: Guide star window information
+title: Observation identifiers
 type: object
 properties:
-  gw_id:
-    title: guide star window identifier
+  obs_id:
+    title: Programmatic observation identifier. The format is 'PPPPPCCAAASSSOOOVVVggsaaeeee' where
+           'PPPPP' is the Program, 'CC' is the execution plan, 'AAA' is the pass, 'SSS' is the
+           segment, 'OOO' is the Observation, 'VVV' is the Visit, 'gg' is the visit file group,
+           's' is the visit file sequence, 'aa' is the visit file activity, and 'eeee' is the
+           exposure ID. The observation ID is the complete concatenation of visit_id +
+           visit_file_statement (visit_file_group + visit_file_sequence + visit_file_activity) +
+           exposure.
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: nvarchar(20)
-      destination: [ScienceCommon.gw_id]
-  gw_fgs_mode:
-    $ref: guidewindow_modes-1.0.0
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: nvarchar(18)
-      destination: [ScienceCommon.gw_fgs_mode]
-  gs_ra:
-    title: "[deg] guide star right ascension"
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_ra]
-  gs_dec:
-    title: "[deg] guide star declination"
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_dec]
-  gs_ura:
-    title: "[deg] guide star right ascension uncertainty"
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
-    archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_ura]
-  gs_udec:
-    title: "[deg] guide star declination uncertainty"
-    type: number
+      datatype: nvarchar(28)
+      destination: [ScienceCommon.obs_id, GuideWindow.obs_id]
+  visit_id:
+    title: A unique identifier for a visit. The format is 'PPPPPCCAAASSSOOOVVV' where 'PPPPP' is the
+           Program, 'CC' is the execution plan, 'AAA' is the pass, 'SSS' is the segment number,
+           'OOO' is the Observation and 'VVV' is the Visit.
+    type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_udec]
-  gs_mag:
-    title: guide star magnitude in detector
-    type: number
+      datatype: nvarchar(19)
+      destination: [ScienceCommon.visit_id, GuideWindow.visit_id]
+  program:
+    title: Program number, defined range is 1..18445; included in obs_id and visit_id as 'PPPPP'.
+    type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_mag]
-  gs_umag:
-    title: guide star magnitude uncertainty
-    type: number
+      datatype: int
+      destination: [ScienceCommon.program, GuideWindow.program]
+  execution_plan:
+    title: Execution plan within the program, defined range is 1..99; included in obs_id and
+           visit_id as 'CC'.
+    type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_umag]
-  data_start:
-    title: MJD start time of guider data within this file
-    type: number
+      datatype: smallint
+      destination: [ScienceCommon.execution_plan, GuideWindow.execution_plan]
+  pass:
+    title: Pass number within execution plan, defined range is 1..999; included in obs_id and
+           visit_id as 'AA'.
+    type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.data_start]
-  data_end:
-    title: MJD end time of guider data within this file
-    type: number
+      datatype: smallint
+      destination: [ScienceCommon.pass, GuideWindow.pass]
+  segment:
+    title: Segment Number within pass, defined range is 1..999; included in obs_id and visit_id as
+           'SSS'.
+    type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.data_end]
-  gs_ctd_x:
-    title: "[arcsec] guide star centroid x position in guider ideal frame"
-    type: number
+      datatype: smallint
+      destination: [ScienceCommon.segment, GuideWindow.segment]
+  observation:
+    title: Observation number within the segment, defined range is 1..999; included in obs_id and
+           visit_id as 'OOO'.
+    type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_ctd_x]
-  gs_ctd_y:
-    title: "[arcsec] guide star centroid y position in guider ideal frame"
-    type: number
+      datatype: smallint
+      destination: [ScienceCommon.observation, GuideWindow.observation]
+  visit:
+    title: Visit number within the observation, defined range of values is 1..999; included in
+           obs_id and visit_id as 'VVV'.
+    type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_ctd_y]
-  gs_ctd_ux:
-    title: uncertainty in the x position of the centroid
-    type: number
+      datatype: smallint
+      destination: [ScienceCommon.visit, GuideWindow.visit]
+  visit_file_group:
+    title: Sequence group within the visit file, defined range of values is 1..99; included in
+           obs_id as 'gg'.
+    type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_ctd_ux]
-  gs_ctd_uy:
-    title: uncertainty in the y position of the centroid
-    type: number
+      datatype: smallint
+      destination: [ScienceCommon.visit_file_group, GuideWindow.visit_file_group]
+  visit_file_sequence:
+    title: Visit file sequence within the group, defined range of values is 1..5; included in
+           obs_id as 's'.
+    type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_ctd_uy]
-  gs_epoch:
-    title: Epoch of guide star coordinates
+      datatype: tinyint
+      destination: [ScienceCommon.visit_file_sequence, GuideWindow.visit_file_sequence]
+  visit_file_activity:
+    title: Visit file activity within the sequence, defined range of values is 1..ZZ; included in
+           obs_id as 'aa'.
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: nvarchar(10)
-      destination: [ScienceCommon.gs_epoch]
-  gs_mura:
-    title: "[mas/yr] Guide star ICRS right ascension proper motion"
-    type: number
+      datatype: nvarchar(2)
+      destination: [ScienceCommon.visit_file_activity, GuideWindow.visit_file_activity]
+  exposure:
+    title: Exposure within the visit, defined range of values is 1..9999; included in obs_id as
+           'eeee'.
+    type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_mura]
-  gs_mudec:
-    title: "[mas/yr] Guide star ICRS declination proper motion"
-    type: number
+      datatype: int
+      destination: [ScienceCommon.observation_exposure, GuideWindow.observation_exposure]
+  template:
+    title: Observation template used
+    type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
-        origin: TBD
+        origin: PSS:dms_visit.template
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_mudec]
-  gs_para:
-    title: Guide star annual parallax
-    type: number
+      datatype: nvarchar(50)
+      destination: [ScienceCommon.template, GuideWindow.template]
+  observation_label:
+    title: Proposer label for the observation
+    type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_para]
-  gs_pattern_error:
-    title: RMS of guide star position
-    description: RMS of guide star position in guide window from pattern matching (error on
-      centroid not explicitly calculated, the FACE information takes all the centroids and
-      calculates the error across the guiding pattern)
-    type: number
-    sdf:
-      special_processing: VALUE_REQUIRED
-      source:
-        origin: TBD
+      datatype: nvarchar(max)
+      destination: [ScienceCommon.observation_label, GuideWindow.observation_label]
+  survey:
+    title: Observation Survey
+    type: string
+    enum: [HLS, EMS, SN, N/A]
     archive_catalog:
-      datatype: float
-      destination: [ScienceCommon.gs_pattern_error]
-  gw_window_xstart:
-    title: Guide window x start position on the detector
-    type: integer
-  gw_window_ystart:
-    title: Guide window y start position on the detector
-    type: integer
-  gw_window_xstop:
-    title: Guide window x stop position on the detector
-    type: integer
-  gw_window_ystop:
-    title: Guide window y stop position on the detector
-    type: integer
-  gw_window_xsize:
-    title: Guide window size in the x direction in detector coordinates
-    type: integer
-  gw_window_ysize:
-    title: Guide window size in the y direction in detector coordinates
-    type: integer
-propertyOrder: [gw_id, gs_ra, gs_dec, gs_ura, gs_udec, gs_mag, gs_umag, gw_fgs_mode,
-                data_start, data_end, gs_ctd_x, gs_ctd_y, gs_ctd_ux, gs_ctd_uy,
-                gs_epoch, gs_mura, gs_mudec, gs_para, gs_pattern_error, gw_window_xstart,
-                gw_window_ystart, gw_window_xstop, gw_window_ystop, gw_window_xsize,
-                gw_window_ysize]
+      datatype: nvarchar(15)
+      destination: [ScienceCommon.survey, GuideWindow.survey]
+propertyOrder: [obs_id, visit_id, program,
+           execution_plan, pass, observation, segment,
+           visit, visit_file_group, visit_file_sequence,
+           visit_file_activity, exposure, template,
+           observation_label, survey]
 flowStyle: block
-required: [gw_id, gs_ra, gs_dec, gs_ura, gs_udec, gs_mag, gs_umag, gw_fgs_mode,
-           data_start, data_end, gs_ctd_x, gs_ctd_y, gs_ctd_ux, gs_ctd_uy,
-           gs_epoch, gs_mura, gs_mudec, gs_para, gs_pattern_error, gw_window_xstart,
-           gw_window_ystart, gw_window_xstop, gw_window_ystop, gw_window_xsize,
-           gw_window_ysize]
+required: [obs_id, visit_id, program,
+           execution_plan, pass, observation, segment,
+           visit, visit_file_group, visit_file_sequence,
+           visit_file_activity, exposure, template,
+           observation_label, survey]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/guidewindow-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/guidewindow-1.0.0.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -16,218 +16,229 @@
             tag: tag:stsci.edu:asdf/time/time-1.1.0
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: datetime2
-              destination: [ScienceCommon.gw_start_time]
+              destination: [GuideWindow.gw_start_time]
           gw_end_time:
             title: UTC time at the end of the guide window exposure
             tag: tag:stsci.edu:asdf/time/time-1.1.0
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: datetime2
-              destination: [ScienceCommon.gw_end_time]
+              destination: [GuideWindow.gw_end_time]
           gw_frame_readout_time:
             title: The readout time for the guide window frame
             type: number
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: float
-              destination: [ScienceCommon.gw_frame_readout_time]
+              destination: [GuideWindow.gw_frame_readout_time]
           gw_function_start_time:
             title: Observatory UTC time at guider function start
             tag: tag:stsci.edu:asdf/time/time-1.1.0
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: datetime2
-              destination: [ScienceCommon.gw_function_start_time]
+              destination: [GuideWindow.gw_function_start_time]
           gw_function_end_time:
             title: Observatory UTC time at guider function end
             tag: tag:stsci.edu:asdf/time/time-1.1.0
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: datetime2
-              destination: [ScienceCommon.gw_function_end_time]
+              destination: [GuideWindow.gw_function_end_time]
           gw_acq_exec_stat:
             title: Guide star window acquisition status
             type: string
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: nvarchar(15)
-              destination: [ScienceCommon.gw_acq_exec_stat]
+              destination: [GuideWindow.gw_acq_exec_stat]
           pedestal_resultant_exp_time:
             title: Total exposure time for the guide window pedestal frames
             description: |
                The cumulative exposure time for all the guide window
                pedestal frames
             type: number
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: float
-              destination: [ScienceCommon.gw_pedestal_resultant_exp_time]
+              destination: [GuideWindow.gw_pedestal_resultant_exp_time]
           signal_resultant_exp_time:
             title: Total exposure time for the guide window resultant frames
             description: |
               The cumulative exposure time for all the guide window
               resultant frames
             type: number
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: float
-              destination: [ScienceCommon.gw_signal_resultant_exp_time]
+              destination: [GuideWindow.gw_signal_resultant_exp_time]
           gw_acq_number:
             title: Guide Window ID "Q"
             description: |
               A single digit representing the guide star acquisition
               number within the visit
             type: integer
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: int
-              destination: [ScienceCommon.gw_acq_number]
+              destination: [GuideWindow.gw_acq_number]
+          gw_science_file_source:
+            title: The science data associated with this guide window
+            description: |
+                The science data file that is associated with this guide window,
+                e.g. "r0000101001001001001_01101_0001_WFI01_uncal.asdf"
+            type: string
+            sdf:
+              special_processing: VALUE_REQUIRED
+              source:
+                origin: Science Data Formatting
+            archive_catalog:
+              datatype: nvarchar(120)
+              destination: [ScienceCommon.gw_science_file_source]
           gw_mode:
             $ref: guidewindow_modes-1.0.0
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: nvarchar(18)
-              destination: [ScienceCommon.gw_mode]
+              destination: [GuideWindow.gw_mode]
           gw_window_xstart:
             title: Guide window x start position on the detector
             type: integer
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: int
-              destination: [ScienceCommon.gw_window_xstart]
+              destination: [GuideWindow.gw_window_xstart]
           gw_window_ystart:
             title: Guide window y start position on the detector
             type: integer
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: int
-              destination: [ScienceCommon.gw_window_ystart]
+              destination: [GuideWindow.gw_window_ystart]
           gw_window_xstop:
             title: Guide window x stop position on the detector
             type: integer
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: int
-              destination: [ScienceCommon.gw_window_xstop]
+              destination: [GuideWindow.gw_window_xstop]
           gw_window_ystop:
             title: Guide window y stop position on the detector
             type: integer
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: int
-              destination: [ScienceCommon.gw_window_ystop]
+              destination: [GuideWindow.gw_window_ystop]
           gw_window_xsize:
             title: Guide window size in the x direction in detector coordinates
             type: integer
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: int
-              destination: [ScienceCommon.gw_window_xsize]
+              destination: [GuideWindow.gw_window_xsize]
           gw_window_ysize:
             title: Guide window size in the y direction in detector coordinates
             type: integer
             sdf:
               special_processing: VALUE_REQUIRED
               source:
                 origin: Science Data Formatting
             archive_catalog:
               datatype: int
-              destination: [ScienceCommon.gw_window_ysize]
+              destination: [GuideWindow.gw_window_ysize]
         required: [gw_start_time, gw_end_time, gw_frame_readout_time,
-                   gw_function_start_time, gw_function_end_time, gw_acq_exec_stat,
-                   pedestal_resultant_exp_time, signal_resultant_exp_time, gw_acq_number,
+                   gw_function_start_time, gw_function_end_time,
+                   gw_acq_exec_stat, pedestal_resultant_exp_time,
+                   signal_resultant_exp_time, gw_acq_number,
                    gw_mode, gw_window_xstart, gw_window_ystart,
                    gw_window_xstop, gw_window_ystop,
-                   gw_window_xsize, gw_window_ysize,]
+                   gw_window_xsize, gw_window_ysize, gw_science_file_source]
   pedestal_frames:
-    title: "Reconstituted and oriented pedestal frame GW images. Dimensions: num_frames,
-            num_combined_resultants (or num_uncombined_resultants), num_reads, x, y"
+    title: "Reconstituted and oriented pedestal frame GW images.
+             Dimensions: num_frames, num_combined_resultants
+             (or num_uncombined_resultants), num_reads, x, y"
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: uint16
         ndim: 5
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
   signal_frames:
     title: "Reconstituted and oriented signal frames. Dimensions: num_frames,
-            num_combined_resultants (or num_uncombined_resultants), num_reads, x, y"
+            num_combined_resultants (or num_uncombined_resultants),
+            num_reads, x, y"
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: uint16
         ndim: 5
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
   amp33:
     title: "Amp 33 reference pixel data. Dimensions: num_frames,
-            num_combined_resultants (or num_uncombined_resultants), num_reads, x, y"
+            num_combined_resultants (or num_uncombined_resultants),
+            num_reads, x, y"
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: uint16
         ndim: 5
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
 propertyOrder: [meta, pedestal_frames, signal_frames, amp33]
 flowStyle: block
 required: [meta, pedestal_frames, signal_frames, amp33]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/photometry-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/photometry-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/pointing-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/pointing-1.0.0.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -11,32 +11,32 @@
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ra_v1]
+      destination: [ScienceCommon.ra_v1, GuideWindow.ra_v1]
   dec_v1:
     title: "[deg] Dec of telescope V1 axis"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.dec_v1]
+      destination: [ScienceCommon.dec_v1, GuideWindow.dec_v1]
   pa_v3:
     title: "[deg] Position angle of telescope V3 axis"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.pa_v3]
+      destination: [ScienceCommon.pa_v3, GuideWindow.pa_v3]
 propertyOrder: [ra_v1, dec_v1, pa_v3]
 flowStyle: block
 required: [ra_v1, dec_v1, pa_v3]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/program-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/program-1.0.0.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -11,64 +11,64 @@
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_program.title
     archive_catalog:
       datatype: nvarchar(200)
-      destination: [ScienceCommon.program_title]
+      destination: [ScienceCommon.program_title, GuideWindow.program_title]
   pi_name:
     title: Principle Investigator name
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         # There are a number of ways to get the pi_name.  Here is one
         # of them: "= apt('./ProposalInformation/PrincipalInvestigator/InvestigatorAddress/LastName') + ', ' + apt('./ProposalInformation/PrincipalInvestigator/InvestigatorAddress/FirstName')"
         origin: TBD
     archive_catalog:
       datatype: nvarchar(100)
-      destination: [ScienceCommon.pi_name]
+      destination: [ScienceCommon.pi_name, GuideWindow.pi_name]
   category:
     title: Program category
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_program.category
     archive_catalog:
       datatype: nvarchar(6)
-      destination: [ScienceCommon.program_category]
+      destination: [ScienceCommon.program_category, GuideWindow.program_category]
   subcategory:
     title: Program subcategory
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_program.subcategory
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceCommon.program_subcategory]
+      destination: [ScienceCommon.program_subcategory, GuideWindow.program_subcategory]
   science_category:
     title: Science category assigned during TAC process
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_program.science_category
     archive_catalog:
       datatype: nvarchar(50)
-      destination: [ScienceCommon.science_category]
+      destination: [ScienceCommon.science_category, GuideWindow.science_category]
   continuation_id:
     title: Continuation of previous Program
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_program.continuation_id
     archive_catalog:
       datatype: int
-      destination: [ScienceCommon.continuation_id]
+      destination: [ScienceCommon.continuation_id, GuideWindow.continuation_id]
 propertyOrder: [title, pi_name, category, subcategory, science_category, continuation_id]
 flowStyle: block
 required: [title, pi_name, category, subcategory, science_category, continuation_id]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/rad_schema-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/rad_schema-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/ramp-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/ramp-1.0.0.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -16,17 +16,15 @@
       tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
       properties:
         value:
           tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
           datatype: float32
           ndim: 3
         unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
+          tag: tag:astropy.org:astropy/units/unit-1.0.0
           enum: ["DN", "electron"]
     pixeldq:
       title: 2-D data quality array for all planes
       tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
       ndim: 2
       datatype: uint32
     groupdq:
@@ -39,81 +37,69 @@
       tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
       properties:
         value:
           tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
           datatype: float32
           ndim: 3
         unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
+          tag: tag:astropy.org:astropy/units/unit-1.0.0
           enum: ["DN", "electron"]
     amp33:
       title: Amp 33 reference pixel data
       tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
       properties:
         value:
           tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
           datatype: uint16
           ndim: 3
         unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
+          tag: tag:astropy.org:astropy/units/unit-1.0.0
           enum: ["DN"]
     border_ref_pix_left:
       title: Original border reference pixels, on left (from viewers perspective).
       tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 3
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
     border_ref_pix_right:
       title: Original border reference pixels, on right (from viewers perspective).
       tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
       properties:
         value:
           tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
           datatype: float32
           ndim: 3
         unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
+          tag: tag:astropy.org:astropy/units/unit-1.0.0
           enum: ["DN"]
     border_ref_pix_top:
       title: Original border reference pixels, on top.
       tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
       properties:
         value:
           tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
           datatype: float32
           ndim: 3
         unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
+          tag: tag:astropy.org:astropy/units/unit-1.0.0
           enum: ["DN"]
     border_ref_pix_bottom:
       title: Original border reference pixels, on bottom.
       tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
       properties:
         value:
           tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
           datatype: float32
           ndim: 3
         unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
+          tag: tag:astropy.org:astropy/units/unit-1.0.0
           enum: ["DN"]
     dq_border_ref_pix_left:
       title: DQ for border reference pixels, on left (from viewers perspective).
       tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
       datatype: uint32
       ndim: 2
     dq_border_ref_pix_right:
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,128 +1,89 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/ramp_fit_output-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/wfi_mosaic-1.0.0
 
-title: Ramp fit output schema
+title: |
+  The schema for WFI Level 3 mosaics.
 
-allOf:
-- type: object
-  properties:
-    meta:
-      allOf:
-        - $ref: common-1.0.0
-    slope:
-      title: Segment-specific slope
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron / s"]
-    sigslope:
-      title: Sigma for segment-specific slope
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron / s"]
-    yint:
-      title: Segment-specific y-intercept
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron"]
-    sigyint:
-      title: Sigma for segment-specific y-intercept
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron"]
-    pedestal:
-      title: Pedestal array
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 2
-        unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron"]
-    weights:
-      title: Weights for segment-specific fits
-      tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-      ndim: 3
-      datatype: float32
-    crmag:
-      title: Approximate CR magnitudes
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron"]
-    var_poisson:
-      title: Variance due to poisson noise for segment-specific slope
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron2 / s2"]
-    var_rnoise:
-      title: Variance due to read noise for segment-specific slope
-      tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-      properties:
-        value:
-          tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-          datatype: float32
-          ndim: 3
-        unit:
-          oneOf:
-            - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-            - tag: tag:astropy.org:astropy/units/unit-1.0.0
-          enum: ["electron2 / s2"]
-  required: [meta, slope, sigslope, yint, sigyint, pedestal, weights, crmag, var_poisson,
-             var_rnoise]
-  propertyOrder: [meta, slope, sigslope, yint, sigyint, pedestal, weights, crmag, var_poisson,
-                  var_rnoise]
+type: object
+properties:
+  meta:
+    allOf:
+      - $ref: common-1.0.0
+      - type: object
+        properties:
+          # Placeholder for 'asn' schema tag
+          # Placeholder for 'dither' schema tag
+          photometry:
+            tag: asdf://stsci.edu/datamodels/roman/tags/photometry-1.0.0
+          resample:
+            tag: asdf://stsci.edu/datamodels/roman/tags/resample-1.0.0
+        required: [photometry]
+  data:
+    title: Science data, excluding border reference pixels.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 2
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron / s"]
+  err:
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 2
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron / s"]
+  context:
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    datatype: uint32
+    ndim: 3
+  weight:
+    tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+    datatype: float32
+    ndim: 2
+  var_poisson:
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 2
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron2 / s2"]
+  var_rnoise:
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 2
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron2 / s2"]
+  var_flat:
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: float32
+        ndim: 2
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["electron2 / s2"]
+  cal_logs:
+    tag: asdf://stsci.edu/datamodels/roman/tags/cal_logs-1.0.0
+propertyOrder: [meta, data, context, err, weight, var_poisson, var_rnoise, var_flat,
+                cal_logs]
 flowStyle: block
+required: [meta, data, context, err, weight, var_poisson, var_rnoise, var_flat,
+           cal_logs]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/ref_file-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/ref_file-1.0.0.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -17,30 +17,32 @@
         type: string
         sdf:
           special_processing: VALUE_REQUIRED
           source:
             origin: TBD
         archive_catalog:
           datatype: nvarchar(120)
-          destination: [ScienceCommon.crds_software_version]
+          destination: [ScienceCommon.crds_software_version, GuideWindow.crds_software_version]
 
       context_used:
         title: CRDS context (.pmap) used to select ref files
         type: string
         sdf:
           special_processing: VALUE_REQUIRED
           source:
             origin: TBD
         archive_catalog:
           datatype: nvarchar(120)
-          destination: [ScienceCommon.crds_context_used]
-
+          destination: [ScienceCommon.crds_context_used, GuideWindow.crds_context_used]
   dark:
     title: Dark reference file information
     type: string
+  distortion:
+    title: Distortion reference file information
+    type: string
   mask:
     title: Mask reference file information
     type: string
   flat:
     title: Flat reference file information
     type: string
   gain:
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/dark-1.0.0.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -44,17 +44,15 @@
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 3
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
   dq:
     title: 2-D data quality array for all planes
     tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
     datatype: uint32
     ndim: 2
   err:
@@ -62,15 +60,13 @@
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 3
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
 required: [meta, data, dq, err]
 flowStyle: block
 propertyOrder: [meta, data, dq, err]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/flat-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/gain-1.0.0.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,13 @@
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 2
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["electron / DN"]
 required: [meta, data]
 flowStyle: block
 propertyOrder: [meta, data]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/inverse_linearity-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/inverse_linearity-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/linearity-1.0.0
 
-title: Inverse linearity correction reference schema
+title: Linearity correction  reference schema
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
-            enum: [INVERSE_LINEARITY]
+            enum: [LINEARITY]
           input_units:
-            title: Units of the input to the inverse linearity polynomial.
-            oneOf:
-              - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-              - tag: tag:astropy.org:astropy/units/unit-1.0.0
+            title: Units of the input to the linearity polynomial.
+            tag: tag:astropy.org:astropy/units/unit-1.0.0
             enum: ["DN"]
           output_units:
-            title: Units of the output of the inverse linearity polynomial.
-            oneOf:
-              - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-              - tag: tag:astropy.org:astropy/units/unit-1.0.0
+            title: Units of the output of the linearity polynomial.
+            tag: tag:astropy.org:astropy/units/unit-1.0.0
             enum: ["DN"]
         required: [output_units, input_units]
   coeffs:
-    title: Inverse linearity coefficients
+    title: Linearity coefficients
     description: |
-      Contains the coefficients of a polynomial to add classic non-linearity
-      to pixels. Both the input to and output from the polynomial are in units
-      of DN. The coefficients have units that contain various powers of DN.
+      Contains the coefficients of a polynomial to correct pixel
+      values for classic non-linearity. Both the input to and
+      output from the polynomial are in units of DN. The coefficients
+      have units that contain various powers of DN.
     tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
     datatype: float32
     # Dimensions: numcoeffs, ysize, xsize
     ndim: 3
   dq:
     title: 2-D data quality array for all planes
     tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/ipc-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/linearity-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/inverse_linearity-1.0.0.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/linearity-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/inverse_linearity-1.0.0
 
-title: Linearity correction  reference schema
+title: Inverse linearity correction reference schema
 
 type: object
 properties:
   meta:
     allOf:
       - $ref: ref_common-1.0.0
       - type: object
         properties:
           reftype:
             type: string
-            enum: [LINEARITY]
+            enum: [INVERSE_LINEARITY]
           input_units:
-            title: Units of the input to the linearity polynomial.
-            oneOf:
-              - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-              - tag: tag:astropy.org:astropy/units/unit-1.0.0
+            title: Units of the input to the inverse linearity polynomial.
+            tag: tag:astropy.org:astropy/units/unit-1.0.0
             enum: ["DN"]
           output_units:
-            title: Units of the output of the linearity polynomial.
-            oneOf:
-              - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-              - tag: tag:astropy.org:astropy/units/unit-1.0.0
+            title: Units of the output of the inverse linearity polynomial.
+            tag: tag:astropy.org:astropy/units/unit-1.0.0
             enum: ["DN"]
         required: [output_units, input_units]
   coeffs:
-    title: Linearity coefficients
+    title: Inverse linearity coefficients
     description: |
-      Contains the coefficients of a polynomial to correct pixel
-      values for classic non-linearity. Both the input to and
-      output from the polynomial are in units of DN. The coefficients
-      have units that contain various powers of DN.
+      Contains the coefficients of a polynomial to add classic non-linearity
+      to pixels. Both the input to and output from the polynomial are in units
+      of DN. The coefficients have units that contain various powers of DN.
     tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
     datatype: float32
     # Dimensions: numcoeffs, ysize, xsize
     ndim: 3
   dq:
     title: 2-D data quality array for all planes
     tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/mask-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/pixelarea-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/readnoise-1.0.0.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -20,15 +20,13 @@
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 2
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
 required: [meta, data]
 flowStyle: block
 propertyOrder: [meta, data]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/ref_common-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/ref_exposure_type-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/saturation-1.0.0.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 2
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
   dq:
     title: 2-D data quality array for all planes
     tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
     datatype: uint32
     ndim: 2
 required: [meta, data, dq]
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/superbias-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,39 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/wfi_img_photom-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/wfi_science_raw-1.0.0
 
-title: WFI imaging photometric flux conversion data model
+title: |
+  The schema for Level 1 WFI science data (both imaging and spectrographic).
 
 type: object
 properties:
   meta:
     allOf:
-      - $ref: ref_common-1.0.0
-      - type: object
-        properties:
-          reftype:
-            type: string
-            enum: [PHOTOM]
-  phot_table:
-    title: Photometric flux conversion factors table
-    type: object
-    patternProperties:
-      "^(F062|F087|F106|F129|F146|F158|F184|F213|GRISM|PRISM|DARK)$":
-        type: object
-        properties:
-          photmjsr:
-            title: Surface brightness, in MJy/steradian
-            anyOf:
-              - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-              - type: "null"
-          uncertainty:
-            title: Uncertainty of surface brightness, in MJy/steradian
-            anyOf:
-              - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-              - type: "null"
-          pixelareasr:
-            title: Nominal pixel area, in steradian
-            anyOf:
-              - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-              - type: "null"
-        required: [photmjsr, uncertainty, pixelareasr]
-    additionalProperties: false
-required: [meta, phot_table]
+      - $ref: common-1.0.0
+  data:
+    title: Science data, including the border reference pixels.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: uint16
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["DN"]
+  amp33:
+    title: Amp 33 reference pixel data.
+    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+    properties:
+      value:
+        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
+        datatype: uint16
+        ndim: 3
+      unit:
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
+        enum: ["DN"]
+propertyOrder: [meta, data, amp33]
 flowStyle: block
-propertyOrder: [meta, phot_table]
+required: [meta, data, amp33]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/target-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/target-1.0.0.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -11,139 +11,139 @@
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_target.target_name
     archive_catalog:
       datatype: nvarchar(100)
-      destination: [ScienceCommon.proposer_target_name]
+      destination: [ScienceCommon.proposer_target_name, GuideWindow.proposer_target_name]
   catalog_name:
     title: Standard astronomical catalog name for target
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_target.standard_target_name
     archive_catalog:
       datatype: nvarchar(256)
-      destination: [ScienceCommon.catalog_name]
+      destination: [ScienceCommon.catalog_name, GuideWindow.catalog_name]
   type:
     title: Type of target
     type: string
     enum: [FIXED, MOVING, GENERIC]
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_target.target_type
     archive_catalog:
       datatype: nvarchar(10)
-      destination: [ScienceCommon.target_type]
+      destination: [ScienceCommon.target_type, GuideWindow.target_type]
   ra:
     title: Target RA at mid time of exposure
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_target.ra_computed
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ra]
+      destination: [ScienceCommon.ra, GuideWindow.ra]
   dec:
     title: Target Dec at mid time of exposure
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_target.dec_computed
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.dec]
+      destination: [ScienceCommon.dec, GuideWindow.dec]
   ra_uncertainty:
     title: Target RA uncertainty
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_target.ra_uncertainty_computed
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ra_uncertainty]
+      destination: [ScienceCommon.ra_uncertainty, GuideWindow.ra_uncertainty]
   dec_uncertainty:
     title: Target Dec uncertainty
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_target.dec_uncertainty_computed
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.dec_uncertainty]
+      destination: [ScienceCommon.dec_uncertainty, GuideWindow.dec_uncertainty]
   proper_motion_ra:
     title: Target proper motion in RA
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_target.ra_proper_motion
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.proper_motion_ra]
+      destination: [ScienceCommon.proper_motion_ra, GuideWindow.proper_motion_ra]
   proper_motion_dec:
     title: Target proper motion in Dec
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_target.dec_proper_motion
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.proper_motion_dec]
+      destination: [ScienceCommon.proper_motion_dec, GuideWindow.proper_motion_dec]
   proper_motion_epoch:
     title: Target proper motion epoch
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_visit.epoch
     archive_catalog:
       datatype: nvarchar(10)
-      destination: [ScienceCommon.proper_motion_epoch]
+      destination: [ScienceCommon.proper_motion_epoch, GuideWindow.proper_motion_epoch]
   proposer_ra:
     title: Proposer's target RA
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:fixed_target.ra_literal
         function: hms_to_degrees
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.proposer_ra]
+      destination: [ScienceCommon.proposer_ra, GuideWindow.proposer_ra]
   proposer_dec:
     title: Proposer's target Dec
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:fixed_target.dec_literal
         function: hms_to_degrees
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.proposer_dec]
+      destination: [ScienceCommon.proposer_dec, GuideWindow.proposer_dec]
   source_type:
     title: Source type used for calibration
     type: string
     enum: [EXTENDED, POINT, UNKNOWN]
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(8)
-      destination: [ScienceCommon.source_type]
+      destination: [ScienceCommon.source_type, GuideWindow.source_type]
 propertyOrder: [proposer_name, catalog_name, type, ra, dec, ra_uncertainty, dec_uncertainty,
            proper_motion_ra, proper_motion_dec, proper_motion_epoch,
            proposer_ra, proposer_dec, source_type]
 flowStyle: block
 required: [proposer_name, catalog_name, type, ra, dec, ra_uncertainty, dec_uncertainty,
            proper_motion_ra, proper_motion_dec, proper_motion_epoch,
            proposer_ra, proposer_dec, source_type]
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/variance-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/variance-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/velocity_aberration-1.0.0.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -11,32 +11,32 @@
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ra_offset]
+      destination: [ScienceCommon.ra_offset, GuideWindow.ra_offset]
   dec_offset:
     title: Velocity aberration declination offset
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.dec_offset]
+      destination: [ScienceCommon.dec_offset, GuideWindow.dec_offset]
   scale_factor:
     title: Velocity aberration scale factor
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.scale_factor]
+      destination: [ScienceCommon.scale_factor, GuideWindow.scale_factor]
 flowStyle: block
 propertyOrder: [ra_offset, dec_offset, scale_factor]
 required: [ra_offset, dec_offset, scale_factor]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/visit-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/visit-1.0.0.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -12,95 +12,95 @@
     enum: [OK, SUSPECT]
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(10)
-      destination: [ScienceCommon.engineering_quality]
+      destination: [ScienceCommon.engineering_quality, GuideWindow.engineering_quality]
   pointing_engdb_quality:
     title: Quality of pointing information from EngDB
     type: string
     enum: [CALCULATED, PLANNED]
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(10)
-      destination: [ScienceCommon.pointing_engdb_quality]
+      destination: [ScienceCommon.pointing_engdb_quality, GuideWindow.pointing_engdb_quality]
   type:
     title: Visit type
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: PSS:dms_visit.visit_type
     archive_catalog:
       datatype: nvarchar(30)
-      destination: [ScienceCommon.visit_type]
+      destination: [ScienceCommon.visit_type, GuideWindow.visit_type]
   start_time:
     title: UTC visit start time
     tag: tag:stsci.edu:asdf/time/time-1.1.0
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: datetime2
-      destination: [ScienceCommon.visit_start_time]
+      destination: [ScienceCommon.visit_start_time, GuideWindow.visit_start_time]
   end_time:
     title: UTC visit end time
     tag: tag:stsci.edu:asdf/time/time-1.1.0
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: datetime2
-      destination: [ScienceCommon.visit_end_time]
+      destination: [ScienceCommon.visit_end_time, GuideWindow.visit_end_time]
   status:
     title: Status of a visit
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(15)
-      destination: [ScienceCommon.visit_status]
+      destination: [ScienceCommon.visit_status, GuideWindow.visit_status]
   total_exposures:
     title: Total number of planned exposures in visit
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [ScienceCommon.visit_total_exposures]
+      destination: [ScienceCommon.visit_total_exposures, GuideWindow.visit_total_exposures]
   internal_target:
     title: At least one exposure in visit is internal
     type: boolean
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nchar(1)
-      destination: [ScienceCommon.visit_internal_target]
+      destination: [ScienceCommon.visit_internal_target, GuideWindow.visit_internal_target]
   target_of_opportunity:
     title: Visit scheduled as target of opportunity
     type: boolean
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nchar(1)
-      destination: [ScienceCommon.target_of_opportunity]
+      destination: [ScienceCommon.target_of_opportunity, GuideWindow.target_of_opportunity]
 propertyOrder: [engineering_quality, pointing_engdb_quality, type,
            start_time, end_time, status, total_exposures, internal_target, target_of_opportunity]
 flowStyle: block
 required: [engineering_quality, pointing_engdb_quality, type,
            start_time, end_time, status, total_exposures, internal_target, target_of_opportunity]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/wcsinfo-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/wcsinfo-1.0.0.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -11,82 +11,82 @@
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.v2_ref]
+      destination: [ScienceCommon.v2_ref, GuideWindow.v2_ref]
   v3_ref:
     title: "[arcsec] Telescope v3 coordinate of the reference point"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.v3_ref]
+      destination: [ScienceCommon.v3_ref, GuideWindow.v3_ref]
   vparity:
     title: Relative sense of rotation between Ideal xy and V2V3
     type: integer
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: int
-      destination: [ScienceCommon.vparity]
+      destination: [ScienceCommon.vparity, GuideWindow.vparity]
   v3yangle:
     title: "[deg] Angle from V3 axis to Ideal y axis"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.v3yangle]
+      destination: [ScienceCommon.v3yangle, GuideWindow.v3yangle]
   ra_ref:
     title: "[deg] Right ascension of the reference point"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.ra_ref]
+      destination: [ScienceCommon.ra_ref, GuideWindow.ra_ref]
   dec_ref:
     title: "[deg] Declination of the reference point"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.dec_ref]
+      destination: [ScienceCommon.dec_ref, GuideWindow.dec_ref]
   roll_ref:
     title: "[deg] V3 roll angle at the ref point (N over E)"
     type: number
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: float
-      destination: [ScienceCommon.roll_ref]
+      destination: [ScienceCommon.roll_ref, GuideWindow.roll_ref]
   s_region:
     title: spatial extent of the observation
     type: string
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(max)
-      destination: [ScienceCommon.s_region]
+      destination: [ScienceCommon.s_region, GuideWindow.s_region]
 propertyOrder: [v2_ref, v3_ref, vparity, v3yangle, ra_ref, dec_ref, roll_ref, s_region]
 flowStyle: block
 required: [v2_ref, v3_ref, vparity, v3yangle, ra_ref, dec_ref, roll_ref, s_region]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/wfi_image-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/wfi_image-1.0.0.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -23,134 +23,114 @@
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 2
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["electron / s"]
   dq:
     tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
     datatype: uint32
     ndim: 2
   err:
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 2
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["electron / s"]
   var_poisson:
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 2
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["electron2 / s2"]
   var_rnoise:
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 2
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["electron2 / s2"]
   var_flat:
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 2
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["electron2 / s2"]
   amp33:
     title: Amp 33 reference pixel data
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: uint16
         ndim: 3
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
   border_ref_pix_left:
     title: Original border reference pixels, on left (from viewers perspective).
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 3
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
   border_ref_pix_right:
     title: Original border reference pixels, on right (from viewers perspective).
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 3
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
   border_ref_pix_top:
     title: Original border reference pixels, on top.
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 3
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
   border_ref_pix_bottom:
     title: Original border reference pixels, on bottom.
     tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
     properties:
       value:
         tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
         datatype: float32
         ndim: 3
       unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
+        tag: tag:astropy.org:astropy/units/unit-1.0.0
         enum: ["DN"]
   dq_border_ref_pix_left:
     title: DQ for border reference pixels, on left (from viewers perspective).
     tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
     datatype: uint32
     ndim: 2
   dq_border_ref_pix_right:
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/wfi_mode-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/wfi_mode-1.0.0.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -14,30 +14,30 @@
     enum: [WFI]
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(5)
-      destination: [ScienceCommon.instrument_name]
+      destination: [ScienceCommon.instrument_name, GuideWindow.instrument_name]
   detector:
     $ref: wfi_detector-1.0.0
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(10)
-      destination: [ScienceCommon.detector]
+      destination: [ScienceCommon.detector, GuideWindow.detector]
   optical_element:
     $ref: wfi_optical_element-1.0.0
     sdf:
       special_processing: VALUE_REQUIRED
       source:
         origin: TBD
     archive_catalog:
       datatype: nvarchar(20)
-      destination: [ScienceCommon.optical_element]
+      destination: [ScienceCommon.optical_element, GuideWindow.optical_element]
 propertyOrder: [detector, optical_element, name]
 flowStyle: block
 required: [detector, optical_element, name]
 ...
```

### Comparing `rad-0.14.2/src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml` & `rad-0.15.0/src/rad/resources/schemas/reference_files/wfi_img_photom-1.0.0.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,63 @@
 %YAML 1.1
 ---
 $schema: asdf://stsci.edu/datamodels/roman/schemas/rad_schema-1.0.0
-id: asdf://stsci.edu/datamodels/roman/schemas/wfi_science_raw-1.0.0
+id: asdf://stsci.edu/datamodels/roman/schemas/reference_files/wfi_img_photom-1.0.0
 
-title: |
-  The schema for Level 1 WFI science data (both imaging and spectrographic).
+title: WFI imaging photometric flux conversion data model
 
 type: object
 properties:
   meta:
     allOf:
-      - $ref: common-1.0.0
-  data:
-    title: Science data, including the border reference pixels.
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: uint16
-        ndim: 3
-      unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["DN"]
-  amp33:
-    title: Amp 33 reference pixel data.
-    tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
-    properties:
-      value:
-        tag: tag:stsci.edu:asdf/core/ndarray-1.0.0
-        datatype: uint16
-        ndim: 3
-      unit:
-        oneOf:
-          - tag: asdf://stsci.edu/datamodels/roman/tags/unit-1.0.0
-          - tag: tag:astropy.org:astropy/units/unit-1.0.0
-        enum: ["DN"]
-propertyOrder: [meta, data, amp33]
+      - $ref: ref_common-1.0.0
+      - type: object
+        properties:
+          reftype:
+            type: string
+            enum: [PHOTOM]
+  phot_table:
+    title: Photometric flux conversion factors table
+    type: object
+    patternProperties:
+      "^(F062|F087|F106|F129|F146|F158|F184|F213|GRISM|PRISM|DARK)$":
+        type: object
+        properties:
+          photmjsr:
+            title: Surface brightness, in MJy/steradian
+            anyOf:
+              - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+                properties:
+                  value:
+                    type: number
+                  unit:
+                    tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+                    enum: [MJy.sr**-1]
+              - type: "null"
+          uncertainty:
+            title: Uncertainty of surface brightness, in MJy/steradian
+            anyOf:
+              - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+                properties:
+                  value:
+                    type: number
+                  unit:
+                    tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+                    enum: [MJy.sr**-1]
+              - type: "null"
+          pixelareasr:
+            title: Nominal pixel area, in steradian
+            anyOf:
+              - tag: tag:stsci.edu:asdf/unit/quantity-1.1.0
+                properties:
+                  value:
+                    type: number
+                  unit:
+                    tag: tag:stsci.edu:asdf/unit/unit-1.0.0
+                    enum: [sr]
+              - type: "null"
+        required: [photmjsr, uncertainty, pixelareasr]
+    additionalProperties: false
+required: [meta, phot_table]
 flowStyle: block
-required: [meta, data, amp33]
+propertyOrder: [meta, phot_table]
 ...
```

### Comparing `rad-0.14.2/src/rad.egg-info/PKG-INFO` & `rad-0.15.0/src/rad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rad
-Version: 0.14.2
+Version: 0.15.0
 Summary: Roman Attribute Dictionary
 Author-email: STScI <help@stsci.edu>
 License: Copyright (C) 2021 Association of Universities for Research in Astronomy (AURA)
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `rad-0.14.2/src/rad.egg-info/SOURCES.txt` & `rad-0.15.0/src/rad.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 tox.ini
 .github/CODEOWNERS
 .github/pull_request_template.md
+.github/workflows/changelog.yml
 .github/workflows/ci.yml
 .github/workflows/ci_cron.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/release.yml
 docs/Makefile
 docs/changes.rst
 docs/conf.py
@@ -54,30 +55,31 @@
 src/rad/resources/schemas/exposure-1.0.0.yaml
 src/rad/resources/schemas/exposure_type-1.0.0.yaml
 src/rad/resources/schemas/guidestar-1.0.0.yaml
 src/rad/resources/schemas/guidewindow-1.0.0.yaml
 src/rad/resources/schemas/guidewindow_modes-1.0.0.yaml
 src/rad/resources/schemas/observation-1.0.0.yaml
 src/rad/resources/schemas/photometry-1.0.0.yaml
-src/rad/resources/schemas/pixelarea-1.0.0.yaml
 src/rad/resources/schemas/pointing-1.0.0.yaml
 src/rad/resources/schemas/program-1.0.0.yaml
 src/rad/resources/schemas/rad_schema-1.0.0.yaml
 src/rad/resources/schemas/ramp-1.0.0.yaml
 src/rad/resources/schemas/ramp_fit_output-1.0.0.yaml
 src/rad/resources/schemas/ref_file-1.0.0.yaml
+src/rad/resources/schemas/resample-1.0.0.yaml
 src/rad/resources/schemas/source_detection-1.0.0.yaml
 src/rad/resources/schemas/target-1.0.0.yaml
 src/rad/resources/schemas/variance-1.0.0.yaml
 src/rad/resources/schemas/velocity_aberration-1.0.0.yaml
 src/rad/resources/schemas/visit-1.0.0.yaml
 src/rad/resources/schemas/wcsinfo-1.0.0.yaml
 src/rad/resources/schemas/wfi_detector-1.0.0.yaml
 src/rad/resources/schemas/wfi_image-1.0.0.yaml
 src/rad/resources/schemas/wfi_mode-1.0.0.yaml
+src/rad/resources/schemas/wfi_mosaic-1.0.0.yaml
 src/rad/resources/schemas/wfi_optical_element-1.0.0.yaml
 src/rad/resources/schemas/wfi_science_raw-1.0.0.yaml
 src/rad/resources/schemas/reference_files/dark-1.0.0.yaml
 src/rad/resources/schemas/reference_files/distortion-1.0.0.yaml
 src/rad/resources/schemas/reference_files/flat-1.0.0.yaml
 src/rad/resources/schemas/reference_files/gain-1.0.0.yaml
 src/rad/resources/schemas/reference_files/inverse_linearity-1.0.0.yaml
@@ -96,12 +98,11 @@
 src/rad/resources/schemas/tagged_scalars/file_date-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/filename-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/model_type-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/origin-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/prd_software_version-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/sdf_software_version-1.0.0.yaml
 src/rad/resources/schemas/tagged_scalars/telescope-1.0.0.yaml
-src/rad/resources/schemas/unit/unit-1.0.0.yaml
 tests/conftest.py
 tests/test_integration.py
 tests/test_manifest.py
 tests/test_schemas.py
```

### Comparing `rad-0.14.2/tests/test_integration.py` & `rad-0.15.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/tests/test_manifest.py` & `rad-0.15.0/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `rad-0.14.2/tests/test_schemas.py` & `rad-0.15.0/tests/test_schemas.py`

 * *Files identical despite different names*

