# Comparing `tmp/permamodel-0.2.1.tar.gz` & `tmp/permamodel-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permamodel-0.2.1.tar", last modified: Thu Apr 20 21:24:50 2023, max compression
+gzip compressed data, was "permamodel-0.2.2.tar", last modified: Fri May 12 21:04:31 2023, max compression
```

## Comparing `permamodel-0.2.1.tar` & `permamodel-0.2.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.373119 permamodel-0.2.1/
--rw-r--r--   0 mpiper     (501) staff       (20)      924 2023-04-20 21:17:39.000000 permamodel-0.2.1/CITATION.cff
--rw-r--r--   0 mpiper     (501) staff       (20)     1077 2023-04-20 21:17:39.000000 permamodel-0.2.1/LICENSE
--rw-r--r--   0 mpiper     (501) staff       (20)      331 2023-04-20 21:17:39.000000 permamodel-0.2.1/MANIFEST.in
--rw-r--r--   0 mpiper     (501) staff       (20)     3318 2023-04-20 21:24:50.373193 permamodel-0.2.1/PKG-INFO
--rw-r--r--   0 mpiper     (501) staff       (20)     1151 2023-04-20 21:17:39.000000 permamodel-0.2.1/README.md
--rw-r--r--   0 mpiper     (501) staff       (20)     4945 2023-04-20 21:17:39.000000 permamodel-0.2.1/noxfile.py
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.342115 permamodel-0.2.1/permamodel/
--rw-r--r--   0 mpiper     (501) staff       (20)      613 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/__init__.py
--rw-r--r--   0 mpiper     (501) staff       (20)       22 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/_version.py
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.344673 permamodel-0.2.1/permamodel/components/
--rw-r--r--   0 mpiper     (501) staff       (20)    22202 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/Ku.py
--rw-r--r--   0 mpiper     (501) staff       (20)    52201 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/Ku_method.py
--rw-r--r--   0 mpiper     (501) staff       (20)       25 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/__init__.py
--rw-r--r--   0 mpiper     (501) staff       (20)    11499 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/bmi_Ku.py
--rw-r--r--   0 mpiper     (501) staff       (20)    16862 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/bmi_Ku_component.py
--rw-r--r--   0 mpiper     (501) staff       (20)    12954 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/bmi_frost_number.py
--rw-r--r--   0 mpiper     (501) staff       (20)    11379 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/bmi_frost_number_Geo.py
--rw-r--r--   0 mpiper     (501) staff       (20)    14052 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/frost_number.py
--rw-r--r--   0 mpiper     (501) staff       (20)    42982 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/frost_number_Geo.py
--rw-r--r--   0 mpiper     (501) staff       (20)    29955 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/components/perma_base.py
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.366952 permamodel-0.2.1/permamodel/data/
--rwxr-xr-x   0 mpiper     (501) staff       (20)  2195333 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/T_CLAY.nc4
--rwxr-xr-x   0 mpiper     (501) staff       (20)  2629756 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/T_OC.nc4
--rwxr-xr-x   0 mpiper     (501) staff       (20)  2329260 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/T_SAND.nc4
--rwxr-xr-x   0 mpiper     (501) staff       (20)  2266288 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/T_SILT.nc4
--rwxr-xr-x   0 mpiper     (501) staff       (20)      196 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/Typical_Thermal_Parameters.csv
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.340057 permamodel-0.2.1/permamodel/data/test_directory/
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.368928 permamodel-0.2.1/permamodel/data/test_directory/inputs/
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/air_temperature.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/frozen_vegetation_diffusivity.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/frozen_vegetation_height.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/snow_density.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/snow_thickness.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/soil_water_content.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/temperature_amplitude.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/thawed_vegetation_diffusivity.nc
--rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/data/test_directory/inputs/thawed_vegetation_height.nc
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.369885 permamodel-0.2.1/permamodel/examples/
--rw-r--r--   0 mpiper     (501) staff       (20)     1540 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/examples/Frostnumber_example_singlesite_singleyear.cfg
--rw-r--r--   0 mpiper     (501) staff       (20)     1668 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/examples/Ku_bmi_example_config.toml
--rw-r--r--   0 mpiper     (501) staff       (20)     1668 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/examples/Ku_example_config.toml
--rw-r--r--   0 mpiper     (501) staff       (20)     3517 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/examples/Ku_method.cfg
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.371422 permamodel-0.2.1/permamodel/tests/
--rw-r--r--   0 mpiper     (501) staff       (20)       40 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/__init__.py
--rw-r--r--   0 mpiper     (501) staff       (20)     7003 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_Ku.py
--rw-r--r--   0 mpiper     (501) staff       (20)      746 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_Ku_method.py
--rw-r--r--   0 mpiper     (501) staff       (20)     3709 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_frost_number.py
--rw-r--r--   0 mpiper     (501) staff       (20)    10122 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_frost_number_Geo.py
--rw-r--r--   0 mpiper     (501) staff       (20)    11856 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_frost_number_Geo_bmi.py
--rw-r--r--   0 mpiper     (501) staff       (20)     8485 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_frost_number_bmi.py
--rw-r--r--   0 mpiper     (501) staff       (20)      820 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/tests/test_package_directories.py
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.372940 permamodel-0.2.1/permamodel/utils/
--rwxr-xr-x   0 mpiper     (501) staff       (20)    83475 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/BMI_base.py
--rwxr-xr-x   0 mpiper     (501) staff       (20)       26 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/__init__.py
--rwxr-xr-x   0 mpiper     (501) staff       (20)     6817 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/file_utils.py
--rwxr-xr-x   0 mpiper     (501) staff       (20)    14005 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/model_input.py
--rwxr-xr-x   0 mpiper     (501) staff       (20)     8788 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/outlets.py
--rwxr-xr-x   0 mpiper     (501) staff       (20)    14496 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/pixels.py
--rwxr-xr-x   0 mpiper     (501) staff       (20)    24124 2023-04-20 21:17:39.000000 permamodel-0.2.1/permamodel/utils/rti_files.py
-drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-04-20 21:24:50.342697 permamodel-0.2.1/permamodel.egg-info/
--rw-r--r--   0 mpiper     (501) staff       (20)     3318 2023-04-20 21:24:50.000000 permamodel-0.2.1/permamodel.egg-info/PKG-INFO
--rw-r--r--   0 mpiper     (501) staff       (20)     2112 2023-04-20 21:24:50.000000 permamodel-0.2.1/permamodel.egg-info/SOURCES.txt
--rw-r--r--   0 mpiper     (501) staff       (20)        1 2023-04-20 21:24:50.000000 permamodel-0.2.1/permamodel.egg-info/dependency_links.txt
--rw-r--r--   0 mpiper     (501) staff       (20)      181 2023-04-20 21:24:50.000000 permamodel-0.2.1/permamodel.egg-info/requires.txt
--rw-r--r--   0 mpiper     (501) staff       (20)       11 2023-04-20 21:24:50.000000 permamodel-0.2.1/permamodel.egg-info/top_level.txt
--rw-r--r--   0 mpiper     (501) staff       (20)     2419 2023-04-20 21:17:39.000000 permamodel-0.2.1/pyproject.toml
--rw-r--r--   0 mpiper     (501) staff       (20)       62 2023-04-20 21:17:39.000000 permamodel-0.2.1/requirements.txt
--rw-r--r--   0 mpiper     (501) staff       (20)      286 2023-04-20 21:24:50.373445 permamodel-0.2.1/setup.cfg
--rw-r--r--   0 mpiper     (501) staff       (20)       63 2023-04-20 21:17:39.000000 permamodel-0.2.1/setup.py
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-05-12 21:04:31.101520 permamodel-0.2.2/
+-rw-r--r--   0 mpiper     (501) staff       (20)      924 2023-05-12 20:59:29.000000 permamodel-0.2.2/CITATION.cff
+-rw-r--r--   0 mpiper     (501) staff       (20)     1077 2023-05-12 20:59:29.000000 permamodel-0.2.2/LICENSE
+-rw-r--r--   0 mpiper     (501) staff       (20)      331 2023-05-12 20:59:29.000000 permamodel-0.2.2/MANIFEST.in
+-rw-r--r--   0 mpiper     (501) staff       (20)     3318 2023-05-12 21:04:31.101622 permamodel-0.2.2/PKG-INFO
+-rw-r--r--   0 mpiper     (501) staff       (20)     1151 2023-05-12 20:59:29.000000 permamodel-0.2.2/README.md
+-rw-r--r--   0 mpiper     (501) staff       (20)     4945 2023-05-12 20:59:29.000000 permamodel-0.2.2/noxfile.py
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-05-12 21:04:31.074566 permamodel-0.2.2/permamodel/
+-rw-r--r--   0 mpiper     (501) staff       (20)      613 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/__init__.py
+-rw-r--r--   0 mpiper     (501) staff       (20)       22 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/_version.py
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-05-12 21:04:31.077564 permamodel-0.2.2/permamodel/components/
+-rw-r--r--   0 mpiper     (501) staff       (20)    22576 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/components/Ku.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    52201 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/components/Ku_method.py
+-rw-r--r--   0 mpiper     (501) staff       (20)       25 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/components/__init__.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    11499 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/components/bmi_Ku.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    16862 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/components/bmi_Ku_component.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    12954 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/components/bmi_frost_number.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    11379 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/components/bmi_frost_number_Geo.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    14052 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/components/frost_number.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    42982 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/components/frost_number_Geo.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    29955 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/components/perma_base.py
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-05-12 21:04:31.096262 permamodel-0.2.2/permamodel/data/
+-rwxr-xr-x   0 mpiper     (501) staff       (20)  2195333 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/T_CLAY.nc4
+-rwxr-xr-x   0 mpiper     (501) staff       (20)  2629756 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/T_OC.nc4
+-rwxr-xr-x   0 mpiper     (501) staff       (20)  2329260 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/T_SAND.nc4
+-rwxr-xr-x   0 mpiper     (501) staff       (20)  2266288 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/T_SILT.nc4
+-rwxr-xr-x   0 mpiper     (501) staff       (20)      196 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/Typical_Thermal_Parameters.csv
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-05-12 21:04:31.072398 permamodel-0.2.2/permamodel/data/test_directory/
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-05-12 21:04:31.097851 permamodel-0.2.2/permamodel/data/test_directory/inputs/
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/test_directory/inputs/air_temperature.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/test_directory/inputs/frozen_vegetation_diffusivity.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/test_directory/inputs/frozen_vegetation_height.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/test_directory/inputs/snow_density.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/test_directory/inputs/snow_thickness.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/test_directory/inputs/soil_water_content.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/test_directory/inputs/temperature_amplitude.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/test_directory/inputs/thawed_vegetation_diffusivity.nc
+-rw-r--r--   0 mpiper     (501) staff       (20)     6544 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/data/test_directory/inputs/thawed_vegetation_height.nc
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-05-12 21:04:31.098571 permamodel-0.2.2/permamodel/examples/
+-rw-r--r--   0 mpiper     (501) staff       (20)     1540 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/examples/Frostnumber_example_singlesite_singleyear.cfg
+-rw-r--r--   0 mpiper     (501) staff       (20)     1818 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/examples/Ku_bmi_example_config.toml
+-rw-r--r--   0 mpiper     (501) staff       (20)     1818 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/examples/Ku_example_config.toml
+-rw-r--r--   0 mpiper     (501) staff       (20)     3517 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/examples/Ku_method.cfg
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-05-12 21:04:31.099862 permamodel-0.2.2/permamodel/tests/
+-rw-r--r--   0 mpiper     (501) staff       (20)       40 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/tests/__init__.py
+-rw-r--r--   0 mpiper     (501) staff       (20)     6996 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/tests/test_Ku.py
+-rw-r--r--   0 mpiper     (501) staff       (20)      746 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/tests/test_Ku_method.py
+-rw-r--r--   0 mpiper     (501) staff       (20)     3709 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/tests/test_frost_number.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    10122 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/tests/test_frost_number_Geo.py
+-rw-r--r--   0 mpiper     (501) staff       (20)    11856 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/tests/test_frost_number_Geo_bmi.py
+-rw-r--r--   0 mpiper     (501) staff       (20)     8485 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/tests/test_frost_number_bmi.py
+-rw-r--r--   0 mpiper     (501) staff       (20)      820 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/tests/test_package_directories.py
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-05-12 21:04:31.101298 permamodel-0.2.2/permamodel/utils/
+-rwxr-xr-x   0 mpiper     (501) staff       (20)    83475 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/utils/BMI_base.py
+-rwxr-xr-x   0 mpiper     (501) staff       (20)       26 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/utils/__init__.py
+-rwxr-xr-x   0 mpiper     (501) staff       (20)     6817 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/utils/file_utils.py
+-rwxr-xr-x   0 mpiper     (501) staff       (20)    14005 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/utils/model_input.py
+-rwxr-xr-x   0 mpiper     (501) staff       (20)     8788 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/utils/outlets.py
+-rwxr-xr-x   0 mpiper     (501) staff       (20)    14496 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/utils/pixels.py
+-rwxr-xr-x   0 mpiper     (501) staff       (20)    24124 2023-05-12 20:59:29.000000 permamodel-0.2.2/permamodel/utils/rti_files.py
+drwxr-xr-x   0 mpiper     (501) staff       (20)        0 2023-05-12 21:04:31.075238 permamodel-0.2.2/permamodel.egg-info/
+-rw-r--r--   0 mpiper     (501) staff       (20)     3318 2023-05-12 21:04:31.000000 permamodel-0.2.2/permamodel.egg-info/PKG-INFO
+-rw-r--r--   0 mpiper     (501) staff       (20)     2112 2023-05-12 21:04:31.000000 permamodel-0.2.2/permamodel.egg-info/SOURCES.txt
+-rw-r--r--   0 mpiper     (501) staff       (20)        1 2023-05-12 21:04:31.000000 permamodel-0.2.2/permamodel.egg-info/dependency_links.txt
+-rw-r--r--   0 mpiper     (501) staff       (20)      181 2023-05-12 21:04:31.000000 permamodel-0.2.2/permamodel.egg-info/requires.txt
+-rw-r--r--   0 mpiper     (501) staff       (20)       11 2023-05-12 21:04:31.000000 permamodel-0.2.2/permamodel.egg-info/top_level.txt
+-rw-r--r--   0 mpiper     (501) staff       (20)     2419 2023-05-12 20:59:29.000000 permamodel-0.2.2/pyproject.toml
+-rw-r--r--   0 mpiper     (501) staff       (20)       62 2023-05-12 20:59:29.000000 permamodel-0.2.2/requirements.txt
+-rw-r--r--   0 mpiper     (501) staff       (20)      286 2023-05-12 21:04:31.101915 permamodel-0.2.2/setup.cfg
+-rw-r--r--   0 mpiper     (501) staff       (20)       63 2023-05-12 20:59:29.000000 permamodel-0.2.2/setup.py
```

### Comparing `permamodel-0.2.1/CITATION.cff` & `permamodel-0.2.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/LICENSE` & `permamodel-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/PKG-INFO` & `permamodel-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permamodel
-Version: 0.2.1
+Version: 0.2.2
 Summary: Permafrost models with a Basic Model Interface
 Author-email: Elchin Jafarov <elchin.jafarov@colorado.edu>, Scott Stewart <scotts@colorado.edu>, Kang Wang <kang.wang@colorado.edu>, Ethan Pierce <ethan.pierce@colorado.edu>, Irina Overeem <irina.overeem@colorado.edu>
 Maintainer-email: Mark Piper <mark.piper@colorado.edu>, Eric Hutton <eric.hutton@colorado.edu>
 License: MIT License
 Project-URL: Homepage, https://permamodel.github.io
 Project-URL: Repository, https://github.com/permamodel/permamodel
 Keywords: bmi,component modeling,earth science,model coupling,numerical modeling,permafrost
