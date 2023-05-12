# Comparing `tmp/scine_puffin-1.1.0.tar.gz` & `tmp/scine_puffin-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scine_puffin-1.1.0.tar", last modified: Mon Aug  8 19:29:51 2022, max compression
+gzip compressed data, was "dist/scine_puffin-1.2.0.tar", last modified: Thu May 11 06:56:29 2023, max compression
```

## Comparing `scine_puffin-1.1.0.tar` & `scine_puffin-1.2.0.tar`

### file list

```diff
@@ -1,136 +1,137 @@
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/dev/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/dev/conan/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-03-08 10:12:42.000000 scine_puffin-1.1.0/dev/conan/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11187 2022-03-08 10:12:42.000000 scine_puffin-1.1.0/dev/conan/base.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2696 2022-08-08 14:00:29.000000 scine_puffin-1.1.0/dev/conan/utils.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-03-08 10:12:42.000000 scine_puffin-1.1.0/dev/__init__.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/docs/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/docs/source/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      574 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/docs/source/api.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       33 2020-04-20 11:11:38.000000 scine_puffin-1.1.0/docs/source/changelog.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5661 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/docs/source/conf.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      316 2022-04-25 06:06:42.000000 scine_puffin-1.1.0/docs/source/configuration.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      208 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/docs/source/index.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2748 2022-04-25 06:06:42.000000 scine_puffin-1.1.0/docs/source/jobs.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      736 2022-04-25 06:06:42.000000 scine_puffin-1.1.0/docs/source/programs.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       78 2020-04-20 11:11:38.000000 scine_puffin-1.1.0/docs/source/readme.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      673 2020-04-20 11:11:38.000000 scine_puffin-1.1.0/docs/Makefile
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      797 2020-04-20 11:11:38.000000 scine_puffin-1.1.0/docs/make.bat
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin/jobs/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin/jobs/templates/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      201 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/scine_puffin/jobs/templates/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    22753 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/templates/job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    13684 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/templates/scine_connectivity_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3812 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/scine_puffin/jobs/templates/scine_hessian_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    14273 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/templates/scine_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3172 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/templates/scine_observers.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5640 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/templates/scine_optimization_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    69605 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/templates/scine_react_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      201 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/scine_puffin/jobs/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7243 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/conformers.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6276 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/gaussian_charge_model_5.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3749 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/scine_puffin/jobs/graph.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11603 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/kinetx_kinetic_modeling.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    13892 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/orca_geometry_optimization.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5777 2022-03-08 10:12:28.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_afir.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5955 2022-03-08 10:12:28.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_bond_orders.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    13376 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_conceptual_dft.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    26984 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_dissociation_cut.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4095 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_geometry_optimization.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3407 2022-03-08 10:12:28.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_hessian.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5176 2022-03-08 10:12:28.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_irc_scan.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    17582 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_react_complex_afir.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    15632 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_react_complex_nt.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    15714 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_react_complex_nt2.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2803 2022-03-08 10:12:28.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_single_point.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    16553 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_step_refinement.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3922 2022-03-08 10:12:28.000000 scine_puffin-1.1.0/scine_puffin/jobs/scine_ts_optimization.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1479 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/scine_puffin/jobs/sleep.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8237 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/swoose_qmmm_forces.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7072 2022-03-08 10:12:28.000000 scine_puffin-1.1.0/scine_puffin/jobs/turbomole_bond_orders.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11054 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobs/turbomole_geometry_optimization.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8629 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/scine_puffin/jobs/turbomole_hessian.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6944 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/scine_puffin/jobs/turbomole_single_point.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin/programs/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      201 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/scine_puffin/programs/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1046 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/cp2k.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1044 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/database.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1024 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/gaussian.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1036 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/kinetx.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1076 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/molassembler.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1027 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/orca.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5900 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/program.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1066 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/readuct.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1890 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/serenity.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1118 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/sparrow.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1078 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/swoose.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1060 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/turbomole.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1034 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/utils.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1197 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/programs/xtb.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin/tests/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin/tests/cp2k/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-03-08 10:12:28.000000 scine_puffin-1.1.0/scine_puffin/tests/cp2k/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4799 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/cp2k/cp2k_test.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-03-08 10:12:28.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7046 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_conformers.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2118 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_gaussian_cm5_charges_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5074 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_graph.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4618 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_kinetx_kinetic_modeling_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2193 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_orca_geometry_optimization_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3672 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_afir.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5408 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_bond_orders_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8993 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_dissociation_cut_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2726 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_geometry_optimization_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8037 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_hessian.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7621 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_irc_scan_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8797 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_react_complex_afir_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    41919 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_react_complex_nt2_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8489 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_react_complex_nt_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2410 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_single_point_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    17231 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_step_refinement_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2716 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_ts_optimization_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1376 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_sleep_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2718 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_turbomole_bond_orders.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2222 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_turbomole_geometry_optimization_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2309 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_turbomole_hessian.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4180 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/jobs/test_turbomole_single_point_job.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin/tests/resources/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      314 2022-03-08 10:12:28.000000 scine_puffin-1.1.0/scine_puffin/tests/resources/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-03-08 10:12:28.000000 scine_puffin-1.1.0/scine_puffin/tests/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1685 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/daemon_test.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6354 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/db_setup.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6820 2022-03-08 10:12:28.000000 scine_puffin-1.1.0/scine_puffin/tests/masm_info_test.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4977 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/tests/testcases.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin/utilities/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      201 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/scine_puffin/utilities/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1376 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/utilities/compound_and_flask_helpers.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    14155 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/utilities/masm_helper.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11171 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/utilities/program_helper.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1787 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/utilities/properties.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10100 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/scine_puffin/utilities/scine_helper.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    13209 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/utilities/turbomole_helper.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      273 2022-08-02 11:49:10.000000 scine_puffin-1.1.0/scine_puffin/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4619 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/scine_puffin/__main__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      200 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/_version.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3997 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/bootstrap.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    19777 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/config.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3638 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/daemon.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    25290 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/scine_puffin/jobloop.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin.egg-info/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10736 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin.egg-info/PKG-INFO
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4459 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin.egg-info/SOURCES.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin.egg-info/dependency_links.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      380 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin.egg-info/entry_points.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-06-17 11:27:16.000000 scine_puffin-1.1.0/scine_puffin.egg-info/not-zip-safe
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       63 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin.egg-info/requires.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       17 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/scine_puffin.egg-info/top_level.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2101 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/CHANGELOG.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      351 2022-01-28 10:05:45.000000 scine_puffin-1.1.0/MANIFEST.in
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8058 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/README.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       63 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/requirements.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      727 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/setup.cfg
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2907 2022-08-08 18:14:29.000000 scine_puffin-1.1.0/setup.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10736 2022-08-08 19:29:51.000000 scine_puffin-1.1.0/PKG-INFO
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/dev/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/dev/conan/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-03-08 10:12:42.000000 scine_puffin-1.2.0/dev/conan/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11187 2022-03-08 10:12:42.000000 scine_puffin-1.2.0/dev/conan/base.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2696 2022-08-08 14:00:29.000000 scine_puffin-1.2.0/dev/conan/utils.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-03-08 10:12:42.000000 scine_puffin-1.2.0/dev/__init__.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/docs/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/docs/source/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      574 2022-01-28 10:05:45.000000 scine_puffin-1.2.0/docs/source/api.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       33 2020-04-20 11:11:38.000000 scine_puffin-1.2.0/docs/source/changelog.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5661 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/docs/source/conf.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      316 2022-04-25 06:06:42.000000 scine_puffin-1.2.0/docs/source/configuration.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      208 2022-01-28 10:05:45.000000 scine_puffin-1.2.0/docs/source/index.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2748 2022-04-25 06:06:42.000000 scine_puffin-1.2.0/docs/source/jobs.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      736 2022-04-25 06:06:42.000000 scine_puffin-1.2.0/docs/source/programs.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       78 2020-04-20 11:11:38.000000 scine_puffin-1.2.0/docs/source/readme.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      673 2020-04-20 11:11:38.000000 scine_puffin-1.2.0/docs/Makefile
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      797 2020-04-20 11:11:38.000000 scine_puffin-1.2.0/docs/make.bat
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin/jobs/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin/jobs/templates/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      201 2022-01-28 10:05:45.000000 scine_puffin-1.2.0/scine_puffin/jobs/templates/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    23258 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/scine_puffin/jobs/templates/job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    13684 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/jobs/templates/scine_connectivity_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3812 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/jobs/templates/scine_hessian_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    14273 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/jobs/templates/scine_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3172 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/jobs/templates/scine_observers.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5649 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/scine_puffin/jobs/templates/scine_optimization_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    76844 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/scine_puffin/jobs/templates/scine_react_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      201 2022-01-28 10:05:45.000000 scine_puffin-1.2.0/scine_puffin/jobs/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7243 2023-01-31 09:52:24.000000 scine_puffin-1.2.0/scine_puffin/jobs/conformers.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6276 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/jobs/gaussian_charge_model_5.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3749 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/jobs/graph.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    14174 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/scine_puffin/jobs/kinetx_kinetic_modeling.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    13892 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/jobs/orca_geometry_optimization.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5777 2022-03-08 10:12:28.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_afir.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5955 2022-03-08 10:12:28.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_bond_orders.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    26074 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_bspline_optimization.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    13379 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_conceptual_dft.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    26984 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_dissociation_cut.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4095 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_geometry_optimization.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3407 2022-03-08 10:12:28.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_hessian.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5176 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_irc_scan.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    17582 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_react_complex_afir.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    15632 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_react_complex_nt.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    15714 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_react_complex_nt2.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2803 2022-03-08 10:12:28.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_single_point.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    16496 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_step_refinement.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3922 2022-03-08 10:12:28.000000 scine_puffin-1.2.0/scine_puffin/jobs/scine_ts_optimization.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1479 2022-01-28 10:05:45.000000 scine_puffin-1.2.0/scine_puffin/jobs/sleep.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8237 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/jobs/swoose_qmmm_forces.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7072 2022-03-08 10:12:28.000000 scine_puffin-1.2.0/scine_puffin/jobs/turbomole_bond_orders.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11054 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/jobs/turbomole_geometry_optimization.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8629 2022-01-28 10:05:45.000000 scine_puffin-1.2.0/scine_puffin/jobs/turbomole_hessian.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6944 2022-01-28 10:05:45.000000 scine_puffin-1.2.0/scine_puffin/jobs/turbomole_single_point.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin/programs/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      201 2022-01-28 10:05:45.000000 scine_puffin-1.2.0/scine_puffin/programs/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1046 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/cp2k.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1044 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/database.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1024 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/gaussian.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1036 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/kinetx.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1076 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/molassembler.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1027 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/orca.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5900 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/programs/program.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1066 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/readuct.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1890 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/serenity.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1118 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/sparrow.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1078 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/swoose.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1060 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/turbomole.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1034 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/utils.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1197 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/programs/xtb.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin/tests/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin/tests/cp2k/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-03-08 10:12:28.000000 scine_puffin-1.2.0/scine_puffin/tests/cp2k/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4799 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/tests/cp2k/cp2k_test.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-03-08 10:12:28.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7046 2023-01-31 09:52:24.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_conformers.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2118 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_gaussian_cm5_charges_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5074 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_graph.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5665 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_kinetx_kinetic_modeling_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2193 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_orca_geometry_optimization_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3672 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_afir.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5408 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_bond_orders_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8993 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_dissociation_cut_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2726 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_geometry_optimization_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8037 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_hessian.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7621 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_irc_scan_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8797 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_react_complex_afir_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    41919 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_react_complex_nt2_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8489 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_react_complex_nt_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2410 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_single_point_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    17231 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_step_refinement_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2716 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_ts_optimization_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1376 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_sleep_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2718 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_turbomole_bond_orders.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2222 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_turbomole_geometry_optimization_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2309 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_turbomole_hessian.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4180 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/jobs/test_turbomole_single_point_job.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin/tests/resources/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      314 2022-03-08 10:12:28.000000 scine_puffin-1.2.0/scine_puffin/tests/resources/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-03-08 10:12:28.000000 scine_puffin-1.2.0/scine_puffin/tests/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1685 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/tests/daemon_test.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6354 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/db_setup.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6820 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/masm_info_test.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4977 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/tests/testcases.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin/utilities/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      201 2022-01-28 10:05:45.000000 scine_puffin-1.2.0/scine_puffin/utilities/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1376 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/utilities/compound_and_flask_helpers.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    14155 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/utilities/masm_helper.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11171 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/utilities/program_helper.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1787 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/utilities/properties.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10100 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/utilities/scine_helper.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    13209 2022-08-08 18:14:29.000000 scine_puffin-1.2.0/scine_puffin/utilities/turbomole_helper.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      273 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/scine_puffin/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4386 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/scine_puffin/__main__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      200 2023-04-21 18:13:57.000000 scine_puffin-1.2.0/scine_puffin/_version.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4393 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/scine_puffin/bootstrap.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    20580 2023-04-21 18:14:56.000000 scine_puffin-1.2.0/scine_puffin/config.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4637 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/scine_puffin/daemon.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    25533 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/scine_puffin/jobloop.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin.egg-info/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10736 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin.egg-info/PKG-INFO
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4507 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin.egg-info/SOURCES.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin.egg-info/dependency_links.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      380 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin.egg-info/entry_points.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-06-17 11:27:16.000000 scine_puffin-1.2.0/scine_puffin.egg-info/not-zip-safe
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       63 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin.egg-info/requires.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       13 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/scine_puffin.egg-info/top_level.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2396 2023-04-21 18:12:51.000000 scine_puffin-1.2.0/CHANGELOG.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      351 2022-01-28 10:05:45.000000 scine_puffin-1.2.0/MANIFEST.in
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8058 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/README.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       63 2023-04-18 13:15:52.000000 scine_puffin-1.2.0/requirements.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      748 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/setup.cfg
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2984 2023-04-21 18:12:40.000000 scine_puffin-1.2.0/setup.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10736 2023-05-11 06:56:29.000000 scine_puffin-1.2.0/PKG-INFO
```

### Comparing `scine_puffin-1.1.0/dev/conan/base.py` & `scine_puffin-1.2.0/dev/conan/base.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/dev/conan/utils.py` & `scine_puffin-1.2.0/dev/conan/utils.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/docs/source/api.rst` & `scine_puffin-1.2.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/docs/source/conf.py` & `scine_puffin-1.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/docs/source/jobs.rst` & `scine_puffin-1.2.0/docs/source/jobs.rst`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/docs/source/programs.rst` & `scine_puffin-1.2.0/docs/source/programs.rst`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/docs/Makefile` & `scine_puffin-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/docs/make.bat` & `scine_puffin-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/templates/job.py` & `scine_puffin-1.2.0/scine_puffin/jobs/templates/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,17 @@
         with the job's ID. The tarball is then moved to the given destination.
 
         Parameters
         ----------
         archive :: str
             The path to move the resulting tarball to.
         """
+        if not os.path.exists(self.work_dir):
+            sys.stderr.write(f"The job directory {self.work_dir} does not exist, cannot archive.\n")
+            return
         basedir = os.path.dirname(self.work_dir)
         # Tar the folder
         tar_gen_path = os.path.join(basedir, self._id.string() + ".tar.gz")
         tar_archive_path = os.path.join(archive, self._id.string() + ".tar.gz")
         with tarfile.open(tar_gen_path, mode="w:gz") as tar:
             tar.add(self.work_dir, arcname=self._id.string(), recursive=True)
         # Move the tar ball
@@ -144,14 +147,17 @@
             os.makedirs(archive)
         shutil.move(tar_gen_path, tar_archive_path)
 
     def clear(self):
         """
         Clears the directory in which the job was run.
         """
+        if not os.path.exists(self.work_dir):
+            sys.stderr.write(f"The job directory {self.work_dir} does not exist, cannot remove anything.\n")
+            return
         shutil.rmtree(self.work_dir)
 
     def verify_connection(self):
         """
         Verifies the connection to the database.
         Returns only if a connection is established, if it is not, the function
         will attempt to generate a connection every 10 seconds, indefinitely.
