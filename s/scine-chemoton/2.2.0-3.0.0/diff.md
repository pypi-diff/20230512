# Comparing `tmp/scine_chemoton-2.2.0.tar.gz` & `tmp/scine_chemoton-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scine_chemoton-2.2.0.tar", last modified: Thu Sep 22 14:29:22 2022, max compression
+gzip compressed data, was "dist/scine_chemoton-3.0.0.tar", last modified: Thu May 11 06:57:31 2023, max compression
```

## Comparing `scine_chemoton-2.2.0.tar` & `scine_chemoton-3.0.0.tar`

### file list

```diff
@@ -1,133 +1,138 @@
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/dev/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/dev/conan/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-09-22 14:08:21.000000 scine_chemoton-2.2.0/dev/conan/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11187 2022-09-22 14:08:21.000000 scine_chemoton-2.2.0/dev/conan/base.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2696 2022-09-22 14:08:21.000000 scine_chemoton-2.2.0/dev/conan/utils.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:08:21.000000 scine_chemoton-2.2.0/dev/__init__.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/docs/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/docs/source/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/docs/source/api/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      102 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/docs/source/api/api.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       52 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/docs/source/api/engine.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1640 2022-09-21 11:47:56.000000 scine_chemoton-2.2.0/docs/source/api/gears.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      475 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/docs/source/api/utilities.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       33 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/docs/source/changelog.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5885 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/docs/source/conf.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      185 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/docs/source/index.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       78 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/docs/source/readme.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      673 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/docs/Makefile
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      797 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/docs/make.bat
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/gears/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/gears/conformers/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/conformers/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     9932 2022-09-21 06:55:53.000000 scine_chemoton-2.2.0/scine_chemoton/gears/conformers/brute_force.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/trial_generator/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      927 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/trial_generator/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    45076 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/trial_generator/bond_based.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6997 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/trial_generator/connectivity_analyzer.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    27212 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/trial_generator/fast_dissociations.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    40849 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/trial_generator/fragment_based.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4921 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2246 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/brute_force.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    22696 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/compound_filters.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2488 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/minimal.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4855 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/minimum_energy_confomer.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    33280 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/reactive_site_filters.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/gears/kinetic_modeling/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/kinetic_modeling/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3671 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/kinetic_modeling/concentration_query_functions.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10438 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/kinetic_modeling/kinetic_modeling.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    20230 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/kinetic_modeling/prepare_kinetic_modeling_job.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5143 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    18752 2022-09-21 06:55:53.000000 scine_chemoton-2.2.0/scine_chemoton/gears/compound.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    17775 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/kinetics.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    41716 2022-09-21 11:47:56.000000 scine_chemoton-2.2.0/scine_chemoton/gears/pathfinder.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    15916 2022-09-21 06:55:53.000000 scine_chemoton-2.2.0/scine_chemoton/gears/reaction.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    41440 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/refinement.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5721 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/scheduler.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4144 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/gears/thermo.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/tests/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/conformers/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/conformers/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8045 2022-09-21 06:55:53.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/conformers/test_brute_force.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    43637 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_bond_based.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6741 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_connectivity_analyzer.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    14760 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_fast_dissociations.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    32406 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_fragment_based.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1151 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/mock_trial_generator.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6092 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/test_brute_force.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    27900 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/test_compound_filters.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10166 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/test_further_dissociations_reactive_site_filters.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6167 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/test_minimal.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8388 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/test_minimum_energy_confomer.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    31254 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/test_reactive_site_filters.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/kinetic_modeling/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/kinetic_modeling/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6259 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/kinetic_modeling/test_kinetic_modeling.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    22459 2022-09-21 06:55:53.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/test_compound.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    16781 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/test_kinetics.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    19945 2022-09-21 06:59:10.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/test_pathfinder.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11409 2022-09-21 06:55:53.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/test_reaction.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    39173 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/test_refinement.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2415 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/test_scheduler.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4653 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/gears/test_thermo.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/tests/resources/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      506 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/resources/__init__.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/reactive_complexes/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/reactive_complexes/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    25714 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/reactive_complexes/test_inter_reactive_complexes.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      712 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/reactive_complexes/test_lebedev_sphere.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1028 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/reactive_complexes/test_masm_pruning.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      720 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/reactive_complexes/test_unit_circle.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5149 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/queries_test.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3889 2022-09-21 06:59:10.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/test_get_molecular_formulas.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2627 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/test_insert_concentration.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2671 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/test_insert_initial_structure.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1109 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/tests/utilities/test_masm.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/tests/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    21236 2022-09-21 06:59:10.000000 scine_chemoton-2.2.0/scine_chemoton/tests/test_database_setup.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/reactive_complexes/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1342 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/reactive_complexes/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    40666 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/reactive_complexes/inter_reactive_complexes.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)   598402 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/reactive_complexes/lebedev_sphere.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8094 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/reactive_complexes/unit_circle.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      733 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/calculation_creation_helpers.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1915 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/compound_and_flask_creation.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7872 2022-09-21 06:59:10.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/energy_query_functions.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4422 2022-09-21 06:59:10.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/get_molecular_formula.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1516 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/insert_concentration.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2408 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/insert_initial_structure.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11592 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/masm.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    13163 2022-09-21 06:55:49.000000 scine_chemoton-2.2.0/scine_chemoton/utilities/queries.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      273 2022-09-21 06:55:53.000000 scine_chemoton-2.2.0/scine_chemoton/__init__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    16581 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/__main__.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      200 2022-09-21 06:59:10.000000 scine_chemoton-2.2.0/scine_chemoton/_version.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2766 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/scine_chemoton/engine.py
-drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton.egg-info/
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6419 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton.egg-info/PKG-INFO
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5079 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton.egg-info/SOURCES.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton.egg-info/dependency_links.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       20 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton.egg-info/entry_points.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-09-21 07:00:13.000000 scine_chemoton-2.2.0/scine_chemoton.egg-info/not-zip-safe
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       84 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton.egg-info/requires.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       19 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/scine_chemoton.egg-info/top_level.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3579 2022-09-21 06:59:10.000000 scine_chemoton-2.2.0/CHANGELOG.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      355 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/MANIFEST.in
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4529 2022-09-21 06:55:48.000000 scine_chemoton-2.2.0/README.rst
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      137 2022-09-21 06:59:10.000000 scine_chemoton-2.2.0/requirements.txt
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      752 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/setup.cfg
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2511 2022-09-21 06:55:53.000000 scine_chemoton-2.2.0/setup.py
--rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6419 2022-09-22 14:29:22.000000 scine_chemoton-2.2.0/PKG-INFO
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/dev/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/dev/conan/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2023-02-15 12:22:00.000000 scine_chemoton-3.0.0/dev/conan/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11187 2022-05-06 11:41:04.000000 scine_chemoton-3.0.0/dev/conan/base.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2696 2023-05-11 06:57:22.000000 scine_chemoton-3.0.0/dev/conan/utils.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2021-09-10 05:25:08.000000 scine_chemoton-3.0.0/dev/__init__.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/docs/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/docs/source/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/docs/source/api/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      102 2021-10-27 12:51:25.000000 scine_chemoton-3.0.0/docs/source/api/api.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       52 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/docs/source/api/engine.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2179 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/docs/source/api/gears.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      475 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/docs/source/api/utilities.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       33 2021-10-27 12:51:25.000000 scine_chemoton-3.0.0/docs/source/changelog.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5725 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/docs/source/conf.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      185 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/docs/source/index.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       78 2021-10-27 12:51:25.000000 scine_chemoton-3.0.0/docs/source/readme.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      673 2020-04-20 12:19:04.000000 scine_chemoton-3.0.0/docs/Makefile
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      797 2020-04-20 12:19:04.000000 scine_chemoton-3.0.0/docs/make.bat
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/gears/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/gears/conformers/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/gears/conformers/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11856 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/conformers/brute_force.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/reaction_rules/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1049 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/reaction_rules/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    12556 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/reaction_rules/distance_rules.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3289 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/reaction_rules/element_rules.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6709 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/reaction_rules/polarization_rules.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/trial_generator/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8360 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/trial_generator/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    46723 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/trial_generator/bond_based.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7026 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/trial_generator/connectivity_analyzer.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    37487 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/trial_generator/fast_dissociations.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    47363 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/trial_generator/fragment_based.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    31491 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/trial_generator/template_based.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    16934 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    37024 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/aggregate_filters.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2437 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/brute_force.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2491 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/minimal.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5038 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/minimum_energy_conformer.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    24331 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/reactive_site_filters.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/gears/kinetic_modeling/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-08-08 07:34:02.000000 scine_chemoton-3.0.0/scine_chemoton/gears/kinetic_modeling/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     9813 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/kinetic_modeling/concentration_query_functions.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11427 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/kinetic_modeling/kinetic_modeling.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    25218 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/kinetic_modeling/prepare_kinetic_modeling_job.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     7639 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    17750 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/compound.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    32632 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/kinetics.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    55914 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/pathfinder.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    17689 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/reaction.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    50986 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/refinement.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10996 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/rerun_calculations.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6018 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/scheduler.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8868 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/gears/thermo.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/tests/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/conformers/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/conformers/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8760 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/conformers/test_brute_force.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    61627 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_bond_based.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6741 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_connectivity_analyzer.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    14144 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_fast_dissociations.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    33164 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_fragment_based.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5944 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/mock_trial_generator.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6092 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/test_brute_force.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10366 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/test_further_dissociations_reactive_site_filters.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    12731 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/test_minimal.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    33736 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/test_reactive_site_filters.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/kinetic_modeling/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-08-08 07:34:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/kinetic_modeling/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    12643 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/kinetic_modeling/test_kinetic_modeling.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    25569 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/test_compound.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    32478 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/test_kinetics.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11856 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/test_reaction.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    42503 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/test_refinement.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2415 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/test_scheduler.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    10662 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/gears/test_thermo.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/tests/resources/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      506 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/resources/__init__.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/tests/utilities/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/tests/utilities/reactive_complexes/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/utilities/reactive_complexes/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    25677 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/utilities/reactive_complexes/test_inter_reactive_complexes.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      712 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/utilities/reactive_complexes/test_lebedev_sphere.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1028 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/utilities/reactive_complexes/test_masm_pruning.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      720 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/utilities/reactive_complexes/test_unit_circle.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/utilities/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5155 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/utilities/queries_test.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4806 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/utilities/test_insert_concentration.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2671 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/utilities/test_insert_initial_structure.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1109 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/utilities/test_masm.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      224 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/tests/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    23492 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/tests/test_database_setup.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/reactive_complexes/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1342 2022-08-08 07:34:02.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/reactive_complexes/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    41008 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/reactive_complexes/inter_reactive_complexes.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)   598402 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/reactive_complexes/lebedev_sphere.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     8094 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/reactive_complexes/unit_circle.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1524 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      733 2022-08-08 07:34:02.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/calculation_creation_helpers.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      900 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/comparisons.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     1917 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/compound_and_flask_creation.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11520 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/energy_query_functions.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5162 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/get_molecular_formula.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2035 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/insert_concentration.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2799 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/insert_initial_structure.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    11592 2022-08-08 07:34:02.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/masm.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    17057 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/utilities/queries.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      273 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/__init__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)    15100 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/__main__.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      200 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/_version.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     3004 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/scine_chemoton/default_settings.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4259 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/scine_chemoton/engine.py
+drwxr-xr-x   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        0 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton.egg-info/
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6617 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton.egg-info/PKG-INFO
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     5299 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton.egg-info/SOURCES.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton.egg-info/dependency_links.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       20 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton.egg-info/entry_points.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)        1 2022-07-21 06:56:24.000000 scine_chemoton-3.0.0/scine_chemoton.egg-info/not-zip-safe
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      101 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton.egg-info/requires.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)       15 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/scine_chemoton.egg-info/top_level.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6003 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/CHANGELOG.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      355 2022-01-28 10:10:02.000000 scine_chemoton-3.0.0/MANIFEST.in
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     4703 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/README.rst
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      154 2023-04-24 09:13:51.000000 scine_chemoton-3.0.0/requirements.txt
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)      761 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/setup.cfg
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     2595 2023-05-11 06:57:14.000000 scine_chemoton-3.0.0/setup.py
+-rw-r--r--   0 tweymuth (57196) CHAB-CHEM-PHYS-Reiher (208550)     6617 2023-05-11 06:57:31.000000 scine_chemoton-3.0.0/PKG-INFO
```

### Comparing `scine_chemoton-2.2.0/dev/conan/base.py` & `scine_chemoton-3.0.0/dev/conan/base.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/dev/conan/utils.py` & `scine_chemoton-3.0.0/dev/conan/utils.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/docs/source/api/gears.rst` & `scine_chemoton-3.0.0/docs/source/api/gears.rst`

 * *Files 18% similar despite different names*

```diff
@@ -5,50 +5,59 @@
 ---------
 .. autoclass:: scine_chemoton.gears.Gear
     :special-members: __call__
 
 Implementations
 ---------------
 
-Compound Sorting
-~~~~~~~~~~~~~~~~
+Aggregate Sorting
+~~~~~~~~~~~~~~~~~
 .. automodule:: scine_chemoton.gears.compound
 
 Conformer Generation
 ~~~~~~~~~~~~~~~~~~~~
 .. automodule:: scine_chemoton.gears.conformers.brute_force
 
 Elementary Steps Exploration
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 .. autoclass:: scine_chemoton.gears.elementary_steps.ElementaryStepGear
 .. automodule:: scine_chemoton.gears.elementary_steps.brute_force
 .. automodule:: scine_chemoton.gears.elementary_steps.minimal
+.. automodule:: scine_chemoton.gears.elementary_steps.minimum_energy_conformer
 .. autoclass:: scine_chemoton.gears.elementary_steps.trial_generator.TrialGenerator
 .. automodule:: scine_chemoton.gears.elementary_steps.trial_generator.bond_based
 .. automodule:: scine_chemoton.gears.elementary_steps.trial_generator.fragment_based
+.. automodule:: scine_chemoton.gears.elementary_steps.trial_generator.fast_dissociations
 .. automodule:: scine_chemoton.gears.elementary_steps.trial_generator.connectivity_analyzer
 
-Compound Filter
-"""""""""""""""
-.. automodule:: scine_chemoton.gears.elementary_steps.compound_filters
+Aggregate Filter
+""""""""""""""""
+.. automodule:: scine_chemoton.gears.elementary_steps.aggregate_filters
 
 Reactive Site Filter
 """"""""""""""""""""
 .. automodule:: scine_chemoton.gears.elementary_steps.reactive_site_filters
 
+Optional Reaction Rules
+"""""""""""""""""""""""
+.. automodule:: scine_chemoton.gears.elementary_steps.reaction_rules
+.. automodule:: scine_chemoton.gears.elementary_steps.reaction_rules.distance_rules
+.. automodule:: scine_chemoton.gears.elementary_steps.reaction_rules.element_rules
+.. automodule:: scine_chemoton.gears.elementary_steps.reaction_rules.polarization_rules
+
 Kinetics
 ~~~~~~~~
 .. automodule:: scine_chemoton.gears.kinetics
 
 Pathfinder
 ~~~~~~~~~~
 .. automodule:: scine_chemoton.gears.pathfinder
 
 Reaction Sorting
-~~~~~~~~~~~~~~~~~~~~~~~
+~~~~~~~~~~~~~~~~
 .. automodule:: scine_chemoton.gears.reaction
 
 Network Refinement
 ~~~~~~~~~~~~~~~~~~
 .. automodule:: scine_chemoton.gears.refinement
 
 Job Scheduling
```

### Comparing `scine_chemoton-2.2.0/docs/source/conf.py` & `scine_chemoton-3.0.0/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
+import sphinx_rtd_theme
+import scine_chemoton
+
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 source_suffix = ['.rst', '.md']
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
@@ -24,23 +27,14 @@
     'sphinx_autodoc_typehints',
     'sphinx.ext.viewcode',
     'matplotlib.sphinxext.plot_directive',
     'numpydoc',
     'sphinx_copybutton',
 ]
 
-# Mock C++ based dependecies
-autodoc_mock_imports = [
-    "scine_database",
-    "scine_utilities",
-    "scine_readuct",
-    "rdkit",
-    "scine_molassembler"
-]
-
 # Configuration options for plot_directive. See:
 # https://github.com/matplotlib/matplotlib/blob/f3ed922d935751e08494e5fb5311d3050a3b637b/lib/matplotlib/sphinxext/plot_directive.py#L81
 plot_html_show_source_link = False
 plot_html_show_formats = False
 
 # Generate the API documentation when building
 autosummary_generate = True
@@ -57,15 +51,14 @@
 copyright = "2019, ETH Zurich, Laboratory for Physical Chemistry, Reiher Group"
 author = "Reiher Group"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-import scine_chemoton
 
 # The short X.Y version.
 version = scine_chemoton.__version__
 # The full version, including alpha/beta/rc tags.
 release = scine_chemoton.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
@@ -89,15 +82,14 @@
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "sphinx_rtd_theme"
-import sphinx_rtd_theme
 
 html_theme_path = [sphinx_rtd_theme.get_html_theme_path()]
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
```

### Comparing `scine_chemoton-2.2.0/docs/Makefile` & `scine_chemoton-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/docs/make.bat` & `scine_chemoton-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/conformers/brute_force.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/conformers/brute_force.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 # -*- coding: utf-8 -*-
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
-import time
 from json import dumps
+from typing import List
+import math
+import time
 
 # Third party imports
 import scine_database as db
 import scine_utilities as utils
 
 # Local application imports
 from .. import Gear
+from ..elementary_steps.aggregate_filters import AggregateFilter
 from ...utilities.queries import model_query, stop_on_timeout
 
 
 class BruteForceConformers(Gear):
     """
     This Gear generates all possible conformers as a guess based on the centroid
     of each Compound. The guesses are then optimized. Deduplication of optimized
@@ -35,44 +38,38 @@
     Conformer guesses are supposed to be the only 'minimum_guess' structures
     assigned to compounds as they are the only ones where the correct graph
     assignment should be possible.
     If no conformer guesses are present they are generated and the associated
     geometry optimizations are scheduled.
     """
 
-    class Options:
+    class Options(Gear.Options):
         """
         The options for the BruteForceConformers Gear.
         """
 
         __slots__ = (
             "cycle_time",
-            "model",
             "conformer_job",
             "minimization_job",
             "conformer_settings",
             "minimization_settings",
             "temperature"
         )
 
         def __init__(self):
+            super().__init__()
             self.cycle_time = 10
             """
             int
                 The minimum number of seconds between two cycles of the Gear.
                 Cycles are finished independent of this option, thus if a cycle
                 takes longer than the cycle_time will effectively lead to longer
                 cycle times and not cause multiple cycles of the same Gear.
             """
-            self.model: db.Model = db.Model("PM6", "", "")
-            """
-            db.Model (Scine::Database::Model)
-                The Model used for the conformer generation.
-                The default is: PM6 using Sparrow.
-            """
             self.conformer_job: db.Job = db.Job("conformers")
             """
             db.Job (Scine::Database::Calculation::Job)
                 The Job used for the generation of new conformer guesses.
                 The default is: the 'conformers' order on a single core.
             """
             self.conformer_settings: utils.ValueCollection = utils.ValueCollection()
@@ -92,40 +89,78 @@
             self.minimization_settings: utils.ValueCollection = utils.ValueCollection()
             """
             utils.ValueCollection
                 Additional settings passed to the geometry optimization
                 calculations. Empty by default.
             """
             self.temperature = 298.15
+            """
+            float
+                Temperature for Boltzmann evaluations
+            """
 
     def __init__(self):
         super().__init__()
-        self.options = self.Options()
+        self.aggregate_filter = AggregateFilter()
         self._required_collections = ["calculations", "compounds", "properties", "structures"]
         # local cache variables
-        self._completed = []
+        self._completed = set()
+
+    def _propagate_db_manager(self, manager: db.Manager):
+        self._sanity_check_configuration()
+        self.aggregate_filter.initialize_collections(manager)
+
+    def _sanity_check_configuration(self):
+        if not isinstance(self.aggregate_filter, AggregateFilter):
+            raise TypeError(f"Expected a AggregateFilter (or a class derived "
+                            f"from it) in {self.name}.aggregate_filter.")
+
+    def clear_cache(self):
+        self._completed = set()
+
+    def valid_compounds(self) -> List[db.ID]:
+        result: List[db.ID] = []
+        # Loop over all compounds
+        for compound in stop_on_timeout(self._compounds.iterate_all_compounds()):
+            compound.link(self._compounds)
+            if self.stop_at_next_break_point:
+                return result
+            # Check for initial reasons to skip
+            compound_id = compound.id()
+            if not compound.explore() or str(compound_id) in self._completed:
+                continue
+            if self.aggregate_filter.filter(compound):
+                result.append(compound_id)
+        return result
 
     def _loop_impl(self):
         # Loop over all compounds
         for compound in stop_on_timeout(self._compounds.iterate_all_compounds()):
             compound.link(self._compounds)
+            if self.stop_at_next_break_point:
+                return
             # Check for initial reasons to skip
             if not compound.explore():
                 continue
-            if compound.id().string() in self._completed:
+            compound_id = compound.id()
+            str_compound_id = str(compound_id)
+            if str_compound_id in self._completed:
+                continue
+            if not self.aggregate_filter.filter(compound):
+                self._completed.add(str_compound_id)  # add filtered out to completed to avoid many filter evaluations
                 continue
 
             # ============================== #
             #  Conformer Guess Generation    #
             # ============================== #
             has_guesses = False
             selection = {
                 "$and": [
                     {"job.order": self.options.conformer_job.order},
-                    {"auxiliaries": {"compound": {"$oid": compound.id().string()}}},
+                    {"auxiliaries": {"compound": {"$oid": str_compound_id}}},
                 ]
                 + model_query(self.options.model)
             }
             hit = self._calculations.get_one_calculation(dumps(selection))
             if hit is not None:
                 conformer_generation = hit
                 conformer_generation.link(self._calculations)
@@ -139,15 +174,15 @@
                 # Generate a conformer job if there was none
                 centroid = db.Structure(compound.get_centroid())
                 centroid.link(self._structures)
                 # Setup conformer generation
                 conformer_generation = db.Calculation()
                 conformer_generation.link(self._calculations)
                 conformer_generation.create(self.options.model, self.options.conformer_job, [centroid.id()])
-                conformer_generation.set_auxiliary("compound", compound.id())
+                conformer_generation.set_auxiliary("compound", compound_id)
                 if self.options.conformer_settings:
                     conformer_generation.set_settings(self.options.conformer_settings)
                 conformer_generation.set_status(db.Status.HOLD)
                 # Continue as there can not be any guesses yet
                 continue
 
             # ====================== #
@@ -177,14 +212,17 @@
                         minimization.link(self._calculations)
                         minimization.create(model, self.options.minimization_job, [guess])
                         # Sleep a bit in order not to make the DB choke
                         time.sleep(0.001)
                         if self.options.minimization_settings:
                             minimization.set_settings(self.options.minimization_settings)
                         minimization.set_status(db.Status.HOLD)
+                        guess_structure = db.Structure(guess)
+                        guess_structure.link(self._structures)
+                        guess_structure.add_calculation("geometry_optimization", minimization.get_id())
                         time.sleep(0.001)
                     else:
                         minimization = hit
                         minimization.link(self._calculations)
                         if minimization.get_status() == db.Status.FAILED:
                             # Failed optimizations shall not stop the completion
                             optimized_structures += 1
@@ -196,30 +234,32 @@
                         else:
                             optimized_structures += 1
 
                 # If all optimizations are done mark this compound as complete
                 if optimized_structures == len(conformer_guesses):
                     self._complete_compound(compound)
 
-    def _complete_compound(self, compound):
-        import math
+    def _complete_compound(self, compound: db.Compound):
         beta = 1 / (utils.BOLTZMANN_CONSTANT / utils.JOULE_PER_HARTREE * self.options.temperature)
         # Use the energy of the first structure as the energy 0-point. Otherwise, we likely have an overflow of the
         # exponential factor below (exp(- beta * energy).
-        reference_energy = 0.0
+        reference_energy = None
         for sid in compound.get_structures():
             structure = db.Structure(sid, self._structures)
             if not structure.has_property("electronic_energy"):
                 continue
             energy_property = structure.query_properties("electronic_energy", self.options.model, self._properties)
+            if not energy_property:
+                raise RuntimeError(f"Could not find electronic energy for structure {sid}, "
+                                   f"something might be wrong with the model for {self.name}:\n{self.options.model}")
             prop = db.NumberProperty(energy_property[-1], self._properties)
             energy = prop.get_data()
-            if reference_energy == 0.0:
+            if reference_energy is None:
                 reference_energy = energy
             energy -= reference_energy
             temperature_model = db.Model.__copy__(self.options.model)
             temperature_model.temperature = self.options.temperature
-            boltzmann_property = db.NumberProperty.make("boltzmann_weight", self.options.model,
+            boltzmann_property = db.NumberProperty.make("boltzmann_weight", temperature_model,
                                                         math.exp(-beta * energy), self._properties)
             boltzmann_property.set_comment("Energy 0-point: " + str(reference_energy))
             structure.add_property("boltzmann_weight", boltzmann_property.id())
-        self._completed.append(compound.id())
+        self._completed.add(str(compound.id()))
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/trial_generator/bond_based.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/trial_generator/bond_based.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
 import time
-from copy import deepcopy
+from collections import defaultdict
 from typing import List, Optional, Tuple, Union, Dict
 from itertools import combinations, product
 from scipy.special import comb
 
 # Third party imports
+from numpy import ndarray
 import scine_database as db
 import scine_utilities as utils
 import scine_molassembler as masm
 
 # Local application imports
 from ....utilities.queries import calculation_exists_in_structure, get_calculation_id
-from ..reactive_site_filters import ReactiveSiteFilter
 from .connectivity_analyzer import ReactionType, ConnectivityAnalyzer
-from . import TrialGenerator
+from . import TrialGenerator, _sanity_check_wrapper
 
 
 class BondBased(TrialGenerator):
     """
     Class to generate reactive complex calculations via bond-based approaches.
 
     Attributes
@@ -33,20 +33,20 @@
     options : BondBased.Options
         The options for generating reactive complex calculations.
     reactive_site_filter : ReactiveSiteFilter
         The filter applied to determine reactive sites, reactive pairs and trial
         reaction coordinates.
     """
 
-    class Options:
+    class Options(TrialGenerator.Options):
         """
         The options for bond-based reactive complex enumeration.
         """
 
-        __slots__ = ("model", "unimolecular", "bimolecular")
+        __slots__ = ("unimolecular_options", "bimolecular_options")
 
         class BimolOptions:
             """
             The options for the generation and exploration of bimolecular reactions.
 
             NOTE: The minimum and maximum bounds regarding the number of bonds to
             be modified/formed/broken have to be understood as strict limitations.
@@ -250,82 +250,56 @@
                     Additional settings passed to Calculation evaluating the possible
                     reactions. These settings are passed to all calculations for which
                     all of the reactive atom pairs are bound in the start structure
                     and cutting them apart would result into at least two separate molecules.
                     Empty by default.
                 """
 
-        def __init__(self):
-            self.model: db.Model = db.Model("PM6", "PM6", "")
-            """
-            db.Model (Scine::Database::Model)
-                The Model used to evaluate the possible reactions.
-                The default is: PM6 using Sparrow.
-            """
-            self.unimolecular = self.UnimolOptions()
+        def __init__(self, parent: Optional[TrialGenerator] = None):
+            super().__init__(parent)
+            self.unimolecular_options = self.UnimolOptions()
             """
             UnimolOptions
                 The options for reactions involving a single molecule.
             """
-            self.bimolecular = self.BimolOptions()
+            self.bimolecular_options = self.BimolOptions()
             """
             BimolOptions
                 The options for reactions involving two molecules, that are set up
                 to be associative in nature.
             """
 
-    def __init__(self):
-        super().__init__()
-        self.options = self.Options()
-        self.reactive_site_filter: ReactiveSiteFilter = ReactiveSiteFilter()
-
-    def _sanity_check_configuration(self):
-        if not isinstance(self.reactive_site_filter, ReactiveSiteFilter):
-            raise TypeError("Expected a ReactiveSiteFilter (or a class derived "
-                            "from it) in BondBased.reactive_site_filter.")
-
-    def bimolecular_reactions(self, structure_list: List[db.Structure]):
-        """
-        Creates reactive complex calculations corresponding to the bimolecular
-        reactions between the structures if there is not already a calculation
-        to search for a reaction of the same structures with the same job order.
-
-        Parameters
-        ----------
-        structure_list :: List[db.Structure]
-            List of the two structures to be considered.
-            The Structures have to be linked to a database.
-        """
-        self._sanity_check_configuration()
-        # Check number of compounds
-        if len(structure_list) != 2:
-            raise RuntimeError("Exactly two structures are needed for setting up a bimolecular reaction.")
+    def clear_cache(self):
+        pass
 
-        structure_id_list = [s.id() for s in structure_list]
+    @_sanity_check_wrapper
+    def bimolecular_coordinates(self, structure_list: List[db.Structure], with_exact_settings_check: bool = False) \
+            -> Dict[
+        Tuple[List[Tuple[int, int]], int],
+        List[Tuple[ndarray, ndarray, float, float]]
+    ]:
 
-        # If there is a reactive complex calculation for the same structures, return
-        if calculation_exists_in_structure(self.options.bimolecular.job.order, structure_id_list, self.options.model,
-                                           self._structures, self._calculations):
-            return
+        if self._quick_bimolecular_already_exists(structure_list, do_fast_query=not with_exact_settings_check):
+            return {}
 
         # Get reactive atoms
-        reactive_atoms1 = self.reactive_site_filter.filter_atoms(
-            [structure_list[0]], list(range(structure_list[0].get_atoms().size()))
-        )
-        reactive_atoms2 = self.reactive_site_filter.filter_atoms(
-            [structure_list[1]], list(range(structure_list[1].get_atoms().size()))
+        n_atoms1 = structure_list[0].get_atoms().size()
+        n_atoms2 = structure_list[1].get_atoms().size()
+        reactive_atoms = self.reactive_site_filter.filter_atoms(
+            structure_list, list(range(n_atoms1)) + [i + n_atoms1 for i in range(n_atoms2)]
         )
+        reactive_atoms1 = [i for i in reactive_atoms if i < n_atoms1]
+        reactive_atoms2 = [i - n_atoms1 for i in reactive_atoms if i >= n_atoms1]
 
-        n_atoms1 = structure_list[0].get_atoms().size()
         # If needed get reactive intrastructural coordinates for both structures
         # split into formation and dissociation
-        allows_intra_reactions = (self.options.bimolecular.max_intra_bond_formations > 0 or
-                                  self.options.bimolecular.max_bond_dissociations > 0)
-        will_probe_intra_reactions = (self.options.bimolecular.max_bond_modifications >
-                                      self.options.bimolecular.min_inter_bond_formations)
+        allows_intra_reactions = (self.options.bimolecular_options.max_intra_bond_formations > 0 or
+                                  self.options.bimolecular_options.max_bond_dissociations > 0)
+        will_probe_intra_reactions = (self.options.bimolecular_options.max_bond_modifications >
+                                      self.options.bimolecular_options.min_inter_bond_formations)
         if allows_intra_reactions and will_probe_intra_reactions:
             filtered_form_pairs1, filtered_diss_pairs1 = self._get_filtered_intraform_and_diss(
                 structure_list[0], reactive_atoms1
             )
             filtered_form_pairs2, filtered_diss_pairs2 = self._get_filtered_intraform_and_diss(
                 structure_list[1], reactive_atoms2
             )
@@ -341,201 +315,248 @@
 
         # Generate reactive pair combinations across the two structures from reactive sites
         shifted_inter_pairs = list(product(reactive_atoms1, (idx + n_atoms1 for idx in reactive_atoms2)))
         filtered_shifted_inter_pairs = self.reactive_site_filter.filter_atom_pairs(
             structure_list, shifted_inter_pairs)
         filtered_unshifted_inter_pairs = [(pair[0], pair[1] - n_atoms1) for pair in filtered_shifted_inter_pairs]
         # Loop through all allowed combinations of inter/intra bond formations and dissociations
-        true_max_inter_bond_formations = min(self.options.bimolecular.max_inter_bond_formations,
-                                             self.options.bimolecular.max_bond_modifications)
-        true_max_intra_bond_formations = min(self.options.bimolecular.max_intra_bond_formations,
-                                             self.options.bimolecular.max_bond_modifications)
-        true_max_bond_dissociations = min(self.options.bimolecular.max_bond_dissociations,
-                                          self.options.bimolecular.max_bond_modifications)
-        range_inter = range(self.options.bimolecular.min_inter_bond_formations, true_max_inter_bond_formations + 1)
-        range_intra = range(self.options.bimolecular.min_intra_bond_formations, true_max_intra_bond_formations + 1)
-        range_diss = range(self.options.bimolecular.min_bond_dissociations, true_max_bond_dissociations + 1)
+        true_max_inter_bond_formations = min(self.options.bimolecular_options.max_inter_bond_formations,
+                                             self.options.bimolecular_options.max_bond_modifications)
+        true_max_intra_bond_formations = min(self.options.bimolecular_options.max_intra_bond_formations,
+                                             self.options.bimolecular_options.max_bond_modifications)
+        true_max_bond_dissociations = min(self.options.bimolecular_options.max_bond_dissociations,
+                                          self.options.bimolecular_options.max_bond_modifications)
+        range_inter = range(
+            self.options.bimolecular_options.min_inter_bond_formations,
+            true_max_inter_bond_formations + 1)
+        range_intra = range(
+            self.options.bimolecular_options.min_intra_bond_formations,
+            true_max_intra_bond_formations + 1)
+        range_diss = range(self.options.bimolecular_options.min_bond_dissociations,
+                           true_max_bond_dissociations + 1)
+
+        result: Dict[
+            Tuple[List[Tuple[int, int]], int],
+            List[Tuple[ndarray, ndarray, float, float]]
+        ] = {}
         for n_inter_form, n_intra_form, n_diss in product(range_inter, range_intra, range_diss):
             s = n_inter_form + n_intra_form + n_diss
-            if s > self.options.bimolecular.max_bond_modifications:
+            if s > self.options.bimolecular_options.max_bond_modifications:
                 continue
-            elif s < self.options.bimolecular.min_bond_modifications:
+            elif s < self.options.bimolecular_options.min_bond_modifications:
                 continue
 
             # Batch all trials before doing a final filter run and adding
             #  the remaining trials. This reduces the number of filter calls
             #  and thus the number of DB look-ups.
-            batch: Dict[tuple, List[tuple]] = {}
 
-            def work_batch(self, n_diss):
-                nonlocal structure_list, structure_id_list
-                nonlocal batch
-                filter_result = self.reactive_site_filter.filter_reaction_coordinates(
-                    structure_list,
-                    batch.keys()
-                )
-                new_calculation_ids = []
-                for pairs in filter_result:
-                    for align1, align2, rot, spread in batch[pairs]:
-                        cid = self._add_reactive_complex_calculation(
-                            structure_id_list,
-                            pairs[:len(pairs) - n_diss],
-                            pairs[len(pairs) - n_diss:],
-                            self.options.bimolecular.job,
-                            self.options.bimolecular.job_settings,
-                            list(align1),
-                            list(align2),
-                            rot,
-                            spread,
-                            0.0,
-                        )
-                        if cid is not None:
-                            new_calculation_ids.append(cid)
-                if new_calculation_ids:
-                    for s in structure_list:
-                        s.add_calculations(self.options.bimolecular.job.order, [new_calculation_ids[0]])
+            # keys: List of pairs
+            # values: information required to build different reactive complexes
+            batch: Dict[
+                Tuple[Tuple[int, int], ...],
+                List[Tuple[ndarray, ndarray, float, float]]
+            ] = defaultdict(list)
 
             reactive_inter_coords = list(combinations(filtered_unshifted_inter_pairs, n_inter_form))
             for (inter_coord, align1, align2, rot, spread, ) in \
-                    self.options.bimolecular.complex_generator.generate_reactive_complexes(
+                    self.options.bimolecular_options.complex_generator.generate_reactive_complexes(
                         structure_list[0], structure_list[1], reactive_inter_coords):
 
                 # Shift to complex indexing
                 shifted_inter_coord = tuple((pair[0], pair[1] + n_atoms1) for pair in inter_coord)
 
                 for intra_form_pairs in combinations(all_filtered_intra_form_pairs, n_intra_form):
                     for diss_pairs in combinations(all_filtered_diss_pairs, n_diss):
 
                         form_pairs = shifted_inter_coord + intra_form_pairs
                         key = form_pairs + diss_pairs
-                        if key in batch:
-                            batch[key].append((align1, align2, rot, spread))
-                        else:
-                            batch[key] = [(align1, align2, rot, spread)]
-                        if len(batch) > 9999:
-                            work_batch(self, n_diss)
-                            batch = {}
-
-            # Add remaining batched trials to DB
-            work_batch(self, n_diss)
-            batch = {}
-        return
+                        batch[key].append((align1, align2, rot, spread))
+
+            filter_result = self.reactive_site_filter.filter_reaction_coordinates(
+                structure_list,
+                list(batch.keys())
+            )
+            for filtered in filter_result:
+                result[(filtered, n_diss)] = batch[filtered]
+        return result
+
+    @_sanity_check_wrapper
+    def bimolecular_reactions(self, structure_list: List[db.Structure], with_exact_settings_check: bool = False):
+        """
+        Creates reactive complex calculations corresponding to the bimolecular
+        reactions between the structures if there is not already a calculation
+        to search for a reaction of the same structures with the same job order.
+
+        Parameters
+        ----------
+        structure_list :: List[db.Structure]
+            List of the two structures to be considered.
+            The Structures have to be linked to a database.
+        with_exact_settings_check :: bool
+            If True, more expensive queries are carried out to check if the settings of the
+            calculations are exactly the same as the settings of the trial generator. This allows to add more
+            inclusive additional reaction trials but the queries are less efficient, therefore this option
+            should be only toggled if necessary.
+        """
+        # already includes quick check for existing calculation
+        coordinate_complex_build_info = self.bimolecular_coordinates(structure_list, with_exact_settings_check)
+        if not coordinate_complex_build_info:
+            return
+        structure_id_list = [s.id() for s in structure_list]
+        new_calculation_ids = []
+        for (pairs, n_diss), complexes in coordinate_complex_build_info.items():
+            for align1, align2, rot, spread in complexes:
+                cid = self._add_reactive_complex_calculation(
+                    structure_id_list,
+                    pairs[:len(pairs) - n_diss],
+                    pairs[len(pairs) - n_diss:],
+                    self.options.bimolecular_options.job,
+                    self.options.bimolecular_options.job_settings,
+                    list(align1),
+                    list(align2),
+                    rot,
+                    spread,
+                    0.0,
+                    check_for_existing=with_exact_settings_check
+                )
+                if cid is not None:
+                    new_calculation_ids.append(cid)
+                else:
+                    print("No new calculation added")
+        if new_calculation_ids:
+            for s in structure_list:
+                s.add_calculations(self.options.bimolecular_options.job.order, [new_calculation_ids[0]])
 
-    def unimolecular_reactions(self, structure: db.Structure):
+    @_sanity_check_wrapper
+    def unimolecular_reactions(self, structure: db.Structure, with_exact_settings_check: bool = False):
         """
         Creates reactive complex calculations corresponding to the unimolecular
         reactions of the structure if there is not already a calculation to
         search for a reaction of the same structure with the same job order.
 
         Parameters
         ----------
         structure :: db.Structure
             The structure to be considered. The Structure has to
             be linked to a database.
-        """
-        self._sanity_check_configuration()
+        with_exact_settings_check :: bool
+            If True, more expensive queries are carried out to check if the settings of the
+            calculations are exactly the same as the settings of the trial generator. This allows to add more
+            inclusive additional reaction trials but the queries are less efficient, therefore this option
+            should be only toggled if necessary.
+        """
+        # already includes quick check for existing calculation
+        filtered_coordinates_per_ndiss = self.unimolecular_coordinates(structure, with_exact_settings_check)
+        if not filtered_coordinates_per_ndiss:
+            return
+        structure_id = structure.id()
+        connectivity_analyzer = ConnectivityAnalyzer(structure)
+        new_calculation_ids = []
+        for filter_result, n_diss in filtered_coordinates_per_ndiss:
+            for pairs in filter_result:
+                # Get reaction type:
+                reaction_type = connectivity_analyzer.get_reaction_type(pairs)
+                # Set up reactive complex calculation
+                if reaction_type in (ReactionType.Associative, ReactionType.Mixed):
+                    settings = self.options.unimolecular_options.job_settings_associative
+                elif reaction_type == ReactionType.Dissociative:
+                    settings = self.options.unimolecular_options.job_settings_dissociative
+                elif reaction_type == ReactionType.Disconnective:
+                    settings = self.options.unimolecular_options.job_settings_disconnective
+                else:
+                    raise RuntimeError(f"Unknown reaction type {reaction_type}")
+
+                cid = self._add_reactive_complex_calculation(
+                    [structure_id],
+                    pairs[:len(pairs) - n_diss],
+                    pairs[len(pairs) - n_diss:],
+                    self.options.unimolecular_options.job,
+                    settings,
+                    check_for_existing=with_exact_settings_check
+                )
+                if cid is not None:
+                    new_calculation_ids.append(cid)
+        if new_calculation_ids:
+            structure.add_calculations(self.options.unimolecular_options.job.order, [new_calculation_ids[0]])
+
+    def _quick_unimolecular_already_exists(self, structure: db.Structure, do_fast_query: bool) -> bool:
         # Rule out compounds too small for intramolecular reactions right away
         atoms = structure.get_atoms()
-        structure_id = structure.id()
-        # No intramolecular reactions for monoatomic compounds
         if atoms.size() == 1:
-            return
-        if atoms.size() == 2 and self.options.unimolecular.max_bond_dissociations < 1:
-            return
+            return False
+        if atoms.size() == 2 and self.options.unimolecular_options.max_bond_dissociations < 1:
+            return False
+        return do_fast_query and calculation_exists_in_structure(
+            self.options.unimolecular_options.job.order,
+            [structure.id()],
+            self.options.model,
+            self._structures,
+            self._calculations)
 
-        # Check whether there is a reactive complex calculation for the same structure already
-        if calculation_exists_in_structure(self.options.unimolecular.job.order, [structure_id], self.options.model,
-                                           self._structures, self._calculations):
-            return
+    def _quick_bimolecular_already_exists(self, structure_list: List[db.Structure], do_fast_query: bool) -> bool:
+        # Check number of compounds
+        if len(structure_list) != 2:
+            raise RuntimeError("Exactly two structures are needed for setting up a bimolecular reaction.")
+        return do_fast_query and calculation_exists_in_structure(
+            self.options.bimolecular_options.job.order,
+            [s.id() for s in structure_list],
+            self.options.model,
+            self._structures,
+            self._calculations)
+
+    @_sanity_check_wrapper
+    def unimolecular_coordinates(self, structure: db.Structure, with_exact_settings_check: bool = False) \
+            -> List[Tuple[List[List[Tuple[int, int]]], int]]:
+        if self._quick_unimolecular_already_exists(structure, do_fast_query=not with_exact_settings_check):
+            return []
 
+        atoms = structure.get_atoms()
         # Get all reactive atoms
         reactive_atoms = self.reactive_site_filter.filter_atoms([structure], list(range(atoms.size())))
         # Get all ordered pairs of reactive atoms
         connectivity_analyzer = ConnectivityAnalyzer(structure)
         filtered_form_pairs, filtered_diss_pairs = self._get_filtered_intraform_and_diss(
             structure, reactive_atoms, connectivity_analyzer
         )
 
         # Loop over all allowed combinations of association and dissociation counts
-        true_max_bond_formations = min(self.options.unimolecular.max_bond_formations,
-                                       self.options.unimolecular.max_bond_modifications)
-        true_max_bond_dissociations = min(self.options.unimolecular.max_bond_dissociations,
-                                          self.options.unimolecular.max_bond_modifications)
-        range_asso = range(self.options.unimolecular.min_bond_formations, true_max_bond_formations + 1)
-        range_diss = range(self.options.unimolecular.min_bond_dissociations, true_max_bond_dissociations + 1)
+        true_max_bond_formations = min(self.options.unimolecular_options.max_bond_formations,
+                                       self.options.unimolecular_options.max_bond_modifications)
+        true_max_bond_dissociations = min(self.options.unimolecular_options.max_bond_dissociations,
+                                          self.options.unimolecular_options.max_bond_modifications)
+        range_asso = range(self.options.unimolecular_options.min_bond_formations, true_max_bond_formations + 1)
+        range_diss = range(self.options.unimolecular_options.min_bond_dissociations,
+                           true_max_bond_dissociations + 1)
+
+        result = []
         for n_asso, n_diss in product(range_asso, range_diss):
             s = n_asso + n_diss
-            if s > self.options.unimolecular.max_bond_modifications:
+            if s > self.options.unimolecular_options.max_bond_modifications:
                 continue
-            elif s < self.options.unimolecular.min_bond_modifications:
+            elif s < self.options.unimolecular_options.min_bond_modifications:
                 continue
 
             # Batch all trials before doing a final filter run and adding the
             #  remaining trials. This reduces the number of filter calls and
             #  thus the number of DB look-ups.
             batch: List[tuple] = []
-
-            def work_batch(self, n_diss):
-                nonlocal structure, structure_id, connectivity_analyzer, batch
-                # Filter current pairs combinations
-                filter_result = self.reactive_site_filter.filter_reaction_coordinates(
-                    [structure],
-                    batch
-                )
-                new_calculation_ids = []
-                for pairs in filter_result:
-                    # Get reaction type:
-                    reaction_type = connectivity_analyzer.get_reaction_type(pairs)
-                    # Set up reactive complex calculation
-                    if reaction_type in (ReactionType.Associative, ReactionType.Mixed):
-                        cid = self._add_reactive_complex_calculation(
-                            [structure_id],
-                            pairs[:len(pairs) - n_diss],
-                            pairs[len(pairs) - n_diss:],
-                            self.options.unimolecular.job,
-                            self.options.unimolecular.job_settings_associative,
-                        )
-                        if cid is not None:
-                            new_calculation_ids.append(cid)
-                    elif reaction_type == ReactionType.Dissociative:
-                        cid = self._add_reactive_complex_calculation(
-                            [structure_id],
-                            pairs[:len(pairs) - n_diss],
-                            pairs[len(pairs) - n_diss:],
-                            self.options.unimolecular.job,
-                            self.options.unimolecular.job_settings_dissociative,
-                        )
-                        if cid is not None:
-                            new_calculation_ids.append(cid)
-                    elif reaction_type == ReactionType.Disconnective:
-                        cid = self._add_reactive_complex_calculation(
-                            [structure_id],
-                            pairs[:len(pairs) - n_diss],
-                            pairs[len(pairs) - n_diss:],
-                            self.options.unimolecular.job,
-                            self.options.unimolecular.job_settings_disconnective,
-                        )
-                        if cid is not None:
-                            new_calculation_ids.append(cid)
-                if new_calculation_ids:
-                    structure.add_calculations(self.options.unimolecular.job.order, [new_calculation_ids[0]])
-
             # Loop over all allowed combinations of reaction coordinates within
             #  the current count of associations and dissociations
             for asso_pairs in combinations(filtered_form_pairs, n_asso):
                 for diss_pairs in combinations(filtered_diss_pairs, n_diss):
                     batch += [asso_pairs + diss_pairs]
-                    if len(batch) > 9999:
-                        work_batch(self, n_diss)
-                        batch = []
-            work_batch(self, n_diss)
-            batch = []
+            filter_result = self.reactive_site_filter.filter_reaction_coordinates(
+                [structure],
+                batch
+            )
+            result.append((filter_result, n_diss))
 
-        return
+        return result
 
+    @_sanity_check_wrapper
     def estimate_n_unimolecular_trials(
         self, structure_file: str, n_reactive_bound_pairs: int = -1, n_reactive_unbound_pairs: int = -1
     ):
         """
         Estimates the number of unimolecular reactive coordinate trials expected
         to arise directly (i.e. as single step elementary reaction trials) from
         the given structure without taking reactive site filters into account.
@@ -561,43 +582,45 @@
 
         Returns
         -------
         int
             The number of reactive trial coordinates expected to arise from this
             structure.
         """
-        self._sanity_check_configuration()
         # Read in atom collection and interpret connectivity from interatomic distances
         atoms = utils.io.read(structure_file)[0]
         n_unbound_pairs, n_bound_pairs = self._get_bound_unbound_pairs_from_atoms(
             atoms, n_reactive_bound_pairs, n_reactive_unbound_pairs
         )
 
         # Get all types of bond modification patterns that are compliant with the options
         # and add the associated number of trials
         n_trials = 0
         for n_form in range(
-            self.options.unimolecular.min_bond_formations, self.options.unimolecular.max_bond_formations + 1
+            self.options.unimolecular_options.min_bond_formations,
+                self.options.unimolecular_options.max_bond_formations + 1
         ):
             for n_diss in range(
-                self.options.unimolecular.min_bond_dissociations, self.options.unimolecular.max_bond_dissociations + 1
+                self.options.unimolecular_options.min_bond_dissociations,
+                    self.options.unimolecular_options.max_bond_dissociations + 1
             ):
                 if not (
-                    self.options.unimolecular.min_bond_modifications
+                    self.options.unimolecular_options.min_bond_modifications
                     <= n_form + n_diss
-                    <= self.options.unimolecular.max_bond_modifications
+                    <= self.options.unimolecular_options.max_bond_modifications
                 ):
                     continue
                 n_form_combis = comb(n_unbound_pairs, n_form)
                 n_diss_combis = comb(n_bound_pairs, n_diss)
                 n_form_diss_combis = n_form_combis * n_diss_combis
                 n_trials += n_form_diss_combis
 
         return n_trials
 
+    @_sanity_check_wrapper
     def estimate_n_bimolecular_trials(
         self,
         structure_file1: str,
         structure_file2: str,
         attack_points_per_site: int = 3,
         n_inter_reactive_pairs: int = -1,
         n_reactive_bound_pairs1: int = -1,
@@ -664,15 +687,14 @@
 
         Returns
         -------
         int
             The number of reactive trial coordinates expected to arise from this
             structure.
         """
-        self._sanity_check_configuration()
         # Read in atom collections and get intramolecular bound and unbound pairs
         atoms1 = utils.io.read(structure_file1)[0]
         n_unbound_pairs1, n_bound_pairs1 = self._get_bound_unbound_pairs_from_atoms(
             atoms1, n_reactive_bound_pairs1, n_reactive_unbound_pairs1
         )
         atoms2 = utils.io.read(structure_file2)[0]
         n_unbound_pairs2, n_bound_pairs2 = self._get_bound_unbound_pairs_from_atoms(
@@ -682,53 +704,55 @@
         n_bound_pairs = n_bound_pairs1 + n_bound_pairs2
         n_unbound_pairs = n_unbound_pairs1 + n_unbound_pairs2
 
         # Get all types of bond modification patterns that are compliant with the options
         # and add the associated number of trials
         n_trials = 0
         # At least on intermolecular coord required
-        if self.options.bimolecular.max_inter_bond_formations < 1:
+        if self.options.bimolecular_options.max_inter_bond_formations < 1:
             return 0
 
         for n_inter in range(
-            self.options.bimolecular.min_inter_bond_formations, self.options.bimolecular.max_inter_bond_formations + 1
+            self.options.bimolecular_options.min_inter_bond_formations,
+                self.options.bimolecular_options.max_inter_bond_formations + 1
         ):
             for n_form in range(
-                self.options.bimolecular.min_intra_bond_formations,
-                self.options.bimolecular.max_intra_bond_formations + 1,
+                self.options.bimolecular_options.min_intra_bond_formations,
+                    self.options.bimolecular_options.max_intra_bond_formations + 1,
             ):
                 for n_diss in range(
-                    self.options.bimolecular.min_bond_dissociations, self.options.bimolecular.max_bond_dissociations + 1
+                    self.options.bimolecular_options.min_bond_dissociations,
+                        self.options.bimolecular_options.max_bond_dissociations + 1
                 ):
                     if not (
-                        self.options.bimolecular.min_bond_modifications
+                        self.options.bimolecular_options.min_bond_modifications
                         <= n_form + n_diss + n_inter
-                        <= self.options.bimolecular.max_bond_modifications
+                        <= self.options.bimolecular_options.max_bond_modifications
                     ):
                         continue
                     n_inter_combis = comb(n_inter_pairs, n_inter)
                     n_form_combis = comb(n_unbound_pairs, n_form)
                     n_diss_combis = comb(n_bound_pairs, n_diss)
                     n_form_diss_combis = n_form_combis * n_diss_combis * n_inter_combis
 
                     # Add rotamers
                     if n_inter == 1:
-                        n_form_diss_combis *= self.options.bimolecular.complex_generator.options.number_rotamers
+                        n_form_diss_combis *= self.options.bimolecular_options.complex_generator.options.number_rotamers
                     # There can be two intermolecular coordinates involving the same atom twice (e.g. "atom on bond")
                     # These are weighted with number_rotamers in the real enumeration but with
                     # number_rotamers_two_on_two here
                     elif n_inter == 2:
                         n_form_diss_combis *= (
-                            self.options.bimolecular.complex_generator.options.number_rotamers_two_on_two
+                            self.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two
                         )
 
                     n_trials += n_form_diss_combis
 
         # Take into account estimate of attack points per site
-        if self.options.bimolecular.complex_generator.options.multiple_attack_points:
+        if self.options.bimolecular_options.complex_generator.options.multiple_attack_points:
             n_trials *= attack_points_per_site * attack_points_per_site
         return n_trials
 
     def _add_reactive_complex_calculation(
         self,
         reactive_structures: List[db.ID],
         association_pairs: List[Tuple[int, int]],
@@ -803,51 +827,53 @@
             settings and model already exists or not (default: False)
 
         Returns
         -------
         calculation :: scine_database.ID
             A calculation that is on hold.
         """
+        this_settings = self._get_settings(settings)
         if lhs_alignment is not None:
-            settings["rc_x_alignment_0"] = lhs_alignment
+            this_settings["rc_x_alignment_0"] = lhs_alignment
         if rhs_alignment is not None:
-            settings["rc_x_alignment_1"] = rhs_alignment
+            this_settings["rc_x_alignment_1"] = rhs_alignment
         if x_rotation is not None:
-            settings["rc_x_rotation"] = x_rotation
+            this_settings["rc_x_rotation"] = x_rotation
         if spread is not None:
-            settings["rc_x_spread"] = spread
+            this_settings["rc_x_spread"] = spread
         if displacement is not None:
-            settings["rc_displacement"] = displacement
+            this_settings["rc_displacement"] = displacement
         if multiplicity is not None:
-            settings["rc_spin_multiplicity"] = multiplicity
+            this_settings["rc_spin_multiplicity"] = multiplicity
         if charge is not None:
-            settings["rc_molecular_charge"] = charge
+            this_settings["rc_molecular_charge"] = charge
 
         if job.order == "scine_react_complex_nt2":
             # nt2 job takes lists of integer where elements 0/1, 2/3 ... N-1, N are combined with each other
             # Flatten pair lists
-            settings["nt_nt_associations"] = [idx for idx_pair in association_pairs for idx in idx_pair]
-            settings["nt_nt_dissociations"] = [idx for idx_pair in dissociation_pairs for idx in idx_pair]
+            this_settings["nt_nt_associations"] = [idx for idx_pair in association_pairs for idx in idx_pair]
+            this_settings["nt_nt_dissociations"] = [idx for idx_pair in dissociation_pairs for idx in idx_pair]
         else:
             raise RuntimeError(
                 "Only 'scine_react_complex_nt2' order supported for bond-based reactive complex calculations."
             )
 
         if len(reactive_structures) > 1:
-            settings["rc_minimal_spin_multiplicity"] = bool(self.options.bimolecular.minimal_spin_multiplicity)
+            this_settings["rc_minimal_spin_multiplicity"] = bool(
+                self.options.bimolecular_options.minimal_spin_multiplicity)
 
         if check_for_existing and get_calculation_id(job.order, reactive_structures, self.options.model,
-                                                     self._calculations, settings=settings) is not None:
+                                                     self._calculations, settings=this_settings) is not None:
             return None
         calculation = db.Calculation()
         calculation.link(self._calculations)
         calculation.create(self.options.model, job, reactive_structures)
         # Sleep a bit in order not to make the DB choke
         time.sleep(0.001)
-        calculation.set_settings(deepcopy(settings))
+        calculation.set_settings(this_settings)
         calculation.set_status(db.Status.HOLD)
         return calculation.id()
 
     def _get_filtered_intraform_and_diss(
         self,
         structure: db.Structure,
         reactive_atoms: List[int],
@@ -937,7 +963,13 @@
                     "Atom collection contains more than one molecule according to distance-based bond orders."
                 )
             graph = graph_result.graphs[0]
 
         n_bound_pairs = graph.E if n_reactive_bound_pairs < 0 else n_reactive_bound_pairs
         n_unbound_pairs = n_pairs - graph.E if n_reactive_unbound_pairs < 0 else n_reactive_unbound_pairs
         return n_unbound_pairs, n_bound_pairs
+
+    def get_unimolecular_job_order(self) -> str:
+        return self.options.unimolecular_options.job.order
+
+    def get_bimolecular_job_order(self) -> str:
+        return self.options.bimolecular_options.job.order
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/trial_generator/connectivity_analyzer.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/trial_generator/connectivity_analyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,17 +79,15 @@
         component_idx_j, mol_idx_j = self.idx_map[atom2]
         # If different molecules not bound
         if component_idx_i != component_idx_j:
             return False
 
         # Same molecule
         assert mol_idx_i != mol_idx_j
-        if self.graphs[component_idx_i].adjacent(mol_idx_i, mol_idx_j):
-            return True
-        return False
+        return self.graphs[component_idx_i].adjacent(mol_idx_i, mol_idx_j)
 
     def get_reaction_type(self, reactive_pair_list: List[Tuple[int, int]]) -> ReactionType:
         """
         Determines what kind of intrastructural reaction
         (associative, dissociative, disconnective) a reactive complex guess
         describes.
 
@@ -128,24 +126,25 @@
             return Type.Associative
 
         # Mixed reaction type
         if associative_count > 0 and len(dissociated_bonds) > 0:
             return Type.Mixed
 
         # Now to distinguish dissociative and disconnective
+        dissociated_bonds = list(set(dissociated_bonds))
         modified_graphs = deepcopy(self.graphs)
         for c, bond in dissociated_bonds:
             if modified_graphs[c].can_remove(bond):
                 modified_graphs[c].remove_bond(bond)
             else:
                 return Type.Disconnective
 
         return Type.Dissociative
 
-    def get_adjacency_matrix(self):
+    def get_adjacency_matrix(self) -> lil_matrix:
         """
         Gets the adjacency matrix for the structure with the indices ordered as
         in the structure.
 
         Returns
         -------
         lil_matrix
@@ -194,15 +193,15 @@
 
         if component_idx1 != component_idx2:
             raise RuntimeError("Graph distance between different Molecules is not defined.")
         return masm.distance(mol_idx_1, self.graphs[component_idx1])[mol_idx_2]
 
     def _get_structure_idx(self, component_idx: int, mol_idx: int) -> int:
         """
-        Get the index of an atom in the structrue from its component index
+        Get the index of an atom in the structure from its component index
         and index in the molecule.
 
         Parameters
         ----------
         component_idx : int
             Which component/molecule the atom belongs to.
         mol_idx : int
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/trial_generator/fast_dissociations.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/trial_generator/fast_dissociations.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,37 +5,39 @@
 See LICENSE.txt for details.
 """
 
 # Standard library imports
 import time
 from copy import deepcopy
 from functools import wraps
-from typing import Callable, Dict, List, Optional, Tuple, Union
+from typing import Callable, Dict, List, Optional, Tuple, Union, Set
 from json import dumps
 from itertools import combinations
 from warnings import warn
 
 # Third party imports
+from numpy import ndarray
 import scine_database as db
 import scine_utilities as utils
 
 # Local application imports
 from ....utilities.queries import stop_on_timeout, get_calculation_id, select_calculation_by_structures
 from ....utilities.energy_query_functions import get_energy_sum_of_elementary_step_side, get_energy_for_structure
-from ..reactive_site_filters import ReactiveSiteFilter
+from ..reactive_site_filters import ReactiveSiteFilter, ReactiveSiteFilterAndArray, ReactiveSiteFilterOrArray
 from .connectivity_analyzer import ReactionType, ConnectivityAnalyzer
 from .bond_based import BondBased
-from ..trial_generator import TrialGenerator
+from ..trial_generator import TrialGenerator, _sanity_check_wrapper
 
 
 def single_structure_assertion(fun: Callable):
     """
     Makes sure that the first argument given to the function `fun` is either a list of db.Structure of len 1 or
     a single db.Structure and then calls the function with the list argument, throws TypeError otherwise
     """
+
     @wraps(fun)
     def _impl(self, structures: Union[List[db.Structure], db.Structure], *args):
         arg = structures
         if isinstance(structures, list):
             if len(structures) != 1:
                 raise TypeError(f"The method {fun.__name__} of the filter {self.__class__.__name__} is only supported"
                                 f"for single structure lists.")
@@ -51,19 +53,31 @@
 
 class FurtherExplorationFilter(ReactiveSiteFilter):
     """
     Class to evaluate if detailed dissociation exploration trials should be setup.
     This base class does not filter anything out.
     """
 
-    def __init__(self):
-        super().__init__()
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)  # required for multiple inheritance
         self._setting_key = 'dissociations'
         self._structure_property_key = 'dissociated_structures'
 
+    def __and__(self, o):
+        if not isinstance(o, FurtherExplorationFilter):
+            raise TypeError("FurtherExplorationFilter expects FurtherExplorationFilter "
+                            "(or derived class) to chain with.")
+        return FurtherExplorationFilterAndArray([self, o])
+
+    def __or__(self, o):
+        if not isinstance(o, FurtherExplorationFilter):
+            raise TypeError("FurtherExplorationFilter expects FurtherExplorationFilter "
+                            "(or derived class) to chain with.")
+        return FurtherExplorationFilterOrArray([self, o])
+
     def filter_atoms(self, _: List[db.Structure], atom_indices: List[int]) -> List[int]:
         return atom_indices
 
     def filter_atom_pairs(self, _: List[db.Structure], pairs: List[Tuple[int, int]]) -> List[Tuple[int, int]]:
         return pairs
 
     def filter_reaction_coordinates(self, _: List[db.Structure], coordinates: List[List[Tuple[int, int]]]) \
@@ -88,14 +102,16 @@
             calculation.link(self._calculations)
             dissociation = calculation.get_settings().get(self._setting_key)
             if dissociation is not None and dissociation in dissociations_list:
                 results = calculation.get_results()
                 if results.elementary_step_ids:
                     for step_id in results.elementary_step_ids:
                         step = db.ElementaryStep(step_id, self._elementary_steps)
+                        if not step.explore():
+                            continue
                         reactant_energy = get_energy_sum_of_elementary_step_side(step, db.Side.LHS, energy_type,
                                                                                  model, self._structures,
                                                                                  self._properties)
                         if reactant_energy is None:
                             continue
                         product_energy = get_energy_sum_of_elementary_step_side(step, db.Side.RHS, energy_type,
                                                                                 model, self._structures,
@@ -133,14 +149,54 @@
             if plain_energies:
                 energies.append(min(plain_energies) * utils.KJPERMOL_PER_HARTREE)
                 continue
             energies.append(None)
         return energies
 
 
+class FurtherExplorationFilterAndArray(FurtherExplorationFilter, ReactiveSiteFilterAndArray):
+    """
+    An array of logically 'and' connected filters.
+
+    Attributes
+    ----------
+    filters : List[FurtherExplorationFilter]
+        A list of filters to be combined.
+    """
+
+    def __init__(self, filters: Optional[List[Union[FurtherExplorationFilter, ReactiveSiteFilter]]] = None):
+        super().__init__(filters=filters)
+        assert filters is None or len(self._filters) == len(filters)
+        for f in self._filters:
+            if not isinstance(f, FurtherExplorationFilter) and not isinstance(f, ReactiveSiteFilter):
+                raise TypeError("FurtherExplorationFilterAndArray expects FurtherExplorationFilter "
+                                "(or derived class) to chain with.")
+        self._join_names(self._filters)
+
+
+class FurtherExplorationFilterOrArray(FurtherExplorationFilter, ReactiveSiteFilterOrArray):
+    """
+    An array of logically 'or' connected filters.
+
+    Attributes
+    ----------
+    filters : List[FurtherExplorationFilter]
+        A list of filters to be combined.
+    """
+
+    def __init__(self, filters: Optional[List[FurtherExplorationFilter]] = None):
+        super().__init__(filters=filters)
+        assert filters is None or len(self._filters) == len(filters)
+        for f in self._filters:
+            if not isinstance(f, FurtherExplorationFilter) and not isinstance(f, ReactiveSiteFilter):
+                raise TypeError("FurtherExplorationFilterOrArray expects FurtherExplorationFilter "
+                                "(or derived class) to chain with.")
+        self._join_names(self._filters)
+
+
 class AllBarrierLessDissociationsFilter(FurtherExplorationFilter):
     def __init__(self, model: db.Model, job_order: str):
         super().__init__()
         self.model = model
         self.job_order = job_order
 
     @single_structure_assertion
@@ -166,14 +222,16 @@
         }
         relevant_step_ids = []
         structure_id = structure.id()
         for reaction in self._reactions.query_reactions(dumps(selection)):
             step_ids = reaction.get_elementary_steps()
             for sid in step_ids:
                 step = db.ElementaryStep(sid, self._elementary_steps)
+                if not step.explore():
+                    continue
                 if step.get_type() != db.ElementaryStepType.BARRIERLESS:
                     # caveat: this relies on logic in reaction gear that we
                     # disable barrierless elementary steps if there is a regular one for the same reaction
                     continue
                 if structure_id in step.get_reactants(db.Side.LHS)[0]:
                     relevant_step_ids.append(sid)
         step_sele = {"results.elementary_steps": {"$in": [{"$oid": str(sid)} for sid in relevant_step_ids]}}
@@ -186,16 +244,15 @@
                 for coordinate, dissociation in zip(coordinates, dissociation_lists):
                     if calc_dissociation == dissociation:
                         filtered.append(coordinate)
         return filtered
 
 
 class ReactionCoordinateMaxDissociationEnergyFilter(FurtherExplorationFilter):
-    def __init__(self, max_dissociation_energy: float, energy_type: str,
-                 model: db.Model, job_order: str):
+    def __init__(self, max_dissociation_energy: float, energy_type: str, model: db.Model, job_order: str):
         super().__init__()
         self.max_dissociation_energy = max_dissociation_energy
         self.energy_type = energy_type
         self.model = model
         self.job_order = job_order
 
     @single_structure_assertion
@@ -225,269 +282,390 @@
     Attributes
     ----------
     options : FastDissociations.Options
         The options for generating dissociations.
     reactive_site_filter : ReactiveSiteFilter
         The filter applied to determine reactive sites, reactive pairs and trial
         reaction coordinates.
+    further_exploration_filter : FurtherExplorationFilter
+        An optional additional filter that can limit further exploration,
+        e.g. based on dissociation energies evaluated in the fast dissociation job.
+        The default filter does not filter any reaction coordinate.
     """
-    __slots__ = ("options", "reactive_site_filter")
 
-    class Options:
+    class Options(BondBased.Options):
         """
         The options for generating dissociations.
         """
 
-        def __init__(self, parent: Optional[TrialGenerator] = None):
-            self._parent = parent  # best be first member to be set, due to __setattr__
-            self.model: db.Model = db.Model("PM6", "PM6", "")
-            """
-            db.Model (Scine::Database::Model)
-                The Model used to evaluate the possible reactions.
-                The default is: PM6 using Sparrow.
-            """
-            self.cutting_job: db.Job = db.Job("scine_dissociation_cut")
-            """
-            db.Job (Scine::Database::Calculation::Job)
-                The Job used to evaluate the possible reactions.
-                The default is: the `scine_dissociation_cut`
-                order on a single core.
-            """
-            self.cutting_job_settings: utils.ValueCollection = utils.ValueCollection({})
-            """
-            utils.ValueCollection
-                Additional settings passed to Calculation evaluating the possible
-                reactions. These settings are passed to all calculations for which
-                all of the reactive atom pairs are bound in the start structure
-                and cutting them apart would result into at least two separate molecules.
-                Empty by default.
-            """
-            self.min_bond_dissociations = 1
-            """
-            int
-                The minimum number of bond dissociations to be
-                encouraged simultaneously during an elementary steps trial calculation.
-                By default 1.
-            """
-            self.max_bond_dissociations = 1
-            """
-            int
-                The maximum number of bond dissociations to be encouraged
-                simultaneously during an elementary steps trial calculation. By default 1.
-            """
-            self.enable_further_explorations: bool = False
-            """
-            bool
-                Whether the dissociations should also be explored with another more detailed job.
-            """
-            self.always_further_explore_dissociative_reactions: bool = True
-            """
-            bool
-                Whether reaction coordinates that only lead to a dissociative reaction type, i.e. bonds are broken,
-                but no two (or more) separate molecules are formed (based on the reaction coordinate), should
-                automatically be explored with the further exploration job.
-                This overrules 'enable_further_explorations' (but only for these reaction types)
-                and the further_exploration_filter is not applied to them.
-            """
-            self.further_exploration_filter = FurtherExplorationFilter()
-            """
-            FurtherExplorationFilter
-                An optional additional filter that can limit further exploration e.g. based on dissociation energies
-                evaluated in the fast dissociation job. The default filter does not filter any reaction coordinate.
-            """
-            self.further_job: db.Job = db.Job("scine_react_complex_nt2")
-            """
-            db.Job (Scine::Database::Calculation::Job)
-                The Job used to evaluate the possible reactions with more detailed PES scans.
-                Jobs with the order `scine_react_complex_nt2` are
-                supported. The default is: the `scine_react_complex_nt2`
-                order on a single core.
-            """
-            self.further_job_settings: utils.ValueCollection = utils.ValueCollection({})
-            """
-            utils.ValueCollection
-                Additional settings passed to Calculation evaluating the possible
-                reactions. These settings are passed to all further explorations and the dissociative
-                reaction coordinates.
-            """
+        class UnimolOptions(BondBased.Options.UnimolOptions):
+            __slots__ = (
+                "cutting_job_settings",
+                "enable_further_explorations",
+                "always_further_explore_dissociative_reactions",
+                "further_job",
+                "further_job_settings",
+                "_parent",
+                "_unusable_settings",
+            )
+
+            def __init__(self, parent: Optional[TrialGenerator] = None):
+                super().__init__()
+                self._parent = parent
+                self._unusable_settings: Set[str] = {
+                    "job_settings_associative",
+                    "job_settings_dissociative",
+                    "job_settings_disconnective",
+                    "min_bond_formations",
+                    "max_bond_formations",
+                }
+                self.job: db.Job = db.Job("scine_dissociation_cut")
+                """
+                db.Job (Scine::Database::Calculation::Job)
+                    The Job used to evaluate the possible reactions.
+                    The default is: the `scine_dissociation_cut`
+                    order on a single core.
+                """
+                self.cutting_job_settings: utils.ValueCollection = utils.ValueCollection({})
+                """
+                utils.ValueCollection
+                    Additional settings passed to Calculation evaluating the possible
+                    reactions. These settings are passed to all calculations for which
+                    all of the reactive atom pairs are bound in the start structure
+                    and cutting them apart would result into at least two separate molecules.
+                    Empty by default.
+                """
+                self.min_bond_dissociations = 1
+                """
+                int
+                    The minimum number of bond dissociations to be
+                    encouraged simultaneously during an elementary steps trial calculation.
+                    By default 1.
+                """
+                self.max_bond_dissociations = 1
+                """
+                int
+                    The maximum number of bond dissociations to be encouraged
+                    simultaneously during an elementary steps trial calculation. By default 1.
+                """
+                self.enable_further_explorations: bool = False
+                """
+                bool
+                    Whether the dissociations should also be explored with another more detailed job.
+                """
+                self.always_further_explore_dissociative_reactions: bool = True
+                """
+                bool
+                    Whether reaction coordinates that only lead to a dissociative reaction type, i.e. bonds are broken,
+                    but no two (or more) separate molecules are formed (based on the reaction coordinate), should
+                    automatically be explored with the further exploration job.
+                    This overrules 'enable_further_explorations' (but only for these reaction types)
+                    and the further_exploration_filter is not applied to them.
+                """
+                self.further_job: db.Job = db.Job("scine_react_complex_nt2")
+                """
+                db.Job (Scine::Database::Calculation::Job)
+                    The Job used to evaluate the possible reactions with more detailed PES scans.
+                    Jobs with the order `scine_react_complex_nt2` are
+                    supported. The default is: the `scine_react_complex_nt2`
+                    order on a single core.
+                """
+                self.further_job_settings: utils.ValueCollection = utils.ValueCollection({})
+                """
+                utils.ValueCollection
+                    Additional settings passed to Calculation evaluating the possible
+                    reactions. These settings are passed to all further explorations and the dissociative
+                    reaction coordinates.
+                """
+
+            def __setattr__(self, item, value):
+                """
+                Overwritten standard method to clear cache of options holding parent whenever an option is changed
+                """
+                super().__setattr__(item, value)
+                if hasattr(self, "_parent") and self._parent is not None:
+                    self._parent.clear_cache()
+                if hasattr(self, "_unusable_settings") and item in self._unusable_settings:
+                    raise NotImplementedError(f"The setting {item} is not implemented for "
+                                              f"{self._parent.__class__.__name__}")
+                # couple together modifications and dissociations
+                elif item == "min_bond_modifications":
+                    super().__setattr__("min_bond_dissociations", value)
+                elif item == "max_bond_modifications":
+                    super().__setattr__("max_bond_dissociations", value)
+                elif item == "min_bond_dissociations":
+                    super().__setattr__("min_bond_modifications", value)
+                elif item == "max_bond_dissociations":
+                    super().__setattr__("max_bond_modifications", value)
 
         def __setattr__(self, item, value):
             """
             Overwritten standard method to clear cache of options holding parent whenever an option is changed
             """
-            super().__setattr__(item, value)
-            if self._parent is not None:
+            # should include all options of the parent class
+            if item in ["_parent", "model", "unimolecular_options", "bimolecular_options", "base_job_settings"]:
+                super().__setattr__(item, value)
+            else:
+                self.unimolecular_options.__setattr__(item, value)
+            if hasattr(self, "_parent") and self._parent is not None:
                 self._parent.clear_cache()
 
     def __init__(self):
         super().__init__()
-        self.options = self.Options(parent=self)
-        self.reactive_site_filter: ReactiveSiteFilter = ReactiveSiteFilter()
+        self.further_exploration_filter = FurtherExplorationFilter()
         self._cache: Dict[str, List[int]] = {}
         self._required_collections = ["manager", "calculations", "structures"]
 
     def clear_cache(self):
         self._cache = {}
 
     def _sanity_check_configuration(self) -> None:
         if not isinstance(self.reactive_site_filter, ReactiveSiteFilter):
             raise TypeError("Expected a ReactiveSiteFilter (or a class derived "
                             "from it) in FastDissociations.reactive_site_filter.")
-        if not isinstance(self.options.further_exploration_filter, FurtherExplorationFilter):
-            raise TypeError("Expected a FurtherExplorationFilter (or a class derived "
-                            "from it) in FastDissociations.options.further_exploration_filter.")
+        if not isinstance(self.further_exploration_filter, FurtherExplorationFilter):
+            raise TypeError(f"Expected a FurtherExplorationFilter (or a class derived "
+                            f"from it) in FastDissociations.further_exploration_filter, not type "
+                            f"{type(self.further_exploration_filter)}.")
         if not isinstance(self._manager, db.Manager):
             raise TypeError("Propagation of db information failed")
-        self.options.further_exploration_filter.initialize_collections(self._manager)
+        self.further_exploration_filter.initialize_collections(self._manager)
 
-    def bimolecular_reactions(self, _: List[db.Structure]) -> None:
+    def bimolecular_coordinates(self, structure_list: List[db.Structure], with_exact_settings_check: bool = False) \
+            -> Dict[
+        Tuple[List[Tuple[int, int]], int],
+        List[Tuple[ndarray, ndarray, float, float]]
+    ]:
+        return {}
+
+    def bimolecular_reactions(self,
+                              structure_list: List[db.Structure],
+                              with_exact_settings_check: bool = False) -> None:
         """
         Bimolecular reactions are not supported by this TrialGenerator.
 
         Parameters
         ----------
-        _ :: List[db.Structure]
+        structure_list :: List[db.Structure]
             List of the two structures to be considered.
+        with_exact_settings_check :: bool
+            If True, more expensive queries are carried out to check if the settings of the
+            calculations are exactly the same as the settings of the trial generator. This allows to add more
+            inclusive additional reaction trials but the queries are less efficient, therefore this option
+            should be only toggled if necessary.
         """
         warn(f"Bimolecular reactions are not supported by the {self.__class__.__name__} TrialGenerator.")
 
-    def unimolecular_reactions(self, structure: db.Structure) -> None:
-        """
-        Creates reactive complex calculations corresponding to the unimolecular
-        reactions of the structure if there is not already a calculation to
-        search for a reaction of the same structure with the same job order, model and settings.
-
-        Parameters
-        ----------
-        structure :: db.Structure
-            The structure to be considered. The Structure has to
-            be linked to a database.
-        """
-        self._sanity_check_configuration()
-        if self.options.max_bond_dissociations < 1:
-            return
+    @_sanity_check_wrapper
+    def unimolecular_coordinates(self, structure: db.Structure, with_exact_settings_check: bool = False) \
+            -> List[Tuple[List[List[Tuple[int, int]]], int]]:
+        return self.unimolecular_fast_coordinates(structure, with_exact_settings_check) + \
+            self.unimolecular_further_explore_coordinates(structure, with_exact_settings_check)
+
+    def unimolecular_fast_coordinates(self, structure: db.Structure, with_exact_settings_check: bool = False) \
+            -> List[Tuple[List[List[Tuple[int, int]]], int]]:
+        if self.options.unimolecular_options.max_bond_dissociations < 1:
+            return []
         # Rule out compounds too small for intramolecular reactions right away
         atoms = structure.get_atoms()
         structure_id = structure.id()
         str_structure_id = str(structure_id)
         # No intramolecular reactions for monoatomic compounds
         if atoms.size() == 1:
-            return
-
+            return []
         # We are filling the cache with structure as key.
         # The value is a list of the so far maximum explored dissociations
         # e.g. 1 at once (break 5-7), 2 at once (break 5-7 and 3-6 in one step), and so on
         # the ordering is fast disconnective [0], slow dissociative [1], and slow disconnective [2]
         if str_structure_id not in self._cache:
             self._cache[str_structure_id] = [0, 0, 0]
         current_cache_entry = self._cache[str_structure_id]
         allowed_types: List[bool] = [True,
-                                     self.options.always_further_explore_dissociative_reactions,
-                                     self.options.enable_further_explorations]
+                                     self.options.unimolecular_options.always_further_explore_dissociative_reactions,
+                                     self.options.unimolecular_options.enable_further_explorations]
 
         # Get all reactive atoms
         reactive_atoms = self.reactive_site_filter.filter_atoms([structure], list(range(atoms.size())))
-        further_reactive_atoms = self.options.further_exploration_filter.filter_atoms(structure, reactive_atoms)
         # Get all ordered pairs of reactive atoms
         connectivity_analyzer = ConnectivityAnalyzer(structure)
         fast_diss_pairs: List[Tuple[int, int]] = self._get_filtered_intraform_and_diss(
             structure, reactive_atoms, connectivity_analyzer)[1]
-        further_diss_pairs: List[Tuple[int, int]] = self._get_filtered_intraform_and_diss(
-            structure, further_reactive_atoms, connectivity_analyzer)[1]
 
+        result: List[Tuple[List[List[Tuple[int, int]]], int]] = []
         # Loop over possible options of dissociations
-        for n_diss in range(self.options.min_bond_dissociations, self.options.max_bond_dissociations + 1):
+        for n_diss in range(self.options.unimolecular_options.min_bond_dissociations,
+                            self.options.unimolecular_options.max_bond_dissociations + 1):
             if n_diss < 1:
                 continue
             # determine allowed number of simultaneous dissociations for each subtype based on cache and settings
-            allowed_for_n = [i < n_diss and active for i, active in zip(current_cache_entry, allowed_types)]
-            if not any([allowed for allowed in allowed_for_n]):
+            allowed_for_n = [i < n_diss and active for i, active in zip(current_cache_entry[:2], allowed_types[:2])]
+            if not with_exact_settings_check and not any([allowed for allowed in allowed_for_n]):
                 # skip already if none of the three types are allowed for this number of dissociations
                 continue
-            dissociative_coordinates = []
             all_coordinates = [list(x) for x in combinations(fast_diss_pairs, n_diss)]  # type: ignore
-            """ Fast dissociations """
             filtered_coordinates = self.reactive_site_filter.filter_reaction_coordinates([structure], all_coordinates)
-            if allowed_for_n[0]:
+            result.append((filtered_coordinates, n_diss))
+
+        return result
+
+    def unimolecular_further_explore_coordinates(self, structure: db.Structure,
+                                                 with_exact_settings_check: bool = False) \
+            -> List[Tuple[List[List[Tuple[int, int]]], int]]:
+        if self.options.unimolecular_options.max_bond_dissociations < 1 \
+                or not self.options.unimolecular_options.enable_further_explorations:
+            return []
+        # Rule out compounds too small for intramolecular reactions right away
+        atoms = structure.get_atoms()
+        structure_id = structure.id()
+        str_structure_id = str(structure_id)
+        # No intramolecular reactions for monoatomic compounds
+        if atoms.size() == 1:
+            return []
+        # We are filling the cache with structure as key.
+        # The value is a list of the so far maximum explored dissociations
+        # e.g. 1 at once (break 5-7), 2 at once (break 5-7 and 3-6 in one step), and so on
+        # the ordering is fast disconnective [0], slow dissociative [1], and slow disconnective [2]
+        if str_structure_id not in self._cache:
+            self._cache[str_structure_id] = [0, 0, 0]
+        current_cache_entry = self._cache[str_structure_id]
+
+        # Get all reactive atoms
+        reactive_atoms = self.reactive_site_filter.filter_atoms([structure], list(range(atoms.size())))
+        further_reactive_atoms = self.further_exploration_filter.filter_atoms(structure, reactive_atoms)
+        # Get all ordered pairs of reactive atoms
+        connectivity_analyzer = ConnectivityAnalyzer(structure)
+        further_diss_pairs: List[Tuple[int, int]] = self._get_filtered_intraform_and_diss(
+            structure, further_reactive_atoms, connectivity_analyzer)[1]
+        result: List[Tuple[List[List[Tuple[int, int]]], int]] = []
+        # Loop over possible options of dissociations
+        for n_diss in range(self.options.unimolecular_options.min_bond_dissociations,
+                            self.options.unimolecular_options.max_bond_dissociations + 1):
+            if n_diss < 1:
+                continue
+            if not with_exact_settings_check and n_diss < current_cache_entry[2]:
+                # skip already if further exploration is not allowed for this number of dissociations
+                continue
+            # determine allowed number of simultaneous dissociations for each subtype based on cache and settings
+            pairs = self.further_exploration_filter.filter_atom_pairs(structure, further_diss_pairs)
+            for slow_diss_pairs in combinations(pairs, n_diss):
+                diss_pairs = list(slow_diss_pairs)
+                # we assume here that
+                # The further filter will be more restrictive than the fast filter, hence we don't need to add
+                # dissociative coordinate, since they are covered by the standard way
+                reaction_type = connectivity_analyzer.get_reaction_type(diss_pairs)
+                if reaction_type != ReactionType.Disconnective:
+                    continue
+                # Check whether trial coordinate is to be considered
+                if self.reactive_site_filter.filter_reaction_coordinates([structure], [diss_pairs]) and \
+                        self.further_exploration_filter.filter_reaction_coordinates(structure, [diss_pairs]):
+                    result.append(([diss_pairs], n_diss))
+
+        return result
+
+    @_sanity_check_wrapper
+    def unimolecular_reactions(self, structure: db.Structure, with_exact_settings_check: bool = False) -> None:
+        """
+        Creates reactive complex calculations corresponding to the unimolecular
+        reactions of the structure if there is not already a calculation to
+        search for a reaction of the same structure with the same job order, model and settings.
+
+        Parameters
+        ----------
+        structure :: db.Structure
+            The structure to be considered. The Structure has to
+            be linked to a database.
+        with_exact_settings_check :: bool
+            If True, more expensive queries are carried out to check if the settings of the
+            calculations are exactly the same as the settings of the trial generator. This allows to add more
+            inclusive additional reaction trials but the queries are less efficient, therefore this option
+            should be only toggled if necessary.
+        """
+        fast_coordinates = self.unimolecular_fast_coordinates(structure, with_exact_settings_check)
+        further_coordinates = self.unimolecular_further_explore_coordinates(structure, with_exact_settings_check)
+        if not fast_coordinates and not further_coordinates:
+            return
+        connectivity_analyzer = ConnectivityAnalyzer(structure)
+        structure_id = structure.id()
+        str_structure_id = str(structure.id())
+        allowed_types: List[bool] = [True,
+                                     self.options.unimolecular_options.always_further_explore_dissociative_reactions,
+                                     self.options.unimolecular_options.enable_further_explorations]
+        current_cache_entry = self._cache[str_structure_id]
+
+        for filtered_coordinates, n_diss in fast_coordinates:
+            dissociative_coordinates = []
+            """ Fast dissociations """
+            if allowed_types[0]:
                 calculation_ids = []
                 # TODO in first cache run, we are constructing the settings and then check if calculation
                 # with these settings exists
                 # a faster strategy would be to construct all possible settings (based on coordinates)
                 # and then query calculations once for all still uncovered settings and create calculations for those
                 for diss_pairs in filtered_coordinates:
                     # Get reaction type:
                     reaction_type = connectivity_analyzer.get_reaction_type(diss_pairs)
                     if reaction_type == ReactionType.Dissociative:
                         dissociative_coordinates.append(diss_pairs)
                     if reaction_type != ReactionType.Disconnective:
                         continue
                     cid = self._add_disconnective_calculation(structure_id, diss_pairs,
-                                                              self.options.cutting_job,
-                                                              self.options.cutting_job_settings)
+                                                              self.options.unimolecular_options.job,
+                                                              self.options.unimolecular_options.cutting_job_settings,
+                                                              check_for_existing=True)
                     if cid is not None:
                         calculation_ids.append(cid)
                 if calculation_ids:
                     # only add first due to limited entry space for mongodb document
-                    structure.add_calculation(self.options.cutting_job.order, calculation_ids[0])
+                    structure.add_calculation(self.options.unimolecular_options.job.order, calculation_ids[0])
+                # update cache
                 current_cache_entry[0] = n_diss
 
             """ Slow dissociative coordinates """
-            if allowed_for_n[1]:
-                filtered_coordinates = self.reactive_site_filter.filter_reaction_coordinates([structure],
-                                                                                             dissociative_coordinates)
+            if allowed_types[1]:
                 calculation_ids = []
                 # TODO see fast dissociations
-                for diss_pairs in filtered_coordinates:
+                for diss_pairs in dissociative_coordinates:
                     cid = self._add_reactive_complex_calculation([structure_id], [], diss_pairs,
-                                                                 self.options.further_job,
-                                                                 self.options.further_job_settings,
+                                                                 self.options.unimolecular_options.further_job,
+                                                                 self.options.unimolecular_options.further_job_settings,
                                                                  check_for_existing=True)
                     if cid is not None:
                         calculation_ids.append(cid)
                 if calculation_ids:
                     # only add first due to limited entry space for mongodb document
-                    structure.add_calculations(self.options.further_job.order, calculation_ids)
+                    structure.add_calculations(self.options.unimolecular_options.further_job.order, calculation_ids)
+                # update cache
                 current_cache_entry[1] = n_diss
 
+        for filtered_coordinates, n_diss in further_coordinates:
             """ Slow dissociations """
-            if allowed_for_n[2]:
-                pairs = self.options.further_exploration_filter.filter_atom_pairs(structure, further_diss_pairs)
+            if allowed_types[2]:  # should not be needed, but just to be sure
                 calculation_ids = []
                 # TODO see fast dissociations
-                for slow_diss_pairs in combinations(pairs, n_diss):
-                    diss_pairs = list(slow_diss_pairs)
-                    if current_cache_entry[1] >= n_diss and diss_pairs in dissociative_coordinates:
-                        # we already explored this because it is solely dissociative
-                        continue
-                    # Get reaction type:
-                    reaction_type = connectivity_analyzer.get_reaction_type(diss_pairs)
-                    if reaction_type != ReactionType.Disconnective:
-                        continue
-                    # Check whether trial coordinate is to be considered
-                    if self.reactive_site_filter.filter_reaction_coordinates([structure], [diss_pairs]) and \
-                            self.options.further_exploration_filter.filter_reaction_coordinates(structure,
-                                                                                                [diss_pairs]):
-                        cid = self._add_reactive_complex_calculation([structure_id], [], diss_pairs,
-                                                                     self.options.further_job,
-                                                                     self.options.further_job_settings,
-                                                                     check_for_existing=True)
-                        if cid is not None:
-                            calculation_ids.append(cid)
+                for slow_diss_pairs in filtered_coordinates:
+                    cid = self._add_reactive_complex_calculation([structure_id], [], slow_diss_pairs,
+                                                                 self.options.unimolecular_options.further_job,
+                                                                 self.options.unimolecular_options.further_job_settings,
+                                                                 check_for_existing=True)
+                    if cid is not None:
+                        calculation_ids.append(cid)
                 if calculation_ids:
                     # only add first due to limited entry space for mongodb document
-                    structure.add_calculations(self.options.further_job.order, calculation_ids)
+                    structure.add_calculations(self.options.unimolecular_options.further_job.order, calculation_ids)
+                # update cache
                 current_cache_entry[2] = n_diss
 
     def _add_disconnective_calculation(
-        self,
-        reactive_structure: db.ID,
-        dissociation_pairs: List[Tuple[int, int]],
-        job: db.Job,
-        settings: utils.ValueCollection,
-    ) -> Union[db.ID, None]:
+            self,
+            reactive_structure: db.ID,
+            dissociation_pairs: List[Tuple[int, int]],
+            job: db.Job,
+            settings: utils.ValueCollection,
+            check_for_existing: bool = False
+    ) -> Optional[db.ID]:
         """
         Adds a reactive calculation for a bond-based approach (i.e., one during which it is tried to form/break
         bonds between designated atom pairs) to the database and puts it on hold.
 
         Parameters
         ----------
 
@@ -495,26 +673,33 @@
             The ID of the reactant.
         dissociation_pairs:: List[Tuple[int, int]]
             List of atom index pairs in between which a bond dissociation is to
             be encouraged.
         job :: scine_database.Job
         settings :: scine_utilities.ValueCollection
         """
+        this_settings = self._get_settings(settings)
 
         if job.order == "scine_dissociation_cut":
             # job takes lists of integer where elements 0/1, 2/3 ... N-1, N are combined with each other
             # Flatten pair lists
-            settings["dissociations"] = FurtherExplorationFilter.dissociation_setting_from_reaction_coordinate(
+            this_settings["dissociations"] = FurtherExplorationFilter.dissociation_setting_from_reaction_coordinate(
                 dissociation_pairs)
         else:
             raise RuntimeError("Only 'scine_dissociation_cut' order supported for fast dissociations")
 
-        if get_calculation_id(job.order, [reactive_structure], self.options.model,
-                              self._calculations, settings=settings) is not None:
+        if check_for_existing and get_calculation_id(job.order, [reactive_structure], self.options.model,
+                                                     self._calculations, settings=this_settings) is not None:
             return None
         calculation = db.Calculation(db.ID(), self._calculations)
         calculation.create(self.options.model, job, [reactive_structure])
         # Sleep a bit in order not to make the DB choke
         time.sleep(0.001)
-        calculation.set_settings(deepcopy(settings))
+        calculation.set_settings(deepcopy(this_settings))
         calculation.set_status(db.Status.HOLD)
         return calculation.id()
+
+    def get_unimolecular_job_order(self) -> str:
+        return self.options.unimolecular_options.job.order
+
+    def get_bimolecular_job_order(self) -> str:
+        raise RuntimeError("Bimolecular reactions are not supported by this TrialGenerator.")
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/trial_generator/fragment_based.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/trial_generator/fragment_based.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
 import time
-from copy import deepcopy
+from collections import defaultdict
 from itertools import combinations, product
-from typing import Iterator, List, Tuple, Optional
+from typing import Dict, Iterator, List, Tuple, Optional, Generator
 from json import dumps
 
 # Third party imports
+from numpy import ndarray
 import scine_database as db
 import scine_utilities as utils
 
 # Local application imports
-from ....utilities.queries import model_query, select_calculation_by_structures
-from ....utilities.calculation_creation_helpers import finalize_calculation
-from ..reactive_site_filters import ReactiveSiteFilter
+from scine_chemoton.utilities.queries import model_query, calculation_exists_in_structure, get_calculation_id
 from .connectivity_analyzer import ReactionType, ConnectivityAnalyzer
-from . import TrialGenerator
+from . import TrialGenerator, _sanity_check_wrapper
 
 
 class FragmentBased(TrialGenerator):
     """
     Class to generate reactive complex calculations via fragment-based approaches.
 
     Attributes
@@ -42,24 +41,23 @@
         a certain fragment composition is allowed, the fragment composition
         is considered.
         For bimolecular reactions with two diatomic fragments the reactive pairs
         correspond to the atoms facing each other in the (unrotated) reactive
         complex.
     """
 
-    class Options:
+    class Options(TrialGenerator.Options):
         """
         The options for the fragment-based reactive complex enumeration.
         """
 
         __slots__ = (
-            "model",
-            "unimolecular_dissociation",
-            "unimolecular_association",
-            "bimolecular_association",
+            "unimolecular_dissociation_options",
+            "unimolecular_association_options",
+            "bimolecular_association_options",
         )
 
         class BimolAssociationOptions:
             """
             The options for the exploration of bimolecular reactions.
             """
 
@@ -228,94 +226,165 @@
                 """
                 int
                     Maximum number of bonds between two atoms forming a reactive
                     fragment. This option is only effective if
                     `consider_diatomic_fragments` is `True`. (default: 1)
                 """
 
-        def __init__(self):
-            self.model: db.Model = db.Model("PM6", "", "")
-            """
-            db.Model (Scine::Database::Model)
-                The Model used to evaluate the possible reactions.
-                The default is: PM6 using Sparrow.
-            """
-            self.unimolecular_dissociation = self.UnimolDissociationOptions()
+        def __init__(self, parent: Optional[TrialGenerator] = None):
+            super().__init__(parent)
+            self.unimolecular_dissociation_options = self.UnimolDissociationOptions()
             """
             UnimolDissociationOptions
                 The settings for reactions involving a single molecule, that are
                 set up to be dissociative in nature.
             """
-            self.unimolecular_association = self.UnimolAssociationOptions()
+            self.unimolecular_association_options = self.UnimolAssociationOptions()
             """
             UnimolAssociationOptions
                 The settings for reactions involving a single molecule, that are
                 set up to be associative in nature.
             """
-            self.bimolecular_association = self.BimolAssociationOptions()
+            self.bimolecular_association_options = self.BimolAssociationOptions()
             """
             BimolAssociationOptions
                 The settings for reactions involving two molecules, that are set up
                 to be associative in nature.
             """
 
-    def __init__(self):
-        super().__init__()
-        self.options = self.Options()
-        self.reactive_site_filter = ReactiveSiteFilter()
+    def clear_cache(self):
+        pass
+
+    @_sanity_check_wrapper
+    def bimolecular_coordinates(self, structure_list: List[db.Structure], with_exact_settings_check: bool = False) \
+            -> Dict[
+        Tuple[List[Tuple[int, int]], int],
+        List[Tuple[ndarray, ndarray, float, float]]
+    ]:
+        # Check number of compounds
+        if len(structure_list) != 2:
+            raise RuntimeError("Exactly two structures are needed for setting up an intermolecular reaction.")
+        if self._quick_bimolecular_already_exists(structure_list, do_fast_query=not with_exact_settings_check):
+            return {}
+        result = defaultdict(list)
+        for (
+                inter_pairs,
+                align1,
+                align2,
+                rot,
+                spread,
+        ) in self._generate_bimolecular_coordinates(structure_list):
+            # 0 because n_diss is always 0 for fragment based
+            result[(inter_pairs, 0)].append((align1, align2, rot, spread))
+        return result
 
-    def bimolecular_reactions(self, structure_list: List[db.Structure]):
+    def _quick_bimolecular_already_exists(self, structure_list: List[db.Structure], do_fast_query: bool) -> bool:
+        """
+            If there is a reactive complex calculation for the same structures, return True
+        """
+        if not do_fast_query:
+            return False
+        structure_id_list = [structure.id() for structure in structure_list]
+        return calculation_exists_in_structure(
+            self.get_bimolecular_job_order(),
+            structure_id_list,
+            self.options.model,
+            self._structures,
+            self._calculations
+        )
+
+    @_sanity_check_wrapper
+    def bimolecular_reactions(self, structure_list: List[db.Structure], with_exact_settings_check: bool = False):
         """
         Creates reactive complex calculations corresponding to the bimolecular
         reactions between the structures if there is not already a calculation
         to search for a reaction of the same structures with the same job order.
 
         Parameters
         ----------
         structure_list :: List[db.Structure]
             List of the two structures to be considered.
             The Structures have to be linked to a database.
+        with_exact_settings_check :: bool
+            If True, more expensive queries are carried out to check if the settings of the
+            calculations are exactly the same as the settings of the trial generator. This allows to add more
+            inclusive additional reaction trials but the queries are less efficient, therefore this option
+            should be only toggled if necessary.
         """
         # Check number of compounds
         if len(structure_list) != 2:
             raise RuntimeError("Exactly two structures are needed for setting up an intermolecular reaction.")
 
         structure_id_list = [s.id() for s in structure_list]
 
         # If there is a reactive complex calculation for the same structures, return
-        selection = select_calculation_by_structures(
-            self.options.bimolecular_association.job.order,
-            structure_id_list,
-            self.options.model)
-        if self._calculations.get_one_calculation(dumps(selection)) is not None:
+        if self._quick_bimolecular_already_exists(structure_list, do_fast_query=not with_exact_settings_check):
             return
 
+        new_calculation_ids = []
+        # add calculations
+        for (
+                inter_pairs,
+                align1,
+                align2,
+                rot,
+                spread,
+        ) in self._generate_bimolecular_coordinates(structure_list):
+            # First element of interstructural pair belongs to first structure and second to second
+            # Indexes in the rhs and lhs list refer to the individual structures so no shifting necessary
+            lhs = list(set(pair[0] for pair in inter_pairs))
+            rhs = list(set(pair[1] for pair in inter_pairs))
+            # Set up calculation because no further intrastructural components supported
+            cid = self._add_reactive_complex_calculation(
+                structure_id_list,
+                ReactionType.Associative,
+                lhs,
+                rhs,
+                self.options.bimolecular_association_options.job,
+                self.options.bimolecular_association_options.job_settings,
+                list(align1),
+                list(align2),
+                rot,
+                spread,
+                0.0,
+                check_for_existing=with_exact_settings_check
+            )
+            if cid is not None:
+                new_calculation_ids.append(cid)
+        if new_calculation_ids:
+            for s in structure_list:
+                s.add_calculations(self.get_bimolecular_job_order(), [new_calculation_ids[0]])
+
+    def _generate_bimolecular_coordinates(self, structure_list: List[db.Structure]) -> Generator[
+        Tuple[List[Tuple[int, int]], ndarray, ndarray, float, float], None, None
+    ]:
         # Get single reactive atoms per structure
-        reactive_monoatomic1 = self.reactive_site_filter.filter_atoms(
-            [structure_list[0]], range(structure_list[0].get_atoms().size())
-        )
-        reactive_monoatomic2 = self.reactive_site_filter.filter_atoms(
-            [structure_list[1]], range(structure_list[1].get_atoms().size())
+        n_atoms1 = structure_list[0].get_atoms().size()
+        n_atoms2 = structure_list[1].get_atoms().size()
+        reactive_atoms = self.reactive_site_filter.filter_atoms(
+            structure_list, list(range(n_atoms1)) + [i + n_atoms1 for i in range(n_atoms2)]
         )
+        reactive_monoatomic1 = [i for i in reactive_atoms if i < n_atoms1]
+        reactive_monoatomic2 = [i - n_atoms1 for i in reactive_atoms if i >= n_atoms1]
         # Get reactive pairs within each structure in agreement with distance settings
         reactive_diatomic1 = []
         reactive_diatomic2 = []
 
-        if self.options.bimolecular_association.consider_diatomic_fragments:
+        if self.options.bimolecular_association_options.consider_diatomic_fragments:
             connectivity_analyzer1 = ConnectivityAnalyzer(structure_list[0])
             connectivity_analyzer2 = ConnectivityAnalyzer(structure_list[1])
             reactive_diatomic1 = self._get_intrastructural_pairs(
                 connectivity_analyzer1,
                 reactive_monoatomic1,
-                (1, self.options.bimolecular_association.max_within_fragment_graph_distance),
+                (1, self.options.bimolecular_association_options.max_within_fragment_graph_distance),
             )
             reactive_diatomic2 = self._get_intrastructural_pairs(
                 connectivity_analyzer2,
                 reactive_monoatomic2,
-                (1, self.options.bimolecular_association.max_within_fragment_graph_distance),
+                (1, self.options.bimolecular_association_options.max_within_fragment_graph_distance),
             )
 
         # Generate reactive pair combinations across the two structures from reactive sites
         # Applies the reactive_site_filter's filter_atom_pair method
         inter_coords = list(
             self._generate_inter_reactive_coords(
                 structure_list, reactive_monoatomic1, reactive_monoatomic2, reactive_diatomic1, reactive_diatomic2
@@ -335,204 +404,152 @@
         # For each coord generate the corresponding reactive complexes
         for (
             inter_pairs,
             align1,
             align2,
             rot,
             spread,
-        ) in self.options.bimolecular_association.complex_generator.generate_reactive_complexes(
+        ) in self.options.bimolecular_association_options.complex_generator.generate_reactive_complexes(
             structure_list[0], structure_list[1], inter_coords
         ):
-            # First element of interstructural pair belongs to first structure and second to second
-            # Indexes in the rhs and lhs list refer to the individual structures so no shifting necessary
-            lhs = list(set(pair[0] for pair in inter_pairs))
-            rhs = list(set(pair[1] for pair in inter_pairs))
-            # Set up calculation bc no further intrastructural components supported
-            self._add_reactive_complex_calculation(
-                structure_id_list,
-                ReactionType.Associative,
-                lhs,
-                rhs,
-                self.options.bimolecular_association.job,
-                self.options.bimolecular_association.job_settings,
-                list(align1),
-                list(align2),
-                rot,
-                spread,
-                0.0,
-            )
-        return
+            yield inter_pairs, align1, align2, rot, spread
 
-    def unimolecular_reactions(self, structure: db.Structure):
+    def _quick_unimolecular_already_exists(self, structure: db.Structure, do_fast_query: bool) -> bool:
         """
-        Creates reactive complex calculations corresponding to the unimolecular
-        reactions of the structure if there is not already a calculation to
-        search for a reaction of the same structure with the same job order.
-
-        Parameters
-        ----------
-        structure :: db.Structure
-            The structure to be considered. The Structure has to
-            be linked to a database.
+            If there is a reactive complex calculation for the same structures, return True
         """
-
         # Rule out compounds too small for intramolecular reactions right away
         atoms = structure.get_atoms()
-        structure_id = structure.id()
         # No intramolecular reactions for monoatomic compounds
         if atoms.size() == 1:
-            return
+            return True
         # Only consider diatomic structures if dissociations are to be considered
-        if atoms.size() == 2 and not self.options.unimolecular_dissociation.enabled:
-            return
+        if atoms.size() == 2 and not self.options.unimolecular_dissociation_options.enabled:
+            return True
+        # check later for complete check
+        if not do_fast_query:
+            return False
+        return calculation_exists_in_structure(
+            self.get_unimolecular_job_order(),
+            [structure.id()],
+            self.options.model,
+            self._structures,
+            self._calculations
+        )
 
-        # Check whether there is a reactive complex calculation for the same structure already
-        if self.options.unimolecular_dissociation.enabled:
-            selection = {
-                "$and": [
-                    {"job.order": {"$eq": self.options.unimolecular_dissociation.job.order}},
-                    {"structures": [{"$oid": structure_id.string()}]},
-                    *model_query(self.options.model)
-                ]
-            }
-            if self._calculations.get_one_calculation(dumps(selection)) is not None:
-                return
-        if self.options.unimolecular_association.enabled:
-            selection = {
-                "$and": [
-                    {"job.order": {"$eq": self.options.unimolecular_association.job.order}},
-                    {"structures": [{"$oid": structure_id.string()}]},
-                    *model_query(self.options.model)
-                ]
-            }
-            if self._calculations.get_one_calculation(dumps(selection)) is not None:
-                return
+    @_sanity_check_wrapper
+    def unimolecular_coordinates(self, structure: db.Structure, with_exact_settings_check: bool = False) \
+            -> List[Tuple[List[List[Tuple[int, int]]], int]]:
+        if self._quick_unimolecular_already_exists(structure, do_fast_query=not with_exact_settings_check):
+            return []
+
+        result = []
 
+        atoms = structure.get_atoms()
         connectivity_analyzer = ConnectivityAnalyzer(structure)
         reactive_atoms = self.reactive_site_filter.filter_atoms([structure], list(range(atoms.size())))
 
         # Associative reactions
-        if self.options.unimolecular_association.enabled:
+        if self.options.unimolecular_association_options.enabled:
             # Atom on atom
             # Pairs allowed wrt distance bound options
             monoatomic_fragment_pairs = self._get_intrastructural_pairs(
                 connectivity_analyzer,
                 reactive_atoms,
                 (
-                    self.options.unimolecular_association.min_inter_fragment_graph_distance,
-                    self.options.unimolecular_association.max_inter_fragment_graph_distance,
+                    self.options.unimolecular_association_options.min_inter_fragment_graph_distance,
+                    self.options.unimolecular_association_options.max_inter_fragment_graph_distance,
                 ),
             )
             filtered_monoatomic_fragment_pairs = self.reactive_site_filter.filter_atom_pairs(
                 [structure], monoatomic_fragment_pairs
             )
             atom_on_atom_coordinates = [[pair] for pair in filtered_monoatomic_fragment_pairs]
-            for coord in self.reactive_site_filter.filter_reaction_coordinates([structure], atom_on_atom_coordinates):
+            filtered_coords = self.reactive_site_filter.filter_reaction_coordinates([structure],
+                                                                                    atom_on_atom_coordinates)
+            for coord in filtered_coords:
+                # sanity check
                 if len(coord) != 1:
                     # Should not be reached
                     raise RuntimeError("Monoatomic fragment coordinate has to be of length one.")
-                # Determine reaction type for intramolecular reactions
-                reaction_type = connectivity_analyzer.get_reaction_type(coord)
-                # If indeed associative (should be if min_graph_distance was set to > 1)
-                if reaction_type == ReactionType.Associative:
-                    self._add_reactive_complex_calculation(
-                        [structure_id],
-                        reaction_type,
-                        [coord[0][0]],
-                        [coord[0][1]],
-                        self.options.unimolecular_association.job,
-                        self.options.unimolecular_association.job_settings,
-                    )
+            result.append((filtered_coords, 0))
             # Diatomic fragments
-            if self.options.unimolecular_association.consider_diatomic_fragments:
+            if self.options.unimolecular_association_options.consider_diatomic_fragments:
                 diatomic_fragments = self._get_intrastructural_pairs(
                     connectivity_analyzer,
                     reactive_atoms,
-                    (1, self.options.unimolecular_association.max_within_fragment_graph_distance),
+                    (1, self.options.unimolecular_association_options.max_within_fragment_graph_distance),
                 )
                 # Monoatomic to diatomic (e.g. "atom on bond" if max_within_fragment_graph_distance==1)
                 for atom in reactive_atoms:
                     for frag in diatomic_fragments:
                         if atom in frag:
                             continue
                         # Check whether both atoms of the diatomic fragment respect the distance bounds wrt the
                         # monoatomic fragment
                         if not self._check_all_inter_fragment_distances(
-                            connectivity_analyzer,
-                            [atom],
-                            frag,
-                            (
-                                self.options.unimolecular_association.min_inter_fragment_graph_distance,
-                                self.options.unimolecular_association.max_inter_fragment_graph_distance,
-                            ),
+                                connectivity_analyzer,
+                                [atom],
+                                list(frag),
+                                (
+                                    self.options.unimolecular_association_options.min_inter_fragment_graph_distance,
+                                    self.options.unimolecular_association_options.max_inter_fragment_graph_distance,
+                                ),
                         ):
                             continue
                         coord = [(atom, frag[0]), (atom, frag[1])]
                         # Both pairs have to be reactive
                         if len(self.reactive_site_filter.filter_atom_pairs([structure], coord)) != 2:
                             continue
                         # Coordinate has to be reactive
                         if len(self.reactive_site_filter.filter_reaction_coordinates([structure], [coord])) != 1:
                             continue
                         if connectivity_analyzer.get_reaction_type(coord) == ReactionType.Associative:
-                            self._add_reactive_complex_calculation(
-                                [structure_id],
-                                ReactionType.Associative,
-                                [atom],
-                                frag,
-                                self.options.unimolecular_association.job,
-                                self.options.unimolecular_association.job_settings,
-                            )
+                            result.append(([coord], 0))
                 # Diatomic to diatomic (e.g. "bond on bond" if max_within_fragment_graph_distance==1)
                 for frag1, frag2 in combinations(diatomic_fragments, 2):
                     if len(set(frag1 + frag2)) < 4:
                         # Atoms shall not appear on lhs AND rhs at the same time
                         continue
                     # All possible pair interpretations between the two fragments shall respect the distance bounds
                     if not self._check_all_inter_fragment_distances(
-                        connectivity_analyzer,
-                        frag1,
-                        frag2,
-                        (
-                            self.options.unimolecular_association.min_inter_fragment_graph_distance,
-                            self.options.unimolecular_association.max_inter_fragment_graph_distance,
-                        ),
+                            connectivity_analyzer,
+                            frag1,
+                            frag2,
+                            (
+                                self.options.unimolecular_association_options.min_inter_fragment_graph_distance,
+                                self.options.unimolecular_association_options.max_inter_fragment_graph_distance,
+                            ),
                     ):
                         continue
 
                     coord = [(frag1[0], frag2[0]), (frag1[1], frag2[1])]
                     shuffled_coord = [(frag1[0], frag2[1]), (frag1[1], frag2[0])]
                     # Check whether any of the reactive pair interpretations is reactive
                     if (
-                        len(self.reactive_site_filter.filter_atom_pairs([structure], coord)) < 2
-                        and len(self.reactive_site_filter.filter_atom_pairs([structure], shuffled_coord)) < 2
+                            len(self.reactive_site_filter.filter_atom_pairs([structure], coord)) < 2
+                            and len(self.reactive_site_filter.filter_atom_pairs([structure], shuffled_coord)) < 2
                     ):
                         continue
                     # Check whether any of the reaction coordinate interpretations is reactive
                     if (
-                        len(self.reactive_site_filter.filter_reaction_coordinates([structure], [coord, shuffled_coord]))
-                        == 0
+                            len(self.reactive_site_filter.filter_reaction_coordinates([structure],
+                                                                                      [coord, shuffled_coord]))
+                            == 0
                     ):
                         continue
                     # Only consider if there is no direct bond between fragments
                     if connectivity_analyzer.get_reaction_type(coord) != ReactionType.Associative:
                         continue
                     if connectivity_analyzer.get_reaction_type(shuffled_coord) != ReactionType.Associative:
                         continue
-                    self._add_reactive_complex_calculation(
-                        [structure_id],
-                        ReactionType.Associative,
-                        frag1,
-                        frag2,
-                        self.options.unimolecular_association.job,
-                        self.options.unimolecular_association.job_settings,
-                    )
+                    result.append(([coord], 0))
 
         # Dissociative reactions
-        if self.options.unimolecular_dissociation.enabled:
+        if self.options.unimolecular_dissociation_options.enabled:
             # Only adjacent (i.e. with a graph distance of 1) atoms are made subject to dissociation
             diss_pairs = self._get_intrastructural_pairs(connectivity_analyzer, reactive_atoms, (1, 1))
             # Filter wrt pair filter
             filtered_diss_pairs = self.reactive_site_filter.filter_atom_pairs([structure], diss_pairs)
             # Filter wrt coordinate filter
             filtered_coords = self.reactive_site_filter.filter_reaction_coordinates(
                 [structure], [[pair] for pair in filtered_diss_pairs]
@@ -540,52 +557,142 @@
             for coord in filtered_coords:
                 # Dissociative coordinates only consist of one pair each
                 if len(coord) > 1:
                     # Should not be reached
                     raise RuntimeError(
                         "Only one simultaneous dissociation supported in fragment based trial generator."
                     )
-                i = coord[0][0]
-                j = coord[0][1]
-                # Determine reaction type for intramolecular reactions
-                reaction_type = connectivity_analyzer.get_reaction_type([(i, j)])
-                # Add calculation
-                if reaction_type == ReactionType.Dissociative:
-                    self._add_reactive_complex_calculation(
-                        [structure_id],
-                        reaction_type,
-                        [i],
-                        [j],
-                        self.options.unimolecular_dissociation.job,
-                        self.options.unimolecular_dissociation.job_settings_dissociative,
-                    )
-                if reaction_type == ReactionType.Disconnective:
-                    self._add_reactive_complex_calculation(
-                        [structure_id],
-                        reaction_type,
-                        [i],
-                        [j],
-                        self.options.unimolecular_dissociation.job,
-                        self.options.unimolecular_dissociation.job_settings_disconnective,
-                    )
+            result.append((filtered_coords, 1))
+
+        return result
+
+    def get_unimolecular_job_order(self) -> str:
+        if self.options.unimolecular_dissociation_options.enabled and \
+                self.options.unimolecular_association_options.enabled:
+            assert self.options.unimolecular_dissociation_options.job.order == \
+                self.options.unimolecular_association_options.job.order
+            return self.options.unimolecular_association_options.job.order
+        elif self.options.unimolecular_dissociation_options.enabled:
+            return self.options.unimolecular_dissociation_options.job.order
+        elif self.options.unimolecular_association_options.enabled:
+            return self.options.unimolecular_association_options.job.order
+        else:
+            raise RuntimeError('No reactions enabled, cannot report job order.')
+
+    def get_bimolecular_job_order(self) -> str:
+        return self.options.bimolecular_association_options.job.order
+
+    @_sanity_check_wrapper
+    def unimolecular_reactions(self, structure: db.Structure, with_exact_settings_check: bool = False):
+        """
+        Creates reactive complex calculations corresponding to the unimolecular
+        reactions of the structure if there is not already a calculation to
+        search for a reaction of the same structure with the same job order.
+
+        Parameters
+        ----------
+        structure :: db.Structure
+            The structure to be considered. The Structure has to
+            be linked to a database.
+        with_exact_settings_check :: bool
+            If True, more expensive queries are carried out to check if the settings of the
+            calculations are exactly the same as the settings of the trial generator. This allows to add more
+            inclusive additional reaction trials but the queries are less efficient, therefore this option
+            should be only toggled if necessary.
+        """
+        if self.options.unimolecular_dissociation_options.enabled and \
+                self.options.unimolecular_association_options.enabled:
+            assert self.options.unimolecular_dissociation_options.job.order == \
+                self.options.unimolecular_association_options.job.order
+        if self._quick_unimolecular_already_exists(structure, do_fast_query=not with_exact_settings_check):
+            return
+        structure_id = structure.id()
+
+        # Check whether there is a reactive complex calculation for the same structure already
+        if self.options.unimolecular_dissociation_options.enabled:
+            selection = {
+                "$and": [
+                    {"job.order": {"$eq": self.options.unimolecular_dissociation_options.job.order}},
+                    {"structures": [{"$oid": structure_id.string()}]},
+                    *model_query(self.options.model)
+                ]
+            }
+            if self._calculations.get_one_calculation(dumps(selection)) is not None:
+                return
+        if self.options.unimolecular_association_options.enabled:
+            selection = {
+                "$and": [
+                    {"job.order": {"$eq": self.options.unimolecular_association_options.job.order}},
+                    {"structures": [{"$oid": structure_id.string()}]},
+                    *model_query(self.options.model)
+                ]
+            }
+            if self._calculations.get_one_calculation(dumps(selection)) is not None:
+                return
+
+        reaction_coordinates = self.unimolecular_coordinates(structure, with_exact_settings_check)
+        connectivity_analyzer = ConnectivityAnalyzer(structure)
+
+        def n_diss_error(r_type: ReactionType, n: int) -> str:
+            return f"Analyzed reaction type to be {r_type}, but reaction coordinate " \
+                   f"specifies {n} dissociations, this should not be possible in " \
+                   f"{self.__class__.__name__}"
+
+        new_calculation_ids = []
+        for coordinates, n_diss in reaction_coordinates:
+            for coord in coordinates:
+                reaction_type = connectivity_analyzer.get_reaction_type(coord)
+                if reaction_type == ReactionType.Associative:
+                    if n_diss != 0:
+                        raise RuntimeError(n_diss_error(reaction_type, n_diss))
+                    job = self.options.unimolecular_association_options.job
+                    settings = self.options.unimolecular_association_options.job_settings
+                elif reaction_type == ReactionType.Dissociative:
+                    if n_diss == 0:
+                        raise RuntimeError(n_diss_error(reaction_type, n_diss))
+                    job = self.options.unimolecular_dissociation_options.job
+                    settings = self.options.unimolecular_dissociation_options.job_settings_dissociative
+                elif reaction_type == ReactionType.Disconnective:
+                    if n_diss == 0:
+                        raise RuntimeError(n_diss_error(reaction_type, n_diss))
+                    job = self.options.unimolecular_dissociation_options.job
+                    settings = self.options.unimolecular_dissociation_options.job_settings_disconnective
+                else:
+                    raise RuntimeError(f"Unknown reaction type {reaction_type}")
+                lhs = list(set([c[0] for c in coord]))
+                rhs = list(set([c[1] for c in coord]))
+                cid = self._add_reactive_complex_calculation(
+                    [structure_id],
+                    reaction_type,
+                    lhs,
+                    rhs,
+                    job,
+                    settings,
+                    check_for_existing=with_exact_settings_check
+                )
+                if cid is not None:
+                    new_calculation_ids.append(cid)
+        if new_calculation_ids:
+            structure.add_calculations(self.get_unimolecular_job_order(), [new_calculation_ids[0]])
 
     def _add_reactive_complex_calculation(
         self,
         reactive_structures: List[db.ID],
         reaction_type: ReactionType,
         lhs_list: List[int],
         rhs_list: List[int],
         job: db.Job,
         settings: utils.ValueCollection,
         lhs_alignment: Optional[List[float]] = None,
         rhs_alignment: Optional[List[float]] = None,
         x_rotation: Optional[float] = None,
         spread: Optional[float] = None,
         displacement: Optional[float] = None,
-    ):
+        check_for_existing: bool = False,
+    ) -> Optional[db.ID]:
         """
         Adds a reactive calculation to the database and puts it on hold.
 
         Parameters
         ----------
 
         reactive_structures :: List[db.ID]
@@ -622,68 +729,78 @@
             the x-axis after ``lhs_alignment``, ``rhs_alignment``, and
             ``x_rotation`` have been applied.
         displacement :: float
             In case of two structures building the reactive complex, this option
             adds a random displacement to all atoms (random direction, random
             length). The maximum length of this displacement (per atom) is set to
             be the value of this option.
+        check_for_existing :: bool
+            Whether it should be checked if a calculation with these exact
+            settings and model already exists or not (default: False)
         """
         model = self.options.model
-        calculation = db.Calculation()
-        calculation.link(self._calculations)
-        calculation.create(model, job, reactive_structures)
+        this_settings = self._get_settings(settings)
         # Sleep a bit in order not to make the DB choke
         time.sleep(0.001)
         if lhs_alignment is not None:
-            settings["rc_x_alignment_0"] = lhs_alignment
+            this_settings["rc_x_alignment_0"] = lhs_alignment
         if rhs_alignment is not None:
-            settings["rc_x_alignment_1"] = rhs_alignment
+            this_settings["rc_x_alignment_1"] = rhs_alignment
         if x_rotation is not None:
-            settings["rc_x_rotation"] = x_rotation
+            this_settings["rc_x_rotation"] = x_rotation
         if spread is not None:
-            settings["rc_x_spread"] = spread
+            this_settings["rc_x_spread"] = spread
         if displacement is not None:
-            settings["rc_displacement"] = displacement
+            this_settings["rc_displacement"] = displacement
         if job.order == "scine_react_complex_afir":
-            settings["afir_afir_rhs_list"] = rhs_list
-            settings["afir_afir_lhs_list"] = lhs_list
+            this_settings["afir_afir_rhs_list"] = rhs_list
+            this_settings["afir_afir_lhs_list"] = lhs_list
             # Repulsive for dissociations
-            settings["afir_afir_attractive"] = not bool(reaction_type.value)
+            this_settings["afir_afir_attractive"] = not bool(reaction_type.value)
             # Use maximum fragment distance if disconnective
-            settings["afir_afir_use_max_fragment_distance"] = bool(reaction_type == ReactionType.Disconnective)
+            this_settings["afir_afir_use_max_fragment_distance"] = bool(reaction_type == ReactionType.Disconnective)
             if reaction_type == ReactionType.Disconnective:
                 # Set fragment distance for convergence to 3*sum of maximum covalent radii within i and j
                 struct = db.Structure(reactive_structures[0])
                 struct.link(self._structures)
                 atoms = struct.get_atoms()
                 covalent_max = [
                     max(utils.ElementInfo.covalent_radius(atoms.get_element(atom_index)) for atom_index in frag)
                     for frag in (rhs_list, lhs_list)
                 ]
-                settings["afir_afir_max_fragment_distance"] = 3 * sum(covalent_max)
+                this_settings["afir_afir_max_fragment_distance"] = 3 * sum(covalent_max)
             else:
-                del settings["afir_afir_max_fragment_distance"]
+                del this_settings["afir_afir_max_fragment_distance"]
 
         elif job.order == "scine_react_complex_nt":
-            settings["nt_nt_rhs_list"] = rhs_list
-            settings["nt_nt_lhs_list"] = lhs_list
+            this_settings["nt_nt_rhs_list"] = rhs_list
+            this_settings["nt_nt_lhs_list"] = lhs_list
             # Repulsive for dissociations; attractive (False) for dissociative/disconnective
-            settings["nt_nt_attractive"] = not bool(reaction_type.value)
+            this_settings["nt_nt_attractive"] = not bool(reaction_type.value)
         else:
             raise RuntimeError(
                 "Only 'scine_react_complex_afir' and 'scine_react_complex_nt' "
                 "order supported for fragment-based reactive complex calculations."
             )
 
         if len(reactive_structures) > 1:
-            settings["rc_minimal_spin_multiplicity"] = bool(
-                self.options.bimolecular_association.minimal_spin_multiplicity
+            this_settings["rc_minimal_spin_multiplicity"] = bool(
+                self.options.bimolecular_association_options.minimal_spin_multiplicity
             )
-        calculation.set_settings(deepcopy(settings))
-        finalize_calculation(calculation, self._structures)
+
+        if check_for_existing and get_calculation_id(job.order, reactive_structures, model,
+                                                     self._calculations, settings=this_settings) is not None:
+            return None
+
+        calculation = db.Calculation()
+        calculation.link(self._calculations)
+        calculation.create(model, job, reactive_structures)
+        calculation.set_settings(this_settings)
+        calculation.set_status(db.Status.HOLD)
+        return calculation.id()
 
     def _generate_inter_reactive_coords(
         self,
         structure_list: List[db.Structure],
         reactive_monoatomic1: List[int],
         reactive_monoatomic2: List[int],
         reactive_diatomic1: List[Tuple[int, int]],
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/__init__.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/minimum_energy_conformer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,117 +1,124 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
-from abc import abstractmethod, ABC
-from json import dumps
-from typing import List
+# Standard library imports
+from typing import Tuple, List
+import math
 
+# Third party imports
 import scine_database as db
+import scine_utilities as utils
 
 # Local application imports
-from .compound_filters import CompoundFilter
-from .trial_generator.bond_based import BondBased
-from .. import Gear
-from scine_chemoton.utilities.queries import stop_on_timeout
+from . import ElementaryStepGear
+from ...utilities.energy_query_functions import get_energy_for_structure
 
 
-class ElementaryStepGear(Gear, ABC):
+class MinimumEnergyConformerElementarySteps(ElementaryStepGear):
     """
-    Base class for elementary step reaction generators
+    This Gear probes Reactions by trying to react the minimum energy conformer of each
+    Compound with the minimum energy conformer of the other Compound.
+    For each Structure--Structure combination multiple arrangements (possible
+    Elementary Steps) will be tested.
+
+    This Gear does not consider Flasks/Complexes as reactive, they are not probed
+    for elementary steps.
+
+    Attributes
+    ----------
+    options :: Options
+        The options for the gear.
+    aggregate_filter :: scine_chemoton.gears.elementary_steps.aggregate_filters.AggregateFilter
+        A filter for allowed reaction combinations, per default everything
+        is permitted, no filter is applied.
+    trial_generator :: TrialGenerator
+        The generator to set up elementary step trial calculations by enumerating
+        reactive complexes and trial reaction coordinates
+
+    Notes
+    -----
+    This function assumes maximum spin when adding two Structures into one
+    reactive complex.
+    The need for elementary step guesses is tested by:
+
+    a. for bimolecular reactions: checking whether there is already a
+        calculation to search for a bimolecular reaction of the same
+        structures with the same job order
+    b. for unimolecular reactions: checking whether there is already a
+        calculation to search for an intramolecular reaction of the same
+        structure  with the same job order
     """
 
-    class Options:
-        """
-        The options for an ElementarySteps Gear.
-        """
+    class Options(ElementaryStepGear.Options):
 
-        __slots__ = ("cycle_time", "enable_unimolecular_trials", "enable_bimolecular_trials")
+        __slots__ = ("energy_upper_bound", "max_number_structures")
 
-        def __init__(self):
-            self.cycle_time = 10
-            """
-            int
-                Sleep time between cycles, in seconds.
-            """
-            self.enable_unimolecular_trials = True
+        def __init__(self, *args, **kwargs):
+            super().__init__(*args, **kwargs)
+            self.energy_upper_bound = 12.0
             """
-            bool
-                If `True`, enables the exploration of unimolecular reactions.
+            float
+                Upper bound for the energy difference to the conformer with the lowest energy to
+                be considered in the reaction trial generation (in kJ/mol). Default is 12 kJ/mol
+                which corresponds to an occupation change of ~ 1 % (according to their Boltzmann
+                exponential factors).
             """
-            self.enable_bimolecular_trials = True
+            self.max_number_structures = math.inf
             """
-            bool
-                If `True`, enables the exploration of bimolecular reactions.
+            int
+                The maximum number of structures considered for each compound.
             """
 
+    options: Options
+
     def __init__(self):
         super().__init__()
-        self._required_collections = ["calculations", "compounds", "properties", "reactions", "structures"]
-        self.options = self.Options()
-        self.compound_filter: CompoundFilter = CompoundFilter()
-        self.trial_generator = BondBased()
-
-    def _sanity_check_configuration(self):
-        if not isinstance(self.compound_filter, CompoundFilter):
-            raise TypeError("Expected a CompoundFilter (or a class derived "
-                            "from it) in ElementaryStepGear.compound_filter.")
-
-    def _propagate_db_manager(self, manager: db.Manager):
-        self.trial_generator.initialize_collections(manager)
-        if hasattr(self.trial_generator, 'reactive_site_filter'):
-            self.trial_generator.reactive_site_filter.initialize_collections(manager)
-        if hasattr(self, 'compound_filter'):
-            self.compound_filter.initialize_collections(manager)
-
-    def _loop_impl(self):
-
-        self._sanity_check_configuration()
-
-        # Loop over all compounds
-        selection = {"exploration_disabled": {"$ne": True}}
-        for compound_one in stop_on_timeout(self._compounds.iterate_compounds(dumps(selection))):
-            compound_one.link(self._compounds)
-            eligible_sid_one = None
-            if self.options.enable_unimolecular_trials and self.compound_filter.filter(compound_one):
-                eligible_sid_one = sorted(self._get_eligible_structures(compound_one))
-                for sid_one in eligible_sid_one:
-                    structure_one = db.Structure(sid_one, self._structures)
-                    self.trial_generator.unimolecular_reactions(structure_one)
-            # Get intermolecular reaction partners
-            if not self.options.enable_bimolecular_trials:
+        self._energy_label = "electronic_energy"
+        """
+        str
+            The property label for the energy property.
+        """
+
+    def _check_if_conformers_are_present(self, compound) -> bool:
+        centroid = db.Structure(compound.get_centroid(), self._structures)
+        return centroid.has_property("boltzmann_weight")
+
+    def _get_all_energies_and_structure_ids(self, compound: db.Compound) -> List[Tuple[float, db.ID]]:
+        energies_sids: List[Tuple[float, db.ID]] = list()
+        for sid in compound.get_structures():
+            structure = db.Structure(sid, self._structures)
+            # Only consider optimized structures, no guess structures or duplicates
+            if not structure.explore() or structure.get_label() not in [
+                db.Label.MINIMUM_OPTIMIZED,
+                db.Label.USER_OPTIMIZED,
+            ]:
                 continue
-            if eligible_sid_one is None:
-                eligible_sid_one = sorted(self._get_eligible_structures(compound_one))
-            if not eligible_sid_one:
-                break
-            c_id_one = compound_one.id().string()
-            selection = {"exploration_disabled": {"$ne": True}}
-            for compound_two in stop_on_timeout(self._compounds.iterate_compounds(dumps(selection))):
-                compound_two.link(self._compounds)
-                # Make this loop run lower triangular + diagonal only
-                c_id_two = compound_two.id().string()
-                sorted_ids = sorted([c_id_one, c_id_two])
-                # Second criterion needed to not exclude diagonal
-                if sorted_ids[0] == c_id_two and c_id_one != c_id_two:
-                    continue
-                # Filter
-                if not self.compound_filter.filter(compound_one, compound_two):
-                    continue
-                eligible_sid_two = sorted(self._get_eligible_structures(compound_two))
-                if not eligible_sid_two:
-                    continue
-                same_compounds = c_id_one == c_id_two
-                for i, sid_one in enumerate(eligible_sid_one):
-                    for j, sid_two in enumerate(eligible_sid_two):
-                        if same_compounds and j > i:
-                            break
-                        structure_one = db.Structure(sid_one, self._structures)
-                        structure_two = db.Structure(sid_two, self._structures)
-                        self.trial_generator.bimolecular_reactions([structure_one, structure_two])
+            energy = get_energy_for_structure(structure, self._energy_label, self.options.model,
+                                              self._structures, self._properties)
+            # There may not be an energy available for every structure at the given model.
+            if energy is not None:
+                energies_sids.append((energy, sid))
+        return energies_sids
 
-    @abstractmethod
     def _get_eligible_structures(self, compound: db.Compound) -> List[db.ID]:
-        pass
+        if not self._check_if_conformers_are_present(compound):
+            return []
+        energies_s_ids = self._get_all_energies_and_structure_ids(compound)
+        if not energies_s_ids:
+            return []
+        energies_s_ids_sorted = sorted(energies_s_ids, key=lambda tup: tup[0])
+        minimum_energy = min(energies_s_ids_sorted, key=lambda tup: tup[0])[0]
+        eligible_sids = list()
+        n_added = 0
+        threshold = self.options.energy_upper_bound * utils.HARTREE_PER_KJPERMOL
+        for energy, s_id in energies_s_ids_sorted:
+            if abs(energy - minimum_energy) <= threshold:
+                eligible_sids.append(s_id)
+                n_added += 1
+            if n_added >= self.options.max_number_structures:
+                break
+        return eligible_sids
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/brute_force.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/brute_force.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,17 +25,20 @@
     This Gear does not consider Flasks/Complexes as reactive, they are not probed
     for elementary steps.
 
     Attributes
     ----------
     options :: BruteForceElementarySteps.Options
         The options for the BruteForceElementarySteps Gear.
-    filter :: scine_chemoton.gears.elementary_steps.compound_filter.CompoundFilter
+    aggregate_filter :: scine_chemoton.gears.elementary_steps.aggregate_filters.AggregateFilter
         A filter for allowed reaction combinations, per default everything
         is permitted, no filter is applied.
+    trial_generator :: TrialGenerator
+        The generator to set up elementary step trial calculations by enumerating
+        reactive complexes and trial reaction coordinates
 
     Notes
     -----
     This function assumes maximum spin when adding two Structures into one
     reactive complex.
     The need for elementary step guesses is tested by:
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/compound_filters.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/reactive_site_filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,595 +2,582 @@
 # -*- coding: utf-8 -*-
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
-from typing import Dict, List, Optional
-from collections import Counter
-import numpy as np
+import ast
+from typing import List, Optional, Tuple, Union
 
 # Third party imports
 import scine_database as db
-import scine_utilities as utils
 
-from scine_chemoton.gears import HoldsCollections
-
-
-class CompoundFilter(HoldsCollections):
-    """
-    The base and default class for all filters. The default is to allow/pass all
-    given checks.
-
-    CompoundFilters are optional barriers in Chemoton that allow the user to cut down
-    the exponential growth of the combinatorial explosion. The different
-    subclasses of this main CompoundFilter allow for a tailored choice of which
-    additional branches of the network to allow.
+# Local application imports
+from .reaction_rules.distance_rules import DistanceRuleSet
+from .reaction_rules.element_rules import ElementRuleSet, SimpleElementCombinationRule
+from .reaction_rules.polarization_rules import PolarizationRuleSet
+from scine_chemoton.gears import HoldsCollections, HasName
+from scine_chemoton.utilities.masm import deserialize_molecules, distinct_atoms, get_atom_pairs
+
+
+class ReactiveSiteFilter(HoldsCollections, HasName):
+    """
+    The base and default class for all reactive site filters. The default is to
+    allow/pass all given checks.
+
+    ReactiveSiteFilter are optional barriers in Chemoton that allow the user to
+    cut down the exponential growth of the combinatorial explosion. The
+    different subclasses of this main ReactiveSiteFilter allow for a tailored
+    choice of which parts of a molecule to deem reactive.
 
     There are some predefined filters that will be given in Chemoton, however,
     it should be simple to extend as needed even on a per-project basis.
     The key element when sub-classing this interface is to override the `filter`
     functions as defined here. When sub-classing please be aware that these
     filters are expected to be called often. Having each call do loops over
     entire collections is not wise.
 
     For the latter reason, user defined subclasses are intended to be more
     complex, allowing for non-database stored/cached data across a run.
     This can be a significant speed-up and allow for more intricate filtering.
+
+    The different filter methods are applied in a subsequent matter, i.e.,
+    only the atoms that pass the atom filter will be used to construct atom pairs,
+    and only those of the atom pairs that pass the pair filter will be used to
+    construct trial reaction coordinates in the TrialGenerators.
+
+    NOTE: Although there is the possibility to apply a filter to many sites /
+    trial coordinates simultaneously, there is no guarantee that all possible
+    sites / coordinates with the specified settings are passed at the same time.
     """
 
     def __init__(self):
         super().__init__()
-        self._required_collections = ["calculations", "compounds", "elementary_steps",
+        self._remove_chemoton_from_name()
+        self._required_collections = ["calculations", "compounds", "elementary_steps", "flasks",
                                       "properties", "structures", "reactions"]
 
     def __and__(self, o):
-        if not isinstance(o, CompoundFilter):
-            raise TypeError("CompoundFilter expects CompoundFilter "
+        if not isinstance(o, ReactiveSiteFilter):
+            raise TypeError("ReactiveSiteFilter expects ReactiveSiteFilter "
                             "(or derived class) to chain with.")
-        return CompoundFilterAndArray([self, o])
+        return ReactiveSiteFilterAndArray([self, o])
 
     def __or__(self, o):
-        if not isinstance(o, CompoundFilter):
-            raise TypeError("CompoundFilter expects CompoundFilter "
+        if not isinstance(o, ReactiveSiteFilter):
+            raise TypeError("ReactiveSiteFilter expects ReactiveSiteFilter "
                             "(or derived class) to chain with.")
-        return CompoundFilterOrArray([self, o])
+        return ReactiveSiteFilterOrArray([self, o])
 
-    def filter(self, _: db.Compound, __: db.Compound = None) -> bool:
+    def filter_atoms(self, _: List[db.Structure], atom_indices: List[int]) -> List[int]:
         """
-        The blueprint for a filter function, checking if both of the compounds
-        are allowed to be used in an exploration (logical and). If only one
-        compound is given a check using only that one compound is performed.
-        This default CompoundFilter accepts all compounds.
+        The blueprint for a filter function, checking  a list of atoms
+        regarding their reactivity as defined by the filter.
 
-        Attributes
+        Parameters
         ----------
-        _ :: db.Compound
-            The compound to be checked.
-        _ :: db.Compound
-            The other compound to be checked in the case of bimolecular reactions.
+        _ : List[db.Structure]
+            The structures to be checked. Unused in this function.
+        atom_indices : [List[int]]
+            The list of atoms to consider. If several structures are listed
+            atom indices are expected to refer to the entity of all structure
+            in the order they are given in the structure list.
+            For example, the first atom of the second structure has the index
+            equalling the number of atoms of the first structure.
 
         Returns
         -------
-        result :: bool
-            True if the compound passed the check/filter, False if the compound
-            did not pass the check and should not be used.
+        result : List[int]
+            The list of all relevant atom indices after applying the filter.
         """
-        return True
+        return atom_indices
 
+    def filter_atom_pairs(
+            self, _: List[db.Structure], pairs: List[Tuple[int, int]]
+    ) -> List[Tuple[int, int]]:
+        """
+        The blueprint for a filter function, checking a list of atom pairs
+        regarding their reactivity as defined by the filter.
+
+        Parameters
+        ----------
+        _ : List[db.Structure]
+            The structures to be checked. Unused in this implementation.
+        pairs : List[Tuple[int, int]]
+            The list of atom pairs to consider. If several structures are listed
+            atom indices are expected to refer to the entity of all structure in
+            the order they are given in the structure list.
+            For example, the first atom of the second structure has the index
+            equalling the number of atoms of the first structure.
 
-class CompoundFilterAndArray(CompoundFilter):
+        Returns
+        -------
+        result :: List[Tuple[int, int]]
+            The list of all relevant reactive atom pairs (given as atom index
+            pairs) after applying the filter.
+        """
+        return pairs
+
+    def filter_reaction_coordinates(
+            self, _: List[db.Structure], coordinates: List[List[Tuple[int, int]]]
+    ) -> List[List[Tuple[int, int]]]:
+        """
+        The blueprint for a filter function, checking  a list of trial reaction
+        coordinates each given as a tuple of reactive atom pairs for their
+        reactivity as defined by the filter.
+
+        Parameters
+        ----------
+        _ : List[db.Structure]
+            The structures to be checked. Unused in this implementation.
+        coordinates : List[List[Tuple[int, int]]]
+            The list of trial reaction coordinates to consider.
+            If several structures are listed atom indices are expected to refer
+            to the entity of all structure in the order they are given in the
+            structure list.
+            For example, the first atom of the second structure has the index
+            equalling the number of atoms of the first structure.
+
+        Returns
+        -------
+        result :: List[List[Tuple[int, int]]]
+            The list of all relevant reaction coordinates given as tuples of
+            reactive atom pairs after applying the filter.
+        """
+        return coordinates
+
+
+class ReactiveSiteFilterAndArray(ReactiveSiteFilter):
     """
     An array of logically 'and' connected filters.
 
     Attributes
     ----------
-    filters :: List[CompoundFilter]
+    filters : List[ReactiveSiteFilter]
         A list of filters to be combined.
     """
 
-    def __init__(self, filters: Optional[List[CompoundFilter]] = None):
-        super().__init__()
+    def __init__(self, filters: Optional[List[ReactiveSiteFilter]] = None, **kwargs):
+        super().__init__(**kwargs)  # required for multiple inheritance
         if filters is None:
             filters = []
         self._filters = filters
         for f in filters:
-            if not isinstance(f, CompoundFilter):
-                raise TypeError("CompoundFilterAndArray expects CompoundFilter "
+            if not isinstance(f, ReactiveSiteFilter):
+                raise TypeError("ReactiveSiteFilterAndArray expects ReactiveSiteFilter "
                                 "(or derived class) to chain with.")
+        self._join_names(self._filters)
+
+    def filter_atoms(self, structure_list: List[db.Structure], atom_indices: List[int]) -> List[int]:
+        distinct = atom_indices
+        for filter in self._filters:
+            distinct = filter.filter_atoms(structure_list, distinct)
+
+        return distinct
+
+    def filter_atom_pairs(
+            self, structure_list: List[db.Structure], pairs: List[Tuple[int, int]]
+    ) -> List[Tuple[int, int]]:
+        distinct = pairs
+        for filter in self._filters:
+            distinct = filter.filter_atom_pairs(structure_list, pairs=distinct)
+        return distinct
+
+    def filter_reaction_coordinates(
+            self, structure_list: List[db.Structure], coordinates: List[List[Tuple[int, int]]]
+    ) -> List[List[Tuple[int, int]]]:
+        distinct = coordinates
+        for filter in self._filters:
+            distinct = filter.filter_reaction_coordinates(structure_list, coordinates=distinct)
+        return distinct
 
-    def filter(self, compound_one: db.Compound, compound_two: db.Compound = None) -> bool:
-        ret = True
+    def initialize_collections(self, manager: db.Manager) -> None:
         for f in self._filters:
-            ret = ret and f.filter(compound_one, compound_two)
-        return ret
+            f.initialize_collections(manager)
+
+    def __iter__(self):
+        return (f for f in self._filters)
 
 
-class CompoundFilterOrArray(CompoundFilter):
+class ReactiveSiteFilterOrArray(ReactiveSiteFilter):
     """
     An array of logically 'or' connected filters.
 
     Attributes
     ----------
-    filters :: List[CompoundFilter]
+    filters : List[ReactiveSiteFilter]
         A list of filters to be combined.
     """
 
-    def __init__(self, filters: List[CompoundFilter] = None):
+    def __init__(self, filters: Optional[List[ReactiveSiteFilter]] = None):
         super().__init__()
         if filters is None:
             filters = []
         self._filters = filters
         for f in filters:
-            if not isinstance(f, CompoundFilter):
-                raise TypeError("CompoundFilterOrArray expects CompoundFilter "
+            if not isinstance(f, ReactiveSiteFilter):
+                raise TypeError("ReactiveSiteFilterOrArray expects ReactiveSiteFilter "
                                 "(or derived class) to chain with.")
+        self._join_names(self._filters)
 
-    def filter(self, compound_one: db.Compound, compound_two: db.Compound = None) -> bool:
-        ret = False
-        for f in self._filters:
-            ret = ret or f.filter(compound_one, compound_two)
+    def filter_atoms(self, structure_list: List[db.Structure], atom_indices: List[int]) -> List[int]:
+        ret: List[int] = []
+        for filter in self._filters:
+            distinct = filter.filter_atoms(structure_list, atom_indices)
+            ret = list(set(ret) | set(distinct))
         return ret
 
+    def filter_atom_pairs(
+            self, structure_list: List[db.Structure], pairs: List[Tuple[int, int]]
+    ) -> List[Tuple[int, int]]:
+        ret: List[Tuple[int, int]] = []
+        for filter in self._filters:
+            distinct = filter.filter_atom_pairs(structure_list, pairs=pairs)
+            ret = list(set(ret) | set(distinct))
+        return ret
 
-class ElementCountFilter(CompoundFilter):
-    """
-    Filters by atom counts. All given compounds must resolve to structures
-    that separately fall below the given threshold. No assumptions about atom
-    counts of possible combinations/products are made in this filter.
-
-    Attributes
-    ----------
-    atom_type_count :: Dict[str,int]
-        A dictionary giving the number (values) of allowed occurrences of each
-        atom type (atom symbol string given as keys). Atom symbols not given
-        as keys are interpreted as forbidden.
-    structures :: db.Collection
-        The collection of structures to be used for the counting of elements.
-    """
-
-    def __init__(self, atom_type_count: Dict[str, int], structures: db.Collection):
-        super().__init__()
-        self.counts: Counter = Counter()
-        for k, v in atom_type_count.items():
-            self.counts.update({k.capitalize(): v})
-        self._structures = structures
-
-    def filter(self, compound_one: db.Compound, compound_two: db.Compound = None) -> bool:
-        # One compound case
-        if compound_two is None:
-            structure = db.Structure(compound_one.get_centroid())
-            return self._check_atom_counts(structure)
-        # Two compounds case
-        structure_one = db.Structure(compound_one.get_centroid())
-        structure_two = db.Structure(compound_two.get_centroid())
-        return self._check_atom_counts(structure_one) and self._check_atom_counts(structure_two)
-
-    def _check_atom_counts(self, structure: db.Structure) -> bool:
-        """
-        Checks the atom counts of the given structure against the requirements
-        set in the member variable.
-
-        Attributes
-        ----------
-        structure :: db.Structure
-            The structure of which to check the atom counts.
+    def filter_reaction_coordinates(
+            self, structure_list: List[db.Structure], coordinates: List[List[Tuple[int, int]]]
+    ) -> List[List[Tuple[int, int]]]:
+        ret: List[List[Tuple[int, int]]] = []
+        for filter in self._filters:
+            distinct = filter.filter_reaction_coordinates(structure_list, coordinates=coordinates)
+            for d in distinct:
+                if d not in ret:
+                    ret.append(d)
+        return ret
 
-        Returns
-        -------
-        result :: bool
-            True if the structure passed the check/filter, False if not.
-        """
-        structure.link(self._structures)
-        atoms = structure.get_atoms()
-        elements = [str(x) for x in atoms.elements]
-        for k, v in Counter(elements).items():
-            if self.counts.get(k, 0) - v < 0:
-                return False
-        return True
+    def initialize_collections(self, manager: db.Manager) -> None:
+        for f in self._filters:
+            f.initialize_collections(manager)
 
+    def __iter__(self):
+        return (f for f in self._filters)
 
-class ElementSumCountFilter(CompoundFilter):
-    """
-    Filters by atom counts. All given compounds must resolve to structures
-    that together fall below the given threshold.
 
-    Attributes
-    ----------
-    atom_type_count :: Dict[str,int]
-        A dictionary giving the number (values) of allowed occurrences of each
-        atom type (atom symbol string given as keys). Atom symbols not given
-        as keys are interpreted as forbidden.
-    structures :: db.Collection
-        The collection of structures to be used for the counting of
-        elements.
+class MasmChemicalRankingFilter(ReactiveSiteFilter):
     """
+    Filters atoms by chemical ranking as determined by the Molassembler graph
+    representation.
+    NOTE: Only atoms that pass the atom filtering are considered for the
+    generation of reactive pairs and trial reaction coordinates.
+    Pairs/trial coordinates built from different atoms of the same molecule that
+    are regarded as alike based on the Molassembler graph representation, can,
+    however, be distinct/valid. However, these will not be generated when this
+    filter is applied. Use with care!
+    NOTE: This filter does not have any specific filter methods for pairs and
+    reaction coordinates. The methods of the `ReactiveSiteFilter` base class
+    will be applied.
+
+    Attributes
+    ----------
+    prune : str
+        Whether to prune by molassembler's ranking distinct atoms descriptor.
+        Allowed values: `'None'`, `'Hydrogen'`, `'All'`
+    """
+
+    def __init__(self, prune: str = "None"):
+        super().__init__()
+        self.prune = prune
+        valid_option_values = ["None", "Hydrogen", "All"]
+        if prune not in valid_option_values:
+            raise RuntimeError(f"Option for masm atom pruning invalid: {prune}")
+
+    def filter_atoms(self, structure_list: List[db.Structure], atom_indices: List[int]) -> List[int]:
+
+        if self.prune == "None":
+            return atom_indices
+        distinct = []
+        idx_shift = 0  # To account for the shifting of indices in structures further down the structure_list
+        for structure in structure_list:
+            atom_map = ast.literal_eval(structure.get_graph("masm_idx_map"))
+            mols = deserialize_molecules(structure)
+            for c, m in enumerate(mols):
+                mol_distinct = distinct_atoms(m, self.prune == "Hydrogen")
+                atom_distinct = [atom_map.index((c, i)) + idx_shift for i in mol_distinct]
+                distinct.extend(atom_distinct)
+            idx_shift += structure.get_atoms().size()
+
+        return list(set(atom_indices) & set(distinct))
+
+
+class SimpleRankingFilter(ReactiveSiteFilter):
+    """
+    Filters atoms and bonds by a simple ranking algorithm.
+    All atom types are assigned a basic rank/importance, with ``H`` being rank
+    0, ``C`` being rank 1, ``['N', 'O', 'S', 'P', 'Si']`` being rank 2 and all
+    other elements being rank 3. Based on these initial rankings an importance
+    of atoms and bonds is calculated.
+
+    For atoms the base rank of them self and all bonded atoms is added to give
+    the final importance. Hence, a carbon in CH_4 would rank as 1 and one in
+    CH3OH would rank as 3. The protons in this example would rank 1 and 1, 2.
+
+    For atom pairs and coordinates, the ranking of the atoms in the bond is
+    simply added.
+
+    Attributes
+    ----------
+    atom_threshold : int
+        The threshold for the importance of atoms. All atoms ranking above the
+        threshold will be considered for reactions.
+    pair_threshold : int
+        The threshold for the importance of atom pairs, All pairs ranking above
+        the threshold will be considered for reactions.
+    coordinate_threshold : int
+        The threshold for the importance of trial reaction coordinates, All
+        reaction coordinates ranking above the threshold will be considered
+        for reactions.
+    """
+
+    def __init__(self, atom_threshold: int = 0, pair_threshold: int = 0, coordinate_threshold: int = 0):
+        super().__init__()
+        self.atom_threshold = atom_threshold
+        self.pair_threshold = pair_threshold
+        self.coordinate_threshold = coordinate_threshold
+
+    def filter_atoms(self, structure_list: List[db.Structure], atom_indices: List[int]) -> List[int]:
+        idx_shift = 0  # To account for the shifting of indices in structures further down the structure_list
+        above_threshold = []
+        for structure in structure_list:
+            neighbors = get_atom_pairs(structure, (1, 1), "None")
+            initial_ranks = self._rank_atoms(structure)
+            ranks = [r for r in initial_ranks]
+            for i, j in neighbors:
+                ranks[i] += initial_ranks[j]
+                ranks[j] += initial_ranks[i]
+            for i, rank in enumerate(ranks):
+                if rank > self.atom_threshold:
+                    above_threshold.append(i + idx_shift)
+            idx_shift += structure.get_atoms().size()
+
+        return list(set(atom_indices) & set(above_threshold))
+
+    def filter_atom_pairs(
+            self, structure_list: List[db.Structure], pairs: List[Tuple[int, int]]
+    ) -> List[Tuple[int, int]]:
+        all_atom_ranks = []  # Concatenated atom ranks in the order of the structures
+        for structure in structure_list:
+            neighbors = get_atom_pairs(structure, (1, 1), "None")
+            initial_ranks = self._rank_atoms(structure)
+            atom_ranks = [r for r in initial_ranks]
+            for i, j in neighbors:
+                atom_ranks[i] += initial_ranks[j]
+                atom_ranks[j] += initial_ranks[i]
+
+            all_atom_ranks += atom_ranks
+
+        above_threshold = []
+        for i, j in pairs:
+            if (all_atom_ranks[i] + all_atom_ranks[j]) > self.pair_threshold:
+                above_threshold.append((i, j))
+
+        return above_threshold
+
+    def filter_reaction_coordinates(
+            self, structure_list: List[db.Structure], coordinates: List[List[Tuple[int, int]]]
+    ) -> List[List[Tuple[int, int]]]:
+        all_atom_ranks = []  # Concatenated atom ranks in the order of the structures
+        for structure in structure_list:
+            neighbors = get_atom_pairs(structure, (1, 1), "None")
+            initial_ranks = self._rank_atoms(structure)
+            atom_ranks = [r for r in initial_ranks]
+            for i, j in neighbors:
+                atom_ranks[i] += initial_ranks[j]
+                atom_ranks[j] += initial_ranks[i]
+
+            all_atom_ranks += atom_ranks
+
+        above_threshold = []
+        for coord in coordinates:
+            if sum((all_atom_ranks[pair[0]] + all_atom_ranks[pair[1]]) for pair in coord) > self.coordinate_threshold:
+                above_threshold.append(coord)
 
-    def __init__(self, atom_type_count: Dict[str, int], structures: db.Collection):
-        super().__init__()
-        self.counts: Counter = Counter()
-        for k, v in atom_type_count.items():
-            self.counts.update({k.capitalize(): v})
-        self._structures = structures
-
-    def filter(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
-        # One compound case
-        if compound_two is None:
-            structure = db.Structure(compound_one.get_centroid())
-            counter_tot = self._get_element_counter(structure)
-        # Two compounds case
-        else:
-            structure_one = db.Structure(compound_one.get_centroid())
-            counter_one = self._get_element_counter(structure_one)
-
-            structure_two = db.Structure(compound_two.get_centroid())
-            counter_two = self._get_element_counter(structure_two)
-
-            counter_tot = counter_one + counter_two
-
-        for k, v in counter_tot.items():
-            if self.counts.get(k, 0) - v < 0:
-                return False
-
-        return True
-
-    def _get_element_counter(self, structure: db.Structure) -> Counter:
-        """
-        Gets the element counter of the given structure.
-
-        Attributes
-        ----------
-        structure :: db.Structure
-            The structure of which to get the atom counter.
-
-        Returns
-        -------
-        result :: Counter
-            The Counter of the elements of the given structure.
-        """
+        return above_threshold
 
-        structure.link(self._structures)
+    def _rank_atoms(self, structure: db.Structure):
         atoms = structure.get_atoms()
         elements = [str(x) for x in atoms.elements]
+        ranks = []
+        for e in elements:
+            if e == "H":
+                ranks.append(0)
+            elif e == "C":
+                ranks.append(1)
+            elif e in ["N", "O", "S", "P", "Si"]:
+                ranks.append(2)
+            else:
+                ranks.append(3)
+        return ranks
+
+
+class AtomRuleBasedFilter(ReactiveSiteFilter):
+    """
+    A filter that only classifies atoms as reactive if they correspond to a given rule.
+    The rules are given for each element. They may be an exact, required distance to another
+    atom/element, or they may label an atom as generally reactive or not reactive. If no rules
+    are given for an element, all atoms of this type will be considered as non-reactive independent of exclude_mode\n
+
+    Example rules::
+
+      reactive_site_rules = {
+        'H': DistanceRuleOrArray([SimpleDistanceRule('O', 3), SimpleDistanceRule('N', 1)]),
+        'C': DistanceRuleOrArray([SimpleDistanceRule('O', 2), SimpleDistanceRule('N', 2)]),
+        'O': True,
+        'N': True
+      }
 
-        return Counter(elements)
-
-
-class MolecularWeightFilter(CompoundFilter):
+    Allow reactions for all O and N, for all H that are exactly in a distance of 3 bonds to O or one bond
+    to N, and for all C that are at most two bonds away from O or N.
     """
-    Filters by molecular weight. All given compounds must resolve to structures
-    that separately fall below the given threshold. No assumptions about weights
-    of possible combinations/products are made in this filter.
 
-    Attributes
-    ----------
-    max_weight :: float
-        The maximum weight to be allowed, given in unified atomic mass units (u).
-        For example, dinitrogen has a weight of about 28 u.
-    structures :: db.Collection
-        The collection of structures to be used for the molecular weight
-        calculations.
-    """
-
-    def __init__(self, max_weight: float, structures: db.Collection):
-        super().__init__()
-        self.max_weight = max_weight
-        self._structures = structures
-
-    def filter(self, compound_one: db.Compound, compound_two: db.Compound = None) -> bool:
-        # One compound case
-        if compound_two is None:
-            structure = db.Structure(compound_one.get_centroid())
-            return self._calculate_weight(structure) < self.max_weight
-        # Two compounds case
-        structure_one = db.Structure(compound_one.get_centroid())
-        structure_two = db.Structure(compound_two.get_centroid())
-        weight_one = self._calculate_weight(structure_one)
-        weight_two = self._calculate_weight(structure_two)
-        return weight_one < self.max_weight and weight_two < self.max_weight
-
-    def _calculate_weight(self, structure: db.Structure) -> float:
+    def __init__(self, rules: Union[DistanceRuleSet, dict], exclude_mode=False):
         """
-        Calculates the molecular weight, given a DB structure.
-
-        Attributes
+        Parameters
         ----------
-        structure :: db.Structure
-            The structure of which to calculate the molecular weight.
-
-        Returns
-        -------
-        weight :: float
-            The molecular weight in a.u. .
+        rules :: Union[DistanceRuleSet, dict]
+            The dictionary containing the rules (vide supra). The given dictionary is checked for correct typing.
+        exclude_mode :: bool
+            If true, all atoms are excluded that correspond to the given rules.
         """
-        structure.link(self._structures)
-        atoms = structure.get_atoms()
-        weight = 0.0
-        for e in atoms.elements:
-            weight += utils.ElementInfo.mass(e)
-        return weight
-
-
-class IDFilter(CompoundFilter):
-    """
-    Filters by compound id. Returns true only for the specified compounds.
-    Used for testing purposes.
-
-    Attributes
-    ----------
-    reactive_ids :: List[db.ID]
-        The IDs of the compounds to be considered as reactive.
-    """
-
-    def __init__(self, ids: List[db.ID]):
-        super().__init__()
-        self.reactive_ids = set(id.string() for id in ids)
-
-    def filter(self, compound_one: db.Compound, compound_two: db.Compound = None) -> bool:
-        # Get compound ids
-        compound_ids = set()
-        compound_ids.add(compound_one.get_id().string())
-        if compound_two is not None:
-            compound_ids.add(compound_two.get_id().string())
-        return compound_ids.issubset(self.reactive_ids)
-
-
-class SelfReactionFilter(CompoundFilter):
-    """
-    Filters out bimolecular reactions of compounds with themselves.
-    """
-
-    def filter(self, compound_one: db.Compound, compound_two: db.Compound = None) -> bool:
-        if compound_two is None:
-            # Do not rule out unimolecular reactions
-            return True
-        # Get compound ids
-        compound_one_id = compound_one.get_id().string()
-        compound_two_id = compound_two.get_id().string()
-        return compound_one_id != compound_two_id
-
-
-class TrueMinimumFilter(CompoundFilter):
-    """
-    Filters by checking if compound fulfills requirement to be considered a
-    true minimum. This includes having frequencies and all of them are above a
-    given threshold.
-    All given compounds must resolve to structures that separately only have
-    frequencies above the given threshold. Single atoms or ions are considered
-    as minima automatically.
-    Frequencies must be calculated with the ThermoGear during an exploration,
-    otherwise all compounds and combinations of them are filtered out.
-
-    Attributes
-    ----------
-    structures :: db.Collection
-        The collection of structures to be used to be checked for being a true
-        minimum.
-    properties :: db.Collection
-        The collection of properties to be used to look up frequencies of
-        structures.
-    imaginary_frequency_threshold :: float
-        The frequency in atomic units above which a structure is considered a
-        minimum structure.
-        For example, a molecule with one imaginary frequency of -1e-4 (-138 cm^-1)
-        can be considered a minimum by setting the threshold to -1.1e-4 (-152 cm^-1)
-    """
-
-    def __init__(
-        self,
-        structures: db.Collection,
-        properties: db.Collection,
-        imaginary_frequency_threshold: float = 0.0,
-    ):
         super().__init__()
-        self._structures = structures
-        self._properties = properties
-        self.imaginary_frequency_threshold = imaginary_frequency_threshold
-
-    def filter(self, compound_one: db.Compound, compound_two: db.Compound = None) -> bool:
-        # One compound case
-        if compound_two is None:
-            structure = db.Structure(compound_one.get_centroid())
-            return self._frequency_check(structure)
-        # Two compounds case
-        structure_one = db.Structure(compound_one.get_centroid())
-        structure_two = db.Structure(compound_two.get_centroid())
-        # Frequency Check
-        freq_check_one = self._frequency_check(structure_one)
-        freq_check_two = self._frequency_check(structure_two)
-        return freq_check_one and freq_check_two
-
-    def _frequency_check(self, structure: db.Structure) -> bool:
-        """
-        Checks a structure for its validity as true minimum, meaning it has only
-        frequencies above a set threshold.
-        If no frequencies are available, it fails the check, unless it is a
-        single atom.
-
-        Attributes
-        ----------
-        structure :: db.Structure
-            The structure of which the frequencies are checked.
+        if not isinstance(rules, DistanceRuleSet):
+            self._rules = DistanceRuleSet(rules)
+        else:
+            self._rules = rules
+        self._return_value_upon_hit = not exclude_mode
 
-        Returns
-        -------
-        result :: bool
-            Boolean indicating if structure is true minimum.
-        """
-        structure.link(self._structures)
-        # # # Check for single atom
-        if len(structure.get_atoms()) == 1:
-            return True
-
-        # # # Check, if frequencies exist; if not, the compound will not be
-        # # # considered for exploration
-        if not structure.has_property("frequencies"):
-            return False
-        # # # Get Frequencies
-        freq_id = structure.get_property("frequencies")
-        freq = self._properties.get_vector_property(freq_id)
-        freq.link(self._properties)
-
-        # # # Check, if there is a frequency below the threshold
-        return not np.any(freq.get_data() < self.imaginary_frequency_threshold)
-
-
-class CatalystFilter(CompoundFilter):
-    """
-    Filters by defining an important structural motive.
-    A user defined set of atoms present in a structure identify it to be the, or
-    a version of the catalyst. This simple check should work great for common
-    transition metal catalysts.
-
-    Only specific reactions revolving around a catalytic cycle are then allowed:
-    i) reactions that feature the catalyst and one other compound that is not
-    the catalyst.
-    ii) reactions that only involve a single compound (not restricted to the
-    catalyst, unless specified otherwise with flag (see parameters))
+    def filter_atoms(self, structure_list: List[db.Structure], atom_indices: List[int]) -> List[int]:
+        reactive_atom_indices = []
+        idx_shift = 0
+        for structure in structure_list:
+            atoms = structure.get_atoms()
+            elements = [str(x) for x in atoms.elements]
+            molecules = deserialize_molecules(structure)
+            idx_map = ast.literal_eval(structure.get_graph("masm_idx_map"))
+            for i, e in enumerate(elements):
+                # If no rule is specified, set the atom to be not reactive.
+                if e not in self._rules:
+                    continue
+                rule = self._rules[e]
+                if rule.filter_by_rule(molecules, idx_map, elements, i) == self._return_value_upon_hit:
+                    reactive_atom_indices.append(i + idx_shift)
+            idx_shift += structure.get_atoms().size()
+        return list(set(atom_indices) & set(reactive_atom_indices))
+
+
+class ElementWiseReactionCoordinateFilter(ReactiveSiteFilter):
+    """
+    A filter that can restrict the combination of atoms with a specific element.
+    The filter can be operated in two modes: Allow all reaction coordinates for the
+    element combinations encoded in the rules or forbid all of them.\n
+    Example rules::
+
+      reaction_coordinate_rules = {
+        'H': ['H', 'C']
+      }
 
-    Attributes
-    ----------
-    atom_type_count :: Dict[str,int]
-        A dictionary giving the number (values) of atoms that are expected to be
-        only present in - and thus defining - the catalyst. Atom type (atom
-        symbol strings) are given as keys. Atom symbols not given are considered
-        to be irrelevant to the check and may be present in the catalyst. In
-        order to ban atoms, set their count to zero.
-    structures :: db.Collection
-        The collection of structures to be used for the counting of elements.
-    restrict_unimolecular_to_catalyst :: bool
-        Whether unimolecular reactions should also be limited to the catalyst.
+    In the default "forbid-mode" these rules mean that no reaction coordinates between two H-atoms and H and C are
+    allowed.
     """
 
-    def __init__(self, atom_type_count: Dict[str, int], structures: db.Collection,
-                 restrict_unimolecular_to_catalyst: bool = False):
-        super().__init__()
-        self.counts: Counter = Counter()
-        for k, v in atom_type_count.items():
-            self.counts.update({k.capitalize(): v})
-        self._structures = structures
-        self._restrict_unimolecular_to_catalyst = restrict_unimolecular_to_catalyst
-
-    def filter(self, compound_one: db.Compound, compound_two: db.Compound = None) -> bool:
-        # One compound case
-        if compound_two is None:
-            if self._restrict_unimolecular_to_catalyst:
-                return self._check_if_catalyst(db.Structure(compound_one.get_centroid()))
-            return True
-        # Two compounds case
-        structure_one = db.Structure(compound_one.get_centroid())
-        structure_two = db.Structure(compound_two.get_centroid())
-        return self._check_if_catalyst(structure_one) != self._check_if_catalyst(structure_two)
-
-    def _check_if_catalyst(self, structure: db.Structure) -> bool:
+    def __init__(self, rules: Union[ElementRuleSet, dict], reactive_if_rules_apply: bool = False):
         """
-        Check if the given structure is the or a version of the catalyst.
-
-        Attributes
+        Parameters
         ----------
-        structure :: db.Structure
-            The structure of which to check.
-
-        Returns
-        -------
-        check :: bool
-            True is the structure is a version of the catalyst.
+        rules : Union[ElementRuleSet, dict]
+            The dictionary containing the rules. The given dictionary is checked for correct typing.
+        reactive_if_rules_apply : bool
+            The mode to operate the filter in. If true, only reaction coordinates in the given rule set pass.
+            If false, no reaction coordinate in the given rule set pass. By default, false.
         """
-        structure.link(self._structures)
-        atoms = structure.get_atoms()
-        elements = [str(x) for x in atoms.elements]
-        actual = Counter(elements)
-        for k, v in self.counts.items():
-            if actual.get(k, 0) != v:
-                return False
-        return True
+        super().__init__()
+        if not isinstance(rules, ElementRuleSet):
+            self._rules = ElementRuleSet(rules, rule_type=SimpleElementCombinationRule)
+        else:
+            self._rules = rules
+        self._reactive_if_rules_apply = reactive_if_rules_apply
 
+    def filter_atom_pairs(
+            self, structure_list: List[db.Structure], pairs: List[Tuple[int, int]]
+    ) -> List[Tuple[int, int]]:
+        all_element_symbols = []
+        for structure in structure_list:
+            atoms = structure.get_atoms()
+            elements = [str(x) for x in atoms.elements]
+            all_element_symbols += elements
+
+        valid_pairs = []
+        for pair in pairs:
+            rule_applies = self._any_rule_applies(all_element_symbols[pair[0]], all_element_symbols[pair[1]])
+            if self._reactive_if_rules_apply == rule_applies:
+                valid_pairs.append(pair)
+        return valid_pairs
+
+    def _any_rule_applies(self, element_1: str, element_2: str):
+        if element_1 in self._rules:
+            if self._rules[element_1].rule_applies(element_1, element_2):
+                return True
+        return element_2 in self._rules and self._rules[element_2].rule_applies(element_1, element_2)
 
-class AtomNumberFilter(CompoundFilter):
-    """
-    Filters out all compounds with a total number of atoms larger than the given
-    value. For multiple compounds the total number of atoms has to be equal or
-    smaller than the given value.
 
-    Attributes
-    ----------
-    max_n_atoms :: int
-        The maximum number of allowed atoms.
-    structures :: db.Collection
-        The collection of structures to be used for the counting of elements.
+class HeuristicPolarizationReactionCoordinateFilter(ReactiveSiteFilter):
     """
+    Reaction coordinates are only allowed that combine polarizations '+' and '-', or '+-' with either '+' or '-'.
+    The polarizations are defined by the given PolarizationRuleSet
 
-    def __init__(self, max_n_atoms: int, structures: db.Collection):
-        super().__init__()
-        self.max_n_atoms = max_n_atoms
-        self._structures = structures
+    Example rules::
 
-    def filter(self, compound_one: db.Compound, compound_two: db.Compound = None) -> bool:
-        structure_one = db.Structure(compound_one.get_centroid())
-        structure_one.link(self._structures)
-        n_atoms = len(structure_one.get_atoms())
-        if not (compound_two is None):
-            structure_two = db.Structure(compound_two.get_centroid())
-            structure_two.link(self._structures)
-            n_atoms += len(structure_two.get_atoms())
-        return n_atoms <= self.max_n_atoms
-
-
-class OneCompoundIDFilter(CompoundFilter):
-    """
-    Filters all compounds that are not present on a given "white list" of IDs.
-    In the case of multiple compounds, at least one has to be present in the
-    list. Note that this is identical to the IDFilter in the case of only one
-    compound.
+      rules = {
+        'H': [PolarizationFunctionalGroupRule("+", 2, 'C', (3, 3), {'N': 1, 'O': 1})],
+        'C': PaulingElectronegativityRule(),
+        'N': PaulingElectronegativityRule(),
+        'O': PaulingElectronegativityRule()
+      }
 
-    Attributes
-    ----------
-    reactive_ids :: List[db.ID]
-        The IDs of the compounds to be considered as reactive.
     """
 
-    def __init__(self, ids: List[db.ID]):
+    def __init__(self, rules: Union[PolarizationRuleSet, dict]):
+        """
+        Parameters
+        ----------
+        rules : Union[PolarizationRuleSet, dict]
+            The dictionary containing the rules. The given dictionary is checked for correct typing.
+        """
         super().__init__()
-        self.reactive_ids = set(id.string() for id in ids)
-
-    def filter(self, compound_one: db.Compound, compound_two: db.Compound = None) -> bool:
-        if compound_one.get_id().string() in self.reactive_ids:
-            return True
-        if compound_two is not None:
-            if compound_two.get_id().string() in self.reactive_ids:
-                return True
-        return False
-
-
-class SelectedCompoundIDFilter(CompoundFilter):
-    """
-    Filters all compounds for which one needs to be one a given "white list"
-    of reactive compounds and the other has to be either on a list of
-    compounds of interest or on the list of reactive compounds.
-
-    Attributes
-    ----------
-    reactive_ids :: List[db.ID]
-        The IDs of the compounds to be considered as reactive.
-    selected_ids :: List[db.ID]
-        The IDs of the compounds to be of interest.
-    """
+        if not isinstance(rules, PolarizationRuleSet):
+            self._rules = PolarizationRuleSet(rules)
+        else:
+            self._rules = rules
 
-    def __init__(self, reactive_ids: List[db.ID], selected_ids: List[db.ID]):
-        super().__init__()
-        self.reactive_ids = set(id.string() for id in reactive_ids)
-        self.selected_ids = set(id.string() for id in selected_ids)
+    def filter_atom_pairs(
+            self, structure_list: List[db.Structure], pairs: List[Tuple[int, int]]
+    ) -> List[Tuple[int, int]]:
+        all_polarization_characters = []
+        for structure in structure_list:
+            all_polarization_characters += self._get_characters_for_structure(structure)
+
+        valid_pairs = []
+        for pair in pairs:
+            character_0 = all_polarization_characters[pair[0]]
+            character_1 = all_polarization_characters[pair[1]]
+            plus_minus = '+' in character_0 and '-' in character_1
+            minus_plus = '-' in character_0 and '+' in character_1
+            # Valid atom pairs must combine + and - signs.
+            if plus_minus or minus_plus:
+                valid_pairs.append(pair)
+        return valid_pairs
 
-    def filter(self, compound_one: db.Compound, compound_two: db.Compound = None) -> bool:
-        # One compound case: the id has to be a member of the reactive_ids.
-        # Two compound case: one of the ids has to be a member of the reactive_ids.
-        #                   The other one has to be either a member of the reactive_ids or the selected_ids.
-        one_is_reactive = compound_one.get_id().string() in self.reactive_ids
-        # One compound case
-        if compound_two is None:
-            return one_is_reactive
-        # Two compound case
-        two_is_reactive = compound_two.get_id().string() in self.reactive_ids
-        one_is_selected = compound_one.get_id().string() in self.selected_ids or one_is_reactive
-        two_is_selected = compound_two.get_id().string() in self.selected_ids or two_is_reactive
-        return (one_is_reactive and two_is_selected) or (two_is_reactive and one_is_selected)
+    def _get_characters_for_structure(self, structure: db.Structure):
+        atoms = structure.get_atoms()
+        elements = [str(x) for x in atoms.elements]
+        molecules = deserialize_molecules(structure)
+        idx_map = ast.literal_eval(structure.get_graph("masm_idx_map"))
+        string_list = []
+        for atom_index, element in enumerate(elements):
+            if element not in self._rules:
+                string_list.append('')
+            else:
+                rule = self._rules[element]
+                string_list.append(rule.string_from_rule(molecules, idx_map, elements, atom_index))
+        return string_list
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/minimal.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/minimal.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     This Gear does not consider Flasks/Complexes as reactive, they are not probed
     for elementary steps.
 
     Attributes
     ----------
     options :: MinimalElementarySteps.Options
         The options for the MinimalElementarySteps Gear.
-    compound_filter :: scine_chemoton.gears.elementary_steps.compound_filters.CompoundFilter
+    aggregate_filter :: scine_chemoton.gears.elementary_steps.aggregate_filters.AggregateFilter
         A filter for allowed reaction combinations, per default everything
         is permitted, no filter is applied.
     trial_generator :: TrialGenerator
         The generator to set up elementary step trial calculations by enumerating
         reactive complexes and trial reaction coordinates
 
     Notes
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/elementary_steps/reactive_site_filters.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/elementary_steps/aggregate_filters.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,766 +2,924 @@
 # -*- coding: utf-8 -*-
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
-from typing import List, Optional, Tuple
+from typing import Dict, List, Optional, Union
+from collections import Counter
+import numpy as np
 
 # Third party imports
 import scine_database as db
-import scine_molassembler as masm
+import scine_utilities as utils
 
-# Local application imports
-from ...utilities.masm import deserialize_molecules, distinct_atoms, get_atom_pairs
-from scine_chemoton.gears import HoldsCollections
+from scine_chemoton.gears import HoldsCollections, HasName
+from ..kinetic_modeling.concentration_query_functions import query_concentration_with_object
 
 
-class ReactiveSiteFilter(HoldsCollections):
+class AggregateFilter(HoldsCollections, HasName):
     """
-    The base and default class for all reactive site filters. The default is to
-    allow/pass all given checks.
+    The base and default class for all filters. The default is to allow/pass all
+    given checks.
 
-    ReactiveSiteFilter are optional barriers in Chemoton that allow the user to
-    cut down the exponential growth of the combinatorial explosion. The
-    different subclasses of this main ReactiveSiteFilter allow for a tailored
-    choice of which parts of a molecule to deem reactive.
+    CompoundFilters are optional barriers in Chemoton that allow the user to cut down
+    the exponential growth of the combinatorial explosion. The different
+    subclasses of this main AggregateFilter allow for a tailored choice of which
+    additional branches of the network to allow.
 
     There are some predefined filters that will be given in Chemoton, however,
     it should be simple to extend as needed even on a per-project basis.
     The key element when sub-classing this interface is to override the `filter`
     functions as defined here. When sub-classing please be aware that these
     filters are expected to be called often. Having each call do loops over
     entire collections is not wise.
 
     For the latter reason, user defined subclasses are intended to be more
     complex, allowing for non-database stored/cached data across a run.
     This can be a significant speed-up and allow for more intricate filtering.
-
-    The different filter methods are applied in a subsequent matter, i.e.,
-    only the atoms that pass the atom filter will be used to construct atom pairs,
-    and only those of the atom pairs that pass the pair filter will be used to
-    construct trial reaction coordinates in the TrialGenerators.
-
-    NOTE: Although there is the possibility to apply a filter to many sites /
-    trial coordinates simultaneously, there is no guarantee that all possible
-    sites / coordinates with the specified settings are passed at the same time.
     """
 
     def __init__(self):
         super().__init__()
-        self._required_collections = ["calculations", "compounds", "elementary_steps", "flasks",
-                                      "properties", "structures", "reactions"]
+        self._remove_chemoton_from_name()
+        self._required_collections = ["calculations", "compounds", "elementary_steps",
+                                      "flasks", "properties", "structures", "reactions"]
+        self._can_cache: bool = True
+        self._currently_caches: bool = True
+        self._cache: Dict[int, bool] = {}
 
     def __and__(self, o):
-        if not isinstance(o, ReactiveSiteFilter):
-            raise TypeError("ReactiveSiteFilter expects ReactiveSiteFilter "
+        if not isinstance(o, AggregateFilter):
+            raise TypeError("AggregateFilter expects AggregateFilter "
                             "(or derived class) to chain with.")
-        return ReactiveSiteFilterAndArray([self, o])
+        return AggregateFilterAndArray([self, o])
 
     def __or__(self, o):
-        if not isinstance(o, ReactiveSiteFilter):
-            raise TypeError("ReactiveSiteFilter expects ReactiveSiteFilter "
+        if not isinstance(o, AggregateFilter):
+            raise TypeError("AggregateFilter expects AggregateFilter "
                             "(or derived class) to chain with.")
-        return ReactiveSiteFilterOrArray([self, o])
+        return AggregateFilterOrArray([self, o])
 
-    def filter_atoms(self, _: List[db.Structure], atom_indices: List[int]) -> List[int]:
+    def disable_caching(self) -> None:
+        """
+        Disables the cache in this filter and flushes the existing cache.
         """
-        The blueprint for a filter function, checking  a list of atoms
-        regarding their reactivity as defined by the filter.
+        self._currently_caches = False
+        self._cache = {}
 
-        Parameters
-        ----------
-        _ : List[db.Structure]
-            The structures to be checked. Unused in this function.
-        atom_indices : [List[int]]
-            The list of atoms to consider. If several structures are listed
-            atom indices are expected to refer to the entity of all structure
-            in the order they are given in the structure list.
-            For example, the first atom of the second structure has the index
-            equalling the number of atoms of the first structure.
+    def enable_caching(self) -> None:
+        """
+        Enables the cache in this filter.
+        """
+        if self._can_cache:
+            self._currently_caches = True
+        else:
+            raise RuntimeError("Cannot enable_caching in filter that cannot cache.")
 
+    def currently_caches(self) -> bool:
+        """
         Returns
         -------
-        result : List[int]
-            The list of all relevant atom indices after applying the filter.
+        result :: bool
+            True if the filter is currently set to cache results, and return
+            results from cache if possible.
         """
-        return atom_indices
+        return self._currently_caches
 
-    def filter_atom_pairs(
-            self, _: List[db.Structure], pairs: List[Tuple[int, int]]
-    ) -> List[Tuple[int, int]]:
+    def can_cache(self) -> bool:
+        """
+        Returns
+        -------
+        result :: bool
+            True if the filter can possibly cache results.
         """
-        The blueprint for a filter function, checking a list of atom pairs
-        regarding their reactivity as defined by the filter.
+        return self._can_cache
 
-        Parameters
+    @staticmethod
+    def _hash_compounds(compound: db.Compound, optional_compound: Optional[db.Compound] = None) -> int:
+        if optional_compound is not None:
+            return hash(';'.join(sorted([compound.get_id().string(), optional_compound.get_id().string()])))
+        else:
+            return hash(compound.get_id().string())
+
+    def filter(self, compound: db.Compound, optional_compound: Optional[db.Compound] = None) -> bool:
+        """
+        The filter function, checking if both of the compounds
+        are allowed to be used in an exploration (logical and). If only one
+        compound is given a check using only that one compound is performed.
+        This default AggregateFilter accepts all compounds.
+
+        Attributes
         ----------
-        _ : List[db.Structure]
-            The structures to be checked. Unused in this implementation.
-        pairs : List[Tuple[int, int]]
-            The list of atom pairs to consider. If several structures are listed
-            atom indices are expected to refer to the entity of all structure in
-            the order they are given in the structure list.
-            For example, the first atom of the second structure has the index
-            equalling the number of atoms of the first structure.
+        compound :: db.Compound
+            The compound to be checked.
+        optional_compound :: db.Compound
+            The other compound to be checked in the case of bimolecular reactions.
 
         Returns
         -------
-        result :: List[Tuple[int, int]]
-            The list of all relevant reactive atom pairs (given as atom index
-            pairs) after applying the filter.
-        """
-        return pairs
-
-    def filter_reaction_coordinates(
-            self, _: List[db.Structure], coordinates: List[List[Tuple[int, int]]]
-    ) -> List[List[Tuple[int, int]]]:
-        """
-        The blueprint for a filter function, checking  a list of trial reaction
-        coordinates each given as a tuple of reactive atom pairs for their
-        reactivity as defined by the filter.
+        result :: bool
+            True if the compound passed the check/filter, False if the compound
+            did not pass the check and should not be used.
+        """
+        if self._can_cache and self._currently_caches:
+            key = self._hash_compounds(compound, optional_compound)
+            result = self._cache.get(key)
+            if result is None:
+                result = self._filter_impl(compound, optional_compound)
+                self._cache[key] = result
+            return result
+        else:
+            return self._filter_impl(compound, optional_compound)
+
+    def _filter_impl(self, _: db.Compound, __: Optional[db.Compound] = None) -> bool:
+        """
+        The blueprint for a filter implementation function.
+        See public function for detailed description.
+        This default AggregateFilter accepts all compounds.
 
-        Parameters
+        Attributes
         ----------
-        _ : List[db.Structure]
-            The structures to be checked. Unused in this implementation.
-        coordinates : List[List[Tuple[int, int]]]
-            The list of trial reaction coordinates to consider.
-            If several structures are listed atom indices are expected to refer
-            to the entity of all structure in the order they are given in the
-            structure list.
-            For example, the first atom of the second structure has the index
-            equalling the number of atoms of the first structure.
+        _ :: db.Compound
+            The compound to be checked.
+        __ :: db.Compound
+            The other compound to be checked in the case of bimolecular reactions.
 
         Returns
         -------
-        result :: List[List[Tuple[int, int]]]
-            The list of all relevant reaction coordinates given as tuples of
-            reactive atom pairs after applying the filter.
+        result :: bool
+            True if the compound passed the check/filter, False if the compound
+            did not pass the check and should not be used.
         """
-        return coordinates
+        return True
 
 
-class ReactiveSiteFilterAndArray(ReactiveSiteFilter):
+class AggregateFilterAndArray(AggregateFilter):
     """
     An array of logically 'and' connected filters.
 
     Attributes
     ----------
-    filters : List[ReactiveSiteFilter]
+    filters :: List[AggregateFilter]
         A list of filters to be combined.
     """
 
-    def __init__(self, filters: Optional[List[ReactiveSiteFilter]] = None):
+    def __init__(self, filters: Optional[List[AggregateFilter]] = None):
         super().__init__()
         if filters is None:
             filters = []
-        self.filters = filters
+        self._filters = filters
         for f in filters:
-            if not isinstance(f, ReactiveSiteFilter):
-                raise TypeError("ReactiveSiteFilterAndArray expects ReactiveSiteFilter "
+            if not isinstance(f, AggregateFilter):
+                raise TypeError("AggregateFilterAndArray expects AggregateFilter "
                                 "(or derived class) to chain with.")
+        self._join_names(self._filters)
+        # Check if caching is an option
+        self._can_cache = True
+        self._currently_caches = True
+        for f in self._filters:
+            if not f.can_cache():
+                self._can_cache = False
+                self._currently_caches = False
+                break
+        # Disable all caches if this array can cache
+        #   If this filter can not cache, lower filters
+        #   that can cache are still allowed to
+        if self._can_cache:
+            for f in self._filters:
+                f.disable_caching()
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        ret = True
+        for f in self._filters:
+            ret = ret and f.filter(compound_one, compound_two)
+        return ret
+
+    def initialize_collections(self, manager: db.Manager) -> None:
+        for f in self._filters:
+            f.initialize_collections(manager)
 
-    def filter_atoms(self, structure_list: List[db.Structure], atom_indices: List[int]) -> List[int]:
-        distinct = atom_indices
-        for filter in self.filters:
-            distinct = filter.filter_atoms(structure_list, distinct)
-
-        return distinct
-
-    def filter_atom_pairs(
-            self, structure_list: List[db.Structure], pairs: List[Tuple[int, int]]
-    ) -> List[Tuple[int, int]]:
-        distinct = pairs
-        for filter in self.filters:
-            distinct = filter.filter_atom_pairs(structure_list, pairs=distinct)
-        return distinct
-
-    def filter_reaction_coordinates(
-            self, structure_list: List[db.Structure], coordinates: List[List[Tuple[int, int]]]
-    ) -> List[List[Tuple[int, int]]]:
-        distinct = coordinates
-        for filter in self.filters:
-            distinct = filter.filter_reaction_coordinates(structure_list, coordinates=distinct)
-        return distinct
+    def __iter__(self):
+        return (f for f in self._filters)
 
 
-class ReactiveSiteFilterOrArray(ReactiveSiteFilter):
+class AggregateFilterOrArray(AggregateFilter):
     """
     An array of logically 'or' connected filters.
 
     Attributes
     ----------
-    filters : List[ReactiveSiteFilter]
+    filters :: List[AggregateFilter]
         A list of filters to be combined.
     """
 
-    def __init__(self, filters: Optional[List[ReactiveSiteFilter]] = None):
+    def __init__(self, filters: Optional[List[AggregateFilter]] = None):
         super().__init__()
         if filters is None:
             filters = []
-        self.filters = filters
+        self._filters = filters
         for f in filters:
-            if not isinstance(f, ReactiveSiteFilter):
-                raise TypeError("ReactiveSiteFilterOrArray expects ReactiveSiteFilter "
+            if not isinstance(f, AggregateFilter):
+                raise TypeError("AggregateFilterOrArray expects AggregateFilter "
                                 "(or derived class) to chain with.")
-
-    def filter_atoms(self, structure_list: List[db.Structure], atom_indices: List[int]) -> List[int]:
-        ret: List[int] = []
-        for filter in self.filters:
-            distinct = filter.filter_atoms(structure_list, atom_indices)
-            ret = list(set(ret) | set(distinct))
+        self._join_names(self._filters)
+        # Check if caching is an option
+        self._can_cache = True
+        self._currently_caches = True
+        for f in self._filters:
+            if not f.can_cache():
+                self._can_cache = False
+                self._currently_caches = False
+                break
+        # Disable all caches if this array can cache
+        #   If this filter can not cache, lower filters
+        #   that can cache are still allowed to
+        if self._can_cache:
+            for f in self._filters:
+                f.disable_caching()
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        ret = False
+        for f in self._filters:
+            ret = ret or f.filter(compound_one, compound_two)
         return ret
 
-    def filter_atom_pairs(
-            self, structure_list: List[db.Structure], pairs: List[Tuple[int, int]]
-    ) -> List[Tuple[int, int]]:
-        ret: List[Tuple[int, int]] = []
-        for filter in self.filters:
-            distinct = filter.filter_atom_pairs(structure_list, pairs=pairs)
-            ret = list(set(ret) | set(distinct))
-        return ret
+    def initialize_collections(self, manager: db.Manager) -> None:
+        for f in self._filters:
+            f.initialize_collections(manager)
 
-    def filter_reaction_coordinates(
-            self, structure_list: List[db.Structure], coordinates: List[List[Tuple[int, int]]]
-    ) -> List[List[Tuple[int, int]]]:
-        ret: List[List[Tuple[int, int]]] = []
-        for filter in self.filters:
-            distinct = filter.filter_reaction_coordinates(structure_list, coordinates=coordinates)
-            ret = list(set(ret) | set(distinct))
-        return ret
+    def __iter__(self):
+        return (f for f in self._filters)
 
 
-class MasmChemicalRankingFilter(ReactiveSiteFilter):
+class ElementCountFilter(AggregateFilter):
     """
-    Filters atoms by chemical ranking as determined by the Molassembler graph
-    representation.
-    NOTE: Only atoms that pass the atom filtering are considered for the
-    generation of reactive pairs and trial reaction coordinates.
-    Pairs/trial coordinates built from different atoms of the same molecule that
-    are regarded as alike based on the Molassembler graph representation, can,
-    however, be distinct/valid. However, these will not be generated when this
-    filter is applied. Use with care!
-    NOTE: This filter does not have any specific filter methods for pairs and
-    reaction coordinates. The methods of the `ReactiveSiteFilter` base class
-    will be applied.
-
-    Attributes
-    ----------
-    prune : str
-        Whether to prune by molassembler's ranking distinct atoms descriptor.
-        Allowed values: `'None'`, `'Hydrogen'`, `'All'`
-    """
-
-    def __init__(self, prune: str = "None"):
-        super().__init__()
-        self.prune = prune
-        valid_option_values = ["None", "Hydrogen", "All"]
-        if prune not in valid_option_values:
-            msg = "Option for masm atom pruning invalid: {}"
-            raise RuntimeError(msg.format(prune))
-
-    def filter_atoms(self, structure_list: List[db.Structure], atom_indices: List[int]) -> List[int]:
-        import ast
-
-        if self.prune == "None":
-            return atom_indices
-        distinct = []
-        idx_shift = 0  # To account for the shifting of indices in structures further down the structure_list
-        for structure in structure_list:
-            atom_map = ast.literal_eval(structure.get_graph("masm_idx_map"))
-            mols = deserialize_molecules(structure)
-            for c, m in enumerate(mols):
-                mol_distinct = distinct_atoms(m, self.prune == "Hydrogen")
-                atom_distinct = [atom_map.index((c, i)) + idx_shift for i in mol_distinct]
-                distinct.extend(atom_distinct)
-            idx_shift += structure.get_atoms().size()
-
-        return list(set(atom_indices) & set(distinct))
-
-
-class SimpleRankingFilter(ReactiveSiteFilter):
-    """
-    Filters atoms and bonds by a simple ranking algorithm.
-    All atom types are assigned a basic rank/importance, with ``H`` being rank
-    0, ``C`` being rank 1, ``['N', 'O', 'S', 'P', 'Si']`` being rank 2 and all
-    other elements being rank 3. Based on these initial rankings an importance
-    of atoms and bonds is calculated.
-
-    For atoms the base rank of them self and all bonded atoms is added to give
-    the final importance. Hence a carbon in CH_4 would rank as 1 and one in
-    CH3OH would rank as 3. The protons in this example would rank 1 and 1, 2.
-
-    For atom pairs and coordinates, the ranking of the atoms in the bond is
-    simply added.
-
-    Attributes
-    ----------
-    atom_threshold : int
-        The threshold for the importance of atoms. All atoms ranking above the
-        threshold will be considered for reactions.
-    pair_threshold : int
-        The threshold for the importance of atom pairs, All pairs ranking above
-        the threshold will be considered for reactions.
-    coordinate_threshold : int
-        The threshold for the importance of trial reaction coordinates, All
-        reaction coordinates ranking above the threshold will be considered
-        for reactions.
-    """
-
-    def __init__(self, atom_threshold: int = 0, pair_threshold: int = 0, coordinate_threshold: int = 0):
-        super().__init__()
-        self.atom_threshold = atom_threshold
-        self.pair_threshold = pair_threshold
-        self.coordinate_threshold = coordinate_threshold
-
-    def filter_atoms(self, structure_list: List[db.Structure], atom_indices: List[int]) -> List[int]:
-        idx_shift = 0  # To account for the shifting of indices in structures further down the structure_list
-        above_threshold = []
-        for structure in structure_list:
-            neighbors = get_atom_pairs(structure, (1, 1), "None")
-            initial_ranks = self._rank_atoms(structure)
-            ranks = [r for r in initial_ranks]
-            for i, j in neighbors:
-                ranks[i] += initial_ranks[j]
-                ranks[j] += initial_ranks[i]
-            for i, rank in enumerate(ranks):
-                if rank > self.atom_threshold:
-                    above_threshold.append(i + idx_shift)
-            idx_shift += structure.get_atoms().size()
-
-        return list(set(atom_indices) & set(above_threshold))
-
-    def filter_atom_pairs(
-            self, structure_list: List[db.Structure], pairs: List[Tuple[int, int]]
-    ) -> List[Tuple[int, int]]:
-        all_atom_ranks = []  # Concatenated atom ranks in the order of the structures
-        for structure in structure_list:
-            neighbors = get_atom_pairs(structure, (1, 1), "None")
-            initial_ranks = self._rank_atoms(structure)
-            atom_ranks = [r for r in initial_ranks]
-            for i, j in neighbors:
-                atom_ranks[i] += initial_ranks[j]
-                atom_ranks[j] += initial_ranks[i]
-
-            all_atom_ranks += atom_ranks
-
-        above_threshold = []
-        for i, j in pairs:
-            if (all_atom_ranks[i] + all_atom_ranks[j]) > self.pair_threshold:
-                above_threshold.append((i, j))
-
-        return above_threshold
-
-    def filter_reaction_coordinates(
-            self, structure_list: List[db.Structure], coordinates: List[List[Tuple[int, int]]]
-    ) -> List[List[Tuple[int, int]]]:
-        all_atom_ranks = []  # Concatenated atom ranks in the order of the structures
-        for structure in structure_list:
-            neighbors = get_atom_pairs(structure, (1, 1), "None")
-            initial_ranks = self._rank_atoms(structure)
-            atom_ranks = [r for r in initial_ranks]
-            for i, j in neighbors:
-                atom_ranks[i] += initial_ranks[j]
-                atom_ranks[j] += initial_ranks[i]
-
-            all_atom_ranks += atom_ranks
-
-        above_threshold = []
-        for coord in coordinates:
-            if sum((all_atom_ranks[pair[0]] + all_atom_ranks[pair[1]]) for pair in coord) > self.coordinate_threshold:
-                above_threshold.append(coord)
+    Filters by atom counts. All given compounds must resolve to structures
+    that separately fall below the given threshold. No assumptions about atom
+    counts of possible combinations/products are made in this filter.
 
-        return above_threshold
+    Attributes
+    ----------
+    atom_type_count :: Dict[str,int]
+        A dictionary giving the number (values) of allowed occurrences of each
+        atom type (atom symbol string given as keys). Atom symbols not given
+        as keys are interpreted as forbidden.
+    """
+
+    def __init__(self, atom_type_count: Dict[str, int]):
+        super().__init__()
+        self.counts: Counter = Counter()
+        for k, v in atom_type_count.items():
+            self.counts.update({k.capitalize(): v})
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        # One compound case
+        if compound_two is None:
+            structure = db.Structure(compound_one.get_centroid())
+            return self._check_atom_counts(structure)
+        # Two compounds case
+        structure_one = db.Structure(compound_one.get_centroid())
+        structure_two = db.Structure(compound_two.get_centroid())
+        return self._check_atom_counts(structure_one) and self._check_atom_counts(structure_two)
+
+    def _check_atom_counts(self, structure: db.Structure) -> bool:
+        """
+        Checks the atom counts of the given structure against the requirements
+        set in the member variable.
+
+        Attributes
+        ----------
+        structure :: db.Structure
+            The structure of which to check the atom counts.
 
-    def _rank_atoms(self, structure: db.Structure):
+        Returns
+        -------
+        result :: bool
+            True if the structure passed the check/filter, False if not.
+        """
+        structure.link(self._structures)
         atoms = structure.get_atoms()
         elements = [str(x) for x in atoms.elements]
-        ranks = []
-        for e in elements:
-            if e == "H":
-                ranks.append(0)
-            elif e == "C":
-                ranks.append(1)
-            elif e in ["N", "O", "S", "P", "Si"]:
-                ranks.append(2)
-            else:
-                ranks.append(3)
-        return ranks
-
-
-class AtomRuleBasedFilter(ReactiveSiteFilter):
-    """
-    A filter that only classifies atoms as reactive if they correspond to a given rule.
-    The rules are given for each element. They may be a maximum required distance to another
-    atom/element or they may label an atom as generally reactive or not reactive. If not rules
-    are given for an element. All atoms of this type will be considered as non-reactive.\n
-    Example rules:
-    reactive_site_rules = {
-    'H': [ReactiveRuleFilterOrArray([('O', 3), ('N', 1)])],
-    'C': [ReactiveRuleFilterOrArray([('O', 2), ('N', 2)])],
-    'O': True,
-    'N': True
-    }
-    Allow reactions for all O and N, for all H that are at most in a distance of 3 bonds to O or one bond
-    to N, and for all C that are at most two bonds away from O or N.
-
-    Attributes
-    ----------
-    rules : dict
-        The dictionary containing the rules (vide supra).
-    """
-
-    def __init__(self, rules: dict):
-        super().__init__()
-        self._rules = rules
-
-    def filter_atoms(self, structure_list: List[db.Structure], atom_indices: List[int]) -> List[int]:
-        import ast
-        reactive_atom_indices = []
-        idx_shift = 0
-        for structure in structure_list:
-            atoms = structure.get_atoms()
-            elements = [str(x) for x in atoms.elements]
-            molecules = deserialize_molecules(structure)
-            idx_map = ast.literal_eval(structure.get_graph("masm_idx_map"))
-            for i, e in enumerate(elements):
-                # If no rule is specified, set the atom to be not reactive.
-                if e not in self._rules:
-                    continue
-                rule_set = self._rules[e]
-                # resolve lists of logical and/or arrays.
-                if isinstance(rule_set, List):
-                    for rule_array in rule_set:
-                        if rule_array.filter_by_rule(molecules, idx_map, elements, i):
-                            reactive_atom_indices.append(i + idx_shift)
-                            break
-                    continue
-                # Simple boolean rule, e.g., 'Si' : False
-                if rule_set:
-                    reactive_atom_indices.append(i + idx_shift)
-            idx_shift += structure.get_atoms().size()
-        return list(set(atom_indices) & set(reactive_atom_indices))
+        for k, v in Counter(elements).items():
+            if self.counts.get(k, 0) - v < 0:
+                return False
+        return True
+
+
+class ElementSumCountFilter(AggregateFilter):
+    """
+    Filters by atom counts. All given compounds must resolve to structures
+    that together fall below the given threshold.
+
+    Attributes
+    ----------
+    atom_type_count :: Dict[str,int]
+        A dictionary giving the number (values) of allowed occurrences of each
+        atom type (atom symbol string given as keys). Atom symbols not given
+        as keys are interpreted as forbidden.
+    """
 
-    class ReactiveRuleFilterAndArray:
+    def __init__(self, atom_type_count: Dict[str, int]):
+        super().__init__()
+        self.counts: Counter = Counter()
+        for k, v in atom_type_count.items():
+            self.counts.update({k.capitalize(): v})
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        # One compound case
+        if compound_two is None:
+            structure = db.Structure(compound_one.get_centroid())
+            counter_tot = self._get_element_counter(structure)
+        # Two compounds case
+        else:
+            structure_one = db.Structure(compound_one.get_centroid())
+            counter_one = self._get_element_counter(structure_one)
+
+            structure_two = db.Structure(compound_two.get_centroid())
+            counter_two = self._get_element_counter(structure_two)
+
+            counter_tot = counter_one + counter_two
+
+        for k, v in counter_tot.items():
+            if self.counts.get(k, 0) - v < 0:
+                return False
+
+        return True
+
+    def _get_element_counter(self, structure: db.Structure) -> Counter:
         """
-        An array of logically 'and' connected rules.
+        Gets the element counter of the given structure.
 
         Attributes
         ----------
-        primitive_rules : List[Tuple[str, int]]
-            A list of bond distance based rules that have all to be fulfilled.
-            Syntax example: ('O', 2) -> An oxygen atom has to be within two bonds distance of the current atom for it
-            to be allowed to react.
-        """
-
-        def __init__(self, primitive_rules: Optional[List[Tuple[str, int]]] = None):
-            if primitive_rules is None:
-                primitive_rules = []
-            self._primitive_rules = primitive_rules
-
-        def filter_by_rule(self, molecules: List[masm.Molecule], idx_map: List[Tuple[int, int]], elements: List[str],
-                           atom_index: int) -> bool:
-            mol_idx, i = idx_map[atom_index]
-            distances = masm.distance(i, molecules[mol_idx].graph)
-            for rule in self._primitive_rules:
-                max_distance = rule[1]
-                element_key = rule[0]
-                rule_fulfilled = False
-                for j, e in enumerate(elements):
-                    if e == element_key and distances[idx_map[j][1]] == max_distance:
-                        rule_fulfilled = True
-                        break
-                # All rules have to be fulfilled. Stop if one is not given.
-                if not rule_fulfilled:
-                    return False
-            return True
+        structure :: db.Structure
+            The structure of which to get the atom counter.
+
+        Returns
+        -------
+        result :: Counter
+            The Counter of the elements of the given structure.
+        """
+
+        structure.link(self._structures)
+        atoms = structure.get_atoms()
+        elements = [str(x) for x in atoms.elements]
+
+        return Counter(elements)
+
+
+class MolecularWeightFilter(AggregateFilter):
+    """
+    Filters by molecular weight. All given compounds must resolve to structures
+    that separately fall below the given threshold. No assumptions about weights
+    of possible combinations/products are made in this filter.
+
+    Attributes
+    ----------
+    max_weight :: float
+        The maximum weight to be allowed, given in unified atomic mass units (u).
+        For example, dinitrogen has a weight of about 28 u.
+    allow_additions_above_limit :: bool
+        If true only checks if the reactants are each above the given limit.
+        If false, assumes complete additions may happen and restricts all
+        combinations where the sum of weights is above the given limit.
+    """
 
-    class ReactiveRuleFilterOrArray:
+    def __init__(self, max_weight: float, allow_additions_above_limit: bool = True):
+        super().__init__()
+        self.max_weight = max_weight
+        self.allow_additions_above_limit = allow_additions_above_limit
+        self._weight_cache: Dict[str, float] = {}
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        cid_one = compound_one.get_id().string()
+        # One compound case
+        if compound_two is None:
+            weight = self._weight_cache.get(cid_one)
+            if weight is None:
+                structure = db.Structure(compound_one.get_centroid())
+                weight = self._calculate_weight(structure)
+                self._weight_cache = {cid_one: weight}
+            return weight < self.max_weight
+        # Two compounds case
+        cid_two = compound_two.get_id().string()
+        weight_one = self._weight_cache.get(cid_one)
+        if weight_one is None:
+            structure_one = db.Structure(compound_one.get_centroid())
+            weight_one = self._calculate_weight(structure_one)
+        weight_two = self._weight_cache.get(cid_two)
+        if weight_two is None:
+            structure_two = db.Structure(compound_two.get_centroid())
+            weight_two = self._calculate_weight(structure_two)
+        self._weight_cache = {
+            cid_one: weight_one,
+            cid_two: weight_two
+        }
+        if self.allow_additions_above_limit:
+            return weight_one < self.max_weight and weight_two < self.max_weight
+        else:
+            return (weight_one + weight_two) < self.max_weight
+
+    def _calculate_weight(self, structure: db.Structure) -> float:
         """
-        An array of logically 'or' connected rules.
+        Calculates the molecular weight, given a DB structure.
 
         Attributes
         ----------
-        primitive_rules : List[Tuple[str, int]]
-            A list of bond distance based rules of which at least one has to be fulfilled.
-            Syntax example: ('O', 2) -> An oxygen atom has to be at a distance of two bonds of the current atom for it
-            to be allowed to react.
-        """
-
-        def __init__(self, primitive_rules: Optional[List[Tuple[str, int]]] = None):
-            if primitive_rules is None:
-                primitive_rules = []
-            self._primitive_rules = primitive_rules
-
-        def filter_by_rule(self, molecules: List[masm.Molecule], idx_map: List[Tuple[int, int]], elements: List[str],
-                           atom_index: int) -> bool:
-            mol_idx, i = idx_map[atom_index]
-            distances = masm.distance(i, molecules[mol_idx].graph)
-            for rule in self._primitive_rules:
-                max_distance = rule[1]
-                element_key = rule[0]
-                for j, e in enumerate(elements):
-                    if e == element_key and distances[idx_map[j][1]] == max_distance:
-                        return True
-            return False
+        structure :: db.Structure
+            The structure of which to calculate the molecular weight.
 
-    class FunctionalGroupRule:
+        Returns
+        -------
+        weight :: float
+            The molecular weight in a.u. .
         """
-        A rule that encodes a distance criterion to a very general functional group. The functional group is
-        encoded in terms of a central atom type, a list of hetero atoms, the number of bonds to the central
-        atom and the number of hetero atoms bonded to the central atom.\n
-        carbonyle_group_d2 = FunctionalGroupRule(2, ['O'], 'C', 3, 1)
-        imine_group_d0 = FunctionalGroupRule(0, ['N'], 'C', 3, 1)
-        acetal_group_d1 =  FunctionalGroupRule(0, ['O'], 'C', 4, 2)
-        acetal_like_group_d1   =  FunctionalGroupRule(0, ['O, N'], 'C', 4, 2)
+        structure.link(self._structures)
+        atoms = structure.get_atoms()
+        weight = 0.0
+        for e in atoms.elements:
+            weight += utils.ElementInfo.mass(e)
+        return weight
+
+
+class IdFilter(AggregateFilter):
+    """
+    Filters by compound id. Returns true only for the specified compounds.
+    Used for testing purposes.
+
+    Attributes
+    ----------
+    reactive_ids :: List[str]
+        The IDs of the compounds to be considered as reactive.
+    """
+
+    def __init__(self, ids: List[str]):
+        super().__init__()
+        self.reactive_ids = set(ids)
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        # Get compound ids
+        compound_ids = set()
+        compound_ids.add(compound_one.get_id().string())
+        if compound_two is not None:
+            compound_ids.add(compound_two.get_id().string())
+        return compound_ids.issubset(self.reactive_ids)
+
+
+class SelfReactionFilter(AggregateFilter):
+    """
+    Filters out bimolecular reactions of compounds with themselves.
+    """
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        if compound_two is None:
+            # Do not rule out unimolecular reactions
+            return True
+        # Get compound ids
+        compound_one_id = compound_one.get_id().string()
+        compound_two_id = compound_two.get_id().string()
+        return compound_one_id != compound_two_id
+
+
+class TrueMinimumFilter(AggregateFilter):
+    """
+    Filters by checking if compound fulfills requirement to be considered a
+    true minimum. This includes having frequencies and all of them are above a
+    given threshold.
+    All given compounds must resolve to structures that separately only have
+    frequencies above the given threshold. Single atoms or ions are considered
+    as minima automatically.
+    Frequencies must be calculated with the ThermoGear during an exploration,
+    otherwise all compounds and combinations of them are filtered out.
+
+    Attributes
+    ----------
+    imaginary_frequency_threshold :: float
+        The frequency in atomic units above which a structure is considered a
+        minimum structure.
+        For example, a molecule with one imaginary frequency of -1e-4 (-138 cm^-1)
+        can be considered a minimum by setting the threshold to -1.1e-4 (-152 cm^-1)
+    """
+
+    def __init__(self, imaginary_frequency_threshold: float = 0.0):
+        super().__init__()
+        self.imaginary_frequency_threshold = imaginary_frequency_threshold
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        # One compound case
+        if compound_two is None:
+            structure = db.Structure(compound_one.get_centroid())
+            return self._frequency_check(structure)
+        # Two compounds case
+        structure_one = db.Structure(compound_one.get_centroid())
+        structure_two = db.Structure(compound_two.get_centroid())
+        # Frequency Check
+        freq_check_one = self._frequency_check(structure_one)
+        freq_check_two = self._frequency_check(structure_two)
+        return freq_check_one and freq_check_two
+
+    def _frequency_check(self, structure: db.Structure) -> bool:
+        """
+        Checks a structure for its validity as true minimum, meaning it has only
+        frequencies above a set threshold.
+        If no frequencies are available, it fails the check, unless it is a
+        single atom.
 
         Attributes
         ----------
-        distance : int
-            The bond distance to the functional group that must be matched.
-        hetero_atoms : List[str]
-            The list of atoms that are considered hetero atoms for this group.
-        central_atom : str
-            The central atom element symbol (default 'C')
-        n_bonds : int
-            The number of bonds to the central atom.
-        n_hetero_atoms : int
-            The number of hetero atoms that must bond to the central atom to constitute the group.
+        structure :: db.Structure
+            The structure of which the frequencies are checked.
 
+        Returns
+        -------
+        result :: bool
+            Boolean indicating if structure is true minimum.
         """
+        structure.link(self._structures)
+        # # # Check for single atom
+        if len(structure.get_atoms()) == 1:
+            return True
 
-        def __init__(self, distance: int, hetero_atoms: List[str], central_atom: str = 'C', n_bonds: int = 3,
-                     n_hetero_atoms: int = 1):
-            self._distance = distance
-            self._hetero_atoms = hetero_atoms
-            self._central_atom = central_atom
-            self._n_bonds = n_bonds
-            self._n_hetero_atoms = n_hetero_atoms
-
-        def filter_by_rule(self, molecules: List[masm.Molecule], idx_map: List[Tuple[int, int]], elements: List[str],
-                           atom_index: int) -> bool:
-            mol_idx, i = idx_map[atom_index]
-            distances_i = masm.distance(i, molecules[mol_idx].graph)
-            # Loop all C within the distance
-            for atom_j, e in enumerate(elements):
-                mol_jdx, j = idx_map[atom_j]
-                if e == self._central_atom and distances_i[j] == self._distance:
-                    distances_j = masm.distance(j, molecules[mol_jdx].graph)
-                    # For carbonyle or imine groups, there must be at least one hetero atom in distance of 1 to j and
-                    # exactly three atoms with distance of 1 to j
-                    n_close_to_j = 0
-                    n_hetero_atoms_found = 0
-                    for atom_k, e_k in enumerate(elements):
-                        _, k = idx_map[atom_k]
-                        if distances_j[k] == 1:
-                            n_close_to_j += 1
-                            if e_k in self._hetero_atoms:
-                                n_hetero_atoms_found += 1
-                            if n_close_to_j > self._n_bonds:
-                                break
-                    if n_hetero_atoms_found == self._n_hetero_atoms and n_close_to_j == self._n_bonds:
-                        return True
+        # # # Check, if frequencies exist; if not, the compound will not be
+        # # # considered for exploration
+        if not structure.has_property("frequencies"):
             return False
+        # # # Get Frequencies
+        freq_id = structure.get_property("frequencies")
+        freq = self._properties.get_vector_property(freq_id)
+        freq.link(self._properties)
+
+        # # # Check, if there is a frequency below the threshold
+        return not np.any(freq.get_data() < self.imaginary_frequency_threshold)
+
+
+class CatalystFilter(AggregateFilter):
+    """
+    Filters by defining an important structural motive.
+    A user defined set of atoms present in a structure identify it to be the, or
+    a version of the catalyst. This simple check should work great for common
+    transition metal catalysts.
+
+    Only specific reactions revolving around a catalytic cycle are then allowed:
+    i) reactions that feature the catalyst and one other compound that is not
+    the catalyst.
+    ii) reactions that only involve a single compound (not restricted to the
+    catalyst, unless specified otherwise with flag (see parameters))
+
+    Attributes
+    ----------
+    atom_type_count :: Dict[str,int]
+        A dictionary giving the number (values) of atoms that are expected to be
+        only present in - and thus defining - the catalyst. Atom type (atom
+        symbol strings) are given as keys. Atom symbols not given are considered
+        to be irrelevant to the check and may be present in the catalyst. In
+        order to ban atoms, set their count to zero.
+    restrict_unimolecular_to_catalyst :: bool
+        Whether unimolecular reactions should also be limited to the catalyst.
+    """
+
+    def __init__(self, atom_type_count: Dict[str, int], restrict_unimolecular_to_catalyst: bool = False):
+        super().__init__()
+        self.counts: Counter = Counter()
+        for k, v in atom_type_count.items():
+            self.counts.update({k.capitalize(): v})
+        self._restrict_unimolecular_to_catalyst = restrict_unimolecular_to_catalyst
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        # One compound case
+        if compound_two is None:
+            if self._restrict_unimolecular_to_catalyst:
+                return self._check_if_catalyst(db.Structure(compound_one.get_centroid()))
+            return True
+        # Two compounds case
+        structure_one = db.Structure(compound_one.get_centroid())
+        structure_two = db.Structure(compound_two.get_centroid())
+        return self._check_if_catalyst(structure_one) != self._check_if_catalyst(structure_two)
+
+    def _check_if_catalyst(self, structure: db.Structure) -> bool:
+        """
+        Check if the given structure is the or a version of the catalyst.
+
+        Attributes
+        ----------
+        structure :: db.Structure
+            The structure of which to check.
+
+        Returns
+        -------
+        check :: bool
+            True is the structure is a version of the catalyst.
+        """
+        structure.link(self._structures)
+        atoms = structure.get_atoms()
+        elements = [str(x) for x in atoms.elements]
+        actual = Counter(elements)
+        for k, v in self.counts.items():
+            if actual.get(k, 0) != v:
+                return False
+        return True
 
 
-class ElementWiseReactionCoordinateFilter(ReactiveSiteFilter):
+class AtomNumberFilter(AggregateFilter):
+    """
+    Filters out all compounds with a total number of atoms larger than the given
+    value. For multiple compounds the total number of atoms has to be equal or
+    smaller than the given value.
+
+    Attributes
+    ----------
+    max_n_atoms :: int
+        The maximum number of allowed atoms.
     """
-    A filter that can restrict the combination of atoms with a specific element.
-    The filter can be operated in two modes: Allow all reaction coordinates for the
-    element combinations encoded in the rules or forbid all of them.\n
-    Example rules:
-    reaction_coordinate_rules = {
-    'H': ['H', 'C']
-    }
-    In the default "forbid-mode" these rules mean that no reaction coordinates between two H-atoms and H and C are
-    allowed.
+
+    def __init__(self, max_n_atoms: int):
+        super().__init__()
+        self.max_n_atoms = max_n_atoms
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        structure_one = db.Structure(compound_one.get_centroid())
+        structure_one.link(self._structures)
+        n_atoms = len(structure_one.get_atoms())
+        if not (compound_two is None):
+            structure_two = db.Structure(compound_two.get_centroid())
+            structure_two.link(self._structures)
+            n_atoms += len(structure_two.get_atoms())
+        return n_atoms <= self.max_n_atoms
+
+
+class OneAggregateIdFilter(AggregateFilter):
+    """
+    Filters all compounds that are not present on a given "white list" of IDs.
+    In the case of multiple compounds, at least one has to be present in the
+    list. Note that this is identical to the IdFilter in the case of only one
+    compound.
 
     Attributes
     ----------
-    rules : dict
-        The dictionary containing the rules (vide supra).
-    reactive_if_rules_apply : bool
-        The mode to operate the filter in. If true, only reaction coordinates in the given rule set pass.
-        If false, no reaction coordinate in the given rule set pass. By default, false.
-    """
-
-    def __init__(self, rules: dict, reactive_if_rules_apply: bool = False):
-        super().__init__()
-        self._rules = rules
-        self._reactive_if_rules_apply = reactive_if_rules_apply
-
-    def filter_reaction_coordinates(
-            self, structure_list: List[db.Structure], coordinates: List[List[Tuple[int, int]]]
-    ) -> List[List[Tuple[int, int]]]:
-        all_element_symbols = []
-        for structure in structure_list:
-            atoms = structure.get_atoms()
-            elements = [str(x) for x in atoms.elements]
-            all_element_symbols += elements
-
-        valid_coordinates = []
-        for coord in coordinates:
-            skip = False
-            for pair in coord:
-                element_0 = all_element_symbols[pair[0]]
-                element_1 = all_element_symbols[pair[1]]
-                e_0_in_rule = False
-                e_1_in_rule = False
-                if element_0 in self._rules:
-                    e_0_in_rule = element_1 in self._rules[element_0]
-                if element_1 in self._rules:
-                    e_1_in_rule = element_0 in self._rules[element_1]
-                # If the rules are meant to exclude reaction coordinates, either e_0_in_rule or e_1_in_rule
-                # have to be true to skip the coordinate.
-                # If the rules are meant to include reaction coordinates, both of e_0_in_rule and e_1_in_rule have to
-                # be false to skip it.
-                if (not self._reactive_if_rules_apply and (e_0_in_rule or e_1_in_rule)) \
-                        or (self._reactive_if_rules_apply and not (e_0_in_rule or e_1_in_rule)):
-                    skip = True
-                    break
-            if not skip:
-                valid_coordinates.append(coord)
-        return valid_coordinates
+    reactive_ids :: List[str]
+        The IDs of the compounds to be considered as reactive.
+    """
+
+    def __init__(self, ids: List[str]):
+        super().__init__()
+        self.reactive_ids = set(ids)
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        if compound_one.get_id().string() in self.reactive_ids:
+            return True
+        if compound_two is not None:
+            if compound_two.get_id().string() in self.reactive_ids:
+                return True
+        return False
 
 
-class HeuristicPolarizationReactionCoordinateFilter(ReactiveSiteFilter):
+class SelectedAggregateIdFilter(AggregateFilter):
     """
-    A filter that assigns polarizations (+, -, or +-) to each atom. Reaction coordinates are only allowed
-    that combine + and - or +- with either + or -.
-    Example rules:
-    rules = {
-    'H': [PaulingElectronegativityRule(), FunctionalGroupRule("+", 2, ['N', 'O'], 'C', 3, 1)],
-    'C': [PaulingElectronegativityRule()],
-    'N': [PaulingElectronegativityRule()],
-    'O': [PaulingElectronegativityRule()]
-    }
+    Filters all compounds for which one needs to be one a given "white list"
+    of reactive compounds and the other has to be either on a list of
+    compounds of interest or on the list of reactive compounds.
 
     Attributes
     ----------
-    rules : dict
-        The dictionary containing the rules. The rule object must implement a function called string_from_rule(...).
+    reactive_ids :: List[str]
+        The IDs of the compounds to be considered as reactive.
+    selected_ids :: Optional[List[str]]
+        The IDs of the compounds to be of interest.
     """
 
-    def __init__(self, rules: dict):
+    def __init__(self, reactive_ids: List[str], selected_ids: Optional[List[str]] = None):
         super().__init__()
-        self._rules = rules
+        self.reactive_ids = set(reactive_ids)
+        if selected_ids is None:
+            selected_ids = []
+        self.selected_ids = set(selected_ids)
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        # One compound case: the id has to be a member of the reactive_ids.
+        # Two compound case: one of the ids has to be a member of the reactive_ids.
+        #                   The other one has to be either a member of the reactive_ids or the selected_ids.
+        one_is_reactive = compound_one.get_id().string() in self.reactive_ids
+        # One compound case
+        if compound_two is None:
+            return one_is_reactive
+        # Two compound case
+        two_is_reactive = compound_two.get_id().string() in self.reactive_ids
+        one_is_selected = compound_one.get_id().string() in self.selected_ids or one_is_reactive
+        two_is_selected = compound_two.get_id().string() in self.selected_ids or two_is_reactive
+        return (one_is_reactive and two_is_selected) or (two_is_reactive and one_is_selected)
+
+
+class ConcentrationPropertyFilter(AggregateFilter):
+    def __init__(self, property_labels: List[str], min_value: float, filter_only_pairs: bool, structures: db.Collection,
+                 properties: db.Collection):
+        """
+        Filters all compounds that have a concentration lower than a given value. For the two compound case,
+        the product of both concentrations has to be larger than this value. The filter may be set to only
+        filter for the two-compound case.
 
-    class PaulingElectronegativityRule:
+        Parameters
+        ----------
+        property_label :: str
+            The label for the concentration to filter with.
+        min_value :: float
+            The minimum concentration/concentration product.
+        filter_only_pairs :: bool
+            If true, the filter will always return True for the single compound case.
+        structures :: db.Collection
+            The structure collection.
+        properties :: db.Collection
+            The property collection.
         """
-        Polarization rule for the Pauli electronegativity scalar.
+        super().__init__()
+        self._property_labels = property_labels
+        self._min_value = min_value
+        self._properties = properties
+        self._structures = structures
+        self._filter_only_paris = filter_only_pairs
+        self._can_cache: bool = False
+        self._currently_caches: bool = False
 
-        Attributes
+    def _filter_impl(self, compound: db.Compound, optional_compound: Optional[db.Compound] = None) -> bool:
+        if self._filter_only_paris and optional_compound is None:
+            return True
+        concentration = self._get_concentration(compound)
+        if optional_compound is not None:
+            concentration *= self._get_concentration(optional_compound)
+        if concentration > self._min_value:
+            return True
+        return False
+
+    def _get_concentration(self, compound: db.Compound):
+        concentrations: List[float] = list()
+        for label in self._property_labels:
+            concentration = query_concentration_with_object(label, compound, self._properties, self._structures)
+            concentrations.append(concentration)
+        return max(concentrations)
+
+
+class ChargeCombinationFilter(AggregateFilter):
+    def __init__(self, structures: db.Collection):
+        """
+        Forbids the combination of compounds with the same sign, non-zero charge.
+
+        Parameters
         ----------
-        min_difference : dict
-            The minimum difference in electronegativities to assign a polarization.
+        structures :: db.Collection
+            The structure collection.
         """
+        super().__init__()
+        self._structures = structures
 
-        def __init__(self, min_difference: float = 0.4):
-            super().__init__()
-            self._min_difference = min_difference
-
-        def string_from_rule(self, molecules: List[masm.Molecule], idx_map: List[Tuple[int, int]], elements: List[str],
-                             atom_index: int) -> str:
-            """
-            Return '+' if the atom is electron poor, '-' if it is electron rich, some combination thereof if the
-            atom is neighbouring elements with significantly higher and lower electronegativity, and '' if it is
-            neighbouring neither.
-            """
-            from scine_utilities import ElementInfo
-            mol_idx, i = idx_map[atom_index]
-            distances_i = masm.distance(i, molecules[mol_idx].graph)
-            return_str = ''
-            for j, distance in enumerate(distances_i):
-                if distance == 1:
-                    atom_j = idx_map.index((mol_idx, j))
-                    element_i = ElementInfo.element_from_symbol(elements[atom_index])
-                    element_j = ElementInfo.element_from_symbol(elements[atom_j])
-                    electronegativity_i = ElementInfo.pauling_electronegativity(element_i)
-                    electronegativity_j = ElementInfo.pauling_electronegativity(element_j)
-                    difference = electronegativity_i - electronegativity_j
-                    if abs(difference) < self._min_difference:
-                        continue
-                    if difference <= 0.0:
-                        return_str += '+'
-                    else:
-                        # i > j
-                        return_str += '-'
-            return return_str
-
-    class FunctionalGroupRule:
-        """
-        Polarization rule for functional groups.
-        The functional group is encoded in terms of a central atom type, a
-        list of hetero atoms, the number of bonds to the central atom and the
-        number of hetero atoms bonded to the central atom.\n
-        carbonyle_group_d2 = FunctionalGroupRule('+' ,2, ['O'], 'C', 3, 1)
-        imine_group_d0 = FunctionalGroupRule('+' ,0, ['N'], 'C', 3, 1)
-        acetal_group_d1 =  FunctionalGroupRule('+', 0, ['O'], 'C', 4, 2)
-        acetal_like_group_d1   =  FunctionalGroupRule('+', 0, ['O, N'], 'C', 4, 2)
+    def _filter_impl(self, compound: db.Compound, optional_compound: Optional[db.Compound] = None) -> bool:
+        if optional_compound is None:
+            return True
+        charge_one = db.Structure(compound.get_centroid(), self._structures).charge
+        charge_two = db.Structure(optional_compound.get_centroid(), self._structures).charge
+        both_plus = charge_one > 0 and charge_two > 0
+        both_minus = charge_one < 0 and charge_two < 0
+        if both_minus or both_plus:
+            return False
+        return True
 
-        Attributes
+
+class LastKineticModelingFilter(AggregateFilter):
+    def __init__(self, manager: db.Manager, kinetic_modeling_job_order: Optional[str] = None,
+                 aggregate_settings_key: Optional[str] = None):
+        """
+        Allow only compounds that were handled in the last kinetic modeling calculation or have a non-zero start
+        concentration.
+
+        Parameters
         ----------
-        character : str
-            The polarization character (+ or -) to assign if the rule applies.
-        distance : int
-            The bond distance to the functional group that must be matched.
-        hetero_atoms : List[str]
-            The list of atoms that are considered hetero atoms for this group.
-        central_atom : str
-            The central atom element symbol (default 'C')
-        n_bonds : int
-            The number of bonds to the central atom.
-        n_hetero_atoms : int
-            The number of hetero atoms that must bond to the central atom to constitute the group.
-        """
-
-        def __init__(self, character: str, distance: int, hetero_atoms: List[str], central_atom: str = 'C',
-                     n_bonds: int = 3, n_hetero_atoms: int = 1):
-            self._character = character
-            self._rule = AtomRuleBasedFilter.FunctionalGroupRule(
-                distance, hetero_atoms, central_atom, n_bonds, n_hetero_atoms)
-
-        def string_from_rule(self, molecules: List[masm.Molecule], idx_map: List[Tuple[int, int]], elements: List[str],
-                             atom_index: int) -> str:
-            if self._rule.filter_by_rule(molecules, idx_map, elements, atom_index):
-                return self._character
-            else:
-                return ''
-
-    def filter_reaction_coordinates(
-            self, structure_list: List[db.Structure], coordinates: List[List[Tuple[int, int]]]
-    ) -> List[List[Tuple[int, int]]]:
-        all_polarization_characters = []
-        for structure in structure_list:
-            all_polarization_characters += self._get_characters_for_structure(structure)
-
-        valid_coordinates = []
-        for coord in coordinates:
-            skip = False
-            for pair in coord:
-                character_0 = all_polarization_characters[pair[0]]
-                character_1 = all_polarization_characters[pair[1]]
-                plus_minus = '+' in character_0 and '-' in character_1
-                minus_plus = '-' in character_0 and '+' in character_1
-                # All atom pairs must combine + and - signs.
-                if not (plus_minus or minus_plus):
-                    skip = True
+        manager : db.Manager
+            The database manager.
+        kinetic_modeling_job_order : Optional[str]
+            The kinetic modeling job order. By default, "kinetx_kinetic_modeling".
+        aggregate_settings_key : Optional[str]
+            The key to the aggregate ids in the kinetic modeling job. By default, "aggregate_ids".
+        """
+        super().__init__()
+        self._structures: db.Collection = manager.get_collection("structures")
+        self._compounds: db.Collection = manager.get_collection("compounds")
+        self._properties: db.Collection = manager.get_collection("properties")
+        self._calculations: db.Collection = manager.get_collection("calculations")
+        self._start_structure: Union[None, db.Structure] = None
+        if not kinetic_modeling_job_order:
+            kinetic_modeling_job_order = "kinetx_kinetic_modeling"
+        self._kinetic_modeling_job_order: str = kinetic_modeling_job_order
+        if not aggregate_settings_key:
+            aggregate_settings_key = "aggregate_ids"
+        self._aggregate_settings_key = aggregate_settings_key
+        self._n_calculations_last = 0
+        self._aggregate_str_ids_in_last_job: List[db.ID] = list()
+        self._can_cache: bool = False
+        self._currently_caches: bool = False
+
+    def _filter_impl(self, compound: db.Compound, optional_compound: Optional[db.Compound] = None) -> bool:
+        if not self._start_structure:
+            self._initialize_start_structure()
+        self._update_aggregate_ids_in_last_job()
+        if compound.id().string() not in self._aggregate_str_ids_in_last_job:
+            start_concentration = query_concentration_with_object(
+                "start_concentration", compound, self._properties, self._structures)
+            if start_concentration <= 0.0:
+                return False
+        if optional_compound:
+            if optional_compound.id().string() not in self._aggregate_str_ids_in_last_job:
+                start_concentration = query_concentration_with_object(
+                    "start_concentration", optional_compound, self._properties, self._structures)
+                if start_concentration <= 0.0:
+                    return False
+        return True
+
+    def _initialize_start_structure(self) -> None:
+        for compound in self._compounds.iterate_all_compounds():
+            compound.link(self._compounds)
+            c_start = query_concentration_with_object(
+                "start_concentration", compound, self._properties, self._structures)
+            if c_start > 0.0:
+                self._start_structure = db.Structure(compound.get_centroid(), self._structures)
+                break
+        if not self._start_structure:
+            raise RuntimeError("LastKineticModelingFilter: No compound with a non-zero starting concentration is"
+                               " given! This may prevent the exploration of further species and is not allowed.")
+
+    def _update_aggregate_ids_in_last_job(self) -> None:
+        assert self._start_structure
+        if self._start_structure.has_calculations(self._kinetic_modeling_job_order):
+            calc_ids = self._start_structure.get_calculations(self._kinetic_modeling_job_order)
+            if len(calc_ids) == self._n_calculations_last:
+                return
+            for i, calc_id in enumerate(reversed(calc_ids)):
+                calculation = db.Calculation(calc_id, self._calculations)
+                if calculation.get_status() == db.Status.COMPLETE:
+                    aggregate_str_ids = calculation.get_settings()[self._aggregate_settings_key]
+                    self._aggregate_str_ids_in_last_job = aggregate_str_ids  # type: ignore
+                    self._n_calculations_last = len(calc_ids) - i
                     break
-            if not skip:
-                valid_coordinates.append(coord)
-        return valid_coordinates
 
-    def _get_characters_for_structure(self, structure: db.Structure):
-        import ast
-        atoms = structure.get_atoms()
-        n_atoms = len(atoms)
-        elements = [str(x) for x in atoms.elements]
-        molecules = deserialize_molecules(structure)
-        idx_map = ast.literal_eval(structure.get_graph("masm_idx_map"))
-        string_list = ['' for _ in range(n_atoms)]
-        for atom_index in range(n_atoms):
-            for rule in self._rules[elements[atom_index]]:
-                string_list[atom_index] += rule.string_from_rule(molecules, idx_map, elements, atom_index)
-        return string_list
+
+class SelectedStructureIdFilter(SelectedAggregateIdFilter):
+    """
+    See SelectedAggregateIdFilter, but filters for compounds that include the given Structure IDs.
+    """
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        compound_one_structures = [str(sid) for sid in compound_one.get_structures()]
+        one_is_reactive = any(sid in self.reactive_ids for sid in compound_one_structures)
+        # One compound case
+        if compound_two is None:
+            return one_is_reactive
+        compound_two_structures = [str(sid) for sid in compound_two.get_structures()]
+        two_is_reactive = any(sid in self.reactive_ids for sid in compound_two_structures)
+        one_is_selected = any(sid in self.selected_ids for sid in compound_one_structures)
+        two_is_selected = any(sid in self.selected_ids for sid in compound_two_structures)
+        return (one_is_reactive and two_is_selected) or (two_is_reactive and one_is_selected)
+
+
+class CompoundCostPropertyFilter(AggregateFilter):
+    """
+    Filters by compound cost. Any given compound must have a compound cost
+    below the given threshold.
+    For any pair of compounds, the sum of their compound costs must be below
+    the threshold as well.
+
+    Attributes
+    ----------
+    max_compound_cost : float
+            The threshold for the allowed overall compound costs of one or the
+            sum of two compounds.
+
+    Notes
+    -----
+    Always the last compound cost entry is considered.
+    If a compound has no compound cost assigned, it is considered to have a
+    compound cost of 1e12. This corresponds to +inf in the Pathfinder logic.
+    """
+
+    def __init__(self, max_compound_cost: float):
+        super().__init__()
+        self._max_compound_cost = max_compound_cost
+
+    def _filter_impl(self, compound_one: db.Compound, compound_two: Optional[db.Compound] = None) -> bool:
+        cc_one = self._get_compound_cost(compound_one)
+        # Unimolecular case
+        if compound_two is None and cc_one < self._max_compound_cost:
+            return True
+        # Bimolecular case
+        if compound_two is not None:
+            cc_two = self._get_compound_cost(compound_two)
+            if cc_one + cc_two < self._max_compound_cost:
+                return True
+        return False
+
+    def _get_compound_cost(self, compound: db.Compound):
+        centroid = db.Structure(compound.get_centroid(), self._structures)
+        property_list = centroid.get_properties("compound_cost")
+        # Return +inf for compound cost has no compound_cost yet
+        if len(property_list) < 1:
+            return 1e12
+        # # # Pick last entry of list
+        prop = db.NumberProperty(property_list[-1], self._properties)
+        return prop.get_data()
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/kinetic_modeling/kinetic_modeling.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/kinetic_modeling/kinetic_modeling.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,42 +32,43 @@
         The options for the KineticModeling gear.
 
     Notes
     -----
     The kinetic modeling can be run in a sleepy mode. In this mode, kinetic modeling jobs are only set up
     if all other jobs are terminated (not new, hold, or pending).
     """
-    class Options:
+    class Options(Gear.Options):
         """
         The options for the KineticModeling Gear.
         """
 
         __slots__ = (
             "cycle_time",
-            "model",
             "elementary_step_interval",
             "energy_label",
             "job",
             "time_step",
             "solver",
             "batch_interval",
             "n_batches",
             "convergence",
             "sleeper_mode",
             "ts_energy_threshold_deduplication",
             "rate_from_lowest_conformer",
             "use_spline_barrier",
             "max_barrier",
             "min_barrier_intermolecular",
-            "instant_barrierless",
             "min_barrier_intramolecular",
-            "only_active_aggregates"
+            "min_flux_truncation",
+            "diffusion_controlled_barrierless",
+            "use_max_flux_for_truncation"
         )
 
         def __init__(self):
+            super().__init__()
             self.cycle_time = 30
             """
             int
                 The minimum number of seconds between two cycles of the Gear.
                 Cycles are finished independent of this option, thus if a cycle
                 takes longer than the cycle_time will effectively lead to longer
                 cycle times and not cause multiple cycles of the same Gear.
@@ -80,19 +81,14 @@
             self.elementary_step_interval = 100
             """
             int
                 Set up a kinetic modeling job if at least this number of new
                 elementary steps were added to the network and are eligible according
                 to reaction-barrier cut-off, and electronic structure model.
             """
-            self.model = db.Model("PM6", "", "")
-            """
-            db.Model
-                The electronic structure model to be used for the reaction rate determination.
-            """
             self.energy_label = "electronic_energy"
             """
             str
                 The property lable to be used as the energy for the reaction rate determination.
             """
             self.time_step = 1e-8
             """
@@ -157,36 +153,50 @@
                 The minimum allowed barrier in kJ/mol for intermolecular reactions.
             """
             self.min_barrier_intramolecular = 0.0
             """
             float
                 The minimum allowed barrier in kJ/mol for intramolecular reactions.
             """
-            self.only_active_aggregates = True
+            self.min_flux_truncation = 1e-9
+            """
+            float
+                Minimum flux of all aggregates in a reaction in a previous kinetic modeling job. If the flux is lower
+                than this threshold, the reaction is excluded from the kinetic modeling.
+            """
+            self.diffusion_controlled_barrierless = True
             """
             bool
-                If true, reactions are only included in the kinetic modeling if the lhs or rhs consists purely of
-                aggregates that are considered explorable.
+                If true, all barrierless reactions are assigned the maximum rate according to the
+                min_barrier_intramolecular and min_barrier_intermolecular settings.
+            """
+            self.use_max_flux_for_truncation = False
+            """
+            bool
+                If true, the maximum entry of all concentration fluxes for a given reaction is used for the flux based
+                truncation.
             """
 
     def __init__(self):
         super().__init__()
-        self.options = self.Options()
-        self._required_collections = ["calculations", "elementary_steps", "properties", "reactions", "structures"]
+        self._required_collections = ["calculations", "elementary_steps", "properties", "reactions", "structures",
+                                      "flasks", "compounds"]
         self._n_reactions_started_last = 0
 
     def _loop_impl(self):
         # Allow only one kinetic modeling calculation to be queuing at a time
         n_already_set_up = self._get_n_queuing_kinetic_modeling_calculations()
         if n_already_set_up > 0:
             return
         # Run the kinetic modeling if all other calculations are done, independent on the elementary-step interval.
         n_calc_still_waiting = self._get_n_queuing_calculations()
         if self.options.sleeper_mode and n_calc_still_waiting > 0:
             return
+        if self.options.sleeper_mode and not self._reaction_gear_finished():
+            return
         n_qualified_reactions = 0
         if n_calc_still_waiting > 0 and not self.options.sleeper_mode:
             n_qualified_reactions = self._get_n_qualified_reactions()
 
         if (n_qualified_reactions - self._n_reactions_started_last) // self.options.elementary_step_interval > 0:
             self._set_up_job(n_qualified_reactions)
         elif n_calc_still_waiting == 0:
@@ -210,14 +220,20 @@
         selection = {
             "$and": [
                 {"$or": [{"status": "new"}, {"status": "hold"}, {"status": "pending"}]},
             ]
         }
         return self._calculations.count(dumps(selection))
 
+    def _reaction_gear_finished(self) -> bool:
+        selection = {
+            "reaction": ""
+        }
+        return self._elementary_steps.count(dumps(selection)) == 0
+
     def _get_n_qualified_reactions(self):
         n_qualified_reactions = 0
         for reaction in stop_on_timeout(self._reactions.iterate_reactions(dumps({}))):
             reaction.link(self._reactions)
             elementary_steps = reaction.get_elementary_steps()
             for elementary_step_id in elementary_steps:
                 elementary_step = db.ElementaryStep(elementary_step_id, self._elementary_steps)
@@ -229,23 +245,27 @@
                 if lhs is None or rhs is None:
                     continue
                 else:
                     n_qualified_reactions += 1
         return n_qualified_reactions
 
     def _set_up_job(self, n_qualified_reactions: int):
+        if self.stop_at_next_break_point:
+            return
         self._n_reactions_started_last = n_qualified_reactions
         job_factory = KineticModelingJobFactory(deepcopy(self.options.model), self._manager,
                                                 self.options.energy_label, self.options.job,
                                                 self.options.ts_energy_threshold_deduplication,
                                                 self.options.rate_from_lowest_conformer,
                                                 self.options.use_spline_barrier, self.options.max_barrier,
                                                 self.options.min_barrier_intermolecular,
                                                 self.options.min_barrier_intramolecular,
-                                                self.options.only_active_aggregates)
+                                                self.options.min_flux_truncation, "",
+                                                self.options.diffusion_controlled_barrierless,
+                                                self.options.use_max_flux_for_truncation)
         settings = utils.ValueCollection({})
         settings["time_step"] = self.options.time_step
         settings["solver"] = self.options.solver
         settings["batch_interval"] = self.options.batch_interval
         settings["n_batches"] = self.options.n_batches
         settings["energy_label"] = self.options.energy_label
         settings["convergence"] = self.options.convergence
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/kinetic_modeling/prepare_kinetic_modeling_job.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/reaction.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,381 +3,354 @@
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
 from json import dumps
-from typing import Tuple, Union, List, Optional, Dict, Set
+from typing import List, Union, Optional, Tuple
+from warnings import warn
+import numpy as np
+from copy import copy
 
 # Third party imports
 import scine_database as db
 import scine_utilities as utils
 
-from ...utilities.queries import (
-    stop_on_timeout,
-    model_query
-)
-from .concentration_query_functions import query_concentration_with_object
-from ...utilities.energy_query_functions import get_barriers_for_elementary_step_by_type, get_energy_for_structure,\
-    rate_constant_from_barrier
-from ...utilities.compound_and_flask_creation import get_compound_or_flask, get_aggregate_type
+# Local application imports
+from . import Gear
+from ..utilities.queries import stop_on_timeout
+from ..utilities.energy_query_functions import get_energy_for_structure
+from ..utilities.compound_and_flask_creation import get_compound_or_flask
 
 
-class KineticModelingJobFactory:
+class BasicReactionHousekeeping(Gear):
     """
-    This class sets up kinetic modeling jobs.
+    This Gear updates all Elementary Steps stored in the database such that they
+    are added to an existing Reaction or that a new Reaction is created if the
+    Step does not fit an existing one.
 
     Attributes
     ----------
-    model : db.Model
-        The electronic structure model used for the reaction rates.
-    manager : db.Manager
-        The database manager.
-    energy_label : str
-        The property label to be used for the reaction rate determination.
-    job : db.Job
-        The job to set up.
-    ts_energy_threshold_deduplication : float
-        If two reactions are mirrors/inverses of one another all elementary steps with the same transition state
-        energy are eliminated. This threshold determines the energy tolerance for the elimination.
-    rate_from_lowest_conformer : bool
-        Calculate the reaction rate always with respect to the energy of the
-        lowest energy conformer without any reweighing.
-    use_spline_barrier : bool
-        If true, the reaction barrier from the spline is used.
-    max_barrier : float
-        The maximum allowed barrier.
-    min_barrier_intermolecular : float
-        The minimum allowed barrier in kJ/mol for intermolecular reactions.
-    min_barrier_intramolecular : float
-        The minimum allowed barrier in kJ/mol for intramolecular reactions.
-    only_active_aggregates : bool
-        If true, reactions are only included in the kinetic modeling if the lhs or rhs consists purely of
-        aggregates that are considered explorable.
-    _structure_weights : dict
-        The Boltzmann populations for each structure of each compound.
-        Constructed on the fly when create_kinetic_modeling_job is called.
+    options :: BasicReactionHousekeeping.Options
+        The options for the BasicReactionHousekeeping Gear.
+
+    Notes
+    -----
+    Checks for all Elementary Steps without a 'reaction'.
     """
 
-    def __init__(self, model: db.Model, manager: db.Manager, energy_label: str, job: db.Job,
-                 ts_energy_threshold_deduplication, rate_from_lowest_conformer, use_spline_barrier,
-                 max_barrier, min_barrier_intermolecular, min_barrier_intramolecular,
-                 only_active_aggregates):
-        self._model = model
-        self._kinetic_modeling_job = job
-        self._properties = manager.get_collection("properties")
-        self._elementary_steps = manager.get_collection("elementary_steps")
-        self._compounds = manager.get_collection("compounds")
-        self._reactions = manager.get_collection("reactions")
-        self._structures = manager.get_collection("structures")
-        self._calculations = manager.get_collection("calculations")
-        self._flasks = manager.get_collection("flasks")
-        self._energy_label = energy_label
-        self._structure_weights: Dict[str, Dict[str, float]] = dict()
-        self._ts_energy_threshold_deduplication = ts_energy_threshold_deduplication
-        self._rate_from_lowest_conformer = rate_from_lowest_conformer
-        self._use_spline_barrier = use_spline_barrier
-        self._min_rate_constant = rate_constant_from_barrier(max_barrier, float(model.temperature))
-        self._max_rate_constant_inter = rate_constant_from_barrier(min_barrier_intermolecular, float(model.temperature))
-        self._max_rate_constant_intra = rate_constant_from_barrier(min_barrier_intramolecular, float(model.temperature))
-        self._only_active_aggregates = only_active_aggregates
-        self._min_flux_truncation = 1e-6
+    def __init__(self):
+        super().__init__()
+        self.options = self.Options()
+        self._required_collections = ["compounds", "elementary_steps", "flasks", "reactions", "properties",
+                                      "structures"]
+        self._reaction_cache: Optional[dict] = None
 
-    def create_kinetic_modeling_job(self, settings: utils.ValueCollection) -> bool:
+    class Options(Gear.Options):
         """
-        Create the kinetic modeling job.
-
-        Parameters
-        ----------
-        settings : utils.ValueCollection
-            The job settings.
-
-        Return
-        ------
-        bool
-            True if the calculation was set up. False, otherwise.
+        The options for the BasicReactionHousekeeping Gear.
         """
-        a_id_list, a_type_list, lhs_rates_per_reaction, rhs_rates_per_reaction, reaction_ids = self._collect_all_data()
-        all_structure_ids = [db.ID(s_id_str) for c_id_str in self._structure_weights for s_id_str in
-                             self._structure_weights[c_id_str]]
-        concentrations = self._get_starting_concentrations(a_id_list, a_type_list)
-        if sum(concentrations) == 0.0:
-            print("No starting concentrations are available!")
-            return False
-        # Sum up the ordinary differential equations.
-        lhs_rates = [sum(rates) for rates in lhs_rates_per_reaction]
-        rhs_rates = [sum(rates) for rates in rhs_rates_per_reaction]
-        settings["lhs_rates"] = lhs_rates
-        settings["rhs_rates"] = rhs_rates
-        settings["start_concentrations"] = concentrations
-        settings["reaction_ids"] = [r_id.string() for r_id in reaction_ids]
-        settings["aggregate_ids"] = [c_id.string() for c_id in a_id_list]
-        settings["aggregate_types"] = a_type_list  # type: ignore
-        settings["energy_model_program"] = self._model.program
-        self._model.program = "any"
-        if self._calc_already_set_up(all_structure_ids, settings):
-            return False
-        calc = db.Calculation(db.ID())
-        calc.link(self._calculations)
-        calc.create(self._model, self._kinetic_modeling_job, [])
-        calc.set_settings(settings)
-        calc.set_structures(all_structure_ids)
-        calc.set_status(db.Status.NEW)
-        return True
-
-    def _calc_already_set_up(self, structure_ids: List[db.ID], settings: utils.ValueCollection) -> bool:
-        # This query is terribly slow. But it should only be rarely necessary to do it.
-        structures_string_ids = [{"$oid": str(s_id)} for s_id in structure_ids]
-        selection = {
-            "$and": [
-                {"job.order": {"$eq": self._kinetic_modeling_job.order}},
-                {"structures": {"$all": structures_string_ids, "$size": len(structures_string_ids)}},
-                {"settings.solver": settings["solver"]},
-            ]
-            + model_query(self._model)  # type: ignore
-        }
-        # (direct setting comparison in query is dependent on order in dict and string-double comparison has problems)
-        for calculation in stop_on_timeout(iter(self._calculations.query_calculations(dumps(selection)))):
-            calculation.link(self._calculations)
-            if calculation.get_settings() == settings:
-                return True
-        return False
 
-    def _get_structure_weights(self, aggregate_id: db.ID, aggregate_type: db.CompoundOrFlask) -> dict:
-        string_id = aggregate_id.string()
-        if string_id not in self._structure_weights:
-            self._structure_weights[string_id] = self._calculate_structure_weights(aggregate_id, aggregate_type)
-        return self._structure_weights[string_id]
-
-    def _calculate_structure_weights(self, aggregate_id: db.ID, aggregate_type: db.CompoundOrFlask) -> dict:
-        import math
-        temperature = float(self._model.temperature)
-        beta_per_hartree = 1.0 / (utils.BOLTZMANN_CONSTANT * utils.HARTREE_PER_JOULE * temperature)
-        aggregate = get_compound_or_flask(aggregate_id, aggregate_type, self._compounds, self._flasks)
-        structures_ids = aggregate.get_structures()
-        weight_dict = dict()
-        total_weight = 0.0
-        energies: List[Optional[float]] = []
-        reference_energy = 0.0
-        for s_id in structures_ids:
-            structure = db.Structure(s_id, self._structures)
-            structure_properties = structure.query_properties(self._energy_label, self._model, self._properties)
-            if not structure_properties:
-                energies.append(None)
+        __slots__ = ("cycle_time",
+                     "use_structure_deduplication",
+                     "use_energy_deduplication",
+                     "use_rmsd_deduplication",
+                     "energy_tolerance",
+                     "rmsd_tolerance")
+
+        def __init__(self):
+            super().__init__()
+            self.cycle_time = 10
+            """
+            int
+                The minimum number of seconds between two cycles of the Gear.
+                Cycles are finished independent of this option, thus if a cycle
+                takes longer than the cycle_time will effectively lead to longer
+                cycle times and not cause multiple cycles of the same Gear.
+            """
+            self.use_structure_deduplication = True
+            """
+            bool
+                If true duplicated elementary steps are not sorted into reactions.
+                The criterion is that all structures on the lhs of the elementary step
+                have to be identical. This criterion can be combined with other selection criteria.
+                Steps are only eliminated if all selection criteria signal identical steps.
+            """
+            self.use_energy_deduplication = True
+            """
+            bool
+                If true duplicated elementary steps are not sorted into reactions.
+                The criterion is that the total electronic energy of the transition state
+                (if available) has to be within the threshold limits of `energy_tolerance`.
+                This criterion can be combined with other selection criteria. Steps are only eliminated
+                if all selection criteria signal identical steps.
+            """
+            self.use_rmsd_deduplication = True
+            """
+            bool
+                If true duplicated elementary steps are not sorted into reactions.
+                The criterion is that the RMSD of the transition state coordinates
+                (if available) have to be within the threshold limits of `rmsd_tolerance`.
+                This criterion can be combined with other selection criteria. Steps are only eliminated
+                if all selection criteria signal identical steps. Note that this deduplication
+                strategy may fail to eliminate elementary steps if the atom ordering the transition
+                state differs.
+            """
+            self.energy_tolerance = 1e-5
+            """
+            float
+                The energy tolerance for the transition state energy deduplication.
+            """
+            self.rmsd_tolerance = 1e-3
+            """
+            float
+                The RMSD tolerance for the transition state RMSD deduplication.
+            """
+
+    def _loop_impl(self):
+        # Setup query for elementary steps without reactions
+        selection = {"$and": [
+            {"reaction": ""},
+            {"analysis_disabled": {"$ne": True}}
+        ]}
+        uses_elementary_step_deduplication =\
+            self.options.use_structure_deduplication or self.options.use_energy_deduplication or \
+            self.options.use_rmsd_deduplication
+        # Loop over all results
+        for step in stop_on_timeout(self._elementary_steps.iterate_elementary_steps(dumps(selection))):
+            step.link(self._elementary_steps)
+            reactants = step.get_reactants(db.Side.BOTH)
+            if self.stop_at_next_break_point:
+                return
+
+            # Determine structure types
+            types = [[], []]
+            aggregates = [[], []]
+            all_structures_have_aggregates = True
+            for i, side in enumerate(reactants):
+                if not all_structures_have_aggregates:
+                    # we are breaking here to avoid rhs evaluation if lhs is already incomplete
+                    break
+                for structure_id in side:
+                    structure = db.Structure(structure_id, self._structures)
+                    # check aggregate
+                    if not structure.has_aggregate():
+                        all_structures_have_aggregates = False
+                        break
+                    else:
+                        aggregates[i].append(structure.get_aggregate())
+                    # check label
+                    label = structure.get_label()
+                    if label in [db.Label.MINIMUM_OPTIMIZED, db.Label.USER_OPTIMIZED, db.Label.DUPLICATE]:
+                        types[i].append(db.CompoundOrFlask.COMPOUND)
+                    elif label == db.Label.COMPLEX_OPTIMIZED:
+                        types[i].append(db.CompoundOrFlask.FLASK)
+                    else:
+                        raise RuntimeError(f"Structure label '{str(label)}' is not supported for aggregation.")
+            if not all_structures_have_aggregates:
                 continue
-            prop = db.NumberProperty(structure_properties[-1], self._properties)
-            energy = prop.get_data()
-            energies.append(energy)
-            if energy < reference_energy:
-                reference_energy = energy
-        for i, opt_energy in enumerate(energies):
-            if opt_energy is None:
+
+            self._replace_duplicate_structures(step)
+            # Check for a reactions with the same structures/compounds
+            true_hit, is_parallel = self._check_cached_reactions(aggregates[0], aggregates[1])
+            if true_hit is not None:
+                if not is_parallel:
+                    self._invert_elementary_step(step)
+                # Add elementary step to reaction if it is not duplicated.
+                if uses_elementary_step_deduplication and self._is_duplicate(step, true_hit):
+                    step.disable_analysis()
+                    step.disable_exploration()
+                reaction = true_hit
+                # check for regular vs barrierless
+                self._disable_barrierless_if_mixed_types_in_reaction(reaction, step)
+                reaction.add_elementary_step(step.id())
+                step.set_reaction(reaction.id())
                 continue
-            s_id = structures_ids[i]
-            weight = math.exp(- beta_per_hartree * (opt_energy - reference_energy))
-            weight_dict[s_id.string()] = weight
-            total_weight += weight
-        if not self._rate_from_lowest_conformer:
-            for key in weight_dict:
-                weight_dict[key] /= total_weight
-        return weight_dict
-
-    def _collect_all_data(self) -> Tuple[List[db.ID], List[db.CompoundOrFlask], List[List[float]], List[List[float]],
-                                         List[db.ID]]:
-        old_zero_flux_reaction_ids = self._get_old_zero_flux_reactions()
-        lhs_rates_per_reaction = []
-        rhs_rates_per_reaction = []
-        c_id_list = list()
-        c_type_list = list()
-        # Search for duplicated reactions and eliminate all non-unique transition states.
-        reaction_step_tuples = list()
-        # exclude reactions that were unimportant previously.
-        rxn_string_ids = [{"$oid": str(r_id)} for r_id in old_zero_flux_reaction_ids]
-        selection = {
-            "_id": {"$nin": rxn_string_ids}
-        }
-        for reaction in self._reactions.iterate_reactions(dumps(selection)):
+            # Generate new reaction
+            reaction = db.Reaction(db.ID(), self._reactions)
+            reaction.create(aggregates[0], aggregates[1], types[0], types[1])
+            reaction.add_elementary_step(step.id())
+            step.set_reaction(reaction.id())
+            self._add_reaction_to_aggregate(aggregates[0] + aggregates[1], types[0] + types[1], reaction.id())
+            self._add_to_cache(reaction, aggregates[0], aggregates[1])
+
+    def _check_cached_reactions(
+            self, lhs_aggregates: List[db.ID], rhs_aggregates: List[db.ID]
+    ) -> Tuple[Optional[db.Reaction], bool]:
+        self._rebuild_cache()
+        assert self._reaction_cache is not None
+        key = ','.join(sorted([x.string() for x in lhs_aggregates]))
+        key += '<->'
+        key += ','.join(sorted([x.string() for x in rhs_aggregates]))
+        if key in self._reaction_cache:
+            reaction = db.Reaction(db.ID(self._reaction_cache[key]))
             reaction.link(self._reactions)
-            # check if the lhs or rhs side of the reaction consists purely of explorable compounds
-            reactant_ids = reaction.get_reactants(db.Side.BOTH)
-            reactant_types = reaction.get_reactant_types(db.Side.BOTH)
-            # collect the elementary steps.
-            elementary_steps = reaction.get_elementary_steps()
-            lhs_rates_per_elementary_step = []
-            rhs_rates_per_elementary_step = []
-            qualified_elementary_steps = []
-            for elementary_step_id in elementary_steps:
-                elementary_step = db.ElementaryStep(elementary_step_id, self._elementary_steps)
-                if not elementary_step.analyze():
-                    continue
-                lhs_rate, rhs_rate = self._get_reaction_rates_according_to_model(self._model, elementary_step_id,
-                                                                                 reaction)
-                if lhs_rate is None or rhs_rate is None:
-                    continue
-                lhs_rates_per_elementary_step.append(lhs_rate)
-                rhs_rates_per_elementary_step.append(rhs_rate)
-                qualified_elementary_steps.append(elementary_step.id())
-
-            n_elementary_steps = len(qualified_elementary_steps)
-            # Stop if no elementary steps qualify.
-            if n_elementary_steps < 1:
-                continue
+            return reaction, True
+        key = ','.join(sorted([x.string() for x in rhs_aggregates]))
+        key += '<->'
+        key += ','.join(sorted([x.string() for x in lhs_aggregates]))
+        if key in self._reaction_cache:
+            reaction = db.Reaction(db.ID(self._reaction_cache[key]))
+            reaction.link(self._reactions)
+            return reaction, False
+        return None, True
 
-            all_ids = reactant_ids[0] + reactant_ids[1]
-            all_types = reactant_types[0] + reactant_types[1]
-            for o_id, o_type in zip(all_ids, all_types):
-                if o_id not in c_id_list:
-                    c_id_list.append(o_id)
-                    c_type_list.append(o_type)
-
-            # Weight the elementary step according to the Boltzmann populations of their structures.
-            lhs_new_rate_constants = list()
-            rhs_new_rate_constants = list()
-            new_qualified_steps = list()
-            for i, elementary_step_id in enumerate(qualified_elementary_steps):
-                step = db.ElementaryStep(elementary_step_id, self._elementary_steps)
-                # Barrier-less reactions will always be assigned the dummy diffusion rate constant.
-                if step.get_type == db.ElementaryStepType.BARRIERLESS:
-                    lhs_rate_constant = self._max_rate_constant_inter
-                    rhs_rate_constant = self._max_rate_constant_inter
-                else:
-                    lhs_weight, rhs_weight = self._get_structure_weights_for_elementary_step(elementary_step_id)
-                    assert lhs_weight <= 1.0
-                    assert rhs_weight <= 1.0
-                    lhs_rate_constant = lhs_rates_per_elementary_step[i] * lhs_weight
-                    rhs_rate_constant = rhs_rates_per_elementary_step[i] * rhs_weight
-                    if lhs_rate_constant < self._min_rate_constant and rhs_rate_constant < self._min_rate_constant:
-                        continue
-                    reactant_types = reaction.get_reactant_types(db.Side.BOTH)
-                    lhs_is_intra_molecular = len(reactant_types[0]) == 1
-                    rhs_is_intra_molecular = len(reactant_types[1]) == 1
-                    lhs_rate_constant = min(self._max_rate_constant_intra, lhs_rate_constant)\
-                        if lhs_is_intra_molecular else min(self._max_rate_constant_inter, lhs_rate_constant)
-                    rhs_rate_constant = min(self._max_rate_constant_intra, rhs_rate_constant)\
-                        if rhs_is_intra_molecular else min(self._max_rate_constant_inter, rhs_rate_constant)
-                lhs_new_rate_constants.append(lhs_rate_constant)
-                rhs_new_rate_constants.append(rhs_rate_constant)
-                new_qualified_steps.append(elementary_step_id)
-            if len(lhs_new_rate_constants) < 1:
-                continue
-            lhs_rates_per_reaction.append(lhs_new_rate_constants)
-            rhs_rates_per_reaction.append(rhs_new_rate_constants)
-            reaction_step_tuples.append(tuple((reaction, new_qualified_steps)))
-        reaction_ids = [reaction.id() for reaction, _ in reaction_step_tuples]
-        assert len(lhs_rates_per_reaction) == len(rhs_rates_per_reaction)
-        assert len(reaction_ids) == len(rhs_rates_per_reaction)
-        return c_id_list, c_type_list, lhs_rates_per_reaction, rhs_rates_per_reaction, reaction_ids
-
-    def _get_starting_concentrations(self, aggregate_ids: List[db.ID], aggregate_types: List[db.CompoundOrFlask])\
-            -> List[float]:
-        concentrations = []
-        for o_id, o_type in zip(aggregate_ids, aggregate_types):
-            aggregate = get_compound_or_flask(o_id, o_type, self._compounds, self._flasks)
-            start_concentration = query_concentration_with_object("start_concentration", aggregate, self._properties,
-                                                                  self._structures)
-            concentrations.append(start_concentration)
-        return concentrations
-
-    def _get_structure_weights_for_elementary_step(self, elementary_step_id: db.ID) -> Tuple[float, float]:
-        elementary_step = db.ElementaryStep(elementary_step_id, self._elementary_steps)
-        structure_ids = elementary_step.get_reactants(db.Side.BOTH)
-        lhs_weight = 1.0
-        for s_id in structure_ids[0]:
+    def _rebuild_cache(self) -> None:
+        if self._reaction_cache is None:
+            self._reaction_cache = {}
+            for r in self._reactions.iterate_reactions('{}'):
+                r.link(self._reactions)
+                reactants = r.get_reactants(db.Side.BOTH)
+                key = ','.join(sorted([x.string() for x in reactants[0]]))
+                key += '<->'
+                key += ','.join(sorted([x.string() for x in reactants[1]]))
+                self._reaction_cache[key] = r.get_id().string()
+
+    def _add_to_cache(
+        self, reaction: db.Reaction, lhs_aggregates: List[db.ID], rhs_aggregates: List[db.ID]
+    ) -> None:
+        assert self._reaction_cache is not None
+        key = ','.join(sorted([x.string() for x in lhs_aggregates]))
+        key += '<->'
+        key += ','.join(sorted([x.string() for x in rhs_aggregates]))
+        assert key not in self._reaction_cache
+        self._reaction_cache[key] = reaction.get_id().string()
+
+    def _replace_duplicate_structures(self, elementary_step: db.ElementaryStep):
+        reactants = elementary_step.get_reactants(db.Side.BOTH)
+        unique_lhs = self._make_unique_structure_id_list(reactants[0])
+        unique_rhs = self._make_unique_structure_id_list(reactants[1])
+        elementary_step.set_reactants(unique_lhs, db.Side.LHS)
+        elementary_step.set_reactants(unique_rhs, db.Side.RHS)
+
+    def _make_unique_structure_id_list(self, id_list):
+        unique_list: List[db.ID] = list()
+        for s_id in id_list:
             structure = db.Structure(s_id, self._structures)
-            aggregate_type = get_aggregate_type(structure)
-            c_id = db.Structure(s_id, self._structures).get_aggregate()
-            lhs_weight *= self._get_structure_weights(c_id, aggregate_type)[s_id.string()]
-        rhs_weight = 1.0
-        for s_id in structure_ids[1]:
-            structure = db.Structure(s_id, self._structures)
-            aggregate_type = get_aggregate_type(structure)
-            c_id = db.Structure(s_id, self._structures).get_aggregate()
-            rhs_weight *= self._get_structure_weights(c_id, aggregate_type)[s_id.string()]
-        return lhs_weight, rhs_weight
-
-    def _is_parallel_to_reaction(self, step: db.ElementaryStep, reaction: db.Reaction):
-        rxn_reactants = reaction.get_reactants(db.Side.BOTH)
-        step_reactant_structure_ids = step.get_reactants(db.Side.BOTH)
-        if len(rxn_reactants[0]) != len(step_reactant_structure_ids[0]):
-            assert len(rxn_reactants[0]) == len(step_reactant_structure_ids[1])
-            return False
-        for s_id in step_reactant_structure_ids[0]:
-            aggregate_id = db.Structure(s_id, self._structures).get_aggregate()
-            if aggregate_id not in rxn_reactants[0]:
-                assert aggregate_id in rxn_reactants[1]
-                return False
-        for s_id in step_reactant_structure_ids[1]:
-            aggregate_id = db.Structure(s_id, self._structures).get_aggregate()
-            if aggregate_id not in rxn_reactants[1]:
-                assert aggregate_id in rxn_reactants[0]
-                return False
-        return True
-
-    def _get_reaction_rates_according_to_model(self, model, elementary_step_id, reaction)\
-            -> Union[Tuple[float, float], Tuple[None, None]]:
-        temperature = float(model.temperature)
-        if temperature is None:
-            return None, None
-        elementary_step = db.ElementaryStep(elementary_step_id, self._elementary_steps)
-        elementary_step_type = elementary_step.get_type()
-
-        lhs_barrier = None
-        rhs_barrier = None
-        if elementary_step_type == db.ElementaryStepType.BARRIERLESS:
-            reactants = elementary_step.get_reactants(db.Side.BOTH)
-            # TODO Include some sophisticated model for barrierless reactions.
-            for s_id in reactants[0] + reactants[1]:
-                energy = get_energy_for_structure(db.Structure(s_id), self._energy_label, model, self._structures,
-                                                  self._properties)
-                if energy is None:
-                    return None, None
-            lhs_barrier = 0.0
-            rhs_barrier = 0.0
-        else:
-            if self._use_spline_barrier:
-                lhs_barrier, rhs_barrier = elementary_step.get_barrier_from_spline()
+            if structure.get_label() == db.Label.DUPLICATE:
+                unique_list.append(structure.get_original())
             else:
-                lhs_barrier, rhs_barrier = get_barriers_for_elementary_step_by_type(elementary_step, self._energy_label,
-                                                                                    model, self._structures,
-                                                                                    self._properties)
-        if lhs_barrier is None or rhs_barrier is None:
-            return None, None
-        rhs_rate = rate_constant_from_barrier(rhs_barrier, temperature)
-        lhs_rate = rate_constant_from_barrier(lhs_barrier, temperature)
-        is_parallel = self._is_parallel_to_reaction(elementary_step, reaction)
-        if is_parallel:
-            return lhs_rate, rhs_rate
-        else:
-            return rhs_rate, lhs_rate
-
-    def _get_old_zero_flux_reactions(self) -> List[db.ID]:
-        reaction_ids = self._get_reactions_in_last_kinetic_modeling_jobs()
-        zero_flux_reactions = list()
-        for rxn_id in reaction_ids:
-            if self._reaction_has_zero_flux(rxn_id):
-                zero_flux_reactions.append(rxn_id)
-        return zero_flux_reactions
+                unique_list.append(s_id)
+        return unique_list
 
-    def _get_reactions_in_last_kinetic_modeling_jobs(self) -> List[db.ID]:
-        selection = {"$and": [
-            {"status": "complete"},
-            {"job.order": self._kinetic_modeling_job.order}
-        ]
-        }
-        reaction_str_id_set: Set[str] = set()
-        for calculation in self._calculations.iterate_calculations(dumps(selection)):
-            calculation.link(self._calculations)
-            str_ids = calculation.get_settings()["reaction_ids"]
-            reaction_str_id_set = reaction_str_id_set.union(str_ids)
-        return [db.ID(str_id) for str_id in reaction_str_id_set]
-
-    def _reaction_has_zero_flux(self, reaction_id: db.ID) -> bool:
-        reaction = db.Reaction(reaction_id, self._reactions)
-        reactants = reaction.get_reactants(db.Side.BOTH)
-        reactant_types = reaction.get_reactant_types(db.Side.BOTH)
-        for a_id, a_type in zip(reactants[0] + reactants[1], reactant_types[0] + reactant_types[1]):
-            aggregate = get_compound_or_flask(a_id, a_type, self._compounds, self._flasks)
-            flux = query_concentration_with_object("concentration_flux", aggregate, self._properties, self._structures)
-            if flux < self._min_flux_truncation:
-                return True
+    @staticmethod
+    def _invert_elementary_step(elementary_step: db.ElementaryStep):
+        reactants = copy(elementary_step.get_reactants(db.Side.BOTH))
+        elementary_step.set_reactants(reactants[1], db.Side.LHS)
+        elementary_step.set_reactants(reactants[0], db.Side.RHS)
+        if elementary_step.has_spline():
+            spline = elementary_step.get_spline()
+            knots = np.flipud(np.asarray([1 - x for x in spline.knots]))
+            trajectory = np.flipud(spline.data)
+            ts_position = 1 - spline.ts_position
+            elements = spline.elements
+            inverted_spline = utils.bsplines.TrajectorySpline(elements, knots, trajectory, ts_position)
+            elementary_step.set_spline(inverted_spline)
+
+    def _disable_barrierless_if_mixed_types_in_reaction(self, reaction: db.Reaction, new_step: db.ElementaryStep):
+        """
+        If we have a regular elementary step and a barrierless elementary step for an identical reaction,
+        we are for now distrusting the barrierless steps and disable them, but keep them in the reaction.
+
+        NOTE: This will not work with old databases that have not worked with this method before out of the box.
+        To ensure backwards applicability, the content of the reaction collection has to be deleted first.
+        NOTE: This method assumes there are only TWO types of elementary steps.
+        """
+        # we have two possible procedures here:
+        # 1) check new step type:
+        #    - if regular, loop over all steps of reaction and disable all barrierless steps
+        #    - if barrierless, loop over steps of reaction, if we find a regular step, break and disable new
+        # 2) check type of first enabled step in reaction:
+        #    - if different to new step type, check new type
+        #        - if regular, loop over all steps of reaction and disable barrierless
+        #        - if barrierless, only disable new
+        #    - if identical do nothing
+        # case 2 seems to be more efficient, works on the assumption that newly added entry has always been checked,
+        # hence added note in doc string
+        step_type = None
+        steps = reaction.get_elementary_steps()
+        # find step type of first enabled step in reaction
+        for step_id in steps:
+            reaction_step = db.ElementaryStep(step_id, self._elementary_steps)
+            if reaction_step.explore() and reaction_step.analyze():
+                step_type = reaction_step.get_type()
+                break
+        # we have a mismatch between the first activate step in reaction and the new step
+        if step_type is not None and step_type != new_step.get_type():
+            warn(f"Found barrierless and regular elementary step for identical reaction {str(reaction.id())}. "
+                 f"We are now disabling all barrierless steps in this reaction.")
+            new_type = new_step.get_type()
+            if new_type == db.ElementaryStepType.BARRIERLESS:
+                # new is barrierless, first enabled was regular, hence we should not need to check all steps of reaction
+                new_step.disable_exploration()
+                new_step.disable_analysis()
+            elif new_type == db.ElementaryStepType.REGULAR:
+                # new step is regular, and first enabled was barrierless, disable all barrierless in reaction
+                for step_id in steps:
+                    reaction_step = db.ElementaryStep(step_id, self._elementary_steps)
+                    if reaction_step.get_type() == db.ElementaryStepType.BARRIERLESS:
+                        reaction_step.disable_exploration()
+                        reaction_step.disable_analysis()
+            else:
+                raise TypeError(f"Unsupported elementary step type for elementary step {str(new_step.id())}")
+
+    def _add_reaction_to_aggregate(self, aggregates_to_change: List[db.ID], aggregate_types: List[db.CompoundOrFlask],
+                                   reaction_id: db.ID):
+        for aggregate_id, aggregate_type in zip(aggregates_to_change, aggregate_types):
+            flask_or_compound = get_compound_or_flask(aggregate_id, aggregate_type, self._compounds, self._flasks)
+            flask_or_compound.add_reaction(reaction_id)
+
+    def _same_energy(self, ts_new_energy: Union[float, None], ts_old: db.Structure, model: db.Model) -> bool:
+        ts_old_energy = get_energy_for_structure(ts_old, "electronic_energy", model, self._structures,
+                                                 self._properties)
+        # Check transition state energy.
+        if ts_old_energy is None or ts_new_energy is None:
+            return False
+        abs_difference = abs(ts_old_energy - ts_new_energy)
+        return abs_difference <= self.options.energy_tolerance
+
+    def _same_coordinates(self, ts_positions_new: np.ndarray, ts_elements: List[utils.ElementType],
+                          ts_old: db.Structure) -> bool:
+        fit = utils.QuaternionFit(ts_positions_new, ts_old.get_atoms().positions, ts_elements)
+        rmsd = fit.get_weighted_rmsd()
+        # Check structure RMSD
+        # TODO It may be possible to reorder the atoms of both transition states to be in identical
+        # order before checking the RMSD using atom-index maps.
+        return rmsd <= self.options.rmsd_tolerance
+
+    def _same_starting_structures(self, lhs_new_step: List[db.ID], old_step: db.ElementaryStep) -> bool:
+        lhs_old_step = old_step.get_reactants(db.Side.LHS)[0]
+        if len(lhs_old_step) != len(lhs_new_step):
+            return False
+        return sorted(lhs_old_step) == sorted(lhs_new_step)
+
+    def _is_duplicate(self, elementary_step: db.ElementaryStep, reaction: db.Reaction) -> bool:
+        lhs_new_step = elementary_step.get_reactants(db.Side.LHS)[0]
+        if not elementary_step.has_transition_state():
+            return False
+        ts_new = db.Structure(elementary_step.get_transition_state(), self._structures)
+        model = ts_new.model
+        ts_new_energy = get_energy_for_structure(
+            ts_new, "electronic_energy", model, self._structures, self._properties)
+        ts_positions_new = ts_new.get_atoms().positions
+        ts_elements = ts_new.get_atoms().elements
+        for old_step_id in reaction.get_elementary_steps():
+            old_step = db.ElementaryStep(old_step_id, self._elementary_steps)
+            if self.options.use_structure_deduplication:
+                if not self._same_starting_structures(lhs_new_step, old_step):
+                    continue
+
+            if not old_step.has_transition_state():
+                continue
+            ts_old = db.Structure(old_step.get_transition_state(), self._structures)
+
+            if self.options.use_energy_deduplication:
+                if not self._same_energy(ts_new_energy, ts_old, model):
+                    continue
+            if self.options.use_rmsd_deduplication:
+                if not self._same_coordinates(ts_positions_new, ts_elements, ts_old):
+                    continue
+
+            # If all checks signal identical structures. This is a duplicate!
+            return True
         return False
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/__init__.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,21 +2,28 @@
 # -*- coding: utf-8 -*-
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
-from typing import List
+from abc import ABC, abstractmethod
+from ctypes import c_int
+from enum import Enum
+from setproctitle import setproctitle
+from typing import List, Callable, Optional
 import signal
 import time
 
 # Third party imports
 import scine_database as db
 
+from scine_chemoton.utilities import connect_to_db
+from scine_chemoton.utilities.comparisons import attribute_comparison
+
 
 class HoldsCollections:
 
     def __init__(self):
         super().__init__()  # necessary for multiple inheritance
         self._required_collections: List[str] = []
         self._manager = None
@@ -48,100 +55,171 @@
                                           f"is not possible, we are only supporting {self.possible_attributes()}.")
         for attr in self._required_collections:
             if attr == "manager":
                 setattr(self, f"_{attr}", manager)
             else:
                 setattr(self, f"_{attr}", manager.get_collection(attr))
 
+    def unset_collections(self) -> None:
+        if hasattr(self, "_parent"):
+            setattr(self, "_parent", None)
+        for attr in self.possible_attributes():
+            setattr(self, f"_{attr}", None)
+        self._unset_collections_of_attributes(self)
+
+    def _unset_collections_of_attributes(self, inst):
+        if not hasattr(inst, '__dict__'):
+            return
+        for key, attr in inst.__dict__.items():
+            if isinstance(attr, HoldsCollections):
+                attr.unset_collections()
+            elif isinstance(attr, db.Collection) or isinstance(attr, db.Manager):
+                setattr(inst, key, None)
+                continue
+            elif hasattr(attr, '__dict__') and not isinstance(attr, Enum):
+                self._unset_collections_of_attributes(attr)
+            if hasattr(attr, '__iter__') and not isinstance(attr, str):
+                for a in attr:
+                    self._unset_collections_of_attributes(a)
+
+
+class HasName:
+
+    def __init__(self):
+        super().__init__()  # necessary for multiple inheritance
+        self._name = 'Chemoton' + self.__class__.__name__
+
+    @property
+    def name(self) -> str:
+        return self._name
+
+    @name.setter
+    def name(self, n: str):
+        self._name = n
+
+    def _give_current_process_own_name(self) -> None:
+        setproctitle(self.name)
+
+    def _remove_chemoton_from_name(self) -> None:
+        self._name = self._name.replace("Chemoton", "")
+
+    def _join_names(self, objects: list) -> None:
+        self._name += "(" + ", ".join(f.name for f in objects) + ")"
+
+    def __str__(self):
+        return self.name
 
-class Gear(HoldsCollections):
+
+class Gear(ABC, HoldsCollections, HasName):
     """
     The base class for all Gears.
 
     A Gear in Chemoton is a continuous loop that alters, analyzes or interacts
     in any other way with a reaction network stored in a SCINE Database.
     Each Gear has to be attached to an Engine(:class:`scine_chemoton.engine.Engine`)
     and will then help in driving the exploration of chemical reaction networks
     forward.
 
-    Extending the features of Chemoton can be done by add new Gears or altering
+    Extending the features of Chemoton can be done by adding new Gears or altering
     existing ones.
     """
 
+    class Options:
+
+        __slots__ = "model"
+
+        def __init__(self):
+            self.model = db.Model("PM6", "PM6", "")
+
+        def __eq__(self, other) -> bool:
+            return attribute_comparison(self, other)
+
     def __init__(self):
         super().__init__()
+        self.options = self.Options()
         self.name = 'Chemoton' + self.__class__.__name__ + 'Gear'
+        self.stop_at_next_break_point = False
+
+    def __eq__(self, other):
+        if not isinstance(other, Gear):
+            return False
+        return self.stop_at_next_break_point == other.stop_at_next_break_point \
+            and self.options == other.options
 
     class _DelayedKeyboardInterrupt:
+        def __init__(self, callable: Optional[Callable]):
+            self.signal_received = False
+            self.callable = callable
+
         def __enter__(self):
-            self.signal_received = False  # pylint: disable=attribute-defined-outside-init
             self.old_handler = \
                 signal.signal(signal.SIGINT, self.handler)  # pylint: disable=attribute-defined-outside-init
 
         def handler(self, sig, frame):
-            self.signal_received = (sig, frame)  # pylint: disable=attribute-defined-outside-init
+            self.signal_received = (sig, frame)
+            if self.callable is not None:
+                self.callable()
 
         def __exit__(self, type, value, traceback):
             signal.signal(signal.SIGINT, self.old_handler)
             if self.signal_received:
                 self.old_handler(*self.signal_received)
 
-    def __call__(self, credentials: db.Credentials, single: bool = False):
+    def __call__(self, credentials: db.Credentials, loop_count: c_int, single: bool = False):
         """
         Starts the main loop of the Gear, then acting on the database referenced
         by the given credentials.
 
         Parameters
         ----------
         credentials :: db.Credentials (Scine::Database::Credentials)
             The credentials to a database storing a reaction network.
         single :: bool
             If true, runs only a single iteration of the actual loop.
             Default: false, meaning endless repetition of the loop.
         """
-        try:
-            import setproctitle
-            setproctitle.setproctitle(self.name)
-        except ModuleNotFoundError:
-            pass
+        self._give_current_process_own_name()
+
         # Make sure cycle time exists
         sleep = getattr(getattr(self, "options"), "cycle_time")
 
-        # Prepare database connection
-        if self._manager is None or self._manager.get_credentials() != credentials:
-            self._manager = db.Manager()
-            self._manager.set_credentials(credentials)
-            self._manager.connect()
-            time.sleep(1.0)
-            if not self._manager.has_collection("calculations"):
-                raise RuntimeError("Stopping Gear/Engine: database is missing collections.")
-
-            # Get required collections
-            self.initialize_collections(self._manager)
-            self._propagate_db_manager(self._manager)
+        # Prepare database connection and members
+        _initialize_a_gear_to_a_db(self, credentials)
 
         # Infinite loop with sleep
         last_cycle = time.time()
         # Instant first loop
-        with self._DelayedKeyboardInterrupt():
+        with self._DelayedKeyboardInterrupt(callable=self.stop):
             self._loop_impl()
+        loop_count.value += 1
         # Stop if only a single loop was requested
         if single:
             return
         while True:
             # Wait if needed
             now = time.time()
             if now - last_cycle < sleep:
                 time.sleep(sleep - now + last_cycle)
             last_cycle = time.time()
 
-            with self._DelayedKeyboardInterrupt():
+            with self._DelayedKeyboardInterrupt(callable=self.stop):
                 self._loop_impl()
+            loop_count.value += 1
 
-    def _loop_impl(self):
-        """
-        Main loop to be implemented by all derived Gears.
-        """
-        raise NotImplementedError
+    @abstractmethod
+    def _loop_impl(self):  # Main loop to be implemented by all derived Gears.
+        pass
 
     def _propagate_db_manager(self, manager: db.Manager):
         pass
+
+    def stop(self) -> None:
+        self.stop_at_next_break_point = True
+
+
+def _initialize_a_gear_to_a_db(gear: Gear, credentials: db.Credentials) -> None:
+    if gear._manager is None or gear._manager.get_credentials() != credentials:
+        gear._manager = connect_to_db(credentials)
+        # Get required collections
+        gear.initialize_collections(gear._manager)
+    # always propagate in case a member has been changed
+    gear._propagate_db_manager(gear._manager)
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/compound.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/compound.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 See LICENSE.txt for details.
 """
 
 # Standard library imports
 from json import dumps
 from typing import Union, Tuple, Dict, List
 from warnings import warn
+from copy import copy
 
 # Third party imports
 import scine_database as db
 import scine_utilities as utils
 import scine_molassembler as masm
 
 # Local application imports
 from . import Gear
 from ..utilities.queries import stop_on_timeout, calculation_exists_in_structure
 from ..utilities.calculation_creation_helpers import finalize_calculation
+from ..utilities.masm import mol_from_cbor
 
 
 class BasicAggregateHousekeeping(Gear):
     """
     This Gear updates all relevant Structures stored in the database with
     bond orders and graph representations.
     This data is then used to sort each Structure into existing Compounds/Flasks or to
@@ -39,15 +41,14 @@
     that do not have an Aggregate assigned. The Gear then generates bond orders and molecular graphs
     ('masm_cbor_graph', and 'masm_decision_list') if they are not yet present.
     Using the molecular graphs the Structures are then sorted into Compounds/Flasks.
     """
 
     def __init__(self):
         super().__init__()
-        self.options = self.Options()
         self._required_collections = ["calculations", "compounds", "flasks",
                                       "properties", "structures", "reactions"]
         self._compound_map: Dict[int, Dict[Tuple[int, int, int], List[db.ID]]] = dict()
         """
         Caching map from n_atoms, n_molecules, charge, multiplicity to compound ids.
         """
         self._flask_map: Dict[int, Dict[Tuple[int, int, int], List[db.ID]]] = dict()
@@ -55,44 +56,38 @@
         Caching map from n_atoms, n_molecules, charge, multiplicity to flask ids.
         """
         self._unique_structures: Dict[str, List[Tuple[db.ID, str]]] = dict()
         """
         Caching map from compound id to list of structure ids and decision lists.
         """
 
-    class Options:
+    class Options(Gear.Options):
         """
-        The options for the BasicAggregateHouseKeeping Gear.
+        The options for the BasicAggregateHousekeeping Gear.
         """
 
         __slots__ = [
             "cycle_time",
-            "model",
             "bond_order_job",
             "bond_order_settings",
             "graph_job",
             "graph_settings",
             "exclude_misguided_conformer_optimizations"
         ]
 
         def __init__(self):
+            super().__init__()
             self.cycle_time = 10
             """
             int
                 The minimum number of seconds between two cycles of the Gear.
                 Cycles are finished independent of this option, thus if a cycle
                 takes longer than the cycle_time will effectively lead to longer
                 cycle times and not cause multiple cycles of the same Gear.
             """
-            self.model: db.Model = db.Model("PM6", "PM6", "")
-            """
-            db.Model (Scine::Database::Model)
-                The Model used for the bond order calculations.
-                The default is: PM6 using Sparrow.
-            """
             self.bond_order_job: db.Job = db.Job("scine_bond_orders")
             """
             db.Job (Scine::Database::Calculation::Job)
                 The Job used for the bond order calculations.
                 The default is: the 'scine_bond_orders' order on a single core.
             """
             self.bond_order_settings: utils.ValueCollection = utils.ValueCollection()
@@ -128,16 +123,15 @@
             self._unique_structures[key] = []
             for s_id in structure_ids:
                 structure = db.Structure(s_id, self._structures)
                 if structure.get_label() in [db.Label.DUPLICATE, db.Label.MINIMUM_GUESS]:
                     continue
                 self._unique_structures[key].append((s_id, structure.get_graph("masm_decision_list")))
 
-    def _add_to_unique_structures(self, structure: db.Structure):
-        key = structure.get_aggregate().string()
+    def _add_to_unique_structures(self, key: str, structure: db.Structure):
         if key in self._unique_structures:
             self._unique_structures[key].append((structure.id(), structure.get_graph("masm_decision_list")))
         else:
             self._unique_structures[key] = [(structure.id(), structure.get_graph("masm_decision_list"))]
 
     def _create_compound_map(self):
         for compound in stop_on_timeout(self._compounds.iterate_all_compounds()):
@@ -146,87 +140,60 @@
 
     def _create_flask_map(self):
         for flask in stop_on_timeout(self._flasks.iterate_all_flasks()):
             flask.link(self._flasks)
             self._add_to_map(flask, self._flask_map)
 
     def _add_to_map(self, aggregate: Union[db.Compound, db.Flask], cache_map: Dict):
-        n_atoms, n_molecules, charge, multiplicity, graph = self._get_aggregate_info(aggregate)
+        sum_formula, n_molecules, charge, multiplicity, mols = self._get_aggregate_info(aggregate)
         key = (n_molecules, charge, multiplicity)
-        if n_atoms in cache_map:
-            if key in cache_map[n_atoms]:
-                cache_map[n_atoms][key].append((aggregate.id(), graph))
+        if sum_formula in cache_map:
+            if key in cache_map[sum_formula]:
+                if (aggregate.id(), mols) in cache_map[sum_formula][key]:
+                    return
+                cache_map[sum_formula][key].append((aggregate.id(), mols))
                 return
             else:
-                cache_map[n_atoms][key] = [(aggregate.id(), graph)]
+                cache_map[sum_formula][key] = [(aggregate.id(), mols)]
                 return
-        cache_map[n_atoms] = {key: [(aggregate.id(), graph)]}
+        cache_map[sum_formula] = {key: [(aggregate.id(), mols)]}
 
-    def _get_aggregate_info(self, aggregate: Union[db.Compound, db.Flask]) -> Tuple[int, int, int, int, str]:
-        # We could even think about adding the graph here too ...
-        centroid = db.Structure(aggregate.get_centroid(), self._structures)
-        graph = centroid.get_graph("masm_cbor_graph")
-        return len(centroid.get_atoms()), len(graph.split(";")), centroid.get_charge(), centroid.get_multiplicity(),\
-            graph
+    def _get_sum_formula(self, mols: List[masm.Molecule]) -> str:
+        sum_formulas = []
+        for m in mols:
+            sum_formulas.append(m.graph.__repr__().split()[-1])
+        sum_formulas.sort()
+        return ','.join(sum_formulas)
 
     @staticmethod
-    def _get_aggregate_from_map(n_atoms: int, n_molecules: int, charge: int, multiplicity: int, graph,
+    def _get_aggregate_from_map(sum_formula: str, n_molecules: int, charge: int, multiplicity: int, mols,
                                 cache_map: Dict) -> Union[db.ID, None]:
-        if n_atoms in cache_map:
+        if sum_formula in cache_map:
             key = (n_molecules, charge, multiplicity)
-            if key in cache_map[n_atoms]:
-                for a_id, ref_graph in cache_map[n_atoms][key]:
-                    if masm.JsonSerialization.equal_molecules(ref_graph, graph):
+            if key in cache_map[sum_formula]:
+                for a_id, ref_mols in cache_map[sum_formula][key]:
+                    remaining_mols = copy(ref_mols)
+                    for m in mols:
+                        idx = remaining_mols.index(m) if m in remaining_mols else None
+                        if idx is not None:
+                            remaining_mols.pop(idx)
+                        else:
+                            break
+                    else:
                         return a_id
         return None
 
     def _loop_impl(self):
         if not self._compound_map:
             self._create_compound_map()
         if not self._flask_map:
             self._create_flask_map()
         if not self._unique_structures:
             self._create_unique_structure_map()
         self._check_for_aggregates()
-        self._check_compounds_in_flasks()
-
-    def _check_compounds_in_flasks(self):
-        """
-        Check for Flasks without Compounds.
-        Complete them if ALL sub-structures are assigned a Compound.
-        """
-        # Check for flasks without compounds
-        selection = {
-            "compounds": {"$size": 0}
-        }
-        for flask in stop_on_timeout(self._flasks.iterate_flasks(dumps(selection))):
-            flask.link(self._flasks)
-            flask_centroid = db.Structure(flask.get_centroid(), self._structures)
-            if not flask_centroid.has_graph("masm_cbor_graph") or not flask_centroid.has_graph("masm_idx_map"):
-                warn(f"Centroid {str(flask_centroid.id())} of flask {str(flask.id())} is missing a graph")
-                continue
-            graphs = flask_centroid.get_graph("masm_cbor_graph").split(';')
-            compounds = []
-            n_atoms_per_molecule = self.get_n_atoms(flask_centroid)
-            n_graphs_missing = len(n_atoms_per_molecule)
-            for i, n_atoms in enumerate(n_atoms_per_molecule):
-                if n_atoms not in self._compound_map:
-                    break
-                for key in self._compound_map[n_atoms]:
-                    compound_list = self._compound_map[n_atoms][key]
-                    for c_id, current in compound_list:
-                        # we are looping in reverse, so we can pop the element if identical while looping
-                        # we loop through because one compound could be part of flask multiple times
-                        # e.g. solute with 2 water molecules
-                        if masm.JsonSerialization.equal_molecules(graphs[i], current):
-                            compounds.append(c_id)
-                            n_graphs_missing -= 1
-                        if n_graphs_missing == 0:
-                            flask.set_compounds(compounds)
-                            break
 
     def _check_for_aggregates(self):
         # Setup query for optimized structures without aggregate
         selection = {
             "$and": [
                 {
                     "$or": [
@@ -238,14 +205,16 @@
                 {"aggregate": ""},
                 {"analysis_disabled": {"$ne": True}},
             ]
         }
         # Loop over all results
         for structure in stop_on_timeout(self._structures.iterate_structures(dumps(selection))):
             structure.link(self._structures)
+            if self.stop_at_next_break_point:
+                return
             if structure.has_graph("masm_cbor_graph"):
                 # Check if graph exists
                 graph = structure.get_graph("masm_cbor_graph")
                 label = structure.get_label()
                 if ";" in graph:
                     if label != db.Label.COMPLEX_OPTIMIZED:
                         warn(f"Structure '{str(structure.id())}' received incorrect label '{str(label)}', "
@@ -261,28 +230,31 @@
                 self._setup_bond_order_job(structure.id())
                 continue
 
             # If a graph exists but no aggregate is registered, generate a new aggregate
             # or append the structure to an existing compound
             matching_aggregate = self._get_matching_aggregate(structure)
             if matching_aggregate is not None:
-                structure.set_aggregate(matching_aggregate.id())
-                matching_aggregate.add_structure(structure.id())
                 # Check if duplicate in same aggregate
                 duplicate = self._query_duplicate(structure, matching_aggregate)
                 if duplicate is not None:
                     structure.set_label(db.Label.DUPLICATE)
                     structure.set_comment("Structure is a duplicate of {:s}.".format(str(duplicate.id())))
-                    structure.set_as_duplicate_of(duplicate.id())
+                    structure.set_original(duplicate.id())
+                else:
+                    # only add aggregate info for non-duplicates
+                    structure.set_aggregate(matching_aggregate.id())
+                    matching_aggregate.add_structure(structure.id())
             else:
                 # Create a new aggregate but only if the structure is not a misguided conformer optimization
                 # TODO this query may become a bottleneck for huge databases.
                 #      avoiding a query into the calculations would be much preferred
                 selection = {
                     "$and": [
+                        {"status": {"$in": ["complete", "failed", "analyzed"]}},
                         {"results.structures": {"$oid": structure.id().string()}},
                         {"results.elementary_steps": {"$size": 0}},
                     ]
                 }
                 hit = None
                 if self.options.exclude_misguided_conformer_optimizations:
                     hit = self._calculations.get_one_calculation(dumps(selection))
@@ -337,58 +309,75 @@
         # Setup calculation of a graph
         calculation = db.Calculation(db.ID(), self._calculations)
         calculation.create(self.options.model, self.options.graph_job, [structure_id])
         if self.options.graph_settings:
             calculation.set_settings(self.options.graph_settings)
         finalize_calculation(calculation, self._structures)
 
+    def _get_aggregate_info(
+        self, aggregate: Union[db.Compound, db.Flask]
+    ) -> Tuple[str, int, int, int, List[masm.Molecule]]:
+        # We could even think about adding the graph here too ...
+        centroid = db.Structure(aggregate.get_centroid(), self._structures)
+        graph = centroid.get_graph("masm_cbor_graph")
+        mols = [mol_from_cbor(m) for m in graph.split(";")]
+        sum_formula = self._get_sum_formula(mols)
+        return sum_formula, len(graph.split(";")), centroid.get_charge(), centroid.get_multiplicity(),\
+            mols
+
     def _get_matching_aggregate(self, structure: db.Structure) -> Union[db.Compound, db.Flask, None]:
         """
         Queries database for matching aggregate of the given structure based on:
           * graph (irrespective of order for flasks)
           * charge
           * multiplicity
         Returns None if no matching aggregate in DB yet
         """
         graph = structure.get_graph("masm_cbor_graph")
+        mols = [mol_from_cbor(m) for m in graph.split(";")]
         charge = structure.get_charge()
         multiplicity = structure.get_multiplicity()
-        n_atoms = len(structure.get_atoms())
-        n_molecules = len(graph.split(";"))
+        sum_formula = self._get_sum_formula(mols)
+        n_molecules = len(mols)
         if n_molecules > 1:
-            f_id = self._get_aggregate_from_map(n_atoms, n_molecules, charge, multiplicity, graph, self._flask_map)
+            f_id = self._get_aggregate_from_map(
+                sum_formula, n_molecules, charge, multiplicity, mols, self._flask_map
+            )
             if f_id:
                 return db.Flask(f_id, self._flasks)
         else:
-            c_id = self._get_aggregate_from_map(n_atoms, n_molecules, charge, multiplicity, graph, self._compound_map)
+            c_id = self._get_aggregate_from_map(
+                sum_formula, n_molecules, charge, multiplicity, mols, self._compound_map
+            )
             if c_id:
                 return db.Compound(c_id, self._compounds)
         return None
 
     def _query_duplicate(self, structure: db.Structure, aggregate: Union[db.Compound, db.Flask]) \
             -> Union[db.Structure, None]:
         """
         Check based on decision lists if the given aggregate has a duplicate structure to the given structure
         NOTE: not implemented for flasks yet
         """
         if isinstance(aggregate, db.Flask):
             # currently not possible
             return None
-        decision_list = structure.get_graph("masm_decision_list")
         key = aggregate.id().string()
         if key in self._unique_structures:
             similar_structures = self._unique_structures[key]
+            decision_list = structure.get_graph("masm_decision_list")
+            model = structure.get_model()
             for sid, ref_decision_list in similar_structures:
                 if not masm.JsonSerialization.equal_decision_lists(decision_list, ref_decision_list):
                     continue
                 similar_structure = db.Structure(sid, self._structures)
-                if similar_structure.get_model() == structure.get_model():
+                if similar_structure.get_model() == model:
                     return similar_structure
 
-        self._add_to_unique_structures(structure)
+        self._add_to_unique_structures(key, structure)
         return None
 
     @staticmethod
     def get_n_atoms(structure: db.Structure) -> List[int]:
         import ast
         idx_map = ast.literal_eval(structure.get_graph("masm_idx_map"))
         n_mols = 2
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/pathfinder.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/pathfinder.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,64 +2,66 @@
 # -*- coding: utf-8 -*-
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
-from typing import Iterator, List, Tuple, Union, Dict
+from typing import Optional, Iterator, List, Tuple, Union, Dict
 import networkx as nx
 import numpy as np
+import json
+import sys
 from itertools import islice
 
 # Third party imports
 import scine_database as db
 
 # Local application imports
 from ..utilities.energy_query_functions import get_energy_for_structure, get_barriers_for_elementary_step_by_type, \
-    get_elementery_step_with_min_ts_energy, rate_constant_from_barrier
+    get_elementary_step_with_min_ts_energy, rate_constant_from_barrier
 from ..utilities.get_molecular_formula import get_molecular_formula_of_aggregate
 
 
 class Pathfinder:
     """
     A class to represent a list of reactions as a graph and query this graph for simple paths between two nodes.
     In a simple path, every node part of the path is visited only once.
 
     Attributes
     ----------
-    _calculations :: db.Collection
+    _calculations : db.Collection
         Collection of the calculations of the connected database.
-    _compounds :: db.Collection
+    _compounds : db.Collection
         Collection of the compounds of the connected database.
-    _flasks :: db.Collection
+    _flasks : db.Collection
         Collection of the flasks of the connected database.
-    _reactions :: db.Collection
+    _reactions : db.Collection
         Collection of the reactions of the connected database.
-    _elementary_steps :: db.Collection
+    _elementary_steps : db.Collection
         Collection of the elementary steps of the connected database.
-    _structures :: db.Collection
+    _structures : db.Collection
         Collection of the structures of the connected database.
-    _properties :: db.Collection
+    _properties : db.Collection
         Collection of the properties of the connected database.
     graph_handler
         A class handling the construction of the graph. Can be adapted to one's needs.
-    _use_old_iterator :: bool
+    _use_old_iterator : bool
         Bool to indicate if the old iterator shall be used querying for paths between a source - target pair.
-    _unique_iterator_memory :: Tuple[Tuple[List[str], float], Iterator]
+    _unique_iterator_memory : Tuple[Tuple[List[str], float], Iterator]
         Memory of iterator with the corresponding path and its length as well as the iterator.
-    start_compounds :: List[str]
+    start_compounds : List[str]
         A list containing the compounds which are present at the start.
-    start_compounds_set :: bool
+    start_compounds_set : bool
         Bool to indicate if start_compounds are set.
-    _pseudo_inf :: float
+    _pseudo_inf : float
         Float for edges with infinite weight.
-    compound_costs :: Dict[str, float]
+    compound_costs : Dict[str, float]
         A dictionary containing the cost of the compounds with the compounds as keys.
-    compound_costs_solved :: bool
+    compound_costs_solved : bool
         Bool to indicate if all compounds have a compound cost.
     """
 
     def __init__(self, db_manager: db.Manager):
         self.options = self.Options()
         self.manager = db_manager
         # Get required collections
@@ -79,20 +81,22 @@
 
         # Compound costs
         self.start_compounds: List[str] = []
         self.start_compounds_set = False
         self._pseudo_inf = 1e12
         self.compound_costs: Dict[str, float] = {}
         self.compound_costs_solved = False
+        self.graph_updated_with_compound_costs = False
 
     class Options:
         """
         A class to vary the setup of Pathfinder.
         """
-        __slots__ = {"graph_handler", "barrierless_weight", "model", "use_energy_threshold", "energy_threshold"}
+        __slots__ = {"graph_handler", "barrierless_weight", "model", "filter_negative_barriers", "use_structure_model",
+                     "structure_model", "energy_threshold"}
 
         def __init__(self):
             self.graph_handler: str = "basic"  # pylint: disable=no-member
             """
             A string indicating which graph handler to be used.
             """
             self.barrierless_weight: float = 1.0  # 0.01
@@ -100,15 +104,19 @@
             The weight for barrierless reactions (basic) and rate constant (barrier), respectively.
             """
             self.model: Union[None, db.Model] = None
             """
             The model for the compounds to be included.
             """
             # in kJ / mol
-            self.use_energy_threshold: bool = False
+            self.filter_negative_barriers: bool = False
+
+            self.use_structure_model: bool = False
+
+            self.structure_model: Union[None, db.Model] = None
             self.energy_threshold: float = 100.0
 
     @staticmethod
     def get_valid_graph_handler_options() -> List[str]:
         return ["basic", "barrier"]
 
     def _construct_graph_handler(self):
@@ -121,21 +129,21 @@
         RuntimeError
             Invalid options for graph handler.
         """
         if not self.graph_handler:
             if self.options.graph_handler not in self.get_valid_graph_handler_options():
                 raise RuntimeError("Invalid graph handler option.")
             if self.options.graph_handler == "basic":
-                self.graph_handler = self.BasicHandler(self.manager)
+                self.graph_handler = self.BasicHandler(self.manager, self.options.model, self.options.structure_model)
                 self.graph_handler.barrierless_weight = self.options.barrierless_weight
-                self.graph_handler.model = self.options.model
             elif self.options.graph_handler == "barrier":
-                self.graph_handler = self.BarrierBasedHandler(self.manager, self.options.model)
+                self.graph_handler = self.BarrierBasedHandler(
+                    self.manager, self.options.model, self.options.structure_model)
                 self.graph_handler.barrierless_weight = self.options.barrierless_weight
-                self.graph_handler.model = self.options.model
+                self.graph_handler.filter_negative_barriers = self.options.filter_negative_barriers
                 self.graph_handler._map_elementary_steps_to_reactions()
                 self.graph_handler._calculate_rate_constant_normalization()
 
     def _reset_iterator_memory(self):
         """
         Reset memory for unique memory.
         """
@@ -173,15 +181,15 @@
         n_skipped_paths : int
             Number of skipped paths from, by default 0. For example, when four paths are found (``n_requested_paths=4``)
             and ``n_skipped_paths=2``, the third, fourth, fifth and sixth path are returned. Therefore, this allows to
             set the starting point of the query.
 
         Returns
         -------
-        found_paths :: List[Tuple[List[str] float]]
+        found_paths : List[Tuple[List[str] float]]
             List of paths where each item (path) consists of the list of nodes of the path and its length.
         """
         assert self.graph_handler
         found_paths = []
         for path in self._k_shortest_paths(self.graph_handler.graph, source, target, n_requested_paths,
                                            weight="weight", path_start=n_skipped_paths):
             path_length = nx.path_weight(self.graph_handler.graph, path, "weight")
@@ -209,15 +217,15 @@
         target : str
             The ID of the targeted compound as string.
         number : int
             The number of unique paths to be returned. Per default, 3 paths are returned.
 
         Returns
         -------
-        path_tuple_list :: List[Tuple[List[str], float]]
+        path_tuple_list : List[Tuple[List[str], float]]
             List of paths where each item (path) consists the list of nodes of the path and its length.
         """
         assert self.graph_handler
         counter = 0
         path_tuple_list = list()
         # # # Initialise iterator over shortest simple paths if it is either not set or source/target do not match
         if not self._use_old_iterator or \
@@ -267,26 +275,31 @@
             self._unique_iterator_memory = ((new_path, new_path_cost), path_iterator)
         return path_tuple_list
 
     def get_elementary_step_sequence(self, path: List[str]) -> str:
         """
         Prints the sequence of elementary steps of a path with the compounds written as molecular formulas
         with multiplicity and charge as well as the final cost of the path.
-        Reactant node is printed in red, product node in blue to enhance readability.
+        Reactant node is returned in red, product node in blue to enhance readability.
 
         Parameters
         ----------
-        path :: Tuple[List[str] float]
+        path : Tuple[List[str] float]
             Path containing a list of the traversed nodes and the cost of this path.
+
+        Returns
+        -------
+        str
+            A string of the elementary step sequence of a given path.
         """
         sequence_string = ""
         assert self.graph_handler
         # # # Loop over elementary steps by dissecting path
-        for i in np.arange(0, len(path) - 2, 2):
-            step = path[i:i + 3]
+        for k in np.arange(0, len(path) - 2, 2):
+            step = path[k:k + 3]
             # # # Count Reactants
             reactants = [step[0]]
             reactants += self.graph_handler.graph.edges[step[0], step[1]]['required_compounds']
             # # # Count Products
             products = [step[2]]
             products += self.graph_handler.graph.edges[step[1], step[2]]['required_compounds']
 
@@ -314,14 +327,74 @@
                         rxn_eq += " + "
                 if i == 0:
                     rxn_eq += " -> "
             sequence_string += rxn_eq + "\n"
 
         return sequence_string
 
+    def get_overall_reaction_equation(self, path: List[str]) -> str:
+        """
+        Summarize a given path to a reaction equation and return its string.
+        Count the appearance of compounds in a reaction, -1 for reactants and +1 for products.
+        Returns the factor and the compound as molecular formula.
+
+        Parameters
+        ----------
+        path : List[str]
+            Path containing a list of the traversed nodes.
+
+        Returns
+        -------
+        str
+            A string of the overall reaction equation of a given path.
+        """
+        total_counter: Dict[str, float] = {}
+        assert self.graph_handler
+        # # # Loop over elementary steps
+        for i in np.arange(0, len(path) - 2, 2):
+            step = path[i:i + 3]
+            # # # Count Reactants
+            tmp_reactants = [step[0]]
+            tmp_reactants += self.graph_handler.graph.edges[step[0], step[1]]['required_compounds']
+            for key in tmp_reactants:
+                if key not in total_counter.keys():
+                    total_counter[key] = 0
+                total_counter[key] -= 1
+            # # # Count Products
+            tmp_products = [step[2]]
+            tmp_products += self.graph_handler.graph.edges[step[1], step[2]]['required_compounds']
+            for key in tmp_products:
+                if key not in total_counter.keys():
+                    total_counter[key] = 0
+                total_counter[key] += 1
+        # # # Contract reactant and product lists
+        reactants = [(cmp_id, abs(value)) for cmp_id, value in total_counter.items() if value < 0]
+        products = [(cmp_id, abs(value)) for cmp_id, value in total_counter.items() if value > 0]
+
+        reaction_equation = ""
+        for i, side in enumerate([reactants, products]):
+            for j, cmp_count in enumerate(side):
+                aggregate_id = cmp_count[0]
+                # # # Identify Compound or Flask
+                if self.graph_handler.graph.nodes[aggregate_id]['type'] == db.CompoundOrFlask.COMPOUND.name:
+                    aggregate_type = db.CompoundOrFlask.COMPOUND
+                elif self.graph_handler.graph.nodes[aggregate_id]['type'] == db.CompoundOrFlask.FLASK.name:
+                    aggregate_type = db.CompoundOrFlask.FLASK
+
+                aggregate_str = get_molecular_formula_of_aggregate(
+                    db.ID(aggregate_id), aggregate_type, self._compounds, self._flasks, self._structures)
+
+                reaction_equation += str(cmp_count[1]) + " " + aggregate_str
+                if j < len(side) - 1:
+                    reaction_equation += " + "
+            if i == 0:
+                reaction_equation += " = "
+
+        return reaction_equation
+
     @staticmethod
     def _k_shortest_paths(graph: nx.DiGraph, source: str, target: str, n_paths: int, weight: Union[str, None] = None,
                           path_start: int = 0) -> List[List[str]]:
         """
         Finding k shortest paths between a source and target node in a given graph.
         The length of the returned paths increases.
 
@@ -333,25 +406,25 @@
           https://networkx.org/documentation/stable/reference/algorithms/generated/ \
           networkx.algorithms.simple_paths.shortest_simple_paths.html
         * [1]: Jin Y. Yen, “Finding the K Shortest Loopless Paths in a Network”, Management Science, Vol. 17, No. 11,
                Theory Series (Jul., 1971), pp. 712-716.
 
         Parameters
         ----------
-        graph :: nx.DiGraph
+        graph : nx.DiGraph
             The graph to be queried.
-        source :: str
+        source : str
             The ID of the starting compound as string.
-        target :: str
+        target : str
             The ID of the targeted compound as string.
-        n_paths :: int
+        n_paths : int
             The number of paths to be returned.
-        weight :: Union[str, None], optional
+        weight : Union[str, None], optional
             The key for the weight encoded in the edges to be used.
-        path_start :: int, optional
+        path_start : int, optional
             An index of the first returned path, by default 0
 
         Returns
         -------
         List[List[str]]
             List of paths, each path consisting of a list of nodes.
         """
@@ -361,40 +434,46 @@
 
     def set_start_conditions(self, conditions: Dict[str, float]):
         """
         Add the IDs of the start compounds to self.start_compounds and add entries for cost in self.compound_cost.
 
         Parameters
         ----------
-        conditions :: Dict[str float]
+        conditions : Dict[str float]
             The IDs of the compounds as keys and its given cost as values.
         """
         # # # Reset Start conditions, if already set previously
         if self.start_compounds_set:
+            # # # Reset 'weight' if compound costs were solved
+            if self.graph_updated_with_compound_costs:
+                self.reset_graph_compound_costs()
+            # # # Reset compound costs and start compounds
             self.compound_costs = {}
             self.start_compounds = []
+            self.compound_costs_solved = False
+            self.graph_updated_with_compound_costs = False
         # # # Loop over conditions and set them
         for cmp_id, cmp_cost in conditions.items():
             self.compound_costs[cmp_id] = cmp_cost
             self.start_compounds.append(cmp_id)
         self.start_compounds_set = True
 
     def __weight_func(self, u: str, _: str, d: Dict):
         """
         Calculates the weight of the edge d connecting u with _ (directional!).
         Only consider the costs of the required compounds if the edge d is from a compound node to a reaction node.
         If the edge d connects a reaction node with a compound node, the returned weight should be 0.
 
         Parameters
         ----------
-        u :: str
+        u : str
             The ID of start node.
-        _ :: str
+        _ : str
             The ID of end node.
-        d :: Dict
+        d : Dict
             The edge connecting u and _ as dictionary
 
         Returns
         -------
         float
             Sum over the edge weight and the costs of the required compounds.
         """
@@ -413,19 +492,17 @@
 
     def calculate_compound_costs(self, recursive: bool = True):
         """
         Determine the cost for all compounds via determining their shortest paths from the ``start_compounds``.
         If this succeeds, set ``compound_costs_solved`` to ``True``. Otherwise it stays ``False``.
 
         The algorithm works as follows:
-        Given the starting conditions, one loops over the individual starting compounds as long as:\n
-
-        - the ``_pseudo_inf`` entries in ``compound_costs`` are reduced
-        - for any entry in ``compounds_cost`` a lower cost is found
-
+        Given the starting conditions, one loops over the individual starting compounds as long as:
+        - the self._pseudo_inf entries in self.compound_costs are reduced
+        - for any entry in self.compounds_cost a lower cost is found
         With each starting compound, one loops over compounds which have yet no cost assigned.
         For each start - target compound pair, the shortest path is determined employing Dijkstra's algorithm.
         The weight function checks the ``weight`` of the edges as well as the costs of the required compounds listed in
         the ``required_compounds`` of the traversed edges.
         If the path exceeds the length of self._pseudo_inf, this path is not considered for further evaluation.
         The weight of the starting compound is added to the tmp_cost.
         If the target compound has no weight assigned yet in ``compound_costs`` OR
@@ -440,30 +517,31 @@
         Notes
         -----
         * Checks if the start compounds are set.
         * Checks if the graph contains any nodes.
 
         Parameters
         ----------
-        recursive :: bool
+        recursive : bool
             All compounds are checked for shorter paths, True by default.
             If set to False, compounds for which a cost has been determined are not checked in the next loop.
         """
         assert self.graph_handler
         if not self.start_compounds_set:
-            raise RuntimeError("No start conditions given")
+            raise RuntimeError("No start conditions given.")
         if len(self.graph_handler.graph.nodes) == 0:
-            raise RuntimeError("No nodes in graph")
+            raise RuntimeError("No nodes in graph.")
         cmps_to_check = [n for n in self.graph_handler.graph.nodes if ';' not in n
                          and n not in self.start_compounds]
         # # # Set all compounds to be checked to pseudo inf cost
         for cmp_id in cmps_to_check:
             self.compound_costs[cmp_id] = self._pseudo_inf
         # # # Dictionary for current run
         tmp_compound_costs: Dict[str, float] = {}
+        no_path_to_cmps = list()
         # # # Determine convergence variables for while loop
         current_inf_count = sum(value == self._pseudo_inf for value in self.compound_costs.values())
         prev_inf_count = current_inf_count
         # # # Convergence criteria
         compound_costs_change = None
         compound_costs_opt_change = 1
         converged = False
@@ -471,16 +549,28 @@
         while (not converged):
             compound_costs_opt_change = 0
             print("Remaining Nodes:", len(cmps_to_check))
             for tmp_start_node in self.start_compounds:
                 # # # Loop over all nodes to be checked starting from start nodes
                 for target in cmps_to_check:
                     # # # Determine cost and path with dijkstra's algorithm
-                    tmp_cost, _ = nx.single_source_dijkstra(self.graph_handler.graph, tmp_start_node, target,
-                                                            cutoff=None, weight=self.__weight_func)
+                    try:
+                        tmp_cost, _ = nx.single_source_dijkstra(self.graph_handler.graph, tmp_start_node, target,
+                                                                cutoff=None, weight=self.__weight_func)
+                    # # # Catch nodes with no paths, remove them from compounds to check list
+                    except nx.NetworkXNoPath as error:
+                        print(error.__str__()[:-1] + " from " + tmp_start_node + ".")
+                        # # # Remove target if no way found from other starting compounds
+                        if (target not in tmp_compound_costs.keys()) and \
+                           (self.compound_costs[target] == self._pseudo_inf) and \
+                           (tmp_start_node == self.start_compounds[-1]):
+                            print("Removing " + target + " from compounds to check.")
+                            # # # Append target to be removed
+                            no_path_to_cmps.append(target)
+                        continue
                     # # # Check if the obtained cost is larger than infinity (pseudo_inf)
                     # # # and continue with the next target if this is the case
                     if (tmp_cost - self._pseudo_inf) > 0.0:
                         continue
                     # # # Add cost of the starting node
                     tmp_cost += self.compound_costs[tmp_start_node]
                     # # # Check for value in compound_costs dict and
@@ -491,14 +581,18 @@
                     if self.compound_costs[target] == self._pseudo_inf or (
                             self.compound_costs != self._pseudo_inf and 10e-6 < self.compound_costs[target] - tmp_cost):
                         # # # Not discovered in current run OR new tmp cost lower than stored cost
                         if (target not in tmp_compound_costs.keys()):
                             tmp_compound_costs[target] = tmp_cost
                         elif (tmp_cost < tmp_compound_costs[target]):
                             tmp_compound_costs[target] = tmp_cost
+                # # # Remove targets for no path could be found
+                for cmp in no_path_to_cmps:
+                    cmps_to_check.remove(cmp)
+                no_path_to_cmps = list()
             # # # Write obtained compound_costs to overall dictionary
             for key, value in tmp_compound_costs.items():
                 self.compound_costs[key] = value
                 # # # Remove found nodes if recursive is false
                 if not recursive:
                     cmps_to_check.remove(key)
             # # # Reset tmp_pr_cost
@@ -527,59 +621,125 @@
         The edges of the resulting graph contain a weight including the required_compound_costs based on the starting
         conditions.
         All analysis of the graph therefore depend on the starting conditions.
 
         Notes
         -----
         * Checks if the compound costs have successfully been determined.
+        * Checks if the graph has been updated with the compound costs.
         """
 
         # # # Check if all costs are available
         if not self.compound_costs_solved:
-            unsolved_cmp = [key for key, _ in self.compound_costs.items()]
-            raise RuntimeError("The following cmp have no cost assigned:\n" + str(unsolved_cmp) +
-                               "\nReconsider the starting conditions.")
+            unsolved_cmp = [key for key, value in self.compound_costs.items() if value == self._pseudo_inf]
+            sys.stderr.write("Warning: The following compounds have no cost assigned:\n" + str(unsolved_cmp) +
+                             "\nGraph will be updated anyway, but maybe reconsider the starting conditions.\n")
+        # # # Check if graph has been updated
+        if self.graph_updated_with_compound_costs:
+            raise Warning("The graph has been updated previously.")
         # # # Reset unique_iterator_list as graph changes
         self._reset_iterator_memory()
         for node in self.compound_costs.keys():
             # # # Loop over all edges of compound and manipulate weight
             for target_node, attributes in self.graph_handler.graph[node].items():
                 required_compound_costs = np.asarray([self.compound_costs[k] for k in attributes['required_compounds']])
                 tot_required_compound_costs = np.sum(required_compound_costs)
                 # # # Set required compound costs in edge
                 self.graph_handler.graph.edges[node,
                                                target_node]['required_compound_costs'] = tot_required_compound_costs
                 # # # Add required compound costs to weight
                 self.graph_handler.graph.edges[node, target_node]['weight'] += tot_required_compound_costs
+        # # # Set bool for update
+        self.graph_updated_with_compound_costs = True
+
+    def reset_graph_compound_costs(self):
+        """
+        Reset the 'weight' of edges from compound to reaction nodes by subtracting the required compound costs.
+        Allows to re-calculate the compound costs under different starting conditions.
+
+         Notes
+        -----
+        * Checks if the compound costs have successfully been determined.
+        """
+        if not self.graph_updated_with_compound_costs:
+            raise RuntimeError("Graph not updated with compound costs.")
+        for node in self.compound_costs.keys():
+            # # # Loop over all edges of compound and manipulate weight
+            for target_node in self.graph_handler.graph[node].keys():
+                # # # Get required compound costs from edge
+                tot_required_compound_costs = self.graph_handler.graph.edges[node,
+                                                                             target_node]['required_compound_costs']
+                # # # Subtract required compound costs from weight
+                self.graph_handler.graph.edges[node, target_node]['weight'] -= tot_required_compound_costs
+                # # # Set required compound costs back to 0.0
+                self.graph_handler.graph.edges[node, target_node]['required_compound_costs'] = 0.0
+        # # # Reset bools for compound costs
+        self.compound_costs_solved = False
+        self.graph_updated_with_compound_costs = False
+
+    def export_graph(self, filename: str = "graph.json"):
+        """
+        Export graph as dictionary to .json file.
+
+        Parameters
+        ----------
+        filename : str, optional
+            Name of the file to write graph into, by default "graph.json".
+        """
+        assert self.graph_handler
+        graph_as_dict = nx.convert.to_dict_of_dicts(self.graph_handler.graph)
+        # # # Add node type to dictionary
+        for node in self.graph_handler.graph.nodes:
+            graph_as_dict[node]['type'] = self.graph_handler.graph.nodes[node]['type']
+        with open(filename, 'w') as f:
+            json.dump(graph_as_dict, f, indent=4)
+
+    def export_compound_costs(self, filename: str = "compound_costs.json"):
+        """
+        Export the compound cost dictionary to a .json file.
+
+        Parameters
+        ----------
+        filename : str, optional
+            Name of the file to write compound costs into, by default "compound_costs.json"
+        """
+        assert len(self.compound_costs) > 0
+        with open(filename, 'w') as f:
+            json.dump(self.compound_costs, f, indent=4)
 
-    # Base Class for adding a reaction; up weight to rxn node is just one per default, no further info
     class BasicHandler:
         """
         A basic class to handle the construction of the nx.DiGraph.
         A list of reactions can be added differently, depending on the implementation of ``_get_weight`` and
         ``get_valid_reaction_ids``.
 
         Attributes
         ----------
-        graph :: nx.DiGraph
+        graph : nx.DiGraph
             The directed graph.
-        db_manager :: db.Manager
+        db_manager : db.Manager
             The database manager for the connected database.
-        barrierless_weight :: float
+        barrierless_weight : float
             The weight to be set for barrierless reactions.
-        model :: Union[None, db.Model]
+        model : Union[None, db.Model]
             A model for filtering the valid reactions.
             Per default None, reactions are included regardless of the model.
         """
 
-        def __init__(self, manager: db.Manager, model: db.Model = None):
+        def __init__(self, manager: db.Manager, model: Optional[db.Model] = None,
+                     structure_model: Optional[db.Model] = None):
             self.graph = nx.DiGraph()
             self.db_manager = manager
             self.barrierless_weight = 1.0
             self.model: Union[None, db.Model] = model
+            self.filter_negative_barriers = False
+            self.use_structure_model = False
+            self.structure_model: Union[None, db.Model] = structure_model
+            if self.structure_model is not None:
+                self.use_structure_model = True
             # Collections
             self._compounds = self.db_manager.get_collection("compounds")
             self._flasks = self.db_manager.get_collection("flasks")
             self._structures = self.db_manager.get_collection("structures")
             self._properties = self.db_manager.get_collection("properties")
             self._reactions = self.db_manager.get_collection("reactions")
             self._elementary_steps = self.db_manager.get_collection("elementary_steps")
@@ -603,29 +763,33 @@
             | D -> R\\ :sub:`2` -> B
 
             Representing this reaction in the graph yields 4 compound nodes,
             2 reaction nodes (same reaction) and 16 edges (2*2*2*2).
             The weights assigned to the edges depends on the ``_get_weight`` implementation.
 
             The edges from a compound node to a reaction node contain several information:
-                :weight: the weight of the edge
-                        1.0 if the reaction is not barrierless, otherwise it is set to ``barrierless_weight``
-                :required_compounds: the IDs of the other reagents of this side of the reaction in a list
-                :required_compound_costs: the sum over all compound costs of the compounds in the ``required_compounds``
-                                          list.
-                                          None by default.
+                weight:
+                the weight of the edge
+                1 if the reaction is not barrierless, otherwise it is set to self.barrierless_weight
+                required_compounds:
+                the IDs of the other reagents of this side of the reaction in a list
+                required_compound_costs:
+                the sum over all compound costs of the compounds in the required_compounds list
+                None by default
 
             The edges from a reaction node to a compound node contain several information:
-                :weight: the weight of the edge, set to 0.0
-                :required_compounds: the IDs of the other products emerging;
-                                        added for easier information extraction during the path analysis
+                weight:
+                the weight of the edge, set to 0
+                required_compounds:
+                the IDs of the other products emerging;
+                added for easier information extraction during the path analysis
 
             Parameters
             ----------
-            reaction :: db.Reaction
+            reaction : db.Reaction
                 The reaction to be added to the graph.
             """
             # Add two rxn nodes
             rxn_nodes = []
             reaction_id = reaction.id().string()
 
             for i in range(0, 2):
@@ -669,15 +833,15 @@
 
         def _get_weight(self, reaction: db.Reaction) -> Tuple[float, float]:
             """
             Determining the weights for the edges of the given reaction.
 
             Parameters
             ----------
-            reaction :: db.Reaction
+            reaction : db.Reaction
                 Reaction of interest
 
             Returns
             -------
             Tuple[float, float]
                 Weight for connections to the LHS reaction node, weight for connections to the RHS reaction node
             """
@@ -705,121 +869,171 @@
 
         def _valid_reaction(self, reaction: db.Reaction) -> bool:
             """
             Checks if a given reaction is valid.
             A reaction is considered valid if at least one elementary step of the reaction has an electronic energy
             assigned to its first structure, if required calculated with the set db.Model.
 
+            If 'use_structure_model' is set to True, the elementary steps are checked if the first structure of the
+            elementary step has the required structure model.
+
+            If 'filter_negative_barriers' is set to True, the elementary step is checked if the electronic energy
+            barrier in any direction is None or negative.
+
             Parameters
             ----------
-            reaction :: db.Reaction
-                _description_
+            reaction : db.Reaction
+                The reaction which shall be checked for one valid elementary step.
 
             Returns
             -------
             bool
                 Bool indicating if the reaction is valid.
             """
             reaction.link(self._reactions)
+
             for es_id in reaction.get_elementary_steps():
+                valid_structures = False
+                valid_barriers = True
                 es = db.ElementaryStep(es_id, self._elementary_steps)
-                first_structure_lhs = db.Structure(es.get_reactants()[0][0])
+                first_structure_lhs = db.Structure(es.get_reactants()[0][0], self._structures)
                 # # # Model Check
                 # Check if model is not specified (None)
-                if self.model is None:
-                    first_structure_lhs.link(self._structures)
+                if self.model is None:  # type: ignore
                     if len(first_structure_lhs.get_properties("electronic_energy")) > 0:
                         return True
                 # Check, if energy of this structure with specified model exists
                 else:
+                    assert self.model
+                    if self.use_structure_model:
+                        assert self.structure_model
+                    # Structure model check if wanted here, structure must have model
+                    if self.use_structure_model and \
+                       self.structure_model != first_structure_lhs.get_model():  # type: ignore
+                        # # # Skip structure if the structure model does not fit the set model
+                        continue
                     first_structure_lhs_e = get_energy_for_structure(
                         first_structure_lhs, "electronic_energy", self.model, self._structures, self._properties)
+                    # # # Structure validity check
                     if first_structure_lhs_e is not None:
+                        valid_structures = True
+                    if self.filter_negative_barriers:
+                        barriers = get_barriers_for_elementary_step_by_type(es, "electronic_energy", self.model,
+                                                                            self._structures, self._properties)
+                        if None in barriers or (barriers[0] < 0.0 or barriers[1] < 0.0):  # type: ignore
+                            valid_barriers = False
+                    # # # Final structure and barrier check
+                    if valid_structures and valid_barriers:
                         return True
             # If all elementary steps of this reaction fail the checks, this reaction is not valid
             return False
 
     class BarrierBasedHandler(BasicHandler):
         """
         A class derived from the basic graph handler class to encode the reaction barrier information in the edges.
         The barriers of the elementary step with the minimal TS energy of a reaction are employed.
         The barriers are converted to rate constants, normalized over all rate constants in the graph and then the cost
         function :math:`|log(normalized\\ rate\\ constant)|` is applied to obtain the weight.
 
         Attributes
         ----------
-        temperature :: float
+        temperature : float
             The temperature for calculating the rate constants from the barriers. Default is 298.15 K.
-        _rate_constant_normalization :: float
+        _rate_constant_normalization : float
             The factor to normalize the rate constant.
-        _rxn_to_es_map :: Dict[str, db.ID]
+        _rxn_to_es_map : Dict[str, db.ID]
             A dictionary holding the ID of the elementary step with the lowest TS energy for each reaction.
         """
 
-        def __init__(self, db_manager: db.Manager, model: db.Model):
-            super().__init__(db_manager, model)
+        def __init__(self, db_manager: db.Manager, model: db.Model, structure_model: Union[None, db.Model] = None):
+            super().__init__(db_manager, model, structure_model)
             self.temperature = 298.15
+            self.check_barriers = False
             self._rate_constant_normalization = 1.0
             self._rxn_to_es_map: Dict[str, db.ID] = {}
 
         def set_temperature(self, temperature: float):
             """
             Setting the temperature for determining the rate constants.
 
             Parameters
             ----------
-            temperature :: float
+            temperature : float
                 The temperature in Kelvin.
             """
             self.temperature = temperature
 
         def get_temperature(self):
             """
             Gets the set temperature.
 
             Returns
             -------
-            self.temperature :: float
+            self.temperature : float
                 The set temperature.
             """
             return self.temperature
 
+        def get_valid_reaction_ids(self):
+            return [db.ID(key) for key in self._rxn_to_es_map.keys()]
+
+        def _get_valid_reaction_ids(self):
+
+            valid_ids: List[db.ID] = list()
+            for reaction in self._reactions.iterate_all_reactions():
+                if self._valid_reaction(reaction):
+                    valid_ids.append(reaction.id())
+            return valid_ids
+
         def _map_elementary_steps_to_reactions(self):
             """
             Loop over all reactions to get the elementary step with the lowest TS energy for each reaction.
             The corresponding db.ID of the elementary step is written to the _rxn_to_es_map.
             """
-            for reaction_id in self.get_valid_reaction_ids():
+            for reaction_id in self._get_valid_reaction_ids():
                 reaction = db.Reaction(reaction_id, self._reactions)
                 # # # Go for gibbs energy first
-                es_id = get_elementery_step_with_min_ts_energy(
+                es_id = get_elementary_step_with_min_ts_energy(
                     reaction,
                     "gibbs_free_energy",
                     self.model,
                     self._elementary_steps,
                     self._structures,
-                    self._properties)
+                    self._properties,
+                    self.structure_model)
                 # # # If unsuccessful, attempt electronic energy
                 if es_id is None:
-                    es_id = get_elementery_step_with_min_ts_energy(
+                    es_id = get_elementary_step_with_min_ts_energy(
                         reaction,
                         "electronic_energy",
                         self.model,
                         self._elementary_steps,
                         self._structures,
-                        self._properties)
+                        self._properties,
+                        self.structure_model)
+                    # # # If es_id still None, continue; pure safety measure
+                    if es_id is None:
+                        continue
+                # Enforce non-negative barriers
+                if self.filter_negative_barriers:
+                    es = db.ElementaryStep(es_id, self._elementary_steps)
+                    barriers = get_barriers_for_elementary_step_by_type(es, "electronic_energy", self.model,
+                                                                        self._structures, self._properties)
+                    if None in barriers or (barriers[0] < 0.0 or barriers[1] < 0.0):
+                        es_id = self._get_elementary_step_with_min_ts_energy_and_non_negative_barriers(reaction)
                 # # # Write elementary step to map
                 self._rxn_to_es_map[reaction_id.string()] = es_id
 
         def _calculate_rate_constant_normalization(self):
             """
             Determine the rate constant normalization factor for calculating the edge weights.
             Loops over the _rxn_to_es_map, converts every barrier to the rate constant and adds it to the sum of rate
             constants.
             For barrierless elementary steps, twice the barrierless_weight is added.
+            For elementary steps with negative barriers, for the negative barrier(s) the barrierless_weight is added.
 
             The rate constant normalization is then the inverse of the final sum.
             """
 
             k_sum = 0.0
 
             for es_id in self._rxn_to_es_map.values():
@@ -829,35 +1043,45 @@
                 else:
                     # # # Retrieve barriers of elementary step in kJ/mol
                     barriers = get_barriers_for_elementary_step_by_type(
                         es, "gibbs_free_energy", self.model, self._structures, self._properties)
                     if None in barriers:
                         barriers = get_barriers_for_elementary_step_by_type(
                             es, "electronic_energy", self.model, self._structures, self._properties)
-                    k_lhs = rate_constant_from_barrier(barriers[0], self.temperature)
-                    k_rhs = rate_constant_from_barrier(barriers[1], self.temperature)
+                    # # # Use user defined barrierless weight for negative barriers
+                    # Check LHS Barrier
+                    if barriers[0] < 0.0:
+                        k_lhs = self.barrierless_weight
+                    else:
+                        k_lhs = rate_constant_from_barrier(barriers[0], self.temperature)
+                    # Check RHS Barrier
+                    if barriers[1] < 0.0:
+                        k_rhs = self.barrierless_weight
+                    else:
+                        k_rhs = rate_constant_from_barrier(barriers[1], self.temperature)
                     k_sum += k_lhs + k_rhs
 
-            self._rate_constant_normalization = 1 / k_sum
+            if k_sum != 0.0:
+                self._rate_constant_normalization = 1 / k_sum
 
         def _get_weight(self, reaction: db.Reaction) -> Tuple[float, float]:
             """
             Determines the weight for a given reaction.
             The weight is calculated by determining the rate constant from the barrier, normalizing the constant with
             the rate_constant_normalization and taking the abs(log()) of the corresponding product.
-            For barrierless reactions, the barrierless_weight is taken as rate constants.
+            For barrierless reactions and negative barriers, the barrierless_weight is taken as rate constants.
 
             Parameters
             ----------
-            reaction :: db.Reaction
+            reaction : db.Reaction
                The reaction for which the weights should be determined.
 
             Returns
             -------
-            weights :: Tuple(float, float)
+            weights : Tuple(float, float)
                 The weight for the LHS -> RxnNode and  for the RHS -> RxnNode.
             """
             # # # Look up elementary step id for reaction
             es_id = self._rxn_to_es_map[reaction.id().string()]
             es_step = db.ElementaryStep(es_id, self._elementary_steps)
             # # # Barrierless weights for barrierless reactions
             if es_step.get_type() == db.ElementaryStepType.BARRIERLESS:
@@ -868,12 +1092,69 @@
                 # # # Retrieve barriers of elementary step in kJ/mol
                 barriers = get_barriers_for_elementary_step_by_type(
                     es_step, "gibbs_free_energy", self.model, self._structures, self._properties)
                 if None in barriers:
                     barriers = get_barriers_for_elementary_step_by_type(
                         es_step, "electronic_energy", self.model, self._structures, self._properties)
                 assert barriers[0]
-                k_lhs = rate_constant_from_barrier(barriers[0], self.temperature)
-                k_rhs = rate_constant_from_barrier(barriers[1], self.temperature)
+                # Check LHS Barrier
+                if barriers[0] < 0.0:
+                    k_lhs = self.barrierless_weight
+                else:
+                    k_lhs = rate_constant_from_barrier(barriers[0], self.temperature)
+                # Check RHS Barrier
+                if barriers[1] < 0.0:
+                    k_rhs = self.barrierless_weight
+                else:
+                    k_rhs = rate_constant_from_barrier(barriers[1], self.temperature)
 
             return abs(np.log(k_lhs * self._rate_constant_normalization)), \
                 abs(np.log(k_rhs * self._rate_constant_normalization))
+
+        def _get_elementary_step_with_min_ts_energy_and_non_negative_barriers(self, reaction: db.Reaction):
+            """
+            Gets the elementary step ID with the lowest energy of the corresponding transition state
+            of a valid reaction, without a negative barrier in the forward and backward directions.
+
+            Parameters
+            ----------
+            reaction : db.Reaction
+                The reaction for which the elementary steps shall be analyzed.
+
+            Returns
+            -------
+            elementary_step_id : db.ID
+                The ID of the elementary step with the lowest TS energy without negative barriers.
+            """
+            # # # Get all es steps of the reaction
+            el_steps = reaction.get_elementary_steps()
+            es_data: List[Tuple[float, float, float, db.ID]] = list()
+            assert self.model
+            if self.use_structure_model:
+                assert self.structure_model
+            # # # Loop over the steps and retrieve TS energy and barrier information
+            for es_id in el_steps:
+                es = db.ElementaryStep(es_id, self._elementary_steps)
+                barriers = get_barriers_for_elementary_step_by_type(
+                    es, "electronic_energy", self.model, self._structures, self._properties)
+                if None in barriers:
+                    continue
+                # # # Check for mypy
+                assert barriers[0] is not None and barriers[1] is not None
+                if es.get_type() == db.ElementaryStepType.BARRIERLESS:
+                    return es_id
+                # # # TS Retrieval and check structure model
+                ts = db.Structure(es.get_transition_state(), self._structures)
+                if self.use_structure_model and ts.get_model() != self.structure_model:  # type: ignore
+                    continue
+                ts_energy = get_energy_for_structure(
+                    ts, "electronic_energy", self.model, self._structures, self._properties)
+                # # # Check for mypy
+                assert ts_energy is not None
+                # # # Append tuple of ts energy, lhs barrier, rhs barrier and id to list
+                es_data.append((ts_energy, barriers[0], barriers[1], es_id))  # type: ignore
+            # # # Sort the es data by lowest TS energy
+            es_data_sorted = [item for item in sorted(es_data, key=lambda item: item[0])]
+            # # # Return first elementary step id where all barriers are positive (> 0.0)
+            for data in es_data_sorted:
+                if data[1] > 0.0 and data[2] > 0.0:
+                    return data[3]
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/refinement.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/refinement.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,26 +6,29 @@
 """
 
 # Standard library imports
 from collections import Counter
 from json import dumps
 from typing import Dict, List, Tuple, Union, Set, Optional
 from warnings import warn
+import os
+import pickle
 
 # Third party imports
 import scine_database as db
 import scine_utilities as utils
 
 # Local application imports
 from ..gears import Gear
 from ..utilities.queries import (
     identical_reaction,
     model_query,
     stop_on_timeout,
-    get_calculation_id_from_structure
+    get_calculation_id_from_structure,
+    query_calculation_in_id_set
 )
 from ..utilities.energy_query_functions import get_energy_for_structure, get_barriers_for_elementary_step_by_type
 from ..utilities.calculation_creation_helpers import finalize_calculation
 
 
 class NetworkRefinement(Gear):
     """
@@ -46,25 +49,25 @@
       'refine_optimizations'
         New optimizations of all minima and TS in the network with the refinement model.
         Minima are checked via the CompoundGear to be within the same compound
         TS should be checked for validity with an IRC within the optimization job in Puffin
       'double_ended_refinement'
         Check successful single ended react jobs and try to find a TS for these reactions with a double ended search
       'double_ended_new_connections'
-        Check structures of same PES without a unimolecular reaction combining their compounds to be connected via a
+        Check structures of same PES without an unimolecular reaction combining their compounds to be connected via a
         double ended search. This can also be done with the same model with which the structures were generated.
       'refine_single_ended_search'
         Perform single ended searches again with the refinement model, if they were already successful with a different
         model. Equality of products is not checked.
       'refine_structures_and_irc'
         Perform single ended searches again starting with the transition state of the previous transition state
         search.
     """
 
-    class Options:
+    class Options(Gear.Options):
         """
         The options for the NetworkRefinement Gear.
         """
 
         __slots__ = (
             "cycle_time",
             "pre_refine_model",
@@ -83,20 +86,25 @@
             "single_ended_job",
             "single_ended_job_settings",
             "single_ended_step_refinement_job",
             "single_ended_step_refinement_settings",
             "max_barrier",
             "exclude_barrierless",
             "transition_state_energy_window",
+            "refine_n_per_reaction",
             "reaction_based_loop",
             "jobs_to_wait_for",
-            "caching_file_name"
+            "caching_file_name",
+            "manual_reaction_selection",
+            "reaction_ids_to_refine",
+            "elementary_step_index_file_name"
         )
 
         def __init__(self):
+            super().__init__()
             self.cycle_time = 101
             """
             int
                 The minimum number of seconds between two cycles of the Gear.
                 Cycles are finished independent of this option, thus if a cycle
                 takes longer than the cycle_time will effectively lead to longer
                 cycle times and not cause multiple cycles of the same Gear.
@@ -191,15 +199,15 @@
             """
             self.tsopt_job_settings: utils.ValueCollection = utils.ValueCollection()
             """
             utils.ValueCollection
                 Additional settings for optimizing all transition states.
                 Empty by default.
             """
-            self.double_ended_job: db.Job = db.Job("scine_react_double_ended")  # TODO Write puffin job
+            self.double_ended_job: db.Job = db.Job("scine_bspline_optimization_job")
             """
             db.Job (Scine::Database::Calculation::Job)
                 The Job used for searching for a transition state between two compounds.
                 The default is: the 'scine_react_double_ended' order on a single core.
             """
             self.double_ended_job_settings: utils.ValueCollection = utils.ValueCollection()
             """
@@ -245,14 +253,19 @@
             """
             self.transition_state_energy_window = 1000.0
             """
             float
                 Energy window for the elementary step selection in kJ/mol for reaction based refinement
                 (see reaction_based_loop).
             """
+            self.refine_n_per_reaction = 1000
+            """
+            int
+                The maximum number of elementary steps to refine for a given reaction.
+            """
             self.reaction_based_loop = False
             """
             bool
                 If true, the elementary steps are traversed reaction wise and the elementary
                 steps that are refined can be narrowed down by the transition_state_energy_window, e.g.,
                 transition states with an energy higher than this window with respect to the lowest
                 energy transition state for the reaction are not considered.
@@ -263,29 +276,45 @@
                 Wait for these jobs to finish for each reaction before setting up reaction-wise refinement calculations.
             """
             self.caching_file_name = ".chemoton_refinement_calculation_id_cache.pickle"
             """
             str
                 The name of the file used to save the already considered calculation ids.
             """
+            self.manual_reaction_selection = False
+            """
+            bool
+                If true the list "reaction_ids_to_refine" is used to select the reactions to refine. By default, False.
+            """
+            self.reaction_ids_to_refine = list()
+            """
+            List[db.ID]
+                A list of reaction ids which should be refined if a manual selection is required. By default an empty
+                list.
+            """
+            self.elementary_step_index_file_name = ".chemoton_refinement_elementary_step_index.pickle"
+            """
+            str
+                The file name for the elementary step index.
+            """
 
     def __init__(self):
         super().__init__()
-        self.options = self.Options()
         self._required_collections = ["calculations", "compounds", "elementary_steps", "flasks", "reactions",
                                       "properties", "structures"]
         self._calculation_id_cache = {
             "refine_single_points": set(),
             "refine_optimizations": set(),
             "double_ended_refinement": set(),
             "double_ended_new_connections": set(),
             "refine_single_ended_search": set(),
             "refine_structures_and_irc": set(),
         }
         self._lhs_optimization_calculations = dict()
+        self._elementary_step_to_calculation_map: Dict[str, str] = dict()
 
     def _loop_impl(self):
         if self.options.pre_refine_model == self.options.post_refine_model and (
             sum(self.options.refinements.values()) != 1 or not self.options.refinements["double_ended_new_connections"]
         ) and not (self.options.use_calculation_model and
                    self.options.calculation_model != self.options.pre_refine_model):
             # new_connections would make sense to have identical model --> allow it if this is the only activated
@@ -294,40 +323,74 @@
             raise RuntimeError("pre_refine_model and post_refine_model must be different!")
         if self.options.refinements["refine_single_points"]:
             self._loop_steps("refine_single_points")
         if self.options.refinements["refine_optimizations"]:
             warn("WARNING: optimized TS verification after refinement is not implemented by default, yet")
             self._loop_steps("refine_optimizations")
         if self.options.refinements["double_ended_refinement"]:
-            warn("WARNING: double ended job is not implemented by default, yet")
+            # warn("WARNING: double ended job is not implemented by default, yet")
             self._loop_steps("double_ended_refinement")
         if self.options.refinements["double_ended_new_connections"]:
             warn("WARNING: double ended job is not implemented by default, yet")
             self._double_ended_new_connections_loop()
         if self.options.refinements["refine_single_ended_search"]:
             self._loop_steps("refine_single_ended_search")
         if self.options.refinements["refine_structures_and_irc"]:
             self._loop_steps("refine_structures_and_irc")
 
     def _loop_steps(self, job_label: str):
-        if self.options.reaction_based_loop:
+        if self.options.reaction_based_loop or self.options.manual_reaction_selection:
             self._loop_reactions_with_barrier_screening(job_label)
         else:
             self._loop_elementary_step_with_barrier_screening(job_label)
 
     def _refine_existing_react_jobs(
-        self, job: db.Job, settings: utils.ValueCollection, keys_to_take_over: List[str], add_products: bool,
-            structure_ids, old_settings, products
+        self, job: db.Job, settings: utils.ValueCollection, keys_to_take_over: List[str],
+            structure_ids, old_settings, elementary_step=None
     ):
         new_settings = utils.ValueCollection({k: v for k, v in old_settings.items() if k in keys_to_take_over})
         # add new settings defined for refinement
         new_settings.update(settings.as_dict())
-        if add_products:
-            new_settings.update({"bspline_bspline_products": [str(sid) for sid in products]})
-            structure_ids += products
+        if elementary_step:
+            if elementary_step.get_type() != db.ElementaryStepType.REGULAR:
+                return
+            transition_state_id = elementary_step.get_transition_state()
+            auxiliaries = {"transition-state-id": transition_state_id,
+                           "elementary-step-id": elementary_step.id()}
+
+            transition_state = db.Structure(transition_state_id, self._structures)
+            # Check if the calculation already exists. If so, it will have an entry on the transition state of the
+            # elementary step. This calculation is uniquely defined by
+            # 1. The fact that it is assigned to the TS.
+            # 2. The model.
+            # 3. The job order
+            # 4. The settings + auxiliaries.
+            calc_id_strs = set([c_id.string() for c_id in transition_state.query_calculations(
+                job.order, self.options.post_refine_model, self._calculations)])
+            calc_ids = query_calculation_in_id_set(calc_id_strs, 2, self._calculations,
+                                                   settings=new_settings, auxiliaries=auxiliaries)
+            if not calc_ids:
+                spline = elementary_step.get_spline()
+                _, atoms_start = spline.evaluate(0)
+                _, atoms_end = spline.evaluate(1)
+                model = transition_state.get_model()
+                charge = transition_state.get_charge()
+                spin = transition_state.get_multiplicity()
+                step_reactants = elementary_step.get_reactants(db.Side.BOTH)
+                reactant_label = db.Label.COMPLEX_GUESS if len(step_reactants[0]) > 1 else db.Label.MINIMUM_GUESS
+                product_label = db.Label.COMPLEX_GUESS if len(step_reactants[1]) > 1 else db.Label.MINIMUM_GUESS
+
+                reactant_structure = db.Structure.make(atoms_start, charge, spin, model, reactant_label,
+                                                       self._structures)
+                product_structure = db.Structure.make(atoms_end, charge, spin, model, product_label, self._structures)
+                calc_id = self._create_refinement_calculation([reactant_structure.id(), product_structure.id()], job,
+                                                              new_settings, auxiliaries)
+                transition_state.add_calculation(job.order, calc_id)
+            return
+
         if not self._refinement_calculation_already_setup(structure_ids, job, new_settings):
             self._create_refinement_calculation(structure_ids, job, new_settings)
 
     def _refine_structures_and_irc(self, structure_ids, ts_id, old_settings):
         new_settings = utils.ValueCollection({k: v for k, v in old_settings.items()})
         # add new settings defined for refinement
         new_settings.update(self.options.single_ended_step_refinement_settings.as_dict())
@@ -342,15 +405,16 @@
     def _refine_single_points(self, structure_ids):
         for structure in structure_ids:
             # Check if a calculation for this is already scheduled
             already_set_up = self._refinement_calculation_already_setup(
                 [structure], self.options.sp_job, self.options.sp_job_settings
             )
             if not already_set_up:
-                self._create_refinement_calculation([structure], self.options.sp_job, self.options.sp_job_settings)
+                _ = self._create_refinement_calculation([structure], self.options.sp_job,
+                                                        self.options.sp_job_settings)
 
     def _refine_optimizations(self, structure_ids):
         calculation_ids = list()
         for sid in structure_ids:
             structure = db.Structure(sid, self._structures)
             structure.link(self._structures)
             refine_job, refine_settings = self._get_opt_refinement(structure.get_label())
@@ -375,14 +439,17 @@
                     ]
                 },
                 {"aggregate": {"$ne": ""}},
             ]
             + model_query(self.options.pre_refine_model)
         }
         for structure_i in stop_on_timeout(iter(self._structures.query_structures(dumps(selection_i)))):
+            if self.stop_at_next_break_point:
+                return
+
             structure_i.link(self._structures)
             aggregate_i = structure_i.get_aggregate()
             # get PES data
             charge = structure_i.get_charge()
             multiplicity = structure_i.get_multiplicity()
             atoms_i = structure_i.get_atoms()
             n_atoms = len(atoms_i)
@@ -431,27 +498,27 @@
                     self._create_refinement_calculation(
                         [structure_i.id(), structure_j.id()],
                         self.options.double_ended_job,
                         self.options.double_ended_job_settings,
                     )
 
     def _create_refinement_calculation(self, structure_ids: List[db.ID], job: db.Job, settings: utils.ValueCollection,
-                                       auxiliaries: dict = None) -> db.ID:
+                                       auxiliaries: Optional[dict] = None) -> db.ID:
         calc = db.Calculation()
         calc.link(self._calculations)
         calc.create(self.options.post_refine_model, job, structure_ids)
         if auxiliaries is not None:
             calc.set_auxiliaries(auxiliaries)
         calc.set_settings(settings)
         finalize_calculation(calc, self._structures)
         return calc.id()
 
-    def _refinement_calculation_already_setup(
-        self, structure_ids: List[db.ID], job: db.Job, settings: utils.ValueCollection, auxiliaries: dict = None
-    ) -> Union[db.ID, None]:
+    def _refinement_calculation_already_setup(self, structure_ids: List[db.ID], job: db.Job,
+                                              settings: utils.ValueCollection, auxiliaries: Optional[dict] = None) \
+            -> Union[db.ID, None]:
         return get_calculation_id_from_structure(job.order, structure_ids, self.options.post_refine_model,
                                                  self._structures, self._calculations, settings, auxiliaries)
 
     def _get_opt_refinement(self, label: db.Label) -> Tuple[db.Job, utils.ValueCollection]:
         if label == db.Label.TS_OPTIMIZED:
             return self.options.tsopt_job, self.options.tsopt_job_settings
         else:
@@ -467,65 +534,113 @@
             "rc_x_spread",
             "rc_displacement",
             "rc_spin_multiplicity",
             "rc_molecular_charge",
         ]
 
     @staticmethod
+    def _double_ended_keys_to_take_over() -> List[str]:
+        return [
+            "opt_convergence_max_iterations",
+            "opt_convergence_step_max_coefficient",
+            "opt_convergence_step_rms",
+            "opt_convergence_gradient_max_coefficient",
+            "opt_convergence_gradient_rms",
+            "opt_convergence_requirement",
+            "opt_convergence_delta_value",
+            "opt_geoopt_coordinate_system",
+            "opt_bfgs_use_trust_radius",
+            "opt_bfgs_trust_radius",
+            "ircopt_convergence_max_iterations",
+            "ircopt_convergence_step_max_coefficient",
+            "ircopt_convergence_step_rms",
+            "ircopt_convergence_gradient_max_coefficient",
+            "ircopt_convergence_gradient_rms",
+            "ircopt_convergence_requirement",
+            "ircopt_convergence_delta_value",
+            "ircopt_geoopt_coordinate_system",
+            "ircopt_bfgs_use_trust_radius",
+            "ircopt_bfgs_trust_radius",
+            "irc_convergence_max_iterations",
+            "irc_sd_factor",
+            "irc_irc_initial_step_size",
+            "irc_stop_on_error",
+            "irc_convergence_step_max_coefficient",
+            "irc_convergence_step_rms",
+            "irc_convergence_gradient_max_coefficient",
+            "irc_convergence_gradient_rms",
+            "irc_convergence_delta_value",
+            "irc_irc_coordinate_system",
+            "tsopt_convergence_max_iterations",
+            "tsopt_convergence_step_max_coefficient",
+            "tsopt_convergence_step_rms",
+            "tsopt_convergence_gradient_max_coefficient",
+            "tsopt_convergence_gradient_rms",
+            "tsopt_convergence_requirement",
+            "tsopt_convergence_delta_value",
+            "tsopt_optimizer",
+            "tsopt_geoopt_coordinate_system",
+            "tsopt_bofill_trust_radius",
+            "tsopt_bofill_follow_mode",
+        ]
+
+    @staticmethod
     def _single_ended_keys_to_take_over() -> List[str]:
         return [
             "nt_nt_rhs_list",
             "nt_nt_lhs_list",
             "nt_nt_attractive",
             "nt_nt_associations",
             "nt_nt_dissociations",
             "afir_afir_rhs_list",
             "afir_afir_lhs_list",
             "afir_afir_attractive",
             "afir_afir_use_max_fragment_distance",
         ]
 
     def _save_calculation_id_cache(self):
-        import pickle
         # save dictionary to pickle file
         with open(self.options.caching_file_name, 'wb') as file:
             pickle.dump(self._calculation_id_cache, file, protocol=pickle.HIGHEST_PROTOCOL)
 
     def _load_calculation_id_cache(self):
-        import pickle
-        import os
         if os.path.exists(self.options.caching_file_name) and os.path.getsize(self.options.caching_file_name) > 0:
             with open(self.options.caching_file_name, "rb") as file:
                 load_cache = pickle.load(file)
                 if load_cache:
                     self._calculation_id_cache.update(load_cache)
 
-    def _loop_elementary_step_with_barrier_screening(self, job_label):
+    def _loop_elementary_step_with_barrier_screening(self, job_label: str):
         """
         Create refinement calculations under the condition that there is a calculation that produced an elementary
         step with a barrier less than self.options.max_barrier.
 
         Parameters
         ----------
-        job_label: The label for the refinement to be executed.
+        job_label: str
+            The label for the refinement to be executed.
         """
         self._load_calculation_id_cache()
         cache = self._calculation_id_cache[job_label]
         model_to_search_with = self.options.pre_refine_model
         if self.options.use_calculation_model:
             model_to_search_with = self.options.calculation_model
         selection = {
             "$and": [
                 {"status": "complete"},
                 {"results.elementary_steps.0": {"$exists": True}},
             ]
-            + model_query(model_to_search_with)
+            + model_query(model_to_search_with)  # type: ignore
         }
-        cache_update = list()
+        cache_update: List[str] = list()
         for calculation in stop_on_timeout(self._calculations.iterate_calculations(dumps(selection))):
+            if self.stop_at_next_break_point:
+                cache.update(set(cache_update))
+                self._save_calculation_id_cache()
+                return
             str_id = calculation.id().string()
             if str_id in cache:
                 continue
             calculation.link(self._calculations)
             elementary_steps = [db.ElementaryStep(step_id, self._elementary_steps) for step_id in
                                 calculation.get_results().get_elementary_steps()]
             all_barrierless = True
@@ -533,62 +648,117 @@
                 if step.get_type() != db.ElementaryStepType.BARRIERLESS:
                     all_barrierless = False
             if self.options.exclude_barrierless and all_barrierless:
                 continue
             calculation_fully_done = self._set_up_calculation(job_label, calculation)
             if calculation_fully_done:
                 cache_update.append(str_id)
+
         cache.update(set(cache_update))
         self._save_calculation_id_cache()
 
+    def _create_elementary_step_index(self):
+        indexing_model = self.options.pre_refine_model
+        if self.options.use_calculation_model:
+            indexing_model = self.options.calculation_model
+        selection = {
+            "$and": [
+                {"status": "complete"},
+                {"results.elementary_steps.0": {"$exists": True}},
+            ]
+            + model_query(indexing_model)
+        }
+        self._elementary_step_to_calculation_map = dict()
+        for calculation in stop_on_timeout(self._calculations.iterate_calculations(dumps(selection))):
+            calculation.link(self._calculations)
+            self._update_elementary_step_index(calculation)
+        self._save_elementary_step_index()
+
+    def _save_elementary_step_index(self):
+        # save dictionary to pickle file
+        with open(self.options.elementary_step_index_file_name, 'wb') as file:
+            pickle.dump(self._elementary_step_to_calculation_map, file, protocol=pickle.HIGHEST_PROTOCOL)
+
+    def _load_elementary_step_index(self):
+        if os.path.exists(self.options.elementary_step_index_file_name)\
+                and os.path.getsize(self.options.elementary_step_index_file_name) > 0:
+            with open(self.options.elementary_step_index_file_name, "rb") as file:
+                load_cache = pickle.load(file)
+                if load_cache:
+                    self._elementary_step_to_calculation_map.update(load_cache)
+
+    def _update_elementary_step_index(self, calculation: db.Calculation):
+        elementary_step_ids = calculation.get_results().elementary_step_ids
+        for step_id in elementary_step_ids:
+            self._elementary_step_to_calculation_map[step_id.string()] = calculation.id().string()
+
+    def _get_calculation_id_for_step(self, elementary_step_id: db.ID) -> Optional[db.ID]:
+        if elementary_step_id.string() in self._elementary_step_to_calculation_map:
+            return db.ID(self._elementary_step_to_calculation_map[elementary_step_id.string()])
+        # TODO: This will be slow and could time out. But I do not see a better way to do it at the moment.
+        selection = {
+            "$and": [
+                {"results.elementary_steps": {"$oid": elementary_step_id.string()}}
+            ]
+        }
+        calc = self._calculations.get_one_calculation(dumps(selection))
+        if calc is None:
+            print(f"Failed to find calculation that resulted in elementary step "
+                  f"{str(elementary_step_id)}")
+            return None
+        calc.link(self._calculations)
+        self._update_elementary_step_index(calc)
+        return calc.id()
+
     def _loop_reactions_with_barrier_screening(self, job_label: str):
         """
         Create refinement calculations for only a selection of the elementary
         steps for each reaction (e.g. the most favorable one).
 
         Parameters
         ----------
         job_label: The label for the refinement to be executed.
         """
         # TODO: Maybe better some preselection or caching of already refined reaction ids?
         if self._exploration_calculations_still_running():
             return
+        # Create an elementary step id to calculation id map if necessary.
+        self._load_elementary_step_index()
+        if not self._elementary_step_to_calculation_map:
+            self._create_elementary_step_index()
+        if not self.options.manual_reaction_selection:
+            for reaction in stop_on_timeout(self._reactions.iterate_all_reactions()):
+                if self.stop_at_next_break_point:
+                    return
+                reaction.link(self._reactions)
+                self._refine_reaction(reaction, job_label)
+        else:
+            for r_id in self.options.reaction_ids_to_refine:
+                reaction = db.Reaction(r_id, self._reactions)
+                self._refine_reaction(reaction, job_label)
+        self._save_elementary_step_index()
+
+    def _refine_reaction(self, reaction: db.Reaction, job_label: str) -> None:
+        elementary_steps = self._get_all_elementary_steps(reaction)
+        if not elementary_steps:
+            return
         model_to_search_with = self.options.pre_refine_model
         if self.options.use_calculation_model:
             model_to_search_with = self.options.calculation_model
-        for reaction in stop_on_timeout(self._reactions.iterate_all_reactions()):
-            reaction.link(self._reactions)
-            elementary_steps = self._get_all_elementary_steps(reaction)
-            if not elementary_steps:
-                continue
-            eligible_steps = self._select_elementary_steps(elementary_steps)
-            for step_id in eligible_steps:
-                # TODO: This will be slow. But I do not see a better way to do it at the moment.
-                selection = {
-                    "$and": [
-                        {"results.elementary_steps": {"$oid": step_id.string()}}
-                    ] + model_query(model_to_search_with)
-                }
-                calc = self._calculations.get_one_calculation(dumps(selection))
-                if calc is None:
-                    raise RuntimeError(f"Failed to find calculation that resulted in elementary step "
-                                       f"{str(step_id)} with model {str(model_to_search_with)}")
-                self._set_up_calculation(job_label, db.Calculation(calc.id(), self._calculations))
+
+        eligible_steps = self._select_elementary_steps(elementary_steps, model_to_search_with)
+        for step_id in eligible_steps:
+            calc_id = None
+            if job_label in ["refine_structures_and_irc", "refine_single_ended_search", "double_ended_refinement"]:
+                calc_id = self._get_calculation_id_for_step(step_id)
+            if calc_id:
+                calculation = db.Calculation(calc_id, self._calculations)
+            self._set_up_calculation(job_label, calculation, step_id)
 
     def _get_job_order(self, job_label: str):
-        """
-        Resolve the job order according to the refinement task.
-        Parameters
-        ----------
-        job_label :: str
-            The refinement task.
-        Returns
-        -------
-            The puffin job order.
-        """
         if job_label == "refine_structures_and_irc":
             return self.options.single_ended_step_refinement_job.order
         elif job_label == "refine_single_points":
             return self.options.sp_job.order
         elif job_label == "refine_optimizations":
             return self.options.opt_job.order
         elif job_label == "refine_single_ended_search":
@@ -644,49 +814,67 @@
                 lhs_barrier, rhs_barrier = get_barriers_for_elementary_step_by_type(
                     elementary_step, "electronic_energy", self.options.pre_refine_model,
                     self._structures, self._properties)
                 if lhs_barrier is not None and rhs_barrier is not None:
                     elementary_steps.append(step_id)
         return elementary_steps
 
-    def _select_elementary_steps(self, elementary_steps: List[db.ID]) -> List[db.ID]:
+    def _all_structures_match_model(self, structure_ids: List[db.ID], model: db.Model) -> bool:
+        for s_id in structure_ids:
+            structure = db.Structure(s_id, self._structures)
+            structure_model = structure.get_model()
+            if structure_model != model:
+                return False
+        return True
+
+    def _select_elementary_steps(self, elementary_steps: List[db.ID], model: db.Model) -> List[db.ID]:
         """
         Select the most favorable (the lowest energy transition state) elementary step(s) for a given reaction according
         to the given energy window.
         Parameters
         ----------
         elementary_steps :: List[db.ID]
             The list of all elementary steps with the given model.
         Returns
         -------
         List[db.ID]
             The list of the selected elementary steps.
         """
         # Get minimum energy ts-elementary step + some extra
         energy_step_tuples: List[Tuple[float, db.ID]] = list()
+        structure_model = self.options.pre_refine_model
+        if self.options.use_calculation_model:
+            structure_model = self.options.calculation_model
         for step_id in elementary_steps:
             elementary_step = db.ElementaryStep(step_id, self._elementary_steps)
+            lhs_rhs_structure_ids = elementary_step.get_reactants(db.Side.BOTH)
+            if not self._all_structures_match_model(lhs_rhs_structure_ids[0] + lhs_rhs_structure_ids[1],
+                                                    structure_model):
+                continue
+            energy: Optional[float] = 0.0
             if elementary_step.get_type() != db.ElementaryStepType.BARRIERLESS:
-                ts = db.Structure(elementary_step.get_transition_state())
-                energy: Optional[float] = get_energy_for_structure(ts, "electronic_energy",
-                                                                   self.options.pre_refine_model, self._structures,
-                                                                   self._properties)
+                ts = db.Structure(elementary_step.get_transition_state(), self._structures)
+                if ts.get_model() != model:
+                    continue
+                energy = get_energy_for_structure(ts, "electronic_energy", self.options.pre_refine_model,
+                                                  self._structures, self._properties)
                 if energy is None:
                     continue
                 energy_step_tuples.append(tuple((energy, step_id)))  # type: ignore
-                break
 
         if len(energy_step_tuples) < 1:
             return []
         sorted_energy_step_tuples = sorted(energy_step_tuples, key=lambda tup: tup[0])
         minimum_energy: float = min(sorted_energy_step_tuples, key=lambda tup: tup[0])[0]
         threshold = self.options.transition_state_energy_window * utils.HARTREE_PER_KJPERMOL
-        eligible_step_ids = list()
+        eligible_step_ids = [sorted_energy_step_tuples[0][1]]
+        sorted_energy_step_tuples.pop(0)
         for energy, step_id in sorted_energy_step_tuples:
-            if abs(energy - minimum_energy) <= threshold:
+            if abs(energy - minimum_energy) < threshold\
+                    and len(eligible_step_ids) <= self.options.refine_n_per_reaction:
                 eligible_step_ids.append(step_id)
             else:
                 break
         return eligible_step_ids
 
     def _get_optimized_structure_ids(self, original_structures_ids: List[db.ID]):
         """
@@ -715,95 +903,101 @@
             if result_structures:
                 optimized_lhs_s_ids.append(result_structures[0])
         if len(optimized_lhs_s_ids) == len(original_structures_ids):
             return optimized_lhs_s_ids
         else:
             return list()
 
-    def _set_up_calculation(self, job_label: str, calculation: db.Calculation) -> bool:
+    def _all_structures_have_energy(self, structure_id_list: List[db.ID]):
+        for s_id in structure_id_list:
+            s = db.Structure(s_id)
+            energy = get_energy_for_structure(s, "electronic_energy", self.options.post_refine_model, self._structures,
+                                              self._properties)
+            if energy is None:
+                return False
+        return True
+
+    def _set_up_calculation(self, job_label: str, calculation: db.Calculation,
+                            targeted_step_id: Optional[db.ID] = None) -> bool:
         """
         Set up the refinement calculation or if needed geometry optimizations to be run before the refinement.
         Parameters
         ----------
         job_label :: str
             The job label for the refinement.
         calculation :: db.Calculation
             The original calculation that needs to be refined. Settings may be required from the calculation object.
         Returns
         -------
         bool
             Return True if the input calculation is fully handled. Returns False if the input calculation
             needs to be revisited by the gear.
         """
-        elementary_steps = [db.ElementaryStep(step_id, self._elementary_steps) for step_id in
-                            calculation.get_results().get_elementary_steps()]
+        assert calculation
+        if targeted_step_id:
+            elementary_steps = [db.ElementaryStep(targeted_step_id, self._elementary_steps)]
+        else:
+            elementary_steps = [db.ElementaryStep(step_id, self._elementary_steps) for step_id in
+                                calculation.get_results().get_elementary_steps()]
 
         transition_state_id = None
         rhs_lhs_structure_id_set: Set[str] = set()
         for elementary_step in elementary_steps:
             # If all elementary steps are sorted into a reaction, there should no duplicates be present anymore.
             # If duplicates are still there, we may waste a lot of time calculating energies/geometries etc. for
             # duplicate elementary steps.
-            if not elementary_step.has_reaction():
-                return False
+            if not elementary_step.has_reaction() or not elementary_step.analyze():
+                continue
 
             reactants = elementary_step.get_reactants(db.Side.BOTH)
             rhs_lhs_structure_id_set = rhs_lhs_structure_id_set.union(
                 set([s_id.string() for s_id in reactants[0] + reactants[1]]))
             if elementary_step.has_transition_state():
                 transition_state_id = elementary_step.get_transition_state()
                 if self._barrier_exceeded(elementary_step):
                     return True
-                if job_label == "refine_single_points":
-                    transition_state = db.Structure(transition_state_id)
-                    energy = get_energy_for_structure(transition_state, "electronic_energy",
-                                                      self.options.post_refine_model, self._structures,
-                                                      self._properties)
-                    if energy is not None:
-                        return True
-                break
 
         rhs_lhs_structure_list = [db.ID(str_id) for str_id in rhs_lhs_structure_id_set]
         if transition_state_id is not None:
             all_structure_ids_list = rhs_lhs_structure_list + [transition_state_id]
         else:
             all_structure_ids_list = rhs_lhs_structure_list
         if job_label == "refine_structures_and_irc" and transition_state_id is not None:
             reactant_structure_ids = self._get_optimized_structure_ids(calculation.get_structures())
-            if reactant_structure_ids:
-                self._refine_structures_and_irc(reactant_structure_ids, transition_state_id, calculation.get_settings())
+            if reactant_structure_ids and self._all_structures_have_graph(reactant_structure_ids):
+                self._refine_structures_and_irc(reactant_structure_ids, transition_state_id,
+                                                calculation.get_settings())
             else:
                 return False
         elif job_label == "refine_single_points":
+            if self._all_structures_have_energy(rhs_lhs_structure_list):
+                return True
             self._refine_single_points(all_structure_ids_list)
         elif job_label == "refine_optimizations":
             self._refine_optimizations(all_structure_ids_list)
         elif job_label == "refine_single_ended_search":
             reactant_structure_ids = self._get_optimized_structure_ids(calculation.get_structures())
             if reactant_structure_ids and self._all_structures_have_graph(reactant_structure_ids):
                 self._refine_existing_react_jobs(self.options.single_ended_job, self.options.single_ended_job_settings,
-                                                 self._rc_keys() + self._single_ended_keys_to_take_over(), False,
-                                                 reactant_structure_ids,  # + [transition_state_id]  # is this needed?
-                                                 calculation.get_settings(), [])
+                                                 self._rc_keys() + self._single_ended_keys_to_take_over(),
+                                                 reactant_structure_ids, calculation.get_settings())
             else:
                 return False
         elif job_label == "double_ended_refinement":
             for elementary_step in elementary_steps:
-                reactant_products = elementary_step.get_reactants(db.Side.BOTH)
-                reactant_structure_ids = self._get_optimized_structure_ids(reactant_products[0])
-                product_structure_ids = self._get_optimized_structure_ids(reactant_products[1])
-                if reactant_structure_ids and product_structure_ids\
-                        and self._all_structures_have_graph(reactant_structure_ids)\
-                        and self._all_structures_have_graph(product_structure_ids):
-                    self._refine_existing_react_jobs(self.options.double_ended_job,
-                                                     self.options.double_ended_job_settings, self._rc_keys(),
-                                                     True, reactant_structure_ids, calculation.get_settings(),
-                                                     product_structure_ids)
-                else:
+                if self.options.double_ended_job.order != "scine_bspline_optimization_job":
+                    raise RuntimeError("Only the logic for the scine_bspline_optimization job is implemented!")
+                if not elementary_step.has_reaction():
                     return False
+                if elementary_step.get_type() != db.ElementaryStepType.REGULAR:
+                    continue
+                self._refine_existing_react_jobs(self.options.double_ended_job,
+                                                 self.options.double_ended_job_settings,
+                                                 self._double_ended_keys_to_take_over(),
+                                                 [], calculation.get_settings(), elementary_step)
         else:
             raise RuntimeError("The job label is not resolved for elementary step refinement.")
         return True
 
     def _barrier_exceeded(self, elementary_step: db.ElementaryStep) -> bool:
         """
         Check the barrier of the elementary step.
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/gears/scheduler.py` & `scine_chemoton-3.0.0/scine_chemoton/gears/scheduler.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,113 +37,118 @@
     with the allowed number of active Calculations.
     The gap between these numbers will be closed by activating Calculations
     that are currently on hold.
     The order of the execution of the jobs as well as their activation does not
     necessarily follow the chronological order of their generation.
     """
 
-    class Options:
+    class Options(Gear.Options):
         """
         The options for the Scheduler Gear.
         """
 
         __slots__ = ("cycle_time", "job_counts", "job_priorities")
 
         def __init__(self):
+            super().__init__()
             self.cycle_time = 10
             """
             int
                 The minimum number of seconds between two cycles of the Gear.
                 Cycles are finished independent of this option, thus if a cycle
                 takes longer than the cycle_time will effectively lead to longer
                 cycle times and not cause multiple cycles of the same Gear.
             """
             self.job_counts: Dict[str, int] = {
                 "scine_geometry_optimization": 50,
+                "scine_ts_optimization": 50,
+                "scine_single_point": 50,
                 "scine_bond_orders": 50,
                 "graph": 100,
                 "scine_hessian": 10,
                 "scine_react_complex_afir": 10,
                 "scine_react_complex_nt": 10,
                 "scine_react_complex_nt2": 10,
+                "scine_step_refinement": 10,
                 "scine_dissociation_cut": 10,
                 "conformers": 2,
                 "final_conformer_deduplication": 2,
+                "kinetx_kinetic_modeling": 1,
+                "scine_bspline_optimization_job": 50,
             }
             """
             Dict[str, int]
                 The number of Calculations to be set to run at any given time.
                 Counts are given per order type (i.e. 'scine_hessian').
-                Defaults are:
-                scine_geometry_optimization: 50,
-                scine_bond_orders: 50,
-                graph: 100,
-                scine_hessian: 10,
-                scine_react_complex: 10,
-                conformers: 2
             """
             self.job_priorities: Dict[str, int] = {
                 "scine_geometry_optimization": 2,
                 "scine_ts_optimization": 2,
+                "scine_single_point": 5,
                 "scine_bond_orders": 2,
                 "graph": 2,
                 "scine_hessian": 2,
                 "scine_react_complex_afir": 5,
                 "scine_react_complex_nt": 5,
                 "scine_react_complex_nt2": 5,
+                "scine_step_refinement": 5,
                 "scine_dissociation_cut": 5,
                 "conformers": 2,
                 "final_conformer_deduplication": 2,
-                "scine_step_refinement": 5,
-                "scine_single_point": 5
+                "kinetx_kinetic_modeling": 1,
+                "scine_bspline_optimization_job": 5
             }
             """
             Dict[str, int]
                 The priority number of Calculations, which determines which are executed first.
                 Priorities are given per order type (i.e. 'scine_hessian').
                 A lower number corresponds to earlier execution.
                 The possible range of numbers is 1 to 10.
-                Defaults are:
-                scine_geometry_optimization: 2,
-                scine_bond_orders: 2,
-                graph: 2,
-                scine_hessian: 2,
-                scine_react_complex: 5,
-                conformers: 2
             """
 
     def __init__(self):
         super().__init__()
-        self.options = self.Options()
         self._required_collections = ["calculations"]
 
     def _loop_impl(self):
+        self._options_sanity_check()
+        selection = {"status": "hold"}
+        if self._calculations.get_one_calculation(dumps(selection)) is None:
+            return
         # Check how many calculations are scheduled to be run for each job type
         for order in self.options.job_counts:
             selection = {
                 "$and": [
                     {"status": "new"},
                     {"job.order": order},
                 ]
             }
             hits = 0
+            # Skip if no jobs of this order are allowed to run
             if hits >= self.options.job_counts[order]:
                 continue
-            # Count new jobs for the given order
-            for calculation in self._calculations.iterate_calculations(dumps(selection)):
-                hits += 1
-                if hits >= self.options.job_counts[order]:
+            # Skip if enough jobs are active
+            hits = self._calculations.count(dumps(selection))
+            if hits >= self.options.job_counts[order]:
+                continue
+            # If all new jobs were counted and there are free slots as defined by
+            #   the job_count start new jobs (set them from 'hold' to 'new')
+            selection = {"$and": [{"status": "hold"}, {"job.order": order}]}
+            diff = self.options.job_counts[order] - hits
+            for calculation in stop_on_timeout(self._calculations.iterate_calculations(dumps(selection))):
+                if self.stop_at_next_break_point:
+                    return
+                calculation.link(self._calculations)
+                # Sleep a bit in order not to make the DB choke
+                time.sleep(0.001)
+                calculation.set_status(db.Status.NEW)
+                calculation.set_priority(self.options.job_priorities[order])
+                diff -= 1
+                if diff <= 0:
                     break
-            else:
-                # If all new jobs were counted and there are free slots as defined by
-                #   the job_count start new jobs (set them from 'hold' to 'new')
-                selection = {"$and": [{"status": "hold"}, {"job.order": order}]}
-                diff = self.options.job_counts[order] - hits
-                for calculation in stop_on_timeout(self._calculations.iterate_calculations(dumps(selection))):
-                    calculation.link(self._calculations)
-                    # Sleep a bit in order not to make the DB choke
-                    time.sleep(0.001)
-                    calculation.set_status(db.Status.NEW)
-                    calculation.set_priority(self.options.job_priorities[order])
-                    diff -= 1
-                    if diff <= 0:
-                        break
+            if self.stop_at_next_break_point:
+                return
+
+    def _options_sanity_check(self):
+        for k in self.options.job_counts:
+            if k not in self.options.job_priorities:
+                raise ValueError(f"Missing key '{k}' in 'job_priorities'.")
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/gears/conformers/test_brute_force.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/gears/conformers/test_brute_force.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 # Local application tests imports
 from ... import test_database_setup as db_setup
 from ...resources import resources_root_path
 
 # Local application imports
 from ....engine import Engine
+from ....gears import _initialize_a_gear_to_a_db
 from ....gears.conformers.brute_force import BruteForceConformers
 
 
 def test_conformer_job_setup():
     # Connect to test DB
     manager = db_setup.get_clean_db("test_conformers_brute_force_conf")
 
@@ -47,21 +48,31 @@
     # Setup gear
     conformer_gear = BruteForceConformers()
     conformer_gear.options.model = model
     conformer_gear.options.conformer_job = db.Job("fake_conformer_generation")
     conformer_engine = Engine(manager.get_credentials(), fork=False)
     conformer_engine.set_gear(conformer_gear)
 
+    _initialize_a_gear_to_a_db(conformer_gear, manager.get_credentials())
+    assert len(conformer_gear.valid_compounds()) == 1
     # Run a single loop
     conformer_engine.run(single=True)
 
     # Checks
     hits = calculations.query_calculations(dumps({}))
     assert len(hits) == 1
 
+    # does not change with multiple runs
+    conformer_engine.run(single=True)
+    assert len(calculations.query_calculations(dumps({}))) == 1
+    conformer_gear.clear_cache()
+    conformer_engine.set_gear(conformer_gear)
+    conformer_engine.run(single=True)
+    assert len(calculations.query_calculations(dumps({}))) == 1
+
     calculation = db.Calculation(hits[0].id())
     calculation.link(calculations)
 
     assert len(calculation.get_structures()) == 1
     assert calculation.get_structures()[0].string() == centroid.id().string()
     assert calculation.get_status() == db.Status.HOLD
     assert calculation.get_job().order == "fake_conformer_generation"
@@ -136,14 +147,17 @@
         calculation = db.Calculation(hit.id())
         calculation.link(calculations)
         if calculation.get_job().order == "fake_conformer_generation":
             continue
         assert len(calculation.get_structures()) == 1
         assert calculation.get_status() == db.Status.HOLD
         assert calculation.get_job().order == "fake_opt"
+        guess_structure = db.Structure(calculation.get_structures()[0])
+        guess_structure.link(structures)
+        assert guess_structure.get_calculations("geometry_optimization")[0] == calculation.get_id()
 
     # Run a second loop
     conformer_engine.run(single=True)
 
     # Check again
     hits = calculations.query_calculations(dumps({}))
     assert len(hits) == 13
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_bond_based.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_bond_based.py`

 * *Files 18% similar despite different names*

```diff
@@ -53,46 +53,46 @@
         structure_list.append(structure)
 
     # Setup trial generator with impossible settings:
     # Cannot fulfil all minimum requirements and the bond modification boundaries simultaneously
     trial_generator = BondBased()
     trial_generator.initialize_collections(manager)
     trial_generator.options.model = model
-    trial_generator.options.bimolecular.min_bond_modifications = 1
-    trial_generator.options.bimolecular.max_bond_modifications = 2
-    trial_generator.options.bimolecular.min_inter_bond_formations = 1
-    trial_generator.options.bimolecular.max_inter_bond_formations = 2
-    trial_generator.options.bimolecular.min_intra_bond_formations = 1
-    trial_generator.options.bimolecular.max_intra_bond_formations = 1
-    trial_generator.options.bimolecular.min_bond_dissociations = 1
-    trial_generator.options.bimolecular.max_bond_dissociations = 1
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers = 1
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers_two_on_two = 1
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 2
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_intra_bond_formations = 1
+    trial_generator.options.bimolecular_options.min_bond_dissociations = 1
+    trial_generator.options.bimolecular_options.max_bond_dissociations = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
     # Generate trials
     trial_generator.bimolecular_reactions(structure_list)
 
     # Checks
     hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     assert len(hits) == 0
     hits = calculations.query_calculations(json.dumps({}))
     assert len(hits) == 0
 
     # Setup trial coordinator with only one or two inter coordinates
-    trial_generator.options.bimolecular.min_bond_modifications = 1
-    trial_generator.options.bimolecular.max_bond_modifications = 2
-    trial_generator.options.bimolecular.min_inter_bond_formations = 1
-    trial_generator.options.bimolecular.max_inter_bond_formations = 2
-    trial_generator.options.bimolecular.min_intra_bond_formations = 0
-    trial_generator.options.bimolecular.max_intra_bond_formations = 0
-    trial_generator.options.bimolecular.min_bond_dissociations = 0
-    trial_generator.options.bimolecular.max_bond_dissociations = 0
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers = 1
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers_two_on_two = 1
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 2
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 0
+    trial_generator.options.bimolecular_options.max_intra_bond_formations = 0
+    trial_generator.options.bimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.bimolecular_options.max_bond_dissociations = 0
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
     # Generate trials
     trial_generator.bimolecular_reactions(structure_list)
 
     # Expected number of trials
     # One intercoordinate: 4 * 3 = 12
     # Two intercoordinates: 12 choose 2 = 66
     # Sum: 78
@@ -108,27 +108,29 @@
         assert calculation.get_job().order == "scine_react_complex_nt2"
         n_formed = len(calculation.get_setting("nt_nt_associations"))
         assert n_formed in (2, 4)  # Two entries per pair
         n_diss = len(calculation.get_setting("nt_nt_dissociations"))
         assert n_diss == 0
         assert 2 <= n_formed + n_diss <= 4
         calculation.wipe()
+    for structure in structure_list:
+        structure.clear_all_calculations()
 
     # Setup trial coordinator with only one inter coordinate or one inter and one dissociation
-    trial_generator.options.bimolecular.min_bond_modifications = 1
-    trial_generator.options.bimolecular.max_bond_modifications = 2
-    trial_generator.options.bimolecular.min_inter_bond_formations = 1
-    trial_generator.options.bimolecular.max_inter_bond_formations = 1
-    trial_generator.options.bimolecular.min_intra_bond_formations = 0
-    trial_generator.options.bimolecular.max_intra_bond_formations = 0
-    trial_generator.options.bimolecular.min_bond_dissociations = 0
-    trial_generator.options.bimolecular.max_bond_dissociations = 1
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers = 1
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers_two_on_two = 1
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 0
+    trial_generator.options.bimolecular_options.max_intra_bond_formations = 0
+    trial_generator.options.bimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.bimolecular_options.max_bond_dissociations = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
     # Generate trials
     trial_generator.bimolecular_reactions(structure_list)
 
     # Expected number of trials
     # One intercoordinate: 4 * 3 = 12
     # One inter and one diss = 12 * 5 = 60
     # Sum: 72
@@ -144,27 +146,29 @@
         assert calculation.get_job().order == "scine_react_complex_nt2"
         n_formed = len(calculation.get_setting("nt_nt_associations"))
         assert n_formed == 2  # Two entries per pair
         n_diss = len(calculation.get_setting("nt_nt_dissociations"))
         assert n_diss in (0, 2)
         assert 2 <= n_formed + n_diss <= 4
         calculation.wipe()
+    for structure in structure_list:
+        structure.clear_all_calculations()
 
     # Setup trial coordinator with only one inter and one associative intra
-    trial_generator.options.bimolecular.min_bond_modifications = 1  # Not to be reached
-    trial_generator.options.bimolecular.max_bond_modifications = 2
-    trial_generator.options.bimolecular.min_inter_bond_formations = 1
-    trial_generator.options.bimolecular.max_inter_bond_formations = 1
-    trial_generator.options.bimolecular.min_intra_bond_formations = 1
-    trial_generator.options.bimolecular.max_intra_bond_formations = 1
-    trial_generator.options.bimolecular.min_bond_dissociations = 0
-    trial_generator.options.bimolecular.max_bond_dissociations = 0
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers = 1
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers_two_on_two = 1
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1  # Not to be reached
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_intra_bond_formations = 1
+    trial_generator.options.bimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.bimolecular_options.max_bond_dissociations = 0
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
     # Generate trials
     trial_generator.bimolecular_reactions(structure_list)
 
     # Expected number of trials
     # Number or intermolecular pairs= 4 * 3 = 12
     # Number of intramolecular associative pairs = 4
     # 4*12 = 48 combinations
@@ -180,27 +184,31 @@
         assert calculation.get_job().order == "scine_react_complex_nt2"
         n_formed = len(calculation.get_setting("nt_nt_associations"))
         assert n_formed == 4  # Two entries per pair
         n_diss = len(calculation.get_setting("nt_nt_dissociations"))
         assert n_diss == 0
         assert 2 <= n_formed + n_diss <= 4
         calculation.wipe()
+    for structure in structure_list:
+        structure.clear_all_calculations()
 
     # Setup  trial generator with mixed inter, intra associative and dissociative coordinates
-    trial_generator.options.bimolecular.min_bond_modifications = 1
-    trial_generator.options.bimolecular.max_bond_modifications = 2
-    trial_generator.options.bimolecular.min_inter_bond_formations = 1
-    trial_generator.options.bimolecular.max_inter_bond_formations = 2
-    trial_generator.options.bimolecular.min_intra_bond_formations = 0
-    trial_generator.options.bimolecular.max_intra_bond_formations = 3  # Not to be reached due to max bond modifications
-    trial_generator.options.bimolecular.min_bond_dissociations = 0
-    trial_generator.options.bimolecular.max_bond_dissociations = 3  # Not to be reached due to max bond modifications
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers = 1
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers_two_on_two = 1
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 2
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 0
+    # Not to be reached due to max bond modifications
+    trial_generator.options.bimolecular_options.max_intra_bond_formations = 3
+    trial_generator.options.bimolecular_options.min_bond_dissociations = 0
+    # Not to be reached due to max bond modifications
+    trial_generator.options.bimolecular_options.max_bond_dissociations = 3
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
     # Generate trials
     trial_generator.bimolecular_reactions(structure_list)
 
     # Checks
     hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     assert len(hits) == 0
 
@@ -248,14 +256,226 @@
     hits = calculations.query_calculations(json.dumps({}))
     assert len(hits) == 372
 
     # Cleaning
     manager.wipe()
 
 
+def test_bimol_enhancement():
+    """
+    Tests whether bimolecular elementary step trials are set up correctly
+    with the bond-based trial generator with enhancing
+    """
+    # Connect to test DB
+    manager = db_setup.get_clean_db("chemoton_test_bimol_bond_based_enhancement")
+
+    # Get collections
+    structures = manager.get_collection("structures")
+    compounds = manager.get_collection("compounds")
+    calculations = manager.get_collection("calculations")
+
+    # Add fake data
+    model = db.Model("FAKE", "FAKE", "F-AKE")
+    rr = resources_root_path()
+    structure_list = []
+    for mol in ["hydrogenperoxide", "water"]:
+        graph = json.load(open(os.path.join(rr, mol + ".json"), "r"))
+        structure = db.Structure()
+        structure.link(structures)
+        structure.create(os.path.join(rr, mol + ".xyz"), 0, 1)
+        structure.set_label(db.Label.MINIMUM_OPTIMIZED)
+        structure.set_graph("masm_cbor_graph", graph["masm_cbor_graph"])
+        structure.set_graph("masm_idx_map", graph["masm_idx_map"])
+        structure.set_graph("masm_decision_list", graph["masm_decision_list"])
+        compound = db.Compound()
+        compound.link(compounds)
+        compound.create([structure.id()])
+        structure.set_aggregate(compound.id())
+        structure_list.append(structure)
+
+    # Setup trial generator with impossible settings:
+    # Cannot fulfil all minimum requirements and the bond modification boundaries simultaneously
+    trial_generator = BondBased()
+    trial_generator.initialize_collections(manager)
+    trial_generator.options.model = model
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 2
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_intra_bond_formations = 1
+    trial_generator.options.bimolecular_options.min_bond_dissociations = 1
+    trial_generator.options.bimolecular_options.max_bond_dissociations = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
+    # Generate trials
+    trial_generator.bimolecular_reactions(structure_list)
+
+    # Checks
+    hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
+    assert len(hits) == 0
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 0
+
+    # Setup trial coordinator with only one inter and/or one associative intra
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 0
+    trial_generator.options.bimolecular_options.max_intra_bond_formations = 1
+    trial_generator.options.bimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.bimolecular_options.max_bond_dissociations = 0
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
+    # Generate trials
+    trial_generator.bimolecular_reactions(structure_list, with_exact_settings_check=True)
+
+    # Expected number of trials
+    # Number or intermolecular pairs= 4 * 3 = 12
+    # Number of intramolecular associative pairs = 4
+    # 4*12 = 48 combinations
+    # Number of only intermolecular pairs = 12
+    # sum = 60
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 60
+
+    for hit in hits:
+        calculation = db.Calculation(hit.id())
+        calculation.link(calculations)
+        assert len(calculation.get_structures()) == 2
+        assert calculation.get_status() == db.Status.HOLD
+        assert calculation.get_model() == model
+        assert calculation.get_job().order == "scine_react_complex_nt2"
+        n_formed = len(calculation.get_setting("nt_nt_associations"))
+        assert 1 < n_formed <= 4  # Two entries per pair
+        n_diss = len(calculation.get_setting("nt_nt_dissociations"))
+        assert n_diss == 0
+        assert 1 <= n_formed + n_diss <= 4
+
+    # running again will give the same results
+    trial_generator.bimolecular_reactions(structure_list, with_exact_settings_check=True)
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 60
+
+    # Setup trial coordinator with one or two inter coordinates
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 2
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 0
+    trial_generator.options.bimolecular_options.max_intra_bond_formations = 0
+    trial_generator.options.bimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.bimolecular_options.max_bond_dissociations = 0
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
+    # Generate trials
+    trial_generator.bimolecular_reactions(structure_list, with_exact_settings_check=True)
+
+    # Expected number of trials
+    # One intercoordinate: 4 * 3 = 12 were already generated
+    # Two intercoordinates: 12 choose 2 = 66
+    # Sum: 66 + 60 already existing = 126
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 126
+
+    for hit in hits:
+        calculation = db.Calculation(hit.id())
+        calculation.link(calculations)
+        assert len(calculation.get_structures()) == 2
+        assert calculation.get_status() == db.Status.HOLD
+        assert calculation.get_model() == model
+        assert calculation.get_job().order == "scine_react_complex_nt2"
+        n_formed = len(calculation.get_setting("nt_nt_associations"))
+        assert n_formed in (2, 4)  # Two entries per pair
+        n_diss = len(calculation.get_setting("nt_nt_dissociations"))
+        assert n_diss == 0
+        assert 2 <= n_formed + n_diss <= 4
+
+    # Setup  trial generator with mixed inter, intra associative and dissociative coordinates
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 2
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 0
+    # Not to be reached due to max bond modifications
+    trial_generator.options.bimolecular_options.max_intra_bond_formations = 3
+    trial_generator.options.bimolecular_options.min_bond_dissociations = 0
+    # Not to be reached due to max bond modifications
+    trial_generator.options.bimolecular_options.max_bond_dissociations = 3
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
+    # Generate trials
+    trial_generator.bimolecular_reactions(structure_list, with_exact_settings_check=True)
+
+    # Checks
+    hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
+    assert len(hits) == 0
+
+    # Expected number of hits:
+    # number of intermolecular pairs = n_atoms(H2O) * n_atoms(H2O2) = 3*4 = 12
+    # number of pairs of pairs = n_pairs over 2 = 12 over 2 = 66
+    # Number of bonds: 3 (H2O2) + 2 (H2O) = 5
+    # Number of intramolecular unbound pairs: 3 (H2O2) + 1 (H2O) = 4
+    # Expected number of hits:
+    # Two intermol coordinates: 66
+    # One intermol coordinate: 12
+    # One intermol + one diss: 12*5 = 60
+    # One intermol + one intramol formation = 12*4 = 48
+    # Sum: 186
+
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 186
+
+    for hit in hits:
+        calculation = db.Calculation(hit.id())
+        calculation.link(calculations)
+        assert len(calculation.get_structures()) == 2
+        assert calculation.get_status() == db.Status.HOLD
+        assert calculation.get_model() == model
+        assert calculation.get_job().order == "scine_react_complex_nt2"
+        n_formed = len(calculation.get_setting("nt_nt_associations"))
+        assert n_formed in (2, 4)  # Two entries per pair
+        n_diss = len(calculation.get_setting("nt_nt_dissociations"))
+        assert n_diss in (0, 2)  # Two entries per pair
+        assert 2 <= n_formed + n_diss <= 4
+
+    # Run a second time
+    trial_generator.bimolecular_reactions(structure_list)
+
+    # Check again
+    hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
+    assert len(hits) == 0
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 186
+
+    # Run a third time, unchanged with enhanced settings check
+    trial_generator.bimolecular_reactions(structure_list, with_exact_settings_check=True)
+
+    # Check again
+    hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
+    assert len(hits) == 0
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 186
+
+    # Rerun with a different model
+    model2 = db.Model("FAKE2", "", "")
+    trial_generator.options.model = model2
+    trial_generator.bimolecular_reactions(structure_list)
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 372
+
+    # Cleaning
+    manager.wipe()
+
+
 def test_unimol_dissociations():
     """
     Tests whether unimolecular elementary step trials containing only
     dissociations are set up correctly with the bond-based trial generator
     """
     # Connect to test DB
     manager = db_setup.get_clean_db("chemoton_test_unimol_dissociations_bond_based")
@@ -277,39 +497,40 @@
         structure.set_graph("masm_cbor_graph", graph["masm_cbor_graph"])
         structure.set_graph("masm_idx_map", graph["masm_idx_map"])
         structure.set_graph("masm_decision_list", graph["masm_decision_list"])
         compound = db.Compound()
         compound.link(compounds)
         compound.create([structure.id()])
         structure.set_aggregate(compound.id())
+    structure.clear_all_calculations()
 
     # Setup trial generator with settings that cannot be fulfilled
     trial_generator = BondBased()
     trial_generator.initialize_collections(manager)
     trial_generator.options.model = model
-    trial_generator.options.unimolecular.min_bond_modifications = 1
-    trial_generator.options.unimolecular.max_bond_modifications = 1
-    trial_generator.options.unimolecular.min_bond_dissociations = 2
-    trial_generator.options.unimolecular.min_bond_formations = 2
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1
+    trial_generator.options.unimolecular_options.max_bond_modifications = 1
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 2
+    trial_generator.options.unimolecular_options.min_bond_formations = 2
     # Generate trials
     trial_generator.unimolecular_reactions(structure)
 
     # Checks
     hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     assert len(hits) == 0
     hits = calculations.query_calculations(json.dumps({}))
     assert len(hits) == 0
 
     # Exactly one dissociation at once
-    trial_generator.options.unimolecular.min_bond_modifications = 1
-    trial_generator.options.unimolecular.max_bond_modifications = 1
-    trial_generator.options.unimolecular.min_bond_dissociations = 1
-    trial_generator.options.unimolecular.max_bond_dissociations = 1
-    trial_generator.options.unimolecular.min_bond_formations = 0
-    trial_generator.options.unimolecular.max_bond_formations = 0
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1
+    trial_generator.options.unimolecular_options.max_bond_modifications = 1
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 1
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 1
+    trial_generator.options.unimolecular_options.min_bond_formations = 0
+    trial_generator.options.unimolecular_options.max_bond_formations = 0
 
     trial_generator.unimolecular_reactions(structure)
     # Expected number of hits = number of bonds = 16
     hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     assert len(hits) == 0
     hits = calculations.query_calculations(json.dumps({}))
     assert len(hits) == 16
@@ -333,22 +554,23 @@
         n_formed = len(calculation.get_setting("nt_nt_associations"))
         assert n_formed == 0
         n_diss = len(calculation.get_setting("nt_nt_dissociations"))
         assert n_diss == 2  # Two entries per pair
         assert 2 <= n_formed + n_diss <= 2
         # Cleaning
         calculation.wipe()
+    structure.clear_all_calculations()
 
     # Try exactly two dissociations at once
-    trial_generator.options.unimolecular.min_bond_modifications = 1  # Not to be reached
-    trial_generator.options.unimolecular.max_bond_modifications = 2
-    trial_generator.options.unimolecular.min_bond_dissociations = 2
-    trial_generator.options.unimolecular.max_bond_dissociations = 2
-    trial_generator.options.unimolecular.min_bond_formations = 0
-    trial_generator.options.unimolecular.max_bond_formations = 0
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1  # Not to be reached
+    trial_generator.options.unimolecular_options.max_bond_modifications = 2
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 2
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 2
+    trial_generator.options.unimolecular_options.min_bond_formations = 0
+    trial_generator.options.unimolecular_options.max_bond_formations = 0
 
     # Expected number of hits = number of bonds choose 2 = 16 choose 2 = 120
     trial_generator.unimolecular_reactions(structure)
     hits = calculations.query_calculations(json.dumps({}))
     assert len(hits) == 120
 
     for hit in hits:
@@ -360,22 +582,23 @@
         n_formed = len(calculation.get_setting("nt_nt_associations"))
         assert n_formed == 0
         n_diss = len(calculation.get_setting("nt_nt_dissociations"))
         assert n_diss == 4  # Two entries per pair
         assert 2 <= n_formed + n_diss <= 4
         # Cleaning
         calculation.wipe()
+    structure.clear_all_calculations()
 
     # Try one or two dissociations at once
-    trial_generator.options.unimolecular.min_bond_modifications = 1
-    trial_generator.options.unimolecular.max_bond_modifications = 3  # Not to be reached
-    trial_generator.options.unimolecular.min_bond_dissociations = 1
-    trial_generator.options.unimolecular.max_bond_dissociations = 2
-    trial_generator.options.unimolecular.min_bond_formations = 0
-    trial_generator.options.unimolecular.max_bond_formations = 0
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1
+    trial_generator.options.unimolecular_options.max_bond_modifications = 3  # Not to be reached
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 1
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 2
+    trial_generator.options.unimolecular_options.min_bond_formations = 0
+    trial_generator.options.unimolecular_options.max_bond_formations = 0
 
     # Expected number of hits
     # Single dissociations = number of bonds = 16
     # Double dissociations = number of bonds choose 2 = 16 choose 2 = 120
     # Sum: 136
     trial_generator.unimolecular_reactions(structure)
     hits = calculations.query_calculations(json.dumps({}))
@@ -428,36 +651,36 @@
         compound.create([structure.id()])
         structure.set_aggregate(compound.id())
 
     # Setup trial generator with settings that cannot be fulfilled
     trial_generator = BondBased()
     trial_generator.initialize_collections(manager)
     trial_generator.options.model = model
-    trial_generator.options.unimolecular.min_bond_modifications = 2
-    trial_generator.options.unimolecular.max_bond_modifications = 1
-    trial_generator.options.unimolecular.min_bond_dissociations = 0
-    trial_generator.options.unimolecular.max_bond_dissociations = 0
-    trial_generator.options.unimolecular.min_bond_formations = 0
-    trial_generator.options.unimolecular.max_bond_formations = 1
+    trial_generator.options.unimolecular_options.min_bond_modifications = 2
+    trial_generator.options.unimolecular_options.max_bond_modifications = 1
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.min_bond_formations = 0
+    trial_generator.options.unimolecular_options.max_bond_formations = 1
     # Generate trials
     trial_generator.unimolecular_reactions(structure)
 
     # Checks
     hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     assert len(hits) == 0
     hits = calculations.query_calculations(json.dumps({}))
     assert len(hits) == 0
 
     # Test exactly one association
-    trial_generator.options.unimolecular.min_bond_modifications = 1
-    trial_generator.options.unimolecular.max_bond_modifications = 1
-    trial_generator.options.unimolecular.min_bond_dissociations = 0
-    trial_generator.options.unimolecular.max_bond_dissociations = 0
-    trial_generator.options.unimolecular.min_bond_formations = 1
-    trial_generator.options.unimolecular.max_bond_formations = 1
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1
+    trial_generator.options.unimolecular_options.max_bond_modifications = 1
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.min_bond_formations = 1
+    trial_generator.options.unimolecular_options.max_bond_formations = 1
 
     trial_generator.unimolecular_reactions(structure)
     # Expected number of hits:
     # Number of pairs: 4 choose 2 = 6
     # Number of bonds: 3
     # Number of unbound pairs = expected number of hits = 3
 
@@ -479,22 +702,23 @@
         n_formed = len(calculation.get_setting("nt_nt_associations"))
         assert n_formed == 2  # 2 entries per pair
         n_diss = len(calculation.get_setting("nt_nt_dissociations"))
         assert n_diss == 0
         assert 2 <= n_formed + n_diss <= 2
         # Clean up
         calculation.wipe()
+    structure.clear_all_calculations()
 
     # Test exactly two associations
-    trial_generator.options.unimolecular.min_bond_modifications = 2
-    trial_generator.options.unimolecular.max_bond_modifications = 2
-    trial_generator.options.unimolecular.min_bond_dissociations = 0
-    trial_generator.options.unimolecular.max_bond_dissociations = 0
-    trial_generator.options.unimolecular.min_bond_formations = 1  # Not to be reached
-    trial_generator.options.unimolecular.max_bond_formations = 2
+    trial_generator.options.unimolecular_options.min_bond_modifications = 2
+    trial_generator.options.unimolecular_options.max_bond_modifications = 2
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.min_bond_formations = 1  # Not to be reached
+    trial_generator.options.unimolecular_options.max_bond_formations = 2
 
     trial_generator.unimolecular_reactions(structure)
     # Expected number of hits:
     # Number of unbound pairs choose 2 = 3 choose 2 = 3
 
     hits = calculations.query_calculations(json.dumps({}))
     assert len(hits) == 3
@@ -509,22 +733,23 @@
         n_formed = len(calculation.get_setting("nt_nt_associations"))
         assert n_formed == 4  # 2 entries per pair
         n_diss = len(calculation.get_setting("nt_nt_dissociations"))
         assert n_diss == 0
         assert 4 <= n_formed + n_diss <= 4
         # Clean up
         calculation.wipe()
+    structure.clear_all_calculations()
 
     # Test one or two associations
-    trial_generator.options.unimolecular.min_bond_modifications = 1
-    trial_generator.options.unimolecular.max_bond_modifications = 2
-    trial_generator.options.unimolecular.min_bond_dissociations = 0
-    trial_generator.options.unimolecular.max_bond_dissociations = 0
-    trial_generator.options.unimolecular.min_bond_formations = 1  # Not to be reached
-    trial_generator.options.unimolecular.max_bond_formations = 2
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1
+    trial_generator.options.unimolecular_options.max_bond_modifications = 2
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.min_bond_formations = 1  # Not to be reached
+    trial_generator.options.unimolecular_options.max_bond_formations = 2
 
     trial_generator.unimolecular_reactions(structure)
     # Expected number of hits:
     # Number of unbound pairs = 3
     # Number of unbound pairs choose 2 = 3 choose 2 = 3
     # Sum: 6
 
@@ -579,20 +804,20 @@
         compound.create([structure.id()])
         structure.set_aggregate(compound.id())
 
     # Setup trial generator for either one dissociation or one association
     trial_generator = BondBased()
     trial_generator.initialize_collections(manager)
     trial_generator.options.model = model
-    trial_generator.options.unimolecular.min_bond_modifications = 1
-    trial_generator.options.unimolecular.max_bond_modifications = 1
-    trial_generator.options.unimolecular.min_bond_dissociations = 0
-    trial_generator.options.unimolecular.max_bond_dissociations = 1
-    trial_generator.options.unimolecular.min_bond_formations = 0
-    trial_generator.options.unimolecular.max_bond_formations = 1
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1
+    trial_generator.options.unimolecular_options.max_bond_modifications = 1
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 1
+    trial_generator.options.unimolecular_options.min_bond_formations = 0
+    trial_generator.options.unimolecular_options.max_bond_formations = 1
     # Generate trials
     trial_generator.unimolecular_reactions(structure)
 
     # Expected number of hits:
     # Number of bond: 3
     # Number of unbound pairs: 3
     # Sum: 6
@@ -621,29 +846,156 @@
         n_formed = len(calculation.get_setting("nt_nt_associations"))
         assert n_formed in (0, 2)  # 2 entries per pair
         n_diss = len(calculation.get_setting("nt_nt_dissociations"))
         assert n_diss in (0, 2)
         assert 2 <= n_formed + n_diss <= 2
         # Clean up
         calculation.wipe()
+    structure.clear_all_calculations()
 
     # Setup trial generator up to 3 intramolecular coordinates of any type
     trial_generator = BondBased()
     trial_generator.initialize_collections(manager)
     trial_generator.options.model = model
-    trial_generator.options.unimolecular.min_bond_modifications = 1
-    trial_generator.options.unimolecular.max_bond_modifications = 3
-    trial_generator.options.unimolecular.min_bond_dissociations = 0
-    trial_generator.options.unimolecular.max_bond_dissociations = 3
-    trial_generator.options.unimolecular.min_bond_formations = 0
-    trial_generator.options.unimolecular.max_bond_formations = 3
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1
+    trial_generator.options.unimolecular_options.max_bond_modifications = 3
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 3
+    trial_generator.options.unimolecular_options.min_bond_formations = 0
+    trial_generator.options.unimolecular_options.max_bond_formations = 3
+    # Generate trials
+    trial_generator.unimolecular_reactions(structure)
+
+    # Expected number of hits:
+    # Number of pairs (bound + unbound) = one modification: 6
+    # Two modifications: 6 choose 2: 15
+    # Three modifications: 6 choose 3: 20
+    # Sum: 41
+
+    hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
+    assert len(hits) == 0
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 41
+
+    # Run a second time
+    trial_generator.unimolecular_reactions(structure)
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 41
+
+    for hit in hits:
+        calculation = db.Calculation(hit.id())
+        calculation.link(calculations)
+        assert len(calculation.get_structures()) == 1
+        assert calculation.get_status() == db.Status.HOLD
+        assert calculation.get_model() == model
+        assert calculation.get_job().order == "scine_react_complex_nt2"
+        n_formed = len(calculation.get_setting("nt_nt_associations"))
+        assert n_formed in (0, 2, 4, 6)  # 2 entries per pair
+        n_diss = len(calculation.get_setting("nt_nt_dissociations"))
+        assert n_diss in (0, 2, 4, 6)  # 2 entries per pair
+        assert 2 <= n_formed + n_diss <= 6
+
+    # Rerun with a different model
+    model2 = db.Model("FAKE2", "", "")
+    trial_generator.options.model = model2
+    trial_generator.unimolecular_reactions(structure)
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 82
+
+    # Cleaning
+    manager.wipe()
+
+
+def test_unimol_mixed_enhancement():
+    """
+    Tests whether unimolecular elementary step trials containing only
+    dissociations and associations are set up correctly with the bond-based
+    trial generator
+    """
+    # Connect to test DB
+    manager = db_setup.get_clean_db("chemoton_test_unimol_mixed_bond_based_enhancement")
+
+    # Get collections
+    structures = manager.get_collection("structures")
+    compounds = manager.get_collection("compounds")
+    calculations = manager.get_collection("calculations")
+
+    # Add fake data
+    model = db.Model("FAKE", "FAKE", "F-AKE")
+    rr = resources_root_path()
+    for mol in ["hydrogenperoxide"]:
+        graph = json.load(open(os.path.join(rr, mol + ".json"), "r"))
+        structure = db.Structure()
+        structure.link(structures)
+        structure.create(os.path.join(rr, mol + ".xyz"), 0, 1)
+        structure.set_label(db.Label.MINIMUM_OPTIMIZED)
+        structure.set_graph("masm_cbor_graph", graph["masm_cbor_graph"])
+        structure.set_graph("masm_idx_map", graph["masm_idx_map"])
+        structure.set_graph("masm_decision_list", graph["masm_decision_list"])
+        compound = db.Compound()
+        compound.link(compounds)
+        compound.create([structure.id()])
+        structure.set_aggregate(compound.id())
+
+    # Setup trial generator for either one dissociation or one association
+    trial_generator = BondBased()
+    trial_generator.initialize_collections(manager)
+    trial_generator.options.model = model
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1
+    trial_generator.options.unimolecular_options.max_bond_modifications = 1
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 1
+    trial_generator.options.unimolecular_options.min_bond_formations = 0
+    trial_generator.options.unimolecular_options.max_bond_formations = 1
     # Generate trials
     trial_generator.unimolecular_reactions(structure)
 
     # Expected number of hits:
+    # Number of bond: 3
+    # Number of unbound pairs: 3
+    # Sum: 6
+    hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
+    assert len(hits) == 0
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 6
+
+    trial_generator.unimolecular_reactions(structure)
+
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 6
+
+    # Run a second time
+    trial_generator.unimolecular_reactions(structure)
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 6
+
+    for hit in hits:
+        calculation = db.Calculation(hit.id())
+        calculation.link(calculations)
+        assert len(calculation.get_structures()) == 1
+        assert calculation.get_status() == db.Status.HOLD
+        assert calculation.get_model() == model
+        assert calculation.get_job().order == "scine_react_complex_nt2"
+        n_formed = len(calculation.get_setting("nt_nt_associations"))
+        assert n_formed in (0, 2)  # 2 entries per pair
+        n_diss = len(calculation.get_setting("nt_nt_dissociations"))
+        assert n_diss in (0, 2)
+        assert 2 <= n_formed + n_diss <= 2
+
+    # Setup trial generator up to 3 intramolecular coordinates of any type
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1
+    trial_generator.options.unimolecular_options.max_bond_modifications = 3
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 3
+    trial_generator.options.unimolecular_options.min_bond_formations = 0
+    trial_generator.options.unimolecular_options.max_bond_formations = 3
+    # Generate trials
+    trial_generator.unimolecular_reactions(structure, with_exact_settings_check=True)
+
+    # Expected number of hits:
     # Number of pairs (bound + unbound) = one modification: 6
     # Two modifications: 6 choose 2: 15
     # Three modifications: 6 choose 3: 20
     # Sum: 41
 
     hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     assert len(hits) == 0
@@ -685,64 +1037,64 @@
     unimolecular reactions is correct
     """
     rr = resources_root_path()
     structure_file = os.path.join(rr, "hydrogenperoxide.xyz")
     trial_generator = BondBased()
 
     # Options that should not allow any trials
-    trial_generator.options.unimolecular.min_bond_modifications = 2
-    trial_generator.options.unimolecular.max_bond_modifications = 1
+    trial_generator.options.unimolecular_options.min_bond_modifications = 2
+    trial_generator.options.unimolecular_options.max_bond_modifications = 1
     n_trials = trial_generator.estimate_n_unimolecular_trials(structure_file)
     assert n_trials == 0
 
-    trial_generator.options.unimolecular.min_bond_modifications = 3
-    trial_generator.options.unimolecular.max_bond_modifications = 4
-    trial_generator.options.unimolecular.min_bond_dissociations = 0
-    trial_generator.options.unimolecular.max_bond_dissociations = 1
-    trial_generator.options.unimolecular.min_bond_formations = 0
-    trial_generator.options.unimolecular.max_bond_formations = 1
+    trial_generator.options.unimolecular_options.min_bond_modifications = 3
+    trial_generator.options.unimolecular_options.max_bond_modifications = 4
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 1
+    trial_generator.options.unimolecular_options.min_bond_formations = 0
+    trial_generator.options.unimolecular_options.max_bond_formations = 1
     n_trials = trial_generator.estimate_n_unimolecular_trials(structure_file)
     assert n_trials == 0
 
     # Test legitimate options with all pairs
     # Associations only
-    trial_generator.options.unimolecular.min_bond_modifications = 1
-    trial_generator.options.unimolecular.max_bond_modifications = 3
-    trial_generator.options.unimolecular.min_bond_dissociations = 0
-    trial_generator.options.unimolecular.max_bond_dissociations = 0
-    trial_generator.options.unimolecular.min_bond_formations = 0
-    trial_generator.options.unimolecular.max_bond_formations = 1
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1
+    trial_generator.options.unimolecular_options.max_bond_modifications = 3
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.min_bond_formations = 0
+    trial_generator.options.unimolecular_options.max_bond_formations = 1
     # Expected number of trials
     # 1 form: 3
     # Sum: 3
     n_trials = trial_generator.estimate_n_unimolecular_trials(structure_file)
     assert n_trials == 3
 
     # Dissociations only
-    trial_generator.options.unimolecular.min_bond_modifications = 1
-    trial_generator.options.unimolecular.max_bond_modifications = 3
-    trial_generator.options.unimolecular.min_bond_dissociations = 0
-    trial_generator.options.unimolecular.max_bond_dissociations = 3
-    trial_generator.options.unimolecular.min_bond_formations = 0
-    trial_generator.options.unimolecular.max_bond_formations = 0
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1
+    trial_generator.options.unimolecular_options.max_bond_modifications = 3
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 3
+    trial_generator.options.unimolecular_options.min_bond_formations = 0
+    trial_generator.options.unimolecular_options.max_bond_formations = 0
     # Expected number of trials
     # 1 diss: 3
     # 2 diss: 3
     # 3 diss: 1
     # Sum: 7
     n_trials = trial_generator.estimate_n_unimolecular_trials(structure_file)
     assert n_trials == 7
 
     # Mixed associations and dissociations
-    trial_generator.options.unimolecular.min_bond_modifications = 1
-    trial_generator.options.unimolecular.max_bond_modifications = 3
-    trial_generator.options.unimolecular.min_bond_dissociations = 0
-    trial_generator.options.unimolecular.max_bond_dissociations = 1
-    trial_generator.options.unimolecular.min_bond_formations = 0
-    trial_generator.options.unimolecular.max_bond_formations = 2
+    trial_generator.options.unimolecular_options.min_bond_modifications = 1
+    trial_generator.options.unimolecular_options.max_bond_modifications = 3
+    trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.unimolecular_options.max_bond_dissociations = 1
+    trial_generator.options.unimolecular_options.min_bond_formations = 0
+    trial_generator.options.unimolecular_options.max_bond_formations = 2
     # Expected number of trials
     # 1 diss: 3
     # 1 form: 3
     # 2 form: 3
     # 1 form + 1 diss = 3*3 = 9
     # 2 form + 1 diss = 3*3 = 9
     # Sum: 27
@@ -786,90 +1138,92 @@
     """
     rr = resources_root_path()
     structure_file1 = os.path.join(rr, "hydrogenperoxide.xyz")
     structure_file2 = os.path.join(rr, "water.xyz")
     trial_generator = BondBased()
 
     # Options that should not allow any trials
-    trial_generator.options.bimolecular.min_bond_modifications = 2
-    trial_generator.options.bimolecular.max_bond_modifications = 1
+    trial_generator.options.bimolecular_options.min_bond_modifications = 2
+    trial_generator.options.bimolecular_options.max_bond_modifications = 1
     n_trials = trial_generator.estimate_n_bimolecular_trials(structure_file1, structure_file2)
     assert n_trials == 0
 
-    trial_generator.options.bimolecular.min_bond_modifications = 1
-    trial_generator.options.bimolecular.max_bond_modifications = 2
-    trial_generator.options.bimolecular.min_inter_bond_formations = 0
-    trial_generator.options.bimolecular.max_inter_bond_formations = 0
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 0
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 0
     n_trials = trial_generator.estimate_n_bimolecular_trials(structure_file1, structure_file2)
     assert n_trials == 0
 
-    trial_generator.options.bimolecular.min_bond_modifications = 2
-    trial_generator.options.bimolecular.max_bond_modifications = 1
+    trial_generator.options.bimolecular_options.min_bond_modifications = 2
+    trial_generator.options.bimolecular_options.max_bond_modifications = 1
     n_trials = trial_generator.estimate_n_bimolecular_trials(structure_file1, structure_file2)
     assert n_trials == 0
 
-    trial_generator.options.bimolecular.min_bond_modifications = 1
-    trial_generator.options.bimolecular.max_bond_modifications = 1
-    trial_generator.options.bimolecular.min_inter_bond_formations = 0
-    trial_generator.options.bimolecular.max_inter_bond_formations = 1
-    trial_generator.options.bimolecular.min_intra_bond_formations = 1
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 1
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 0
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 1
     n_trials = trial_generator.estimate_n_bimolecular_trials(structure_file1, structure_file2)
     assert n_trials == 0
 
     # Test legitimate options with all pairs
     # One or two intermolecular bond formations
-    trial_generator.options.bimolecular.min_bond_modifications = 1
-    trial_generator.options.bimolecular.max_bond_modifications = 2
-    trial_generator.options.bimolecular.min_inter_bond_formations = 1
-    trial_generator.options.bimolecular.max_inter_bond_formations = 2
-    trial_generator.options.bimolecular.min_intra_bond_formations = 0
-    trial_generator.options.bimolecular.max_intra_bond_formations = 0
-    trial_generator.options.bimolecular.min_bond_dissociations = 0
-    trial_generator.options.bimolecular.max_bond_dissociations = 0
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers = 1
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers_two_on_two = 1
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 2
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 0
+    trial_generator.options.bimolecular_options.max_intra_bond_formations = 0
+    trial_generator.options.bimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.bimolecular_options.max_bond_dissociations = 0
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
     # Expected number of trials
     # One intercoordinate: 4 * 3 = 12
     # Two intercoordinates: 12 choose 2 = 66
     # Sum: 78
     n_trials = trial_generator.estimate_n_bimolecular_trials(structure_file1, structure_file2)
     assert n_trials == 78
 
     # Setup trial coordinator with only one inter coordinate or one inter and one dissociation
-    trial_generator.options.bimolecular.min_bond_modifications = 1
-    trial_generator.options.bimolecular.max_bond_modifications = 2
-    trial_generator.options.bimolecular.min_inter_bond_formations = 1
-    trial_generator.options.bimolecular.max_inter_bond_formations = 1
-    trial_generator.options.bimolecular.min_intra_bond_formations = 0
-    trial_generator.options.bimolecular.max_intra_bond_formations = 0
-    trial_generator.options.bimolecular.min_bond_dissociations = 0
-    trial_generator.options.bimolecular.max_bond_dissociations = 1
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers = 1
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers_two_on_two = 1
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 0
+    trial_generator.options.bimolecular_options.max_intra_bond_formations = 0
+    trial_generator.options.bimolecular_options.min_bond_dissociations = 0
+    trial_generator.options.bimolecular_options.max_bond_dissociations = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
     # Expected number of trials
     # One intercoordinate: 4 * 3 = 12
     # One inter and one diss = 12 * 5 = 60
     # Sum: 72
     n_trials = trial_generator.estimate_n_bimolecular_trials(structure_file1, structure_file2, attack_points_per_site=2)
     assert n_trials == 72
 
     # Mixed inter, intra and dissociative
-    trial_generator.options.bimolecular.min_bond_modifications = 1
-    trial_generator.options.bimolecular.max_bond_modifications = 2
-    trial_generator.options.bimolecular.min_inter_bond_formations = 1
-    trial_generator.options.bimolecular.max_inter_bond_formations = 2
-    trial_generator.options.bimolecular.min_intra_bond_formations = 0
-    trial_generator.options.bimolecular.max_intra_bond_formations = 3  # Not to be reached due to max bond modifications
-    trial_generator.options.bimolecular.min_bond_dissociations = 0
-    trial_generator.options.bimolecular.max_bond_dissociations = 3  # Not to be reached due to max bond modifications
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers = 1
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers_two_on_two = 1
+    trial_generator.options.bimolecular_options.min_bond_modifications = 1
+    trial_generator.options.bimolecular_options.max_bond_modifications = 2
+    trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+    trial_generator.options.bimolecular_options.max_inter_bond_formations = 2
+    trial_generator.options.bimolecular_options.min_intra_bond_formations = 0
+    # Not to be reached due to max bond modifications
+    trial_generator.options.bimolecular_options.max_intra_bond_formations = 3
+    trial_generator.options.bimolecular_options.min_bond_dissociations = 0
+    # Not to be reached due to max bond modifications
+    trial_generator.options.bimolecular_options.max_bond_dissociations = 3
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
     # Expected number of hits:
     # number of intermolecular pairs = n_atoms(H2O) * n_atoms(H2O2) = 3*4 = 12
     # number of pairs of pairs = n_pairs over 2 = 12 over 2 = 66
     # Number of bonds: 3 (H2O2) + 2 (H2O) = 5
     # Number of intramolecular unbound pairs: 3 (H2O2) + 1 (H2O) = 4
     # Expected number of hits:
     # Two intermol coordinates: 66
@@ -877,77 +1231,77 @@
     # One intermol + one diss: 12*5 = 60
     # One intermol + one intramol formation = 12*4 = 48
     # Sum: 186
     n_trials = trial_generator.estimate_n_bimolecular_trials(structure_file1, structure_file2, attack_points_per_site=2)
     assert n_trials == 186
 
     # Influence of rotamers
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers = 2
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers_two_on_two = 3
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 2
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 3
     # Expected number of trials
     # Two intermol coordinates*number_rotamers_two_on_two: 66*3
     # One intermol coordinate*number_rotamers: 12*2
     # One intermol + one diss*number_rotamers : 12*5*2
     # One intermol + one intramol formation*number_rotamers = 12*4*2
     # Sum:
     n_trials = trial_generator.estimate_n_bimolecular_trials(structure_file1, structure_file2)
     assert n_trials == 438
 
     # Influence of multiple attack points
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers = 1
-    trial_generator.options.bimolecular.complex_generator.options.number_rotamers_two_on_two = 1
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = True
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.number_rotamers_two_on_two = 1
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = True
     # Expected number of trials
     # 186 * 2**2
     # Sum: 744
     n_trials = trial_generator.estimate_n_bimolecular_trials(structure_file1, structure_file2, attack_points_per_site=2)
     assert n_trials == 744
 
     # Test with limited number of reactive pairs
     # Only one reactive intermolecular pair
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
     n_trials = trial_generator.estimate_n_bimolecular_trials(
         structure_file1, structure_file2, attack_points_per_site=2, n_inter_reactive_pairs=1
     )
     # Expected number of trials:
     # One intermol coordinate: 1
     # Two intermol coordinates: 0
     # One intermol + one diss: 1*5 = 5
     # One intermol + one intramol formation = 1*4 = 4
     # Sum: 10
     assert n_trials == 10
 
     # Only one reactive intermolecular pair
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
     n_trials = trial_generator.estimate_n_bimolecular_trials(
         structure_file1, structure_file2, attack_points_per_site=2, n_inter_reactive_pairs=1
     )
     # Expected number of trials:
     # One intermol coordinate: 1
     # Two intermol coordinates: 0
     # One intermol + one diss: 1*5 = 5
     # One intermol + one intramol formation = 1*4 = 4
     # Sum: 10
     assert n_trials == 10
 
     # Only two reactive diss pairs in H2O2
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
     n_trials = trial_generator.estimate_n_bimolecular_trials(
         structure_file1, structure_file2, attack_points_per_site=2, n_inter_reactive_pairs=1, n_reactive_bound_pairs1=2
     )
     # Expected number of trials:
     # One intermol coordinate: 1
     # Two intermol coordinates: 0
     # One intermol + one diss: 1*4 = 4
     # One intermol + one intramol formation = 1*4 = 4
     # Sum: 9
     assert n_trials == 9
 
     # No intramolecular reactive pairs in H2O
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
     n_trials = trial_generator.estimate_n_bimolecular_trials(
         structure_file1,
         structure_file2,
         attack_points_per_site=2,
         n_inter_reactive_pairs=1,
         n_reactive_bound_pairs1=2,
         n_reactive_unbound_pairs2=0,
@@ -957,12 +1311,12 @@
     # Two intermol coordinates: 0
     # One intermol + one diss: 1*4 = 4
     # One intermol + one intramol formation = 1*3 = 3
     # Sum: 8
     assert n_trials == 8
 
     # No reactive intermolecular pairs
-    trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_options.complex_generator.options.multiple_attack_points = False
     n_trials = trial_generator.estimate_n_bimolecular_trials(
         structure_file1, structure_file2, attack_points_per_site=2, n_inter_reactive_pairs=0
     )
     assert n_trials == 0
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_connectivity_analyzer.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_connectivity_analyzer.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_fast_dissociations.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_fast_dissociations.py`

 * *Files 12% similar despite different names*

```diff
@@ -107,14 +107,21 @@
     # Run a second time
     trial_generator.unimolecular_reactions(structure)
     # Check again
     assert not structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     hits = calculations.query_calculations(json.dumps({}))
     assert len(hits) == 10
 
+    # Run a third time with exact settings check
+    trial_generator.unimolecular_reactions(structure, with_exact_settings_check=True)
+    # Check again
+    assert not structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
+    hits = calculations.query_calculations(json.dumps({}))
+    assert len(hits) == 10
+
     # with dissociative explorations
     trial_generator.options.always_further_explore_dissociative_reactions = True
     trial_generator.unimolecular_reactions(structure)
     assert not structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     more_hits = calculations.query_calculations(json.dumps({}))
     # Expect previous 10 + 6 C-C bonds
     assert len(more_hits) == 16
@@ -236,37 +243,35 @@
         assert len(calculation.get_structures()) == 1
         assert calculation.get_status() == db.Status.HOLD
         assert calculation.get_job().order in ["scine_dissociation_cut", "scine_react_complex_nt2"]
         assert calculation.get_model() == model
         n_diss = calculation.get_settings().get("dissociations")
         n_diss_nt = calculation.get_settings().get("nt_nt_dissociations")
         assert n_diss is None and len(n_diss_nt) == 4 or len(n_diss) == 4 and n_diss_nt is None
-        # Cleaning
-        calculation.wipe()
 
     """ 0-2 """
     trial_generator.options.always_further_explore_dissociative_reactions = False
     trial_generator.options.enable_further_explorations = False
     # Try one or two dissociations at once
     trial_generator.options.min_bond_dissociations = 0
     trial_generator.options.max_bond_dissociations = 2
     # Generate trials
-    trial_generator.unimolecular_reactions(structure)
+    trial_generator.unimolecular_reactions(structure, with_exact_settings_check=True)
 
     # Expected number of hits
     # Single dissociations = 10 C-H bonds
-    # Double dissociations = number of bonds choose 2 = 16 choose 2 = 120
-    # Sum: 130
+    # Double dissociations = number of bonds choose 2 = 16 choose 2 = 120, but already done
+    # Sum: 10 + 240 = 250
     trial_generator.unimolecular_reactions(structure)
     hits = calculations.query_calculations(json.dumps({}))
-    assert len(hits) == 130
+    assert len(hits) == 250
     # Run a second time
     trial_generator.unimolecular_reactions(structure)
     hits = calculations.query_calculations(json.dumps({}))
-    assert len(hits) == 130
+    assert len(hits) == 250
 
     # with dissociative explorations
     trial_generator.options.always_further_explore_dissociative_reactions = True
     trial_generator.unimolecular_reactions(structure)
     assert not structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     more_hits = calculations.query_calculations(json.dumps({}))
     # 6 C-C pure single dissociations
@@ -277,40 +282,22 @@
     assert len(more_hits) == len(hits) + 6
 
     # with further explorations
     trial_generator.options.enable_further_explorations = True
     trial_generator.unimolecular_reactions(structure)
     assert not structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     most_hits = calculations.query_calculations(json.dumps({}))
-    assert len(most_hits) == len(hits) + len(more_hits)
+    # 10 new fast + 6 pure single dissociations
+    assert len(most_hits) == 250 + 10 + 6
     # Run a second time
     trial_generator.unimolecular_reactions(structure)
     most_hits = calculations.query_calculations(json.dumps({}))
-    assert len(most_hits) == len(hits) + len(more_hits)
-
-    for hit in hits:
-        calculation = db.Calculation(hit.id(), calculations)
-        assert len(calculation.get_structures()) == 1
-        assert calculation.get_status() == db.Status.HOLD
-        assert calculation.get_model() == model
-        assert calculation.get_job().order == "scine_dissociation_cut"
-        n_diss = len(calculation.get_setting("dissociations"))
-        assert n_diss in (2, 4)
-
-    for hit in more_hits:
-        calculation = db.Calculation(hit.id(), calculations)
-        assert len(calculation.get_structures()) == 1
-        assert calculation.get_status() == db.Status.HOLD
-        assert calculation.get_job().order in ["scine_dissociation_cut", "scine_react_complex_nt2"]
-        assert calculation.get_model() == model
-        n_diss = calculation.get_settings().get("dissociations")
-        n_diss_nt = calculation.get_settings().get("nt_nt_dissociations")
-        assert n_diss is None and len(n_diss_nt) in (2, 4) or len(n_diss) in (2, 4) and n_diss_nt is None
+    assert len(most_hits) == 250 + 10 + 6
 
-    for hit in most_hits:
+    for hit in hits + more_hits + most_hits:
         calculation = db.Calculation(hit.id(), calculations)
         assert len(calculation.get_structures()) == 1
         assert calculation.get_status() == db.Status.HOLD
         assert calculation.get_job().order in ["scine_dissociation_cut", "scine_react_complex_nt2"]
         assert calculation.get_model() == model
         n_diss = calculation.get_settings().get("dissociations")
         n_diss_nt = calculation.get_settings().get("nt_nt_dissociations")
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_fragment_based.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/trial_generator/test_fragment_based.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,19 +51,19 @@
         structure.set_aggregate(compound.id())
         structure_list.append(structure)
 
     # Set up trial generator
     trial_generator = FragmentBased()
     trial_generator.initialize_collections(manager)
     trial_generator.options.model = model
-    trial_generator.options.bimolecular_association.complex_generator.options.number_rotamers = 1
-    trial_generator.options.bimolecular_association.complex_generator.options.number_rotamers_two_on_two = 1
-    trial_generator.options.bimolecular_association.complex_generator.options.multiple_attack_points = False
-    trial_generator.options.bimolecular_association.consider_diatomic_fragments = True
-    trial_generator.options.bimolecular_association.max_within_fragment_graph_distance = 1
+    trial_generator.options.bimolecular_association_options.complex_generator.options.number_rotamers = 1
+    trial_generator.options.bimolecular_association_options.complex_generator.options.number_rotamers_two_on_two = 1
+    trial_generator.options.bimolecular_association_options.complex_generator.options.multiple_attack_points = False
+    trial_generator.options.bimolecular_association_options.consider_diatomic_fragments = True
+    trial_generator.options.bimolecular_association_options.max_within_fragment_graph_distance = 1
     # Generate trials
     trial_generator.bimolecular_reactions(structure_list)
 
     # Checks
     hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     assert len(hits) == 0
 
@@ -112,14 +112,16 @@
         lhs = calculation.get_setting("nt_nt_lhs_list")
         assert len(lhs) in (1, 2)  # monoatomic and diatomic fragments
         rhs = calculation.get_setting("nt_nt_rhs_list")
         assert len(rhs) in (1, 2)  # monoatomic and diatomic fragments
         assert len(set(lhs)) == len(lhs)
         assert len(set(rhs)) == len(rhs)
         calculation.wipe()
+    for s in structure_list:
+        s.clear_calculations("scine_react_complex_nt")
 
     # Reset model
     trial_generator.options.model = model
 
     # Tests with filters
     class AtomFilter(ReactiveSiteFilter):
         """
@@ -155,14 +157,16 @@
         lhs = calculation.get_setting("nt_nt_lhs_list")
         assert len(lhs) == 1
         rhs = calculation.get_setting("nt_nt_rhs_list")
         assert len(rhs) == 1  # monoatomic and diatomic fragments
         assert len(set(lhs)) == len(lhs)
         assert len(set(rhs)) == len(rhs)
         calculation.wipe()
+    for s in structure_list:
+        s.clear_calculations("scine_react_complex_nt")
 
     class PairFilter(ReactiveSiteFilter):
         """
         A reactive site filter implementing only a filter for atom pairs.
         Only O-O pairs are considered as reactive.
         """
 
@@ -197,14 +201,16 @@
         lhs = calculation.get_setting("nt_nt_lhs_list")
         assert len(lhs) in (1, 2)
         rhs = calculation.get_setting("nt_nt_rhs_list")
         assert len(rhs) in (1, 2)  # monoatomic and diatomic fragments
         assert len(set(lhs)) == len(lhs)
         assert len(set(rhs)) == len(rhs)
         calculation.wipe()
+    for s in structure_list:
+        s.clear_calculations("scine_react_complex_nt")
 
     class CoordinateFilter(ReactiveSiteFilter):
         """
         A reactive site filter implementing only a filter for reaction
         coordinate.
         Only O-O bonds combined with an O atom are to be considered as reactive
         """
@@ -246,14 +252,16 @@
         lhs = calculation.get_setting("nt_nt_lhs_list")
         assert len(lhs) in (1, 2)
         rhs = calculation.get_setting("nt_nt_rhs_list")
         assert len(rhs) in (1, 2)  # monoatomic and diatomic fragments
         assert len(set(lhs)) == len(lhs)
         assert len(set(rhs)) == len(rhs)
         calculation.wipe()
+    for s in structure_list:
+        s.clear_calculations("scine_react_complex_nt")
 
     class ImpossibleFilter(ReactiveSiteFilter):
         """
         A reactive site filter allowing only H atoms to be reactive and
         O-O reactive pairs, i.e., ultimately no reaction coordinates will be
         generated.
         """
@@ -318,16 +326,16 @@
         compound.add_structure(structure.id())
         structure.set_aggregate(compound.id())
 
     # Set up trial generator
     trial_generator = FragmentBased()
     trial_generator.initialize_collections(manager)
     trial_generator.options.model = model
-    trial_generator.options.unimolecular_dissociation.enabled = True
-    trial_generator.options.unimolecular_association.enabled = False
+    trial_generator.options.unimolecular_dissociation_options.enabled = True
+    trial_generator.options.unimolecular_association_options.enabled = False
 
     # Generate trials
     trial_generator.unimolecular_reactions(structure)
 
     # Checks
     hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     assert len(hits) == 0
@@ -349,14 +357,15 @@
         assert calculation.get_model() == model
         lhs = calculation.get_setting("nt_nt_lhs_list")
         assert len(lhs) == 1
         rhs = calculation.get_setting("nt_nt_rhs_list")
         assert len(rhs) == 1
         assert len(set(lhs + rhs)) == len(rhs) + len(lhs)
         calculation.wipe()
+    structure.clear_calculations("scine_react_complex_nt")
 
     # Test with filter
 
     class AtomFilter(ReactiveSiteFilter):
         """
         A reactive site filter allowing only carbon atoms to be reactive
         """
@@ -387,14 +396,15 @@
         assert calculation.get_model() == model
         lhs = calculation.get_setting("nt_nt_lhs_list")
         assert len(lhs) == 1
         rhs = calculation.get_setting("nt_nt_rhs_list")
         assert len(rhs) == 1
         assert len(set(lhs + rhs)) == len(rhs) + len(lhs)
         calculation.wipe()
+    structure.clear_calculations("scine_react_complex_nt")
 
     class PairFilter(ReactiveSiteFilter):
         """
         A reactive site filter allowing only C-C pairs to be dissociated
         """
 
         def filter_atom_pairs(
@@ -425,14 +435,15 @@
         assert calculation.get_model() == model
         lhs = calculation.get_setting("nt_nt_lhs_list")
         assert len(lhs) == 1
         rhs = calculation.get_setting("nt_nt_rhs_list")
         assert len(rhs) == 1
         assert len(set(lhs + rhs)) == len(rhs) + len(lhs)
         calculation.wipe()
+    structure.clear_calculations("scine_react_complex_nt")
 
     class CoordinateFilter(ReactiveSiteFilter):
         """
         A reactive site filter implementing only a filter for reaction
         coordinate.
         Only C-H bonds are considered as reactive.
         """
@@ -465,14 +476,15 @@
         assert calculation.get_model() == model
         lhs = calculation.get_setting("nt_nt_lhs_list")
         assert len(lhs) == 1
         rhs = calculation.get_setting("nt_nt_rhs_list")
         assert len(rhs) == 1
         assert len(set(lhs + rhs)) == len(rhs) + len(lhs)
         calculation.wipe()
+    structure.clear_calculations("scine_react_complex_nt")
 
     class CombinedFilter(ReactiveSiteFilter):
         """
         A reactive site filter allowing for C atoms and C-C bonds to be reactive
         """
 
         def filter_atoms(self, structure_list: List[db.Structure], atom_indices: List[int]) -> List[int]:
@@ -554,17 +566,17 @@
         compound.add_structure(structure.id())
         structure.set_aggregate(compound.id())
 
     # Set up trial generator
     trial_generator = FragmentBased()
     trial_generator.initialize_collections(manager)
     trial_generator.options.model = model
-    trial_generator.options.unimolecular_dissociation.enabled = False
-    trial_generator.options.unimolecular_association.enabled = True
-    trial_generator.options.unimolecular_association.consider_diatomic_fragments = False
+    trial_generator.options.unimolecular_dissociation_options.enabled = False
+    trial_generator.options.unimolecular_association_options.enabled = True
+    trial_generator.options.unimolecular_association_options.consider_diatomic_fragments = False
 
     # Generate trials
     trial_generator.unimolecular_reactions(structure)
 
     # Checks
     hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     assert len(hits) == 0
@@ -631,21 +643,21 @@
         compound.add_structure(structure.id())
         structure.set_aggregate(compound.id())
 
     # Set up trial generator
     trial_generator = FragmentBased()
     trial_generator.initialize_collections(manager)
     trial_generator.options.model = model
-    trial_generator.options.unimolecular_dissociation.enabled = False
-    trial_generator.options.unimolecular_association.enabled = True
-    trial_generator.options.unimolecular_association.min_inter_fragment_graph_distance = 2
-    trial_generator.options.unimolecular_association.max_inter_fragment_graph_distance = 999
+    trial_generator.options.unimolecular_dissociation_options.enabled = False
+    trial_generator.options.unimolecular_association_options.enabled = True
+    trial_generator.options.unimolecular_association_options.min_inter_fragment_graph_distance = 2
+    trial_generator.options.unimolecular_association_options.max_inter_fragment_graph_distance = 999
     # Enable bond on bond
-    trial_generator.options.unimolecular_association.consider_diatomic_fragments = True
-    trial_generator.options.unimolecular_association.max_within_fragment_graph_distance = 1
+    trial_generator.options.unimolecular_association_options.consider_diatomic_fragments = True
+    trial_generator.options.unimolecular_association_options.max_within_fragment_graph_distance = 1
 
     # Generate trials
     trial_generator.unimolecular_reactions(structure)
 
     # Checks
     hits = structures.query_structures(json.dumps({"label": "reactive_complex_guess"}))
     assert len(hits) == 0
@@ -675,14 +687,15 @@
         assert calculation.get_model() == model
         lhs = calculation.get_setting("nt_nt_lhs_list")
         assert len(lhs) in (1, 2)
         rhs = calculation.get_setting("nt_nt_rhs_list")
         assert len(rhs) in (1, 2)
         assert len(set(lhs + rhs)) == len(rhs) + len(lhs)
         calculation.wipe()
+    structure.clear_calculations("scine_react_complex_nt")
 
     # Test with filter
     class AtomFilter(ReactiveSiteFilter):
         """
         A reactive site filter allowing only hydrogen atoms to be reactive
         """
 
@@ -693,17 +706,15 @@
                 elements += struct.get_atoms().elements
             for i in atom_indices:
                 if elements[i] == utils.ElementType.H:
                     reactive_atoms.append(i)
             return reactive_atoms
 
     trial_generator.reactive_site_filter = AtomFilter()
-
     trial_generator.unimolecular_reactions(structure)
-    hits = calculations.query_calculations(json.dumps({}))
 
     # Only H on H allowed
     hits = calculations.query_calculations(json.dumps({}))
     assert len(hits) == 1
     for hit in hits:
         calculation = db.Calculation(hit.id())
         calculation.link(calculations)
@@ -713,14 +724,15 @@
         assert calculation.get_model() == model
         lhs = calculation.get_setting("nt_nt_lhs_list")
         assert len(lhs) == 1
         rhs = calculation.get_setting("nt_nt_rhs_list")
         assert len(rhs) == 1
         assert len(set(lhs + rhs)) == len(rhs) + len(lhs)
         calculation.wipe()
+    structure.clear_calculations("scine_react_complex_nt")
 
     class PairFilter(ReactiveSiteFilter):
         """
         A reactive site filter allowing only pairs with at least one oxygen
         atom to be reactive
         """
 
@@ -735,15 +747,14 @@
                 if utils.ElementType.O in (elements[pair[0]], elements[pair[1]]):
                     reactive_pairs.append(pair)
             return reactive_pairs
 
     trial_generator.reactive_site_filter = PairFilter()
 
     trial_generator.unimolecular_reactions(structure)
-    hits = calculations.query_calculations(json.dumps({}))
     # Expected number of hits for H1-O1-O2-H2
     # atom on atom:  2 (H1 <-> O2, H2 <-> O1)
     # atom on bond:  0 (would be H on H-O in brute force approach i.e. there is always an H-H reactive pair)
     # bond on bond:  0 (H1-O1 and H2-O2 do not conform to minimum interfragment distance due to O-O bond)
     # Sum:           2
     hits = calculations.query_calculations(json.dumps({}))
     assert len(hits) == 2
@@ -756,14 +767,15 @@
         assert calculation.get_model() == model
         lhs = calculation.get_setting("nt_nt_lhs_list")
         assert len(lhs) == 1
         rhs = calculation.get_setting("nt_nt_rhs_list")
         assert len(rhs) == 1
         assert len(set(lhs + rhs)) == len(rhs) + len(lhs)
         calculation.wipe()
+    structure.clear_calculations("scine_react_complex_nt")
 
     class CoordinateFilter(ReactiveSiteFilter):
         """
         A reactive site filter allowing only coordinates with three distinct
         atoms
         """
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/test_brute_force.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/test_brute_force.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/gears/elementary_steps/test_further_dissociations_reactive_site_filters.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/gears/elementary_steps/test_further_dissociations_reactive_site_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,19 @@
         allowed_coordinates = f.filter_reaction_coordinates(self.structure, self.test_coordinate)
         assert not allowed_coordinates
 
         step.set_type(db.ElementaryStepType.BARRIERLESS)
         allowed_coordinates = f.filter_reaction_coordinates(self.structure, self.test_coordinate)
         assert len(allowed_coordinates) == len(self.test_coordinate)
 
+        # respects disable
+        step.disable_exploration()
+        allowed_coordinates = f.filter_reaction_coordinates(self.structure, self.test_coordinate)
+        assert not allowed_coordinates
+
         # wrong coordinate is still outruled
         allowed_coordinates = f.filter_reaction_coordinates(self.structure, [[(0, 1), (1, 5)]])
         assert not allowed_coordinates
 
     def test_reaction_coordinate_max_dissociation_energy_filter(self):
         energy_type = 'gibbs_free_energy'
         f = ReactionCoordinateMaxDissociationEnergyFilter(100.0, energy_type, self.structure.get_model(),
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/gears/test_compound.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/gears/test_compound.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,565 +3,564 @@
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
 import os
-from json import dumps
+from json import dumps, load
+import unittest
 
 # Third party imports
+import pytest
 import scine_database as db
 
 # Local application tests imports
 from .. import test_database_setup as db_setup
+from ...gears import HoldsCollections
 from ..resources import resources_root_path
 
 # Local application imports
 from ...engine import Engine
 from ...gears.compound import BasicAggregateHousekeeping
 
 
-def test_compound_creation():
-    # Connect to test DB
-    manager = db_setup.get_clean_db("chemoton_test_compound_creation")
-
-    # Get collections
-    structures = manager.get_collection("structures")
-    compounds = manager.get_collection("compounds")
-
-    # Add structure data
-    model = db.Model("FAKE", "FAKE", "F-AKE")
-    rr = resources_root_path()
-    for label in [db.Label.MINIMUM_OPTIMIZED, db.Label.USER_OPTIMIZED]:
-        # Setup clean db
-        manager.init()
+class CompoundTests(unittest.TestCase, HoldsCollections):
 
+    def custom_setup(self, manager: db.Manager) -> None:
+        self._required_collections = ["manager", "elementary_steps", "structures", "calculations",
+                                      "reactions", "compounds", "flasks", "properties"]
+        self.initialize_collections(manager)
+
+    def tearDown(self) -> None:
+        self._manager.wipe()
+
+    def test_compound_creation(self):
+        # Connect to test DB
+        manager = db_setup.get_clean_db("chemoton_test_compound_creation")
+        self.custom_setup(manager)
+
+        # Add structure data
+        model = db.Model("FAKE", "FAKE", "F-AKE")
+        rr = resources_root_path()
+        for label in [db.Label.MINIMUM_OPTIMIZED, db.Label.USER_OPTIMIZED]:
+            # Setup clean database
+            manager.init()
+
+            structure = db.Structure()
+            structure.link(self._structures)
+            structure.create(os.path.join(rr, "water.xyz"), 0, 1)
+            structure.set_label(label)
+            structure.set_graph("masm_cbor_graph",
+                                "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAW"
+                                "FzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
+                                )
+            structure.set_graph("masm_decision_list", "")
+            structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+
+            structure_2 = db.Structure()
+            structure_2.link(self._structures)
+            structure_2.create(os.path.join(rr, "water.xyz"), 1, 2)
+            structure_2.set_label(db.Label.MINIMUM_OPTIMIZED)
+            structure_2.set_graph("masm_cbor_graph",
+                                  "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAW"
+                                  "FzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
+                                  )
+            structure_2.set_graph("masm_decision_list", "(181,182,183,1)")
+            structure_2.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+
+            structure_3 = db.Structure()
+            structure_3.link(self._structures)
+            structure_3.create(os.path.join(rr, "water.xyz"), 0, 3)
+            structure_3.set_label(db.Label.MINIMUM_OPTIMIZED)
+            structure_3.set_graph("masm_cbor_graph",
+                                  "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAW"
+                                  "FzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
+                                  )
+            structure_3.set_graph("masm_decision_list", "(181,182,183,1)")
+            structure_3.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+
+            # Setup gear
+            compound_gear = BasicAggregateHousekeeping()
+            compound_gear.options.model = model
+            compound_engine = Engine(manager.get_credentials(), fork=False)
+            compound_engine.set_gear(compound_gear)
+
+            # Run a single loop
+            compound_engine.run(single=True)
+
+            # Checks
+            hits = self._compounds.query_compounds(dumps({}))
+            assert len(hits) == 3
+
+            all_structure_ids = [structure.id(), structure_2.id(), structure_3.id()]
+            for compound in self._compounds.iterate_all_compounds():
+                compound.link(self._compounds)
+                assert len(compound.get_structures()) == 1
+                assert compound.get_structures()[0] in all_structure_ids
+                assert compound.get_centroid() in all_structure_ids
+            for struc in [structure, structure_2, structure_3]:
+                assert struc.has_aggregate()
+
+            # Wipe database before starting next loop
+            manager.wipe()
+
+    def test_compound_extension(self):
+        # Connect to test DB
+        manager = db_setup.get_clean_db("chemoton_test_compound_extension")
+        self.custom_setup(manager)
+
+        # Add fake data
+        model = db.Model("FAKE", "FAKE", "F-AKE")
+        rr = resources_root_path()
+        centroid = db.Structure()
+        centroid.link(self._structures)
+        centroid.create(os.path.join(rr, "water.xyz"), 0, 1)
+        centroid.set_label(db.Label.USER_OPTIMIZED)
+        centroid.set_graph("masm_cbor_graph",
+                           "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAW"
+                           "FzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
+                           )
+        centroid.set_graph("masm_decision_list", "(1,2,3,1)")
+        centroid.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
         structure = db.Structure()
-        structure.link(structures)
+        structure.link(self._structures)
         structure.create(os.path.join(rr, "water.xyz"), 0, 1)
-        structure.set_label(label)
-        structure.set_graph("masm_cbor_graph", "asdfghjkl")
+        structure.set_label(db.Label.MINIMUM_OPTIMIZED)
+        structure.set_graph("masm_cbor_graph",
+                            "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAW"
+                            "FzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
+                            )
+        structure.set_graph("masm_decision_list", "(181,182,183,1)")
+        structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+
+        compound = db.Compound()
+        compound.link(self._compounds)
+        compound.create([centroid.id()])
+        centroid.set_aggregate(compound.id())
+
+        # Setup gear
+        compound_gear = BasicAggregateHousekeeping()
+        compound_gear.options.model = model
+        compound_engine = Engine(manager.get_credentials(), fork=False)
+        compound_engine.set_gear(compound_gear)
+
+        # Run a single loop
+        compound_engine.run(single=True)
+
+        # Checks
+        assert len(compound.get_structures()) == 2
+        assert compound.get_structures()[1].string() == structure.id().string()
+        assert compound.get_centroid().string() == centroid.id().string()
+        assert structure.has_aggregate()
+        assert structure.get_aggregate().string() == compound.id().string()
+        assert structure.get_label() == db.Label.MINIMUM_OPTIMIZED
+
+    def test_intermediate_deduplication(self):
+        # Connect to test DB
+        manager = db_setup.get_clean_db("chemoton_test_intermediate_deduplication")
+        self.custom_setup(manager)
+
+        # Add fake data
+        model = db.Model("FAKE", "FAKE", "F-AKE")
+        rr = resources_root_path()
+        centroid = db.Structure()
+        centroid.link(self._structures)
+        centroid.create(os.path.join(rr, "water.xyz"), 0, 1)
+        centroid.set_label(db.Label.MINIMUM_OPTIMIZED)
+        centroid.set_graph("masm_cbor_graph",
+                           "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWF"
+                           "zAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
+                           )
+        centroid.set_graph("masm_decision_list", "(10,20,40,1):(110,120,140,1)")
+        centroid.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+        structure = db.Structure()
+        structure.link(self._structures)
+        structure.create(os.path.join(rr, "water.xyz"), 0, 1)
+        structure.set_label(db.Label.MINIMUM_OPTIMIZED)
+        structure.set_graph("masm_cbor_graph",
+                            "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWF"
+                            "zAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
+                            )
+        structure.set_graph("masm_decision_list", "(10,30,40,1):(110,130,140,1)")
+        structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+        compound = db.Compound()
+        compound.link(self._compounds)
+        compound.create([centroid.id()])
+        centroid.set_aggregate(compound.id())
+
+        # Setup gear
+        compound_gear = BasicAggregateHousekeeping()
+        compound_gear.options.model = model
+        compound_engine = Engine(manager.get_credentials(), fork=False)
+        compound_engine.set_gear(compound_gear)
+
+        # Run a single loop
+        compound_engine.run(single=True)
+
+        # Checks
+        assert len(compound.get_structures()) == 1  # duplicate are not added to aggregate
+        assert compound.get_centroid().string() == centroid.id().string()
+        # but we can still use aggregate methods on the structure
+        assert not structure.has_aggregate(recursive=False)
+        assert structure.has_aggregate()
+        assert structure.get_aggregate().string() == compound.id().string()
+        assert structure.get_label() == db.Label.DUPLICATE
+        assert structure.get_original() == centroid.id()
+
+    def test_intermediate_deduplication_empty_dlist(self):
+        # Connect to test DB
+        manager = db_setup.get_clean_db("chemoton_test_intermediate_deduplication_empty_dlist")
+        self.custom_setup(manager)
+
+        # Add fake data
+        model = db.Model("FAKE", "FAKE", "F-AKE")
+        rr = resources_root_path()
+        centroid = db.Structure()
+        centroid.link(self._structures)
+        centroid.create(os.path.join(rr, "water.xyz"), 0, 1)
+        centroid.set_label(db.Label.MINIMUM_OPTIMIZED)
+        centroid.set_graph("masm_cbor_graph",
+                           "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWFzAWF"
+                           "jD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
+                           )
+        centroid.set_graph("masm_decision_list", "")
+        centroid.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+        structure = db.Structure()
+        structure.link(self._structures)
+        structure.create(os.path.join(rr, "water.xyz"), 0, 1)
+        structure.set_label(db.Label.MINIMUM_OPTIMIZED)
+        structure.set_graph("masm_cbor_graph",
+                            "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWFzAWF"
+                            "jD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
+                            )
         structure.set_graph("masm_decision_list", "")
         structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+        compound = db.Compound()
+        compound.link(self._compounds)
+        compound.create([centroid.id()])
+        centroid.set_aggregate(compound.id())
+
+        # Setup gear
+        compound_gear = BasicAggregateHousekeeping()
+        compound_gear.options.model = model
+        compound_engine = Engine(manager.get_credentials(), fork=False)
+        compound_engine.set_gear(compound_gear)
+
+        # Run a single loop
+        compound_engine.run(single=True)
+
+        # Checks
+        assert len(compound.get_structures()) == 1  # duplicate are not added to aggregate
+        assert compound.get_centroid().string() == centroid.id().string()
+        # but we can still use aggregate methods on the structure
+        assert structure.has_aggregate()
+        assert structure.get_aggregate().string() == compound.id().string()
+        assert structure.get_label() == db.Label.DUPLICATE
+        assert structure.get_original() == centroid.id()
+
+    @pytest.mark.filterwarnings("ignore:.+received incorrect label:UserWarning")
+    def test_irrelevant_structure(self):
+        # Connect to test DB
+        manager = db_setup.get_clean_db("chemoton_test_irrelevant_structure")
+        self.custom_setup(manager)
+
+        # Add structure data
+        model = db.Model("FAKE", "FAKE", "F-AKE")
+        rr = resources_root_path()
+        structure = db.Structure()
+        structure.link(self._structures)
+        structure.create(os.path.join(rr, "water.xyz"), 0, 1)
+        structure.set_label(db.Label.MINIMUM_OPTIMIZED)
+        structure.set_graph("masm_cbor_graph",
+                            "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWF"
+                            "zAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
+                            )
+        structure.set_graph("masm_decision_list", "(10,30,40,1)")
+        structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+
+        starting_structure = db.Structure(db.ID(), self._structures)
+        starting_structure.create(os.path.join(rr, "water.xyz"), 0, 1)
+        starting_structure.set_label(db.Label.MINIMUM_OPTIMIZED)
+        starting_structure.set_graph("masm_cbor_graph", "original")
+        starting_structure.set_aggregate(db.ID())
+
+        minimization = db.Calculation(db.ID(), manager.get_collection("calculations"))
+        minimization.create(model, db.Job("scine_geometry_optimization"), [starting_structure.id()])
+        results = db.Results()
+        results.add_structure(structure.id())
+        minimization.set_results(results)
+        minimization.set_status(db.Status.COMPLETE)
+
+        # Setup gear
+        compound_gear = BasicAggregateHousekeeping()
+        compound_gear.options.model = model
+        compound_gear.options.graph_job = db.Job("testy_mac_test_face")
+        compound_engine = Engine(manager.get_credentials(), fork=False)
+        compound_engine.set_gear(compound_gear)
+
+        # Run a single loop
+        compound_engine.run(single=True)
+
+        assert not structure.has_aggregate()
+        assert structure.get_label() == db.Label.IRRELEVANT
+
+    def test_graph_job_setup(self):
+        # Connect to test DB
+        manager = db_setup.get_clean_db("chemoton_test_graph_job_setup")
+        self.custom_setup(manager)
+
+        # Add structure data
+        model = db.Model("FAKE", "FAKE", "F-AKE")
+        rr = resources_root_path()
+        structure = db.Structure()
+        structure.link(self._structures)
+        structure.create(os.path.join(rr, "water.xyz"), 0, 1)
+        structure.set_label(db.Label.MINIMUM_OPTIMIZED)
+        structure.add_property("bond_orders", db.ID())
+
+        # Setup gear
+        compound_gear = BasicAggregateHousekeeping()
+        compound_gear.options.model = model
+        compound_gear.options.graph_job = db.Job("testy_mac_test_face")
+        compound_engine = Engine(manager.get_credentials(), fork=False)
+        compound_engine.set_gear(compound_gear)
 
-        structure_2 = db.Structure()
-        structure_2.link(structures)
-        structure_2.create(os.path.join(rr, "water.xyz"), +1, 2)
-        structure_2.set_label(db.Label.MINIMUM_OPTIMIZED)
-        structure_2.set_graph("masm_cbor_graph",
-                              "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAW"
-                              "FzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
-                              )
-        structure_2.set_graph("masm_decision_list", "(181,182,183,1)")
+        # Run a single loop
+        compound_engine.run(single=True)
+
+        # Checks
+        hits = self._calculations.query_calculations(dumps({}))
+        assert len(hits) == 1
+
+        calculation = db.Calculation(hits[0].id())
+        calculation.link(self._calculations)
+
+        assert len(calculation.get_structures()) == 1
+        assert calculation.get_structures()[0].string() == structure.id().string()
+        assert calculation.get_status() == db.Status.HOLD
+        assert calculation.get_job().order == "testy_mac_test_face"
+
+        # Run a second time
+        compound_engine.run(single=True)
+        hits = self._calculations.query_calculations(dumps({}))
+        assert len(hits) == 1
+
+        # Rerun with a different model
+        model2 = db.Model("FAKE2", "", "")
+        compound_gear.options.model = model2
+        compound_engine.run(single=True)
+        hits = self._calculations.query_calculations(dumps({}))
+        assert len(hits) == 2
+
+    def test_bo_job_setup(self):
+        # Connect to test DB
+        manager = db_setup.get_clean_db("chemoton_test_bo_job_setup")
+        self.custom_setup(manager)
+
+        # Add structure data
+        model = db.Model("FAKE", "FAKE", "F-AKE")
+        rr = resources_root_path()
+        structure = db.Structure()
+        structure.link(self._structures)
+        structure.create(os.path.join(rr, "water.xyz"), 0, 1)
+        structure.set_label(db.Label.MINIMUM_OPTIMIZED)
+
+        # Setup gear
+        compound_gear = BasicAggregateHousekeeping()
+        compound_gear.options.model = model
+        compound_gear.options.bond_order_job = db.Job("eggs_bacon_and_spam")
+        compound_engine = Engine(manager.get_credentials(), fork=False)
+        compound_engine.set_gear(compound_gear)
+
+        # Run a single loop
+        compound_engine.run(single=True)
+
+        # Checks
+        hits = self._calculations.query_calculations(dumps({}))
+        assert len(hits) == 1
+
+        calculation = db.Calculation(hits[0].id())
+        calculation.link(self._calculations)
+
+        assert len(calculation.get_structures()) == 1
+        assert calculation.get_structures()[0].string() == structure.id().string()
+        assert calculation.get_status() == db.Status.HOLD
+        assert calculation.get_job().order == "eggs_bacon_and_spam"
+
+        # Run a second time
+        compound_engine.run(single=True)
+        hits = self._calculations.query_calculations(dumps({}))
+        assert len(hits) == 1
+
+        # Rerun with a different model
+        model2 = db.Model("FAKE2", "", "")
+        compound_gear.options.model = model2
+        compound_engine.run(single=True)
+        hits = self._calculations.query_calculations(dumps({}))
+        assert len(hits) == 2
+
+    def test_flask_creation(self):
+        # Connect to test DB
+        manager = db_setup.get_clean_db("chemoton_test_flask_creation")
+        self.custom_setup(manager)
+
+        # Add structure data
+        model = db.Model("FAKE", "", "")
+        rr = resources_root_path()
+        structure = db.Structure()
+        structure.link(self._structures)
+        structure.create(os.path.join(rr, "proline_propanal_complex.xyz"), 0, 1)
+        structure.set_label(db.Label.COMPLEX_OPTIMIZED)
+        graph = load(open(os.path.join(rr, "proline_propanal_complex.json"), "r"))
+        structure.set_graph("masm_cbor_graph", graph["masm_cbor_graph"])
+        structure.set_graph("masm_idx_map", graph["masm_idx_map"])
+        structure.set_graph("masm_decision_list", graph["masm_decision_list"])
+
+        # Setup gear
+        compound_gear = BasicAggregateHousekeeping()
+        compound_gear.options.model = model
+        compound_engine = Engine(manager.get_credentials(), fork=False)
+        compound_engine.set_gear(compound_gear)
+
+        # Run a single loop
+        compound_engine.run(single=True)
+
+        # Checks
+        hits = self._flasks.query_flasks(dumps({}))
+        assert len(hits) == 1
+
+        flask = db.Flask(hits[0].id())
+        flask.link(self._flasks)
+
+        assert len(flask.get_structures()) == 1
+        assert flask.get_structures()[0].string() == structure.id().string()
+        assert flask.get_centroid().string() == structure.id().string()
+        assert structure.has_aggregate()
+        assert structure.get_aggregate().string() == flask.id().string()
+
+    def test_flask_to_compound_mapping(self):
+        # Connect to test DB
+        manager = db_setup.get_clean_db("chemoton_test_flask_to_compound_mapping")
+        self.custom_setup(manager)
+
+        _, s_id1 = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.MINIMUM_OPTIMIZED)
+        _, s_id2 = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.MINIMUM_OPTIMIZED)
+        structure_1 = db.Structure(s_id1, self._structures)
+        structure_2 = db.Structure(s_id2, self._structures)
+        graph_1 = "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWFzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
+        graph_2 = ("pGFhgqRhYQBhYwJhcqNhbIKBAYEDYmxygoEAgQFhc4KBAYEDYXMBpGFhAGFjA2"
+                   "Fyo2FsgoEAgQJibHKCgQCBAWFzgoEAgQJhcwFhYw9hZ6JhRYODAAMAgwECAIMC"
+                   "AwBhWoQBAQgIYXaDAQAA")
+        structure_1.set_graph("masm_cbor_graph", graph_1)
+        structure_1.set_graph("masm_decision_list", "(10,30,40,1)")
+        structure_1.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+        structure_2.set_graph("masm_cbor_graph", graph_2)
+        structure_2.set_graph("masm_decision_list", "(10,30,40,1):(1, 3, 5, 8)")
         structure_2.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
 
-        structure_3 = db.Structure()
-        structure_3.link(structures)
-        structure_3.create(os.path.join(rr, "water.xyz"), 0, 3)
-        structure_3.set_label(db.Label.MINIMUM_OPTIMIZED)
-        structure_3.set_graph("masm_cbor_graph",
-                              "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAW"
-                              "FzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
-                              )
-        structure_3.set_graph("masm_decision_list", "(181,182,183,1)")
-        structure_3.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+        # Add structure data
+        model = db.Model("FAKE", "FAKE", "F-AKE")
+        rr = resources_root_path()
+        structure = db.Structure()
+        structure.link(self._structures)
+        structure.create(os.path.join(rr, "water.xyz"), 0, 1)
+        structure.set_label(db.Label.COMPLEX_OPTIMIZED)
+        structure.set_graph("masm_cbor_graph", graph_1 + ";" + graph_2)
+        structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2), (1, 3), (1, 4), (1, 5)")
 
         # Setup gear
         compound_gear = BasicAggregateHousekeeping()
         compound_gear.options.model = model
         compound_engine = Engine(manager.get_credentials(), fork=False)
         compound_engine.set_gear(compound_gear)
 
+        assert self._flasks.count(dumps({})) == 0
         # Run a single loop
         compound_engine.run(single=True)
 
         # Checks
-        hits = compounds.query_compounds(dumps({}))
-        assert len(hits) == 3
+        assert self._flasks.count(dumps({})) == 1
+        assert self._flasks.count(dumps({"compounds": {"$size": 0}})) == 1
 
-        all_structure_ids = [structure.id(), structure_2.id(), structure_3.id()]
-        for compound in compounds.iterate_all_compounds():
-            compound.link(compounds)
-            assert len(compound.get_structures()) == 1
-            assert compound.get_structures()[0] in all_structure_ids
-            assert compound.get_centroid() in all_structure_ids
-        for struc in [structure, structure_2, structure_3]:
-            assert struc.has_aggregate()
-
-        # Cleaning
-        manager.wipe()
-
-
-def test_compound_extension():
-    # Connect to test DB
-    manager = db_setup.get_clean_db("chemoton_test_compound_extension")
-
-    # Get collections
-    structures = manager.get_collection("structures")
-    compounds = manager.get_collection("compounds")
-
-    # Add fake data
-    model = db.Model("FAKE", "FAKE", "F-AKE")
-    rr = resources_root_path()
-    centroid = db.Structure()
-    centroid.link(structures)
-    centroid.create(os.path.join(rr, "water.xyz"), 0, 1)
-    centroid.set_label(db.Label.USER_OPTIMIZED)
-    centroid.set_graph("masm_cbor_graph",
-                       "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAW"
-                       "FzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
-                       )
-    centroid.set_graph("masm_decision_list", "(1,2,3,1)")
-    centroid.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-    structure = db.Structure()
-    structure.link(structures)
-    structure.create(os.path.join(rr, "water.xyz"), 0, 1)
-    structure.set_label(db.Label.MINIMUM_OPTIMIZED)
-    structure.set_graph("masm_cbor_graph",
-                        "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAW"
-                        "FzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
-                        )
-    structure.set_graph("masm_decision_list", "(181,182,183,1)")
-    structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-
-    compound = db.Compound()
-    compound.link(compounds)
-    compound.create([centroid.id()])
-    centroid.set_aggregate(compound.id())
-
-    # Setup gear
-    compound_gear = BasicAggregateHousekeeping()
-    compound_gear.options.model = model
-    compound_engine = Engine(manager.get_credentials(), fork=False)
-    compound_engine.set_gear(compound_gear)
-
-    # Run a single loop
-    compound_engine.run(single=True)
-
-    # Checks
-    assert len(compound.get_structures()) == 2
-    assert compound.get_structures()[1].string() == structure.id().string()
-    assert compound.get_centroid().string() == centroid.id().string()
-    assert structure.has_aggregate()
-    assert structure.get_aggregate().string() == compound.id().string()
-    assert structure.get_label() == db.Label.MINIMUM_OPTIMIZED
-
-    # Cleaning
-    manager.wipe()
-
-
-def test_intermediate_deduplication():
-    # Connect to test DB
-    manager = db_setup.get_clean_db("chemoton_test_intermediate_deduplication")
-
-    # Get collections
-    model = db.Model("FAKE", "FAKE", "F-AKE")
-    structures = manager.get_collection("structures")
-    compounds = manager.get_collection("compounds")
-
-    # Add fake data
-    model = db.Model("FAKE", "FAKE", "F-AKE")
-    rr = resources_root_path()
-    centroid = db.Structure()
-    centroid.link(structures)
-    centroid.create(os.path.join(rr, "water.xyz"), 0, 1)
-    centroid.set_label(db.Label.MINIMUM_OPTIMIZED)
-    centroid.set_graph("masm_cbor_graph",
-                       "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWF"
-                       "zAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
-                       )
-    centroid.set_graph("masm_decision_list", "(10,20,40,1):(110,120,140,1)")
-    centroid.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-    structure = db.Structure()
-    structure.link(structures)
-    structure.create(os.path.join(rr, "water.xyz"), 0, 1)
-    structure.set_label(db.Label.MINIMUM_OPTIMIZED)
-    structure.set_graph("masm_cbor_graph",
-                        "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWF"
-                        "zAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
-                        )
-    structure.set_graph("masm_decision_list", "(10,30,40,1):(110,130,140,1)")
-    structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-    compound = db.Compound()
-    compound.link(compounds)
-    compound.create([centroid.id()])
-    centroid.set_aggregate(compound.id())
-
-    # Setup gear
-    compound_gear = BasicAggregateHousekeeping()
-    compound_gear.options.model = model
-    compound_engine = Engine(manager.get_credentials(), fork=False)
-    compound_engine.set_gear(compound_gear)
-
-    # Run a single loop
-    compound_engine.run(single=True)
-
-    # Checks
-    assert len(compound.get_structures()) == 2
-    assert compound.get_structures()[1].string() == structure.id().string()
-    assert compound.get_centroid().string() == centroid.id().string()
-    assert structure.has_aggregate()
-    assert structure.get_aggregate().string() == compound.id().string()
-    assert structure.get_label() == db.Label.DUPLICATE
-    assert structure.is_duplicate_of() == centroid.id()
-
-    # Cleaning
-    manager.wipe()
-
-
-def test_intermediate_deduplication_empty_dlist():
-    # Connect to test DB
-    manager = db_setup.get_clean_db("chemoton_test_intermediate_deduplication")
-
-    # Get collections
-    model = db.Model("FAKE", "FAKE", "F-AKE")
-    structures = manager.get_collection("structures")
-    compounds = manager.get_collection("compounds")
-
-    # Add fake data
-    model = db.Model("FAKE", "FAKE", "F-AKE")
-    rr = resources_root_path()
-    centroid = db.Structure()
-    centroid.link(structures)
-    centroid.create(os.path.join(rr, "water.xyz"), 0, 1)
-    centroid.set_label(db.Label.MINIMUM_OPTIMIZED)
-    centroid.set_graph("masm_cbor_graph",
-                       "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWFzAWF"
-                       "jD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
-                       )
-    centroid.set_graph("masm_decision_list", "")
-    centroid.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-    structure = db.Structure()
-    structure.link(structures)
-    structure.create(os.path.join(rr, "water.xyz"), 0, 1)
-    structure.set_label(db.Label.MINIMUM_OPTIMIZED)
-    structure.set_graph("masm_cbor_graph",
-                        "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWFzAWF"
-                        "jD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
-                        )
-    structure.set_graph("masm_decision_list", "")
-    structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-    compound = db.Compound()
-    compound.link(compounds)
-    compound.create([centroid.id()])
-    centroid.set_aggregate(compound.id())
-
-    # Setup gear
-    compound_gear = BasicAggregateHousekeeping()
-    compound_gear.options.model = model
-    compound_engine = Engine(manager.get_credentials(), fork=False)
-    compound_engine.set_gear(compound_gear)
-
-    # Run a single loop
-    compound_engine.run(single=True)
-
-    # Checks
-    assert len(compound.get_structures()) == 2
-    assert compound.get_structures()[1].string() == structure.id().string()
-    assert compound.get_centroid().string() == centroid.id().string()
-    assert structure.has_aggregate()
-    assert structure.get_aggregate().string() == compound.id().string()
-    assert structure.get_label() == db.Label.DUPLICATE
-    assert structure.is_duplicate_of() == centroid.id()
-
-    # Cleaning
-    manager.wipe()
-
-
-def test_irrelevant_structure():
-    # Connect to test DB
-    manager = db_setup.get_clean_db("chemoton_test_irrelevant_structure")
-
-    # Get collections
-    structures = manager.get_collection("structures")
-
-    # Add structure data
-    model = db.Model("FAKE", "FAKE", "F-AKE")
-    rr = resources_root_path()
-    structure = db.Structure()
-    structure.link(structures)
-    structure.create(os.path.join(rr, "water.xyz"), 0, 1)
-    structure.set_label(db.Label.MINIMUM_OPTIMIZED)
-    structure.set_graph("masm_cbor_graph",
-                        "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWF"
-                        "zAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA;"
-                        "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWF"
-                        "zAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
-                        )
-    structure.set_graph("masm_decision_list", "(10,30,40,1)")
-    structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-
-    starting_structure = db.Structure(db.ID(), structures)
-    starting_structure.create(os.path.join(rr, "water.xyz"), 0, 1)
-    starting_structure.set_label(db.Label.MINIMUM_OPTIMIZED)
-    starting_structure.set_graph("masm_cbor_graph", "original")
-    starting_structure.set_compound(db.ID())
-
-    minimization = db.Calculation(db.ID(), manager.get_collection("calculations"))
-    minimization.create(model, db.Job("scine_geometry_optimization"), [starting_structure.id()])
-    results = db.Results()
-    results.add_structure(structure.id())
-    minimization.set_results(results)
-
-    # Setup gear
-    compound_gear = BasicAggregateHousekeeping()
-    compound_gear.options.model = model
-    compound_gear.options.graph_job = db.Job("testy_mac_test_face")
-    compound_engine = Engine(manager.get_credentials(), fork=False)
-    compound_engine.set_gear(compound_gear)
-
-    # Run a single loop
-    compound_engine.run(single=True)
-
-    assert not structure.has_aggregate()
-    assert structure.get_label() == db.Label.IRRELEVANT
-
-    # Cleaning
-    manager.wipe()
-
-
-def test_graph_job_setup():
-    # Connect to test DB
-    manager = db_setup.get_clean_db("chemoton_test_graph_job_setup")
-
-    # Get collections
-    structures = manager.get_collection("structures")
-    calculations = manager.get_collection("calculations")
-
-    # Add structure data
-    model = db.Model("FAKE", "FAKE", "F-AKE")
-    rr = resources_root_path()
-    structure = db.Structure()
-    structure.link(structures)
-    structure.create(os.path.join(rr, "water.xyz"), 0, 1)
-    structure.set_label(db.Label.MINIMUM_OPTIMIZED)
-    structure.add_property("bond_orders", db.ID())
-
-    # Setup gear
-    compound_gear = BasicAggregateHousekeeping()
-    compound_gear.options.model = model
-    compound_gear.options.graph_job = db.Job("testy_mac_test_face")
-    compound_engine = Engine(manager.get_credentials(), fork=False)
-    compound_engine.set_gear(compound_gear)
-
-    # Run a single loop
-    compound_engine.run(single=True)
-
-    # Checks
-    hits = calculations.query_calculations(dumps({}))
-    assert len(hits) == 1
-
-    calculation = db.Calculation(hits[0].id())
-    calculation.link(calculations)
-
-    assert len(calculation.get_structures()) == 1
-    assert calculation.get_structures()[0].string() == structure.id().string()
-    assert calculation.get_status() == db.Status.HOLD
-    assert calculation.get_job().order == "testy_mac_test_face"
-
-    # Run a second time
-    compound_engine.run(single=True)
-    hits = calculations.query_calculations(dumps({}))
-    assert len(hits) == 1
-
-    # Rerun with a different model
-    model2 = db.Model("FAKE2", "", "")
-    compound_gear.options.model = model2
-    compound_engine.run(single=True)
-    hits = calculations.query_calculations(dumps({}))
-    assert len(hits) == 2
-
-    # Cleaning
-    manager.wipe()
-
-
-def test_bo_job_setup():
-    # Connect to test DB
-    manager = db_setup.get_clean_db("chemoton_test_bo_job_setup")
-
-    # Get collections
-    structures = manager.get_collection("structures")
-    calculations = manager.get_collection("calculations")
-
-    # Add structure data
-    model = db.Model("FAKE", "FAKE", "F-AKE")
-    rr = resources_root_path()
-    structure = db.Structure()
-    structure.link(structures)
-    structure.create(os.path.join(rr, "water.xyz"), 0, 1)
-    structure.set_label(db.Label.MINIMUM_OPTIMIZED)
-
-    # Setup gear
-    compound_gear = BasicAggregateHousekeeping()
-    compound_gear.options.model = model
-    compound_gear.options.bond_order_job = db.Job("eggs_bacon_and_spam")
-    compound_engine = Engine(manager.get_credentials(), fork=False)
-    compound_engine.set_gear(compound_gear)
-
-    # Run a single loop
-    compound_engine.run(single=True)
-
-    # Checks
-    hits = calculations.query_calculations(dumps({}))
-    assert len(hits) == 1
-
-    calculation = db.Calculation(hits[0].id())
-    calculation.link(calculations)
-
-    assert len(calculation.get_structures()) == 1
-    assert calculation.get_structures()[0].string() == structure.id().string()
-    assert calculation.get_status() == db.Status.HOLD
-    assert calculation.get_job().order == "eggs_bacon_and_spam"
-
-    # Run a second time
-    compound_engine.run(single=True)
-    hits = calculations.query_calculations(dumps({}))
-    assert len(hits) == 1
-
-    # Rerun with a different model
-    model2 = db.Model("FAKE2", "", "")
-    compound_gear.options.model = model2
-    compound_engine.run(single=True)
-    hits = calculations.query_calculations(dumps({}))
-    assert len(hits) == 2
-
-    # Cleaning
-    manager.wipe()
-
-
-def test_flask_to_compound_mapping():
-    # Connect to test DB
-    manager = db_setup.get_clean_db("chemoton_test_flask_to_compound_mapping")
-
-    # Get collections
-    structures = manager.get_collection("structures")
-    flasks = manager.get_collection("flasks")
-
-    _, s_id1 = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_OPTIMIZED)
-    _, s_id2 = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_OPTIMIZED)
-    structure_1 = db.Structure(s_id1, structures)
-    structure_2 = db.Structure(s_id2, structures)
-    graph_1 = "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWFzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
-    graph_2 = ("pGFhgqRhYQBhYwJhcqNhbIKBAYEDYmxygoEAgQFhc4KBAYEDYXMBpGFhAGFjA2"
-               "Fyo2FsgoEAgQJibHKCgQCBAWFzgoEAgQJhcwFhYw9hZ6JhRYODAAMAgwECAIMC"
-               "AwBhWoQBAQgIYXaDAQAA")
-    structure_1.set_graph("masm_cbor_graph", graph_1)
-    structure_1.set_graph("masm_decision_list", "(10,30,40,1)")
-    structure_1.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-    structure_2.set_graph("masm_cbor_graph", graph_2)
-    structure_2.set_graph("masm_decision_list", "(10,30,40,1):(1, 3, 5, 8)")
-    structure_2.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-
-    # Add structure data
-    model = db.Model("FAKE", "FAKE", "F-AKE")
-    rr = resources_root_path()
-    structure = db.Structure()
-    structure.link(structures)
-    structure.create(os.path.join(rr, "water.xyz"), 0, 1)
-    structure.set_label(db.Label.COMPLEX_OPTIMIZED)
-    structure.set_graph("masm_cbor_graph", graph_1 + ";" + graph_2)
-    structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2), (1, 3), (1, 4), (1, 5)")
-
-    # Setup gear
-    compound_gear = BasicAggregateHousekeeping()
-    compound_gear.options.model = model
-    compound_engine = Engine(manager.get_credentials(), fork=False)
-    compound_engine.set_gear(compound_gear)
-
-    assert flasks.count(dumps({})) == 0
-    # Run a single loop
-    compound_engine.run(single=True)
-
-    # Checks
-    assert flasks.count(dumps({})) == 1
-    assert flasks.count(dumps({"compounds": {"$size": 2}})) == 1
-    assert flasks.count(dumps({"compounds": {"$size": 0}})) == 0
-
-    # Run a second time
-    compound_engine.run(single=True)
-    assert flasks.count(dumps({})) == 1
-    assert flasks.count(dumps({"compounds": {"$size": 2}})) == 1
-    assert flasks.count(dumps({"compounds": {"$size": 0}})) == 0
-
-    structure = db.Structure()
-    structure.link(structures)
-    structure.create(os.path.join(rr, "water.xyz"), 0, 1)
-    structure.set_label(db.Label.COMPLEX_OPTIMIZED)
-    graph_3 = ("pWFhhqRhYQBhYwphcqRhbIOBAYELgQ1jbG5rgaJhcIIBAmNzZXGGCgsMDw4NYmxyg4EAgQGB"
-               "AmFzg4EBgQuBDWFzAqRhYQBhYwthcqRhbIOBAIEKgQxjbG5rgaJhcIIBAmNzZXGGCwoNDg8M"
-               "Ymxyg4EAgQGBAmFzg4EAgQqBDGFzAqRhYQBhYwxhcqRhbISBCIEJgQuBD2NsbmuBomFwggID"
-               "Y3NlcYYMCwoNDg9ibHKDggABgQKBA2Fzg4IICYELgQ9hcwWkYWEAYWMNYXKkYWyEgQaBB4EK"
-               "gQ5jbG5rgaJhcIICA2NzZXGGDQoLDA8OYmxyg4IAAYECgQNhc4OCBgeBCoEOYXMFpGFhAGFj"
-               "DmFypGFshIEEgQWBDYEPY2xua4GiYXCCAgNjc2Vxhg4NCgsMD2JscoOCAAGBAoEDYXODggQF"
-               "gQ2BD2FzBaRhYQBhYw9hcqRhbISBAoEDgQyBDmNsbmuBomFwggIDY3NlcYYPDAsKDQ5ibHKD"
-               "ggABgQKBA2Fzg4ICA4EMgQ5hcwVhYoGiYWEAYWWCCgthYw9hZ6JhRZCDAAsAgwEKAIMCDwCD"
-               "Aw8AgwQOAIMFDgCDBg0AgwcNAIMIDACDCQwAgwoLAYMKDQCDCwwAgwwPAIMNDgCDDg8AYVqQ"
-               "AQEBAQEBAQEBAQYGBgYGBmF2gwEAAA==")
-    structure.set_graph("masm_cbor_graph", graph_1 + ";" + graph_3)
-    structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2), (1, 3), (1, 4), (1, 5)")
-    compound_engine.run(single=True)
-    assert flasks.count(dumps({})) == 2
-    assert flasks.count(dumps({"compounds": {"$size": 2}})) == 1
-    assert flasks.count(dumps({"compounds": {"$size": 0}})) == 1
-
-    # Cleaning
-    manager.wipe()
-
-
-def test_unique_structures_loading():
-    """
-    Test if the loading of compound already in the database works.
-    This test will set up two compounds with structures, decision lists, and graphs. The
-    structures are then cached as unique structures for each compound. We then check if
-    a third structures is correctly identified as a duplicate.
-    """
-    manager = db_setup.get_clean_db("chemoton_test_flask_to_compound_mapping")
-
-    # Get collections
-    structures = manager.get_collection("structures")
-
-    _, s_id1 = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_OPTIMIZED)
-    _, s_id2 = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_OPTIMIZED)
-    structure_1 = db.Structure(s_id1, structures)
-    structure_2 = db.Structure(s_id2, structures)
-    graph_1 = "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWFzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
-    graph_2 = ("pGFhgqRhYQBhYwJhcqNhbIKBAYEDYmxygoEAgQFhc4KBAYEDYXMBpGFhAGFjA2"
-               "Fyo2FsgoEAgQJibHKCgQCBAWFzgoEAgQJhcwFhYw9hZ6JhRYODAAMAgwECAIMC"
-               "AwBhWoQBAQgIYXaDAQAA")
-    structure_1.set_graph("masm_cbor_graph", graph_1)
-    structure_1.set_graph("masm_decision_list", "(10,30,40,1)")
-    structure_1.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-    structure_2.set_graph("masm_cbor_graph", graph_2)
-    structure_2.set_graph("masm_decision_list", "(10,30,40,1):(1, 3, 5, 8)")
-    structure_2.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-
-    # Add structure data
-    model = db.Model("FAKE", "FAKE", "F-AKE")
-    rr = resources_root_path()
-    duplicate_1 = db.Structure()
-    duplicate_1.link(structures)
-    duplicate_1.create(os.path.join(rr, "water.xyz"), 0, 1)
-    duplicate_1.set_label(db.Label.MINIMUM_OPTIMIZED)
-    duplicate_1.set_graph("masm_cbor_graph", graph_1)
-    duplicate_1.set_graph("masm_decision_list", "(10,30,40,1)")
-    duplicate_1.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-
-    duplicate_2 = db.Structure()
-    duplicate_2.link(structures)
-    duplicate_2.create(os.path.join(rr, "water.xyz"), 0, 1)
-    duplicate_2.set_label(db.Label.MINIMUM_OPTIMIZED)
-    duplicate_2.set_graph("masm_cbor_graph", graph_2)
-    duplicate_2.set_graph("masm_decision_list", "(29, 39, 49, 1):(2, 4, 7, 8)")
-    duplicate_2.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
-
-    # Setup gear
-    compound_gear = BasicAggregateHousekeeping()
-    compound_gear.options.model = model
-    compound_engine = Engine(manager.get_credentials(), fork=False)
-    compound_engine.set_gear(compound_gear)
+        # Run a second time
+        compound_engine.run(single=True)
+        assert self._flasks.count(dumps({})) == 1
+        assert self._flasks.count(dumps({"compounds": {"$size": 0}})) == 1
 
-    # Run a single loop
-    compound_engine.run(single=True)
+        structure = db.Structure()
+        structure.link(self._structures)
+        structure.create(os.path.join(rr, "water.xyz"), 0, 1)
+        structure.set_label(db.Label.COMPLEX_OPTIMIZED)
+        graph_3 = ("pWFhhqRhYQBhYwphcqRhbIOBAYELgQ1jbG5rgaJhcIIBAmNzZXGGCgsMDw4NYmxyg4EAgQGB"
+                   "AmFzg4EBgQuBDWFzAqRhYQBhYwthcqRhbIOBAIEKgQxjbG5rgaJhcIIBAmNzZXGGCwoNDg8M"
+                   "Ymxyg4EAgQGBAmFzg4EAgQqBDGFzAqRhYQBhYwxhcqRhbISBCIEJgQuBD2NsbmuBomFwggID"
+                   "Y3NlcYYMCwoNDg9ibHKDggABgQKBA2Fzg4IICYELgQ9hcwWkYWEAYWMNYXKkYWyEgQaBB4EK"
+                   "gQ5jbG5rgaJhcIICA2NzZXGGDQoLDA8OYmxyg4IAAYECgQNhc4OCBgeBCoEOYXMFpGFhAGFj"
+                   "DmFypGFshIEEgQWBDYEPY2xua4GiYXCCAgNjc2Vxhg4NCgsMD2JscoOCAAGBAoEDYXODggQF"
+                   "gQ2BD2FzBaRhYQBhYw9hcqRhbISBAoEDgQyBDmNsbmuBomFwggIDY3NlcYYPDAsKDQ5ibHKD"
+                   "ggABgQKBA2Fzg4ICA4EMgQ5hcwVhYoGiYWEAYWWCCgthYw9hZ6JhRZCDAAsAgwEKAIMCDwCD"
+                   "Aw8AgwQOAIMFDgCDBg0AgwcNAIMIDACDCQwAgwoLAYMKDQCDCwwAgwwPAIMNDgCDDg8AYVqQ"
+                   "AQEBAQEBAQEBAQYGBgYGBmF2gwEAAA==")
+        structure.set_graph("masm_cbor_graph", graph_1 + ";" + graph_3)
+        structure.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2), (1, 3), (1, 4), (1, 5)")
+        compound_engine.run(single=True)
+        assert self._flasks.count(dumps({})) == 2
+        assert self._flasks.count(dumps({"compounds": {"$size": 0}})) == 2
+
+    def test_unique_structures_loading(self):
+        """
+        Test if the loading of compound already in the database works.
+        This test will set up two compounds with structures, decision lists, and graphs. The
+        structures are then cached as unique structures for each compound. We then check if
+        a third structures is correctly identified as a duplicate.
+        """
+        manager = db_setup.get_clean_db("chemoton_test_unique_structures_loading")
+        self.custom_setup(manager)
+
+        _, s_id1 = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.MINIMUM_OPTIMIZED)
+        _, s_id2 = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.MINIMUM_OPTIMIZED)
+        structure_1 = db.Structure(s_id1, self._structures)
+        structure_2 = db.Structure(s_id2, self._structures)
+        graph_1 = "pGFhgaRhYQBhYwJhcqNhbIKBAIEBYmxygYIAAWFzgYIAAWFzAWFjD2FnomFFgoMAAgCDAQIAYVqDAQEIYXaDAQAA"
+        graph_2 = ("pGFhgqRhYQBhYwJhcqNhbIKBAYEDYmxygoEAgQFhc4KBAYEDYXMBpGFhAGFjA2"
+                   "Fyo2FsgoEAgQJibHKCgQCBAWFzgoEAgQJhcwFhYw9hZ6JhRYODAAMAgwECAIMC"
+                   "AwBhWoQBAQgIYXaDAQAA")
+        structure_1.set_graph("masm_cbor_graph", graph_1)
+        structure_1.set_graph("masm_decision_list", "(10,30,40,1)")
+        structure_1.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+        structure_2.set_graph("masm_cbor_graph", graph_2)
+        structure_2.set_graph("masm_decision_list", "(10,30,40,1):(1, 3, 5, 8)")
+        structure_2.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+
+        # Add structure data
+        model = db.Model("FAKE", "FAKE", "F-AKE")
+        rr = resources_root_path()
+        duplicate_1 = db.Structure()
+        duplicate_1.link(self._structures)
+        duplicate_1.create(os.path.join(rr, "water.xyz"), 0, 1)
+        duplicate_1.set_label(db.Label.MINIMUM_OPTIMIZED)
+        duplicate_1.set_graph("masm_cbor_graph", graph_1)
+        duplicate_1.set_graph("masm_decision_list", "(10,30,40,1)")
+        duplicate_1.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+        duplicate_1.set_model(model)
+
+        duplicate_2 = db.Structure()
+        duplicate_2.link(self._structures)
+        duplicate_2.create(os.path.join(rr, "water.xyz"), 0, 1)
+        duplicate_2.set_label(db.Label.MINIMUM_OPTIMIZED)
+        duplicate_2.set_graph("masm_cbor_graph", graph_2)
+        duplicate_2.set_graph("masm_decision_list", "(29, 39, 49, 1):(2, 4, 7, 8)")
+        duplicate_2.set_graph("masm_idx_map", "(0, 0), (0, 1), (0, 2)")
+        duplicate_2.set_model(model)
+
+        # Setup gear
+        compound_gear = BasicAggregateHousekeeping()
+        compound_gear.options.model = model
+        compound_engine = Engine(manager.get_credentials(), fork=False)
+        compound_engine.set_gear(compound_gear)
+
+        # Run a single loop
+        compound_engine.run(single=True)
 
-    assert duplicate_1.get_label() == db.Label.DUPLICATE
-    assert duplicate_2.get_label() == db.Label.DUPLICATE
+        assert duplicate_1.get_label() == db.Label.DUPLICATE
+        assert duplicate_2.get_label() == db.Label.DUPLICATE
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/gears/test_reaction.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/gears/test_reaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     def test_elementary_step_deduplication(self):
         manager = db_setup.get_clean_db(inspect.currentframe().f_code.co_name)
         self.custom_setup(manager)
         manager = self._manager
         steps = self._elementary_steps
 
         # set up 2 compounds
-        c1_id, s1_id = db_setup.insert_single_empty_structure_compound(manager, db.Label.USER_OPTIMIZED)
-        c2_id, s2_id = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_OPTIMIZED)
+        c1_id, s1_id = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.USER_OPTIMIZED)
+        c2_id, s2_id = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.USER_OPTIMIZED)
 
         # set up step between compounds
         step_one = self._add_new_regular_step([s1_id, s2_id], (70.0, 71.0))
 
         reaction_gear = BasicReactionHousekeeping()
         reaction_engine = Engine(manager.get_credentials(), fork=False)
         reaction_engine.set_gear(reaction_gear)
@@ -67,61 +67,66 @@
         step_two.create([s1_id], [s2_id])
         step_two.set_transition_state(step_one.get_transition_state())
 
         reaction_engine.run(single=True)
         n_reactions = self._reactions.count(dumps({}))
         assert n_reactions == 1
         reaction = db.Reaction(reaction_from_one[0], self._reactions)
-        assert len(reaction.get_elementary_steps()) == 1
+        assert len(reaction.get_elementary_steps()) == 2
         assert not step_two.explore() and not step_two.analyze()
 
         # insert step with same structures and TS for the same reaction with different energy
         step_three = self._add_new_regular_step([s1_id, s2_id], (68.0, 69.0))
 
         # deactivate energy criterion
         reaction_gear.options.use_energy_deduplication = False
         reaction_engine.set_gear(reaction_gear)
         reaction_engine.run(single=True)
 
         # duplicated without energy criterion
         n_reactions = self._reactions.count(dumps({}))
         assert n_reactions == 1
         reaction = db.Reaction(compound_one.get_reactions()[0], self._reactions)
-        assert len(reaction.get_elementary_steps()) == 1
+        assert len(reaction.get_elementary_steps()) == 3
         assert not step_three.explore() and not step_three.analyze()
 
         # no deduplication with energy criterion
         step_three.enable_exploration()
         step_three.enable_analysis()
 
         reaction_gear.options.use_energy_deduplication = True
         reaction_engine.set_gear(reaction_gear)
         reaction_engine.run(single=True)
         n_reactions = self._reactions.count(dumps({}))
         assert n_reactions == 1
         reaction = db.Reaction(compound_one.get_reactions()[0], self._reactions)
-        assert len(reaction.get_elementary_steps()) == 2
+        assert len(reaction.get_elementary_steps()) == 3
         assert step_three.explore() and step_three.analyze()
 
     def test_barrierless_disable(self):
         manager = db_setup.get_clean_db(inspect.currentframe().f_code.co_name)
         self.custom_setup(manager)
         manager = self._manager
 
         # set up 4 compounds
-        _, s1_id = db_setup.insert_single_empty_structure_compound(manager, db.Label.USER_OPTIMIZED)
-        _, s2_id = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_OPTIMIZED)
-        _, s3_id = db_setup.insert_single_empty_structure_compound(manager, db.Label.USER_OPTIMIZED)
-        _, s4_id = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_OPTIMIZED)
+        _, s1_id = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.USER_OPTIMIZED)
+        _, s2_id = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.MINIMUM_OPTIMIZED)
+        _, s3_id = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.USER_OPTIMIZED)
+        _, s4_id = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.MINIMUM_OPTIMIZED)
 
         # set up one step each between two pair of structures
         step0_regular_0 = self._add_new_regular_step([s1_id, s2_id])
         step1_free_0 = self._add_new_barrierless_step([s3_id, s4_id])
 
         reaction_gear = BasicReactionHousekeeping()
+        # disable deduplication
+        reaction_gear.options.use_structure_deduplication = False
+        reaction_gear.options.use_energy_deduplication = False
+        reaction_gear.options.use_rmsd_deduplication = False
+
         reaction_engine = Engine(manager.get_credentials(), fork=False)
         reaction_engine.set_gear(reaction_gear)
         reaction_engine.run(single=True)
 
         assert self._reactions.count(dumps({})) == 2
         assert step0_regular_0.explore() and step0_regular_0.analyze()
         assert step1_free_0.explore() and step1_free_0.analyze()
@@ -183,30 +188,35 @@
         import numpy as np
         manager = db_setup.get_clean_db(inspect.currentframe().f_code.co_name)
         self.custom_setup(manager)
         manager = self._manager
         structures = manager.get_collection("structures")
 
         # set up 2 compounds
-        _, s1_id = db_setup.insert_single_empty_structure_compound(manager, db.Label.USER_OPTIMIZED)
-        _, s2_id = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_OPTIMIZED)
+        _, s1_id = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.USER_OPTIMIZED)
+        _, s2_id = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.MINIMUM_OPTIMIZED)
 
         # set up step between compounds
         step_one = self._add_new_regular_step([s1_id, s2_id], (70.0, 71.0))
         step_two = self._add_new_regular_step([s2_id, s1_id], (70.0, 71.0))
         structure_two = db.Structure(s1_id, structures)
 
         knots = np.asarray([0.0, 0.7, 1.0])
         data = np.asarray([[0.1, 0.0, 0.0, 0.0], [0.2, 0.0, 0.1, 0.0], [0.1, 0.0, 0.3, 0.0]])
         ts_position = 0.7
 
         spline = utils.bsplines.TrajectorySpline(structure_two.get_atoms().elements, knots, data, ts_position)
         step_two.set_spline(spline)
 
         reaction_gear = BasicReactionHousekeeping()
+        # disable deduplication
+        reaction_gear.options.use_structure_deduplication = False
+        reaction_gear.options.use_energy_deduplication = False
+        reaction_gear.options.use_rmsd_deduplication = False
+
         reaction_engine = Engine(manager.get_credentials(), fork=False)
         reaction_engine.set_gear(reaction_gear)
         reaction_engine.run(single=True)
 
         step_one_reactants = step_one.get_reactants(db.Side.BOTH)
         step_two_reactants = step_two.get_reactants(db.Side.BOTH)
 
@@ -232,19 +242,19 @@
     def test_elementary_step_structure_deduplication(self):
         manager = db_setup.get_clean_db(inspect.currentframe().f_code.co_name)
         self.custom_setup(manager)
         manager = self._manager
         structures = manager.get_collection("structures")
 
         # set up 2 compounds
-        _, s1_id = db_setup.insert_single_empty_structure_compound(manager, db.Label.USER_OPTIMIZED)
-        a2_id, s2_id = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_OPTIMIZED)
-        _, duplicate_id = db_setup.insert_single_empty_structure_compound(manager, db.Label.DUPLICATE)
+        _, s1_id = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.USER_OPTIMIZED)
+        a2_id, s2_id = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.MINIMUM_OPTIMIZED)
+        _, duplicate_id = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.DUPLICATE)
         duplicate = db.Structure(duplicate_id, structures)
-        duplicate.set_as_duplicate_of(s2_id)
+        duplicate.set_original(s2_id)
         duplicate.set_aggregate(a2_id)
         step = self._add_new_regular_step([s1_id, duplicate_id], (70.0, 71.0))
 
         reaction_gear = BasicReactionHousekeeping()
         reaction_engine = Engine(manager.get_credentials(), fork=False)
         reaction_engine.set_gear(reaction_gear)
         reaction_engine.run(single=True)
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/gears/test_refinement.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/gears/test_refinement.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # Local application tests imports
 from .. import test_database_setup as db_setup
 
 # Local application imports
 from ...utilities.queries import identical_reaction, model_query
 from ...engine import Engine
 from ...gears.refinement import NetworkRefinement
+from ...utilities.compound_and_flask_creation import get_compound_or_flask
 
 
 def create_new_calculations(elementary_steps, calculations, pre_model, structures):
     n_new_calcs = 0
     for step in elementary_steps.iterate_all_elementary_steps():
         n_new_calcs += 1
         step.link(elementary_steps)
@@ -81,14 +82,15 @@
                 structure.add_calculation(calculation.job.order, calculation.id())
                 structure.set_graph("masm_cbor_graph", "asdfghjkl")
                 structure.set_graph("masm_decision_list", "")
                 s_id_list.append(s_id)
     return len(s_id_list)
 
 
+@pytest.mark.filterwarnings("ignore:.+is not implemented by default:UserWarning")
 def test_incorrect_refinement_input():
     manager = db_setup.get_clean_db("chemoton_test_incorrect_refinement_input")
     refinement_gear = NetworkRefinement()
     refinement_gear.options.pre_refine_model = db.Model("something", "wrong", "because", "identical")
     refinement_gear.options.post_refine_model = db.Model("something", "wrong", "because", "identical")
     refinement_engine = Engine(manager.get_credentials(), fork=False)
     refinement_engine.set_gear(refinement_gear)
@@ -132,19 +134,14 @@
         n_inserts,
     )
     compounds = manager.get_collection("compounds")
     calculations = manager.get_collection("calculations")
     structures = manager.get_collection("structures")
     n_structures_before = structures.count(dumps({}))
 
-    # enable all compounds
-    for c in compounds.iterate_all_compounds():
-        c.link(compounds)
-        c.enable_exploration()
-
     # does nothing per default
     refinement_gear = NetworkRefinement()
     refinement_gear.options.pre_refine_model = db.Model("FAKE", "FAKE", "F-AKE")
     refinement_engine = Engine(manager.get_credentials(), fork=False)
     refinement_engine.set_gear(refinement_gear)
     for _ in range(5):
         refinement_engine.run(single=True)
@@ -152,14 +149,15 @@
     assert compounds.count(dumps({})) == n_compounds
     assert structures.count(dumps({})) == n_structures_before
     assert calculations.count(dumps({})) == 0  # random db does not have calculations
     # Cleaning
     manager.wipe()
 
 
+@pytest.mark.filterwarnings("ignore:.+is not implemented by default:UserWarning")
 def test_refinement_with_wrong_model():
     n_compounds = 10
     n_flasks = 0
     n_reactions = 5
     max_r_per_c = 10
     max_n_products_per_r = 3
     max_n_educts_per_r = 2
@@ -182,23 +180,17 @@
     )
     compounds = manager.get_collection("compounds")
     calculations = manager.get_collection("calculations")
     structures = manager.get_collection("structures")
     elementary_steps = manager.get_collection("elementary_steps")
     n_structures_before = structures.count(dumps({}))
 
-    # enable all compounds
-    for c in compounds.iterate_all_compounds():
-        c.link(compounds)
-        c.enable_exploration()
-
-    added_calculations = create_new_calculations(
-        elementary_steps, calculations, db.Model(
-            "FAKE", "FAKE", "F-AKE"), structures)
-    pre_model = db.Model("NON_EXISTENT", "", "")
+    added_calculations = create_new_calculations(elementary_steps, calculations, db.Model("FAKE", "FAKE", "F-AKE"),
+                                                 structures)
+    pre_model = db.Model("NON_EXISTENT", "FAKE", "F-AKE")
     refine_model = db.Model("a", "b", "c", "d")
     refine_model.solvation = "something"
     refinement_gear = NetworkRefinement()
     refinement_gear.options.pre_refine_model = pre_model
     refinement_gear.options.post_refine_model = refine_model
     refinement_gear.options.refinements = {
         "refine_single_points": True,
@@ -246,18 +238,14 @@
     )
     compounds = manager.get_collection("compounds")
     calculations = manager.get_collection("calculations")
     structures = manager.get_collection("structures")
     elementary_steps = manager.get_collection("elementary_steps")
     n_structures_before = structures.count(dumps({}))
 
-    # enable all compounds
-    for c in compounds.iterate_all_compounds():
-        c.link(compounds)
-        c.enable_exploration()
     structures_to_refine = []
     for e in elementary_steps.iterate_all_elementary_steps():
         e.link(elementary_steps)
         reactants_products = e.get_reactants(db.Side.BOTH)
         transition_state_id = e.get_transition_state()
         structure_ids = reactants_products[0] + [transition_state_id] + reactants_products[1]
         for s_id in structure_ids:
@@ -325,19 +313,14 @@
     )
     compounds = manager.get_collection("compounds")
     calculations = manager.get_collection("calculations")
     structures = manager.get_collection("structures")
     elementary_steps = manager.get_collection("elementary_steps")
     n_structures_before = structures.count(dumps({}))
 
-    # enable all compounds
-    for c in compounds.iterate_all_compounds():
-        c.link(compounds)
-        c.enable_exploration()
-
     pre_model = db.Model("FAKE", "FAKE", "F-AKE")
     added_calculations = create_new_calculations(elementary_steps, calculations, pre_model, structures)
     refine_model = db.Model("a", "b", "c", "d")
     refine_model.solvation = "something"
     refinement_gear = NetworkRefinement()
     refinement_gear.options.pre_refine_model = pre_model
     refinement_gear.options.post_refine_model = refine_model
@@ -360,14 +343,15 @@
     # random db does not have calculations, now calculation for every structure
     assert calculations.count(dumps({})) == added_calculations
     assert calculations.count(dumps({"$and": model_query(refine_model)})) == 0
     # Cleaning
     manager.wipe()
 
 
+@pytest.mark.filterwarnings("ignore:.+is not implemented by default:UserWarning")
 def test_opt_refinement():
     n_compounds = 10
     n_flasks = 0
     n_reactions = 5
     max_r_per_c = 10
     max_n_products_per_r = 3
     max_n_educts_per_r = 2
@@ -390,19 +374,14 @@
     )
     compounds = manager.get_collection("compounds")
     calculations = manager.get_collection("calculations")
     structures = manager.get_collection("structures")
     elementary_steps = manager.get_collection("elementary_steps")
     n_structures_before = structures.count(dumps({}))
 
-    # enable all compounds
-    for c in compounds.iterate_all_compounds():
-        c.link(compounds)
-        c.enable_exploration()
-
     structures_to_refine = []
     for e in elementary_steps.iterate_all_elementary_steps():
         e.link(elementary_steps)
         reactants_products = e.get_reactants(db.Side.BOTH)
         transition_state_id = e.get_transition_state()
         structure_ids = reactants_products[0] + [transition_state_id] + reactants_products[1]
         for s_id in structure_ids:
@@ -452,14 +431,15 @@
 
     assert calc.get_job().order == target_job.order
     assert calc.get_settings() == target_settings
     # Cleaning
     manager.wipe()
 
 
+@pytest.mark.filterwarnings("ignore:.+is not implemented by default:UserWarning")
 def test_sp_and_opt_refinement():
     n_compounds = 10
     n_flasks = 0
     n_reactions = 5
     max_r_per_c = 10
     max_n_products_per_r = 3
     max_n_educts_per_r = 2
@@ -482,19 +462,14 @@
     )
     compounds = manager.get_collection("compounds")
     calculations = manager.get_collection("calculations")
     structures = manager.get_collection("structures")
     elementary_steps = manager.get_collection("elementary_steps")
     n_structures_before = structures.count(dumps({}))
 
-    # enable all compounds
-    for c in compounds.iterate_all_compounds():
-        c.link(compounds)
-        c.enable_exploration()
-
     structures_to_refine = []
     for e in elementary_steps.iterate_all_elementary_steps():
         e.link(elementary_steps)
         reactants_products = e.get_reactants(db.Side.BOTH)
         transition_state_id = e.get_transition_state()
         structure_ids = reactants_products[0] + [transition_state_id] + reactants_products[1]
         for s_id in structure_ids:
@@ -534,85 +509,15 @@
         refinement_gear.options.opt_job.order,
         refinement_gear.options.tsopt_job.order,
     ]
     # Cleaning
     manager.wipe()
 
 
-def test_double_ended_refinement():
-    n_compounds = 10
-    n_flasks = 0
-    n_reactions = 5
-    max_r_per_c = 10
-    max_n_products_per_r = 3
-    max_n_educts_per_r = 2
-    max_s_per_c = 1
-    max_steps_per_r = 1  # must be kept to know the number of expected calculations
-    barrier_limits = (0.1, 100.0)
-    n_inserts = 3
-    manager = db_setup.get_random_db(
-        n_compounds,
-        n_flasks,
-        n_reactions,
-        max_r_per_c,
-        "chemoton_test_double_ended_refinement",
-        max_n_products_per_r,
-        max_n_educts_per_r,
-        max_s_per_c,
-        max_steps_per_r,
-        barrier_limits,
-        n_inserts,
-    )
-    compounds = manager.get_collection("compounds")
-    calculations = manager.get_collection("calculations")
-    structures = manager.get_collection("structures")
-    elementary_steps = manager.get_collection("elementary_steps")
-    n_structures_before = structures.count(dumps({}))
-
-    # enable all compounds
-    for c in compounds.iterate_all_compounds():
-        c.link(compounds)
-        c.enable_exploration()
-
-    # create calculation for each step
-    refinement_gear = NetworkRefinement()
-    pre_model = db.Model("FAKE", "FAKE", "F-AKE")
-    refine_model = db.Model("a", "b", "c", "d")
-    refine_model.solvation = "something"
-    added_calculations = create_new_calculations(elementary_steps, calculations, pre_model, structures)
-    n_opt_calculations = create_fake_optimization_calculations(elementary_steps, refine_model, db.Side.BOTH,
-                                                               refinement_gear.options.opt_job,
-                                                               refinement_gear.options.opt_job_settings,
-                                                               calculations, structures)
-    refinement_gear.options.pre_refine_model = pre_model
-    refinement_gear.options.post_refine_model = refine_model
-    refinement_gear.options.refinements = {
-        "refine_single_points": False,
-        "refine_optimizations": False,
-        "double_ended_refinement": True,
-        "double_ended_new_connections": False,
-        "refine_single_ended_search": False,
-        "refine_structures_and_irc": False,
-    }
-    refinement_gear.options.max_barrier = 2001.0
-    refinement_engine = Engine(manager.get_credentials(), fork=False)
-    refinement_engine.set_gear(refinement_gear)
-    for _ in range(5):
-        refinement_engine.run(single=True)
-
-    assert compounds.count(dumps({})) == n_compounds
-    assert structures.count(dumps({})) == n_structures_before
-    # random db does not have calculations, made calculation for every step, now should have double the calculations
-    assert max_steps_per_r == 1
-    assert calculations.count(dumps({"$and": model_query(refine_model)})) == n_reactions + n_opt_calculations
-    assert calculations.count(dumps({})) == n_reactions + added_calculations + n_opt_calculations
-    # Cleaning
-    manager.wipe()
-
-
+@pytest.mark.filterwarnings("ignore:.+is not implemented by default:UserWarning")
 def test_double_ended_new():
     n_compounds = 10
     n_flasks = 0
     n_reactions = 5
     max_r_per_c = 10
     max_n_products_per_r = 3
     max_n_educts_per_r = 2
@@ -635,19 +540,14 @@
     )
     compounds = manager.get_collection("compounds")
     calculations = manager.get_collection("calculations")
     structures = manager.get_collection("structures")
     reactions = manager.get_collection("reactions")
     n_structures_before = structures.count(dumps({}))
 
-    # enable all compounds
-    for c in compounds.iterate_all_compounds():
-        c.link(compounds)
-        c.enable_exploration()
-
     pre_model = db.Model("FAKE", "FAKE", "F-AKE")
     refine_model = db.Model("a", "b", "c", "d")
     refine_model.solvation = "something"
     refinement_gear = NetworkRefinement()
     refinement_gear.options.pre_refine_model = pre_model
     refinement_gear.options.post_refine_model = refine_model
     refinement_gear.options.refinements = {
@@ -714,19 +614,14 @@
     )
     compounds = manager.get_collection("compounds")
     calculations = manager.get_collection("calculations")
     structures = manager.get_collection("structures")
     elementary_steps = manager.get_collection("elementary_steps")
     n_structures_before = structures.count(dumps({}))
 
-    # enable all compounds
-    for c in compounds.iterate_all_compounds():
-        c.link(compounds)
-        c.enable_exploration()
-
     # create calculation for each step
     pre_model = db.Model("FAKE", "FAKE", "F-AKE")
     added_calculations = create_new_calculations(elementary_steps, calculations, pre_model, structures)
     refine_model = db.Model("a", "b", "c", "d")
     refine_model.solvation = "something"
     refinement_gear = NetworkRefinement()
     n_opt_calculations = create_fake_optimization_calculations(elementary_steps, refine_model, db.Side.LHS,
@@ -792,19 +687,14 @@
         n_inserts,
     )
     compounds = manager.get_collection("compounds")
     calculations = manager.get_collection("calculations")
     structures = manager.get_collection("structures")
     n_structures_before = structures.count(dumps({}))
 
-    # enable all compounds
-    for c in compounds.iterate_all_compounds():
-        c.link(compounds)
-        c.enable_exploration()
-
     # create calculation for each step
     pre_model = db.Model("FAKE", "FAKE", "F-AKE")
     elementary_steps = manager.get_collection("elementary_steps")
     added_calculations = create_new_calculations(elementary_steps, calculations, pre_model, structures)
 
     refine_model = db.Model("a", "b", "c", "d")
     refine_model.solvation = "something"
@@ -933,14 +823,89 @@
         calc = calculations.random_select_calculations(1)[0]
         calc.link(calculations)
     assert calc.get_job().order == refinement_gear.options.single_ended_step_refinement_job.order
     # Cleaning
     manager.wipe()
 
 
+def test_refine_manual_reaction_selection():
+    n_compounds = 10
+    n_flasks = 0
+    n_reactions = 5
+    max_r_per_c = 10
+    max_n_products_per_r = 3
+    max_n_educts_per_r = 2
+    max_s_per_c = 1
+    max_steps_per_r = 3
+    barrier_limits = (0.1, 200)
+    n_inserts = 3
+    manager = db_setup.get_random_db(
+        n_compounds,
+        n_flasks,
+        n_reactions,
+        max_r_per_c,
+        "chemoton_test_refine_manual_reaction_selection",
+        max_n_products_per_r,
+        max_n_educts_per_r,
+        max_s_per_c,
+        max_steps_per_r,
+        barrier_limits,
+        n_inserts,
+    )
+    compounds = manager.get_collection("compounds")
+    flasks = manager.get_collection("flasks")
+    calculations = manager.get_collection("calculations")
+    structures = manager.get_collection("structures")
+    reactions = manager.get_collection("reactions")
+
+    # create calculation for each step
+    pre_model = db.Model("FAKE", "FAKE", "F-AKE")
+    elementary_steps = manager.get_collection("elementary_steps")
+    added_calculations = create_new_calculations(elementary_steps, calculations, pre_model, structures)
+
+    refine_model = db.Model("a", "b", "c", "d")
+    refine_model.solvation = "something"
+    refinement_gear = NetworkRefinement()
+    n_opt_calculations = create_fake_optimization_calculations(elementary_steps, refine_model, db.Side.LHS,
+                                                               refinement_gear.options.opt_job,
+                                                               refinement_gear.options.opt_job_settings,
+                                                               calculations, structures)
+    refinement_gear.options.pre_refine_model = pre_model
+    refinement_gear.options.post_refine_model = refine_model
+    refinement_gear.options.refinements = {
+        "refine_single_points": False,
+        "refine_optimizations": False,
+        "double_ended_refinement": False,
+        "double_ended_new_connections": False,
+        "refine_single_ended_search": False,
+        "refine_structures_and_irc": True,
+    }
+    random_reaction = reactions.get_one_reaction(dumps({}))
+    refinement_gear.options.max_barrier = 2001
+    refinement_gear.options.manual_reaction_selection = True
+    refinement_gear.options.reaction_ids_to_refine = [random_reaction.id()]
+
+    refinement_gear.options.transition_state_energy_window = 0.0
+    refinement_gear.options.jobs_to_wait_for = ["some_react_job"]
+    refinement_engine = Engine(manager.get_credentials(), fork=False)
+    refinement_engine.set_gear(refinement_gear)
+
+    refinement_engine.run(single=True)
+    assert calculations.count(dumps({})) == added_calculations + n_opt_calculations + 1
+    random_reaction.link(reactions)
+    lhs = random_reaction.get_reactants(db.Side.LHS)[0]
+    types = random_reaction.get_reactant_types(db.Side.LHS)[0]
+    aggregate = get_compound_or_flask(lhs[0], types[0], compounds, flasks)
+    structure = db.Structure(aggregate.get_centroid(), structures)
+    assert structure.has_calculation("scine_step_refinement")
+
+    # Cleaning
+    manager.wipe()
+
+
 def test_single_ended_refinement_set_up_optimizations():
     n_compounds = 10
     n_flasks = 0
     n_reactions = 5
     max_r_per_c = 10
     max_n_products_per_r = 3
     max_n_educts_per_r = 2
@@ -975,14 +940,15 @@
     # create calculation for each step
     pre_model = db.Model("FAKE", "FAKE", "F-AKE")
     added_calculations = create_new_calculations(elementary_steps, calculations, pre_model, structures)
     s_id_set = set()
     for calculation in calculations.iterate_all_calculations():
         calculation.link(calculations)
         s_id_set = s_id_set.union([s_id.string() for s_id in calculation.get_structures()])
+        calculation.set_status(db.Status.PENDING)
     n_unique_lhs = len(s_id_set)
 
     refine_model = db.Model("a", "b", "c", "d")
     refine_model.solvation = "something"
     refinement_gear = NetworkRefinement()
     refinement_gear.options.pre_refine_model = pre_model
     refinement_gear.options.post_refine_model = refine_model
@@ -999,11 +965,111 @@
     refinement_engine.set_gear(refinement_gear)
     for _ in range(5):
         refinement_engine.run(single=True)
 
     assert compounds.count(dumps({})) == n_compounds
     assert structures.count(dumps({})) == n_structures_before
     assert max_steps_per_r == 1
+    assert calculations.count(dumps({})) == added_calculations
+
+    for calculation in calculations.iterate_all_calculations():
+        calculation.link(calculations)
+        calculation.set_status(db.Status.COMPLETE)
+
+    for _ in range(5):
+        refinement_engine.run(single=True)
+
+    assert compounds.count(dumps({})) == n_compounds
+    assert structures.count(dumps({})) == n_structures_before
+    assert max_steps_per_r == 1
+    assert n_unique_lhs > 0
     assert calculations.count(dumps({})) == added_calculations + n_unique_lhs
     assert calculations.count(dumps({"$and": model_query(refine_model)})) == n_unique_lhs
     # Cleaning
     manager.wipe()
+
+
+def test_double_ended_refinement():
+    n_compounds = 10
+    n_flasks = 0
+    n_reactions = 5
+    max_r_per_c = 10
+    max_n_products_per_r = 3
+    max_n_educts_per_r = 2
+    max_s_per_c = 1
+    max_steps_per_r = 1  # must be kept to know the number of expected calculations
+    barrier_limits = (0.1, 100.0)
+    n_inserts = 3
+    manager = db_setup.get_random_db(
+        n_compounds,
+        n_flasks,
+        n_reactions,
+        max_r_per_c,
+        "chemoton_test_double_ended_refinement",
+        max_n_products_per_r,
+        max_n_educts_per_r,
+        max_s_per_c,
+        max_steps_per_r,
+        barrier_limits,
+        n_inserts,
+    )
+    compounds = manager.get_collection("compounds")
+    calculations = manager.get_collection("calculations")
+    structures = manager.get_collection("structures")
+    elementary_steps = manager.get_collection("elementary_steps")
+    n_structures_before = structures.count(dumps({}))
+
+    # create calculation for each step
+    pre_model = db.Model("FAKE", "FAKE", "F-AKE")
+    added_calculations = create_new_calculations(elementary_steps, calculations, pre_model, structures)
+    for calculation in calculations.iterate_all_calculations():
+        calculation.link(calculations)
+        calculation.set_status(db.Status.PENDING)
+
+    for step in elementary_steps.iterate_all_elementary_steps():
+        step.link(elementary_steps)
+        if step.get_type() == db.ElementaryStepType.REGULAR:
+            reactant_id = step.get_reactants(db.Side.LHS)[0][0]
+            s = db.Structure(reactant_id, structures)
+            atoms = s.get_atoms()
+            rpi = utils.bsplines.ReactionProfileInterpolation()
+            rpi.append_structure(atoms, 1.0)
+            rpi.append_structure(atoms, 1.0)
+            step.set_spline(rpi.spline(2, 1))
+
+    refine_model = db.Model("a", "b", "c", "d")
+    refine_model.solvation = "something"
+    refinement_gear = NetworkRefinement()
+    refinement_gear.options.pre_refine_model = pre_model
+    refinement_gear.options.post_refine_model = refine_model
+    refinement_gear.options.refinements = {
+        "refine_single_points": False,
+        "refine_optimizations": False,
+        "double_ended_refinement": True,
+        "double_ended_new_connections": False,
+        "refine_single_ended_search": False,
+        "refine_structures_and_irc": False,
+    }
+    refinement_gear.options.max_barrier = 2001.0
+    refinement_engine = Engine(manager.get_credentials(), fork=False)
+    refinement_engine.set_gear(refinement_gear)
+    for _ in range(5):
+        refinement_engine.run(single=True)
+
+    assert compounds.count(dumps({})) == n_compounds
+    assert max_steps_per_r == 1
+    assert structures.count(dumps({})) == n_structures_before
+    assert calculations.count(dumps({})) == added_calculations
+
+    for calculation in calculations.iterate_all_calculations():
+        calculation.link(calculations)
+        calculation.set_status(db.Status.COMPLETE)
+
+    for _ in range(5):
+        refinement_engine.run(single=True)
+
+    assert structures.count(dumps({})) == n_structures_before + n_reactions * 2
+    assert compounds.count(dumps({})) == n_compounds
+    assert calculations.count(dumps({})) == added_calculations + n_reactions
+    assert calculations.count(dumps({"$and": model_query(refine_model)})) == n_reactions
+    # Cleaning
+    manager.wipe()
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/gears/test_scheduler.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/gears/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/utilities/reactive_complexes/test_inter_reactive_complexes.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/utilities/reactive_complexes/test_inter_reactive_complexes.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,23 +136,23 @@
         # # # Move sphere around oxygen atom
         possible_directions = deepcopy(initial_points) * utils.ElementInfo.vdw_radius(elements[index])
         possible_directions += coords[index]
 
         reactive_complex = InterReactiveComplexes()
         # Default pruning
         pruned_directions = reactive_complex._prune_by_repulsion(
-            [index], coords, elements, possible_directions, nearest_neighbors, radius
+            [index], coords, possible_directions, nearest_neighbors, radius
         )
         # Test oxygen, default and 180
         # Default angle must return two points
         if index == 2:
             assert len(pruned_directions) == 2
             # Pruning with angle set to 180
             pruned_directions = reactive_complex._prune_by_repulsion(
-                [index], coords, elements, possible_directions, nearest_neighbors, radius, 180
+                [index], coords, possible_directions, nearest_neighbors, radius, 180
             )
 
             # Angle of 180 must return only one point, with lower repulsion
             ref_direction = np.array([-4.50137903e-03, -3.61081183e00, -1.68185625e-08])
             assert len(pruned_directions) == 1
             assert all([abs(pruned - ref) < 1e-6 for pruned, ref in zip(pruned_directions[0], ref_direction)])
         # Test hydrogen
@@ -186,34 +186,34 @@
         r = InterReactiveComplexes._rotation_to_vector(circle_normal, interatom)
         possible_directions = (r.T.dot(possible_directions.T)).T
         # Move exactly between atoms
         possible_directions += 0.5 * (coords[indices[0]] + coords[indices[1]])
 
         reactive_complex = InterReactiveComplexes()
         pruned_directions = reactive_complex._prune_by_repulsion(
-            indices, coords, elements, possible_directions, nearest_neighbors, radius
+            indices, coords, possible_directions, nearest_neighbors, radius
         )
 
         if indices == [0, 1]:
             ref_direction = np.array([3.02730346, 1.77840469, 1.74108634])
             assert len(pruned_directions) == 3
             assert all([abs(pruned - ref) < 1e-6 for pruned, ref in zip(pruned_directions[0], ref_direction)])
 
             pruned_directions = reactive_complex._prune_by_repulsion(
-                indices, coords, elements, possible_directions, nearest_neighbors, radius, 120
+                indices, coords, possible_directions, nearest_neighbors, radius, 120
             )
             assert len(pruned_directions) == 1
 
         if indices == [1, 2]:
             ref_direction = np.array([3.8721789, 2.36053838, -0.94589071])
             assert len(pruned_directions) == 3
             assert all([abs(pruned - ref) < 1e-6 for pruned, ref in zip(pruned_directions[0], ref_direction)])
 
             pruned_directions = reactive_complex._prune_by_repulsion(
-                indices, coords, elements, possible_directions, nearest_neighbors, radius, 40
+                indices, coords, possible_directions, nearest_neighbors, radius, 40
             )
             assert len(pruned_directions) == 2
 
 
 def test_get_attack_points_per_atom():
     ref_attack_points = np.array(
         [
@@ -472,15 +472,16 @@
 
     # Check whether rotamers of complexes with 4 distinct atoms are properly aligned
     reactive_complex.options.number_rotamers = 500
     reactive_complex.options.number_rotamers_two_on_two = 1
 
     # Align pair[0] with pair[0] and pair[1] with pair[1]
     operations = reactive_complex._set_up_rotamers(
-        coords, elements, list(pair), attack_points[pair][0:1], coords, elements, list(pair), attack_points[pair][0:1]
+        coords, elements, list(pair), attack_points[pair][0:1], coords, elements, list(
+            pair), attack_points[pair][0:1]
     )
 
     # Check, if one rotamer was generated
     assert len(operations) == 1
     tmp_op = operations[-1]
     # Check with ref operation
     for i in range(0, 4):
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/utilities/reactive_complexes/test_lebedev_sphere.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/utilities/reactive_complexes/test_lebedev_sphere.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/utilities/reactive_complexes/test_masm_pruning.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/utilities/reactive_complexes/test_masm_pruning.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/utilities/reactive_complexes/test_unit_circle.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/utilities/reactive_complexes/test_unit_circle.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/utilities/queries_test.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/utilities/queries_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,18 +25,18 @@
         assert {"model.version": "any"} not in q
         assert {'model.method': 'PM6'} in q
 
     def test_identical_reaction_query(self):
         manager = db_setup.get_clean_db("chemoton_test_identical_reaction_query")
         reactions = manager.get_collection("reactions")
         # set up compounds
-        c1 = db_setup.insert_single_empty_structure_compound(manager, db.Label.USER_OPTIMIZED)[0]
-        c2 = db_setup.insert_single_empty_structure_compound(manager, db.Label.USER_OPTIMIZED)[0]
-        c3 = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_OPTIMIZED)[0]
-        c4 = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_OPTIMIZED)[0]
+        c1 = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.USER_OPTIMIZED)[0]
+        c2 = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.USER_OPTIMIZED)[0]
+        c3 = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.MINIMUM_OPTIMIZED)[0]
+        c4 = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.MINIMUM_OPTIMIZED)[0]
         # set up reactions
         r1 = db.Reaction()
         r1.link(reactions)
         r1.create([c1], [c3])
         cl1 = [db.CompoundOrFlask.COMPOUND]
         cl2 = [db.CompoundOrFlask.COMPOUND, db.CompoundOrFlask.COMPOUND]
         assert identical_reaction([c1], [c3], cl1, cl1, reactions)
@@ -61,16 +61,16 @@
 
     def test_calculation_exists_in_structure(self):
         import scine_utilities as utils
         manager = db_setup.get_clean_db("chemoton_test_calculation_exists_in_structure")
         calculations = manager.get_collection("calculations")
         structures = manager.get_collection("structures")
 
-        _, s_id = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_GUESS)
-        _, s_id_2 = db_setup.insert_single_empty_structure_compound(manager, db.Label.MINIMUM_GUESS)
+        _, s_id = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.MINIMUM_GUESS)
+        _, s_id_2 = db_setup.insert_single_empty_structure_aggregate(manager, db.Label.MINIMUM_GUESS)
 
         model = db.Model("FAKE", "FAKE", "F-AKE")
         wrong_model = db.Model("WRONG", "wrong", "wrong")
         calculation = db.Calculation(db.ID(), calculations)
         job = db.Job("some_job")
         calculation.create(model, job, [s_id])
         settings = {
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/utilities/test_insert_initial_structure.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/utilities/test_insert_initial_structure.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/utilities/test_masm.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/utilities/test_masm.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/tests/test_database_setup.py` & `scine_chemoton-3.0.0/scine_chemoton/tests/test_database_setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,26 +2,31 @@
 # -*- coding: utf-8 -*-
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
-from typing import List, Tuple
+from typing import List, Tuple, Union
 from json import dumps
 import os
 import random
 
 # Third party imports
 import scine_database as db
 import scine_utilities as utils
 
 # local imports
 from .resources import resources_root_path
 from ..utilities.queries import identical_reaction
+from ..utilities.energy_query_functions import get_energy_for_structure
+
+
+def get_fake_model() -> db.Model:
+    return db.Model("FAKE", "FAKE", "F-AKE")
 
 
 def get_test_db_credentials(name: str = "chemoton_unittests") -> db.Credentials:
     """
     Generate a set of credentials pointing to a database and server.
     The server IP and port are assumed to be `127.0.0.1` and `27017`
     unless specified otherwise with the environment variables
@@ -125,15 +130,15 @@
     assert n_inserts <= n_compounds
     # enough reactions and allowed products to create the non-user-inserted compounds
     assert n_compounds < (n_reactions - n_flasks) * max_n_products_per_r
     # enough compounds for the biggest possible reaction
     assert n_compounds > max_n_products_per_r + max_n_educts_per_r
     # at least 2 compounds per reaction -> maximum allowed number of reactions
     assert 0.5 * n_compounds * max_r_per_c > n_reactions
-    # worst case all reactions are biggest possible reaction
+    # worst case all reactions are the biggest possible reaction
     assert n_compounds * max_r_per_c > n_reactions * (max_n_products_per_r + max_n_educts_per_r)
 
     manager = get_clean_db(name)
     properties = manager.get_collection("properties")
     compounds = manager.get_collection("compounds")
     flasks = manager.get_collection("flasks")
     reactions = manager.get_collection("reactions")
@@ -154,15 +159,14 @@
             barrier_limits,
             reactions,
             compounds,
             properties,
             structures,
             elementary_steps,
         )
-
     # not guaranteed to have all necessary compounds yet
     # create missing ones and add them as products on reactions where we still have space for them
     n_missing_compounds = n_compounds - compounds.count("{}")
     for _ in range(n_missing_compounds):
         compound_id = _create_compound(max_s_per_c, properties, compounds, structures, user_input=False)
         compound = db.Compound(compound_id)
         compound.link(compounds)
@@ -183,21 +187,22 @@
 
         # if none left, substitute products of reactions that are produced with multiple reactions
         while not got_reaction:
             random_reaction = reactions.random_select_reactions(1)[0]
             random_reaction.link(reactions)
             products = random_reaction.get_reactants(db.Side.RHS)[1]
             for product_id in products:
+                compound_or_flask = random_reaction.get_reactant_type(product_id)
                 selection = {"rhs": {"$elemMatch": {"id": {"$oid": str(product_id)}}}}
                 if reactions.count(dumps(selection)) > 1:
                     multiple_product = db.Compound(product_id)
                     multiple_product.link(compounds)
                     multiple_product.remove_reaction(random_reaction.get_id())
                     random_reaction.remove_reactant(product_id, db.Side.RHS)
-                    random_reaction.add_reactant(compound.get_id(), db.Side.RHS, db.CompoundOrFlask.COMPOUND)
+                    random_reaction.add_reactant(compound.get_id(), db.Side.RHS, compound_or_flask)
                     _redo_elementary_steps(
                         random_reaction,
                         max_steps_per_r,
                         barrier_limits,
                         compounds,
                         structures,
                         elementary_steps,
@@ -308,44 +313,46 @@
 
 def _create_compound(
     max_structures: int,
     properties: db.Collection,
     compounds: db.Collection,
     structures: db.Collection,
     user_input: bool = False,
-    energy_limits: Tuple[float, float] = (-20.0, -10.0)
+    energy_limits: Tuple[float, float] = (-20.0, -10.0),
+    model: db.Model = db.Model("FAKE", "FAKE", "F-AKE")
 ):
     c = db.Compound(db.ID())
     c.link(compounds)
     c.create([])
     for _ in range(random.randint(1, max_structures)):
-        c.add_structure(_fake_structure(c, structures, properties, user_input, energy_limits))
+        c.add_structure(_fake_structure(c, structures, properties, user_input, energy_limits, model))
     c.disable_exploration()
 
     return c.get_id()
 
 
 def _fake_structure(
     compound: db.Compound,
     structures: db.Collection,
     properties: db.Collection,
     user_input: bool,
-    energy_limits: Tuple[float, float] = (-20.0, -10.0)
+    energy_limits: Tuple[float, float] = (-20.0, -10.0),
+    model: db.Model = db.Model("FAKE", "FAKE", "F-AKE")
 ):
     # Add structure data
     structure = db.Structure()
     structure.link(structures)
     structure.create(os.path.join(resources_root_path(), "water.xyz"), 0, 1)
     if user_input:
         structure.set_label(db.Label.USER_OPTIMIZED)
     else:
         structure.set_label(db.Label.MINIMUM_OPTIMIZED)
     structure.set_aggregate(compound.get_id())
-    structure.set_model(db.Model("FAKE", "FAKE", "F-AKE"))
-    add_random_energy(structure, energy_limits, properties)
+    structure.set_model(model)
+    add_random_energy(structure, energy_limits, properties, model)
 
     return structure.get_id()
 
 
 def _create_reaction(
     n_compounds: int,
     max_s_per_c: int,
@@ -439,27 +446,29 @@
 def _add_step(
     reaction: db.Reaction,
     barrier_limits: Tuple[float, float],
     compounds: db.Collection,
     structures: db.Collection,
     elementary_steps: db.Collection,
     properties: db.Collection,
+    model: db.Model = db.Model("FAKE", "FAKE", "F-AKE")
 ) -> db.ID:
     step = db.ElementaryStep()
     step.link(elementary_steps)
-    model = db.Model("FAKE", "FAKE", "F-AKE")
     compound_sides = reaction.get_reactants(db.Side.BOTH)
     # pick random structure for each compound
     step_structures = []
     for side in compound_sides:
         side_structures = []
         for c_id in side:
             c = db.Compound(c_id)
             c.link(compounds)
-            side_structures.append(random.choice(c.get_structures()))
+            selected_structures = [s_id for s_id in c.get_structures() if get_energy_for_structure(
+                db.Structure(s_id, structures), "electronic_energy", model, structures, properties) is not None]
+            side_structures.append(random.choice(selected_structures))
         step_structures.append(side_structures)
     step.create(*step_structures)
     reactant_energies = sum(
         [
             _get_electronic_energy(db.Structure(reactant), structures, properties, model)
             for reactant in step_structures[0]
         ]
@@ -486,30 +495,33 @@
     return step.get_id()
 
 
 def add_random_energy(
     structure: db.Structure,
     energy_limits: Tuple[float, float],
     properties: db.Collection,
+    model: db.Model = db.Model("FAKE", "FAKE", "F-AKE")
 ):
     """
     Adds a random electronic energy property to the given structure within the given limits.
 
     Parameters
     ----------
     structure :: db.Structure
         The Structure to add the energy to
     energy_limits :: Tuple[float, float]
         The lowest and highest possible energy in kJ/mol
     properties :: db.Collection
         The properties collection of the database
+    model :: db.Model
+        The model for the energy.
     """
     prop = db.NumberProperty()
     prop.link(properties)
-    prop.create(db.Model("FAKE", "FAKE", "F-AKE"), "electronic_energy",
+    prop.create(model, "electronic_energy",
                 random.uniform(*energy_limits) * utils.HARTREE_PER_KJPERMOL)
     structure.add_property(prop.get_property_name(), prop.get_id())
 
     return prop.get_id()
 
 
 def _get_electronic_energy(
@@ -524,42 +536,86 @@
         raise RuntimeError("Missing requested electronic energy!")
     # pick last property if multiple
     prop = db.NumberProperty(properties[-1])
     prop.link(properties_coll)
     return prop.get_data() * utils.KJPERMOL_PER_HARTREE
 
 
-def insert_single_empty_structure_compound(manager: db.Manager, label: db.Label) -> Tuple[db.ID, db.ID]:
+def insert_single_empty_structure_aggregate(manager: db.Manager, label: db.Label) -> Tuple[db.ID, db.ID]:
+    """
+    Adds a structure and corresponding compound or flask to the database, only use for testing!
+    A flask is added if a complex is requested.
+
+    Parameters
+    ----------
+    manager :: db.Manager
+        The database manager
+    label :: db.Label
+        The label for the structure of the compound
+
+    Returns
+    -------
+    aggregate, structure :: Tuple[db.ID, db.ID]
+        The IDs of the inserted compound/flask and structure.
+    """
+    build_flask = label in [db.Label.COMPLEX_GUESS, db.Label.COMPLEX_OPTIMIZED]
+    structures = manager.get_collection("structures")
+    structure_xyz = "water.xyz"
+    aggregates = manager.get_collection("compounds")
+    aggregate: Union[db.Compound, db.Flask] = db.Compound()
+    if build_flask:
+        aggregates = manager.get_collection("flasks")
+        aggregate = db.Flask()  # type: ignore
+        structure_xyz = "proline_propanal_complex.xyz"
+    structure = db.Structure()
+    structure.link(structures)
+    rr = resources_root_path()
+    structure.create(os.path.join(rr, structure_xyz), 0, 1)
+    aggregate.link(aggregates)
+    if build_flask:
+        aggregate.create([structure.get_id()], [])  # type: ignore
+    else:
+        aggregate.create([structure.get_id()])  # type: ignore
+    aggregate.disable_exploration()
+    structure.set_aggregate(aggregate.get_id())
+    structure.set_label(label)
+    structure.set_model(db.Model("FAKE", "FAKE", "F-AKE"))
+
+    return aggregate.get_id(), structure.get_id()
+
+
+def insert_single_empty_structure_flask(manager: db.Manager, label: db.Label) -> Tuple[db.ID, db.ID]:
     """
     Adds a structure and corresponding compound to the database, only use for testing!
 
     Parameters
     ----------
     manager :: db.Manager
         The database manager
     label :: db.Label
         The label for the structure of the compound
     -------
-    compound, structure :: Tuple[db.ID, db.ID]
+    flask, structure :: Tuple[db.ID, db.ID]
         The IDs of the inserted compound and structure
     """
     structures = manager.get_collection("structures")
-    compounds = manager.get_collection("compounds")
+    flasks = manager.get_collection("flasks")
     structure = db.Structure()
     structure.link(structures)
     rr = resources_root_path()
-    structure.create(os.path.join(rr, "water.xyz"), 0, 1)
-    compound = db.Compound()
-    compound.link(compounds)
-    compound.create([structure.get_id()])
-    compound.disable_exploration()
-    structure.set_aggregate(compound.get_id())
+    structure.create(os.path.join(rr, "h4o2.xyz"), 0, 1)
+    flask = db.Flask()
+    flask.link(flasks)
+    flask.create([structure.get_id()], [])
+    flask.disable_exploration()
+    structure.set_aggregate(flask.get_id())
     structure.set_label(label)
+    structure.set_model(db.Model("FAKE", "FAKE", "F-AKE"))
 
-    return compound.get_id(), structure.get_id()
+    return flask.get_id(), structure.get_id()
 
 
 def test_random_db():
     n_compounds = 9
     n_reactions = 6
     n_flasks = 1
     max_r_per_c = 10
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/utilities/reactive_complexes/__init__.py` & `scine_chemoton-3.0.0/scine_chemoton/utilities/reactive_complexes/__init__.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/utilities/reactive_complexes/inter_reactive_complexes.py` & `scine_chemoton-3.0.0/scine_chemoton/utilities/reactive_complexes/inter_reactive_complexes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
 import numpy as np
 from copy import deepcopy
-from typing import Dict, List, Optional, Tuple, Union, Generator
+from typing import Dict, List, Optional, Tuple, Union, Generator, Set, Any
 from scipy.sparse.csgraph import connected_components
 from scipy.spatial import distance_matrix
 
 # Third party imports
 import scine_database as db
 import scine_utilities as utils
 
@@ -28,15 +28,15 @@
     lhs_list: List[int],
     rhs_list: List[int],
     x_alignment_0: Optional[List[float]] = None,
     x_alignment_1: Optional[List[float]] = None,
     x_rotation: float = 0.0,
     x_spread: float = 2.0,
     displacement: float = 0.0,
-):
+) -> Tuple[utils.AtomCollection, List[int], List[int]]:
     """
     Assembles a reactive complex from the parameters generated by the
     InterReactiveComplexes class.
 
     Parameters
     ----------
     atoms1, atoms2 :: utils.AtomCollection
@@ -90,15 +90,14 @@
     elements1 = atoms1.elements
     elements2 = atoms2.elements
     coordinates1 = atoms1.positions
     coordinates2 = atoms2.positions
     # Calculate reactive center mean position
     sites1 = lhs_list
     sites2 = rhs_list
-    rhs_list = list(idx + len(elements1) for idx in sites2)
     reactive_center1 = np.mean(coordinates1[sites1], axis=0)
     reactive_center2 = np.mean(coordinates2[sites2], axis=0)
     # Place reactive center mean position into origin
     coord1 = coordinates1 - reactive_center1
     coord2 = coordinates2 - reactive_center2
     # Rotate directions towards each other
     r = np.array(x_alignment_0).reshape((3, 3))
@@ -113,15 +112,16 @@
     coord2 += np.array([x_spread, 0.0, 0.0])
     coord1 -= np.array([x_spread, 0.0, 0.0])
     # Apply small seeded random displacement
     np.random.seed(42)
     coord1 += displacement * (np.random.rand(*coord1.shape) - 0.5) * 2.0 / np.sqrt(3.0)
     coord2 += displacement * (np.random.rand(*coord2.shape) - 0.5) * 2.0 / np.sqrt(3.0)
     start_atoms = utils.AtomCollection(elements1 + elements2, np.concatenate((coord1, coord2), axis=0))
-    return start_atoms, lhs_list, rhs_list
+    shifted_rhs_list = list(idx + len(elements1) for idx in sites2)
+    return start_atoms, lhs_list, shifted_rhs_list
 
 
 class InterReactiveComplexes(ReactiveComplexes):
     """
     Class to generate reactive complexes from two structures.
     """
 
@@ -157,14 +157,15 @@
                 (default: True)
             """
 
     def __init__(self):
         super().__init__()
         self.options = self.Options()
         self.__cache = {}
+        self.lebedev = LebedevSphere()
 
     @staticmethod
     def _rotation_to_vector(to_rotate: np.ndarray, direction: np.ndarray):
         """
         Generates  a rotation matrix to rotate the row vector 'to_rotate' into
         the direction 'direction'.
 
@@ -226,20 +227,21 @@
             The additional shift required to separate the molecules along the x-axis.
         """
 
         extra_shift = 0.0
         for e1, p1 in zip(elem1, coord1):
             for e2, p2 in zip(elem2, coord2):
                 dist_vec = p2 - p1
-                dist = np.linalg.norm(dist_vec)
+                dist2 = np.inner(dist_vec, dist_vec)
                 min_dist = utils.ElementInfo.vdw_radius(e1) + utils.ElementInfo.vdw_radius(e2)
-                if dist < min_dist:
+                min_dist2 = min_dist * min_dist
+                if dist2 < min_dist2:
                     # Compute shift s.t. shifting into the x-direction results
                     #  into the required minimum distance
-                    new_shift = -1.0 * dist_vec[0] + np.sqrt(dist_vec[0] * dist_vec[0] + min_dist ** 2 - dist ** 2)
+                    new_shift = -1.0 * dist_vec[0] + np.sqrt(dist_vec[0] * dist_vec[0] + min_dist2 - dist2)
                     new_shift = 0.5 * new_shift
                     if extra_shift < new_shift:
                         extra_shift = new_shift
         return extra_shift
 
     @staticmethod
     def _prune_buried_points(
@@ -279,24 +281,28 @@
         # Identify close atoms that are not within indices
         close_atoms = []
         vdw_params = []
         centroid = np.mean(coords[list(indices)], axis=0)
         for idx, (c, e) in enumerate(zip(coords, element_types)):
             if idx in indices:
                 continue
-            dist = np.linalg.norm(c - centroid)
-            if dist < 10.0:
+            dist_vec = c - centroid
+            dist2 = np.inner(dist_vec, dist_vec)
+            if dist2 < 100.0:
                 close_atoms.append(c)
                 vdw_params.append(vdw_scaling * utils.ElementInfo.vdw_radius(e))
 
         # Delete all points within the vdW sphere of other atoms
         remaining = []
         for i, point in enumerate(points):
             for c, v in zip(close_atoms, vdw_params):
-                if np.linalg.norm(c - point) < v:
+                v2 = v * v
+                dist_vec = c - point
+                dist2 = np.inner(dist_vec, dist_vec)
+                if dist2 < v2:
                     break
             else:
                 remaining.append(i)
         pruned = np.zeros((len(remaining), 3))
         for i, j in enumerate(remaining):
             pruned[i][0] = points[j][0]
             pruned[i][1] = points[j][1]
@@ -347,15 +353,14 @@
             valley_pruned[i] = points[k]
         return valley_pruned
 
     def _prune_by_repulsion(
         self,
         indices: Union[Tuple[int], Tuple[int, int]],
         coords: np.ndarray,
-        element_types: List,
         points: np.ndarray,
         nearest_neighbors,
         radius: float,
         min_angle_distance: float = 20.0,
     ) -> np.ndarray:
         """
         Prunes points from the given list of points centered around the centroid of the atoms with
@@ -377,16 +382,14 @@
 
         Parameters
         ----------
         indices : Tuple[int]
             The indices of the atoms around whose centroid the points are centered.
         coords : np.ndarray of shape (n,3)
             Atom positions.
-        element_types : List[utils.ElementType] of size n
-            Element types of elements.
         points : np.ndarray of shape (x,3)
             A 2D array (matrix) of points centered around the atom with the index
             'index'.
         nearest_neighbors : List[List[int]] of length x
             The indices of the nearest neighbors of all points.
         radius : float
             The radius of the sphere or circle the points are located on.
@@ -401,34 +404,33 @@
             if no point is left/viable.
         """
         if len(points) == 0:
             return np.zeros((0, 0))
 
         # Identify close atoms
         close_atoms = []
-        vdw_params = []
         centroid = np.mean(coords[list(indices)], axis=0)
-        for idx, (c, e) in enumerate(zip(coords, element_types)):
+        for idx, c in enumerate(coords):
             if idx in indices:
                 continue
-            dist = np.linalg.norm(c - centroid)
-            if dist < 15.0:
+            dist_vec = c - centroid
+            dist2 = np.inner(dist_vec, dist_vec)
+            if dist2 < 225.0:  # 15**2
                 close_atoms.append(c)
-                vdw_params.append(utils.ElementInfo.vdw_radius(e))
 
         # Calculate Repulsion
         repulsion = []
         for p in points:
             r: float = 0.0
             for c in close_atoms:
-                dist = np.linalg.norm(c - p)
-                if dist <= 0.0:
+                dist_vec = c - p
+                d2 = np.inner(dist_vec, dist_vec)
+                if d2 <= 0.0:
                     r += float("inf")
                 else:
-                    d2 = dist * dist
                     r += float(1.0 / (d2 * d2 * d2))
             repulsion.append(r)
 
         if self.options.multiple_attack_points:
             keepers = []
             for i, nn in enumerate(nearest_neighbors):
                 if np.isinf(repulsion[i]):
@@ -483,26 +485,25 @@
         Returns
         -------
         Dict[Tuple[int], np.ndarray]]
             One np.ndarray of shape (n,3) per atom for which there is at least
             one attack point and index of that atom
         """
 
-        lebedev = LebedevSphere()
-        initial_points = lebedev.points
-        nearest_neighbors = lebedev.nearest_neighbors
+        initial_points = self.lebedev.points
+        nearest_neighbors = self.lebedev.nearest_neighbors
 
         per_atom = {}
         for i, e in enumerate(element_types):
             if indices is not None and i not in indices:
                 continue
             possible_directions = deepcopy(initial_points) * utils.ElementInfo.vdw_radius(e)
             possible_directions += coords[i]
             possible_directions = self._prune_by_repulsion(
-                (i,), coords, element_types, possible_directions, nearest_neighbors, utils.ElementInfo.vdw_radius(e)
+                (i,), coords, possible_directions, nearest_neighbors, utils.ElementInfo.vdw_radius(e)
             )
             possible_directions = self._prune_buried_points(
                 (i,), coords, element_types, possible_directions, vdw_scaling=vdw_scaling
             )
             if not possible_directions.size == 0:
                 if (i,) in per_atom:
                     raise RuntimeError("Requested attack points for the same atom twice.")
@@ -555,15 +556,15 @@
             circle_normal = np.array([0.0, 0.0, 1.0])  # Initial points are in xy-plane
             r = self._rotation_to_vector(circle_normal, interatom)
             possible_directions = (r.T.dot(possible_directions.T)).T
             # Move exactly between atoms
             possible_directions += 0.5 * (coords[i] + coords[j])
             # Prune
             possible_directions = self._prune_by_repulsion(
-                (i, j), coords, element_types, possible_directions, nearest_neighbors, circle_radius
+                (i, j), coords, possible_directions, nearest_neighbors, circle_radius
             )
             possible_directions = self._prune_buried_points(
                 (i, j), coords, element_types, possible_directions, vdw_scaling=vdw_scaling
             )
             # Since indices are stored empty entries are not necessary
             if not possible_directions.size == 0:
                 if (i, j) in per_atom_pair:
@@ -792,75 +793,79 @@
         elements1 = atoms1.elements
         id1 = str(structure1.get_id())
 
         # Get structure two data
         atoms2 = structure2.get_atoms()
         coordinates2 = atoms2.positions
         elements2 = atoms2.elements
-        id2 = str(structure1.get_id())
+        id2 = str(structure2.get_id())
 
         # Get all attack points needed
         # A dictionary with the attack points stored for all relevant atoms and
         #  atom pairs with the indices being the keys
+        attack_points1: Dict[Any, np.ndarray] = {}
+        attacked_atoms1: Set[int] = set()
+        attacked_pairs1: Set[Tuple[int, int]] = set()
+        attack_points2: Dict[Any, np.ndarray] = {}
+        attacked_atoms2: Set[int] = set()
+        attacked_pairs2: Set[Tuple[int, int]] = set()
 
         # Load cache if possible
         if id1 in self.__cache:
             attack_points1 = self.__cache[id1]["points"]
             attacked_atoms1 = self.__cache[id1]["atoms"]
             attacked_pairs1 = self.__cache[id1]["pairs"]
-        else:
-            attack_points1 = {}
-            attacked_atoms1 = set()
-            attacked_pairs1 = set()
         if id2 in self.__cache:
             attack_points2 = self.__cache[id2]["points"]
             attacked_atoms2 = self.__cache[id2]["atoms"]
             attacked_pairs2 = self.__cache[id2]["pairs"]
-        else:
-            attack_points2 = {}
-            attacked_atoms2 = set()
-            attacked_pairs2 = set()
-
-        new_attacked_atoms1 = set()
-        new_attacked_pairs1 = set()
-        new_attacked_atoms2 = set()
-        new_attacked_pairs2 = set()
+
+        new_attacked_atoms1: Set[int] = set()
+        new_attacked_pairs1: Set[Tuple[int, int]] = set()
+        new_attacked_atoms2: Set[int] = set()
+        new_attacked_pairs2: Set[Tuple[int, int]] = set()
         for coord in reactive_inter_coords:
 
             if len(coord) > 2:
-                raise RuntimeError("More than two interstructural coordinates are not supported")
+                raise RuntimeError("More than two inter-structural coordinates are not supported")
 
             elif len(coord) == 1:
                 # If one atom pair only, then the sites on both structures are monoatomic
                 if coord[0][0] not in attacked_atoms1:
                     new_attacked_atoms1.add(coord[0][0])
                 if coord[0][1] not in attacked_atoms2:
                     new_attacked_atoms2.add(coord[0][1])
             elif len(coord) == 2:
                 # Get unique reactive atoms per structure to check whether twice the same atom or distinct atom pair
                 struct1_sites = set(pair[0] for pair in coord)
                 struct2_sites = set(pair[1] for pair in coord)
-                if len(struct1_sites) == 1 and not struct1_sites.issubset(attacked_atoms1):
-                    new_attacked_atoms1.update(struct1_sites)
-                elif len(struct1_sites) == 2 and not tuple(sorted(struct1_sites)) in attacked_pairs1:
-                    new_attacked_pairs1.add(tuple(sorted(struct1_sites)))
+                if len(struct1_sites) == 1:
+                    if not struct1_sites.issubset(attacked_atoms1):
+                        new_attacked_atoms1.update(struct1_sites)
+                elif len(struct1_sites) == 2:
+                    tmp_tup = tuple(sorted(struct1_sites))
+                    if tmp_tup not in attacked_pairs1:
+                        new_attacked_pairs1.add((tmp_tup[0], tmp_tup[1]))
                 elif len(struct1_sites) > 2:
                     # Should not be reachable
                     raise RuntimeError(
                         "More than two atoms per structure involved in "
-                        + "interstructural reaction coordinates are not supported"
+                        + "inter-structural reaction coordinates are not supported"
                     )
-                if len(struct2_sites) == 1 and not struct2_sites.issubset(attacked_atoms2):
-                    new_attacked_atoms2.update(struct2_sites)
-                elif len(struct2_sites) == 2 and not tuple(sorted(struct2_sites)) in attacked_pairs2:
-                    new_attacked_pairs2.add(tuple(sorted(struct2_sites)))
+                if len(struct2_sites) == 1:
+                    if not struct2_sites.issubset(attacked_atoms2):
+                        new_attacked_atoms2.update(struct2_sites)
+                elif len(struct2_sites) == 2:
+                    tmp_tup = tuple(sorted(struct2_sites))
+                    if tmp_tup not in attacked_pairs2:
+                        new_attacked_pairs2.add((tmp_tup[0], tmp_tup[1]))
                 elif len(struct2_sites) > 2:
                     # Should not be reachable
                     raise RuntimeError(
-                        "More than two atoms per structure involved in interstructural "
+                        "More than two atoms per structure involved in inter-structural "
                         + "reaction coordinates are not supported"
                     )
 
         # Generate attack points around atoms
         attack_points1.update(self._get_attack_points_per_atom(
             coordinates1, elements1, indices=list(new_attacked_atoms1)))
         attack_points2.update(self._get_attack_points_per_atom(
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/utilities/reactive_complexes/lebedev_sphere.py` & `scine_chemoton-3.0.0/scine_chemoton/utilities/reactive_complexes/lebedev_sphere.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/utilities/reactive_complexes/unit_circle.py` & `scine_chemoton-3.0.0/scine_chemoton/utilities/reactive_complexes/unit_circle.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/utilities/calculation_creation_helpers.py` & `scine_chemoton-3.0.0/scine_chemoton/utilities/calculation_creation_helpers.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/utilities/compound_and_flask_creation.py` & `scine_chemoton-3.0.0/scine_chemoton/utilities/compound_and_flask_creation.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,26 +17,26 @@
     in common. Through this function, we do not have to differentiate between them at every point.
 
     Parameters
     ----------
     object_id :: db.ID
         The ID of the object to construct.
     object_type :: db.CompoundOrFlask
-        The label for Compound or Flaks.
+        The label for Compound or Flask.
     compounds :: db.Collection
         The compounds collection.
     flasks :: db.Collection
         The flasks collection.
 
     Returns
     -------
     Either the flask or compound object.
 
-    Note
-    ----
+    Notes
+    -----
     Raises a runtime error if the object_type is unknown.
     """
     if object_type == db.CompoundOrFlask.COMPOUND:
         return db.Compound(object_id, compounds)
     if object_type == db.CompoundOrFlask.FLASK:
         return db.Flask(object_id, flasks)
     raise RuntimeError("Requested aggregate type is not supported.")
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/utilities/energy_query_functions.py` & `scine_chemoton-3.0.0/scine_chemoton/utilities/energy_query_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,72 +2,90 @@
 # -*- coding: utf-8 -*-
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
-from typing import Union, Tuple
+from typing import Union, Tuple, List, Optional
 import numpy as np
 # Third party imports
 import scine_database as db
 import scine_utilities as utils
 
 
-def get_elementery_step_with_min_ts_energy(reaction: db.Reaction, energy_type: str, model: db.Model,
-                                           elementary_steps: db.Collection, structures: db.Collection,
-                                           properties: db.Collection) -> Union[db.ID, None]:
+def get_elementary_step_with_min_ts_energy(reaction: db.Reaction,
+                                           energy_type: str,
+                                           model: db.Model,
+                                           elementary_steps: db.Collection,
+                                           structures: db.Collection,
+                                           properties: db.Collection,
+                                           structure_model: Optional[db.Model] = None) -> Optional[db.ID]:
     """
     Gets the elementary step ID with the lowest energy of the corresponding transition state of a reaction.
 
-
     Parameters
     ----------
     reaction : db.Reaction
-        _description_
+        The reaction for which the elementary steps shall be analyzed.
     energy_type : str
         The name of the energy property such as 'electronic_energy' or 'gibbs_free_energy'
     model : scine_database.Model
         The model used to calculate the energies.
     elementary_steps : db.Collection
         The elementary step collection.
     structures : scine_database.Collection
         The structure collection.
     properties : scine_database.Collection
         The property collection.
+    structure_model : Optional[db.Model]
+        The model of the transition state. If None, the model of the transition state is not checked.
 
     Returns
     -------
-    Union[db.ID, None]
-        _description_
+    Optional[db.ID]
+        The ID of the elementary step with the lowest TS energy.
     """
     lowest_ts_energy = np.inf
     es_id_with_lowest_ts = None
     # # # Loop over elementary steps
     for es_id in reaction.get_elementary_steps():
         es = db.ElementaryStep(es_id, elementary_steps)
         # # # Type check elementary step and break if barrierless
         if es.get_type() == db.ElementaryStepType.BARRIERLESS:
+            first_structure_lhs = db.Structure(es.get_reactants()[0][0], structures)
+            if structure_model is not None and first_structure_lhs.get_model() != structure_model:
+                continue
+            # # # Energy Check for minima
+            first_structure_lhs_energy = get_energy_for_structure(first_structure_lhs, energy_type, model,
+                                                                  structures, properties)
+            if first_structure_lhs_energy is None:
+                continue
             es_id_with_lowest_ts = es_id
             break
-        ts = db.Structure(es.get_transition_state())
+        ts = db.Structure(es.get_transition_state(), structures)
+        if structure_model is not None and ts.get_model() != structure_model:
+            continue
+
+        # # # Costly safety check that barrier as well as ts_energy exist for this model and energy type
         ts_energy = get_energy_for_structure(
             ts, energy_type, model, structures, properties)
-        if ts_energy is None:
+        barriers = get_barriers_for_elementary_step_by_type(es, energy_type, model, structures, properties)
+        if None in barriers or ts_energy is None:
             continue
-        assert ts_energy
+        # # # Comparison with current lowest energy
         if ts_energy < lowest_ts_energy:
             es_id_with_lowest_ts = es_id
             lowest_ts_energy = ts_energy
 
     return es_id_with_lowest_ts
 
 
 def get_energy_sum_of_elementary_step_side(step: db.ElementaryStep, side: db.Side, energy_type: str, model: db.Model,
-                                           structures: db.Collection, properties: db.Collection) -> Union[float, None]:
+                                           structures: db.Collection, properties: db.Collection) -> Optional[float]:
     """
     Gives the total energy in atomic units of the given side of the step. Returns None if the energy type is
     not available.
 
     Parameters
     ----------
     step : scine_database.ElementaryStep (Scine::Database::ElementaryStep)
@@ -81,15 +99,15 @@
     structures : scine_database.Collection
         The structure collection.
     properties : scine_database.Collection
         The property collection.
 
     Returns
     -------
-    Union[float, None]
+    Optional[float]
         Energy in hartree
     """
     if side == db.Side.BOTH:
         raise RuntimeError("The energy sum of both sides of a step is not supported.")
     index = 0 if side == db.Side.LHS else 1
     energies = [
         get_energy_for_structure(db.Structure(reactant), energy_type, model, structures, properties)
@@ -196,7 +214,52 @@
     """
     barrier_j_per_mol = 1e+3 * barrier
     kbt_in_j = utils.BOLTZMANN_CONSTANT * temperature  # k_B T
     factor = kbt_in_j / utils.PLANCK_CONSTANT  # k_B T / h
     rt_in_j_per_mol = utils.MOLAR_GAS_CONSTANT * temperature  # R T
     beta_in_mol_per_j = 1.0 / rt_in_j_per_mol  # 1 / (R T)
     return factor * np.exp(- beta_in_mol_per_j * barrier_j_per_mol)
+
+
+def get_all_energies_for_aggregate(aggregate: Union[db.Compound, db.Flask], model: db.Model, energy_label: str,
+                                   structures: db.Collection, properties: db.Collection) -> List[Union[float, None]]:
+    all_energies = []
+    for s_id in aggregate.get_structures():
+        structure = db.Structure(s_id)
+        all_energies.append(get_energy_for_structure(structure, energy_label, model, structures, properties))
+    return all_energies
+
+
+def get_min_energy_for_aggregate(aggregate: Union[db.Compound, db.Flask], model: db.Model, energy_label: str,
+                                 structures: db.Collection, properties: db.Collection) -> Optional[float]:
+    all_energies = get_all_energies_for_aggregate(aggregate, model, energy_label, structures, properties)
+    if len(all_energies) < 1:
+        return None
+    non_none_energies = list()
+    for e in all_energies:
+        if e is not None:
+            non_none_energies.append(e)
+    if len(non_none_energies) < 1:
+        return None
+    return min(non_none_energies)
+
+
+def get_min_free_energy_for_aggregate(aggregate: Union[db.Compound, db.Flask], electronic_model: db.Model,
+                                      correction_model: db.Model, structures: db.Collection,
+                                      properties: db.Collection) -> Optional[float]:
+    equal_models = electronic_model == correction_model
+    if equal_models:
+        return get_min_energy_for_aggregate(aggregate, electronic_model, "gibbs_free_energy", structures, properties)
+    all_energies: List[float] = []
+    for s_id in aggregate.get_structures():
+        structure = db.Structure(s_id)
+        electronic_energy = get_energy_for_structure(structure, "electronic_energy", electronic_model, structures,
+                                                     properties)
+        free_energy_correction = get_energy_for_structure(structure, "gibbs_energy_correction", correction_model,
+                                                          structures, properties)
+        if electronic_energy is None or free_energy_correction is None:
+            continue
+        energy = electronic_energy + free_energy_correction
+        all_energies.append(energy)
+    if not all_energies:
+        return None
+    return min(all_energies)
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/utilities/get_molecular_formula.py` & `scine_chemoton-3.0.0/scine_chemoton/utilities/get_molecular_formula.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 # from typing import Union
 import scine_database as db
 import scine_utilities as utils
+import scine_molassembler as masm
 
 
 def get_molecular_formula_of_structure(structure_id: db.ID, structures: db.Collection) -> str:
     """
     Get the molecular formula of a given structure, its charge ("c") and its multiplicity ("m") as a string.
 
     Parameters
@@ -61,15 +62,15 @@
     molecular formula :: str
         The molecular formula of the given aggregate according to the aggregates type.
 
     """
     if object_type == db.CompoundOrFlask.COMPOUND:
         molecular_formula = get_molecular_formula_of_compound(object_id, compounds, structures)
     elif object_type == db.CompoundOrFlask.FLASK:
-        molecular_formula = get_molecular_formula_of_flask(object_id, flasks, compounds, structures)
+        molecular_formula = get_molecular_formula_of_flask(object_id, flasks, structures)
 
     return molecular_formula
 
 
 def get_molecular_formula_of_compound(compound_id: db.ID, compounds: db.Collection, structures: db.Collection) -> str:
     """
     Get the molecular formula of a given compound, its charge ("c") and its multiplicity ("m") as a string.
@@ -92,40 +93,60 @@
     centroid_id = compound.get_centroid()
     return get_molecular_formula_of_structure(centroid_id, structures)
 
 
 def get_molecular_formula_of_flask(
         flask_id: db.ID,
         flasks: db.Collection,
-        compounds: db.Collection,
         structures: db.Collection) -> str:
     """
     Get the molecular formula of a given flask, its charge ("c") and its multiplicity ("m") and the identical
     information of the compounds the flask consists of as a string.
 
     Parameters
     ----------
     flask_id : db.ID
         The database ID of the flask.
     flasks : db.Collection
         The flask collection.
-    compounds : db.Collection
-        The compound collection.
     structures : db.Collection
         The structure collection.
 
     Returns
     -------
     str
-        The molecular formula of the given flask and the molecular formulas of the compounds, e.g. for the water dimer
-        "H4O2 (c:0, m:1) [H2O (c:0, m:1)|H2O (c:0, m:1)]".
+        The molecular formula of the given flask and the molecular formulas of the compounds according to the CBOR
+        graph of its structure, e.g. for the water dimer "H4O2 (c:0, m:1) [H2O | H2O ]".
     """
     flask = db.Flask(flask_id, flasks)
     centroid_id = flask.get_centroid()
     molecular_formula = get_molecular_formula_of_structure(centroid_id, structures) + " ["
-    for compound_id in flask.get_compounds():
-        molecular_formula += get_molecular_formula_of_compound(compound_id, compounds, structures)
-        molecular_formula += "|"
+    centroid = db.Structure(centroid_id, structures)
+    # Loop over individual masm cbor graphs
+    for cmp_cbor_graph in centroid.get_graph("masm_cbor_graph").split(";"):
+        molecular_formula += get_molecular_formula_from_cbor_string(cmp_cbor_graph)
+        molecular_formula += " | "
+    molecular_formula = molecular_formula[:-3] + "]"
+
+    return molecular_formula
+
 
-    molecular_formula = molecular_formula[:-1] + "]"
+def get_molecular_formula_from_cbor_string(cbor_graph: str) -> str:
+    """
+    Get the molecular formula of a given CBOR Graph.
+
+    Parameters
+    ----------
+    cbor_graph :: str
+        The string of a CBOR graph.
+
+    Returns
+    -------
+    str
+        The plain molecular formula of the given CBOR graph.
+    """
+    binary = masm.JsonSerialization.base_64_decode(cbor_graph)
+    serialization = masm.JsonSerialization(binary, masm.JsonSerialization.BinaryFormat.CBOR)
+    masm_molecule = serialization.to_molecule()
+    molecular_formula = utils.generate_chemical_formula([masm_molecule.graph[i] for i in masm_molecule.graph.atoms()])
 
     return molecular_formula
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/utilities/insert_concentration.py` & `scine_chemoton-3.0.0/scine_chemoton/utilities/insert_concentration.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,36 +3,50 @@
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Third party imports
 import scine_database as db
+from warnings import warn
 
 
 def insert_concentration_for_compound(
         database: db.Manager,
         value: float,
         model: db.Model,
         compound_id: db.ID,
         replace_old: bool = True,
         label: str = "start_concentration"
 ):
-    concentration_options = ["start_concentration", "max_concentration", "final_concentration", "concentration_flux"]
-    if label not in concentration_options:
-        raise RuntimeError("The concentration label must be label either: 'start_concentration', 'max_concentration',"
-                           "'final_concentration', or 'concentration_flux'.")
+    compounds = database.get_collection("compounds")
+    compound = db.Compound(compound_id, compounds)
+    centroid_structure = compound.get_centroid()
+    insert_concentration_for_structure(database, value, model, centroid_structure, replace_old, label)
+
+
+def insert_concentration_for_structure(
+        database: db.Manager,
+        value: float,
+        model: db.Model,
+        structure_id: db.ID,
+        replace_old: bool = True,
+        label: str = "start_concentration"):
+    concentration_options = ["start_concentration", "max_concentration", "final_concentration", "concentration_flux",
+                             "manual_activation"]
+    if label not in concentration_options and "_concentration_flux" not in label:
+        warn(f"Your concentration label is not within the suggested labels {str(concentration_options)}."
+             f"This may lead to problems recognizing the concentrations in the individual gears!")
 
     properties = database.get_collection("properties")
-    compounds = database.get_collection("compounds")
+    structures = database.get_collection("structures")
 
-    compound = db.Compound(compound_id, compounds)
-    centroid_structure = compound.get_centroid(database)
+    structure = db.Structure(structure_id, structures)
 
-    if centroid_structure.has_property(label) and replace_old:
-        concentration_prop = db.NumberProperty(centroid_structure.get_properties(label)[-1], properties)
+    if structure.has_property(label) and replace_old:
+        concentration_prop = db.NumberProperty(structure.get_properties(label)[-1], properties)
         concentration_prop.set_data(value)
         return
 
     concentration_prop = db.NumberProperty.make(label, model, value, properties)
-    concentration_prop.set_structure(centroid_structure.id())
-    centroid_structure.add_property(label, concentration_prop.id())
+    concentration_prop.set_structure(structure.id())
+    structure.add_property(label, concentration_prop.id())
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/utilities/insert_initial_structure.py` & `scine_chemoton-3.0.0/scine_chemoton/utilities/insert_initial_structure.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
-from typing import Union
+from typing import Union, Optional
 import warnings
 
 import scine_database as db
 import scine_utilities as utils
 
+from .insert_concentration import insert_concentration_for_structure
+
 
 def insert_initial_structure(
     database: db.Manager,
     molecule_path: Union[str, utils.AtomCollection],
     charge: int,
     multiplicity: int,
     model: db.Model,
     label: db.Label = db.Label.USER_GUESS,
     job: db.Job = db.Job("scine_geometry_optimization"),
     settings: utils.ValueCollection = utils.ValueCollection({}),
+    start_concentration: Optional[float] = None
 ):
     """
     Insert a structure to the database and set up a calculation working on it.
 
     Parameters
     ----------
     database :: db.Manager
@@ -39,14 +42,16 @@
         Model to be used for the calculation.
     label :: db.Label, optional
         Label of the inserted structure, by default db.Label.MINIMUM_GUESS.
     job :: db.Job, optional
         Job to be performed on the initial structure, by default db.Job('scine_geometry_optimization').
     settings :: utils.ValueCollection, optional
         Job settings, by default none.
+    start_concentration :: float
+        The start concentratoin of the compound that will be generated from this structure.
 
     Returns
     -------
     db.Structure, db.Calculation
         The inserted structure and the calculation generated for it
     """
     structures = database.get_collection("structures")
@@ -58,14 +63,17 @@
     if label != db.Label.USER_GUESS:
         warnings.warn(
             "WARNING: You specified a label for your structure input that is not 'user_guess'. This may "
             "hinder the exploration of this structure."
         )
     structure.set_label(label)
 
+    if start_concentration is not None:
+        insert_concentration_for_structure(database, start_concentration, model, structure.id())
+
     calculation = db.Calculation()
     calculation.link(calculations)
     calculation.create(model, job, [structure.id()])
     calculation.set_priority(1)
 
     if settings:
         calculation.set_settings(settings)
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/utilities/masm.py` & `scine_chemoton-3.0.0/scine_chemoton/utilities/masm.py`

 * *Files identical despite different names*

### Comparing `scine_chemoton-2.2.0/scine_chemoton/utilities/queries.py` & `scine_chemoton-3.0.0/scine_chemoton/utilities/queries.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 __copyright__ = """ This code is licensed under the 3-clause BSD license.
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
 from collections import Counter
+from itertools import permutations
+from datetime import datetime
 from json import dumps
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union, Set
 
 # Third party imports
 import scine_database as db
 import scine_utilities as utils
 
 
 class stop_on_timeout:
@@ -106,17 +108,17 @@
     """
     Searches for a reaction with the same aggregates, forward and backward reactions
     are categorized as the same reaction.
 
     Parameters
     ----------
     lhs_aggregates :: List[db.ID]
-        The ids of the aggregates of the left hand side
+        The ids of the aggregates of the left-hand side
     rhs_aggregates :: List[db.ID]
-        The ids of the aggregates of the right hand side
+        The ids of the aggregates of the right-hand side
     lhs_types :: List[db.ID]
         The types of the LHS aggregates.
     rhs_types :: List[db.ID]
         The types of the RHS aggregates.
     reactions :: db.Collection (Scine::Database::Collection)
 
     Returns
@@ -173,34 +175,28 @@
     Setup query for 1) optimized structures linked to an aggregate and 2) transition states
     """
     selection = {
         "$or": [
             {"label": "ts_optimized"},
             {
                 "$and": [
-                    {
-                        "$or": [
-                            {"label": "minimum_optimized"},
-                            {"label": "user_optimized"},
-                            {"label": "complex_optimized"},
-                        ]
-                    },
+                    {'label': {'$in': ["minimum_optimized", "user_optimized", "complex_optimized"]}},
                     {"aggregate": {"$ne": ""}},
                     {"exploration_disabled": {"$ne": True}},
                 ]
             },
         ]
     }
     return selection
 
 
 def select_calculation_by_structures(job_order: str, structure_id_list: List[db.ID], model: db.Model) -> dict:
     """
     Sets up a query for calculations with a specific job order and model working
-    on all of the given structures irrespective of their ordering.
+    on all the given structures irrespective of their ordering.
 
     Parameters
     ----------
     job_order : str
         The job order of the calculations to consider.
     structure_id_list : List[db.ID]
         The list of structure ids of interest.
@@ -208,22 +204,35 @@
         The model the calculations shall use.
 
     Returns
     -------
     dict
         The selection query dictionary.
     """
-    struct_oids = [{"$oid": sid.string()} for sid in structure_id_list]
-    selection = {
-        "$and": [
-            {"job.order": job_order},
-            {"structures": {"$size": len(struct_oids), "$all": struct_oids}},
-            *model_query(model)
-        ]
-    }
+    c = Counter([x.string() for x in structure_id_list])
+    if not any([x > 1 for x in c.values()]):
+        # no duplicates, easier query
+        struct_oids = [{"$oid": sid.string()} for sid in structure_id_list]
+        selection = {
+            "$and": [
+                {"job.order": job_order},
+                {"structures": {"$size": len(struct_oids), "$all": struct_oids}},
+                *model_query(model)
+            ]
+        }
+    else:
+        # generate all permutations of structure_ids to be independent of ordering
+        all_struct_oids = [[{"$oid": sid.string()} for sid in p] for p in permutations(structure_id_list)]
+        selection = {
+            "$and": [
+                {"job.order": job_order},
+                {"structures": {"$in": all_struct_oids}},
+                *model_query(model)
+            ]
+        }
     return selection
 
 
 def calculation_exists_in_structure(job_order: str, structure_id_list: List[db.ID], model: db.Model,
                                     structures: db.Collection, calculations: db.Collection,
                                     settings: Optional[Dict[str, Any]] = None,
                                     auxiliaries: Optional[Dict[str, Any]] = None) -> bool:
@@ -252,29 +261,107 @@
     True, if such a calculation exists. False, otherwise.
 
     """
     return get_calculation_id_from_structure(job_order, structure_id_list, model, structures,
                                              calculations, settings, auxiliaries) is not None
 
 
+def calculation_exists_in_id_set(id_selection: Set[str], n_structures: int, calculations: db.Collection,
+                                 specific_structures: Optional[List[db.ID]] = None,
+                                 settings: Optional[Union[utils.ValueCollection, Dict[str, Any]]] = None,
+                                 auxiliaries: Optional[Dict[str, Any]] = None) -> bool:
+    return query_calculation_in_id_set(id_selection, n_structures, calculations, specific_structures,
+                                       settings, auxiliaries) is not None
+
+
+def query_calculation_in_id_set(id_selection: Set[str], n_structures: int, calculations: db.Collection,
+                                specific_structures: Optional[List[db.ID]] = None,
+                                settings: Optional[Union[utils.ValueCollection, Dict[str, Any]]] = None,
+                                auxiliaries: Optional[Dict[str, Any]] = None) -> Union[db.ID, None]:
+    """
+    Check if a calculation exists that corresponds to the given structures, mode, settings, etc.
+
+    Notes
+    -----
+    If specific_structures is not given, this can lead to false positives, use with caution and only with clear
+    structures cases like a transition state.
+
+    Parameters
+    ----------
+    id_selection : Set[str]
+        The set of calculation ids to consider.
+    n_structures : int
+        The number of structures the calculation should have.
+    calculations : db.Collection
+        The calculation collection.
+    specific_structures : Optional[List[db.ID]]
+        The specific structures the calculation should have.
+    settings : Optional[Union[utils.ValueCollection, Dict[str, Any]]]
+        The settings of the calculation.
+    auxiliaries : Optional[Dict[str, Any]]
+        The auxiliaries of the calculation.
+
+    Returns
+    -------
+    The id of the calculation if it exists, None otherwise.
+    """
+    if specific_structures is not None and len(specific_structures) != n_structures:
+        raise ValueError(f"Number of specific structures ({len(specific_structures)}) does not match "
+                         f"number of structures ({n_structures})")
+    if len(id_selection) < 1:
+        return None
+    compare_settings = None
+    if settings is not None:
+        if isinstance(settings, utils.ValueCollection):
+            compare_settings = settings
+        elif isinstance(settings, dict):
+            compare_settings = utils.ValueCollection(settings)
+        else:
+            raise TypeError(f"Gave incompatible type '{type(settings)}' to 'get_calculation_id_from_structure'")
+
+    calc_id_str = [{"$oid": str_id} for str_id in id_selection]
+    selection = {
+        "$and": [
+            {"_id": {"$in": calc_id_str}},
+            {"structures": {"$size": n_structures}}
+        ]
+    }
+    sorted_specific_structures = None
+    if specific_structures is not None:
+        sorted_specific_structures = sorted([str(i) for i in specific_structures])
+    for calculation in stop_on_timeout(calculations.iterate_calculations(dumps(selection))):
+        calculation.link(calculations)
+        if sorted_specific_structures is not None:
+            if sorted_specific_structures != sorted([str(i) for i in calculation.get_structures()]):
+                continue
+        if compare_settings is not None:
+            if compare_settings != calculation.get_settings():
+                continue
+        if auxiliaries is not None:
+            if auxiliaries != calculation.get_auxiliaries():
+                continue
+        return calculation.id()
+    return None
+
+
 def get_calculation_id_from_structure(job_order: str, structure_id_list: List[db.ID], model: db.Model,
                                       structures: db.Collection, calculations: db.Collection,
                                       settings: Optional[Union[utils.ValueCollection, Dict[str, Any]]] = None,
                                       auxiliaries: Optional[Dict[str, Any]] = None) -> Union[db.ID, None]:
     """
     Search for a calculation corresponding to the given settings. If the calculation is found, its ID is returned.
 
     Parameters
     ----------
     job_order : str
         The job order of the calculations to consider.
     structure_id_list : List[db.ID]
         The list of structure ids of interest.
     model : db.Model
-        The model the calculations shall use.
+        The model, the calculations shall use.
     structures : db.Collection
         The structure collection.
     calculations : db.Collection
         The calculation collection.
     settings : dict (optional)
         The settings of the calculation.
     auxiliaries : dict (optional)
@@ -283,62 +370,58 @@
     Returns
     -------
     Returns the calculation ID if found. Returns None if no calculation corresponds to the given specification.
 
     """
     if len(structure_id_list) < 1:
         return None
+    # Eliminate duplicate structure ids.
+    s_id_list = [db.ID(str_id) for str_id in set([s_id.string() for s_id in structure_id_list])]
     # settings type check, support both dict and ValueCollection and want ValueCollection for speed
-    compare_settings = None
-    if settings is not None:
-        if isinstance(settings, utils.ValueCollection):
-            compare_settings = settings
-        elif isinstance(settings, dict):
-            compare_settings = utils.ValueCollection(settings)
-        else:
-            raise TypeError(f"Gave incompatible type '{type(settings)}' to 'get_calculation_id_from_structure'")
-    structure_0 = db.Structure(structure_id_list[0], structures)
+    structure_0 = db.Structure(s_id_list[0], structures)
     calc_id_set = set([c_id.string() for c_id in structure_0.query_calculations(job_order, model, calculations)])
     if not calc_id_set:
         return None
-    for s_id in structure_id_list:
+    for counter in range(len(s_id_list) - 1):
+        s_id = s_id_list[counter + 1]
         structure = db.Structure(s_id, structures)
         struc_set = set([c_id.string() for c_id in structure.query_calculations(job_order, model, calculations)])
         calc_id_set = calc_id_set.intersection(struc_set)
-    calc_id_str = [{"$oid": str_id} for str_id in calc_id_set]
-    selection = {
-        "$and": [{"_id": {"$in": calc_id_str}}]
-    }
-    for calculation in stop_on_timeout(calculations.iterate_calculations(dumps(selection))):
-        calculation.link(calculations)
-        structures_in_calc_ids = calculation.get_structures()
-        if len(structure_id_list) != len(structures_in_calc_ids):
-            continue
-        # Check structure ids
-        matching_structures = True
-        for s_id in structures_in_calc_ids:
-            if s_id not in structure_id_list:
-                matching_structures = False
-                break
-        if not matching_structures:
-            continue
-        if compare_settings is not None:
-            if compare_settings != calculation.get_settings():
-                continue
-        if auxiliaries is not None:
-            if auxiliaries != calculation.get_auxiliaries():
-                continue
-        return calculation.id()
-    return None
+
+    return query_calculation_in_id_set(calc_id_set, len(structure_id_list), calculations, structure_id_list,
+                                       settings, auxiliaries)
 
 
 def get_calculation_id(job_order: str, structure_id_list: List[db.ID], model: db.Model,
                        calculations: db.Collection,
                        settings: Optional[Union[utils.ValueCollection, Dict[str, Any]]] = None,
                        auxiliaries: Optional[Dict[str, Any]] = None) -> Union[db.ID, None]:
+    """
+    Search for a calculation corresponding to the given settings. If the calculation is found, its ID is returned.
+
+    Parameters
+    ----------
+    job_order : str
+        The job order of the calculations to consider.
+    structure_id_list : List[db.ID]
+        The list of structure ids of interest.
+    model : db.Model
+        The model, the calculations shall use.
+    calculations : db.Collection
+        The calculation collection.
+    settings : dict (optional)
+        The settings of the calculation.
+    auxiliaries : dict (optional)
+        The auxiliaries of the calculation.
+
+    Returns
+    -------
+    Returns the calculation ID if found. Returns None if no calculation corresponds to the given specification.
+
+    """
     if len(structure_id_list) < 1:
         return None
     selection = select_calculation_by_structures(job_order, structure_id_list, model)
     # simple case of no required loop comparisons
     if settings is None and auxiliaries is None:
         hit = calculations.get_one_calculation(dumps(selection))
         if hit is not None:
@@ -360,7 +443,11 @@
             if compare_settings != calculation.get_settings():
                 continue
         if auxiliaries is not None:
             if auxiliaries != calculation.get_auxiliaries():
                 continue
         return calculation.id()
     return None
+
+
+def lastmodified_since(time: datetime) -> Dict[str, Any]:
+    return {'_lastmodified': {'$gt': {"$date": int(time.timestamp() * 1000)}}}
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/__main__.py` & `scine_chemoton-3.0.0/scine_chemoton/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,23 +4,27 @@
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 # Standard library imports
 import os
 import pkg_resources
-import time
+import psutil
 import sys
+import signal
+import time
+from typing import List
 
 # Third party imports
 import scine_database as db
 import scine_utilities as utils
 
 # Local application imports
 from scine_chemoton.utilities.insert_initial_structure import insert_initial_structure
+from scine_chemoton.default_settings import default_nt_settings
 from scine_chemoton.engine import Engine
 from scine_chemoton.gears.scheduler import Scheduler
 from scine_chemoton.gears.thermo import BasicThermoDataCompletion
 from scine_chemoton.gears.compound import BasicAggregateHousekeeping
 from scine_chemoton.gears.reaction import BasicReactionHousekeeping
 from scine_chemoton.gears.refinement import NetworkRefinement
 from scine_chemoton.gears.kinetics import (
@@ -30,16 +34,18 @@
 from scine_chemoton.gears.conformers.brute_force import BruteForceConformers
 from scine_chemoton.gears.elementary_steps.minimal import MinimalElementarySteps
 from scine_chemoton.gears.elementary_steps.trial_generator.bond_based import BondBased
 from scine_chemoton.gears.elementary_steps.trial_generator.fast_dissociations import (
     FastDissociations,
     FurtherExplorationFilter
 )
-from scine_chemoton.gears.elementary_steps.compound_filters import CompoundFilter
+from scine_chemoton.gears.elementary_steps.aggregate_filters import AggregateFilter
 from scine_chemoton.gears.elementary_steps.reactive_site_filters import ReactiveSiteFilter
+from scine_chemoton.utilities import yes_or_no_question
+
 
 # Prepare clean database
 manager = db.Manager()
 db_name = "default"
 ip = os.environ.get('TEST_MONGO_DB_IP', '127.0.0.1')
 port = os.environ.get('TEST_MONGO_DB_PORT', '27017')
 credentials = db.Credentials(ip, int(port), db_name)
@@ -53,27 +59,19 @@
 # model = db.Model("gfn2", "gfn2", "")
 # model = db.Model('dft', 'wb97x_v', 'def2-svp')
 # model = db.Model('dft', 'pbe-d3bj', 'def2-svp')
 model.spin_mode = "unrestricted"
 model.program = "sparrow"
 
 wipe = True
-if len(sys.argv) > 1:
-    if sys.argv[1].upper() == "CONTINUE":
-        wipe = False
+if len(sys.argv) > 1 and sys.argv[1].upper() == "CONTINUE":
+    wipe = False
 
 if wipe:
-    inp = input("Are you sure you want to wipe the database '" + db_name + "'? (y/n): ")
-    while True:
-        if inp.strip().lower() in ["y", "yes"]:
-            break
-        if inp.strip().lower() in ["n", "no"]:
-            wipe = False
-            break
-        inp = input("Did not recognize answer, please answer 'y', if '" + db_name + "' should be wiped: ")
+    wipe = yes_or_no_question(f"Are you sure you want to wipe the database '{db_name}'")
 
 if wipe:
     manager.wipe()
     manager.init()
     time.sleep(1.0)
     # Load initial data
     methanol = pkg_resources.resource_filename("scine_chemoton", "tests/resources/methanol.xyz")
@@ -102,18 +100,36 @@
             {
                 "convergence_max_iterations": 1000,
                 "bfgs_use_trust_radius": True,
             }
         ),
     )
 
+
+# check for existing chemoton process as a sanity check
+# Iterate over all running process
+for proc in psutil.process_iter():
+    try:
+        name = proc.name()
+        process_id = proc.pid
+        if "Chemoton" in name:
+            continue_explore = yes_or_no_question(f"Detected a running Chemoton process '{name}' "
+                                                  f"with id {process_id}. Do you want to continue")
+            if not continue_explore:
+                sys.exit(1)
+    except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
+        pass
+
+
 # ================= #
 #   Start engines   #
 # ================= #
 
+engine_list: List[Engine] = []
+
 # 1) Conformer Engine
 conformer_gear = BruteForceConformers()
 conformer_gear.options.model = model
 conformer_gear.options.conformer_job = db.Job("conformers")
 conformer_gear.options.minimization_job = db.Job("scine_geometry_optimization")
 conformer_gear.options.minimization_settings = utils.ValueCollection(
     {
@@ -121,181 +137,133 @@
         "bfgs_use_trust_radius": True,
         "geoopt_coordinate_system": "cartesianWithoutRotTrans",
     }
 )
 conformer_engine = Engine(credentials)
 conformer_engine.set_gear(conformer_gear)
 conformer_engine.run()
+engine_list.append(conformer_engine)
 
 # 2) Compound generation and sorting
 compound_gear = BasicAggregateHousekeeping()
 compound_gear.options.model = model
 compound_engine = Engine(credentials)
 compound_engine.set_gear(compound_gear)
 compound_engine.run()
+engine_list.append(compound_engine)
 
 # 3) Thermo-chemical data completion
 thermo_gear = BasicThermoDataCompletion()
 thermo_gear.options.model = model
 thermo_gear.options.job = db.Job("scine_hessian")
 thermo_engine = Engine(credentials)
 thermo_engine.set_gear(thermo_gear)
 thermo_engine.run()
+engine_list.append(thermo_engine)
 
 # 4) Reaction Exploration
 #  Set the settings for the elementary step exploration.
 #  These are the main settings for the general exploration
 # 4.1) Starting with the settings for the elementary step trial calculation (here an NT2 calculation)
 nt_job = db.Job("scine_react_complex_nt2")
-nt_settings = utils.ValueCollection(
-    {
-        # # # Settings for the nt task
-        "nt_convergence_max_iterations": 600,
-        "nt_nt_total_force_norm": 0.1,
-        "nt_sd_factor": 1.0,
-        "nt_nt_use_micro_cycles": True,
-        "nt_nt_fixed_number_of_micro_cycles": True,
-        "nt_nt_number_of_micro_cycles": 10,
-        "nt_nt_filter_passes": 10,
-        # # # Settings for the tsopt task
-        "tsopt_convergence_max_iterations": 1000,
-        "tsopt_convergence_step_max_coefficient": 2.0e-3,
-        "tsopt_convergence_step_rms": 1.0e-3,
-        "tsopt_convergence_gradient_max_coefficient": 2.0e-4,
-        "tsopt_convergence_gradient_rms": 1.0e-4,
-        "tsopt_convergence_requirement": 3,
-        "tsopt_convergence_delta_value": 1e-6,
-        "tsopt_optimizer": "bofill",
-        "tsopt_geoopt_coordinate_system": "cartesianWithoutRotTrans",
-        "tsopt_bofill_trust_radius": 0.2,
-        # 'tsopt_bofill_follow_mode': 0, # uncomment to disable automatic mode selection
-        # 'tsopt_dimer_calculate_hessian_once': True, # enable when using dimer
-        # 'tsopt_dimer_trust_radius': 0.1, # enable when using dimer
-        # # # Settings for the irc task
-        "irc_convergence_max_iterations": 100,
-        "irc_sd_factor": 2.0,
-        "irc_irc_initial_step_size": 0.3,
-        "irc_stop_on_error": False,
-        "irc_convergence_step_max_coefficient": 2.0e-3,
-        "irc_convergence_step_rms": 1.0e-3,
-        "irc_convergence_gradient_max_coefficient": 2.0e-4,
-        "irc_convergence_gradient_rms": 1.0e-4,
-        "irc_convergence_delta_value": 1.0e-6,
-        "irc_irc_coordinate_system": "cartesianWithoutRotTrans",
-        # # # Settings for the optimisation after the irc on combined product
-        "ircopt_convergence_max_iterations": 1000,
-        "ircopt_convergence_step_max_coefficient": 2.0e-3,
-        "ircopt_convergence_step_rms": 1.0e-3,
-        "ircopt_convergence_gradient_max_coefficient": 2.0e-4,
-        "ircopt_convergence_gradient_rms": 1.0e-4,
-        "ircopt_convergence_requirement": 3,
-        "ircopt_convergence_delta_value": 1e-6,
-        "ircopt_geoopt_coordinate_system": "cartesianWithoutRotTrans",
-        "ircopt_bfgs_use_trust_radius": True,
-        "ircopt_bfgs_trust_radius": 0.2,
-        # # # Settings for the optimisation after irc
-        "opt_convergence_max_iterations": 1000,
-        "opt_convergence_step_max_coefficient": 2.0e-3,
-        "opt_convergence_step_rms": 1.0e-3,
-        "opt_convergence_gradient_max_coefficient": 2.0e-4,
-        "opt_convergence_gradient_rms": 1.0e-4,
-        "opt_convergence_requirement": 3,
-        "opt_convergence_delta_value": 1e-6,
-        "opt_geoopt_coordinate_system": "cartesianWithoutRotTrans",
-        "opt_bfgs_use_trust_radius": True,
-        "opt_bfgs_trust_radius": 0.4,
-    }
-)
+nt_settings = default_nt_settings()
+
 # 4.2) Choose the reaction types to be probed
 dissociations_gear = MinimalElementarySteps()
+dissociations_gear.aggregate_filter = AggregateFilter()
 dissociations_gear.options.enable_unimolecular_trials = True
 dissociations_gear.options.enable_bimolecular_trials = False
 dissociations_gear.trial_generator = FastDissociations()
-dissociations_gear.trial_generator.options.model = model
-dissociations_gear.compound_filter = CompoundFilter()
 dissociations_gear.trial_generator.reactive_site_filter = ReactiveSiteFilter()
-dissociations_gear.trial_generator.options.cutting_job = db.Job("scine_dissociation_cut")
+dissociations_gear.trial_generator.further_exploration_filter = FurtherExplorationFilter()
+dissociations_gear.trial_generator.options.model = model
+dissociations_gear.trial_generator.options.job = db.Job("scine_dissociation_cut")
 dissociations_gear.trial_generator.options.cutting_job_settings = utils.ValueCollection({})
 dissociations_gear.trial_generator.options.min_bond_dissociations = 1
 dissociations_gear.trial_generator.options.max_bond_dissociations = 1
 dissociations_gear.trial_generator.options.enable_further_explorations = False
 dissociations_gear.trial_generator.options.always_further_explore_dissociative_reactions = True
-dissociations_gear.trial_generator.options.further_exploration_filter = FurtherExplorationFilter()
 dissociations_gear.trial_generator.options.further_job = nt_job
 dissociations_gear.trial_generator.options.further_job_settings = nt_settings
 dissociations_engine = Engine(credentials)
 dissociations_engine.set_gear(dissociations_gear)
 dissociations_engine.run()
+engine_list.append(dissociations_engine)
 
 elementary_step_gear = MinimalElementarySteps()
 elementary_step_gear.trial_generator = BondBased()
 elementary_step_gear.trial_generator.options.model = model
 elementary_step_gear.options.enable_bimolecular_trials = True
 elementary_step_gear.options.enable_unimolecular_trials = True
 # 4.2.1) Minimalistic settings for bimolecular trial reaction coordinates and reactive complex generation
 #        Set-up one trial reaction coordinate consting only of one intermolecular bond formation per trial calculation
 #        NOTE: The number of trial calculations scales steeply with the modification numbers chosen here.
 #              See elementary_step_gear.trial_generator.estimate_n_bimolecular_trials(...) to get an estimate of
 #              how many trials are to be expected from your options for given structures
 #              without enumerating them explicitly.
 #        NOTE: The modification numbers only specify which kind of changes are included in the trial reaction
 #              coordinates. This does not imply that the eventually resulting elementary steps include the same changes.
-elementary_step_gear.trial_generator.options.bimolecular.min_bond_modifications = 1
-elementary_step_gear.trial_generator.options.bimolecular.max_bond_modifications = 1
-elementary_step_gear.trial_generator.options.bimolecular.min_inter_bond_formations = 1
-elementary_step_gear.trial_generator.options.bimolecular.max_inter_bond_formations = 1
-elementary_step_gear.trial_generator.options.bimolecular.min_intra_bond_formations = 0
-elementary_step_gear.trial_generator.options.bimolecular.max_intra_bond_formations = 0
-elementary_step_gear.trial_generator.options.bimolecular.min_bond_dissociations = 0
-elementary_step_gear.trial_generator.options.bimolecular.max_bond_dissociations = 0
-elementary_step_gear.trial_generator.options.bimolecular.complex_generator.options.number_rotamers = 1
-elementary_step_gear.trial_generator.options.bimolecular.complex_generator.options.number_rotamers_two_on_two = 1
-elementary_step_gear.trial_generator.options.bimolecular.complex_generator.options.multiple_attack_points = False
+elementary_step_gear.trial_generator.options.bimolecular_options.min_bond_modifications = 1
+elementary_step_gear.trial_generator.options.bimolecular_options.max_bond_modifications = 1
+elementary_step_gear.trial_generator.options.bimolecular_options.min_inter_bond_formations = 1
+elementary_step_gear.trial_generator.options.bimolecular_options.max_inter_bond_formations = 1
+elementary_step_gear.trial_generator.options.bimolecular_options.min_intra_bond_formations = 0
+elementary_step_gear.trial_generator.options.bimolecular_options.max_intra_bond_formations = 0
+elementary_step_gear.trial_generator.options.bimolecular_options.min_bond_dissociations = 0
+elementary_step_gear.trial_generator.options.bimolecular_options.max_bond_dissociations = 0
+elementary_step_gear.trial_generator.options.bimolecular_options.\
+    complex_generator.options.number_rotamers = 1
+elementary_step_gear.trial_generator.options.bimolecular_options.\
+    complex_generator.options.number_rotamers_two_on_two = 1
+elementary_step_gear.trial_generator.options.bimolecular_options.\
+    complex_generator.options.multiple_attack_points = False
 # 4.2.2) Minimalistic settings for unimolecular additions
 #        Set-up trial reaction coordinates consisting of either one bond formation or one bond dissociation per trial
 #        calculation
 #        NOTE: The number of trial calculations scales steeply with the modification numbers chosen here.
 #              See elementary_step_gear.trial_generator.estimate_n_unimolecular_trials(...) to get an estimate of
 #              how many trials are to be expected from your options for a given structure,
 #              without enumerating them explicitly.
 #        NOTE: The modification numbers only specify which kind of changes are included in the trial reaction
 #              coordinates. This does not imply that the eventually resulting elementary steps include the same changes.
-elementary_step_gear.trial_generator.options.unimolecular.min_bond_modifications = 1
-elementary_step_gear.trial_generator.options.unimolecular.max_bond_modifications = 1
-elementary_step_gear.trial_generator.options.unimolecular.min_bond_formations = 0
-elementary_step_gear.trial_generator.options.unimolecular.max_bond_formations = 1
-elementary_step_gear.trial_generator.options.unimolecular.min_bond_dissociations = 0
-elementary_step_gear.trial_generator.options.unimolecular.max_bond_dissociations = 0
+elementary_step_gear.trial_generator.options.unimolecular_options.min_bond_modifications = 1
+elementary_step_gear.trial_generator.options.unimolecular_options.max_bond_modifications = 1
+elementary_step_gear.trial_generator.options.unimolecular_options.min_bond_formations = 0
+elementary_step_gear.trial_generator.options.unimolecular_options.max_bond_formations = 1
+elementary_step_gear.trial_generator.options.unimolecular_options.min_bond_dissociations = 0
+elementary_step_gear.trial_generator.options.unimolecular_options.max_bond_dissociations = 0
 # 4.3) Apply the basic calculation settings to all different reactions types in the gear
 #      Note: These settings could be different for different reaction types, resulting in better performance.
-elementary_step_gear.trial_generator.options.bimolecular.job = nt_job
-elementary_step_gear.trial_generator.options.bimolecular.job_settings = nt_settings
-elementary_step_gear.trial_generator.options.bimolecular.minimal_spin_multiplicity = False
-elementary_step_gear.trial_generator.options.unimolecular.job = nt_job
+elementary_step_gear.trial_generator.options.bimolecular_options.job = nt_job
+elementary_step_gear.trial_generator.options.bimolecular_options.job_settings = nt_settings
+elementary_step_gear.trial_generator.options.bimolecular_options.minimal_spin_multiplicity = False
+elementary_step_gear.trial_generator.options.unimolecular_options.job = nt_job
 #      Associative job settings are applied when at least one bond formation is included in the trial coordinate
-elementary_step_gear.trial_generator.options.unimolecular.job_settings_associative = nt_settings
+elementary_step_gear.trial_generator.options.unimolecular_options.job_settings_associative = nt_settings
 #      Disconnective job settings are applied when there are no associative components in the trial coordinate and it
 #      would result in splitting the reactant into two or more molecules
-elementary_step_gear.trial_generator.options.unimolecular.job_settings_disconnective = nt_settings
+elementary_step_gear.trial_generator.options.unimolecular_options.job_settings_disconnective = nt_settings
 #      Dissociative job settings are applied when there are no associative components in the trial coordinate but it
 #      would not result in splitting the reactant into two or more molecules
-elementary_step_gear.trial_generator.options.unimolecular.job_settings_dissociative = nt_settings
+elementary_step_gear.trial_generator.options.unimolecular_options.job_settings_dissociative = nt_settings
 # 4.4) Add filters (default ones, filter nothing)
 elementary_step_gear.trial_generator.reactive_site_filter = ReactiveSiteFilter()
-elementary_step_gear.compound_filter = CompoundFilter()
+elementary_step_gear.aggregate_filter = AggregateFilter()
 # Run
 elementary_step_engine = Engine(credentials)
 elementary_step_engine.set_gear(elementary_step_gear)
 elementary_step_engine.run()
+engine_list.append(elementary_step_engine)
 
 # Sorting elementary steps into reactions
 reaction_gear = BasicReactionHousekeeping()
 reaction_engine = Engine(credentials)
 reaction_engine.set_gear(reaction_gear)
 reaction_engine.run()
+engine_list.append(reaction_engine)
 
 # Improve the network with a better model or find more connections with additional double ended searches
 refinement_gear = NetworkRefinement()
 refinement_engine = Engine(credentials)
 refinement_gear.options.refinements = {
     "refine_single_points": False,  # SP for all minima and TS
     "refine_optimizations": False,   # optimize all minima and TS (+ validation)
@@ -306,27 +274,29 @@
 }
 pre_refinement_model = db.Model("PM6", "PM6", "")
 post_refinement_model = db.Model("DFT", "", "")
 refinement_gear.options.pre_refine_model = pre_refinement_model
 refinement_gear.options.post_refine_model = post_refinement_model
 refinement_engine.set_gear(refinement_gear)
 refinement_engine.run()
+engine_list.append(refinement_engine)
 
 # Driving exploration based on kinetics
 kinetics_gear = MinimalConnectivityKinetics()  # activate all compounds
 """
 kinetics_gear = BasicBarrierHeightKinetics()  # activate compound if accessible via reaction with low enough barrier
 kinetics_gear.options.restart = True
 kinetics_gear.options.model = model  # model from which you want to take the energies from
 kinetics_gear.options.max_allowed_barrier = 1000.0  # kJ/mol
 kinetics_gear.options.enforce_free_energies = False  # only consider free energies for barrier height
 """
 kinetics_engine = Engine(credentials)
 kinetics_engine.set_gear(kinetics_gear)
 kinetics_engine.run()
+engine_list.append(kinetics_engine)
 
 # Calculation scheduling
 scheduling_gear = Scheduler()
 scheduling_gear.options.job_counts = {
     "scine_single_point": 500,
     "scine_geometry_optimization": 500,
     "scine_ts_optimization": 500,
@@ -334,10 +304,27 @@
     "scine_hessian": 200,
     "scine_react_complex_nt2": 100,
     "scine_dissociation_cut": 100,
     "conformers": 20,
     "final_conformer_deduplication": 20,
     "graph": 1000,
 }
-scheduling_engine = Engine(credentials, fork=False)
+scheduling_engine = Engine(credentials)
 scheduling_engine.set_gear(scheduling_gear)
 scheduling_engine.run()
+engine_list.append(scheduling_engine)
+
+
+def handler(*_):
+    for engine in engine_list:
+        engine.stop()
+    for engine in engine_list:
+        engine.join()
+    exit(1)
+
+
+# Add more signals if needed
+signal.signal(signal.SIGINT, handler)
+signal.signal(signal.SIGTERM, handler)
+
+while True:
+    time.sleep(1.0)
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton/engine.py` & `scine_chemoton-3.0.0/scine_chemoton/engine.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 Copyright ETH Zurich, Laboratory of Physical Chemistry, Reiher Group.
 See LICENSE.txt for details.
 """
 
 
 # Standard library imports
 import multiprocessing
-from typing import Optional
+from typing import Any, Optional
+import signal
+import os
 
 # Third party imports
 import scine_database as db
 
 # Local application imports
 from .gears import Gear
 
@@ -37,14 +39,15 @@
     """
 
     def __init__(self, credentials: db.Credentials, fork: bool = True):
         self._credentials = credentials
         self._fork = fork
         self._gear: Optional[Gear] = None
         self._proc: Optional[multiprocessing.Process] = None
+        self._loop_count: Optional[Any] = multiprocessing.Value('i', 0)
 
     def set_gear(self, gear: Gear):
         """
         Parameters
         ----------
         gear :: Gear (scine_chemoton.gears.Gears)
             The gear to be used when starting this engine.
@@ -64,25 +67,61 @@
         Raises
         ------
         AttributeError
             If no gear was added to the engine, prior to starting it.
         """
         if not self._gear:
             raise AttributeError
+        if self._loop_count is None:
+            self._loop_count = multiprocessing.Value('i', 0)
         if self._fork and self._gear is not None:
             self._proc = multiprocessing.Process(
-                target=self._gear, args=(self._credentials,), kwargs={"single": single}
+                target=self._gear, args=(self._credentials, self._loop_count), kwargs={"single": single}
             )
             self._proc.start()
         elif self._gear is not None:
-            self._gear(self._credentials, single=single)
+            self._gear(self._credentials, self._loop_count, single=single)  # type: ignore
 
     def stop(self):
         """
+        In case of a forked job this will send an interrupt signal to the forked process, leading to a graceful exit.
+        """
+        if self._fork and self._proc:
+            self._gear.stop()
+            pid = self._proc.pid
+            if pid is not None:
+                os.kill(pid, signal.SIGINT)
+
+    def join(self, timeout: Optional[int] = None):
+        """
+        In case of a forked job this will wait for the graceful exit of the job.
+        If the process has not been signalled to stop, this will also initiate the stop.
+        """
+        if self._fork and self._proc:
+            if self._gear is not None and not self._gear.stop_at_next_break_point:
+                self.stop()
+        self._cleanup(timeout)
+
+    def terminate(self):
+        """
         In case of a forked job this will terminate the forked process.
 
         Notes
         -----
         The job will **NOT** be stopped gracefully.
         """
         if self._fork and self._proc:
             self._proc.terminate()
+        self._cleanup()
+
+    def _cleanup(self, timeout: Optional[int] = None):
+        if self._proc is not None:
+            self._proc.join(timeout)
+            self._proc = None
+        self._loop_count = None
+
+    def get_number_of_gear_loops(self) -> int:
+        if self._gear is None:
+            raise AttributeError("Engine has not received a gear")
+        if self._loop_count is None:
+            return 0
+        return self._loop_count.value  # type: ignore
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton.egg-info/PKG-INFO` & `scine_chemoton-3.0.0/scine_chemoton.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scine-chemoton
-Version: 2.2.0
+Version: 3.0.0
 Summary: Software driving the automated exploration of chemical reaction networks
 Home-page: https://www.scine.ethz.ch
 Author: ETH Zurich, Laboratory of Physical Chemistry, Reiher Group
 Author-email: scine@phys.chem.ethz.ch
 License: BSD (3-clause)
 Description: .. image:: docs/source/res/chemoton_header.png
            :alt: SCINE Chemoton
@@ -31,25 +31,27 @@
         
         Prerequisites
         .............
         
         The key requirements for Chemoton are the Python packages ``scine_utilities``,
         ``scine_database``, and ``scine_molassember``. These packages are available from
         PyPI and can be installed using ``pip``.
-        However, these packages can also be compiled by hand. For the latter case please
-        visit the repositories of each of the packages and follow their guidelines.
+        However, these packages can also be compiled from sources. For the latter case please
+        visit the repositories of each of the packages and follow their guidelines or
+        bootstrap a `puffin <https://github.com/qcscine/puffin>`_ which will install the same
+        dependencies.
         
         Installation
         ............
         
         Chemoton can be installed using ``pip`` (``pip3``) once the repository has been cloned:
         
         .. code-block:: bash
         
-           git clone <chemoton-repo> chemoton
+           git clone https://github.com/qcscine/chemoton.git
            cd chemoton
            pip install -r requirements.txt
            pip install .
         
         A non-root user can install the package using a virtual environment, or
         the ``--user`` flag.
         
@@ -94,35 +96,36 @@
         
            mongod --fork --port=27017 -dbpath=<path to db storage dir> -wiredTigerCacheSizeGB=1 --logpath=mongo.log
         
         2. Configure and bootstrap a ``puffin``:
         
         .. code-block:: bash
         
-           python3 -m puffin configure
+           pip install scine-puffin
+           python3 -m scine_puffin configure
            # Edit the generated puffin.yaml here
-           python3 -m puffin -c puffin.yaml bootstrap
+           python3 -m scine_puffin -c puffin.yaml bootstrap
         
         3. Source the ``puffin`` settings and tell it to listen to the correct DB.
         (Hostname and port should be the default ones.) Then start it.
         
         .. code-block:: bash
         
            source puffin.sh
            export PUFFIN_DATABASE_NAME=default
-           python3 -m puffin -c puffin.yaml start
+           python3 -m scine_puffin -c puffin.yaml start
         
         4. Run the Chemoton exploration defined in the ``__main__`` function:
         
         .. code-block:: bash
         
            python3 -m scine_chemoton wipe
         
         The optional ``wipe`` argument will start the example exploration with a clean
-        ``puffin_tests`` DB; giving the ``continue`` argument will reuse old data.
+        ``default`` DB; giving the ``continue`` argument will reuse old data.
         
         Expanding on the Minimal Example
         ................................
         
         The functionalities used in Chemoton's ``__main__.py`` are a good starting point
         for most simple explorations. The file contains a lot of settings that are
         explicitly set to their defaults in order to show their existence.
@@ -144,15 +147,15 @@
         release as archived on `Zenodo <https://doi.org/10.5281/zenodo.6695583>`_ (DOI
         10.5281/zenodo.6695583; please use the DOI of the respective release).
         
         In addition, we kindly request you to cite the following article when using Chemoton:
         
         J. P. Unsleber, S. A. Grimmel, M. Reiher,
         "Chemoton 2.0: Autonomous Exploration of Chemical Reaction Networks",
-        *arXiv:2202.13011 [physics.chem-ph].*
+        *J. Chem. Theory Comput.*, **2022**, *18*, 5393.
         
         Support and Contact
         -------------------
         
         In case you should encounter problems or bugs, please write a short message
         to scine@phys.chem.ethz.ch.
```

### Comparing `scine_chemoton-2.2.0/scine_chemoton.egg-info/SOURCES.txt` & `scine_chemoton-3.0.0/scine_chemoton.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,88 +17,92 @@
 docs/source/api/api.rst
 docs/source/api/engine.rst
 docs/source/api/gears.rst
 docs/source/api/utilities.rst
 scine_chemoton/__init__.py
 scine_chemoton/__main__.py
 scine_chemoton/_version.py
+scine_chemoton/default_settings.py
 scine_chemoton/engine.py
 scine_chemoton.egg-info/PKG-INFO
 scine_chemoton.egg-info/SOURCES.txt
 scine_chemoton.egg-info/dependency_links.txt
 scine_chemoton.egg-info/entry_points.txt
 scine_chemoton.egg-info/not-zip-safe
 scine_chemoton.egg-info/requires.txt
 scine_chemoton.egg-info/top_level.txt
 scine_chemoton/gears/__init__.py
 scine_chemoton/gears/compound.py
 scine_chemoton/gears/kinetics.py
 scine_chemoton/gears/pathfinder.py
 scine_chemoton/gears/reaction.py
 scine_chemoton/gears/refinement.py
+scine_chemoton/gears/rerun_calculations.py
 scine_chemoton/gears/scheduler.py
 scine_chemoton/gears/thermo.py
 scine_chemoton/gears/conformers/__init__.py
 scine_chemoton/gears/conformers/brute_force.py
 scine_chemoton/gears/elementary_steps/__init__.py
+scine_chemoton/gears/elementary_steps/aggregate_filters.py
 scine_chemoton/gears/elementary_steps/brute_force.py
-scine_chemoton/gears/elementary_steps/compound_filters.py
 scine_chemoton/gears/elementary_steps/minimal.py
-scine_chemoton/gears/elementary_steps/minimum_energy_confomer.py
+scine_chemoton/gears/elementary_steps/minimum_energy_conformer.py
 scine_chemoton/gears/elementary_steps/reactive_site_filters.py
+scine_chemoton/gears/elementary_steps/reaction_rules/__init__.py
+scine_chemoton/gears/elementary_steps/reaction_rules/distance_rules.py
+scine_chemoton/gears/elementary_steps/reaction_rules/element_rules.py
+scine_chemoton/gears/elementary_steps/reaction_rules/polarization_rules.py
 scine_chemoton/gears/elementary_steps/trial_generator/__init__.py
 scine_chemoton/gears/elementary_steps/trial_generator/bond_based.py
 scine_chemoton/gears/elementary_steps/trial_generator/connectivity_analyzer.py
 scine_chemoton/gears/elementary_steps/trial_generator/fast_dissociations.py
 scine_chemoton/gears/elementary_steps/trial_generator/fragment_based.py
+scine_chemoton/gears/elementary_steps/trial_generator/template_based.py
 scine_chemoton/gears/kinetic_modeling/__init__.py
 scine_chemoton/gears/kinetic_modeling/concentration_query_functions.py
 scine_chemoton/gears/kinetic_modeling/kinetic_modeling.py
 scine_chemoton/gears/kinetic_modeling/prepare_kinetic_modeling_job.py
 scine_chemoton/tests/__init__.py
 scine_chemoton/tests/test_database_setup.py
 scine_chemoton/tests/gears/__init__.py
 scine_chemoton/tests/gears/test_compound.py
 scine_chemoton/tests/gears/test_kinetics.py
-scine_chemoton/tests/gears/test_pathfinder.py
 scine_chemoton/tests/gears/test_reaction.py
 scine_chemoton/tests/gears/test_refinement.py
 scine_chemoton/tests/gears/test_scheduler.py
 scine_chemoton/tests/gears/test_thermo.py
 scine_chemoton/tests/gears/conformers/__init__.py
 scine_chemoton/tests/gears/conformers/test_brute_force.py
 scine_chemoton/tests/gears/elementary_steps/__init__.py
 scine_chemoton/tests/gears/elementary_steps/mock_trial_generator.py
 scine_chemoton/tests/gears/elementary_steps/test_brute_force.py
-scine_chemoton/tests/gears/elementary_steps/test_compound_filters.py
 scine_chemoton/tests/gears/elementary_steps/test_further_dissociations_reactive_site_filters.py
 scine_chemoton/tests/gears/elementary_steps/test_minimal.py
-scine_chemoton/tests/gears/elementary_steps/test_minimum_energy_confomer.py
 scine_chemoton/tests/gears/elementary_steps/test_reactive_site_filters.py
 scine_chemoton/tests/gears/elementary_steps/trial_generator/__init__.py
 scine_chemoton/tests/gears/elementary_steps/trial_generator/test_bond_based.py
 scine_chemoton/tests/gears/elementary_steps/trial_generator/test_connectivity_analyzer.py
 scine_chemoton/tests/gears/elementary_steps/trial_generator/test_fast_dissociations.py
 scine_chemoton/tests/gears/elementary_steps/trial_generator/test_fragment_based.py
 scine_chemoton/tests/gears/kinetic_modeling/__init__.py
 scine_chemoton/tests/gears/kinetic_modeling/test_kinetic_modeling.py
 scine_chemoton/tests/resources/__init__.py
 scine_chemoton/tests/utilities/__init__.py
 scine_chemoton/tests/utilities/queries_test.py
-scine_chemoton/tests/utilities/test_get_molecular_formulas.py
 scine_chemoton/tests/utilities/test_insert_concentration.py
 scine_chemoton/tests/utilities/test_insert_initial_structure.py
 scine_chemoton/tests/utilities/test_masm.py
 scine_chemoton/tests/utilities/reactive_complexes/__init__.py
 scine_chemoton/tests/utilities/reactive_complexes/test_inter_reactive_complexes.py
 scine_chemoton/tests/utilities/reactive_complexes/test_lebedev_sphere.py
 scine_chemoton/tests/utilities/reactive_complexes/test_masm_pruning.py
 scine_chemoton/tests/utilities/reactive_complexes/test_unit_circle.py
 scine_chemoton/utilities/__init__.py
 scine_chemoton/utilities/calculation_creation_helpers.py
+scine_chemoton/utilities/comparisons.py
 scine_chemoton/utilities/compound_and_flask_creation.py
 scine_chemoton/utilities/energy_query_functions.py
 scine_chemoton/utilities/get_molecular_formula.py
 scine_chemoton/utilities/insert_concentration.py
 scine_chemoton/utilities/insert_initial_structure.py
 scine_chemoton/utilities/masm.py
 scine_chemoton/utilities/queries.py
```

### Comparing `scine_chemoton-2.2.0/README.rst` & `scine_chemoton-3.0.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -23,25 +23,27 @@
 
 Prerequisites
 .............
 
 The key requirements for Chemoton are the Python packages ``scine_utilities``,
 ``scine_database``, and ``scine_molassember``. These packages are available from
 PyPI and can be installed using ``pip``.
-However, these packages can also be compiled by hand. For the latter case please
-visit the repositories of each of the packages and follow their guidelines.
+However, these packages can also be compiled from sources. For the latter case please
+visit the repositories of each of the packages and follow their guidelines or
+bootstrap a `puffin <https://github.com/qcscine/puffin>`_ which will install the same
+dependencies.
 
 Installation
 ............
 
 Chemoton can be installed using ``pip`` (``pip3``) once the repository has been cloned:
 
 .. code-block:: bash
 
-   git clone <chemoton-repo> chemoton
+   git clone https://github.com/qcscine/chemoton.git
    cd chemoton
    pip install -r requirements.txt
    pip install .
 
 A non-root user can install the package using a virtual environment, or
 the ``--user`` flag.
 
@@ -86,35 +88,36 @@
 
    mongod --fork --port=27017 -dbpath=<path to db storage dir> -wiredTigerCacheSizeGB=1 --logpath=mongo.log
 
 2. Configure and bootstrap a ``puffin``:
 
 .. code-block:: bash
 
-   python3 -m puffin configure
+   pip install scine-puffin
+   python3 -m scine_puffin configure
    # Edit the generated puffin.yaml here
-   python3 -m puffin -c puffin.yaml bootstrap
+   python3 -m scine_puffin -c puffin.yaml bootstrap
 
 3. Source the ``puffin`` settings and tell it to listen to the correct DB.
 (Hostname and port should be the default ones.) Then start it.
 
 .. code-block:: bash
 
    source puffin.sh
    export PUFFIN_DATABASE_NAME=default
-   python3 -m puffin -c puffin.yaml start
+   python3 -m scine_puffin -c puffin.yaml start
 
 4. Run the Chemoton exploration defined in the ``__main__`` function:
 
 .. code-block:: bash
 
    python3 -m scine_chemoton wipe
 
 The optional ``wipe`` argument will start the example exploration with a clean
-``puffin_tests`` DB; giving the ``continue`` argument will reuse old data.
+``default`` DB; giving the ``continue`` argument will reuse old data.
 
 Expanding on the Minimal Example
 ................................
 
 The functionalities used in Chemoton's ``__main__.py`` are a good starting point
 for most simple explorations. The file contains a lot of settings that are
 explicitly set to their defaults in order to show their existence.
@@ -136,14 +139,14 @@
 release as archived on `Zenodo <https://doi.org/10.5281/zenodo.6695583>`_ (DOI
 10.5281/zenodo.6695583; please use the DOI of the respective release).
 
 In addition, we kindly request you to cite the following article when using Chemoton:
 
 J. P. Unsleber, S. A. Grimmel, M. Reiher,
 "Chemoton 2.0: Autonomous Exploration of Chemical Reaction Networks",
-*arXiv:2202.13011 [physics.chem-ph].*
+*J. Chem. Theory Comput.*, **2022**, *18*, 5393.
 
 Support and Contact
 -------------------
 
 In case you should encounter problems or bugs, please write a short message
 to scine@phys.chem.ethz.ch.
```

### Comparing `scine_chemoton-2.2.0/setup.cfg` & `scine_chemoton-3.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,14 @@
 
 [pylint.TYPECHECK]
 ignored-modules = scine_utilities,scine_database,scine_molassembler,scine_readuct,scine_sparrow,scine_swoose,scine_kinetx
 ignored-argument-names = _.*|^ignored_|^unused_|arg|args|kwargs
 disable = C,R,W0511,W0212,W1514,W0622,W0105,W1510
 generated-members = Lock
 ignore = _version.py
-overgeneral-exceptions = Exception
+overgeneral-exceptions = builtins.Exception
 
 [egg_info]
 tag_build = 
 tag_date = 0
 tag_svn_revision = 0
```

### Comparing `scine_chemoton-2.2.0/setup.py` & `scine_chemoton-3.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from os import path
 from setuptools import setup, find_packages
 import sys
 
+
 # NOTE: This file must remain Python 2 compatible for the foreseeable future,
 # to ensure that we error out properly for people with outdated setuptools
 # and/or pip.
 min_version = (3, 6)
 if sys.version_info < min_version:
     error = """
 Chemoton does not support Python {0}.{1}.
@@ -39,15 +40,16 @@
     version=__version__,
     description="Software driving the automated exploration of chemical reaction networks",
     long_description=readme,
     author="ETH Zurich, Laboratory of Physical Chemistry, Reiher Group",
     author_email="scine@phys.chem.ethz.ch",
     url="https://www.scine.ethz.ch",
     python_requires=">={}".format(".".join(str(n) for n in min_version)),
-    packages=find_packages(exclude=["docs", "tests"]),
+    packages=find_packages(include=["scine_chemoton", "scine_chemoton.*"],
+                           exclude=["scine_chemoton.tests*"]),
     entry_points={
         "console_scripts": [
             # 'command = some.module:some_function',
         ],
     },
     include_package_data=True,
     package_data={
```

### Comparing `scine_chemoton-2.2.0/PKG-INFO` & `scine_chemoton-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scine_chemoton
-Version: 2.2.0
+Version: 3.0.0
 Summary: Software driving the automated exploration of chemical reaction networks
 Home-page: https://www.scine.ethz.ch
 Author: ETH Zurich, Laboratory of Physical Chemistry, Reiher Group
 Author-email: scine@phys.chem.ethz.ch
 License: BSD (3-clause)
 Description: .. image:: docs/source/res/chemoton_header.png
            :alt: SCINE Chemoton
@@ -31,25 +31,27 @@
         
         Prerequisites
         .............
         
         The key requirements for Chemoton are the Python packages ``scine_utilities``,
         ``scine_database``, and ``scine_molassember``. These packages are available from
         PyPI and can be installed using ``pip``.
-        However, these packages can also be compiled by hand. For the latter case please
-        visit the repositories of each of the packages and follow their guidelines.
+        However, these packages can also be compiled from sources. For the latter case please
+        visit the repositories of each of the packages and follow their guidelines or
+        bootstrap a `puffin <https://github.com/qcscine/puffin>`_ which will install the same
+        dependencies.
         
         Installation
         ............
         
         Chemoton can be installed using ``pip`` (``pip3``) once the repository has been cloned:
         
         .. code-block:: bash
         
-           git clone <chemoton-repo> chemoton
+           git clone https://github.com/qcscine/chemoton.git
            cd chemoton
            pip install -r requirements.txt
            pip install .
         
         A non-root user can install the package using a virtual environment, or
         the ``--user`` flag.
         
@@ -94,35 +96,36 @@
         
            mongod --fork --port=27017 -dbpath=<path to db storage dir> -wiredTigerCacheSizeGB=1 --logpath=mongo.log
         
         2. Configure and bootstrap a ``puffin``:
         
         .. code-block:: bash
         
-           python3 -m puffin configure
+           pip install scine-puffin
+           python3 -m scine_puffin configure
            # Edit the generated puffin.yaml here
-           python3 -m puffin -c puffin.yaml bootstrap
+           python3 -m scine_puffin -c puffin.yaml bootstrap
         
         3. Source the ``puffin`` settings and tell it to listen to the correct DB.
         (Hostname and port should be the default ones.) Then start it.
         
         .. code-block:: bash
         
            source puffin.sh
            export PUFFIN_DATABASE_NAME=default
-           python3 -m puffin -c puffin.yaml start
+           python3 -m scine_puffin -c puffin.yaml start
         
         4. Run the Chemoton exploration defined in the ``__main__`` function:
         
         .. code-block:: bash
         
            python3 -m scine_chemoton wipe
         
         The optional ``wipe`` argument will start the example exploration with a clean
-        ``puffin_tests`` DB; giving the ``continue`` argument will reuse old data.
+        ``default`` DB; giving the ``continue`` argument will reuse old data.
         
         Expanding on the Minimal Example
         ................................
         
         The functionalities used in Chemoton's ``__main__.py`` are a good starting point
         for most simple explorations. The file contains a lot of settings that are
         explicitly set to their defaults in order to show their existence.
@@ -144,15 +147,15 @@
         release as archived on `Zenodo <https://doi.org/10.5281/zenodo.6695583>`_ (DOI
         10.5281/zenodo.6695583; please use the DOI of the respective release).
         
         In addition, we kindly request you to cite the following article when using Chemoton:
         
         J. P. Unsleber, S. A. Grimmel, M. Reiher,
         "Chemoton 2.0: Autonomous Exploration of Chemical Reaction Networks",
-        *arXiv:2202.13011 [physics.chem-ph].*
+        *J. Chem. Theory Comput.*, **2022**, *18*, 5393.
         
         Support and Contact
         -------------------
         
         In case you should encounter problems or bugs, please write a short message
         to scine@phys.chem.ethz.ch.
```