```

### Comparing `permamodel-0.2.1/README.md` & `permamodel-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/noxfile.py` & `permamodel-0.2.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/__init__.py` & `permamodel-0.2.2/permamodel/__init__.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/components/Ku.py` & `permamodel-0.2.2/permamodel/components/Ku.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,52 +164,60 @@
         self.inputs_dir = config["directories"]["inputs_dir"]
         self.outputs_dir = config["directories"]["outputs_dir"]
 
         # The domain for this model instance
         self.number_of_years = config["domain"]["number_of_years"]
         self.grid_shape = config["domain"]["grid_shape"]
 
-        # Paths to the input data files
-        self.input_files = {var: ncfile for var, ncfile in config["files"].items()}
+        # Input variables
+        self.info = {var: info for var, info in config["variables"].items()}
 
         # Soil properties
         self.soils = {soil: props for soil, props in config["soils"].items()}
 
         # Physical constants
         self.constants = {var: val for var, val in config["constants"].items()}
 
     def read_input_files(self):
         """Read input data files and store fields as instance variables."""
 
-        # Raise an error if there are no input files to read.
-        if len(self.input_files) == 0:
+        # Raise an error if there is no information about variables.
+        if not hasattr(self, "info"):
             raise ValueError(
-                "No input files to read: did you call read_config() first?"
+                "Did not find information about input variables: did you call read_config() first?"
             )
 