@@ -533,19 +539,25 @@
             os.fdopen(original_stderr_fd, "wb"), line_buffering=True
         )
 
     if debug:
         # Do nothing while in debug mode
         prevdir = os.getcwd()
         os.chdir(os.path.expanduser(workdir))
-        with open(job.stdout_path, "w") as stdout, open(job.stderr_path, "w") as stderr:
-            yield
+        try:
+            with open(job.stdout_path, "w") as stdout, open(job.stderr_path, "w") as stderr:
+                yield
+                with open(job.success_file(), "w"):
+                    pass
+            os.chdir(prevdir)
+        except breakable.Break:
             with open(job.success_file(), "w"):
                 pass
-        os.chdir(prevdir)
+            os.chdir(prevdir)
+
     else:
         # Previous directory
         prevdir = os.getcwd()
         # Save a copy of the original stderr fd in saved_stderr_fd
         saved_stderr_fd = os.dup(original_stderr_fd)
         saved_stdout_fd = os.dup(original_stdout_fd)
         # Switch to requested directory
```

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/templates/scine_connectivity_job.py` & `scine_puffin-1.2.0/scine_puffin/jobs/templates/scine_connectivity_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/templates/scine_hessian_job.py` & `scine_puffin-1.2.0/scine_puffin/jobs/templates/scine_hessian_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/templates/scine_job.py` & `scine_puffin-1.2.0/scine_puffin/jobs/templates/scine_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/templates/scine_observers.py` & `scine_puffin-1.2.0/scine_puffin/jobs/templates/scine_observers.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/templates/scine_optimization_job.py` & `scine_puffin-1.2.0/scine_puffin/jobs/templates/scine_optimization_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         label = structure.get_label()
         if label == db.Label.MINIMUM_GUESS or label == db.Label.MINIMUM_OPTIMIZED:
             new_label = db.Label.MINIMUM_OPTIMIZED
         elif label == db.Label.USER_GUESS or label == db.Label.USER_OPTIMIZED:
             new_label = db.Label.USER_OPTIMIZED
         elif label == db.Label.SURFACE_GUESS or label == db.Label.SURFACE_OPTIMIZED:
             new_label = db.Label.SURFACE_OPTIMIZED
-        elif label == db.Label.COMPLEX_GUESS or db.Label.COMPLEX_OPTIMIZED:
+        elif label == db.Label.COMPLEX_GUESS or label == db.Label.COMPLEX_OPTIMIZED:
             new_label = db.Label.COMPLEX_OPTIMIZED
         else:
             error = (
                 "Unknown label '"
                 + str(label)
                 + "' of input structure: '"
                 + str(structure.id())
```

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/templates/scine_react_job.py` & `scine_puffin-1.2.0/scine_puffin/jobs/templates/scine_react_job.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         super().__init__()
         self.name = "ReactJob"  # to be overwritten by child
         self.exploration_key = ""  # to be overwritten by child
         self.own_expected_results = []
         self.rc_key = "rc"
         self.job_key = "job"
         self.rc_opt_system_name = "rcopt"
+        self.single_point_key = "sp"
         # to be extended by child:
         self.settings: Dict[str, Dict[str, Any]] = {
             self.job_key: {
                 "imaginary_wavenumber_threshold": 0.0,
                 "spin_propensity_check": 2,
                 "store_full_mep": False,
                 "store_all_structures": False,
@@ -51,16 +52,30 @@
                 "displacement": 0.0,
             },
             self.rc_opt_system_name: {
                 "output": [self.rc_opt_system_name],
                 "stop_on_error": False,
                 "convergence_max_iterations": 500,
                 "geoopt_coordinate_system": "cartesianWithoutRotTrans",
+            },
+            self.single_point_key: {
+                "expect_charge_separation": False,
+                "charge_separation_threshold": 0.4
             }
         }
+        """
+        expect_charge_separation : If true, fragment charges are no longer determined by rounding, i.e, if a product
+        consists of multiple molecules (according to its graph), the charges are determined initially by rounding.
+        However, then the residual (the difference of the integrated charge to the rounded one) is checked against
+        <charge_separation_threshold>. If this residual exceeds the charge separation threshold, the charge is
+        increased/lowered by one according to its sign. This is especially useful if a clear charge separation only
+        occurs upon separation of the molecules which is often the case for DFT-based descriptions of the electronic
+        structure.
+        charge_separation_threshold : The threshold for the charge separation (vide supra).
+        """
         self.start_graph = ""
         self.end_graph = ""
         self.start_charges = []
         self.start_multiplicities = []
         self.start_decision_lists = []
         self.ref_structure = None
         self.step_direction = None
@@ -580,15 +595,15 @@
         name :: str
             Index into systems dictionary to calculate bond orders for
         total_charge :: str
             The charge of the system
 
         Returns
         -------
-        split_structures :: List[utils.AtomCollection]
+        ordered_structures :: List[utils.AtomCollection]
             List of atom collections corresponding to the split molecules.
         graph_string :: str
             Sorted molassembler cbor graphs separated by semicolons.
         charges :: List[int]
             Charges of the molecules.
         multiplicities :: List[int]
             Minimal multiplicities of the molecules.
@@ -626,43 +641,16 @@
             )
             self.throw_if_not_successful(
                 success, self.systems, [name], ["energy", "atomic_charges"]
             )
             partial_charges = self.systems[name].get_results().atomic_charges
             self.systems[name].get_results().bond_orders = bond_orders
 
-        charges = []
-        n_electrons = []
-        for i in range(len(split_structures)):
-            charges.append(0.0)
-        for i, c in zip(masm_results.component_map, partial_charges):
-            charges[i] += c
-        residual = []
-        for i in range(len(split_structures)):
-            residual.append(charges[i] - round(charges[i]))
-            charges[i] = int(round(charges[i]))
-
-        # Check if electrons were created or vanished by virtue of rounding
-        electron_diff = int(round(sum(charges) - total_charge))
-        if electron_diff < 0:
-            # Remove electrons if need be
-            max_charge_vals = np.array(charges).argsort()[-electron_diff:]
-            for i in max_charge_vals:
-                charges[i] += 1
-        elif electron_diff > 0:
-            # Add electrons if need be
-            min_charge_vals = np.array(charges).argsort()[:electron_diff]
-            for i in min_charge_vals:
-                charges[i] -= 1
-        for i in range(len(split_structures)):
-            electrons = 0.0
-            for elem in split_structures[i].elements:
-                electrons += utils.ElementInfo.Z(elem)
-            electrons -= charges[i]
-            n_electrons.append(int(round(electrons)))
+        charges, n_electrons, _ = self._integrate_charges(masm_results.component_map, partial_charges,
+                                                          split_structures, total_charge)
 
         # This assumes minimal multiplicity, product multiplicities are again checked later around this multiplicity
         multiplicities = [nel % 2 + 1 for nel in n_electrons]
 
         # Sort everything according to graphs and if these are equal according to charges and then multiplicities
         graphs, charges, multiplicities, decision_lists, structure_order = (
             list(start_val)
@@ -675,14 +663,162 @@
         )
         graph_string = ";".join(graphs)
 
         ordered_structures = [split_structures[i] for i in structure_order]
 
         return ordered_structures, graph_string, charges, multiplicities, decision_lists
 
+    @staticmethod
+    def _custom_round(number: float, threshold=0.5) -> float:
+        """
+        Rounding number up or down depending on the threshold.
+        To round down, delta must be smaller than the threshold.
+
+        Parameters
+        ----------
+        number : float
+            Number which should be rounded.
+        threshold : float, optional
+            Threshold when to round up, by default 0.5
+
+        Returns
+        -------
+        float
+            Number rounded according to threshold.
+        """
+        sign = np.copysign(1.0, number)
+        number = abs(number)
+        delta = number - np.trunc(number)
+        if delta < threshold:
+            return np.trunc(number) * sign
+        else:
+            return (np.trunc(number) + 1) * sign
+
+    @staticmethod
+    def _calculate_residual(original_values: List[Any], new_values: List[Any]) -> List[float]:
+        """
+        Calculate the residual where one subtracts new from old values.
+
+        Parameters
+        ----------
+        original_values : List[float]
+            A list of old values.
+        new_values : List[float]
+            A list of new values.
+
+        Returns
+        -------
+        residual : List[float]
+            The list of differences between old and new.
+        """
+        residual = []
+        for i in range(len(original_values)):
+            residual.append(original_values[i] - new_values[i])
+        return residual
+
+    def _distribute_charge(
+            self,
+            total_charge: float,
+            charge_guess,
+            summed_partial_charges: List[float]) -> List[int]:
+        """
+        Check if the sum of the charges of the non-bonded molecules equals the total charge of the supersystem.
+        If this should not be the case, add or remove one charge, depending on the difference between the total charge
+        and the sum of the charge guess.
+        A charge is added where the residual between the partial charges and the charge guess (partial - guess)
+        is maximal and subtracted where it is minimal.
+        The re-evaluated after the charge guess was modified.
+
+        Parameters
+        ----------
+        total_charge : float
+            Total charge of the supersystem.
+        charge_guess : List[int]
+            List of guessed charges for each molecule in the supersystem.
+        summed_partial_charges : List[float]
+            List of the sum over the partial charges of the non-bonded molecules in the supersystem.
+
+        Returns
+        -------
+            charge_guess : List[float]
+                The updated list of guessed charges where the sum equals the total charge of the supersystem.
+        """
+        residual = self._calculate_residual(summed_partial_charges, charge_guess)
+        while (sum(charge_guess) != total_charge):
+            charge_diff = sum(charge_guess) - total_charge
+            # too many electrons, add a charge
+            if charge_diff < 0.0:
+                # Add one charge to selection
+                charge_guess[np.argmax(residual)] += 1
+            # too little electrons, remove a charge
+            else:
+                # Substract one charge from selection
+                charge_guess[np.argmin(residual)] -= 1
+            # Update residual
+            residual = self._calculate_residual(summed_partial_charges, charge_guess)
+        # return updated charge guess
+        return charge_guess
+
+    def _integrate_charges(self, component_map: List[int], partial_charges: List[float],
+                           split_structures, total_charge: float) -> Tuple[List[int], List[int], List[float]]:
+        """
+        Determine the charges, the number of electrons and the residual to the partial charges per molecule of
+        the non-bonded molecules in the supersystem.
+
+        Parameters
+        ----------
+        component_map : List[int]
+            List of indices to map atoms to the molecule it belongs according to molassembler.
+        partial_charges : List[float]
+            The partial charges of the atoms.
+        split_structures : List[utils.AtomCollection]
+            The non-bonded molecules in the supersystem.
+        total_charge : List[utils.AtomCollection]
+            The total charge of the supersystem.
+
+        Returns
+        -------
+        charges : List[int]
+            The charges for each non-bonded molecule in the supersystem.
+        n_electrons : List[int]
+            The number of electrons for each non-bonded molecule in the supersystem.
+        residual : List[float]
+            The difference between the original sum of partial charges and
+            the determined charges per non-bonded molecule in the supersystem.
+
+        """
+        import scine_utilities as utils
+        charges = []
+        n_electrons = []
+        for i in range(len(split_structures)):
+            charges.append(0.0)
+        for i, c in zip(component_map, partial_charges):
+            charges[i] += c
+        summed_partial_charges = deepcopy(charges)
+        print("Charge separation check " + str(self.settings[self.single_point_key]["expect_charge_separation"]))
+        # Update charges to charge guess, only containing ints
+        for i in range(len(split_structures)):
+            if not self.settings[self.single_point_key]["expect_charge_separation"]:
+                charges[i] = int(self._custom_round(charges[i], 0.5))
+            else:
+                charges[i] = int(self._custom_round(charges[i],
+                                 self.settings[self.single_point_key]["charge_separation_threshold"]))
+
+        # Check and re-distribute if necessary
+        updated_charges = self._distribute_charge(total_charge, charges, summed_partial_charges)
+        # Update number of electrons
+        for i in range(len(split_structures)):
+            electrons = 0
+            for elem in split_structures[i].elements:
+                electrons += utils.ElementInfo.Z(elem)
+            electrons -= updated_charges[i]
+            n_electrons.append(int(round(electrons)))
+        residual = self._calculate_residual(summed_partial_charges, updated_charges)
+        return updated_charges, n_electrons, residual
+
     def check_for_barrierless_reaction(self):
         """
         Optimizes the reactive complex, comparing the result to the start
         structures determining if a barrierless reaction occurred.
 
         Returns
         -------
@@ -806,14 +942,17 @@
             backward_structures,
             backward_graph,
             backward_charges,
             backward_multiplicities,
             backward_decision_lists,
         ) = self.get_graph_charges_multiplicities(inputs[1], initial_charge)
 
+        print("Forward charges: " + str(forward_charges))
+        print("Backward charges: " + str(backward_charges))
+
         # Optimize separated forward molecules
         forward_names = self.optimize_structures("forward", forward_structures,
                                                  forward_charges,
                                                  forward_multiplicities,
                                                  calculator_settings)
         # Optimize separated backward molecules
         backward_names = self.optimize_structures("backward", backward_structures,
@@ -915,29 +1054,26 @@
 
         # Compare decision lists of start structures:
         original_decision_lists = self.start_decision_lists
         if self.step_direction == "backward":
             new_decision_lists = forward_decision_lists
         else:
             new_decision_lists = backward_decision_lists
-
         decision_lists_match: bool = True
         for new, orig in zip(new_decision_lists, original_decision_lists):
             if not masm.JsonSerialization.equal_decision_lists(new, orig):
                 decision_lists_match = False
                 break
-
         if not decision_lists_match:
             if self.step_direction == "backward":
                 start_names = forward_names
             else:
                 start_names = backward_names
         else:
             start_names = None
-
         # additional check for double ended methods
         if self.end_graph:
             if (
                 masm.JsonSerialization.equal_molecules(forward_graph, self.start_graph)
                 and masm.JsonSerialization.equal_molecules(backward_graph, self.end_graph)
                 and (not check_charges or forward_charges == self.start_charges)
             ):
@@ -947,15 +1083,14 @@
                 and masm.JsonSerialization.equal_molecules(backward_graph, self.start_graph)
                 and (not check_charges or backward_charges == self.start_charges)
             ):
                 product_names = forward_names
             else:
                 self._calculation.set_comment(self.name + ": IRC does not match double ended method")
                 return None, None
-
         # Check if complexations need to be tracked
         forward_complexation_energy = 0.0
         for name in forward_names:
             forward_complexation_energy -= self.systems[name].get_results().energy
         forward_complexation_energy += self.systems[inputs[0]].get_results().energy
         if forward_complexation_energy < self.complexation_criterion:
             if self.step_direction == "backward":
@@ -967,15 +1102,14 @@
             backward_complexation_energy -= self.systems[name].get_results().energy
         backward_complexation_energy += self.systems[inputs[1]].get_results().energy
         if backward_complexation_energy < self.complexation_criterion:
             if self.step_direction == "backward":
                 self.rhs_complexation = True
             else:
                 self.lhs_complexation = True
-
         return product_names, start_names
 
     def optimize_structures(
         self,
         name_stub: str,
         structures,
         structure_charges: List[int],
@@ -1032,15 +1166,15 @@
                 # generate calculator
                 new = utils.core.load_system_into_calculator(
                     name + ".xyz",
                     self._calculation.get_model().method_family,
                     **structure_calculator_settings,
                 )
                 self.systems[name] = new
-            except BaseException as e:
+            except RuntimeError as e:
                 if stop_on_error:
                     raise e
                 sys.stderr.write(f"{name} cannot be calculated because: {str(e)}")
                 self.systems[name] = None
 
         print("Product Opt Settings:")
         print(self.settings["opt"], "\n")
@@ -1076,15 +1210,15 @@
                 self.throw_if_not_successful(
                     success,
                     self.systems,
                     [structure],
                     ["energy", "bond_orders"],
                     f"{name_stub.capitalize()} optimization failed:\n",
                 )
-            except BaseException as e:
+            except RuntimeError as e:
                 if stop_on_error:
                     raise e
                 sys.stderr.write(f"{structure} cannot be calculated because: {str(e)}")
                 self.systems[structure] = None
         return structure_names
 
     def generate_spline(
@@ -1151,36 +1285,36 @@
             self.work_dir, f"irc_{rev_dir}", f"irc_{rev_dir}.irc.{rev_dir}.trj.xyz"
         )
         if os.path.isfile(fpath):
             trj, energies = read_trj(fpath)
             for pos, e in zip(reversed(trj), reversed(energies)):
                 rpi.append_structure(utils.AtomCollection(trj.elements, pos), e)
         else:
-            raise Exception(
+            raise RuntimeError(
                 f"Missing IRC trajectory file: irc_{rev_dir}/irc_{rev_dir}.irc.{rev_dir}.trj.xyz"
             )
 
         fpath = os.path.join(self.work_dir, "ts", "ts.xyz")
         if os.path.isfile(fpath):
             ts_calc = self.systems[self.output(tsopt_task_name)[0]]
             results = ts_calc.get_results()
             ts_xyz, _ = utils.io.read(fpath)
             rpi.append_structure(ts_xyz, results.energy, True)
         else:
-            raise Exception("Missing TS structure file: ts/ts.xyz")
+            raise RuntimeError("Missing TS structure file: ts/ts.xyz")
 
         fpath = os.path.join(
             self.work_dir, f"irc_{dir}", f"irc_{dir}.irc.{dir}.trj.xyz"
         )
         if os.path.isfile(fpath):
             trj, energies = read_trj(fpath)
             for pos, e in zip(trj, energies):
                 rpi.append_structure(utils.AtomCollection(trj.elements, pos), e)
         else:
-            raise Exception(
+            raise RuntimeError(
                 f"Missing IRC trajectory file: irc_{dir}/irc_{dir}.irc.{dir}.trj.xyz"
             )
 
         fpath = os.path.join(self.work_dir, f"irc_{dir}", f"irc_{dir}.opt.trj.xyz")
         if os.path.isfile(fpath):
             trj, energies = read_trj(fpath)
             for pos, e in zip(trj, energies):
@@ -1190,15 +1324,16 @@
         spline = rpi.spline(n_fit_points, degree)
         return spline
 
     def store_start_structures(
         self,
         start_structure_names: List[str],
         program_helper: Union[ProgramHelper, None],
-        tsopt_task_name: str
+        tsopt_task_name: str,
+        start_structures: Optional[List[Any]] = None
     ):
         """
         Store the new start systems system in the database.
 
         Notes
         -----
         * May throw exception