-        # Read input data from each file.
-        for key, file in self.input_files.items():
-            var = key.replace("_file", "")
-            data = xr.open_dataarray(self.inputs_dir + file)
+        if len(self.info) == 0:
+            raise ValueError(
+                "No input variables found: did you call read_config() first?"
+            )
 
-            data = self.broadcast(data)
+        # Read input data from each file.
+        for var, info in self.info.items():
+            if len(info["nc_file"]) > 0:
+                data = xr.open_dataarray(self.inputs_dir + info["nc_file"])
+                data_cube = self.broadcast(data)
+                setattr(self, var, data_cube)
 
-            setattr(self, var, data)
+            else:
+                data = xr.DataArray([info["scalar"]])
+                data_cube = self.broadcast(data)
+                setattr(self, var, data_cube)
 
         # Read soil properties, if not defined directly in the config file.
         for soil, props in self.soils.items():
             if len(props["nc_file"]) > 0:
                 data = xr.open_dataarray(prop["nc_file"])
-
-                data = self.broadcast(data)
+                data_cube = self.broadcast(data)
 
             else:
-                data = xr.full_like(self.air_temperature, props["scalar_fraction"])
+                data = xr.DataArray([props["scalar_fraction"]])
+                data_cube = self.broadcast(data)
 
-            self.soils[soil]["fraction"] = data
+            self.soils[soil]["fraction"] = data_cube
 
     def broadcast(self, data: xr.DataArray) -> xr.DataArray:
         """Broadcast an xarray DataArray to a shape that matches the model's domain.
 
         Returns:
             data:
                 The input DataArray, with new dimensions of (x, y, time).
@@ -235,16 +243,15 @@
                 },
                 axis=[0, 1, 2],
             )
             data = data.squeeze(dim_name)
 
         else:
             raise ValueError(
-                var
-                + " data cannot be broadcast to shape "
+                "DataArray cannot be broadcast to shape "
                 + str((self.number_of_years, self.grid_shape[0], self.grid_shape[1]))
             )
 
         return data
 
     def construct_results(
         self,
```

### Comparing `permamodel-0.2.1/permamodel/components/Ku_method.py` & `permamodel-0.2.2/permamodel/components/Ku_method.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/components/bmi_Ku.py` & `permamodel-0.2.2/permamodel/components/bmi_Ku.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/components/bmi_Ku_component.py` & `permamodel-0.2.2/permamodel/components/bmi_Ku_component.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/components/bmi_frost_number.py` & `permamodel-0.2.2/permamodel/components/bmi_frost_number.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/components/bmi_frost_number_Geo.py` & `permamodel-0.2.2/permamodel/components/bmi_frost_number_Geo.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/components/frost_number.py` & `permamodel-0.2.2/permamodel/components/frost_number.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/components/frost_number_Geo.py` & `permamodel-0.2.2/permamodel/components/frost_number_Geo.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/components/perma_base.py` & `permamodel-0.2.2/permamodel/components/perma_base.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/T_CLAY.nc4` & `permamodel-0.2.2/permamodel/data/T_CLAY.nc4`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/T_OC.nc4` & `permamodel-0.2.2/permamodel/data/T_OC.nc4`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/T_SAND.nc4` & `permamodel-0.2.2/permamodel/data/T_SAND.nc4`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/T_SILT.nc4` & `permamodel-0.2.2/permamodel/data/T_SILT.nc4`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/test_directory/inputs/air_temperature.nc` & `permamodel-0.2.2/permamodel/data/test_directory/inputs/air_temperature.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/test_directory/inputs/frozen_vegetation_diffusivity.nc` & `permamodel-0.2.2/permamodel/data/test_directory/inputs/frozen_vegetation_diffusivity.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/test_directory/inputs/frozen_vegetation_height.nc` & `permamodel-0.2.2/permamodel/data/test_directory/inputs/frozen_vegetation_height.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/test_directory/inputs/snow_density.nc` & `permamodel-0.2.2/permamodel/data/test_directory/inputs/snow_density.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/test_directory/inputs/snow_thickness.nc` & `permamodel-0.2.2/permamodel/data/test_directory/inputs/snow_thickness.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/test_directory/inputs/soil_water_content.nc` & `permamodel-0.2.2/permamodel/data/test_directory/inputs/soil_water_content.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/test_directory/inputs/temperature_amplitude.nc` & `permamodel-0.2.2/permamodel/data/test_directory/inputs/temperature_amplitude.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/test_directory/inputs/thawed_vegetation_diffusivity.nc` & `permamodel-0.2.2/permamodel/data/test_directory/inputs/thawed_vegetation_diffusivity.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/data/test_directory/inputs/thawed_vegetation_height.nc` & `permamodel-0.2.2/permamodel/data/test_directory/inputs/thawed_vegetation_height.nc`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/examples/Frostnumber_example_singlesite_singleyear.cfg` & `permamodel-0.2.2/permamodel/examples/Frostnumber_example_singlesite_singleyear.cfg`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/examples/Ku_bmi_example_config.toml` & `permamodel-0.2.2/permamodel/examples/Ku_bmi_example_config.toml`

 * *Files 21% similar despite different names*

```diff
@@ -4,24 +4,49 @@
 inputs_dir = "permamodel/data/test_directory/inputs/"
 outputs_dir = "permamodel/data/test_directory/outputs/"
 
 [domain]
 number_of_years = 100 # time
 grid_shape = [100, 100] # [y, x]
 
-[files]
-air_temperature_file = "air_temperature.nc"
-temperature_amplitude_file = "temperature_amplitude.nc"
-snow_thickness_file = "snow_thickness.nc"
-snow_density_file = "snow_density.nc"
-soil_water_content_file = "soil_water_content.nc"
-frozen_vegetation_height_file = "frozen_vegetation_height.nc"
-thawed_vegetation_height_file = "thawed_vegetation_height.nc"
-frozen_vegetation_diffusivity_file = "frozen_vegetation_diffusivity.nc"
-thawed_vegetation_diffusivity_file = "thawed_vegetation_diffusivity.nc"
+[variables.air_temperature]
+nc_file = 'air_temperature.nc'
+scalar = -999
+
+[variables.temperature_amplitude]
+nc_file = 'temperature_amplitude.nc'
+scalar = -999
+
+[variables.snow_thickness]
+nc_file = 'snow_thickness.nc'
+scalar = -999
+
+[variables.snow_density]
+nc_file = 'snow_density.nc'
+scalar = 240.0
+
+[variables.soil_water_content]
+nc_file = 'soil_water_content.nc'
+scalar = -999
+
+[variables.frozen_vegetation_height]
+nc_file = ''
+scalar = 0.1
+
+[variables.thawed_vegetation_height]
+nc_file = ''
+scalar = 0.1
+
+[variables.frozen_vegetation_diffusivity]
+nc_file = ''
+scalar = 2.39e-6
+
+[variables.thawed_vegetation_diffusivity]
+nc_file = ''
+scalar = 1.0556e-6
 
 [soils.sand]
 scalar_fraction = 0.25
 nc_file = '' 
 bulk_density = 1300
 heat_capacity = 1500
 conductivity_thawed_dry = 1.05
```

### Comparing `permamodel-0.2.1/permamodel/examples/Ku_example_config.toml` & `permamodel-0.2.2/permamodel/examples/Ku_example_config.toml`

 * *Files 21% similar despite different names*

```diff
@@ -4,24 +4,49 @@
 inputs_dir = "permamodel/data/test_directory/inputs/"
 outputs_dir = "permamodel/data/test_directory/outputs/"
 
 [domain]
 number_of_years = 100 # time
 grid_shape = [100, 100] # [y, x]
 
-[files]
-air_temperature_file = "air_temperature.nc"
-temperature_amplitude_file = "temperature_amplitude.nc"
-snow_thickness_file = "snow_thickness.nc"
-snow_density_file = "snow_density.nc"
-soil_water_content_file = "soil_water_content.nc"
-frozen_vegetation_height_file = "frozen_vegetation_height.nc"
-thawed_vegetation_height_file = "thawed_vegetation_height.nc"
-frozen_vegetation_diffusivity_file = "frozen_vegetation_diffusivity.nc"
-thawed_vegetation_diffusivity_file = "thawed_vegetation_diffusivity.nc"
+[variables.air_temperature]
+nc_file = 'air_temperature.nc'
+scalar = -999
+
+[variables.temperature_amplitude]
+nc_file = 'temperature_amplitude.nc'
+scalar = -999
+
+[variables.snow_thickness]
+nc_file = 'snow_thickness.nc'
+scalar = -999
+
+[variables.snow_density]
+nc_file = 'snow_density.nc'
+scalar = 240.0
+
+[variables.soil_water_content]
+nc_file = 'soil_water_content.nc'
+scalar = -999
+
+[variables.frozen_vegetation_height]
+nc_file = ''
+scalar = 0.1
+
+[variables.thawed_vegetation_height]
+nc_file = ''
+scalar = 0.1
+
+[variables.frozen_vegetation_diffusivity]
+nc_file = ''
+scalar = 2.39e-6
+
+[variables.thawed_vegetation_diffusivity]
+nc_file = ''
+scalar = 1.0556e-6
 
 [soils.sand]
 scalar_fraction = 0.25
 nc_file = '' 
 bulk_density = 1300
 heat_capacity = 1500
 conductivity_thawed_dry = 1.05
```

### Comparing `permamodel-0.2.1/permamodel/examples/Ku_method.cfg` & `permamodel-0.2.2/permamodel/examples/Ku_method.cfg`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/tests/test_Ku.py` & `permamodel-0.2.2/permamodel/tests/test_Ku.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Ku.read_config(config)
 
     assert Ku.experiment == "test"
     assert Ku.inputs_dir == "permamodel/data/test_directory/inputs/"
     assert Ku.outputs_dir == "permamodel/data/test_directory/outputs/"
     assert Ku.number_of_years == 100
     assert Ku.grid_shape == [100, 100]
-    assert len(Ku.input_files) > 0
+    assert len(Ku.info) > 0
     assert Ku.soils["sand"]["heat_capacity"] == 1500
     assert len(Ku.constants) > 0
 
 
 class TestReadInputs:
     def test_throw_error_if_no_files_list(self, Ku):
         with pytest.raises(ValueError):
```

### Comparing `permamodel-0.2.1/permamodel/tests/test_Ku_method.py` & `permamodel-0.2.2/permamodel/tests/test_Ku_method.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/tests/test_frost_number.py` & `permamodel-0.2.2/permamodel/tests/test_frost_number.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/tests/test_frost_number_Geo.py` & `permamodel-0.2.2/permamodel/tests/test_frost_number_Geo.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/tests/test_frost_number_Geo_bmi.py` & `permamodel-0.2.2/permamodel/tests/test_frost_number_Geo_bmi.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/tests/test_frost_number_bmi.py` & `permamodel-0.2.2/permamodel/tests/test_frost_number_bmi.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/tests/test_package_directories.py` & `permamodel-0.2.2/permamodel/tests/test_package_directories.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/utils/BMI_base.py` & `permamodel-0.2.2/permamodel/utils/BMI_base.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/utils/file_utils.py` & `permamodel-0.2.2/permamodel/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/utils/model_input.py` & `permamodel-0.2.2/permamodel/utils/model_input.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/utils/outlets.py` & `permamodel-0.2.2/permamodel/utils/outlets.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/utils/pixels.py` & `permamodel-0.2.2/permamodel/utils/pixels.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel/utils/rti_files.py` & `permamodel-0.2.2/permamodel/utils/rti_files.py`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/permamodel.egg-info/PKG-INFO` & `permamodel-0.2.2/permamodel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: permamodel
-Version: 0.2.1
+Version: 0.2.2
 Summary: Permafrost models with a Basic Model Interface
 Author-email: Elchin Jafarov <elchin.jafarov@colorado.edu>, Scott Stewart <scotts@colorado.edu>, Kang Wang <kang.wang@colorado.edu>, Ethan Pierce <ethan.pierce@colorado.edu>, Irina Overeem <irina.overeem@colorado.edu>
 Maintainer-email: Mark Piper <mark.piper@colorado.edu>, Eric Hutton <eric.hutton@colorado.edu>
 License: MIT License
 Project-URL: Homepage, https://permamodel.github.io
 Project-URL: Repository, https://github.com/permamodel/permamodel
 Keywords: bmi,component modeling,earth science,model coupling,numerical modeling,permafrost
```

### Comparing `permamodel-0.2.1/permamodel.egg-info/SOURCES.txt` & `permamodel-0.2.2/permamodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `permamodel-0.2.1/pyproject.toml` & `permamodel-0.2.2/pyproject.toml`

 * *Files identical despite different names*