@@ -1207,36 +1342,42 @@
         ----------
         start_structure_names :: List[str]
             The names of the start structure names in the system map.
         program_helper :: Union[ProgramHelper, None]
             The ProgramHelper which might also want to do postprocessing
         tsopt_task_name :: str
             The name of the task where the TS was output
+        start_structures :: Optional[List[db.ID]]
+            Optional list of the starting structure ids. If no list is given. The input
+            structures of the calculation are used.
 
         Returns
         -------
         start_structure_ids :: List[scine_database.ID]
             A list of the database IDs of the start structures.
         """
         import scine_database as db
 
+        if start_structures is None:
+            start_structures = self._calculation.get_structures()
+
         # Update model to make sure there are no 'any' values left
         update_model(
             self.systems[self.output(tsopt_task_name)[0]],
             self._calculation,
             self.config,
         )
 
         start_structure_ids = []
         for name in start_structure_names:
             # Check if the new structures are actually duplicates
             duplicate: Optional[db.ID] = None
             dl = ';'.join(self.make_decision_lists_from_calc(self.systems, name))
             graph = self.make_graph_from_calc(self.systems, name)
-            for initial_id in self._calculation.get_structures():
+            for initial_id in start_structures:
                 initial_structure = db.Structure(initial_id)
                 initial_structure.link(self._structures)
                 initial_graph = initial_structure.get_graph("masm_cbor_graph")
                 if not masm.JsonSerialization.equal_molecules(initial_graph, graph):
                     continue
                 aggregate_id = initial_structure.get_aggregate()
                 if ';' in initial_graph:
@@ -1245,17 +1386,23 @@
                 else:
                     aggregate = db.Compound(aggregate_id)
                     aggregate.link(self._compounds)
                 existing_structures = aggregate.get_structures()
                 for existing_structure_id in existing_structures:
                     existing_structure = db.Structure(existing_structure_id)
                     existing_structure.link(self._structures)
+                    if existing_structure.get_label() in \
+                            [db.Label.DUPLICATE, db.Label.MINIMUM_GUESS, db.Label.USER_GUESS]:
+                        continue
                     existing_structure_dl = existing_structure.get_graph("masm_decision_list")
                     if masm.JsonSerialization.equal_decision_lists(dl, existing_structure_dl):
                         duplicate = existing_structure_id
+                        break
+                if duplicate is not None:
+                    break
             if duplicate is not None:
                 start_structure_ids.append(duplicate)
                 continue
 
             new_structure = self.create_new_structure(self.systems[name], db.Label.MINIMUM_OPTIMIZED)
             self.transfer_properties(self.ref_structure, new_structure)
             self.store_energy(self.systems[name], new_structure)
@@ -1487,28 +1634,36 @@
         for rid in reactant_structur_ids:
             if rid not in original_start_structures:
                 # TODO should duplicates be removed here?
                 db_results.add_structure(rid)
         # intermediate function may have written directly to calculation
         #   results, therefore add to already existing
         self._calculation.set_results(self._calculation.get_results() + db_results)
+        return main_step_lhs, main_step_rhs
 
     def save_mep_in_db(self, elementary_step, charge, multiplicity, model):
         """
         Store each point on the MEP as a structure in the database.
         Attaches `electronic_energy` properties for each point.
 
         Notes
         -----
         * May throw exception
 
         Parameters
         ----------
-        tsopt_task_name :: str
-            Name of the transition state task.
+        elementary_step :: scine_database.ElementaryStep
+            The elementary step of which to store the MEP.
+        charge :: int
+            The total charge of the system.
+        multiplicity :: int
+            The spin multiplicity of the system.
+        model :: scine_database.Model
+            The model with which all energies in the elementary Step were
+            calculated.
         """
         import scine_utilities as utils
         import scine_database as db
         import os
 
         def read_trj(fname):
             trj = utils.io.read_trajectory(utils.io.TrajectoryFormat.Xyz, fname)
@@ -1559,30 +1714,30 @@
         )
         if os.path.isfile(fpath):
             trj, _ = read_trj(fpath)
             for pos in reversed(trj):
                 sid = generate_structure(utils.AtomCollection(trj.elements, pos), charge, multiplicity, model)
                 structure_ids.append(sid)
         else:
-            raise Exception(
+            raise RuntimeError(
                 f"Missing IRC trajectory file: irc_{rev_dir}/irc_{rev_dir}.irc.{rev_dir}.trj.xyz"
             )
 
         structure_ids.append(elementary_step.get_transition_state())
 
         fpath = os.path.join(
             self.work_dir, f"irc_{dir}", f"irc_{dir}.irc.{dir}.trj.xyz"
         )
         if os.path.isfile(fpath):
             trj, _ = read_trj(fpath)
             for pos in trj:
                 sid = generate_structure(utils.AtomCollection(trj.elements, pos), charge, multiplicity, model)
                 structure_ids.append(sid)
         else:
-            raise Exception(
+            raise RuntimeError(
                 f"Missing IRC trajectory file: irc_{dir}/irc_{dir}.irc.{dir}.trj.xyz"
             )
 
         fpath = os.path.join(self.work_dir, f"irc_{dir}", f"irc_{dir}.opt.trj.xyz")
         if os.path.isfile(fpath):
             trj, _ = read_trj(fpath)
             for pos in trj:
```

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/conformers.py` & `scine_puffin-1.2.0/scine_puffin/jobs/conformers.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/gaussian_charge_model_5.py` & `scine_puffin-1.2.0/scine_puffin/jobs/gaussian_charge_model_5.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/graph.py` & `scine_puffin-1.2.0/scine_puffin/jobs/graph.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/kinetx_kinetic_modeling.py` & `scine_puffin-1.2.0/scine_puffin/jobs/kinetx_kinetic_modeling.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 from typing import List
+import numpy as np
 
 import scine_database as db
 
 from .templates.job import Job, breakable, calculation_context, job_configuration_wrapper
 from ..utilities.compound_and_flask_helpers import get_compound_or_flask
 from scine_puffin.config import Configuration
 
@@ -72,15 +73,16 @@
         self.settings = {
             "energy_label": "electronic_energy",
             "time_step": 1e-8,
             "solver": "cash_karp_5",
             "batch_interval": 1000,
             "n_batches": 1000,
             "convergence": 1e-10,
-            "energy_model_program": "any"
+            "energy_model_program": "any",
+            "concentration_label_postfix": ""
         }
         self.model = db.Model("PM6", "PM6", "")
         self._flask_decomposition = dict()
 
     @job_configuration_wrapper
     def run(self, manager, calculation, config: Configuration) -> bool:
         import scine_kinetx as kinetx
@@ -93,70 +95,108 @@
             lhs_rates_per_reaction = self.settings["lhs_rates"]
             rhs_rates_per_reaction = self.settings["rhs_rates"]
             concentrations = self.settings["start_concentrations"]
             self.model = calculation.get_model()
             n_reactions = len(reaction_ids)
             n_aggregates = len(aggregate_id_list)
             if len(reaction_ids) != len(lhs_rates_per_reaction) or len(reaction_ids) != len(rhs_rates_per_reaction):
-                raise Exception("The number of reaction rates differs from the number of reactions.")
+                raise RuntimeError("The number of reaction rates differs from the number of reactions.")
             network_builder = kinetx.NetworkBuilder()
             # Prepare the data arrays / network
             network_builder.reserve(n_compounds=n_aggregates, n_reactions=n_reactions, n_channels_per_reaction=1)
             # Add compounds and reactions
             self._add_all_aggregates(aggregate_id_list, aggregate_type_list, network_builder)
             self._add_all_reactions(reaction_ids, network_builder, aggregate_id_list, lhs_rates_per_reaction,
                                     rhs_rates_per_reaction, aggregate_type_list)
             network = network_builder.generate()
             # Solve network
             time_step = self.settings["time_step"]
             solver = kinetx.get_integrator(self.settings["solver"])
             batch_interval = self.settings["batch_interval"]
             n_batches = self.settings["n_batches"]
             convergence = self.settings["convergence"]
-            concentration_data = kinetx.integrate(network, concentrations, 0.0, time_step, solver,
-                                                  batch_interval, n_batches, convergence)
+            if "max_time" in self.settings:
+                concentration_data, reaction_flux, reaction_flux_forward, reaction_flux_backward = kinetx.integrate(
+                    network, concentrations, 0.0, time_step, solver, batch_interval, n_batches, convergence, True,
+                    self.settings["max_time"])
+            else:
+                concentration_data, reaction_flux, reaction_flux_forward, reaction_flux_backward = kinetx.integrate(
+                    network, concentrations, 0.0, time_step, solver, batch_interval, n_batches, convergence)
             # Save the concentrations
             results = calculation.get_results()
-            self._write_concentrations_to_centroids(aggregate_id_list, aggregate_type_list, concentration_data, manager,
-                                                    results)
+            self._write_concentrations_to_centroids(aggregate_id_list, aggregate_type_list, concentration_data,
+                                                    reaction_flux, reaction_flux_forward, reaction_flux_backward,
+                                                    reaction_ids, manager, results)
             calculation.set_results(results)
             self._disable_all_aggregates()
             self.complete_job()
 
         return self.postprocess_calculation_context()
 
-    def _write_concentrations_to_centroids(self, aggregate_id_list, aggregate_type_list, concentration_data, manager,
-                                           results) -> None:
+    def _resolve_flask_to_compound_mapping(self, concentration_data, aggregate_id_list,
+                                           aggregate_type_list):
+        i = 0
+        new_concentration_data = np.copy(concentration_data)
+        for a_id, a_type in zip(aggregate_id_list, aggregate_type_list):
+            if a_type == db.CompoundOrFlask.FLASK:
+                flask = db.Flask(a_id, self._flasks)
+                compounds_in_flask = flask.get_compounds()
+                for c_id in compounds_in_flask:
+                    if c_id in aggregate_id_list:
+                        j = aggregate_id_list.index(c_id)
+                        new_concentration_data[j, :] += concentration_data[i, :]
+            i += 1
+        return new_concentration_data
+
+    def _write_concentrations_to_centroids(self, aggregate_id_list, aggregate_type_list, original_concentration_data,
+                                           total_reaction_flux, forward_reaction_flux, backward_reaction_flux,
+                                           reaction_ids, manager, results) -> None:
         """
         Write the final and maximum concentrations to the centroids of each compound.
         """
         self.model.program = self.settings["energy_model_program"]
+        concentration_data = self._resolve_flask_to_compound_mapping(original_concentration_data, aggregate_id_list,
+                                                                     aggregate_type_list)
         i = 0
+        post_fix = self.settings["concentration_label_postfix"]
+        print(post_fix)
         for a_id, a_type in zip(aggregate_id_list, aggregate_type_list):
             aggregate = get_compound_or_flask(a_id, a_type, self._compounds, self._flasks)
             centroid = aggregate.get_centroid(manager)
             flux_c = concentration_data[i, 2]
             max_c = concentration_data[i, 1]
             final_c = concentration_data[i, 0]
-            max_concentration_property = db.NumberProperty.make("max_concentration", self.model,
-                                                                max_c, self._properties)
-            final_concentration_property = db.NumberProperty.make("final_concentration", self.model,
-                                                                  final_c, self._properties)
-            concentration_flux_property = db.NumberProperty.make("concentration_flux", self.model,
-                                                                 flux_c, self._properties)
-            results.add_property(max_concentration_property.id())
-            results.add_property(final_concentration_property.id())
-            results.add_property(concentration_flux_property.id())
-            centroid.add_property("max_concentration", max_concentration_property.id())
-            centroid.add_property("final_concentration", final_concentration_property.id())
-            centroid.add_property("concentration_flux", concentration_flux_property.id())
-            max_concentration_property.set_structure(centroid.id())
-            final_concentration_property.set_structure(centroid.id())
-            concentration_flux_property.set_structure(centroid.id())
+            max_concentration_label = "max_concentration" + post_fix
+            final_concentration_label = "final_concentration" + post_fix
+            concentration_flux_label = "concentration_flux" + post_fix
+            self._write_concentration_property(centroid, max_concentration_label, max_c, results)
+            self._write_concentration_property(centroid, final_concentration_label, final_c, results)
+            self._write_concentration_property(centroid, concentration_flux_label, flux_c, results)
             i += 1
+        # Save edge flux (for the time being I will save it as a property to the centroid of the first LHS aggregate).
+        for i, r_id in enumerate(reaction_ids):
+            r_flux_total = total_reaction_flux[i, 0]
+            r_flux_forward = forward_reaction_flux[i, 0]
+            r_flux_backward = backward_reaction_flux[i, 0]
+            total_flux_label = r_id.string() + "_reaction_edge_flux" + post_fix
+            forward_flux_label = r_id.string() + "_forward_edge_flux" + post_fix
+            backward_flux_label = r_id.string() + "_backward_edge_flux" + post_fix
+            a_id = db.Reaction(r_id, self._reactions).get_reactants(db.Side.LHS)[0][0]
+            a_type = db.Reaction(r_id, self._reactions).get_reactant_types(db.Side.LHS)[0][0]
+            aggregate = get_compound_or_flask(a_id, a_type, self._compounds, self._flasks)
+            centroid = aggregate.get_centroid(manager)
+            self._write_concentration_property(centroid, total_flux_label, r_flux_total, results)
+            self._write_concentration_property(centroid, forward_flux_label, r_flux_forward, results)
+            self._write_concentration_property(centroid, backward_flux_label, r_flux_backward, results)
+
+    def _write_concentration_property(self, centroid: db.Structure, label: str, value: float, results: db.Results):
+        prop = db.NumberProperty.make(label, self.model, value, self._properties)
+        results.add_property(prop.id())
+        centroid.add_property(label, prop.id())
+        prop.set_structure(centroid.id())
 
     def _add_all_aggregates(self, aggregate_id_list: List[db.ID], aggregate_type_list: List[db.CompoundOrFlask],
                             network_builder) -> None:
         """
         Add all aggregates to the kinetic model.
         """
         for a_id, a_type in zip(aggregate_id_list, aggregate_type_list):
@@ -214,15 +254,15 @@
         for a_index, n in rhs_stoichiometry:
             a_id = aggregate_id_list[a_index]
             a_type = aggregate_type_list[a_index]
             aggregate = get_compound_or_flask(a_id, a_type, self._compounds, self._flasks)
             centroid = aggregate.get_centroid()
             rhs_mass += n * self._calculate_weight(centroid)
         if abs(rhs_mass - lhs_mass) > 1e-6:
-            raise Exception("Unbalanced masses in reaction. You are destroying/creating atoms!")
+            raise RuntimeError("Unbalanced masses in reaction. You are destroying/creating atoms!")
 
     def _disable_all_aggregates(self):
         """
         Disable the exploration of all aggregates.
         """
         for compound in self._compounds.iterate_all_compounds():
             compound.link(self._compounds)
```

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/orca_geometry_optimization.py` & `scine_puffin-1.2.0/scine_puffin/jobs/orca_geometry_optimization.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_afir.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_afir.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_bond_orders.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_bond_orders.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_conceptual_dft.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_conceptual_dft.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
             # Check that N is >= 1 s.t. N-1 is >= 0
             n_electrons = 0
             elements = structure.get_atoms().elements
             for element in elements:
                 n_electrons += utils.ElementInfo.Z(element)
             if charge >= n_electrons:
-                raise Exception("At least one electron required to calculate cDFT properties.")
+                raise RuntimeError("At least one electron required to calculate cDFT properties.")
 
             charge_plus = charge - 1
             charge_minus = charge + 1
 
             if "spin_multiplicity_plus" in calculation_settings:
                 multiplicity_plus = calculation_settings["spin_multiplicity_plus"]
                 del calculation_settings["spin_multiplicity_plus"]
```

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_dissociation_cut.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_dissociation_cut.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_geometry_optimization.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_geometry_optimization.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_hessian.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_hessian.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_irc_scan.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_irc_scan.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_react_complex_afir.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_react_complex_afir.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_react_complex_nt.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_react_complex_nt.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_react_complex_nt2.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_react_complex_nt2.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_single_point.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_single_point.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_step_refinement.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_step_refinement.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,14 @@
             self.sort_settings(settings_manager.task_settings)
             """ TSOPT JOB """
             ts_guess, keys = settings_manager.prepare_readuct_task(ts_struc,
                                                                    self._calculation,
                                                                    self._calculation.get_settings(),
                                                                    config["resources"])
             self.systems[keys[0]] = ts_guess[keys[0]]
-            self.setup_automatic_mode_selection("tsopt")
             print("TSOpt Settings:")
             print(self.settings["tsopt"], "\n")
             self.systems, success = self.observed_readuct_call(
                 'run_tsopt_task', self.systems, keys, **self.settings["tsopt"])
             self.throw_if_not_successful(
                 success,
                 self.systems,
```

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/scine_ts_optimization.py` & `scine_puffin-1.2.0/scine_puffin/jobs/scine_ts_optimization.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/sleep.py` & `scine_puffin-1.2.0/scine_puffin/jobs/sleep.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/swoose_qmmm_forces.py` & `scine_puffin-1.2.0/scine_puffin/jobs/swoose_qmmm_forces.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/turbomole_bond_orders.py` & `scine_puffin-1.2.0/scine_puffin/jobs/turbomole_bond_orders.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/turbomole_geometry_optimization.py` & `scine_puffin-1.2.0/scine_puffin/jobs/turbomole_geometry_optimization.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/turbomole_hessian.py` & `scine_puffin-1.2.0/scine_puffin/jobs/turbomole_hessian.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/jobs/turbomole_single_point.py` & `scine_puffin-1.2.0/scine_puffin/jobs/turbomole_single_point.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/cp2k.py` & `scine_puffin-1.2.0/scine_puffin/programs/cp2k.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/database.py` & `scine_puffin-1.2.0/scine_puffin/programs/database.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/gaussian.py` & `scine_puffin-1.2.0/scine_puffin/programs/gaussian.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/kinetx.py` & `scine_puffin-1.2.0/scine_puffin/programs/kinetx.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/molassembler.py` & `scine_puffin-1.2.0/scine_puffin/programs/molassembler.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/orca.py` & `scine_puffin-1.2.0/scine_puffin/programs/orca.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/program.py` & `scine_puffin-1.2.0/scine_puffin/programs/program.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/readuct.py` & `scine_puffin-1.2.0/scine_puffin/programs/readuct.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/serenity.py` & `scine_puffin-1.2.0/scine_puffin/programs/serenity.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/sparrow.py` & `scine_puffin-1.2.0/scine_puffin/programs/sparrow.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/swoose.py` & `scine_puffin-1.2.0/scine_puffin/programs/swoose.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/turbomole.py` & `scine_puffin-1.2.0/scine_puffin/programs/turbomole.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/utils.py` & `scine_puffin-1.2.0/scine_puffin/programs/utils.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/programs/xtb.py` & `scine_puffin-1.2.0/scine_puffin/programs/xtb.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/cp2k/cp2k_test.py` & `scine_puffin-1.2.0/scine_puffin/tests/cp2k/cp2k_test.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_conformers.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_conformers.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_gaussian_cm5_charges_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_gaussian_cm5_charges_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_graph.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_graph.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_kinetx_kinetic_modeling_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_turbomole_single_point_job.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,111 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
-from json import dumps
+import os
 
 from ..testcases import (
     JobTestCase,
     skip_without
 )
 
 from ..db_setup import (
     add_calculation,
-    add_compound_and_structure,
-    add_reaction,
-    add_flask_and_structure
+    add_structure
 )
 
+from ..resources import resource_path
 
-class KinetxKineticModelingJobTest(JobTestCase):
 
-    @skip_without('database', 'kinetx')
-    def test_concentrations(self):
+class TurbomoleSinglePointJobTest(JobTestCase):
+
+    @skip_without('database', 'turbomole')
+    def test_energy(self):
         # import Job
-        from scine_puffin.jobs.kinetx_kinetic_modeling import KinetxKineticModeling
+        from scine_puffin.jobs.turbomole_single_point import TurbomoleSinglePoint
         import scine_database as db
 
-        # This reaction network is made up and converges fairly quickly.
-        n_compounds = 5
-        all_compounds = [add_compound_and_structure(self.manager) for _ in range(n_compounds - 1)]
-        flask = add_flask_and_structure(self.manager)
-        dummy_compound = add_compound_and_structure(self.manager)
-        all_compounds.append(flask)
-        all_structure_ids = [c.get_centroid() for c in all_compounds]
-        c_ids = [c.id() for c in all_compounds]
-        all_reaction_ids = [
-            add_reaction(self.manager, [c_ids[0]], [c_ids[2]]).id(),
-            add_reaction(self.manager, [c_ids[1]], [c_ids[3]]).id(),
-            add_reaction(self.manager, [c_ids[2], c_ids[3]], [c_ids[0], c_ids[1]]).id(),
-            add_reaction(self.manager, [c_ids[0], c_ids[1]], [c_ids[4], c_ids[4]]).id()
-        ]
-        _ = add_reaction(self.manager, [dummy_compound.id()], [flask.id()])
-        lhs_rates = [0.1, 0.05, 0.02, 0.02]
-        rhs_rates = [0.05, 0.05, 0.001, 0.0000001]
-        start_concentrations = [0.5, 0.4, 0.0, 0.0, 0.0]
-        reference_data = [3.337327e-02, 5.991047e-05, 6.674503e-02, 5.839152e-05, 2 * 3.998817e-01]
-        reference_max = [0.5, 0.4, 0.07103765, 0.00325947, 2 * 0.3998817]
-        reference_flux = [1.85802001, 1.78338488, 1.45451295, 1.37987782, 2 * 0.40350706]
-
-        for c in all_compounds:
-            c.enable_exploration()
-
-        model = db.Model('FAKE', '', '')
-        job = db.Job('kinetx_kinetic_modeling')
-        settings = {
-            "time_step": 1e-08,
-            "solver": "cash_karp_5",
-            "batch_interval": 1000,
-            "n_batches": 50000,
-            "energy_label": "electronic_energy",
-            "convergence": 1e-10,
-            "lhs_rates": lhs_rates,
-            "rhs_rates": rhs_rates,
-            "start_concentrations": start_concentrations,
-            "reaction_ids": [str(oid) for oid in all_reaction_ids],
-            "aggregate_ids": [str(oid) for oid in c_ids],
-            "aggregate_types": [db.CompoundOrFlask.COMPOUND for _ in range(4)] + [db.CompoundOrFlask.FLASK],
-            "energy_model_program": "DUMMY",
-            "instant_barrierless": False
-        }
-
-        calculation = add_calculation(self.manager, model, job, all_structure_ids, settings)
+        # Setup DB for calculation
+        water = os.path.join(resource_path(), "water.xyz")
+        structure = add_structure(self.manager, water, db.Label.USER_GUESS)
+        model = db.Model('dft', 'pbe', 'def2-SVP')
+        job = db.Job('turbomole_single_point')
+        calculation = add_calculation(self.manager, model, job, [structure.id()])
 
         # Run calculation/job
         config = self.get_configuration()
-        job = KinetxKineticModeling()
+        job = TurbomoleSinglePoint()
         job.prepare(config["daemon"]["job_dir"], calculation.id())
         self.run_job(job, calculation, config)
 
         # Check results
+        assert calculation.get_status() == db.Status.COMPLETE
+        assert structure.has_property("electronic_energy")
+        energy_props = structure.get_properties("electronic_energy")
+        assert len(energy_props) == 1
+        results = calculation.get_results()
+        assert len(results.property_ids) == 1
+        assert energy_props[0] in results.property_ids
+
+        # Check generated properties
+        # Energy
         properties = self.manager.get_collection("properties")
-        structures = self.manager.get_collection("structures")
+        energy = db.NumberProperty(energy_props[0])
+        energy.link(properties)
+        self.assertAlmostEqual(energy.get_data(), -76.26848572171, delta=1e-1)
+
+    @skip_without('database', 'turbomole')
+    def test_charges(self):
+        # import Job
+        from scine_puffin.jobs.turbomole_single_point import TurbomoleSinglePoint
+        import scine_database as db
+        import scine_utilities as utils
+
+        # Setup DB for calculation
+        water = os.path.join(resource_path(), "water.xyz")
+        structure = add_structure(self.manager, water, db.Label.USER_GUESS)
+        model = db.Model('dft', 'pbe', 'def2-SVP')
+        job = db.Job('turbomole_single_point')
+        calculation = add_calculation(self.manager, model, job, [structure.id()])
+        settings = utils.ValueCollection({
+            "calculate_loewdin_charges": True
+        })
+        calculation.set_settings(settings)
+
+        # Run calculation/job
+        config = self.get_configuration()
+        job = TurbomoleSinglePoint()
+        job.prepare(config["daemon"]["job_dir"], calculation.id())
+        self.run_job(job, calculation, config)
+
+        # Check results
+        assert calculation.get_status() == db.Status.COMPLETE
+        assert structure.has_property("electronic_energy")
+        energy_props = structure.get_properties("electronic_energy")
+        assert len(energy_props) == 1
         results = calculation.get_results()
-        assert properties.count(dumps({})) == n_compounds * 3
-        assert len(results.property_ids) == n_compounds * 3
-        assert len(results.structure_ids) == 0
-        assert len(results.elementary_step_ids) == 0
-        for c in all_compounds:
-            assert not c.explore()
-        for i, s_id in enumerate(all_structure_ids):
-            structure = db.Structure(s_id, structures)
-            assert structure.has_property("final_concentration")
-            assert structure.has_property("max_concentration")
-            assert structure.has_property("concentration_flux")
-            final_concentration = db.NumberProperty(structure.get_properties("final_concentration")[0], properties)
-            max_concentration = db.NumberProperty(structure.get_properties("max_concentration")[0], properties)
-            concentration_flux = db.NumberProperty(structure.get_properties("concentration_flux")[0], properties)
-            self.assertAlmostEqual(final_concentration.get_data(), reference_data[i], delta=1e-2)
-            self.assertAlmostEqual(max_concentration.get_data(), reference_max[i], delta=1e-2)
-            self.assertAlmostEqual(concentration_flux.get_data(), reference_flux[i], delta=1e-1)
+        assert len(results.property_ids) == 2
+        assert energy_props[0] in results.property_ids
+
+        assert structure.has_property("loewdin_charges")
+        charge_props = structure.get_properties("loewdin_charges")
+        assert len(charge_props) == 1
+        assert charge_props[0] in results.property_ids
+
+        # Check generated properties
+        # Energy
+        properties = self.manager.get_collection("properties")
+        energy = db.NumberProperty(energy_props[0])
+        energy.link(properties)
+        self.assertAlmostEqual(energy.get_data(), -76.26848572171, delta=1e-1)
+
+        # Charges
+        properties = self.manager.get_collection("properties")
+        charges = db.VectorProperty(charge_props[0])
+        charges.link(properties)
+        self.assertAlmostEqual(charges.get_data()[0], -0.35773, delta=1e-1)
+        self.assertAlmostEqual(charges.get_data()[1], +0.17886, delta=1e-1)
+        self.assertAlmostEqual(charges.get_data()[2], +0.17886, delta=1e-1)
```

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_orca_geometry_optimization_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_orca_geometry_optimization_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_afir.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_afir.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_bond_orders_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_bond_orders_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_dissociation_cut_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_dissociation_cut_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_geometry_optimization_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_geometry_optimization_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_hessian.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_hessian.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_irc_scan_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_irc_scan_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_react_complex_afir_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_react_complex_afir_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_react_complex_nt2_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_react_complex_nt2_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_react_complex_nt_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_react_complex_nt_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_single_point_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_single_point_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_step_refinement_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_step_refinement_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_scine_ts_optimization_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_scine_ts_optimization_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_sleep_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_sleep_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_turbomole_bond_orders.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_turbomole_bond_orders.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_turbomole_geometry_optimization_job.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_turbomole_geometry_optimization_job.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/jobs/test_turbomole_hessian.py` & `scine_puffin-1.2.0/scine_puffin/tests/jobs/test_turbomole_hessian.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/daemon_test.py` & `scine_puffin-1.2.0/scine_puffin/tests/daemon_test.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/db_setup.py` & `scine_puffin-1.2.0/scine_puffin/tests/db_setup.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/masm_info_test.py` & `scine_puffin-1.2.0/scine_puffin/tests/masm_info_test.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/tests/testcases.py` & `scine_puffin-1.2.0/scine_puffin/tests/testcases.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/utilities/compound_and_flask_helpers.py` & `scine_puffin-1.2.0/scine_puffin/utilities/compound_and_flask_helpers.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/utilities/masm_helper.py` & `scine_puffin-1.2.0/scine_puffin/utilities/masm_helper.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/utilities/program_helper.py` & `scine_puffin-1.2.0/scine_puffin/utilities/program_helper.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/utilities/properties.py` & `scine_puffin-1.2.0/scine_puffin/utilities/properties.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/utilities/scine_helper.py` & `scine_puffin-1.2.0/scine_puffin/utilities/scine_helper.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/utilities/turbomole_helper.py` & `scine_puffin-1.2.0/scine_puffin/utilities/turbomole_helper.py`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/scine_puffin/__main__.py` & `scine_puffin-1.2.0/scine_puffin/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 # -*- coding: utf-8 -*-
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 import argparse
-import signal
 import sys
 from typing import Union
 from .bootstrap import bootstrap
 from .config import Configuration
-from .daemon import start_daemon, stop_daemon
-from .jobloop import check_setup, loop, kill_daemon
+from .daemon import start_daemon, stop_daemon, check_environment
+from .jobloop import kill_daemon
 
 
 def setup_config(args: argparse.Namespace) -> Configuration:
     config = Configuration()
     if args.config:
         config.load(args.config)
         print("Loading configuration: " + args.config)
@@ -117,23 +116,16 @@
     print("+----------------------------------+")
     print("|  Starting Puffin in Docker Mode  |")
     print("+----------------------------------+")
     if config is None:
         config = setup_config(parse_arguments())
     print("")
     print("Running with UUID: " + config["daemon"]["uuid"])
-    available_jobs = check_setup(config)
-
-    def exit_gracefully(*args, **kwargs):
-        print("Puffin shutting down gracefully")
-        sys.exit(0)
-
-    signal.signal(signal.SIGINT, exit_gracefully)
-    signal.signal(signal.SIGTERM, exit_gracefully)
-    loop(config, available_jobs)
+    check_environment(config)
+    start_daemon(config, detach=False)
 
 
 def main():
     args = parse_arguments(include_action=True)
     if args.action == "configure":
         configure(args)
         sys.exit()
```

### Comparing `scine_puffin-1.1.0/scine_puffin/bootstrap.py` & `scine_puffin-1.2.0/scine_puffin/bootstrap.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,30 +21,48 @@
     config :: scine_puffin.config.Configuration
        The current configuration of the Puffin.
     """
     # Prepare directories
     initial_dir = os.getcwd()
     jobs = config.daemon()["job_dir"]
     if jobs and not os.path.exists(jobs):
-        os.makedirs(jobs)
+        try:
+            os.makedirs(jobs)
+        except FileExistsError:
+            pass
     software = config.daemon()["software_dir"]
     if software and not os.path.exists(software):
-        os.makedirs(software)
+        try:
+            os.makedirs(software)
+        except FileExistsError:
+            pass
     build_dir = os.path.join(software, "build")
     if build_dir and not os.path.exists(build_dir):
-        os.makedirs(build_dir)
+        try:
+            os.makedirs(build_dir)
+        except FileExistsError:
+            pass
     install_dir = os.path.join(software, "install")
     if install_dir and not os.path.exists(install_dir):
-        os.makedirs(install_dir)
+        try:
+            os.makedirs(install_dir)
+        except FileExistsError:
+            pass
     archive_dir = config.daemon()["archive_dir"]
     if archive_dir and not os.path.exists(archive_dir) and archive_dir:
-        os.makedirs(archive_dir)
+        try:
+            os.makedirs(archive_dir)
+        except FileExistsError:
+            pass
     error_dir = config.daemon()["error_dir"]
     if error_dir and not os.path.exists(error_dir) and error_dir:
-        os.makedirs(error_dir)
+        try:
+            os.makedirs(error_dir)
+        except FileExistsError:
+            pass
 
     # Install minimal requirement
     print("")
     print("Building SCINE Utils from sources.")
     print("")
     utils_build_dir = os.path.join(build_dir, "utils")
     utils = Utils(config.programs()["utils"])
```

### Comparing `scine_puffin-1.1.0/scine_puffin/config.py` & `scine_puffin-1.2.0/scine_puffin/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,20 +96,28 @@
         If existent, the Puffin instance will archive all correctly completed
         jobs into this directory.
       uuid :: str
         A unique name for the Puffin instance. This can be set by the user, if
         not, a unique ID will automatically be generated.
       pid :: str
         The path to the file identifying the PID of the Puffin instance.
+        Automatically populated on start-up if left empty.
+      pid_dir :: str
+        The path to a folder holding the file identifying the PID of the Puffin instance.
       log :: str
         The path to the logfile of the Puffin instance.
       stop :: str
         The path to a file that if existent will prompt the Puffin instance to
         stop taking new jobs and shut down instead. The instance will finish any
         running job though.
+      remove_stop_file :: bool
+        Upon finding a stop file the daemon will stop, if this option is set to
+        ``True`` the found file will be deleted allowing instant restarts.
+        In cases where multiple puffins depend on the same stop file it may be
+        required to keep the stop file, setting this option to ``False``
       cycle_time_in_s :: float
         The time in between scans of the database for new jobs that can be run.
       timeout_in_h :: float
         The number of hours the Puffin instance should stay alive. Once this
         limit is reached, the Puffin is shut down and its running job will be
         killed and re-flagged as `new`.
       idle_timeout_in_h :: float
@@ -205,69 +213,71 @@
         }
         self._data["daemon"] = {
             "mode": "release",
             "job_dir": "/scratch/puffin/jobs",
             "software_dir": "/scratch/puffin/software",
             "error_dir": "",
             "archive_dir": "",
-            "uuid": "puffin-" + uuid.uuid1().hex,
-            "pid": "/scratch/puffin/puffin.pid",
+            "uuid": "",
+            "pid": "",
+            "pid_dir": "/scratch/puffin/",
             "log": "/scratch/puffin/puffin.log",
             "stop": "/scratch/puffin/puffin.stop",
+            "remove_stop_file": True,
             "cycle_time_in_s": 10.0,
             "timeout_in_h": 48.0,
             "touch_time_in_s": 1500.0,
             "job_reset_time_in_s": 7200.0,
             "idle_timeout_in_h": -1.0,
             "max_number_of_jobs": -1,
             "repeated_failure_stop": 100,
-            "enforce_memory_limit": True
+            "enforce_memory_limit": True,
         }
         self._data["programs"] = {
             "readuct": {
                 "available": True,
                 "source": "https://github.com/qcscine/readuct.git",
                 "root": "",
-                "version": "master",
+                "version": "5.0.0",
                 "march": "native",
                 "cxx_compiler_flags": "",
                 "cmake_flags": "",
             },
             "utils": {
                 "available": True,
                 "source": "https://github.com/qcscine/utilities.git",
                 "root": "",
-                "version": "master",
+                "version": "8.0.0",
                 "march": "native",
                 "cxx_compiler_flags": "",
                 "cmake_flags": "",
             },
             "database": {
                 "available": True,
                 "source": "https://github.com/qcscine/database.git",
                 "root": "",
-                "version": "master",
+                "version": "1.2.0",
                 "march": "native",
                 "cxx_compiler_flags": "",
                 "cmake_flags": "",
             },
             "sparrow": {
                 "available": True,
                 "source": "https://github.com/qcscine/sparrow.git",
                 "root": "",
-                "version": "master",
+                "version": "4.0.0",
                 "march": "native",
                 "cxx_compiler_flags": "",
                 "cmake_flags": "",
             },
             "molassembler": {
                 "available": True,
                 "source": "https://github.com/qcscine/molassembler.git",
                 "root": "",
-                "version": "master",
+                "version": "2.0.0",
                 "march": "native",
                 "cxx_compiler_flags": "",
                 "cmake_flags": "",
             },
             "swoose": {
                 'available': False,
                 'source': 'https://github.com/qcscine/swoose.git',
@@ -295,39 +305,39 @@
                 "root": "",
                 "version": "",
             },
             "serenity": {
                 "available": False,
                 "source": "https://github.com/qcscine/serenity_wrapper.git",
                 "root": "",
-                "version": "master",
+                "version": "2.0.0",
                 "march": "native",
                 "cxx_compiler_flags": "",
                 "cmake_flags": "",
             },
             "gaussian": {
                 "available": False,
                 "source": "",
                 "root": "",
                 "version": "g09 Rev. D.01",
             },
             "xtb": {
                 "available": False,
                 "source": "https://github.com/qcscine/xtb_wrapper.git",
                 "root": "",
-                "version": "master",
+                "version": "2.0.0",
                 "march": "native",
                 "cxx_compiler_flags": "",
                 "cmake_flags": "",
             },
             "kinetx": {
                 "available": False,
                 "source": "https://github.com/qcscine/kinetx.git",
                 "root": "",
-                "version": "master",
+                "version": "2.0.0",
                 "march": "native",
                 "cxx_compiler_flags": "",
                 "cmake_flags": "",
             },
         }
 
     def __getitem__(self, key: str) -> dict:
@@ -404,15 +414,15 @@
         yaml_dir = os.path.split(path)[0]
         if yaml_dir:
             if yaml_dir and not os.path.exists(yaml_dir):
                 os.makedirs(yaml_dir)
         with open(path, "w") as outfile:
             yaml.dump(self._data, outfile, default_flow_style=False)
 
-    def load(self, path: str = None):
+    def load(self, path: Optional[str] = None):
         """
         Loads the configuration. The configuration is initialized using the
         default values, then all settings given in the file (if there is one)
         are applied. Finally all settings given as environment variables are
         applied.
 
         Each setting in the config can be set via a corresponding environment
@@ -464,20 +474,27 @@
                 except BaseException as e:
                     raise KeyError(
                         "The environment variable '{}' can not be translated "
                         "into the correct variable type.".format(key)
                     ) from e
                 reduce(operator.getitem, key_chain[:-1], self._data)[key_chain[-1]] = value
 
-        # Generate uuid if none exists
+        # Generate uuid of specified type if unset
         if not self._data["daemon"]["uuid"] or self._data["daemon"]["uuid"] == "uuid1":
             self._data["daemon"]["uuid"] = "puffin-" + uuid.uuid1().hex
         elif self._data["daemon"]["uuid"] == "uuid4":
             self._data["daemon"]["uuid"] = "puffin-" + uuid.uuid4().hex
 
+        # Generate pid file path
+        if not self._data["daemon"]["pid"]:
+            self._data["daemon"]["pid"] = os.path.join(
+                self._data["daemon"]["pid_dir"],
+                f'{self._data["daemon"]["uuid"]}.pid'
+            )
+
     def _apply_changes(self, to_dict: dict, from_dict: dict):
         """
         A small helper applying changes from one dictionary to another, checking
         the types and making sure only existing keys are mapped.
 
         Parameters
         ----------
```

### Comparing `scine_puffin-1.1.0/scine_puffin/daemon.py` & `scine_puffin-1.2.0/scine_puffin/daemon.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,32 @@
         Dummy variable to match the signal dependent function signature.
     _frame
         Dummy variable to match the signal dependent function signature.
     """
     sys.exit(0)
 
 
+def check_environment(config: Configuration):
+    """
+    Checks the runtime environment for problematic configurations that may
+    interfere with job executions down the line.
+
+    Parameters
+    ----------.
+    config :: scine_puffin.config.Configuration
+        The current configuration of the Puffin.
+    """
+    if "OMP_NUM_THREADS" in os.environ:
+        if os.environ["OMP_NUM_THREADS"] != str(config["resources"]["cores"]):
+            raise RuntimeError("Environment variable OMP_NUM_THREADS must "
+                               "match configured number of cores.")
+    else:
+        os.environ["OMP_NUM_THREADS"] = str(config["resources"]["cores"])
+
+
 def stop_daemon(config: Configuration):
     """
     Stops the Puffin gracefully, allowing th current job to finish, then shutting
     down.
 
     Parameters
     ----------.
@@ -38,56 +56,68 @@
     """
     # Generate stop file in order to stop after the current job
     pid_file = config["daemon"]["pid"]
     if os.path.isfile(pid_file):
         stop_file = config.daemon()["stop"]
         basedir = os.path.dirname(stop_file)
         if not os.path.exists(basedir):
-            os.makedirs(basedir)
+            try:
+                os.makedirs(basedir)
+            except FileExistsError:
+                pass
         with open(stop_file, "w"):
             pass
 
 
-def start_daemon(config: Configuration):
+def start_daemon(config: Configuration, detach: bool = True):
     """
     Starts the Puffin, using the given configuration.
 
     Parameters
     ----------.
     config :: scine_puffin.config.Configuration
         The current configuration of the Puffin.
+    detach :: bool
+        If true, forks the daemon process and detaches it.
     """
-    if "OMP_NUM_THREADS" in os.environ:
-        if os.environ["OMP_NUM_THREADS"] != str(config["resources"]["cores"]):
-            raise RuntimeError("Environment variable OMP_NUM_THREADS must "
-                               "match configured number of cores.")
-    else:
-        os.environ["OMP_NUM_THREADS"] = str(config["resources"]["cores"])
+    check_environment(config)
 
     # Ensure existence of the directory for job files
     job_dir = config["daemon"]["job_dir"]
     if job_dir and not os.path.exists(job_dir):
-        os.makedirs(job_dir)
+        try:
+            os.makedirs(job_dir)
+        except FileExistsError:
+            pass
 
     # Ensure existence of the directory for a pid file
     pid = config["daemon"]["pid"]
     pid_dir = os.path.split(config["daemon"]["pid"])[0]
     if pid_dir and not os.path.exists(pid_dir):
-        os.makedirs(pid_dir)
+        try:
+            os.makedirs(pid_dir)
+        except FileExistsError:
+            pass
 
     # Ensure existence of the directory for a stop file
     stop_dir = os.path.split(config["daemon"]["stop"])[0]
     if stop_dir and not os.path.exists(stop_dir):
-        os.makedirs(stop_dir)
+        try:
+            os.makedirs(stop_dir)
+        except FileExistsError:
+            pass
 
     # Generate log file if not present
     if config["daemon"]["log"]:
         log_dir = os.path.split(config["daemon"]["log"])[0]
         if log_dir and not os.path.exists(log_dir):
-            os.makedirs(log_dir)
+            try:
+                os.makedirs(log_dir)
+            except FileExistsError:
+                pass
         if not os.path.exists(config["daemon"]["log"]):
             with open(config["daemon"]["log"], "w"):
                 pass
 
     # Give the daemon a decent name
     setproctitle.setproctitle("puffin")
 
@@ -102,16 +132,25 @@
 
     context = DaemonContext(
         chroot_directory=None,
         working_directory=job_dir,
         stdout=sys.stdout,
         stderr=sys.stderr,
         pidfile=pidfile.TimeoutPIDLockFile(pid),
-        detach_process=True,
+        detach_process=detach,
     )
-    context.signal_map = {signal.SIGTERM: shutdown, signal.SIGTSTP: shutdown}
+
+    def exit_gracefully(*args, **kwargs):
+        print("Puffin shutting down gracefully")
+        stop_daemon(config)
+
+    context.signal_map = {
+        signal.SIGINT: exit_gracefully,
+        signal.SIGTERM: exit_gracefully,
+        signal.SIGTSTP: exit_gracefully
+    }
 
     if config["daemon"]["mode"] == "debug":
         loop(config, available_jobs)
     else:
         with context:
             loop(config, available_jobs)
```

### Comparing `scine_puffin-1.1.0/scine_puffin/jobloop.py` & `scine_puffin-1.2.0/scine_puffin/jobloop.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import time
 import ctypes
 import multiprocessing
 import random
 import traceback
 from datetime import datetime, timedelta
 from importlib import import_module, util
-from typing import Dict, List
+from typing import Any, Dict, List
 from json import dumps
 from .config import Configuration
 
 # A global variable holding the process actually running jobs.
 # This variable is used to be able to interact with (mainly to kill) said
 # process even from outside the loop() function.
 PROCESS = None
@@ -75,38 +75,42 @@
             time.sleep(1.0 + r)
     else:
         manager.connect()
 
 
 def kill_daemon(config: Configuration) -> None:
     """
-    Kills the Puffin instantaneously without any possibility of a graceful
-    exit.
+    Kills the Puffin instantaneously without any possibility of a graceful exit.
 
     Parameters
-    ----------.
+    ----------
     config :: scine_puffin.config.Configuration
-       The current configuration of the Puffin.
+        The current configuration of the Puffin.
     """
     # Remove stop file if present
-    stop_file = config.daemon()["stop"]
-    if os.path.isfile(stop_file):
-        os.remove(stop_file)
+    if config.daemon()["remove_stop_file"]:
+        stop_file = config.daemon()["stop"]
+        if os.path.isfile(stop_file):
+            try:
+                os.remove(stop_file)
+            except FileNotFoundError:
+                pass
 
     # Kill the daemon process
     pid_file = config["daemon"]["pid"]
 
     if PROCESS is not None:
         parent = psutil.Process(PROCESS.pid)
         for child in parent.children(recursive=True):
             child.kill()
         parent.kill()
     if os.path.isfile(pid_file):
         with open(pid_file, "r") as f:
             pid = int(f.readline().strip())
+        os.remove(pid_file)
         parent = psutil.Process(pid)
         for child in parent.children(recursive=True):
             child.kill()
         parent.kill()
 
 
 def loop(config: Configuration, available_jobs: dict) -> None:
@@ -133,17 +137,17 @@
     import scine_database as db
 
     manager = db.Manager()
     slow_connect(manager, config)
 
     # Generate shared variable
     # Shared variables have to be ctypes so this is a bit ugly
-    JOB = multiprocessing.Array(ctypes.c_char, 200)
+    JOB: Any = multiprocessing.Array(ctypes.c_char, 200)
     JOB.value = "".encode("utf-8")
-    CURRENT_DB = multiprocessing.Array(ctypes.c_char, 200)
+    CURRENT_DB: Any = multiprocessing.Array(ctypes.c_char, 200)
     CURRENT_DB.value = manager.get_database_name().encode("utf-8")
 
     # Run the loop in a second process
     PROCESS = multiprocessing.Process(  # pylint: disable=redefined-outer-name
         target=_loop_impl,
         args=(),
         kwargs={
@@ -163,17 +167,14 @@
     touch_time = timedelta(seconds=config["daemon"]["touch_time_in_s"])
     reset_delta = timedelta(seconds=config["daemon"]["job_reset_time_in_s"])
     last_time_with_a_job = datetime.now()
     last_touch = datetime.now()
     start = datetime.now()
     while PROCESS.is_alive():
         time.sleep(1.0)
-        if not manager.has_collection("calculations"):
-            time.sleep(20.0)
-            continue
         # Kill the puffin if it was idle for too long
         now = datetime.now()
         if JOB.value.decode("utf-8"):
             last_time_with_a_job = now
         if idle_timeout is not None and (now - last_time_with_a_job) > idle_timeout:
             _log(config, "Puffin reached idle timeout")
             kill_daemon(config)
@@ -358,15 +359,19 @@
     previous_dbs: List[str] = []
     n_jobs_run = 0
 
     while True:
         # Stop the loop if a stop file has been written
         stop_file = config["daemon"]["stop"]
         if os.path.isfile(stop_file):
-            os.remove(stop_file)
+            if config.daemon()["remove_stop_file"]:
+                try:
+                    os.remove(stop_file)
+                except FileNotFoundError:
+                    pass
             _log(config, "Detected stop file " + stop_file + " and stopped puffin.")
             break
 
         # Wait if needed
         loop_time = datetime.now() - last_cycle
         if loop_time < sleep:
             time.sleep(int(round((sleep - loop_time).total_seconds())))
@@ -459,24 +464,23 @@
         try:
             class_name = available_jobs[job_name]
         except BaseException as e:
             raise KeyError("Missing Job in list of possible jobs.\n" +
                            "Dev-Note: This error should not be reachable.") from e
         module = import_module("scine_puffin.jobs." + job_name)
         class_ = getattr(module, class_name)
-        job = class_()
 
-        SUCCESS = multiprocessing.Value('i', False)  # Create value in shared memory. Use int for bool flag
+        SUCCESS: Any = multiprocessing.Value('i', False)  # Create value in shared memory. Use int for bool flag
         # Run the job in a third process
         JOB_PROCESS = multiprocessing.Process(
             target=_job_execution,
             args=(),
             kwargs={
                 "config": config,
-                "job": job,
+                "job_class": class_,
                 "manager": manager,
                 "calculation": calculation,
                 "SUCCESS": SUCCESS,
             },
         )
         JOB_PROCESS.start()
         start = datetime.now()  # in case we need to abort the job, we can set a runtime
@@ -553,18 +557,19 @@
                     comment = calculation.get_comment()
                     calculation.set_comment("Calculation has been reset.\nComment of previous run: " + comment)
                 # Log and exit
                 _log(config, "Stopping Puffin due to {:d} consecutive failed jobs".format(previously_failed_job_count))
                 break
 
 
-def _job_execution(config: Configuration, job, manager, calculation, SUCCESS=None) -> None:
+def _job_execution(config: Configuration, job_class: type, manager, calculation, SUCCESS=None) -> None:
     """
     We are running job in a separate process to save us from SegFaults and enforce memory limit
     """
+    job = job_class()
     _log(config, "Processing Job: {:s}".format(str(calculation.id())))
     # Prepare job directory and start timer
     start = datetime.now()
     job.prepare(config["daemon"]["job_dir"], calculation.id())
     # Run job
     success = job.run(manager, calculation, config)
     # we already write a runtime in case puffin fails during copying operations
```

### Comparing `scine_puffin-1.1.0/scine_puffin.egg-info/PKG-INFO` & `scine_puffin-1.2.0/scine_puffin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scine-puffin
-Version: 1.1.0
+Version: 1.2.0
 Summary: Calculation handler for SCINE Chemoton
 Home-page: https://www.scine.ethz.ch
 Author: ETH Zurich, Laboratory of Physical Chemistry, Reiher Group
 Author-email: scine@phys.chem.ethz.ch
 License: BSD (3-clause)
 Description: .. image:: docs/source/res/puffin_header.png
            :alt: SCINE Puffin
```

### Comparing `scine_puffin-1.1.0/scine_puffin.egg-info/SOURCES.txt` & `scine_puffin-1.2.0/scine_puffin.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 scine_puffin/jobs/conformers.py
 scine_puffin/jobs/gaussian_charge_model_5.py
 scine_puffin/jobs/graph.py
 scine_puffin/jobs/kinetx_kinetic_modeling.py
 scine_puffin/jobs/orca_geometry_optimization.py
 scine_puffin/jobs/scine_afir.py
 scine_puffin/jobs/scine_bond_orders.py
+scine_puffin/jobs/scine_bspline_optimization.py
 scine_puffin/jobs/scine_conceptual_dft.py
 scine_puffin/jobs/scine_dissociation_cut.py
 scine_puffin/jobs/scine_geometry_optimization.py
 scine_puffin/jobs/scine_hessian.py
 scine_puffin/jobs/scine_irc_scan.py
 scine_puffin/jobs/scine_react_complex_afir.py
 scine_puffin/jobs/scine_react_complex_nt.py
```

### Comparing `scine_puffin-1.1.0/CHANGELOG.rst` & `scine_puffin-1.2.0/CHANGELOG.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 Changelog
 =========
 
+Release 1.2.0
+-------------
+
+New Features:
+    - Add a mechanism to stop multiple Puffins
+    - Generate PID based on UUID, allowing to run multiple Puffins on the same filesystem
+
+New Jobs:
+    - Double ended reaction step refinement.
+
+Further changes:
+    - Various bugfixes and improvements
+
 Release 1.1.0
 -------------
 
 New Features:
  - Support for stable intermediate complexes and barrier-less reactions
     - Strongly interacting complexes containing multiple structures
       are now saved in the database.
```

### Comparing `scine_puffin-1.1.0/README.rst` & `scine_puffin-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `scine_puffin-1.1.0/setup.cfg` & `scine_puffin-1.2.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -27,8 +27,9 @@
 generated-members = Lock
 ignore = _version.py
 overgeneral-exceptions = Exception
 
 [egg_info]
 tag_build = 
 tag_date = 0
+tag_svn_revision = 0
```

### Comparing `scine_puffin-1.1.0/setup.py` & `scine_puffin-1.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,16 @@
     version=__version__,
     author="ETH Zurich, Laboratory of Physical Chemistry, Reiher Group",
     author_email="scine@phys.chem.ethz.ch",
     description="Calculation handler for SCINE Chemoton",
     long_description=readme,
     url="https://www.scine.ethz.ch",
     python_requires=">={}".format(".".join(str(n) for n in min_version)),
-    packages=find_packages(exclude=["docs", "tests"]),
+    packages=find_packages(include=["scine_puffin", "scine_puffin.*"],
+                           exclude=["scine_puffin.tests*"]),
     include_package_data=True,
     package_data={
         "scine_puffin": [
             # When adding files here, remember to update MANIFEST.in as well,
             # or else they will not be included in the distribution on PyPI!
             # 'path/to/data_file',
         ]
```

### Comparing `scine_puffin-1.1.0/PKG-INFO` & `scine_puffin-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scine_puffin
-Version: 1.1.0
+Version: 1.2.0
 Summary: Calculation handler for SCINE Chemoton
 Home-page: https://www.scine.ethz.ch
 Author: ETH Zurich, Laboratory of Physical Chemistry, Reiher Group
 Author-email: scine@phys.chem.ethz.ch
 License: BSD (3-clause)
 Description: .. image:: docs/source/res/puffin_header.png
            :alt: SCINE Puffin
```

