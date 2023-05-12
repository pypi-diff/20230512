# Comparing `tmp/z3-solver-4.9.0.0.tar.gz` & `tmp/z3-solver-4.9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3-solver-4.9.0.0.tar", last modified: Wed Jul  6 16:52:32 2022, max compression
+gzip compressed data, was "z3-solver-4.9.1.0.tar", last modified: Wed Jul  6 19:24:48 2022, max compression
```

## Comparing `z3-solver-4.9.0.0.tar` & `z3-solver-4.9.1.0.tar`

### file list

```diff
@@ -1,2370 +1,2370 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.607698 z3-solver-4.9.0.0/
--rw-r--r--   0 vsts      (1001) docker     (121)      696 2022-07-06 16:52:32.607698 z3-solver-4.9.0.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      509 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/README.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.475698 z3-solver-4.9.0.0/core/
--rw-r--r--   0 vsts      (1001) docker     (121)    27881 2022-07-06 16:52:31.851694 z3-solver-4.9.0.0/core/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1096 2022-07-06 16:52:31.851694 z3-solver-4.9.0.0/core/LICENSE.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.475698 z3-solver-4.9.0.0/core/cmake/
--rw-r--r--   0 vsts      (1001) docker     (121)     1644 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/Z3Config.cmake.in
--rw-r--r--   0 vsts      (1001) docker     (121)      594 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/check_link_atomic.cmake
--rw-r--r--   0 vsts      (1001) docker     (121)      942 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0 vsts      (1001) docker     (121)     2327 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/compiler_lto.cmake
--rw-r--r--   0 vsts      (1001) docker     (121)     5925 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/compiler_warnings.cmake
--rw-r--r--   0 vsts      (1001) docker     (121)      771 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/cxx_compiler_flags_overrides.cmake
--rw-r--r--   0 vsts      (1001) docker     (121)     8433 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/git_utils.cmake
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.475698 z3-solver-4.9.0.0/core/cmake/modules/
--rw-r--r--   0 vsts      (1001) docker     (121)      281 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/modules/DotnetImports.props.in
--rw-r--r--   0 vsts      (1001) docker     (121)    19448 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/modules/FindDotnet.cmake
--rw-r--r--   0 vsts      (1001) docker     (121)     1396 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/modules/FindGMP.cmake
--rw-r--r--   0 vsts      (1001) docker     (121)     8105 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/msvc_legacy_quirks.cmake
--rw-r--r--   0 vsts      (1001) docker     (121)      913 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/target_arch_detect.cmake
--rw-r--r--   0 vsts      (1001) docker     (121)      439 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/target_arch_detect.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15273 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/z3_add_component.cmake
--rw-r--r--   0 vsts      (1001) docker     (121)     1293 2022-07-06 16:51:51.671457 z3-solver-4.9.0.0/core/cmake/z3_add_cxx_flag.cmake
--rw-r--r--   0 vsts      (1001) docker     (121)      794 2022-07-06 16:51:51.675458 z3-solver-4.9.0.0/core/cmake/z3_append_linker_flag_list_to_target.cmake
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.479698 z3-solver-4.9.0.0/core/scripts/
--rw-r--r--   0 vsts      (1001) docker     (121)      391 2022-07-06 16:51:51.691458 z3-solver-4.9.0.0/core/scripts/README
--rw-r--r--   0 vsts      (1001) docker     (121)     3024 2022-07-06 16:51:51.691458 z3-solver-4.9.0.0/core/scripts/build-win-signed.yml
--rwxr-xr-x   0 vsts      (1001) docker     (121)      502 2022-07-06 16:51:51.691458 z3-solver-4.9.0.0/core/scripts/build_libcxx_msan.sh
--rw-r--r--   0 vsts      (1001) docker     (121)     1585 2022-07-06 16:51:51.691458 z3-solver-4.9.0.0/core/scripts/coverage.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      166 2022-07-06 16:51:51.691458 z3-solver-4.9.0.0/core/scripts/generate-doc.yml
--rwxr-xr-x   0 vsts      (1001) docker     (121)     2919 2022-07-06 16:51:51.691458 z3-solver-4.9.0.0/core/scripts/mk_consts_files.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1259 2022-07-06 16:51:51.691458 z3-solver-4.9.0.0/core/scripts/mk_copyright.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1024 2022-07-06 16:51:51.691458 z3-solver-4.9.0.0/core/scripts/mk_def_file.py
--rw-r--r--   0 vsts      (1001) docker     (121)      320 2022-07-06 16:51:51.691458 z3-solver-4.9.0.0/core/scripts/mk_exception.py
--rw-r--r--   0 vsts      (1001) docker     (121)    38118 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/mk_genfile_common.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1236 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/mk_gparams_register_modules_cpp.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1330 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/mk_install_tactic_cpp.py
--rw-r--r--   0 vsts      (1001) docker     (121)      487 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/mk_make.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1144 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/mk_mem_initializer_cpp.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4953 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/mk_nuget_task.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)      810 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/mk_pat_db.py
--rw-r--r--   0 vsts      (1001) docker     (121)     7181 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/mk_project.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8481 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/mk_unix_dist.py
--rw-r--r--   0 vsts      (1001) docker     (121)   143050 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/mk_util.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11676 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/mk_win_dist.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19831 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/nightly.yaml
--rw-r--r--   0 vsts      (1001) docker     (121)      172 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/policy.json
--rwxr-xr-x   0 vsts      (1001) docker     (121)     1100 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/pyg2hpp.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18423 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/release.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      359 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/test-examples-cmake.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      312 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/test-java-cmake.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      396 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/test-jupyter.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      250 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/test-regressions-coverage.yml
--rw-r--r--   0 vsts      (1001) docker     (121)      157 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/test-regressions.yml
--rw-r--r--   0 vsts      (1001) docker     (121)       59 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/test-z3.yml
--rwxr-xr-x   0 vsts      (1001) docker     (121)      353 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/trackall.sh
--rwxr-xr-x   0 vsts      (1001) docker     (121)    77489 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/update_api.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1792 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/update_header_guards.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1855 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/update_include.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)      351 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/vsts-mac.sh
--rw-r--r--   0 vsts      (1001) docker     (121)     1099 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/vsts-vs2013.cmd
--rw-r--r--   0 vsts      (1001) docker     (121)     1334 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/scripts/vsts-vs2017.cmd
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.479698 z3-solver-4.9.0.0/core/src/
--rw-r--r--   0 vsts      (1001) docker     (121)    10867 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/CMakeLists.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.479698 z3-solver-4.9.0.0/core/src/ackermannization/
--rw-r--r--   0 vsts      (1001) docker     (121)      501 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      284 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackermannization_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)      442 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackermannize_bv_model_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      372 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackermannize_bv_model_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2819 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackermannize_bv_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      407 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackermannize_bv_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)      347 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackermannize_bv_tactic_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     2470 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackr_bound_probe.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      478 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackr_bound_probe.h
--rw-r--r--   0 vsts      (1001) docker     (121)      709 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackr_helper.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4412 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackr_helper.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2969 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackr_info.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6840 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackr_model_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      445 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/ackr_model_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9095 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/lackr.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3970 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/lackr.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12716 2022-07-06 16:51:51.695458 z3-solver-4.9.0.0/core/src/ackermannization/lackr_model_constructor.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1475 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/ackermannization/lackr_model_constructor.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1606 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/ackermannization/lackr_model_converter_lazy.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      370 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/ackermannization/lackr_model_converter_lazy.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.483698 z3-solver-4.9.0.0/core/src/api/
--rw-r--r--   0 vsts      (1001) docker     (121)     1806 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    17278 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_algebraic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6608 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_arith.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12639 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_array.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    55592 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_ast.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4905 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_ast_map.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      783 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_ast_map.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4040 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_ast_vector.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      824 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_ast_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13894 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_bv.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3541 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_config_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    14520 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_context.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10275 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_context.h
--rw-r--r--   0 vsts      (1001) docker     (121)    25541 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_datalog.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1236 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_datalog.h
--rw-r--r--   0 vsts      (1001) docker     (121)    23225 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_datatype.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    47134 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_fpa.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6592 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_goal.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      682 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_goal.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4117 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_log.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    14637 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_model.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2033 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_model.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15502 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_numeral.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15556 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_opt.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6635 2022-07-06 16:51:51.699458 z3-solver-4.9.0.0/core/src/api/api_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9638 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_parsers.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3372 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_pb.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2074 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_polynomial.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      596 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_polynomial.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4650 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_qe.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    19880 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_quant.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8792 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_rcf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12498 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_seq.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    36750 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2510 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_special_relations.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3722 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_stats.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      679 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_stats.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16605 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1700 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7619 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/api_util.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.483698 z3-solver-4.9.0.0/core/src/api/c++/
--rw-r--r--   0 vsts      (1001) docker     (121)   180390 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/c++/z3++.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.483698 z3-solver-4.9.0.0/core/src/api/dll/
--rw-r--r--   0 vsts      (1001) docker     (121)      447 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/dll/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      544 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/dll/dll.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.487698 z3-solver-4.9.0.0/core/src/api/dotnet/
--rw-r--r--   0 vsts      (1001) docker     (121)     7896 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/dotnet/AST.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     4190 2022-07-06 16:51:51.703458 z3-solver-4.9.0.0/core/src/api/dotnet/ASTMap.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     7953 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/ASTVector.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     2160 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/AlgebraicNum.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     2465 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/ApplyResult.cs
--rw-r--r--   0 vsts      (1001) docker     (121)    10533 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/ArithExpr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      546 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/ArithSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     1073 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/ArrayExpr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     1735 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/ArraySort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      876 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/BitVecExpr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     2982 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/BitVecNum.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      748 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/BitVecSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     1348 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/BoolExpr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      635 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/BoolSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     5890 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      641 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/CharSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     3779 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/Constructor.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     1205 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/ConstructorList.cs
--rw-r--r--   0 vsts      (1001) docker     (121)   183926 2022-07-06 16:51:51.707458 z3-solver-4.9.0.0/core/src/api/dotnet/Context.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      721 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/DatatypeExpr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     2950 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/DatatypeSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      553 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Deprecated.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     3652 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/EnumSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)    81752 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Expr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     1021 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/FPExpr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     6309 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/FPNum.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      747 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/FPRMExpr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     3709 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/FPRMNum.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      754 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/FPRMSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     1132 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/FPSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      666 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/FiniteDomainExpr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     2734 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/FiniteDomainNum.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     1195 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/FiniteDomainSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)    11689 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Fixedpoint.cs
--rw-r--r--   0 vsts      (1001) docker     (121)    13050 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/FuncDecl.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     6359 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/FuncInterp.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     4099 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Global.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     8839 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Goal.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     2243 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/IDecRefQueue.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      694 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/IntExpr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     2734 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/IntNum.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      714 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/IntSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     1546 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/IntSymbol.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     4341 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Lambda.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     3338 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/ListSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     1849 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Log.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      209 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Microsoft.Z3.Sharp.pc.in
--rw-r--r--   0 vsts      (1001) docker     (121)     3964 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Microsoft.Z3.csproj.in
--rw-r--r--   0 vsts      (1001) docker     (121)     1543 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Microsoft.Z3.props
--rw-r--r--   0 vsts      (1001) docker     (121)      596 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Microsoft.Z3.snk
--rw-r--r--   0 vsts      (1001) docker     (121)      477 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Microsoft.Z3.targets
--rw-r--r--   0 vsts      (1001) docker     (121)      423 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Microsoft.Z3.targets.in
--rw-r--r--   0 vsts      (1001) docker     (121)    11842 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Model.cs
--rw-r--r--   0 vsts      (1001) docker     (121)    48516 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/NativeContext.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     2975 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/NativeFuncInterp.cs
--rw-r--r--   0 vsts      (1001) docker     (121)    13104 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/NativeModel.cs
--rw-r--r--   0 vsts      (1001) docker     (121)    16054 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/NativeSolver.cs
--rw-r--r--   0 vsts      (1001) docker     (121)    14906 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Optimize.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     3339 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/ParamDescrs.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     5002 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Params.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     1635 2022-07-06 16:51:51.711458 z3-solver-4.9.0.0/core/src/api/dotnet/Pattern.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     2649 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/Probe.cs
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.487698 z3-solver-4.9.0.0/core/src/api/dotnet/Properties/
--rw-r--r--   0 vsts      (1001) docker     (121)     1605 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/Properties/AssemblyInfo.cs.in
--rw-r--r--   0 vsts      (1001) docker     (121)     9040 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/Quantifier.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     2733 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/RatNum.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      706 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/ReExpr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      730 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/ReSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      702 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/RealExpr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      715 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/RealSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     1391 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/RelationSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      885 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/SeqExpr.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      560 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/SeqSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      767 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/SetSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)    18335 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/Solver.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     5399 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/Sort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     6270 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/Statistics.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      663 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/Status.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     1593 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/StringSymbol.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     3538 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/Symbol.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     3670 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/Tactic.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     2018 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/TupleSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      835 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/UninterpretedSort.cs
--rw-r--r--   0 vsts      (1001) docker     (121)    11525 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/UserPropagator.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     2578 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/Version.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      817 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/Z3Exception.cs
--rw-r--r--   0 vsts      (1001) docker     (121)     3270 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/Z3Object.cs
--rw-r--r--   0 vsts      (1001) docker     (121)      535 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/cmake_install_gac.cmake.in
--rw-r--r--   0 vsts      (1001) docker     (121)      653 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/dotnet/cmake_uninstall_gac.cmake.in
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.491698 z3-solver-4.9.0.0/core/src/api/java/
--rw-r--r--   0 vsts      (1001) docker     (121)     5055 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/AST.java
--rw-r--r--   0 vsts      (1001) docker     (121)      437 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/ASTDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)     2739 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/ASTMap.java
--rw-r--r--   0 vsts      (1001) docker     (121)     6162 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/ASTVector.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1844 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/AlgebraicNum.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1531 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/ApplyResult.java
--rw-r--r--   0 vsts      (1001) docker     (121)      480 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/ApplyResultDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)      444 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/ArithExpr.java
--rw-r--r--   0 vsts      (1001) docker     (121)      376 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/ArithSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)      454 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/ArrayExpr.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1405 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/ArraySort.java
--rw-r--r--   0 vsts      (1001) docker     (121)      454 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/AstMapDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)      469 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/AstVectorDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)      672 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/BitVecExpr.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1682 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/BitVecNum.java
--rw-r--r--   0 vsts      (1001) docker     (121)      588 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/BitVecSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)      477 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/BoolExpr.java
--rw-r--r--   0 vsts      (1001) docker     (121)      415 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/BoolSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)     7013 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      431 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/CharSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)     3401 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/Constructor.java
--rw-r--r--   0 vsts      (1001) docker     (121)      285 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/ConstructorDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)      845 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/ConstructorList.java
--rw-r--r--   0 vsts      (1001) docker     (121)      301 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/ConstructorListDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)   136585 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/Context.java
--rw-r--r--   0 vsts      (1001) docker     (121)      452 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/DatatypeExpr.java
--rw-r--r--   0 vsts      (1001) docker     (121)     2806 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/DatatypeSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)     2999 2022-07-06 16:51:51.715458 z3-solver-4.9.0.0/core/src/api/java/EnumSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)    68960 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Expr.java
--rw-r--r--   0 vsts      (1001) docker     (121)      664 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FPExpr.java
--rw-r--r--   0 vsts      (1001) docker     (121)     5633 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FPNum.java
--rw-r--r--   0 vsts      (1001) docker     (121)      381 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FPRMExpr.java
--rw-r--r--   0 vsts      (1001) docker     (121)     3127 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FPRMNum.java
--rw-r--r--   0 vsts      (1001) docker     (121)      479 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FPRMSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)      847 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FPSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)      501 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FiniteDomainExpr.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1429 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FiniteDomainNum.java
--rw-r--r--   0 vsts      (1001) docker     (121)      854 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FiniteDomainSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)     9854 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Fixedpoint.java
--rw-r--r--   0 vsts      (1001) docker     (121)      480 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FixedpointDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)    10469 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FuncDecl.java
--rw-r--r--   0 vsts      (1001) docker     (121)     4865 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FuncInterp.java
--rw-r--r--   0 vsts      (1001) docker     (121)      479 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FuncInterpDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)      497 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/FuncInterpEntryDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)     3180 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Global.java
--rw-r--r--   0 vsts      (1001) docker     (121)     6652 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Goal.java
--rw-r--r--   0 vsts      (1001) docker     (121)      449 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/GoalDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)     2366 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/IDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)      445 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/IntExpr.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1339 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/IntNum.java
--rw-r--r--   0 vsts      (1001) docker     (121)      440 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/IntSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1143 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/IntSymbol.java
--rw-r--r--   0 vsts      (1001) docker     (121)     3172 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Lambda.java
--rw-r--r--   0 vsts      (1001) docker     (121)     2575 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/ListSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1450 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Log.java
--rw-r--r--   0 vsts      (1001) docker     (121)     9203 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Model.java
--rw-r--r--   0 vsts      (1001) docker     (121)      450 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/ModelDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)     3230 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/NativeStatic.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    12035 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Optimize.java
--rw-r--r--   0 vsts      (1001) docker     (121)      466 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/OptimizeDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)     2263 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/ParamDescrs.java
--rw-r--r--   0 vsts      (1001) docker     (121)      484 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/ParamDescrsDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)     3202 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Params.java
--rw-r--r--   0 vsts      (1001) docker     (121)      454 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/ParamsDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1246 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Pattern.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1483 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Probe.java
--rw-r--r--   0 vsts      (1001) docker     (121)      455 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/ProbeDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)     7951 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Quantifier.java
--rw-r--r--   0 vsts      (1001) docker     (121)      234 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/README
--rw-r--r--   0 vsts      (1001) docker     (121)     1809 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/RatNum.java
--rw-r--r--   0 vsts      (1001) docker     (121)      453 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/ReExpr.java
--rw-r--r--   0 vsts      (1001) docker     (121)      370 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/ReSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)      415 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/RealExpr.java
--rw-r--r--   0 vsts      (1001) docker     (121)      441 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/RealSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1053 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/RelationSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)      459 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/SeqExpr.java
--rw-r--r--   0 vsts      (1001) docker     (121)      364 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/SeqSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)      492 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/SetSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)    11277 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Solver.java
--rw-r--r--   0 vsts      (1001) docker     (121)      442 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/SolverDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)     3718 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Sort.java
--rw-r--r--   0 vsts      (1001) docker     (121)     4611 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Statistics.java
--rw-r--r--   0 vsts      (1001) docker     (121)      470 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/StatisticsDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)      797 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Status.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1086 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/StringSymbol.java
--rw-r--r--   0 vsts      (1001) docker     (121)     2317 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Symbol.java
--rw-r--r--   0 vsts      (1001) docker     (121)     2543 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Tactic.java
--rw-r--r--   0 vsts      (1001) docker     (121)      459 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/TacticDecRefQueue.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1509 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/TupleSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)      520 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/UninterpretedSort.java
--rw-r--r--   0 vsts      (1001) docker     (121)     2221 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Version.java
--rw-r--r--   0 vsts      (1001) docker     (121)      702 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Z3Exception.java
--rw-r--r--   0 vsts      (1001) docker     (121)     1758 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/Z3Object.java
--rw-r--r--   0 vsts      (1001) docker     (121)       66 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/java/manifest
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.491698 z3-solver-4.9.0.0/core/src/api/js/
--rw-r--r--   0 vsts      (1001) docker     (121)        9 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/js/.nvmrc
--rw-r--r--   0 vsts      (1001) docker     (121)       99 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/js/.prettierrc.json
--rw-r--r--   0 vsts      (1001) docker     (121)     7690 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/js/PUBLISHED_README.md
--rw-r--r--   0 vsts      (1001) docker     (121)      890 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/js/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.467697 z3-solver-4.9.0.0/core/src/api/js/examples/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.491698 z3-solver-4.9.0.0/core/src/api/js/examples/high-level/
--rw-r--r--   0 vsts      (1001) docker     (121)     5915 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/js/examples/high-level/miracle-sudoku.ts
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.491698 z3-solver-4.9.0.0/core/src/api/js/examples/low-level/
--rw-r--r--   0 vsts      (1001) docker     (121)     2205 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/js/examples/low-level/example-raw.ts
--rw-r--r--   0 vsts      (1001) docker     (121)    12715 2022-07-06 16:51:51.719458 z3-solver-4.9.0.0/core/src/api/js/examples/low-level/test-ts-api.ts
--rw-r--r--   0 vsts      (1001) docker     (121)      180 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/jest.config.js
--rw-r--r--   0 vsts      (1001) docker     (121)   410653 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/package-lock.json
--rw-r--r--   0 vsts      (1001) docker     (121)     1738 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/package.json
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.491698 z3-solver-4.9.0.0/core/src/api/js/scripts/
--rw-r--r--   0 vsts      (1001) docker     (121)      570 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/scripts/async-fns.ts
--rw-r--r--   0 vsts      (1001) docker     (121)     3207 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/scripts/build-wasm.ts
--rw-r--r--   0 vsts      (1001) docker     (121)     3051 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/scripts/make-cc-wrapper.ts
--rw-r--r--   0 vsts      (1001) docker     (121)    15968 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/scripts/make-ts-wrapper.ts
--rw-r--r--   0 vsts      (1001) docker     (121)    12210 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/scripts/parse-api.ts
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.491698 z3-solver-4.9.0.0/core/src/api/js/src/
--rw-r--r--   0 vsts      (1001) docker     (121)      645 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/src/browser.ts
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.491698 z3-solver-4.9.0.0/core/src/api/js/src/high-level/
--rw-r--r--   0 vsts      (1001) docker     (121)    14054 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/src/high-level/high-level.test.ts
--rw-r--r--   0 vsts      (1001) docker     (121)    64773 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/src/high-level/high-level.ts
--rw-r--r--   0 vsts      (1001) docker     (121)       55 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/src/high-level/index.ts
--rw-r--r--   0 vsts      (1001) docker     (121)    32381 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/src/high-level/types.ts
--rw-r--r--   0 vsts      (1001) docker     (121)     1653 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/src/high-level/utils.test.ts
--rw-r--r--   0 vsts      (1001) docker     (121)     1568 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/src/high-level/utils.ts
--rw-r--r--   0 vsts      (1001) docker     (121)     2219 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/src/jest.ts
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.491698 z3-solver-4.9.0.0/core/src/api/js/src/low-level/
--rw-r--r--   0 vsts      (1001) docker     (121)      963 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/src/low-level/async-wrapper.js
--rw-r--r--   0 vsts      (1001) docker     (121)      274 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/src/low-level/index.ts
--rw-r--r--   0 vsts      (1001) docker     (121)     1110 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/src/node.ts
--rw-r--r--   0 vsts      (1001) docker     (121)       85 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/tsconfig.build.json
--rw-r--r--   0 vsts      (1001) docker     (121)      354 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/tsconfig.json
--rw-r--r--   0 vsts      (1001) docker     (121)      230 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/js/typedoc.json
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.491698 z3-solver-4.9.0.0/core/src/api/julia/
--rw-r--r--   0 vsts      (1001) docker     (121)      603 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/julia/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1684 2022-07-06 16:51:51.723458 z3-solver-4.9.0.0/core/src/api/julia/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)    32294 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/julia/z3jl.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.491698 z3-solver-4.9.0.0/core/src/api/ml/
--rw-r--r--   0 vsts      (1001) docker     (121)      360 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/ml/META.in
--rw-r--r--   0 vsts      (1001) docker     (121)     9627 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/ml/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)    87711 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/ml/z3.ml
--rw-r--r--   0 vsts      (1001) docker     (121)   130000 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/ml/z3.mli
--rw-r--r--   0 vsts      (1001) docker     (121)      731 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/ml/z3native.ml.pre
--rw-r--r--   0 vsts      (1001) docker     (121)    19862 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/ml/z3native_stubs.c.pre
--rw-r--r--   0 vsts      (1001) docker     (121)      514 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/ml/z3native_stubs.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.495698 z3-solver-4.9.0.0/core/src/api/python/
--rw-r--r--   0 vsts      (1001) docker     (121)       58 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/python/.gitignore
--rw-r--r--   0 vsts      (1001) docker     (121)     5741 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/python/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      509 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/python/README.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      107 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/python/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.495698 z3-solver-4.9.0.0/core/src/api/python/z3/
--rw-r--r--   0 vsts      (1001) docker     (121)      210 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/core/src/api/python/z3/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)   329080 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/python/z3/z3.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16090 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/python/z3/z3num.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1113 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/python/z3/z3poly.py
--rw-r--r--   0 vsts      (1001) docker     (121)    45224 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/python/z3/z3printer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5039 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/python/z3/z3rcf.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4723 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/python/z3/z3types.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11388 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/python/z3/z3util.py
--rw-r--r--   0 vsts      (1001) docker     (121)      464 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/python/z3test.py
--rw-r--r--   0 vsts      (1001) docker     (121)      514 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7193 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_algebraic.h
--rw-r--r--   0 vsts      (1001) docker     (121)   255570 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_api.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5735 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_ast_containers.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14123 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_fixedpoint.h
--rw-r--r--   0 vsts      (1001) docker     (121)    36516 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_fpa.h
--rw-r--r--   0 vsts      (1001) docker     (121)      462 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_logger.h
--rw-r--r--   0 vsts      (1001) docker     (121)      377 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_macros.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12312 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_optimization.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1056 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_polynomial.h
--rw-r--r--   0 vsts      (1001) docker     (121)      450 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_private.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5976 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_rcf.h
--rw-r--r--   0 vsts      (1001) docker     (121)    26456 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_replayer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1581 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_replayer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3901 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_spacer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2220 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/api/z3_v1.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.499698 z3-solver-4.9.0.0/core/src/ast/
--rw-r--r--   0 vsts      (1001) docker     (121)     1205 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/ast/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     5965 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/ast/act_cache.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1488 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/ast/act_cache.h
--rw-r--r--   0 vsts      (1001) docker     (121)    33929 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/core/src/ast/arith_decl_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    24406 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/arith_decl_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)    28544 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/array_decl_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10353 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/array_decl_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)   123605 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)   105176 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9776 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_ll_pp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1527 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_ll_pp.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6603 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_lt.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      765 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_lt.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1665 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_pp.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4075 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_pp_dot.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      591 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_pp_dot.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3097 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_pp_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1501 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_pp_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2243 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_printer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1671 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_printer.h
--rw-r--r--   0 vsts      (1001) docker     (121)    49621 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_smt2_pp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6593 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_smt2_pp.h
--rw-r--r--   0 vsts      (1001) docker     (121)    29730 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_smt_pp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3466 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_smt_pp.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1288 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_trail.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13671 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_translation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3748 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_translation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11327 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5725 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/ast_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)    34774 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/bv_decl_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    21372 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/bv_decl_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7078 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/char_decl_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2825 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/char_decl_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3020 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/cost_evaluator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      800 2022-07-06 16:51:51.735458 z3-solver-4.9.0.0/core/src/ast/cost_evaluator.h
--rw-r--r--   0 vsts      (1001) docker     (121)    57058 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/datatype_decl_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    19278 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/datatype_decl_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5599 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/decl_collector.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1855 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/decl_collector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4529 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/display_dimacs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/display_dimacs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    28780 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/dl_decl_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6338 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/dl_decl_plugin.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.499698 z3-solver-4.9.0.0/core/src/ast/euf/
--rw-r--r--   0 vsts      (1001) docker     (121)      131 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/euf/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    36230 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/euf/euf_egraph.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15564 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/euf/euf_egraph.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4425 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/euf/euf_enode.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12317 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/euf/euf_enode.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8226 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/euf/euf_etable.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5421 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/euf/euf_etable.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2540 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/euf/euf_justification.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15998 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr2polynomial.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3235 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr2polynomial.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2733 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr2var.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1966 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr2var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4388 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr_abstract.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1537 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr_abstract.h
--rw-r--r--   0 vsts      (1001) docker     (121)      700 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr_delta_pair.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3370 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr_functors.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2451 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr_functors.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2186 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr_map.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1465 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr_map.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2119 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr_stat.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      978 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr_stat.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4681 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr_substitution.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3234 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/expr_substitution.h
--rw-r--r--   0 vsts      (1001) docker     (121)      898 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/for_each_ast.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8973 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/for_each_ast.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4906 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/for_each_expr.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6721 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/for_each_expr.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7005 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/format.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7350 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/format.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.499698 z3-solver-4.9.0.0/core/src/ast/fpa/
--rw-r--r--   0 vsts      (1001) docker     (121)      172 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/fpa/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    21618 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/fpa/bv2fpa_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2197 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/fpa/bv2fpa_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)   170799 2022-07-06 16:51:51.739458 z3-solver-4.9.0.0/core/src/ast/fpa/fpa2bv_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12084 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/fpa/fpa2bv_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13835 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/fpa/fpa2bv_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2135 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/fpa/fpa2bv_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    47947 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/fpa_decl_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    17510 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/fpa_decl_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6003 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/func_decl_dependencies.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2815 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/func_decl_dependencies.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2656 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/has_free_vars.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      385 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/has_free_vars.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1379 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/is_variable_test.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1365 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/justified_expr.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5229 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macro_substitution.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1719 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macro_substitution.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.499698 z3-solver-4.9.0.0/core/src/ast/macros/
--rw-r--r--   0 vsts      (1001) docker     (121)      187 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macros/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1810 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macros/cond_macro.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15685 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macros/macro_finder.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1724 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macros/macro_finder.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13607 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macros/macro_manager.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3365 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macros/macro_manager.h
--rw-r--r--   0 vsts      (1001) docker     (121)    32646 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macros/macro_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6067 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macros/macro_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1962 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macros/quantifier_macro_info.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macros/quantifier_macro_info.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13246 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macros/quasi_macros.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2135 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/macros/quasi_macros.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.503698 z3-solver-4.9.0.0/core/src/ast/normal_forms/
--rw-r--r--   0 vsts      (1001) docker     (121)      247 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/normal_forms/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    13210 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/normal_forms/defined_names.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2622 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/normal_forms/defined_names.h
--rw-r--r--   0 vsts      (1001) docker     (121)      892 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/normal_forms/elim_term_ite.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1484 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/normal_forms/elim_term_ite.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4508 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/normal_forms/name_exprs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1700 2022-07-06 16:51:51.743458 z3-solver-4.9.0.0/core/src/ast/normal_forms/name_exprs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    30976 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/normal_forms/nnf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1155 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/normal_forms/nnf.h
--rw-r--r--   0 vsts      (1001) docker     (121)      571 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/normal_forms/nnf_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)    15547 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/normal_forms/pull_quant.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1092 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/normal_forms/pull_quant.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2157 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/num_occurs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1113 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/num_occurs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1353 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/occurs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      397 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/occurs.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.503698 z3-solver-4.9.0.0/core/src/ast/pattern/
--rw-r--r--   0 vsts      (1001) docker     (121)     1119 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/pattern/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    15504 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/pattern/database.smt2
--rw-r--r--   0 vsts      (1001) docker     (121)    14917 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/pattern/expr_pattern_match.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3875 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/pattern/expr_pattern_match.h
--rw-r--r--   0 vsts      (1001) docker     (121)    26717 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/pattern/pattern_inference.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8587 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/pattern/pattern_inference.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9506 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/pb_decl_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4971 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/pb_decl_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4405 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/pp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      349 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/pp.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2110 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/pp_params.pyg
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.503698 z3-solver-4.9.0.0/core/src/ast/proofs/
--rw-r--r--   0 vsts      (1001) docker     (121)      115 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/proofs/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    44936 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/proofs/proof_checker.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4486 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/proofs/proof_checker.h
--rw-r--r--   0 vsts      (1001) docker     (121)    32840 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/proofs/proof_utils.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7464 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/proofs/proof_utils.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3770 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/quantifier_stat.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4164 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/quantifier_stat.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22084 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/recfun_decl_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    14167 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/recfun_decl_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1173 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/recurse_expr.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3414 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/recurse_expr_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2218 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/reg_decl_plugins.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      332 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/reg_decl_plugins.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.507698 z3-solver-4.9.0.0/core/src/ast/rewriter/
--rw-r--r--   0 vsts      (1001) docker     (121)      991 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/rewriter/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    70741 2022-07-06 16:51:51.747458 z3-solver-4.9.0.0/core/src/ast/rewriter/arith_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8245 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/arith_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    27948 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/array_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3306 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/array_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3632 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/ast_counter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2382 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/ast_counter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12556 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bit2int.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2158 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bit2int.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.507698 z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/
--rw-r--r--   0 vsts      (1001) docker     (121)      139 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     4070 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/bit_blaster.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2336 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/bit_blaster.h
--rw-r--r--   0 vsts      (1001) docker     (121)    27664 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/bit_blaster_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1031 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/bit_blaster_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7574 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/bit_blaster_tpl.h
--rw-r--r--   0 vsts      (1001) docker     (121)    40789 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/bit_blaster_tpl_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)    34233 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bool_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9447 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bool_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    26718 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bv_bounds.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4539 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bv_bounds.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3524 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bv_elim.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      992 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bv_elim.h
--rw-r--r--   0 vsts      (1001) docker     (121)    93415 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bv_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    11021 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/bv_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2799 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/cached_var_subst.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1210 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/cached_var_subst.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2671 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/char_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1349 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/char_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4813 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/datatype_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      710 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/datatype_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12301 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/der.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6590 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/der.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4480 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/distribute_forall.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1956 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/distribute_forall.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1351 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/dl_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      583 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/dl_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5648 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/elim_bounds.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1814 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/elim_bounds.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12570 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/enum2bv_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1074 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/enum2bv_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4284 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/expr_replacer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1463 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/expr_replacer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5727 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/expr_safe_replace.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      939 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/expr_safe_replace.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3787 2022-07-06 16:51:51.751458 z3-solver-4.9.0.0/core/src/ast/rewriter/factor_equivs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5146 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/factor_equivs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10477 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/factor_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2286 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/factor_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    28725 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/fpa_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3795 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/fpa_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2619 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/func_decl_replace.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      794 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/func_decl_replace.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5586 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/hoist_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2571 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/hoist_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5533 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/inj_axiom.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      299 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/inj_axiom.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1103 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/label_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      682 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/label_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4574 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/maximize_ac_sharing.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3282 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/maximize_ac_sharing.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1181 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/mk_extract_proc.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      620 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/mk_extract_proc.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3490 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/mk_simplified_app.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      674 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/mk_simplified_app.h
--rw-r--r--   0 vsts      (1001) docker     (121)    43649 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/pb2bv_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1018 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/pb2bv_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9464 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/pb_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1680 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/pb_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8357 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/pb_rewriter_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6452 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/poly_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    36735 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/poly_rewriter_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2681 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/push_app_ite.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2067 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/push_app_ite.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11514 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/quant_hoist.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2017 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/quant_hoist.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1002 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/recfun_replace.h
--rw-r--r--   0 vsts      (1001) docker     (121)      900 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/recfun_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      604 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/recfun_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11498 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15309 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5573 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/rewriter.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    29732 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/rewriter_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1305 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/rewriter_types.h
--rw-r--r--   0 vsts      (1001) docker     (121)    46242 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/seq_axioms.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4469 2022-07-06 16:51:51.755458 z3-solver-4.9.0.0/core/src/ast/rewriter/seq_axioms.h
--rw-r--r--   0 vsts      (1001) docker     (121)    23309 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/rewriter/seq_eq_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6280 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/rewriter/seq_eq_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)   199846 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/rewriter/seq_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    18897 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/rewriter/seq_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6583 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/rewriter/seq_skolem.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10213 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/rewriter/seq_skolem.h
--rw-r--r--   0 vsts      (1001) docker     (121)    35818 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/rewriter/th_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1904 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/rewriter/th_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4058 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/rewriter/value_sweep.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1575 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/rewriter/value_sweep.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9032 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/rewriter/var_subst.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3467 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/rewriter/var_subst.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1005 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/scoped_proof.h
--rw-r--r--   0 vsts      (1001) docker     (121)    64489 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/seq_decl_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    28118 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/seq_decl_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3562 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/shared_occs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2102 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/shared_occs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2609 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/special_relations_decl_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4469 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/special_relations_decl_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)    24694 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/static_features.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9198 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/static_features.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.507698 z3-solver-4.9.0.0/core/src/ast/substitution/
--rw-r--r--   0 vsts      (1001) docker     (121)      167 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/substitution/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1351 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/substitution/expr_offset.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2457 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/substitution/expr_offset_map.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1738 2022-07-06 16:51:51.759458 z3-solver-4.9.0.0/core/src/ast/substitution/matcher.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1297 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/substitution/matcher.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11632 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/substitution/substitution.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7339 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/substitution/substitution.h
--rw-r--r--   0 vsts      (1001) docker     (121)    28561 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/substitution/substitution_tree.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4273 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/substitution/substitution_tree.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5112 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/substitution/unifier.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1817 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/substitution/unifier.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2923 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/substitution/var_offset_map.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3000 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/used_symbols.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3267 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/used_vars.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1426 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/used_vars.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11738 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/value_generator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      744 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/value_generator.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2871 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/well_sorted.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      288 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/ast/well_sorted.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.511698 z3-solver-4.9.0.0/core/src/cmd_context/
--rw-r--r--   0 vsts      (1001) docker     (121)      323 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      190 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/README
--rw-r--r--   0 vsts      (1001) docker     (121)    36300 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/basic_cmds.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      314 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/basic_cmds.h
--rw-r--r--   0 vsts      (1001) docker     (121)    75767 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/cmd_context.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    23447 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/cmd_context.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1470 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/cmd_context_to_goal.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      317 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/cmd_context_to_goal.h
--rw-r--r--   0 vsts      (1001) docker     (121)      877 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/cmd_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3575 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/cmd_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1905 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/echo_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      495 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/echo_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2913 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/eval_cmd.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      237 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/eval_cmd.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.511698 z3-solver-4.9.0.0/core/src/cmd_context/extra_cmds/
--rw-r--r--   0 vsts      (1001) docker     (121)      184 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/extra_cmds/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    21125 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/extra_cmds/dbg_cmds.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      275 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/extra_cmds/dbg_cmds.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8058 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/extra_cmds/polynomial_cmds.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      282 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/extra_cmds/polynomial_cmds.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1591 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/extra_cmds/subpaving_cmds.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      266 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/extra_cmds/subpaving_cmds.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1583 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/parametric_cmd.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2501 2022-07-06 16:51:51.763458 z3-solver-4.9.0.0/core/src/cmd_context/parametric_cmd.h
--rw-r--r--   0 vsts      (1001) docker     (121)    36727 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/cmd_context/pdecl.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    16022 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/cmd_context/pdecl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4841 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/cmd_context/simplify_cmd.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      306 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/cmd_context/simplify_cmd.h
--rw-r--r--   0 vsts      (1001) docker     (121)    35506 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/cmd_context/tactic_cmds.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1340 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/cmd_context/tactic_cmds.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1336 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/cmd_context/tactic_manager.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2151 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/cmd_context/tactic_manager.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.471697 z3-solver-4.9.0.0/core/src/math/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.511698 z3-solver-4.9.0.0/core/src/math/automata/
--rw-r--r--   0 vsts      (1001) docker     (121)       90 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/automata/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      306 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/automata/automaton.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    25355 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/automata/automaton.h
--rw-r--r--   0 vsts      (1001) docker     (121)      800 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/automata/boolean_algebra.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4668 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/automata/symbolic_automata.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16582 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/automata/symbolic_automata_def.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.511698 z3-solver-4.9.0.0/core/src/math/dd/
--rw-r--r--   0 vsts      (1001) docker     (121)       96 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/dd/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    28871 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/dd/dd_bdd.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9224 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/dd/dd_bdd.h
--rw-r--r--   0 vsts      (1001) docker     (121)    44595 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/dd/dd_pdd.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    17301 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/dd/dd_pdd.h
--rw-r--r--   0 vsts      (1001) docker     (121)      809 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/dd/pdd_eval.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1720 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/dd/pdd_interval.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.511698 z3-solver-4.9.0.0/core/src/math/grobner/
--rw-r--r--   0 vsts      (1001) docker     (121)      147 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/grobner/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    30190 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/grobner/grobner.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9167 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/grobner/grobner.h
--rw-r--r--   0 vsts      (1001) docker     (121)    23259 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/grobner/pdd_simplifier.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1305 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/grobner/pdd_simplifier.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16848 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/grobner/pdd_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6947 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/grobner/pdd_solver.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.511698 z3-solver-4.9.0.0/core/src/math/hilbert/
--rw-r--r--   0 vsts      (1001) docker     (121)       93 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/hilbert/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    20941 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/hilbert/heap_trie.h
--rw-r--r--   0 vsts      (1001) docker     (121)    36737 2022-07-06 16:51:51.767458 z3-solver-4.9.0.0/core/src/math/hilbert/hilbert_basis.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7091 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/hilbert/hilbert_basis.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.511698 z3-solver-4.9.0.0/core/src/math/interval/
--rw-r--r--   0 vsts      (1001) docker     (121)      115 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/interval/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      321 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/interval/README
--rw-r--r--   0 vsts      (1001) docker     (121)     3933 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/interval/dep_intervals.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    16433 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/interval/dep_intervals.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15040 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/interval/interval.h
--rw-r--r--   0 vsts      (1001) docker     (121)    70016 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/interval/interval_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)      308 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/interval/interval_mpq.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.519698 z3-solver-4.9.0.0/core/src/math/lp/
--rw-r--r--   0 vsts      (1001) docker     (121)     1209 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1698 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/binary_heap_priority_queue.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2332 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/binary_heap_priority_queue.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6386 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/binary_heap_priority_queue_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1100 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/binary_heap_upair_queue.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1547 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/binary_heap_upair_queue.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3506 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/binary_heap_upair_queue_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10018 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/bound_analyzer_on_row.h
--rw-r--r--   0 vsts      (1001) docker     (121)      505 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/breakpoint.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6918 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/column_info.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1518 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/column_namer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1477 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/conversion_helper.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1281 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/core_solver_pretty_printer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3242 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/core_solver_pretty_printer.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14950 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/core_solver_pretty_printer_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18072 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/cross_nested.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2192 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/dense_matrix.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2960 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/dense_matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5668 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/dense_matrix_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17506 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/emonics.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12694 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/emonics.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2294 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/eta_matrix.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2393 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/eta_matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4168 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/eta_matrix_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3260 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/explanation.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3986 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/factorization.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4525 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/factorization.h
--rw-r--r--   0 vsts      (1001) docker     (121)      910 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/factorization_factory_imp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      724 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/factorization_factory_imp.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8115 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/general_matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15490 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/gomory.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      766 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/gomory.h
--rw-r--r--   0 vsts      (1001) docker     (121)    19154 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/hnf.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10406 2022-07-06 16:51:51.771458 z3-solver-4.9.0.0/core/src/math/lp/hnf_cutter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2627 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/hnf_cutter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3821 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/horner.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1284 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/horner.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1445 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/implied_bound.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1451 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/incremental_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1180 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/indexed_value.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2334 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/indexed_vector.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5616 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/indexed_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2685 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/indexed_vector_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)      839 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/indexer_of_constraints.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3116 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/int_branch.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      636 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/int_branch.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3511 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/int_cube.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      803 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/int_cube.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11113 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/int_gcd_test.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2115 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/int_gcd_test.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17815 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/int_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4251 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/int_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10490 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lar_constraints.h
--rw-r--r--   0 vsts      (1001) docker     (121)      307 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lar_core_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    30779 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lar_core_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7398 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lar_core_solver_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)      396 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lar_solution_signature.h
--rw-r--r--   0 vsts      (1001) docker     (121)    96890 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lar_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    32882 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lar_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5755 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lar_term.h
--rw-r--r--   0 vsts      (1001) docker     (121)      856 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lia_move.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4365 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lp_api.h
--rw-r--r--   0 vsts      (1001) docker     (121)    28057 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lp_bound_propagator.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13646 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lp_core_solver_base.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    25854 2022-07-06 16:51:51.775458 z3-solver-4.9.0.0/core/src/math/lp/lp_core_solver_base.h
--rw-r--r--   0 vsts      (1001) docker     (121)    34703 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_core_solver_base_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2037 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_dual_core_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6155 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_dual_core_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    26448 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_dual_core_solver_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)      520 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_dual_simplex.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2404 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_dual_simplex.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14952 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_dual_simplex_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1460 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_primal_core_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    39887 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_primal_core_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    52683 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_primal_core_solver_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16142 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_primal_core_solver_tableau_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1416 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_primal_simplex.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2660 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_primal_simplex.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13929 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_primal_simplex_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)      937 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_settings.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15166 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_settings.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3507 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_settings_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3093 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7834 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    19603 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_solver_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2413 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_types.h
--rw-r--r--   0 vsts      (1001) docker     (121)      325 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_utils.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6713 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lp_utils.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5522 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lu.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12164 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lu.h
--rw-r--r--   0 vsts      (1001) docker     (121)    32619 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/lu_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)      995 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/matrix.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1683 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3582 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/matrix_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1050 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/mon_eq.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3137 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/monic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9946 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/monomial_bounds.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1126 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/monomial_bounds.h
--rw-r--r--   0 vsts      (1001) docker     (121)    29718 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/mps_reader.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13857 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/nex.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20843 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/nex_creator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9050 2022-07-06 16:51:51.779458 z3-solver-4.9.0.0/core/src/math/lp/nex_creator.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22817 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_basics_lemmas.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4217 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_basics_lemmas.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4660 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_common.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3241 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_common.h
--rw-r--r--   0 vsts      (1001) docker     (121)    62349 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_core.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    19818 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_core.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2636 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_defs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17097 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_intervals.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4291 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_intervals.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2477 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_monotone_lemmas.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      572 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_monotone_lemmas.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13718 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_order_lemmas.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2767 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_order_lemmas.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4134 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_settings.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1665 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1096 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7050 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_tangent_lemmas.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1045 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nla_tangent_lemmas.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9080 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nra_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1089 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/nra_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13508 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/numeric_pair.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5639 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/permutation_matrix.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4579 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/permutation_matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10044 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/permutation_matrix_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)      205 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/random_updater.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      887 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/random_updater.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2059 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/random_updater_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2367 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/row_eta_matrix.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2269 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/row_eta_matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5521 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/row_eta_matrix_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)      300 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/scaler.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2037 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/scaler.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8195 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/scaler_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)      947 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/sparse_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2939 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/square_dense_submatrix.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7152 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/square_dense_submatrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13206 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/square_dense_submatrix_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10910 2022-07-06 16:51:51.783458 z3-solver-4.9.0.0/core/src/math/lp/square_sparse_matrix.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15419 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/lp/square_sparse_matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)    45981 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/lp/square_sparse_matrix_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4571 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/lp/stacked_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4375 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/lp/static_matrix.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    13983 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/lp/static_matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12403 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/lp/static_matrix_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1134 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/lp/tail_matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8680 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/lp/test_bound_analyzer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2708 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/lp/u_set.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2099 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/lp/ul_pair.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11532 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/lp/var_eqs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4150 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/lp/var_register.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.523698 z3-solver-4.9.0.0/core/src/math/polynomial/
--rw-r--r--   0 vsts      (1001) docker     (121)      331 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/polynomial/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      235 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/polynomial/README
--rw-r--r--   0 vsts      (1001) docker     (121)   127290 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/polynomial/algebraic_numbers.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15844 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/polynomial/algebraic_numbers.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2232 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/polynomial/algebraic_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     4452 2022-07-06 16:51:51.787458 z3-solver-4.9.0.0/core/src/math/polynomial/linear_eq_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)   287495 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/polynomial.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    47657 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/polynomial.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8107 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/polynomial_cache.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      831 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/polynomial_cache.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3251 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/polynomial_primes.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1297 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/polynomial_var2value.h
--rw-r--r--   0 vsts      (1001) docker     (121)    28105 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/rpolynomial.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5902 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/rpolynomial.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4420 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/sexpr2upolynomial.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      540 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/sexpr2upolynomial.h
--rw-r--r--   0 vsts      (1001) docker     (121)   116680 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/upolynomial.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    37745 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/upolynomial.h
--rw-r--r--   0 vsts      (1001) docker     (121)    51846 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/upolynomial_factorization.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4050 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/upolynomial_factorization.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15307 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/polynomial/upolynomial_factorization_int.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.523698 z3-solver-4.9.0.0/core/src/math/realclosure/
--rw-r--r--   0 vsts      (1001) docker     (121)      149 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/realclosure/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    13293 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/realclosure/mpz_matrix.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5767 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/realclosure/mpz_matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1162 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/realclosure/rcf_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)   246522 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/realclosure/realclosure.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12608 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/realclosure/realclosure.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.523698 z3-solver-4.9.0.0/core/src/math/simplex/
--rw-r--r--   0 vsts      (1001) docker     (121)      130 2022-07-06 16:51:51.791458 z3-solver-4.9.0.0/core/src/math/simplex/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     3026 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/simplex/bit_matrix.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3692 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/simplex/bit_matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)    43912 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/simplex/model_based_opt.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7126 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/simplex/model_based_opt.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6916 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/simplex/network_flow.h
--rw-r--r--   0 vsts      (1001) docker     (121)    19865 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/simplex/network_flow_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2287 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/simplex/simplex.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7619 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/simplex/simplex.h
--rw-r--r--   0 vsts      (1001) docker     (121)    36196 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/simplex/simplex_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12316 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/simplex/sparse_matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18267 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/simplex/sparse_matrix_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2268 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/simplex/sparse_matrix_ops.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.523698 z3-solver-4.9.0.0/core/src/math/subpaving/
--rw-r--r--   0 vsts      (1001) docker     (121)      207 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    11360 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3665 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving.h
--rw-r--r--   0 vsts      (1001) docker     (121)      417 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_hwf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1160 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_hwf.h
--rw-r--r--   0 vsts      (1001) docker     (121)      424 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_mpf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1216 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_mpf.h
--rw-r--r--   0 vsts      (1001) docker     (121)      418 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_mpff.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      920 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_mpff.h
--rw-r--r--   0 vsts      (1001) docker     (121)      418 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_mpfx.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      920 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_mpfx.h
--rw-r--r--   0 vsts      (1001) docker     (121)      411 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_mpq.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      804 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_mpq.h
--rw-r--r--   0 vsts      (1001) docker     (121)    29828 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_t.h
--rw-r--r--   0 vsts      (1001) docker     (121)    62982 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_t_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)      959 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_types.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.523698 z3-solver-4.9.0.0/core/src/math/subpaving/tactic/
--rw-r--r--   0 vsts      (1001) docker     (121)      190 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/tactic/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    11490 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/tactic/expr2subpaving.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1051 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/tactic/expr2subpaving.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9246 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/tactic/subpaving_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      484 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/math/subpaving/tactic/subpaving_tactic.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.527698 z3-solver-4.9.0.0/core/src/model/
--rw-r--r--   0 vsts      (1001) docker     (121)      471 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/model/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     6842 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/model/array_factory.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      837 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/model/array_factory.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1546 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/model/char_factory.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10370 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/model/datatype_factory.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      743 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/model/datatype_factory.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1846 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/model/fpa_factory.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13055 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/model/func_interp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4331 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/model/func_interp.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17635 2022-07-06 16:51:51.795458 z3-solver-4.9.0.0/core/src/model/model.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3933 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4689 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model2expr.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      809 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model2expr.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3571 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_core.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3263 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_core.h
--rw-r--r--   0 vsts      (1001) docker     (121)    27862 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_evaluator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1765 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_evaluator.h
--rw-r--r--   0 vsts      (1001) docker     (121)      560 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_evaluator_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)    26151 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_implicant.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3682 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_implicant.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18579 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_macro_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10704 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_macro_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)      820 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     2920 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_pp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      320 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_pp.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12108 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_smt2_pp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      489 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_smt2_pp.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2460 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_v2_pp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      351 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/model_v2_pp.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1063 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/numeral_factory.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1062 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/numeral_factory.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4202 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/seq_factory.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1630 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/struct_factory.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1018 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/struct_factory.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3235 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/value_factory.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7578 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/model/value_factory.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.527698 z3-solver-4.9.0.0/core/src/muz/
--rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/README
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.527698 z3-solver-4.9.0.0/core/src/muz/base/
--rw-r--r--   0 vsts      (1001) docker     (121)      374 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     4585 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/bind_variables.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      918 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/bind_variables.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9790 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_boogie_proof.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2810 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_boogie_proof.h
--rw-r--r--   0 vsts      (1001) docker     (121)    45567 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_context.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    22039 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_context.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3909 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_costs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2697 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_costs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4574 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_engine_base.h
--rw-r--r--   0 vsts      (1001) docker     (121)    34320 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_rule.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12305 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_rule.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22668 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_rule_set.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9448 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_rule_set.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1769 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_rule_subsumption_index.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1339 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_rule_subsumption_index.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4107 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_rule_transformer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2779 2022-07-06 16:51:51.799458 z3-solver-4.9.0.0/core/src/muz/base/dl_rule_transformer.h
--rw-r--r--   0 vsts      (1001) docker     (121)    21454 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/base/dl_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    20032 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/base/dl_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16404 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/base/fp_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)    16218 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/base/hnf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      941 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/base/hnf.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11874 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/base/rule_properties.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2251 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/base/rule_properties.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.527698 z3-solver-4.9.0.0/core/src/muz/bmc/
--rw-r--r--   0 vsts      (1001) docker     (121)      103 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/bmc/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    63042 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/bmc/dl_bmc_engine.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1532 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/bmc/dl_bmc_engine.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.527698 z3-solver-4.9.0.0/core/src/muz/clp/
--rw-r--r--   0 vsts      (1001) docker     (121)      101 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/clp/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     7092 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/clp/clp_context.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      807 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/clp/clp_context.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.527698 z3-solver-4.9.0.0/core/src/muz/dataflow/
--rw-r--r--   0 vsts      (1001) docker     (121)       88 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/dataflow/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      377 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/dataflow/dataflow.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8957 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/dataflow/dataflow.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2162 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/dataflow/reachability.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.531698 z3-solver-4.9.0.0/core/src/muz/ddnf/
--rw-r--r--   0 vsts      (1001) docker     (121)      103 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/ddnf/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    29546 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/ddnf/ddnf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1533 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/ddnf/ddnf.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.531698 z3-solver-4.9.0.0/core/src/muz/fp/
--rw-r--r--   0 vsts      (1001) docker     (121)      238 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/fp/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    47821 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/fp/datalog_parser.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      787 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/fp/datalog_parser.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15652 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/fp/dl_cmds.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      611 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/fp/dl_cmds.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1235 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/fp/dl_register_engine.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      545 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/fp/dl_register_engine.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13892 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/fp/horn_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      633 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/fp/horn_tactic.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.531698 z3-solver-4.9.0.0/core/src/muz/rel/
--rw-r--r--   0 vsts      (1001) docker     (121)      675 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/rel/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    11055 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/rel/aig_exporter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2030 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/rel/aig_exporter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    32139 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/rel/check_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7024 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/rel/check_relation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14720 2022-07-06 16:51:51.803458 z3-solver-4.9.0.0/core/src/muz/rel/dl_base.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    50391 2022-07-06 16:51:51.807458 z3-solver-4.9.0.0/core/src/muz/rel/dl_base.h
--rw-r--r--   0 vsts      (1001) docker     (121)    24397 2022-07-06 16:51:51.807458 z3-solver-4.9.0.0/core/src/muz/rel/dl_bound_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6020 2022-07-06 16:51:51.807458 z3-solver-4.9.0.0/core/src/muz/rel/dl_bound_relation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18538 2022-07-06 16:51:51.807458 z3-solver-4.9.0.0/core/src/muz/rel/dl_check_table.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5110 2022-07-06 16:51:51.807458 z3-solver-4.9.0.0/core/src/muz/rel/dl_check_table.h
--rw-r--r--   0 vsts      (1001) docker     (121)    55025 2022-07-06 16:51:51.807458 z3-solver-4.9.0.0/core/src/muz/rel/dl_compiler.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12475 2022-07-06 16:51:51.807458 z3-solver-4.9.0.0/core/src/muz/rel/dl_compiler.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18625 2022-07-06 16:51:51.807458 z3-solver-4.9.0.0/core/src/muz/rel/dl_external_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5419 2022-07-06 16:51:51.807458 z3-solver-4.9.0.0/core/src/muz/rel/dl_external_relation.h
--rw-r--r--   0 vsts      (1001) docker     (121)   100214 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_finite_product_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    14996 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_finite_product_relation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    46503 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_instruction.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    13335 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_instruction.h
--rw-r--r--   0 vsts      (1001) docker     (121)    23843 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_interval_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5301 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_interval_relation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16002 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_lazy_table.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    11637 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_lazy_table.h
--rw-r--r--   0 vsts      (1001) docker     (121)    34292 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_mk_explanations.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2322 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_mk_explanations.h
--rw-r--r--   0 vsts      (1001) docker     (121)    19449 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_mk_similarity_compressor.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1648 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_mk_similarity_compressor.h
--rw-r--r--   0 vsts      (1001) docker     (121)    30985 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_mk_simple_joins.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1341 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_mk_simple_joins.h
--rw-r--r--   0 vsts      (1001) docker     (121)    46802 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_product_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7082 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_product_relation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    67602 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_relation_manager.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    30382 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_relation_manager.h
--rw-r--r--   0 vsts      (1001) docker     (121)    28208 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_sieve_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7789 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_sieve_relation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    54995 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_sparse_table.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    19139 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_sparse_table.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9380 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_table.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3921 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_table.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5275 2022-07-06 16:51:51.811458 z3-solver-4.9.0.0/core/src/muz/rel/dl_table_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20028 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/dl_table_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5488 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/dl_table_relation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13375 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/dl_vector_relation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    21688 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/doc.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12246 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/doc.h
--rw-r--r--   0 vsts      (1001) docker     (121)    27718 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/karr_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2628 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/karr_relation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22528 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/rel_context.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3941 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/rel_context.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8260 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/tbv.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4002 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/tbv.h
--rw-r--r--   0 vsts      (1001) docker     (121)    48305 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/udoc_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6984 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/rel/udoc_relation.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.535698 z3-solver-4.9.0.0/core/src/muz/spacer/
--rw-r--r--   0 vsts      (1001) docker     (121)      803 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/spacer/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    12176 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_antiunify.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1665 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_antiunify.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4695 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_arith_generalizers.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      578 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_callback.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1454 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_callback.h
--rw-r--r--   0 vsts      (1001) docker     (121)   139254 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_context.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    40939 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_context.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10884 2022-07-06 16:51:51.815458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_dl_interface.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_dl_interface.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14082 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_farkas_learner.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1185 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_farkas_learner.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10190 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_generalizers.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4889 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_generalizers.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8265 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_iuc_proof.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1719 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_iuc_proof.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15539 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_iuc_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6479 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_iuc_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5397 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_json.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      922 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_json.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5482 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_legacy_frames.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1415 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_legacy_frames.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3287 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_legacy_mbp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    24425 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_legacy_mev.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3835 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_legacy_mev.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6239 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_manager.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4048 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_manager.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3980 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_matrix.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      750 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_matrix.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2852 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_mbc.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      623 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_mbc.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7060 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_mev_array.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1017 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_mev_array.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6637 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_notes.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    10410 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_pdr.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3205 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_pdr.h
--rw-r--r--   0 vsts      (1001) docker     (121)    28026 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_proof_utils.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2498 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_proof_utils.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12909 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_prop_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4747 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_prop_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    89428 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_qe_project.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1282 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_qe_project.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22789 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_quant_generalizer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7363 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_sat_answer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      917 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_sat_answer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3796 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_sem_matcher.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1617 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_sem_matcher.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4862 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_sym_mux.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2270 2022-07-06 16:51:51.819458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_sym_mux.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2287 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_unsat_core_learner.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2560 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_unsat_core_learner.h
--rw-r--r--   0 vsts      (1001) docker     (121)    26351 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_unsat_core_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3772 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_unsat_core_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)    34388 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4037 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/spacer/spacer_util.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.535698 z3-solver-4.9.0.0/core/src/muz/tab/
--rw-r--r--   0 vsts      (1001) docker     (121)      101 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/tab/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    58114 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/tab/tab_context.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      824 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/tab/tab_context.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.539698 z3-solver-4.9.0.0/core/src/muz/transforms/
--rw-r--r--   0 vsts      (1001) docker     (121)      805 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    10577 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_array_blast.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1747 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_array_blast.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3566 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_array_eq_rewrite.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      966 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_array_eq_rewrite.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10470 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_array_instantiation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5633 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_array_instantiation.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2248 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_backwards.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      593 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_backwards.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11841 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_bit_blast.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      579 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_bit_blast.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6697 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_coalesce.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1185 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_coalesce.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6737 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_coi_filter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1029 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_coi_filter.h
--rw-r--r--   0 vsts      (1001) docker     (121)      638 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_different.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6419 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_elim_term_ite.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      829 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_elim_term_ite.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6141 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_filter_rules.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2401 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_filter_rules.h
--rw-r--r--   0 vsts      (1001) docker     (121)    19752 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_interp_tail_simplifier.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2997 2022-07-06 16:51:51.823458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_interp_tail_simplifier.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10871 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_karr_invariants.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_karr_invariants.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5696 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_loop_counter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1075 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_loop_counter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13782 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_magic_sets.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4217 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_magic_sets.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4392 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_magic_symbolic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      704 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_magic_symbolic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13079 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_quantifier_abstraction.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1472 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_quantifier_abstraction.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9577 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_quantifier_instantiation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1878 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_quantifier_instantiation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    30893 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_rule_inliner.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7090 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_rule_inliner.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7929 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_scale.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1109 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_scale.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4220 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_separate_negated_tails.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1422 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_separate_negated_tails.h
--rw-r--r--   0 vsts      (1001) docker     (121)    31324 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_slice.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2836 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_slice.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12907 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_subsumption_checker.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2537 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_subsumption_checker.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13624 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_synchronize.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4244 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_synchronize.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14778 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_unbound_compressor.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2888 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_unbound_compressor.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1860 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_unfold.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      988 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_unfold.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4247 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_transforms.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      355 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/muz/transforms/dl_transforms.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.539698 z3-solver-4.9.0.0/core/src/nlsat/
--rw-r--r--   0 vsts      (1001) docker     (121)      251 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/nlsat/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     3470 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_assignment.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1006 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_clause.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2031 2022-07-06 16:51:51.827458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_clause.h
--rw-r--r--   0 vsts      (1001) docker     (121)    29391 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_evaluator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1415 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_evaluator.h
--rw-r--r--   0 vsts      (1001) docker     (121)    75082 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_explain.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3508 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_explain.h
--rw-r--r--   0 vsts      (1001) docker     (121)    30681 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_interval_set.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3424 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_interval_set.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4352 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_justification.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1406 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     2704 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_scoped_literal_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)   139432 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6854 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1904 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_types.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5911 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/nlsat_types.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.539698 z3-solver-4.9.0.0/core/src/nlsat/tactic/
--rw-r--r--   0 vsts      (1001) docker     (121)      238 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/tactic/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    14350 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/tactic/goal2nlsat.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1544 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/tactic/goal2nlsat.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8835 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/tactic/nlsat_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      461 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/tactic/nlsat_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2337 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/tactic/qfnra_nlsat_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      503 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/nlsat/tactic/qfnra_nlsat_tactic.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.543698 z3-solver-4.9.0.0/core/src/opt/
--rw-r--r--   0 vsts      (1001) docker     (121)      421 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/opt/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    38366 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/opt/maxcore.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      720 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/opt/maxcore.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6546 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/opt/maxlex.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      411 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/opt/maxlex.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13065 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/opt/maxsmt.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6701 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/opt/maxsmt.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5124 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/opt/opt_cmds.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      350 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/opt/opt_cmds.h
--rw-r--r--   0 vsts      (1001) docker     (121)    61201 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/opt/opt_context.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    14147 2022-07-06 16:51:51.831458 z3-solver-4.9.0.0/core/src/opt/opt_context.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14064 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_cores.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2047 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_cores.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9087 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_lns.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2483 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_lns.h
--rw-r--r--   0 vsts      (1001) docker     (121)      468 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_mux.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3387 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     3303 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_pareto.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2678 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_pareto.h
--rw-r--r--   0 vsts      (1001) docker     (121)    24914 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_parse.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      442 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_parse.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7282 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_preprocess.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1041 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_preprocess.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7432 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_sls_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18868 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5755 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/opt_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    19967 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/optsmt.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2256 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/optsmt.h
--rw-r--r--   0 vsts      (1001) docker     (121)    27288 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/pb_sls.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      844 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/pb_sls.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4710 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/sortmax.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3174 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/totalizer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1202 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/totalizer.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10471 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/wmax.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      414 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/opt/wmax.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.543698 z3-solver-4.9.0.0/core/src/params/
--rw-r--r--   0 vsts      (1001) docker     (121)      487 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1668 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/arith_rewriter_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)      873 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/array_rewriter_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)      862 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/bit_blaster_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1182 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/bool_rewriter_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     1443 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/bv_rewriter_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     7280 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/context_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2177 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/context_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)      309 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/fpa2bv_rewriter_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)      305 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/fpa_rewriter_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     1422 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/pattern_inference_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1355 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/pattern_inference_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1507 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/pattern_inference_params_helper.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)      724 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/poly_rewriter_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     1062 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/rewriter_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)      221 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/params/seq_rewriter_params.pyg
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.471697 z3-solver-4.9.0.0/core/src/parsers/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.543698 z3-solver-4.9.0.0/core/src/parsers/smt2/
--rw-r--r--   0 vsts      (1001) docker     (121)      152 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/parsers/smt2/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1111 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/parsers/smt2/marshal.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      433 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/parsers/smt2/marshal.h
--rw-r--r--   0 vsts      (1001) docker     (121)   130536 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/parsers/smt2/smt2parser.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      633 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/parsers/smt2/smt2parser.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11474 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/parsers/smt2/smt2scanner.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2884 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/parsers/smt2/smt2scanner.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.543698 z3-solver-4.9.0.0/core/src/parsers/util/
--rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/parsers/util/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1689 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/parsers/util/cost_parser.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      656 2022-07-06 16:51:51.835458 z3-solver-4.9.0.0/core/src/parsers/util/cost_parser.h
--rw-r--r--   0 vsts      (1001) docker     (121)      405 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/parsers/util/parser_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     3361 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/parsers/util/pattern_validation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      953 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/parsers/util/pattern_validation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13917 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/parsers/util/scanner.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1865 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/parsers/util/scanner.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3565 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/parsers/util/simple_parser.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1673 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/parsers/util/simple_parser.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.547698 z3-solver-4.9.0.0/core/src/qe/
--rw-r--r--   0 vsts      (1001) docker     (121)      443 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/CMakeLists.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.547698 z3-solver-4.9.0.0/core/src/qe/lite/
--rw-r--r--   0 vsts      (1001) docker     (121)      128 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/lite/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    88561 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/lite/qe_lite.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1948 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/lite/qe_lite.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.547698 z3-solver-4.9.0.0/core/src/qe/mbp/
--rw-r--r--   0 vsts      (1001) docker     (121)      213 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    24770 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/mbp_arith.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1719 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/mbp_arith.h
--rw-r--r--   0 vsts      (1001) docker     (121)    60573 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/mbp_arrays.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1091 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/mbp_arrays.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11163 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/mbp_datatypes.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      991 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/mbp_datatypes.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10814 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/mbp_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3614 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/mbp_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15291 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/mbp_solve_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1390 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/mbp_solve_plugin.h
--rw-r--r--   0 vsts      (1001) docker     (121)    43940 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/mbp_term_graph.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4736 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/mbp/mbp_term_graph.h
--rw-r--r--   0 vsts      (1001) docker     (121)    73862 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/nlarith_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4752 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/nlarith_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)    34705 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/nlqsat.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      573 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/nlqsat.h
--rw-r--r--   0 vsts      (1001) docker     (121)    92355 2022-07-06 16:51:51.839459 z3-solver-4.9.0.0/core/src/qe/qe.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12062 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe.h
--rw-r--r--   0 vsts      (1001) docker     (121)    96004 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_arith_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10296 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_array_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5550 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_bool_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2535 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_bv_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1946 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_cmd.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      303 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_cmd.h
--rw-r--r--   0 vsts      (1001) docker     (121)    30943 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_datatype_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8042 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_dl_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    18384 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_mbi.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4820 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_mbi.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14736 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_mbp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1636 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_mbp.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3613 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      458 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qe_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    49526 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qsat.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4927 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/qe/qsat.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.551698 z3-solver-4.9.0.0/core/src/sat/
--rw-r--r--   0 vsts      (1001) docker     (121)      938 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    11849 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/dimacs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3217 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/dimacs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    31073 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_aig_cuts.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9166 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_aig_cuts.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9746 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_aig_finder.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1757 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_aig_finder.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3040 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_allocator.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15302 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_anf_simplifier.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3530 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_anf_simplifier.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16870 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_asymm_branch.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2677 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_asymm_branch.h
--rw-r--r--   0 vsts      (1001) docker     (121)      899 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_asymm_branch_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)    10836 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_bcd.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2241 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_bcd.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9197 2022-07-06 16:51:51.843459 z3-solver-4.9.0.0/core/src/sat/sat_big.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2511 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_big.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15094 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_binspr.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3462 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_binspr.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7294 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_clause.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8170 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_clause.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2390 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_clause_set.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1135 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_clause_set.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1127 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_clause_use_list.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3691 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_clause_use_list.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8343 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_cleaner.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      892 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_cleaner.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10707 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_config.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6218 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_config.h
--rw-r--r--   0 vsts      (1001) docker     (121)    26607 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_cut_simplifier.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6678 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_cut_simplifier.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8125 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_cutset.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6677 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_cutset.h
--rw-r--r--   0 vsts      (1001) docker     (121)    29615 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_cutset_compute_shift.h
--rw-r--r--   0 vsts      (1001) docker     (121)    19144 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_ddfw.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7292 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_ddfw.h
--rw-r--r--   0 vsts      (1001) docker     (121)    32192 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_drat.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6327 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_drat.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10797 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_elim_eqs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1247 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_elim_eqs.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10323 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_elim_vars.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1831 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_elim_vars.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5584 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_extension.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20068 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_gc.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8709 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_integrity_checker.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1045 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_integrity_checker.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2895 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_justification.h
--rw-r--r--   0 vsts      (1001) docker     (121)    27706 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_local_search.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10184 2022-07-06 16:51:51.847458 z3-solver-4.9.0.0/core/src/sat/sat_local_search.h
--rw-r--r--   0 vsts      (1001) docker     (121)    94612 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_lookahead.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    25137 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_lookahead.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9212 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_lut_finder.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2766 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_lut_finder.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16925 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_model_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5417 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_model_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7378 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_mus.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1627 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_mus.h
--rw-r--r--   0 vsts      (1001) docker     (121)    23162 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_npn3_finder.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5251 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_npn3_finder.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9433 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_parallel.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3227 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_parallel.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13579 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     8490 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_prob.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4083 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_prob.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10701 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_probing.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2628 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_probing.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10522 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_scc.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1587 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_scc.h
--rw-r--r--   0 vsts      (1001) docker     (121)      357 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_scc_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)    78437 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_simplifier.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9102 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_simplifier.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4427 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_simplifier_params.pyg
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.551698 z3-solver-4.9.0.0/core/src/sat/sat_solver/
--rw-r--r--   0 vsts      (1001) docker     (121)      217 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/sat_solver/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    40388 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/sat_solver/inc_sat_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      631 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/sat_solver/inc_sat_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)   171418 2022-07-06 16:51:51.851459 z3-solver-4.9.0.0/core/src/sat/sat_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    35517 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/sat_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1872 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/sat_solver_core.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5032 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/sat_types.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4441 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/sat_watched.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5923 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/sat_watched.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8002 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/sat_xor_finder.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2544 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/sat_xor_finder.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.555698 z3-solver-4.9.0.0/core/src/sat/smt/
--rw-r--r--   0 vsts      (1001) docker     (121)      914 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    19668 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/arith_axioms.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4404 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/arith_diagnostics.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    25688 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/arith_internalize.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    11239 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/arith_proof_checker.h
--rw-r--r--   0 vsts      (1001) docker     (121)    55744 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/arith_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    19978 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/arith_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    26968 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/array_axioms.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5841 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/array_diagnostics.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8619 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/array_internalize.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    11878 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/array_model.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9463 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/array_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    14538 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/array_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4016 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/atom2bool_var.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1000 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/atom2bool_var.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1949 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/ba_xor.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4993 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/bv_ackerman.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1985 2022-07-06 16:51:51.855459 z3-solver-4.9.0.0/core/src/sat/smt/bv_ackerman.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13251 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/bv_delay_internalize.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    29463 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/bv_internalize.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3958 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/bv_invariant.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    34926 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/bv_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    18435 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/bv_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    32588 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/dt_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6904 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/dt_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6647 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/euf_ackerman.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2351 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/euf_ackerman.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17163 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/euf_internalize.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/euf_invariant.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12208 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/euf_model.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6236 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/euf_proof.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10581 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/euf_relevancy.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5611 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/euf_relevancy.h
--rw-r--r--   0 vsts      (1001) docker     (121)    36792 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/euf_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    19990 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/euf_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15245 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/fpa_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2726 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/fpa_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8019 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/pb_card.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2159 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/pb_card.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1879 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/pb_constraint.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5869 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/pb_constraint.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9869 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/pb_internalize.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9357 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/pb_pb.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2715 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/pb_pb.h
--rw-r--r--   0 vsts      (1001) docker     (121)   130799 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/pb_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    18410 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/pb_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1453 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/pb_solver_interface.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1241 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/q_clause.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4473 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/q_clause.h
--rw-r--r--   0 vsts      (1001) docker     (121)    23629 2022-07-06 16:51:51.859459 z3-solver-4.9.0.0/core/src/sat/smt/q_ematch.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5499 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_ematch.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8588 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_eval.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1403 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_eval.h
--rw-r--r--   0 vsts      (1001) docker     (121)   162088 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_mam.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1473 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_mam.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20963 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_mbi.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4618 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_mbi.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12086 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_model_fixer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4079 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_model_fixer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9561 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_queue.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2106 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_queue.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11172 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3032 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/q_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11639 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/recfun_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4630 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/recfun_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)      818 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/sat_internalizer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2047 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/sat_smt.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11029 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/sat_th.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    11528 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/sat_th.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9321 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/user_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6376 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/user_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14902 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/smt/xor_solver.d
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.555698 z3-solver-4.9.0.0/core/src/sat/tactic/
--rw-r--r--   0 vsts      (1001) docker     (121)      194 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/tactic/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    35680 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/tactic/goal2sat.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2771 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/tactic/goal2sat.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10509 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/tactic/sat2goal.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2749 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/tactic/sat2goal.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9019 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/tactic/sat_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      772 2022-07-06 16:51:51.863459 z3-solver-4.9.0.0/core/src/sat/tactic/sat_tactic.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.555698 z3-solver-4.9.0.0/core/src/shell/
--rw-r--r--   0 vsts      (1001) docker     (121)     2061 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     7517 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/datalog_frontend.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      251 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/datalog_frontend.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8529 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/dimacs_frontend.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      257 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/dimacs_frontend.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18857 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/drat_frontend.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      137 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/drat_frontend.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3012 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/lp_frontend.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      162 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/lp_frontend.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15360 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/main.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4337 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/opt_frontend.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      255 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/opt_frontend.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2330 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/options.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4006 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/smtlib_frontend.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      403 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/smtlib_frontend.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1237 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/z3_log_frontend.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      295 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/shell/z3_log_frontend.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.567698 z3-solver-4.9.0.0/core/src/smt/
--rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    12501 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/arith_eq_adapter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2461 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/arith_eq_adapter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17412 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/arith_eq_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2574 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/arith_eq_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9711 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/database.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14730 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/database.smt
--rw-r--r--   0 vsts      (1001) docker     (121)    68535 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/diff_logic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22572 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/dyn_ack.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4338 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/dyn_ack.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22263 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/expr_context_simplifier.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2422 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/expr_context_simplifier.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4875 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/fingerprints.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3172 2022-07-06 16:51:51.867459 z3-solver-4.9.0.0/core/src/smt/fingerprints.h
--rw-r--r--   0 vsts      (1001) docker     (121)   167885 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/mam.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1480 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/mam.h
--rw-r--r--   0 vsts      (1001) docker     (121)    24172 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/old_interval.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7120 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/old_interval.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.567698 z3-solver-4.9.0.0/core/src/smt/params/
--rw-r--r--   0 vsts      (1001) docker     (121)      360 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)      930 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/dyn_ack_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      890 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/dyn_ack_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1809 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/preprocessor_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2146 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/preprocessor_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1999 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/qi_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3586 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/qi_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6390 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/smt_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10549 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/smt_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17135 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/smt_params_helper.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     3412 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_arith_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4156 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_arith_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)      931 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_array_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1203 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_array_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1052 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_bv_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1039 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_bv_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)      637 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_datatype_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)      686 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_pb_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      533 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_pb_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)      427 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_seq_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      507 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_seq_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2335 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_str_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4192 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/params/theory_str_params.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.567698 z3-solver-4.9.0.0/core/src/smt/proto_model/
--rw-r--r--   0 vsts      (1001) docker     (121)      124 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/proto_model/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    12209 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/proto_model/proto_model.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3412 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/proto_model/proto_model.h
--rw-r--r--   0 vsts      (1001) docker     (121)    21315 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/qi_queue.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3642 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/qi_queue.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3164 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/seq_axioms.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4527 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/seq_axioms.h
--rw-r--r--   0 vsts      (1001) docker     (121)    40668 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/seq_eq_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9363 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/seq_ne_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3719 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/seq_offset_eq.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1364 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/seq_offset_eq.h
--rw-r--r--   0 vsts      (1001) docker     (121)    33961 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/seq_regex.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7452 2022-07-06 16:51:51.871459 z3-solver-4.9.0.0/core/src/smt/seq_regex.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1467 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt2_extra_cmds.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      276 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt2_extra_cmds.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3367 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_almost_cg_table.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1785 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_almost_cg_table.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6124 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_arith_value.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1292 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_arith_value.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2800 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_b_justification.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3915 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_bool_var_data.h
--rw-r--r--   0 vsts      (1001) docker     (121)    45977 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_case_split_queue.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1476 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_case_split_queue.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7895 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_cg_table.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7041 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_cg_table.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6180 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_checker.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1209 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_checker.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4708 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_clause.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9157 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_clause.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5637 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_clause_proof.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2119 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_clause_proof.h
--rw-r--r--   0 vsts      (1001) docker     (121)    59769 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_conflict_resolution.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9754 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_conflict_resolution.h
--rw-r--r--   0 vsts      (1001) docker     (121)    23797 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_consequences.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)   188272 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_context.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    64013 2022-07-06 16:51:51.875459 z3-solver-4.9.0.0/core/src/smt/smt_context.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16995 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_context_inv.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    28741 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_context_pp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4664 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_context_stat.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12382 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_enode.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15036 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_enode.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2375 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_eq_justification.h
--rw-r--r--   0 vsts      (1001) docker     (121)      714 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_failure.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10603 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_farkas_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2783 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_farkas_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9244 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_for_each_relevant_expr.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2911 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_for_each_relevant_expr.h
--rw-r--r--   0 vsts      (1001) docker     (121)    21878 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_implied_equalities.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      565 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_implied_equalities.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17935 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_induction.cpp.disabled
--rw-r--r--   0 vsts      (1001) docker     (121)     4926 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_induction.h.disabled
--rw-r--r--   0 vsts      (1001) docker     (121)    70087 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_internalizer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15178 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_justification.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15086 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_justification.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8472 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_kernel.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9654 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_kernel.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3503 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_literal.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1629 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_literal.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5359 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_lookahead.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      648 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_lookahead.h
--rw-r--r--   0 vsts      (1001) docker     (121)    21839 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_model_checker.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3821 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_model_checker.h
--rw-r--r--   0 vsts      (1001) docker     (121)   102564 2022-07-06 16:51:51.879459 z3-solver-4.9.0.0/core/src/smt/smt_model_finder.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4594 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_model_finder.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20692 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_model_generator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9740 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_model_generator.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9066 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_parallel.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      436 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_parallel.h
--rw-r--r--   0 vsts      (1001) docker     (121)    31287 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_quantifier.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5880 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_quantifier.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1724 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_quantifier_instances.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16299 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_quick_checker.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3708 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_quick_checker.h
--rw-r--r--   0 vsts      (1001) docker     (121)    23903 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_relevancy.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6004 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_relevancy.h
--rw-r--r--   0 vsts      (1001) docker     (121)    40421 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_setup.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3911 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_setup.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17917 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      513 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)      347 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_statistics.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1194 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_statistics.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8597 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_theory.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    20897 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_theory.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1622 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_types.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1698 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_value_sort.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      402 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/smt_value_sort.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2332 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/spanning_tree.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1183 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/spanning_tree_base.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15989 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/spanning_tree_def.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.567698 z3-solver-4.9.0.0/core/src/smt/tactic/
--rw-r--r--   0 vsts      (1001) docker     (121)      266 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/tactic/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     9936 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/tactic/ctx_solver_simplify_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      496 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/tactic/ctx_solver_simplify_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14836 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/tactic/smt_tactic_core.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      844 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/tactic/smt_tactic_core.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3855 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/tactic/unit_subsumption_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      719 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/tactic/unit_subsumption_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)      467 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/theory_arith.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    59928 2022-07-06 16:51:51.883459 z3-solver-4.9.0.0/core/src/smt/theory_arith.h
--rw-r--r--   0 vsts      (1001) docker     (121)    86410 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_arith_aux.h
--rw-r--r--   0 vsts      (1001) docker     (121)   141116 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_arith_core.h
--rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_arith_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13206 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_arith_eq.h
--rw-r--r--   0 vsts      (1001) docker     (121)    44997 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_arith_int.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8042 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_arith_inv.h
--rw-r--r--   0 vsts      (1001) docker     (121)    86158 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_arith_nl.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18245 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_arith_pp.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16883 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_array.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4414 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_array.h
--rw-r--r--   0 vsts      (1001) docker     (121)    24061 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_array_bapa.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      702 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_array_bapa.h
--rw-r--r--   0 vsts      (1001) docker     (121)    38789 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_array_base.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9093 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_array_base.h
--rw-r--r--   0 vsts      (1001) docker     (121)    31628 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_array_full.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3641 2022-07-06 16:51:51.887459 z3-solver-4.9.0.0/core/src/smt/theory_array_full.h
--rw-r--r--   0 vsts      (1001) docker     (121)    82485 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_bv.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12842 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_bv.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16133 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_char.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2654 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_char.h
--rw-r--r--   0 vsts      (1001) docker     (121)    43801 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_datatype.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5940 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_datatype.h
--rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_dense_diff_logic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10696 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_dense_diff_logic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    44314 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_dense_diff_logic_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)      675 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_diff_logic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    13237 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_diff_logic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    45130 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_diff_logic_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9608 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_dl.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      290 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_dl.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1444 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_dummy.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1421 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_dummy.h
--rw-r--r--   0 vsts      (1001) docker     (121)    24747 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_fpa.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4139 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_fpa.h
--rw-r--r--   0 vsts      (1001) docker     (121)   143694 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_lra.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2812 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_lra.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1881 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_opt.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      836 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_opt.h
--rw-r--r--   0 vsts      (1001) docker     (121)    78857 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_pb.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    16098 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_pb.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16770 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_recfun.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4399 2022-07-06 16:51:51.891459 z3-solver-4.9.0.0/core/src/smt/theory_recfun.h
--rw-r--r--   0 vsts      (1001) docker     (121)   105237 2022-07-06 16:51:51.895459 z3-solver-4.9.0.0/core/src/smt/theory_seq.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    29522 2022-07-06 16:51:51.895459 z3-solver-4.9.0.0/core/src/smt/theory_seq.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1400 2022-07-06 16:51:51.895459 z3-solver-4.9.0.0/core/src/smt/theory_seq_empty.h
--rw-r--r--   0 vsts      (1001) docker     (121)    43020 2022-07-06 16:51:51.895459 z3-solver-4.9.0.0/core/src/smt/theory_special_relations.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8022 2022-07-06 16:51:51.895459 z3-solver-4.9.0.0/core/src/smt/theory_special_relations.h
--rw-r--r--   0 vsts      (1001) docker     (121)   396808 2022-07-06 16:51:51.899459 z3-solver-4.9.0.0/core/src/smt/theory_str.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    31268 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/theory_str.h
--rw-r--r--   0 vsts      (1001) docker     (121)    74390 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/theory_str_mc.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    78101 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/theory_str_regex.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12756 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/theory_user_propagator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6673 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/theory_user_propagator.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4464 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/theory_utvpi.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10723 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/theory_utvpi.h
--rw-r--r--   0 vsts      (1001) docker     (121)    32925 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/theory_utvpi_def.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12098 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/theory_wmaxsat.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4920 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/theory_wmaxsat.h
--rw-r--r--   0 vsts      (1001) docker     (121)      865 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/uses_theory.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      643 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/uses_theory.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4129 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/watch_list.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5754 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/smt/watch_list.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.571698 z3-solver-4.9.0.0/core/src/solver/
--rw-r--r--   0 vsts      (1001) docker     (121)      408 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/CMakeLists.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.571698 z3-solver-4.9.0.0/core/src/solver/assertions/
--rw-r--r--   0 vsts      (1001) docker     (121)      140 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/assertions/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    23012 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/assertions/asserted_formulas.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    13686 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/assertions/asserted_formulas.h
--rw-r--r--   0 vsts      (1001) docker     (121)    16802 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/check_logic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      563 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/check_logic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1714 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/check_sat_result.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3372 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/check_sat_result.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13898 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/combined_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      514 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/combined_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)      654 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/combined_solver_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)    11537 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/mus.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1504 2022-07-06 16:51:51.903459 z3-solver-4.9.0.0/core/src/solver/mus.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1413 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/parallel_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)    27558 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/parallel_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      317 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/parallel_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)      504 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/progress_callback.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4019 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/smt_logics.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      995 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/smt_logics.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9392 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8704 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6434 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/solver2tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      516 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/solver2tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3094 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/solver_na2as.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/solver_na2as.h
--rw-r--r--   0 vsts      (1001) docker     (121)      485 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/solver_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)    13341 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/solver_pool.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1386 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/solver_pool.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12642 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/tactic2solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      983 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/solver/tactic2solver.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.571698 z3-solver-4.9.0.0/core/src/tactic/
--rw-r--r--   0 vsts      (1001) docker     (121)      489 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/CMakeLists.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.571698 z3-solver-4.9.0.0/core/src/tactic/aig/
--rw-r--r--   0 vsts      (1001) docker     (121)      141 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/aig/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    57231 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/aig/aig.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2169 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/aig/aig.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3003 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/aig/aig_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      398 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/aig/aig_tactic.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.575698 z3-solver-4.9.0.0/core/src/tactic/arith/
--rw-r--r--   0 vsts      (1001) docker     (121)     1082 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     5009 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/add_bounds_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      737 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/add_bounds_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4596 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/arith_bounds_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      943 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/arith_bounds_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7637 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/bound_manager.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2709 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/bound_manager.h
--rw-r--r--   0 vsts      (1001) docker     (121)    30252 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/bound_propagator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10599 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/bound_propagator.h
--rw-r--r--   0 vsts      (1001) docker     (121)    19613 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/bv2int_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4345 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/bv2int_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    22792 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/bv2real_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8499 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/bv2real_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3043 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/card2bv_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3532 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/card2bv_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10738 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/degree_shift_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      729 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/degree_shift_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13172 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/diff_neq_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      753 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/diff_neq_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12766 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/eq2bv_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      533 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/eq2bv_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11133 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/factor_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      447 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/factor_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10817 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/fix_dl_var_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      846 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/fix_dl_var_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    61765 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/fm_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      649 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/fm_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13331 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/lia2card_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      631 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/lia2card_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11585 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/lia2pb_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      511 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/lia2pb_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8164 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/linear_equation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2724 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/linear_equation.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17058 2022-07-06 16:51:51.915459 z3-solver-4.9.0.0/core/src/tactic/arith/nla2bv_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      648 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/nla2bv_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5784 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/normalize_bounds_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      611 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/normalize_bounds_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2969 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/pb2bv_model_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      923 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/pb2bv_model_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    38030 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/pb2bv_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      597 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/pb2bv_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    19112 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/probe_arith.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2854 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/probe_arith.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17625 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/propagate_ineqs_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      996 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/propagate_ineqs_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    37167 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/purify_arith_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1855 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/purify_arith_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    14530 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/recover_01_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      764 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/arith/recover_01_tactic.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.575698 z3-solver-4.9.0.0/core/src/tactic/bv/
--rw-r--r--   0 vsts      (1001) docker     (121)      664 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     9452 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bit_blaster_model_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      564 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bit_blaster_model_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5418 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bit_blaster_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      654 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bit_blaster_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17075 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bv1_blaster_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      990 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bv1_blaster_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6766 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bv_bound_chk_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      466 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bv_bound_chk_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    23632 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bv_bounds_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      745 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bv_bounds_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18044 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bv_size_reduction_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      753 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bv_size_reduction_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    15135 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bvarray2uf_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2152 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bvarray2uf_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3752 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bvarray2uf_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      553 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/bvarray2uf_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4830 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/dt2bv_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      509 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/dt2bv_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10915 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/elim_small_bv_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      511 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/elim_small_bv_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10638 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/max_bv_sharing_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      747 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/bv/max_bv_sharing_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2638 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/converter.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.579698 z3-solver-4.9.0.0/core/src/tactic/core/
--rw-r--r--   0 vsts      (1001) docker     (121)     1368 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/core/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     7023 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/core/blast_term_ite_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      722 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/core/blast_term_ite_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    24508 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/core/cofactor_elim_term_ite.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      700 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/core/cofactor_elim_term_ite.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2063 2022-07-06 16:51:51.919459 z3-solver-4.9.0.0/core/src/tactic/core/cofactor_term_ite_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      579 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/cofactor_term_ite_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2094 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/collect_occs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      545 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/collect_occs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6152 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/collect_statistics_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/collect_statistics_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20473 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/ctx_simplify_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1807 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/ctx_simplify_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2102 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/der_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      338 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/der_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4433 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/distribute_forall_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      449 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/distribute_forall_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17947 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/dom_simplify_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4339 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/dom_simplify_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5283 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/elim_term_ite_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      542 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/elim_term_ite_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    33793 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/elim_uncnstr_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      512 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/elim_uncnstr_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8848 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/injectivity_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      467 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/injectivity_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3246 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/nnf_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      581 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/nnf_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6781 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/occf_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      743 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/occf_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    21647 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/pb_preprocess_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      579 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/pb_preprocess_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7814 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/propagate_values_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      553 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/propagate_values_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18141 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/reduce_args_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      565 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/reduce_args_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18593 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/reduce_invertible_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      522 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/reduce_invertible_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2902 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/simplify_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1373 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/simplify_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    46582 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/solve_eqs_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      562 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/solve_eqs_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6452 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/special_relations_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1878 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/special_relations_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4893 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/split_clause_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      535 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/split_clause_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20911 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/symmetry_reduce_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      461 2022-07-06 16:51:51.923459 z3-solver-4.9.0.0/core/src/tactic/core/symmetry_reduce_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    33057 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/core/tseitin_cnf_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      899 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/core/tseitin_cnf_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3169 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/dependency_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1005 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/dependency_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)      749 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/equiv_proof_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1111 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/equiv_proof_converter.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.579698 z3-solver-4.9.0.0/core/src/tactic/fd_solver/
--rw-r--r--   0 vsts      (1001) docker     (121)      244 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fd_solver/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    13816 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fd_solver/bounded_int2bv_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      358 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fd_solver/bounded_int2bv_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7367 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fd_solver/enum2bv_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      344 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fd_solver/enum2bv_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1281 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fd_solver/fd_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      717 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fd_solver/fd_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5999 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fd_solver/pb2bv_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      355 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fd_solver/pb2bv_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)    77411 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fd_solver/smtfd_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      546 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fd_solver/smtfd_solver.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1036 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/filter_model_converter.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.579698 z3-solver-4.9.0.0/core/src/tactic/fpa/
--rw-r--r--   0 vsts      (1001) docker     (121)      347 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fpa/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     3033 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fpa/fpa2bv_model_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1202 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fpa/fpa2bv_model_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4635 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fpa/fpa2bv_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      468 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fpa/fpa2bv_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4498 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fpa/qffp_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      900 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fpa/qffp_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fpa/qffplra_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      591 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/fpa/qffplra_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6453 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/generic_model_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1947 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/generic_model_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)    20473 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/goal.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8414 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/goal.h
--rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/goal_num_occurs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      616 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/goal_num_occurs.h
--rw-r--r--   0 vsts      (1001) docker     (121)      518 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/goal_shared_occs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1056 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/goal_shared_occs.h
--rw-r--r--   0 vsts      (1001) docker     (121)      590 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/goal_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      249 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/goal_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6208 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/horn_subsume_model_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1905 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/horn_subsume_model_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5352 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/model_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3478 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/model_converter.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.579698 z3-solver-4.9.0.0/core/src/tactic/portfolio/
--rw-r--r--   0 vsts      (1001) docker     (121)      393 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/portfolio/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     2389 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/portfolio/default_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      497 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/portfolio/default_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5762 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/portfolio/smt_strategic_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      345 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/portfolio/solver2lookahead.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      279 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/portfolio/solver2lookahead.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5238 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/portfolio/solver_subsumption_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      438 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/portfolio/solver_subsumption_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13583 2022-07-06 16:51:51.927459 z3-solver-4.9.0.0/core/src/tactic/probe.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3968 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/probe.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4167 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/proof_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1310 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/proof_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2350 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/replace_proof_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1066 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/replace_proof_converter.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.583698 z3-solver-4.9.0.0/core/src/tactic/sls/
--rw-r--r--   0 vsts      (1001) docker     (121)      253 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/sls/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    12411 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/sls/bvsls_opt_engine.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1915 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/sls/bvsls_opt_engine.h
--rw-r--r--   0 vsts      (1001) docker     (121)    21118 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/sls/sls_engine.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3958 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/sls/sls_engine.h
--rw-r--r--   0 vsts      (1001) docker     (121)    32923 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/sls/sls_evaluator.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2441 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/sls/sls_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)      852 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/sls/sls_powers.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4059 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/sls/sls_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      469 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/sls/sls_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    37151 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/sls/sls_tracker.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.583698 z3-solver-4.9.0.0/core/src/tactic/smtlogics/
--rw-r--r--   0 vsts      (1001) docker     (121)      825 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1251 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/nra_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      355 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/nra_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2031 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfaufbv_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      443 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfaufbv_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1349 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfauflia_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      449 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfauflia_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5026 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfbv_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      603 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfbv_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4199 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfidl_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      432 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfidl_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8629 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qflia_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      602 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qflia_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2886 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qflra_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      429 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qflra_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4327 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfnia_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      429 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfnia_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1619 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfnra_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      429 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfnra_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1028 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfuf_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      433 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfuf_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)      466 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfufbv_ackr_model_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      388 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfufbv_ackr_model_converter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6481 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfufbv_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      626 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfufbv_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)      481 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfufbv_tactic_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)     4079 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/quant_tactics.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1591 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/quant_tactics.h
--rw-r--r--   0 vsts      (1001) docker     (121)      652 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/smt_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      531 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/smtlogics/smt_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7453 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4637 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)      827 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/tactic_exception.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1827 2022-07-06 16:51:51.931459 z3-solver-4.9.0.0/core/src/tactic/tactic_params.pyg
--rw-r--r--   0 vsts      (1001) docker     (121)    42859 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/tactical.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3596 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/tactical.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.583698 z3-solver-4.9.0.0/core/src/tactic/ufbv/
--rw-r--r--   0 vsts      (1001) docker     (121)      380 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/ufbv/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     4024 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/ufbv/macro_finder_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      439 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/ufbv/macro_finder_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3553 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/ufbv/quasi_macros_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      445 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/ufbv/quasi_macros_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)    28684 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/ufbv/ufbv_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    11400 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/ufbv/ufbv_rewriter.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2121 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/ufbv/ufbv_rewriter_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      488 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/ufbv/ufbv_rewriter_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2663 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/ufbv/ufbv_tactic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      578 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/ufbv/ufbv_tactic.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3686 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/tactic/user_propagator_base.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.591698 z3-solver-4.9.0.0/core/src/test/
--rw-r--r--   0 vsts      (1001) docker     (121)     3277 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    20838 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/algebraic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3463 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/api.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1404 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/api_bug.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1641 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/arith_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1502 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/arith_simplifier_plugin.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4462 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/ast.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2473 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/bdd.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7171 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/bit_blaster.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6684 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/bit_vector.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6798 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/bits.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      886 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/buffer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4166 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/chashtable.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1436 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/check_assumptions.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9269 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/cnf_backbones.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2097 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/cube_clause.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1682 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/datalog_parser.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6262 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/ddnf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4346 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/diff_logic.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3092 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/dl_context.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12015 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/dl_product_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9644 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/dl_query.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    11675 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/dl_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2790 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/dl_table.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1293 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/dl_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15078 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/doc.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4117 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/egraph.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1034 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/escaped.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1050 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/ex.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3066 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/expr_rand.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1643 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/expr_substitution.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    18313 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/ext_numeral.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1587 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/f2n.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      675 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/factor_rewriter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8368 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/finder.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2368 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/fixed_bit_vector.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1609 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/for_each_file.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      478 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/for_each_file.h
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.591698 z3-solver-4.9.0.0/core/src/test/fuzzing/
--rw-r--r--   0 vsts      (1001) docker     (121)      169 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/fuzzing/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     2080 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/fuzzing/expr_delta.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      899 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/fuzzing/expr_delta.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10966 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/fuzzing/expr_rand.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1092 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/fuzzing/expr_rand.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3661 2022-07-06 16:51:51.935459 z3-solver-4.9.0.0/core/src/test/get_consequences.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4290 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/get_implied_equalities.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2926 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/hashtable.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3994 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/heap.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1477 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/heap_trie.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    16590 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/hilbert_basis.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2139 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/horn_subsume_model_converter.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2162 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/hwf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2216 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/im_float_config.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5277 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/inf_rational.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    14651 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/interval.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7957 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/karr.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1154 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/list.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.591698 z3-solver-4.9.0.0/core/src/test/lp/
--rw-r--r--   0 vsts      (1001) docker     (121)      654 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/lp/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     4749 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/lp/argument_parser.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9167 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/lp/gomory_test.h
--rw-r--r--   0 vsts      (1001) docker     (121)   139388 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/lp/lp.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      313 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/lp/lp_main.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    28926 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/lp/nla_solver_test.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    13381 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/lp/smt_reader.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1763 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/lp/test_file_reader.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7752 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/main.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1064 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/map.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3463 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/matcher.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1169 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/memory.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1542 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/model2expr.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12428 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/model_based_opt.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2241 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/model_evaluator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2047 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/model_retrieval.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1011 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/mpbq.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1807 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/mpf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    19394 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/mpff.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1649 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/mpfx.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3513 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/mpq.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    16789 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/mpz.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1550 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/nlarith_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    25206 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/nlsat.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    25450 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/no_overflow.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3320 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/object_allocator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6996 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/old_interval.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1313 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/optional.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9195 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/parray.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7668 2022-07-06 16:51:51.939459 z3-solver-4.9.0.0/core/src/test/pb2bv.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10175 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/pdd.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7720 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/pdd_solver.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2281 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/permutation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    80338 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/polynomial.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6654 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/polynorm.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      838 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/prime_generator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      920 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/proof_checker.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    18036 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/qe_arith.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    19280 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/quant_elim.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9650 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/quant_solve.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      431 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/random.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    16327 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/rational.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5118 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/rcf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      322 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/region.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3574 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/sat_local_search.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1391 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/sat_lookahead.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2746 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/sat_user_scope.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1391 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/scoped_timer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1755 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/simple_parser.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4746 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/simplex.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7767 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/simplifier.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1532 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/small_object_allocator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4013 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/smt2print_parse.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      783 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/smt_context.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1305 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/solver_pool.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    19191 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/sorting_network.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1648 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/stack.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      874 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/string_buffer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1600 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/substitution.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1246 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/symbol.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      950 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/symbol_table.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3926 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/tbv.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1871 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/test_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)      991 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/theory_dl.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4595 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/theory_pb.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      206 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/timeout.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3856 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/total_order.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      625 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/totalizer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5393 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/trigo.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    30163 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/udoc_relation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3915 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/uint_set.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    43146 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/upolynomial.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1763 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/value_generator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1167 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/value_sweep.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2904 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/var_subst.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1335 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/vector.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      708 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/test/zstring.cpp
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.603698 z3-solver-4.9.0.0/core/src/util/
--rw-r--r--   0 vsts      (1001) docker     (121)     1433 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/util/CMakeLists.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     1313 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/util/approx_nat.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1183 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/util/approx_nat.h
--rw-r--r--   0 vsts      (1001) docker     (121)      893 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/util/approx_set.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6239 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/util/approx_set.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5533 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/util/array.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3738 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/util/array_map.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2398 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/util/backtrackable_set.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10525 2022-07-06 16:51:51.943459 z3-solver-4.9.0.0/core/src/util/basic_interval.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10016 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/bit_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2870 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/bit_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6556 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/bit_vector.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6008 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/bit_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6597 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/buffer.h
--rw-r--r--   0 vsts      (1001) docker     (121)      895 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/cancel_eh.h
--rw-r--r--   0 vsts      (1001) docker     (121)    21351 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/chashtable.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6535 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/checked_int64.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1306 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/cmd_context_types.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4372 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/cmd_context_types.h
--rw-r--r--   0 vsts      (1001) docker     (121)      718 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/common_msgs.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      932 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/common_msgs.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2721 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/container_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2928 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/debug.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2595 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/debug.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1355 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/dec_ref_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8572 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/dependency.h
--rw-r--r--   0 vsts      (1001) docker     (121)      300 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/dictionary.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2193 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/dlist.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3679 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/double_manager.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1268 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/ema.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1419 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/env_params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      411 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/env_params.h
--rw-r--r--   0 vsts      (1001) docker     (121)      759 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/error_codes.h
--rw-r--r--   0 vsts      (1001) docker     (121)      673 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/event_handler.h
--rw-r--r--   0 vsts      (1001) docker     (121)      883 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/ext_gcd.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9168 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/ext_numeral.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6983 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/f2n.h
--rw-r--r--   0 vsts      (1001) docker     (121)      580 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/file_path.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4493 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/fixed_bit_vector.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4015 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/fixed_bit_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)    25448 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/gparams.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4759 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/gparams.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2179 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/hash.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     6338 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/hash.h
--rw-r--r--   0 vsts      (1001) docker     (121)    28352 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/hashtable.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8081 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/heap.h
--rw-r--r--   0 vsts      (1001) docker     (121)    17467 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/hwf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5205 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/hwf.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1907 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/id_gen.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4035 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/id_var_list.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10330 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/inf_eps_rational.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1167 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/inf_int_rational.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     9308 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/inf_int_rational.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4953 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/inf_rational.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    12367 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/inf_rational.h
--rw-r--r--   0 vsts      (1001) docker     (121)      350 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/inf_s_integer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    10263 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/inf_s_integer.h
--rw-r--r--   0 vsts      (1001) docker     (121)      596 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/lbool.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      651 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/lbool.h
--rw-r--r--   0 vsts      (1001) docker     (121)      751 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/lim_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2158 2022-07-06 16:51:51.947459 z3-solver-4.9.0.0/core/src/util/list.h
--rw-r--r--   0 vsts      (1001) docker     (121)      555 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/luby.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      456 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/luby.h
--rw-r--r--   0 vsts      (1001) docker     (121)      325 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/machine.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8252 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/map.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6356 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/max_cliques.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11366 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/memory_manager.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3438 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/memory_manager.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6199 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/min_cut.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1453 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/min_cut.h
--rw-r--r--   0 vsts      (1001) docker     (121)    25098 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpbq.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    13896 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpbq.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1167 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpbqi.h
--rw-r--r--   0 vsts      (1001) docker     (121)    73951 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    11247 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpf.h
--rw-r--r--   0 vsts      (1001) docker     (121)    46099 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpff.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    15279 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpff.h
--rw-r--r--   0 vsts      (1001) docker     (121)    24653 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpfx.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    11435 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpfx.h
--rw-r--r--   0 vsts      (1001) docker     (121)    13802 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpn.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     3034 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpn.h
--rw-r--r--   0 vsts      (1001) docker     (121)    12270 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpq.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    26459 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpq.h
--rw-r--r--   0 vsts      (1001) docker     (121)      761 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpq_inf.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7732 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpq_inf.h
--rw-r--r--   0 vsts      (1001) docker     (121)    70068 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpz.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    19409 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpz.h
--rw-r--r--   0 vsts      (1001) docker     (121)    11044 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mpzzp.h
--rw-r--r--   0 vsts      (1001) docker     (121)      985 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/mutex.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1573 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/nat_set.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1745 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/numeral_buffer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6365 2022-07-06 16:51:51.951459 z3-solver-4.9.0.0/core/src/util/obj_hashtable.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1236 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/obj_mark.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5516 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/obj_pair_hashtable.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1612 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/obj_pair_set.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3285 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/obj_ref.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2758 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/obj_ref_hashtable.h
--rw-r--r--   0 vsts      (1001) docker     (121)     5487 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/obj_triple_hashtable.h
--rw-r--r--   0 vsts      (1001) docker     (121)     8415 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/object_allocator.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2822 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/optional.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1530 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/page.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      994 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/page.h
--rw-r--r--   0 vsts      (1001) docker     (121)    33686 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/params.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5054 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/params.h
--rw-r--r--   0 vsts      (1001) docker     (121)    18251 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/parray.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1552 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/permutation.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2201 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/permutation.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1376 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/plugin_manager.h
--rw-r--r--   0 vsts      (1001) docker     (121)      682 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/pool.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3240 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/prime_generator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1025 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/prime_generator.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2132 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/ptr_scoped_buffer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1302 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/queue.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3515 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/rational.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)    16662 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/rational.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2415 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/ref.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3910 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/ref_buffer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6758 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/ref_pair_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/ref_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10941 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/ref_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3366 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/region.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1958 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/region.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2244 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/rlimit.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2130 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/rlimit.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1308 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/s_integer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     5939 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/s_integer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6065 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/sat_literal.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1124 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/scoped_ctrl_c.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      810 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/scoped_ctrl_c.h
--rw-r--r--   0 vsts      (1001) docker     (121)      814 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/scoped_limit_trail.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4527 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/scoped_numeral.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1540 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/scoped_numeral_buffer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1770 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/scoped_numeral_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1976 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/scoped_ptr_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3298 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/scoped_timer.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      582 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/scoped_timer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4683 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/scoped_vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9158 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/sexpr.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2802 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/sexpr.h
--rw-r--r--   0 vsts      (1001) docker     (121)      570 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/sign.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7516 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/small_object_allocator.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1634 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/small_object_allocator.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1802 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/smt2_util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      403 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/smt2_util.h
--rw-r--r--   0 vsts      (1001) docker     (121)    54782 2022-07-06 16:51:51.955459 z3-solver-4.9.0.0/core/src/util/sorting_network.h
--rw-r--r--   0 vsts      (1001) docker     (121)      497 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/sstream.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3735 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/stack.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1286 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/stack.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1326 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/stacked_value.h
--rw-r--r--   0 vsts      (1001) docker     (121)    21382 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/state_graph.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     7290 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/state_graph.h
--rw-r--r--   0 vsts      (1001) docker     (121)     7152 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/statistics.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     1225 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/statistics.h
--rw-r--r--   0 vsts      (1001) docker     (121)      503 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/stats.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1882 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/stopwatch.h
--rw-r--r--   0 vsts      (1001) docker     (121)      679 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/str_hashtable.h
--rw-r--r--   0 vsts      (1001) docker     (121)      686 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/stream_buffer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3860 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/string_buffer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4713 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/symbol.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     4536 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/symbol.h
--rw-r--r--   0 vsts      (1001) docker     (121)     4753 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/symbol_table.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1403 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/timeit.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      572 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/timeit.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1111 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/timeout.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      301 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/timeout.h
--rw-r--r--   0 vsts      (1001) docker     (121)      689 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/timer.h
--rw-r--r--   0 vsts      (1001) docker     (121)     3980 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/top_sort.h
--rw-r--r--   0 vsts      (1001) docker     (121)    10448 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/total_order.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1239 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/tptr.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1621 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/trace.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2374 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/trace.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9693 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/trail.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1013 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/uint_map.h
--rw-r--r--   0 vsts      (1001) docker     (121)     9681 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/uint_set.h
--rw-r--r--   0 vsts      (1001) docker     (121)     6276 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/union_find.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2662 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/util.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     8419 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/util.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1591 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/var_queue.h
--rw-r--r--   0 vsts      (1001) docker     (121)    19790 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/vector.h
--rw-r--r--   0 vsts      (1001) docker     (121)     2922 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/warning.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      541 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/warning.h
--rw-r--r--   0 vsts      (1001) docker     (121)     1743 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/z3_exception.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)      879 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/z3_exception.h
--rw-r--r--   0 vsts      (1001) docker     (121)      298 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/z3_version.h.cmake.in
--rw-r--r--   0 vsts      (1001) docker     (121)      263 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/z3_version.h.in
--rw-r--r--   0 vsts      (1001) docker     (121)     7749 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/zstring.cpp
--rw-r--r--   0 vsts      (1001) docker     (121)     2824 2022-07-06 16:51:51.959459 z3-solver-4.9.0.0/core/src/util/zstring.h
--rw-r--r--   0 vsts      (1001) docker     (121)      352 2022-07-06 16:52:31.851694 z3-solver-4.9.0.0/core/z3.pc.cmake.in
--rw-r--r--   0 vsts      (1001) docker     (121)      107 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)    13637 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 16:52:32.607698 z3-solver-4.9.0.0/z3/
--rw-r--r--   0 vsts      (1001) docker     (121)      210 2022-07-06 16:51:51.727458 z3-solver-4.9.0.0/z3/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)   329080 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/z3/z3.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16090 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/z3/z3num.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1113 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/z3/z3poly.py
--rw-r--r--   0 vsts      (1001) docker     (121)    45224 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/z3/z3printer.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5039 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/z3/z3rcf.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4723 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/z3/z3types.py
--rw-r--r--   0 vsts      (1001) docker     (121)    11388 2022-07-06 16:51:51.731458 z3-solver-4.9.0.0/z3/z3util.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.762395 z3-solver-4.9.1.0/
+-rw-r--r--   0 vsts      (1001) docker     (121)      696 2022-07-06 19:24:48.762395 z3-solver-4.9.1.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      509 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/README.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.586393 z3-solver-4.9.1.0/core/
+-rw-r--r--   0 vsts      (1001) docker     (121)    27881 2022-07-06 19:24:47.978386 z3-solver-4.9.1.0/core/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     1096 2022-07-06 19:24:47.978386 z3-solver-4.9.1.0/core/LICENSE.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.586393 z3-solver-4.9.1.0/core/cmake/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1644 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/Z3Config.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (121)      594 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/check_link_atomic.cmake
+-rw-r--r--   0 vsts      (1001) docker     (121)      942 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     2327 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/compiler_lto.cmake
+-rw-r--r--   0 vsts      (1001) docker     (121)     5925 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/compiler_warnings.cmake
+-rw-r--r--   0 vsts      (1001) docker     (121)      771 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/cxx_compiler_flags_overrides.cmake
+-rw-r--r--   0 vsts      (1001) docker     (121)     8433 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/git_utils.cmake
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.586393 z3-solver-4.9.1.0/core/cmake/modules/
+-rw-r--r--   0 vsts      (1001) docker     (121)      281 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/modules/DotnetImports.props.in
+-rw-r--r--   0 vsts      (1001) docker     (121)    19448 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/modules/FindDotnet.cmake
+-rw-r--r--   0 vsts      (1001) docker     (121)     1396 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/modules/FindGMP.cmake
+-rw-r--r--   0 vsts      (1001) docker     (121)     8105 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/msvc_legacy_quirks.cmake
+-rw-r--r--   0 vsts      (1001) docker     (121)      913 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/target_arch_detect.cmake
+-rw-r--r--   0 vsts      (1001) docker     (121)      439 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/target_arch_detect.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    15273 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/z3_add_component.cmake
+-rw-r--r--   0 vsts      (1001) docker     (121)     1293 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/z3_add_cxx_flag.cmake
+-rw-r--r--   0 vsts      (1001) docker     (121)      794 2022-07-06 19:24:04.657826 z3-solver-4.9.1.0/core/cmake/z3_append_linker_flag_list_to_target.cmake
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.590393 z3-solver-4.9.1.0/core/scripts/
+-rw-r--r--   0 vsts      (1001) docker     (121)      391 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/README
+-rw-r--r--   0 vsts      (1001) docker     (121)     3024 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/build-win-signed.yml
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      502 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/build_libcxx_msan.sh
+-rw-r--r--   0 vsts      (1001) docker     (121)     1585 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/coverage.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      166 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/generate-doc.yml
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     2919 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_consts_files.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1259 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_copyright.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     1024 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_def_file.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      320 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_exception.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    38118 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_genfile_common.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     1236 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_gparams_register_modules_cpp.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     1330 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_install_tactic_cpp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      487 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_make.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     1144 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_mem_initializer_cpp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4953 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_nuget_task.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      810 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_pat_db.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7181 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_project.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8481 2022-07-06 19:24:04.677826 z3-solver-4.9.1.0/core/scripts/mk_unix_dist.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   143050 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/mk_util.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11676 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/mk_win_dist.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19831 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/nightly.yaml
+-rw-r--r--   0 vsts      (1001) docker     (121)      172 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/policy.json
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     1100 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/pyg2hpp.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    18423 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/release.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      359 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/test-examples-cmake.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      312 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/test-java-cmake.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      396 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/test-jupyter.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      250 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/test-regressions-coverage.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)      157 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/test-regressions.yml
+-rw-r--r--   0 vsts      (1001) docker     (121)       59 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/test-z3.yml
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      353 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/trackall.sh
+-rwxr-xr-x   0 vsts      (1001) docker     (121)    77489 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/update_api.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1792 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/update_header_guards.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1855 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/update_include.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)      351 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/vsts-mac.sh
+-rw-r--r--   0 vsts      (1001) docker     (121)     1099 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/vsts-vs2013.cmd
+-rw-r--r--   0 vsts      (1001) docker     (121)     1334 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/scripts/vsts-vs2017.cmd
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.590393 z3-solver-4.9.1.0/core/src/
+-rw-r--r--   0 vsts      (1001) docker     (121)    10867 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.590393 z3-solver-4.9.1.0/core/src/ackermannization/
+-rw-r--r--   0 vsts      (1001) docker     (121)      501 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      284 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackermannization_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)      442 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackermannize_bv_model_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      372 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackermannize_bv_model_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2819 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackermannize_bv_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      407 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackermannize_bv_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      347 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackermannize_bv_tactic_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     2470 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackr_bound_probe.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      478 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackr_bound_probe.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      709 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackr_helper.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4412 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackr_helper.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2969 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackr_info.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6840 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackr_model_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      445 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/ackr_model_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9095 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/lackr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3970 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/lackr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12716 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/lackr_model_constructor.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1475 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/lackr_model_constructor.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1606 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/lackr_model_converter_lazy.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      370 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/ackermannization/lackr_model_converter_lazy.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.594393 z3-solver-4.9.1.0/core/src/api/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1806 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/api/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    17278 2022-07-06 19:24:04.681826 z3-solver-4.9.1.0/core/src/api/api_algebraic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6608 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_arith.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12639 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_array.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    55592 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_ast.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4905 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_ast_map.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      783 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_ast_map.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4040 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_ast_vector.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      824 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_ast_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13894 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_bv.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3541 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_config_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    14520 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_context.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10275 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_context.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    25541 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_datalog.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1236 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_datalog.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    23225 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_datatype.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    47134 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_fpa.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6592 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_goal.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      682 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_goal.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4117 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_log.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    14637 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_model.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2033 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_model.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15502 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_numeral.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    15556 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_opt.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6635 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9638 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_parsers.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3372 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_pb.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2074 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_polynomial.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      596 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_polynomial.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4650 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_qe.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    19880 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_quant.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8792 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_rcf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12498 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_seq.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    36750 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1744 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2510 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_special_relations.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3722 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_stats.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      679 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_stats.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16605 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1700 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7619 2022-07-06 19:24:04.685826 z3-solver-4.9.1.0/core/src/api/api_util.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.594393 z3-solver-4.9.1.0/core/src/api/c++/
+-rw-r--r--   0 vsts      (1001) docker     (121)   180390 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/c++/z3++.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.594393 z3-solver-4.9.1.0/core/src/api/dll/
+-rw-r--r--   0 vsts      (1001) docker     (121)      447 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dll/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      544 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dll/dll.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.598394 z3-solver-4.9.1.0/core/src/api/dotnet/
+-rw-r--r--   0 vsts      (1001) docker     (121)     7896 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/AST.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     4190 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/ASTMap.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     7953 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/ASTVector.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     2160 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/AlgebraicNum.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     2465 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/ApplyResult.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)    10533 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/ArithExpr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      546 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/ArithSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1073 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/ArrayExpr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1735 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/ArraySort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      876 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/BitVecExpr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     2982 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/BitVecNum.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      748 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/BitVecSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1348 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/BoolExpr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      635 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/BoolSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     5890 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      641 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/CharSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     3779 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/Constructor.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1205 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/ConstructorList.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)   183926 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/Context.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      721 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/DatatypeExpr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     2950 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/DatatypeSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      553 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/Deprecated.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     3652 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/EnumSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)    81752 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/Expr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1021 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/FPExpr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     6309 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/FPNum.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      747 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/FPRMExpr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     3709 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/FPRMNum.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      754 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/FPRMSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1132 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/FPSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      666 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/FiniteDomainExpr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     2734 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/FiniteDomainNum.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1195 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/FiniteDomainSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)    11689 2022-07-06 19:24:04.689826 z3-solver-4.9.1.0/core/src/api/dotnet/Fixedpoint.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)    13050 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/FuncDecl.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     6359 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/FuncInterp.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     4099 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Global.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     8839 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Goal.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     2243 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/IDecRefQueue.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      694 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/IntExpr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     2734 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/IntNum.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      714 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/IntSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1546 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/IntSymbol.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     4341 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Lambda.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     3338 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/ListSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1849 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Log.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      209 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Microsoft.Z3.Sharp.pc.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     3964 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Microsoft.Z3.csproj.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     1543 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Microsoft.Z3.props
+-rw-r--r--   0 vsts      (1001) docker     (121)      596 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Microsoft.Z3.snk
+-rw-r--r--   0 vsts      (1001) docker     (121)      477 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Microsoft.Z3.targets
+-rw-r--r--   0 vsts      (1001) docker     (121)      423 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Microsoft.Z3.targets.in
+-rw-r--r--   0 vsts      (1001) docker     (121)    11842 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Model.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)    48516 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/NativeContext.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     2975 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/NativeFuncInterp.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)    13104 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/NativeModel.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)    16054 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/NativeSolver.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)    14906 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Optimize.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     3339 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/ParamDescrs.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     5002 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Params.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1635 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Pattern.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     2649 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Probe.cs
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.598394 z3-solver-4.9.1.0/core/src/api/dotnet/Properties/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1605 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Properties/AssemblyInfo.cs.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     9040 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Quantifier.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     2733 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/RatNum.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      706 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/ReExpr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      730 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/ReSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      702 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/RealExpr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      715 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/RealSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1391 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/RelationSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      885 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/SeqExpr.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      560 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/SeqSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      767 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/SetSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)    18335 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Solver.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     5399 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Sort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     6270 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Statistics.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      663 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Status.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     1593 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/StringSymbol.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     3538 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Symbol.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     3670 2022-07-06 19:24:04.693826 z3-solver-4.9.1.0/core/src/api/dotnet/Tactic.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     2018 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/dotnet/TupleSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      835 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/dotnet/UninterpretedSort.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)    11525 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/dotnet/UserPropagator.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     2578 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/dotnet/Version.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      817 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/dotnet/Z3Exception.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)     3270 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/dotnet/Z3Object.cs
+-rw-r--r--   0 vsts      (1001) docker     (121)      535 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/dotnet/cmake_install_gac.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (121)      653 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/dotnet/cmake_uninstall_gac.cmake.in
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.602393 z3-solver-4.9.1.0/core/src/api/java/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5055 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/AST.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      437 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ASTDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     2739 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ASTMap.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     6162 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ASTVector.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1844 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/AlgebraicNum.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1531 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ApplyResult.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      480 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ApplyResultDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      444 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ArithExpr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      376 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ArithSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      454 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ArrayExpr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1405 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ArraySort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      454 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/AstMapDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      469 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/AstVectorDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      672 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/BitVecExpr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1682 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/BitVecNum.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      588 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/BitVecSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      477 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/BoolExpr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      415 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/BoolSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     7013 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      431 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/CharSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     3401 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/Constructor.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      285 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ConstructorDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      845 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ConstructorList.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      301 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ConstructorListDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)   136585 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/Context.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      452 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/DatatypeExpr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     2806 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/DatatypeSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     2999 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/EnumSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)    68960 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/Expr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      664 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FPExpr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     5633 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FPNum.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      381 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FPRMExpr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     3127 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FPRMNum.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      479 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FPRMSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      847 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FPSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      501 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FiniteDomainExpr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1429 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FiniteDomainNum.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      854 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FiniteDomainSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     9854 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/Fixedpoint.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      480 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FixedpointDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)    10469 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FuncDecl.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     4865 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FuncInterp.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      479 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FuncInterpDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      497 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/FuncInterpEntryDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     3180 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/Global.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     6652 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/Goal.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      449 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/GoalDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     2366 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/IDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      445 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/IntExpr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1339 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/IntNum.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      440 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/IntSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1143 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/IntSymbol.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     3172 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/Lambda.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     2575 2022-07-06 19:24:04.697826 z3-solver-4.9.1.0/core/src/api/java/ListSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1450 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Log.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     9203 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Model.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      450 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/ModelDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     3230 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/NativeStatic.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    12035 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Optimize.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      466 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/OptimizeDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     2263 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/ParamDescrs.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      484 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/ParamDescrsDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     3202 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Params.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      454 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/ParamsDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1246 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Pattern.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1483 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Probe.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      455 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/ProbeDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     7951 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Quantifier.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      234 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/README
+-rw-r--r--   0 vsts      (1001) docker     (121)     1809 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/RatNum.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      453 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/ReExpr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      370 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/ReSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      415 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/RealExpr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      441 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/RealSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1053 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/RelationSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      459 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/SeqExpr.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      364 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/SeqSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      492 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/SetSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)    11277 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Solver.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      442 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/SolverDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     3718 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Sort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     4611 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Statistics.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      470 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/StatisticsDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      797 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Status.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1086 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/StringSymbol.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     2317 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Symbol.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     2543 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Tactic.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      459 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/TacticDecRefQueue.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1509 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/TupleSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      520 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/UninterpretedSort.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     2221 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Version.java
+-rw-r--r--   0 vsts      (1001) docker     (121)      702 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Z3Exception.java
+-rw-r--r--   0 vsts      (1001) docker     (121)     1758 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/Z3Object.java
+-rw-r--r--   0 vsts      (1001) docker     (121)       66 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/java/manifest
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.602393 z3-solver-4.9.1.0/core/src/api/js/
+-rw-r--r--   0 vsts      (1001) docker     (121)        9 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/js/.nvmrc
+-rw-r--r--   0 vsts      (1001) docker     (121)       99 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/js/.prettierrc.json
+-rw-r--r--   0 vsts      (1001) docker     (121)     7690 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/js/PUBLISHED_README.md
+-rw-r--r--   0 vsts      (1001) docker     (121)      890 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/js/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.578393 z3-solver-4.9.1.0/core/src/api/js/examples/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.602393 z3-solver-4.9.1.0/core/src/api/js/examples/high-level/
+-rw-r--r--   0 vsts      (1001) docker     (121)     5915 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/js/examples/high-level/miracle-sudoku.ts
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.602393 z3-solver-4.9.1.0/core/src/api/js/examples/low-level/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2205 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/js/examples/low-level/example-raw.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)    12715 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/js/examples/low-level/test-ts-api.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)      180 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/js/jest.config.js
+-rw-r--r--   0 vsts      (1001) docker     (121)   410649 2022-07-06 19:24:04.701826 z3-solver-4.9.1.0/core/src/api/js/package-lock.json
+-rw-r--r--   0 vsts      (1001) docker     (121)     1737 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/package.json
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.602393 z3-solver-4.9.1.0/core/src/api/js/scripts/
+-rw-r--r--   0 vsts      (1001) docker     (121)      570 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/scripts/async-fns.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)     3207 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/scripts/build-wasm.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)     3051 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/scripts/make-cc-wrapper.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)    15968 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/scripts/make-ts-wrapper.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)    12210 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/scripts/parse-api.ts
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.602393 z3-solver-4.9.1.0/core/src/api/js/src/
+-rw-r--r--   0 vsts      (1001) docker     (121)      645 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/src/browser.ts
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.602393 z3-solver-4.9.1.0/core/src/api/js/src/high-level/
+-rw-r--r--   0 vsts      (1001) docker     (121)    14054 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/src/high-level/high-level.test.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)    64773 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/src/high-level/high-level.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)       55 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/src/high-level/index.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)    32381 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/src/high-level/types.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)     1653 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/src/high-level/utils.test.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)     1568 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/src/high-level/utils.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)     2219 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/src/jest.ts
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.602393 z3-solver-4.9.1.0/core/src/api/js/src/low-level/
+-rw-r--r--   0 vsts      (1001) docker     (121)      963 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/src/low-level/async-wrapper.js
+-rw-r--r--   0 vsts      (1001) docker     (121)      274 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/src/low-level/index.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)     1110 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/src/node.ts
+-rw-r--r--   0 vsts      (1001) docker     (121)       85 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/tsconfig.build.json
+-rw-r--r--   0 vsts      (1001) docker     (121)      354 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/tsconfig.json
+-rw-r--r--   0 vsts      (1001) docker     (121)      230 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/js/typedoc.json
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.606393 z3-solver-4.9.1.0/core/src/api/julia/
+-rw-r--r--   0 vsts      (1001) docker     (121)      603 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/julia/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     1684 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/julia/README.md
+-rw-r--r--   0 vsts      (1001) docker     (121)    32294 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/julia/z3jl.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.606393 z3-solver-4.9.1.0/core/src/api/ml/
+-rw-r--r--   0 vsts      (1001) docker     (121)      360 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/ml/META.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     9627 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/ml/README.md
+-rw-r--r--   0 vsts      (1001) docker     (121)    87711 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/ml/z3.ml
+-rw-r--r--   0 vsts      (1001) docker     (121)   130000 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/ml/z3.mli
+-rw-r--r--   0 vsts      (1001) docker     (121)      731 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/ml/z3native.ml.pre
+-rw-r--r--   0 vsts      (1001) docker     (121)    19862 2022-07-06 19:24:04.705826 z3-solver-4.9.1.0/core/src/api/ml/z3native_stubs.c.pre
+-rw-r--r--   0 vsts      (1001) docker     (121)      514 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/ml/z3native_stubs.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.606393 z3-solver-4.9.1.0/core/src/api/python/
+-rw-r--r--   0 vsts      (1001) docker     (121)       58 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/.gitignore
+-rw-r--r--   0 vsts      (1001) docker     (121)     5741 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      509 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/README.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      107 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.606393 z3-solver-4.9.1.0/core/src/api/python/z3/
+-rw-r--r--   0 vsts      (1001) docker     (121)      210 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/z3/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   329080 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/z3/z3.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16090 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/z3/z3num.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1113 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/z3/z3poly.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    45224 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/z3/z3printer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5039 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/z3/z3rcf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4723 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/z3/z3types.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11388 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/z3/z3util.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      464 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/python/z3test.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      514 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/z3.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7193 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/core/src/api/z3_algebraic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   255570 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_api.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5735 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_ast_containers.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14123 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_fixedpoint.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    36516 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_fpa.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      462 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_logger.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      377 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_macros.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12312 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_optimization.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1056 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_polynomial.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      450 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_private.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5976 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_rcf.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    26456 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_replayer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1581 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_replayer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3901 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_spacer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2220 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/api/z3_v1.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.610394 z3-solver-4.9.1.0/core/src/ast/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1205 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/ast/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     5965 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/ast/act_cache.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1488 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/ast/act_cache.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    33929 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/ast/arith_decl_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    24406 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/ast/arith_decl_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    28544 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/ast/array_decl_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10353 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/ast/array_decl_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   123605 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/ast/ast.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)   105176 2022-07-06 19:24:04.713827 z3-solver-4.9.1.0/core/src/ast/ast.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9776 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_ll_pp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1527 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_ll_pp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6603 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_lt.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      765 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_lt.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1665 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_pp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4075 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_pp_dot.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      591 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_pp_dot.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3097 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_pp_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1501 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_pp_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2243 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_printer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1671 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_printer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    49621 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_smt2_pp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6593 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_smt2_pp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    29730 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_smt_pp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3466 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_smt_pp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1288 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_trail.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13671 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_translation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3748 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_translation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11327 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5725 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/ast_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    34774 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/bv_decl_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    21372 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/bv_decl_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7078 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/char_decl_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2825 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/char_decl_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3020 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/cost_evaluator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      800 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/cost_evaluator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    57058 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/datatype_decl_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    19278 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/datatype_decl_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5599 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/decl_collector.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1855 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/decl_collector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4529 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/display_dimacs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/display_dimacs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    28780 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/dl_decl_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6338 2022-07-06 19:24:04.717827 z3-solver-4.9.1.0/core/src/ast/dl_decl_plugin.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.610394 z3-solver-4.9.1.0/core/src/ast/euf/
+-rw-r--r--   0 vsts      (1001) docker     (121)      131 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/euf/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    36230 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/euf/euf_egraph.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    15564 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/euf/euf_egraph.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4425 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/euf/euf_enode.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12317 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/euf/euf_enode.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8226 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/euf/euf_etable.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5421 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/euf/euf_etable.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2540 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/euf/euf_justification.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15998 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr2polynomial.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3235 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr2polynomial.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2733 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr2var.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1966 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr2var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4388 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr_abstract.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1537 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr_abstract.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      700 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr_delta_pair.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3370 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr_functors.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2451 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr_functors.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2186 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr_map.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1465 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr_map.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2119 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr_stat.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      978 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr_stat.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4681 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr_substitution.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3234 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/expr_substitution.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      898 2022-07-06 19:24:04.721827 z3-solver-4.9.1.0/core/src/ast/for_each_ast.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8973 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/for_each_ast.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4906 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/for_each_expr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6721 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/for_each_expr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7005 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/format.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7350 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/format.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.610394 z3-solver-4.9.1.0/core/src/ast/fpa/
+-rw-r--r--   0 vsts      (1001) docker     (121)      172 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/fpa/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    21618 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/fpa/bv2fpa_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2197 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/fpa/bv2fpa_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   170799 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/fpa/fpa2bv_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12084 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/fpa/fpa2bv_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13835 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/fpa/fpa2bv_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2135 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/fpa/fpa2bv_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    47947 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/fpa_decl_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    17510 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/fpa_decl_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6003 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/func_decl_dependencies.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2815 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/func_decl_dependencies.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2656 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/has_free_vars.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      385 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/has_free_vars.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1379 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/is_variable_test.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1365 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/justified_expr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5229 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macro_substitution.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1719 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macro_substitution.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.610394 z3-solver-4.9.1.0/core/src/ast/macros/
+-rw-r--r--   0 vsts      (1001) docker     (121)      187 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macros/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     1810 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macros/cond_macro.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15685 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macros/macro_finder.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1724 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macros/macro_finder.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13607 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macros/macro_manager.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3365 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macros/macro_manager.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    32646 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macros/macro_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6067 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macros/macro_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1962 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macros/quantifier_macro_info.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2000 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macros/quantifier_macro_info.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13246 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macros/quasi_macros.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2135 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/macros/quasi_macros.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.614394 z3-solver-4.9.1.0/core/src/ast/normal_forms/
+-rw-r--r--   0 vsts      (1001) docker     (121)      247 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/normal_forms/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    13210 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/normal_forms/defined_names.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2622 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/normal_forms/defined_names.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      892 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/normal_forms/elim_term_ite.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1484 2022-07-06 19:24:04.725827 z3-solver-4.9.1.0/core/src/ast/normal_forms/elim_term_ite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4508 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/normal_forms/name_exprs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1700 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/normal_forms/name_exprs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    30976 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/normal_forms/nnf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1155 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/normal_forms/nnf.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      571 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/normal_forms/nnf_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)    15547 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/normal_forms/pull_quant.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1092 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/normal_forms/pull_quant.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2157 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/num_occurs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1113 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/num_occurs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1353 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/occurs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      397 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/occurs.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.614394 z3-solver-4.9.1.0/core/src/ast/pattern/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1119 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/pattern/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    15504 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/pattern/database.smt2
+-rw-r--r--   0 vsts      (1001) docker     (121)    14917 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/pattern/expr_pattern_match.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3875 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/pattern/expr_pattern_match.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    26717 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/pattern/pattern_inference.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8587 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/pattern/pattern_inference.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9506 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/pb_decl_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4971 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/pb_decl_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4405 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/pp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      349 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/pp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2110 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/pp_params.pyg
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.614394 z3-solver-4.9.1.0/core/src/ast/proofs/
+-rw-r--r--   0 vsts      (1001) docker     (121)      115 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/proofs/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    44936 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/proofs/proof_checker.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4486 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/proofs/proof_checker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    32840 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/proofs/proof_utils.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7464 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/proofs/proof_utils.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3770 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/quantifier_stat.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4164 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/quantifier_stat.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22084 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/recfun_decl_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    14167 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/recfun_decl_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1173 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/recurse_expr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3414 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/recurse_expr_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2218 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/reg_decl_plugins.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      332 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/reg_decl_plugins.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.618394 z3-solver-4.9.1.0/core/src/ast/rewriter/
+-rw-r--r--   0 vsts      (1001) docker     (121)      991 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/rewriter/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    70741 2022-07-06 19:24:04.729827 z3-solver-4.9.1.0/core/src/ast/rewriter/arith_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8245 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/arith_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    27948 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/array_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3306 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/array_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3632 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/ast_counter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2382 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/ast_counter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12556 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bit2int.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2158 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bit2int.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.618394 z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/
+-rw-r--r--   0 vsts      (1001) docker     (121)      139 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     4070 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/bit_blaster.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2336 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/bit_blaster.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    27664 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/bit_blaster_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1031 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/bit_blaster_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7574 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/bit_blaster_tpl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    40789 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/bit_blaster_tpl_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    34233 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bool_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9447 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bool_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    26718 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bv_bounds.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4539 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bv_bounds.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3524 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bv_elim.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      992 2022-07-06 19:24:04.733827 z3-solver-4.9.1.0/core/src/ast/rewriter/bv_elim.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    93415 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/bv_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    11021 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/bv_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2799 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/cached_var_subst.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1210 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/cached_var_subst.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2671 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/char_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1349 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/char_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4813 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/datatype_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      710 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/datatype_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12301 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/der.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6590 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/der.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4480 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/distribute_forall.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1956 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/distribute_forall.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1351 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/dl_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      583 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/dl_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5648 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/elim_bounds.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1814 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/elim_bounds.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12570 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/enum2bv_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1074 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/enum2bv_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4284 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/expr_replacer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1463 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/expr_replacer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5727 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/expr_safe_replace.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      939 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/expr_safe_replace.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3787 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/factor_equivs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5146 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/factor_equivs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10477 2022-07-06 19:24:04.737827 z3-solver-4.9.1.0/core/src/ast/rewriter/factor_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2286 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/factor_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    28725 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/fpa_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3795 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/fpa_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2619 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/func_decl_replace.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      794 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/func_decl_replace.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5586 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/hoist_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2571 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/hoist_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5533 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/inj_axiom.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      299 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/inj_axiom.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1103 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/label_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      682 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/label_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4574 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/maximize_ac_sharing.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3282 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/maximize_ac_sharing.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1181 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/mk_extract_proc.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      620 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/mk_extract_proc.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3490 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/mk_simplified_app.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      674 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/mk_simplified_app.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    43649 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/pb2bv_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1018 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/pb2bv_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9464 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/pb_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1680 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/pb_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8357 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/pb_rewriter_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6452 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/poly_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    36735 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/poly_rewriter_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2681 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/push_app_ite.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2067 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/push_app_ite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11514 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/quant_hoist.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2017 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/quant_hoist.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1002 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/recfun_replace.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      900 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/recfun_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      604 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/recfun_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11498 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    15309 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5573 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/rewriter.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    29732 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/rewriter_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1305 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/rewriter_types.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    46242 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/seq_axioms.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4469 2022-07-06 19:24:04.741827 z3-solver-4.9.1.0/core/src/ast/rewriter/seq_axioms.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    23309 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/rewriter/seq_eq_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6280 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/rewriter/seq_eq_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   199846 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/rewriter/seq_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    18897 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/rewriter/seq_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6583 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/rewriter/seq_skolem.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10213 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/rewriter/seq_skolem.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    35818 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/rewriter/th_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1904 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/rewriter/th_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4058 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/rewriter/value_sweep.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1575 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/rewriter/value_sweep.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9032 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/rewriter/var_subst.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3467 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/rewriter/var_subst.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1005 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/scoped_proof.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    64489 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/seq_decl_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    28118 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/seq_decl_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3562 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/shared_occs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2102 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/shared_occs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2609 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/special_relations_decl_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4469 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/special_relations_decl_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    24694 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/static_features.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9198 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/static_features.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.618394 z3-solver-4.9.1.0/core/src/ast/substitution/
+-rw-r--r--   0 vsts      (1001) docker     (121)      167 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/substitution/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     1351 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/substitution/expr_offset.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2457 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/substitution/expr_offset_map.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1738 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/substitution/matcher.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1297 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/substitution/matcher.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11632 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/substitution/substitution.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7339 2022-07-06 19:24:04.745827 z3-solver-4.9.1.0/core/src/ast/substitution/substitution.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    28561 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/ast/substitution/substitution_tree.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4273 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/ast/substitution/substitution_tree.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5112 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/ast/substitution/unifier.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1817 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/ast/substitution/unifier.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2923 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/ast/substitution/var_offset_map.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3000 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/ast/used_symbols.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3267 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/ast/used_vars.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1426 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/ast/used_vars.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11738 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/ast/value_generator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      744 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/ast/value_generator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2871 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/ast/well_sorted.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      288 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/ast/well_sorted.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.618394 z3-solver-4.9.1.0/core/src/cmd_context/
+-rw-r--r--   0 vsts      (1001) docker     (121)      323 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      190 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/README
+-rw-r--r--   0 vsts      (1001) docker     (121)    36300 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/basic_cmds.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      314 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/basic_cmds.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    75767 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/cmd_context.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    23447 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/cmd_context.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1470 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/cmd_context_to_goal.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      317 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/cmd_context_to_goal.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      877 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/cmd_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3575 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/cmd_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1905 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/echo_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      495 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/echo_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2913 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/eval_cmd.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      237 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/eval_cmd.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.622394 z3-solver-4.9.1.0/core/src/cmd_context/extra_cmds/
+-rw-r--r--   0 vsts      (1001) docker     (121)      184 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/extra_cmds/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    21125 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/extra_cmds/dbg_cmds.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      275 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/extra_cmds/dbg_cmds.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8058 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/extra_cmds/polynomial_cmds.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      282 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/extra_cmds/polynomial_cmds.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1591 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/extra_cmds/subpaving_cmds.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      266 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/extra_cmds/subpaving_cmds.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1583 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/parametric_cmd.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2501 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/parametric_cmd.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    36727 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/pdecl.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    16022 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/pdecl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4841 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/simplify_cmd.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      306 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/simplify_cmd.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    35506 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/tactic_cmds.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1340 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/tactic_cmds.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1336 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/tactic_manager.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2151 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/cmd_context/tactic_manager.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.582393 z3-solver-4.9.1.0/core/src/math/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.622394 z3-solver-4.9.1.0/core/src/math/automata/
+-rw-r--r--   0 vsts      (1001) docker     (121)       90 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/math/automata/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      306 2022-07-06 19:24:04.749827 z3-solver-4.9.1.0/core/src/math/automata/automaton.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    25355 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/automata/automaton.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      800 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/automata/boolean_algebra.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4668 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/automata/symbolic_automata.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16582 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/automata/symbolic_automata_def.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.622394 z3-solver-4.9.1.0/core/src/math/dd/
+-rw-r--r--   0 vsts      (1001) docker     (121)       96 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/dd/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    28871 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/dd/dd_bdd.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9224 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/dd/dd_bdd.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    44595 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/dd/dd_pdd.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    17301 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/dd/dd_pdd.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      809 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/dd/pdd_eval.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1720 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/dd/pdd_interval.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.622394 z3-solver-4.9.1.0/core/src/math/grobner/
+-rw-r--r--   0 vsts      (1001) docker     (121)      147 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/grobner/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    30190 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/grobner/grobner.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9167 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/grobner/grobner.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    23259 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/grobner/pdd_simplifier.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1305 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/grobner/pdd_simplifier.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16848 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/grobner/pdd_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6947 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/grobner/pdd_solver.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.622394 z3-solver-4.9.1.0/core/src/math/hilbert/
+-rw-r--r--   0 vsts      (1001) docker     (121)       93 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/hilbert/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    20941 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/hilbert/heap_trie.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    36737 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/hilbert/hilbert_basis.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7091 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/hilbert/hilbert_basis.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.622394 z3-solver-4.9.1.0/core/src/math/interval/
+-rw-r--r--   0 vsts      (1001) docker     (121)      115 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/interval/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      321 2022-07-06 19:24:04.753827 z3-solver-4.9.1.0/core/src/math/interval/README
+-rw-r--r--   0 vsts      (1001) docker     (121)     3933 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/interval/dep_intervals.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    16433 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/interval/dep_intervals.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15040 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/interval/interval.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    70016 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/interval/interval_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      308 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/interval/interval_mpq.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.630394 z3-solver-4.9.1.0/core/src/math/lp/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1209 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     1698 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/binary_heap_priority_queue.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2332 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/binary_heap_priority_queue.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6386 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/binary_heap_priority_queue_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1100 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/binary_heap_upair_queue.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1547 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/binary_heap_upair_queue.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3506 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/binary_heap_upair_queue_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10018 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/bound_analyzer_on_row.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      505 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/breakpoint.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6918 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/column_info.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1518 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/column_namer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1477 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/conversion_helper.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1281 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/core_solver_pretty_printer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3242 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/core_solver_pretty_printer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14950 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/core_solver_pretty_printer_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18072 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/cross_nested.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2192 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/dense_matrix.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2960 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/dense_matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5668 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/dense_matrix_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17506 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/emonics.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12694 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/emonics.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2294 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/eta_matrix.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2393 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/eta_matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4168 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/eta_matrix_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3260 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/explanation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3986 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/factorization.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4525 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/factorization.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      910 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/factorization_factory_imp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      724 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/factorization_factory_imp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8115 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/general_matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15490 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/gomory.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      766 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/gomory.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    19154 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/hnf.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10406 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/hnf_cutter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2627 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/hnf_cutter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3821 2022-07-06 19:24:04.757827 z3-solver-4.9.1.0/core/src/math/lp/horner.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1284 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/horner.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1445 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/implied_bound.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1451 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/incremental_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1180 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/indexed_value.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2334 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/indexed_vector.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5616 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/indexed_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2685 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/indexed_vector_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      839 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/indexer_of_constraints.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3116 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/int_branch.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      636 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/int_branch.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3511 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/int_cube.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      803 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/int_cube.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11113 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/int_gcd_test.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2115 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/int_gcd_test.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17815 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/int_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4251 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/int_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10490 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lar_constraints.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      307 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lar_core_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    30779 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lar_core_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7398 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lar_core_solver_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      396 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lar_solution_signature.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    96890 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lar_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    32882 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lar_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5755 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lar_term.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      856 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lia_move.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4365 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lp_api.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    28057 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lp_bound_propagator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13646 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lp_core_solver_base.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    25854 2022-07-06 19:24:04.761827 z3-solver-4.9.1.0/core/src/math/lp/lp_core_solver_base.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    34703 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_core_solver_base_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2037 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_dual_core_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6155 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_dual_core_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    26448 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_dual_core_solver_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      520 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_dual_simplex.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2404 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_dual_simplex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14952 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_dual_simplex_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1460 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_primal_core_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    39887 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_primal_core_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    52683 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_primal_core_solver_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16142 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_primal_core_solver_tableau_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1416 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_primal_simplex.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2660 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_primal_simplex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13929 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_primal_simplex_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      937 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_settings.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    15166 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_settings.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3507 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_settings_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3093 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7834 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    19603 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_solver_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2413 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_types.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      325 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_utils.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6713 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lp_utils.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5522 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lu.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12164 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lu.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    32619 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/lu_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      995 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/matrix.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1683 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3582 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/matrix_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1050 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/mon_eq.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3137 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/monic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9946 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/monomial_bounds.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1126 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/monomial_bounds.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    29718 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/mps_reader.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13857 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/nex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    20843 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/nex_creator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9050 2022-07-06 19:24:04.765827 z3-solver-4.9.1.0/core/src/math/lp/nex_creator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22817 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_basics_lemmas.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4217 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_basics_lemmas.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4660 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_common.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3241 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_common.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    62349 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_core.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    19818 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_core.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2636 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_defs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17097 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_intervals.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4291 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_intervals.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2477 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_monotone_lemmas.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      572 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_monotone_lemmas.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13718 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_order_lemmas.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2767 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_order_lemmas.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4134 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_settings.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1665 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1096 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7050 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_tangent_lemmas.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1045 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nla_tangent_lemmas.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9080 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nra_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1089 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/nra_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13508 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/numeric_pair.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5639 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/permutation_matrix.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4579 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/permutation_matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10044 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/permutation_matrix_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      205 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/random_updater.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      887 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/random_updater.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2059 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/random_updater_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2367 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/row_eta_matrix.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2269 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/row_eta_matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5521 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/row_eta_matrix_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      300 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/scaler.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2037 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/scaler.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8195 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/scaler_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      947 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/sparse_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2939 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/square_dense_submatrix.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7152 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/square_dense_submatrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13206 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/square_dense_submatrix_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10910 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/square_sparse_matrix.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    15419 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/square_sparse_matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    45981 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/square_sparse_matrix_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4571 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/stacked_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4375 2022-07-06 19:24:04.769827 z3-solver-4.9.1.0/core/src/math/lp/static_matrix.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    13983 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/lp/static_matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12403 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/lp/static_matrix_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1134 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/lp/tail_matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8680 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/lp/test_bound_analyzer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2708 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/lp/u_set.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2099 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/lp/ul_pair.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11532 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/lp/var_eqs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4150 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/lp/var_register.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.634394 z3-solver-4.9.1.0/core/src/math/polynomial/
+-rw-r--r--   0 vsts      (1001) docker     (121)      331 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/polynomial/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      235 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/polynomial/README
+-rw-r--r--   0 vsts      (1001) docker     (121)   127290 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/polynomial/algebraic_numbers.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    15844 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/polynomial/algebraic_numbers.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2232 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/polynomial/algebraic_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     4452 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/polynomial/linear_eq_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   287495 2022-07-06 19:24:04.773827 z3-solver-4.9.1.0/core/src/math/polynomial/polynomial.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    47657 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/polynomial.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8107 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/polynomial_cache.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      831 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/polynomial_cache.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3251 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/polynomial_primes.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1297 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/polynomial_var2value.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    28105 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/rpolynomial.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5902 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/rpolynomial.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4420 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/sexpr2upolynomial.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      540 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/sexpr2upolynomial.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   116680 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/upolynomial.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    37745 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/upolynomial.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    51846 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/upolynomial_factorization.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4050 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/upolynomial_factorization.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15307 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/polynomial/upolynomial_factorization_int.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.634394 z3-solver-4.9.1.0/core/src/math/realclosure/
+-rw-r--r--   0 vsts      (1001) docker     (121)      149 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/realclosure/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    13293 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/realclosure/mpz_matrix.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5767 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/realclosure/mpz_matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1162 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/realclosure/rcf_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)   246522 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/realclosure/realclosure.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12608 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/realclosure/realclosure.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.634394 z3-solver-4.9.1.0/core/src/math/simplex/
+-rw-r--r--   0 vsts      (1001) docker     (121)      130 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/simplex/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     3026 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/simplex/bit_matrix.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3692 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/simplex/bit_matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    43912 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/simplex/model_based_opt.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7126 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/simplex/model_based_opt.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6916 2022-07-06 19:24:04.777828 z3-solver-4.9.1.0/core/src/math/simplex/network_flow.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    19865 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/simplex/network_flow_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2287 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/simplex/simplex.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7619 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/simplex/simplex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    36196 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/simplex/simplex_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12316 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/simplex/sparse_matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18267 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/simplex/sparse_matrix_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2268 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/simplex/sparse_matrix_ops.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.634394 z3-solver-4.9.1.0/core/src/math/subpaving/
+-rw-r--r--   0 vsts      (1001) docker     (121)      207 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    11360 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3665 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      417 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_hwf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1160 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_hwf.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      424 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_mpf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1216 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_mpf.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      418 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_mpff.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      920 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_mpff.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      418 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_mpfx.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      920 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_mpfx.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      411 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_mpq.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      804 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_mpq.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    29828 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_t.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    62982 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_t_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      959 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_types.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.634394 z3-solver-4.9.1.0/core/src/math/subpaving/tactic/
+-rw-r--r--   0 vsts      (1001) docker     (121)      190 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/tactic/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    11490 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/tactic/expr2subpaving.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1051 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/tactic/expr2subpaving.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9246 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/tactic/subpaving_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      484 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/math/subpaving/tactic/subpaving_tactic.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.634394 z3-solver-4.9.1.0/core/src/model/
+-rw-r--r--   0 vsts      (1001) docker     (121)      471 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     6842 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/array_factory.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      837 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/array_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1546 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/char_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10370 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/datatype_factory.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      743 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/datatype_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1846 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/fpa_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13055 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/func_interp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4331 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/func_interp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17635 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/model.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3933 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/model.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4689 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/model2expr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      809 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/model2expr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3571 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/model_core.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3263 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/model_core.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    27862 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/model_evaluator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1765 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/model_evaluator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      560 2022-07-06 19:24:04.781828 z3-solver-4.9.1.0/core/src/model/model_evaluator_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)    26151 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/model_implicant.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3682 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/model_implicant.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18579 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/model_macro_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10704 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/model_macro_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      820 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/model_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     2920 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/model_pp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      320 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/model_pp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12108 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/model_smt2_pp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      489 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/model_smt2_pp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2460 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/model_v2_pp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      351 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/model_v2_pp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1063 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/numeral_factory.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1062 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/numeral_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4202 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/seq_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1630 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/struct_factory.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1018 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/struct_factory.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3235 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/value_factory.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7578 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/model/value_factory.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.638394 z3-solver-4.9.1.0/core/src/muz/
+-rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/README
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.638394 z3-solver-4.9.1.0/core/src/muz/base/
+-rw-r--r--   0 vsts      (1001) docker     (121)      374 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     4585 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/bind_variables.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      918 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/bind_variables.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9790 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_boogie_proof.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2810 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_boogie_proof.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    45567 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_context.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    22039 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_context.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3909 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_costs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2697 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_costs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4574 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_engine_base.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    34320 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_rule.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12305 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_rule.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22668 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_rule_set.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9448 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_rule_set.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1769 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_rule_subsumption_index.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1339 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_rule_subsumption_index.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4107 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_rule_transformer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2779 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_rule_transformer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    21454 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    20032 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/dl_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16404 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/fp_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)    16218 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/hnf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      941 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/hnf.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11874 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/rule_properties.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2251 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/base/rule_properties.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.638394 z3-solver-4.9.1.0/core/src/muz/bmc/
+-rw-r--r--   0 vsts      (1001) docker     (121)      103 2022-07-06 19:24:04.785828 z3-solver-4.9.1.0/core/src/muz/bmc/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    63042 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/bmc/dl_bmc_engine.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1532 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/bmc/dl_bmc_engine.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.638394 z3-solver-4.9.1.0/core/src/muz/clp/
+-rw-r--r--   0 vsts      (1001) docker     (121)      101 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/clp/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     7092 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/clp/clp_context.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      807 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/clp/clp_context.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.638394 z3-solver-4.9.1.0/core/src/muz/dataflow/
+-rw-r--r--   0 vsts      (1001) docker     (121)       88 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/dataflow/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      377 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/dataflow/dataflow.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8957 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/dataflow/dataflow.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2162 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/dataflow/reachability.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.638394 z3-solver-4.9.1.0/core/src/muz/ddnf/
+-rw-r--r--   0 vsts      (1001) docker     (121)      103 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/ddnf/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    29546 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/ddnf/ddnf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1533 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/ddnf/ddnf.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.638394 z3-solver-4.9.1.0/core/src/muz/fp/
+-rw-r--r--   0 vsts      (1001) docker     (121)      238 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/fp/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    47821 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/fp/datalog_parser.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      787 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/fp/datalog_parser.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15652 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/fp/dl_cmds.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      611 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/fp/dl_cmds.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1235 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/fp/dl_register_engine.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      545 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/fp/dl_register_engine.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13892 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/fp/horn_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      633 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/fp/horn_tactic.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.642394 z3-solver-4.9.1.0/core/src/muz/rel/
+-rw-r--r--   0 vsts      (1001) docker     (121)      675 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/rel/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    11055 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/rel/aig_exporter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2030 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/rel/aig_exporter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    32139 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/rel/check_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7024 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/rel/check_relation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14720 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/rel/dl_base.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    50391 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/rel/dl_base.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    24397 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/rel/dl_bound_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6020 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/rel/dl_bound_relation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18538 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/rel/dl_check_table.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5110 2022-07-06 19:24:04.789828 z3-solver-4.9.1.0/core/src/muz/rel/dl_check_table.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    55025 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_compiler.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12475 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_compiler.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18625 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_external_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5419 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_external_relation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   100214 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_finite_product_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    14996 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_finite_product_relation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    46503 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_instruction.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    13335 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_instruction.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    23843 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_interval_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5301 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_interval_relation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16002 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_lazy_table.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    11637 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_lazy_table.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    34292 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_mk_explanations.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2322 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_mk_explanations.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    19449 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_mk_similarity_compressor.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1648 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_mk_similarity_compressor.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    30985 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_mk_simple_joins.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1341 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_mk_simple_joins.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    46802 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_product_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7082 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_product_relation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    67602 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_relation_manager.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    30382 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_relation_manager.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    28208 2022-07-06 19:24:04.793828 z3-solver-4.9.1.0/core/src/muz/rel/dl_sieve_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7789 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/dl_sieve_relation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    54995 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/dl_sparse_table.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    19139 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/dl_sparse_table.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9380 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/dl_table.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3921 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/dl_table.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5275 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/dl_table_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    20028 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/dl_table_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5488 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/dl_table_relation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13375 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/dl_vector_relation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    21688 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/doc.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12246 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/doc.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    27718 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/karr_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2628 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/karr_relation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22528 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/rel_context.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3941 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/rel_context.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8260 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/tbv.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4002 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/tbv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    48305 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/udoc_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6984 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/rel/udoc_relation.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.646394 z3-solver-4.9.1.0/core/src/muz/spacer/
+-rw-r--r--   0 vsts      (1001) docker     (121)      803 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/spacer/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    12176 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_antiunify.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1665 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_antiunify.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4695 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_arith_generalizers.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      578 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_callback.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1454 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_callback.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   139254 2022-07-06 19:24:04.797828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_context.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    40939 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_context.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10884 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_dl_interface.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1974 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_dl_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14082 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_farkas_learner.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1185 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_farkas_learner.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10190 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_generalizers.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4889 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_generalizers.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8265 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_iuc_proof.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1719 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_iuc_proof.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15539 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_iuc_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6479 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_iuc_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5397 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_json.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      922 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_json.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5482 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_legacy_frames.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1415 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_legacy_frames.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3287 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_legacy_mbp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    24425 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_legacy_mev.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3835 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_legacy_mev.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6239 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_manager.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4048 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_manager.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3980 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_matrix.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      750 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2852 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_mbc.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      623 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_mbc.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7060 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_mev_array.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1017 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_mev_array.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6637 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_notes.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    10410 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_pdr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3205 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_pdr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    28026 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_proof_utils.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2498 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_proof_utils.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12909 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_prop_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4747 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_prop_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    89428 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_qe_project.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1282 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_qe_project.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22789 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_quant_generalizer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7363 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_sat_answer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      917 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_sat_answer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3796 2022-07-06 19:24:04.801828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_sem_matcher.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1617 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_sem_matcher.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4862 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_sym_mux.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2270 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_sym_mux.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2287 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_unsat_core_learner.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2560 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_unsat_core_learner.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    26351 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_unsat_core_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3772 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_unsat_core_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    34388 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4037 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/spacer/spacer_util.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.646394 z3-solver-4.9.1.0/core/src/muz/tab/
+-rw-r--r--   0 vsts      (1001) docker     (121)      101 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/tab/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    58114 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/tab/tab_context.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      824 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/tab/tab_context.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.646394 z3-solver-4.9.1.0/core/src/muz/transforms/
+-rw-r--r--   0 vsts      (1001) docker     (121)      805 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    10577 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_array_blast.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1747 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_array_blast.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3566 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_array_eq_rewrite.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      966 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_array_eq_rewrite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10470 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_array_instantiation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5633 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_array_instantiation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2248 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_backwards.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      593 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_backwards.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11841 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_bit_blast.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      579 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_bit_blast.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6697 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_coalesce.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1185 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_coalesce.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6737 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_coi_filter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1029 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_coi_filter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      638 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_different.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6419 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_elim_term_ite.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      829 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_elim_term_ite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6141 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_filter_rules.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2401 2022-07-06 19:24:04.805828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_filter_rules.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    19752 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_interp_tail_simplifier.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2997 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_interp_tail_simplifier.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10871 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_karr_invariants.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_karr_invariants.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5696 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_loop_counter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1075 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_loop_counter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13782 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_magic_sets.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4217 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_magic_sets.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4392 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_magic_symbolic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      704 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_magic_symbolic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13079 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_quantifier_abstraction.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1472 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_quantifier_abstraction.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9577 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_quantifier_instantiation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1878 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_quantifier_instantiation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    30893 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_rule_inliner.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7090 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_rule_inliner.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7929 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_scale.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1109 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_scale.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4220 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_separate_negated_tails.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1422 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_separate_negated_tails.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    31324 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_slice.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2836 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_slice.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12907 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_subsumption_checker.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2537 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_subsumption_checker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13624 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_synchronize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4244 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_synchronize.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14778 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_unbound_compressor.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2888 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_unbound_compressor.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1860 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_unfold.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      988 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_unfold.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4247 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_transforms.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      355 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/muz/transforms/dl_transforms.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.650394 z3-solver-4.9.1.0/core/src/nlsat/
+-rw-r--r--   0 vsts      (1001) docker     (121)      251 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/nlsat/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     3470 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_assignment.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1006 2022-07-06 19:24:04.809828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_clause.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2031 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_clause.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    29391 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_evaluator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1415 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_evaluator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    75082 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_explain.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3508 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_explain.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    30681 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_interval_set.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3424 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_interval_set.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4352 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_justification.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1406 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     2704 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_scoped_literal_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   139432 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6854 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1904 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_types.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5911 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/nlsat_types.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.650394 z3-solver-4.9.1.0/core/src/nlsat/tactic/
+-rw-r--r--   0 vsts      (1001) docker     (121)      238 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/tactic/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    14350 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/tactic/goal2nlsat.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1544 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/tactic/goal2nlsat.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8835 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/tactic/nlsat_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      461 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/tactic/nlsat_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2337 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/tactic/qfnra_nlsat_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      503 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/nlsat/tactic/qfnra_nlsat_tactic.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.650394 z3-solver-4.9.1.0/core/src/opt/
+-rw-r--r--   0 vsts      (1001) docker     (121)      421 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/opt/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    38366 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/opt/maxcore.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      720 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/opt/maxcore.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6546 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/opt/maxlex.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      411 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/opt/maxlex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13065 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/opt/maxsmt.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6701 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/opt/maxsmt.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5124 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/opt/opt_cmds.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      350 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/opt/opt_cmds.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    61201 2022-07-06 19:24:04.813828 z3-solver-4.9.1.0/core/src/opt/opt_context.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    14147 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_context.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14064 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_cores.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2047 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_cores.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9087 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_lns.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2483 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_lns.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      468 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_mux.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3387 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     3303 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_pareto.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2678 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_pareto.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    24914 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_parse.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      442 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_parse.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7282 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_preprocess.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1041 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_preprocess.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7432 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_sls_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18868 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5755 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/opt_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    19967 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/optsmt.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2256 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/optsmt.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    27288 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/pb_sls.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      844 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/pb_sls.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4710 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/sortmax.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3174 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/totalizer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1202 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/totalizer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10471 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/wmax.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      414 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/opt/wmax.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.650394 z3-solver-4.9.1.0/core/src/params/
+-rw-r--r--   0 vsts      (1001) docker     (121)      487 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     1668 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/arith_rewriter_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)      873 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/array_rewriter_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)      862 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/bit_blaster_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1182 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/bool_rewriter_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     1443 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/bv_rewriter_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     7280 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/context_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2177 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/context_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      309 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/fpa2bv_rewriter_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)      305 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/fpa_rewriter_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     1422 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/pattern_inference_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1355 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/pattern_inference_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1507 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/pattern_inference_params_helper.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)      724 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/poly_rewriter_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     1062 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/rewriter_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)      221 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/params/seq_rewriter_params.pyg
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.582393 z3-solver-4.9.1.0/core/src/parsers/
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.650394 z3-solver-4.9.1.0/core/src/parsers/smt2/
+-rw-r--r--   0 vsts      (1001) docker     (121)      152 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/parsers/smt2/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     1111 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/parsers/smt2/marshal.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      433 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/parsers/smt2/marshal.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   130536 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/parsers/smt2/smt2parser.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      633 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/parsers/smt2/smt2parser.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11474 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/parsers/smt2/smt2scanner.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2884 2022-07-06 19:24:04.817828 z3-solver-4.9.1.0/core/src/parsers/smt2/smt2scanner.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.650394 z3-solver-4.9.1.0/core/src/parsers/util/
+-rw-r--r--   0 vsts      (1001) docker     (121)      193 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/parsers/util/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     1689 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/parsers/util/cost_parser.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      656 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/parsers/util/cost_parser.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      405 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/parsers/util/parser_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     3361 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/parsers/util/pattern_validation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      953 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/parsers/util/pattern_validation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13917 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/parsers/util/scanner.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1865 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/parsers/util/scanner.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3565 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/parsers/util/simple_parser.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1673 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/parsers/util/simple_parser.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.654394 z3-solver-4.9.1.0/core/src/qe/
+-rw-r--r--   0 vsts      (1001) docker     (121)      443 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.654394 z3-solver-4.9.1.0/core/src/qe/lite/
+-rw-r--r--   0 vsts      (1001) docker     (121)      128 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/lite/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    88561 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/lite/qe_lite.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1948 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/lite/qe_lite.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.654394 z3-solver-4.9.1.0/core/src/qe/mbp/
+-rw-r--r--   0 vsts      (1001) docker     (121)      213 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    24770 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/mbp_arith.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1719 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/mbp_arith.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    60573 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/mbp_arrays.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1091 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/mbp_arrays.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11163 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/mbp_datatypes.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      991 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/mbp_datatypes.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10814 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/mbp_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3614 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/mbp_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15291 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/mbp_solve_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1390 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/mbp_solve_plugin.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    43940 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/mbp_term_graph.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4736 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/mbp/mbp_term_graph.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    73862 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/nlarith_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4752 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/nlarith_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    34705 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/nlqsat.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      573 2022-07-06 19:24:04.821828 z3-solver-4.9.1.0/core/src/qe/nlqsat.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    92355 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12062 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    96004 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_arith_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10296 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_array_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5550 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_bool_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2535 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_bv_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1946 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_cmd.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      303 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_cmd.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    30943 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_datatype_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8042 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_dl_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    18384 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_mbi.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4820 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_mbi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14736 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_mbp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1636 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_mbp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3613 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      458 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qe_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    49526 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qsat.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4927 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/qe/qsat.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.662394 z3-solver-4.9.1.0/core/src/sat/
+-rw-r--r--   0 vsts      (1001) docker     (121)      938 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    11849 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/dimacs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3217 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/dimacs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    31073 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_aig_cuts.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9166 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_aig_cuts.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9746 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_aig_finder.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1757 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_aig_finder.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3040 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_allocator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15302 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_anf_simplifier.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3530 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_anf_simplifier.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16870 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_asymm_branch.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2677 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_asymm_branch.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      899 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_asymm_branch_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)    10836 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_bcd.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2241 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_bcd.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9197 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_big.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2511 2022-07-06 19:24:04.825828 z3-solver-4.9.1.0/core/src/sat/sat_big.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15094 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_binspr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3462 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_binspr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7294 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_clause.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8170 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_clause.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2390 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_clause_set.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1135 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_clause_set.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1127 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_clause_use_list.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3691 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_clause_use_list.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8343 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_cleaner.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      892 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_cleaner.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10707 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_config.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6218 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_config.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    26607 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_cut_simplifier.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6678 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_cut_simplifier.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8125 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_cutset.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6677 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_cutset.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    29615 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_cutset_compute_shift.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    19144 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_ddfw.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7292 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_ddfw.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    32192 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_drat.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6327 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_drat.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10797 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_elim_eqs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1247 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_elim_eqs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10323 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_elim_vars.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1831 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_elim_vars.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5584 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_extension.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    20068 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_gc.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8709 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_integrity_checker.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1045 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_integrity_checker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2895 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_justification.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    27706 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_local_search.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10184 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_local_search.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    94612 2022-07-06 19:24:04.829828 z3-solver-4.9.1.0/core/src/sat/sat_lookahead.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    25137 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_lookahead.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9212 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_lut_finder.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2766 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_lut_finder.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16925 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_model_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5417 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_model_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7378 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_mus.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1627 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_mus.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    23162 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_npn3_finder.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5251 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_npn3_finder.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9433 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_parallel.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3227 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_parallel.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13579 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     8490 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_prob.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4083 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_prob.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10701 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_probing.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2628 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_probing.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10522 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_scc.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1587 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_scc.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      357 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_scc_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)    78437 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_simplifier.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9102 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_simplifier.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4427 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_simplifier_params.pyg
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.662394 z3-solver-4.9.1.0/core/src/sat/sat_solver/
+-rw-r--r--   0 vsts      (1001) docker     (121)      217 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_solver/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    40388 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_solver/inc_sat_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      631 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/sat_solver/inc_sat_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   171418 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    35517 2022-07-06 19:24:04.833828 z3-solver-4.9.1.0/core/src/sat/sat_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1872 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/sat_solver_core.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5032 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/sat_types.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4441 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/sat_watched.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5923 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/sat_watched.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8002 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/sat_xor_finder.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2544 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/sat_xor_finder.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.666394 z3-solver-4.9.1.0/core/src/sat/smt/
+-rw-r--r--   0 vsts      (1001) docker     (121)      914 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    19668 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/arith_axioms.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4404 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/arith_diagnostics.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    25688 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/arith_internalize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    11239 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/arith_proof_checker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    55744 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/arith_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    19978 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/arith_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    26968 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/array_axioms.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5841 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/array_diagnostics.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8619 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/array_internalize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    11878 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/array_model.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9463 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/array_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    14538 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/array_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4016 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/atom2bool_var.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1000 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/atom2bool_var.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1949 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/ba_xor.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4993 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/bv_ackerman.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1985 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/bv_ackerman.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13251 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/bv_delay_internalize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    29463 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/bv_internalize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3958 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/bv_invariant.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    34926 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/bv_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    18435 2022-07-06 19:24:04.837828 z3-solver-4.9.1.0/core/src/sat/smt/bv_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    32588 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/dt_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6904 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/dt_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6647 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/euf_ackerman.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2351 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/euf_ackerman.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17163 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/euf_internalize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/euf_invariant.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12208 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/euf_model.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6236 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/euf_proof.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10581 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/euf_relevancy.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5611 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/euf_relevancy.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    36792 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/euf_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    19990 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/euf_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15245 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/fpa_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2726 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/fpa_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8019 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/pb_card.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2159 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/pb_card.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1879 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/pb_constraint.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5869 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/pb_constraint.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9869 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/pb_internalize.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9357 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/pb_pb.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2715 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/pb_pb.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   130799 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/pb_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    18410 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/pb_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1453 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/pb_solver_interface.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1241 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/q_clause.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4473 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/q_clause.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    23629 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/q_ematch.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5499 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/q_ematch.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8588 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/q_eval.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1403 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/q_eval.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   162088 2022-07-06 19:24:04.841828 z3-solver-4.9.1.0/core/src/sat/smt/q_mam.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1473 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/q_mam.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    20963 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/q_mbi.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4618 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/q_mbi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12086 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/q_model_fixer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4079 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/q_model_fixer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9561 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/q_queue.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2106 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/q_queue.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11172 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/q_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3032 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/q_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11639 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/recfun_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4630 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/recfun_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      818 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/sat_internalizer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2047 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/sat_smt.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11029 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/sat_th.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    11528 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/sat_th.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9321 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/user_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6376 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/user_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14902 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/smt/xor_solver.d
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.670394 z3-solver-4.9.1.0/core/src/sat/tactic/
+-rw-r--r--   0 vsts      (1001) docker     (121)      194 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/tactic/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    35680 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/tactic/goal2sat.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2771 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/tactic/goal2sat.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10509 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/tactic/sat2goal.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2749 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/tactic/sat2goal.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9019 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/tactic/sat_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      772 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/sat/tactic/sat_tactic.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.670394 z3-solver-4.9.1.0/core/src/shell/
+-rw-r--r--   0 vsts      (1001) docker     (121)     2061 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     7517 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/datalog_frontend.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      251 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/datalog_frontend.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8529 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/dimacs_frontend.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      257 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/dimacs_frontend.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18857 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/drat_frontend.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      137 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/drat_frontend.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3012 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/lp_frontend.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      162 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/lp_frontend.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15360 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/main.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4337 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/opt_frontend.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      255 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/opt_frontend.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2330 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/options.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4006 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/smtlib_frontend.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      403 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/smtlib_frontend.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1237 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/z3_log_frontend.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      295 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/shell/z3_log_frontend.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.690394 z3-solver-4.9.1.0/core/src/smt/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/smt/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    12501 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/smt/arith_eq_adapter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2461 2022-07-06 19:24:04.845829 z3-solver-4.9.1.0/core/src/smt/arith_eq_adapter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17412 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/arith_eq_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2574 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/arith_eq_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9711 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/database.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14730 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/database.smt
+-rw-r--r--   0 vsts      (1001) docker     (121)    68535 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/diff_logic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22572 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/dyn_ack.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4338 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/dyn_ack.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22263 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/expr_context_simplifier.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2422 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/expr_context_simplifier.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4875 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/fingerprints.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3172 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/fingerprints.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   167885 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/mam.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1480 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/mam.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    24172 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/old_interval.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7120 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/old_interval.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.694395 z3-solver-4.9.1.0/core/src/smt/params/
+-rw-r--r--   0 vsts      (1001) docker     (121)      360 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)      930 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/dyn_ack_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      890 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/dyn_ack_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1809 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/preprocessor_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2146 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/preprocessor_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1999 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/qi_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3586 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/qi_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6390 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/smt_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10549 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/smt_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17135 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/smt_params_helper.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     3412 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/theory_arith_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4156 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/theory_arith_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      931 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/theory_array_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1203 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/theory_array_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1052 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/theory_bv_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1039 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/theory_bv_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      637 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/theory_datatype_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      686 2022-07-06 19:24:04.849829 z3-solver-4.9.1.0/core/src/smt/params/theory_pb_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      533 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/params/theory_pb_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      427 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/params/theory_seq_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      507 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/params/theory_seq_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2335 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/params/theory_str_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4192 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/params/theory_str_params.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.694395 z3-solver-4.9.1.0/core/src/smt/proto_model/
+-rw-r--r--   0 vsts      (1001) docker     (121)      124 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/proto_model/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    12209 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/proto_model/proto_model.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3412 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/proto_model/proto_model.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    21315 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/qi_queue.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3642 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/qi_queue.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3164 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/seq_axioms.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4527 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/seq_axioms.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    40668 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/seq_eq_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9363 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/seq_ne_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3719 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/seq_offset_eq.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1364 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/seq_offset_eq.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    33961 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/seq_regex.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7452 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/seq_regex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1467 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt2_extra_cmds.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      276 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt2_extra_cmds.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3367 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_almost_cg_table.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1785 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_almost_cg_table.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6124 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_arith_value.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1292 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_arith_value.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2800 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_b_justification.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3915 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_bool_var_data.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    45977 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_case_split_queue.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1476 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_case_split_queue.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7895 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_cg_table.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7041 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_cg_table.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6180 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_checker.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1209 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_checker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4708 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_clause.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9157 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_clause.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5637 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_clause_proof.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2119 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_clause_proof.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    59769 2022-07-06 19:24:04.853829 z3-solver-4.9.1.0/core/src/smt/smt_conflict_resolution.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9754 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_conflict_resolution.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    23797 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_consequences.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)   188272 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_context.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    64013 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_context.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16995 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_context_inv.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    28741 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_context_pp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4664 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_context_stat.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12382 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_enode.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    15036 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_enode.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2375 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_eq_justification.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      714 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_failure.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10603 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_farkas_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2783 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_farkas_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9244 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_for_each_relevant_expr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2911 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_for_each_relevant_expr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    21878 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_implied_equalities.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      565 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_implied_equalities.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17935 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_induction.cpp.disabled
+-rw-r--r--   0 vsts      (1001) docker     (121)     4926 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_induction.h.disabled
+-rw-r--r--   0 vsts      (1001) docker     (121)    70087 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_internalizer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    15178 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_justification.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    15086 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_justification.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8472 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_kernel.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9654 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_kernel.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3503 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_literal.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1629 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_literal.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5359 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_lookahead.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      648 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_lookahead.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    21839 2022-07-06 19:24:04.857829 z3-solver-4.9.1.0/core/src/smt/smt_model_checker.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3821 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_model_checker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   102564 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_model_finder.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4594 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_model_finder.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    20692 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_model_generator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9740 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_model_generator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9066 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_parallel.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      436 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_parallel.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    31287 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_quantifier.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5880 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_quantifier.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1724 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_quantifier_instances.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16299 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_quick_checker.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3708 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_quick_checker.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    23903 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_relevancy.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6004 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_relevancy.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    40421 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_setup.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3911 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_setup.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17917 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      513 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      347 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_statistics.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1194 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_statistics.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8597 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_theory.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    20897 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_theory.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1622 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_types.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1698 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_value_sort.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      402 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/smt_value_sort.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2332 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/spanning_tree.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1183 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/spanning_tree_base.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15989 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/spanning_tree_def.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.694395 z3-solver-4.9.1.0/core/src/smt/tactic/
+-rw-r--r--   0 vsts      (1001) docker     (121)      266 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/tactic/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     9936 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/tactic/ctx_solver_simplify_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      496 2022-07-06 19:24:04.861829 z3-solver-4.9.1.0/core/src/smt/tactic/ctx_solver_simplify_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14836 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/tactic/smt_tactic_core.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      844 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/tactic/smt_tactic_core.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3855 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/tactic/unit_subsumption_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      719 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/tactic/unit_subsumption_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      467 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_arith.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    59928 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_arith.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    86410 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_arith_aux.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   141116 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_arith_core.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_arith_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13206 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_arith_eq.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    44997 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_arith_int.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8042 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_arith_inv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    86158 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_arith_nl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18245 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_arith_pp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16883 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_array.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4414 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_array.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    24061 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_array_bapa.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      702 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_array_bapa.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    38789 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_array_base.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9093 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_array_base.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    31628 2022-07-06 19:24:04.865829 z3-solver-4.9.1.0/core/src/smt/theory_array_full.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3641 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_array_full.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    82485 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_bv.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12842 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_bv.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16133 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_char.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2654 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_char.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    43801 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_datatype.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5940 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_datatype.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_dense_diff_logic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10696 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_dense_diff_logic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    44314 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_dense_diff_logic_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      675 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_diff_logic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    13237 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_diff_logic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    45130 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_diff_logic_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9608 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_dl.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      290 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_dl.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1444 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_dummy.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1421 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_dummy.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    24747 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_fpa.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4139 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_fpa.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   143694 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_lra.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2812 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_lra.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1881 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_opt.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      836 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_opt.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    78857 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_pb.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    16098 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_pb.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16770 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_recfun.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4399 2022-07-06 19:24:04.869829 z3-solver-4.9.1.0/core/src/smt/theory_recfun.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   105237 2022-07-06 19:24:04.873829 z3-solver-4.9.1.0/core/src/smt/theory_seq.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    29522 2022-07-06 19:24:04.873829 z3-solver-4.9.1.0/core/src/smt/theory_seq.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1400 2022-07-06 19:24:04.873829 z3-solver-4.9.1.0/core/src/smt/theory_seq_empty.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    43020 2022-07-06 19:24:04.873829 z3-solver-4.9.1.0/core/src/smt/theory_special_relations.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8022 2022-07-06 19:24:04.873829 z3-solver-4.9.1.0/core/src/smt/theory_special_relations.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   396808 2022-07-06 19:24:04.873829 z3-solver-4.9.1.0/core/src/smt/theory_str.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    31268 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/theory_str.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    74390 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/theory_str_mc.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    78101 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/theory_str_regex.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12756 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/theory_user_propagator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6673 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/theory_user_propagator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4464 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/theory_utvpi.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10723 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/theory_utvpi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    32925 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/theory_utvpi_def.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12098 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/theory_wmaxsat.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4920 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/theory_wmaxsat.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      865 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/uses_theory.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      643 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/uses_theory.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4129 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/watch_list.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5754 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/smt/watch_list.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.698395 z3-solver-4.9.1.0/core/src/solver/
+-rw-r--r--   0 vsts      (1001) docker     (121)      408 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.698395 z3-solver-4.9.1.0/core/src/solver/assertions/
+-rw-r--r--   0 vsts      (1001) docker     (121)      140 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/assertions/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    23012 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/assertions/asserted_formulas.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    13686 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/assertions/asserted_formulas.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    16802 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/check_logic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      563 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/check_logic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1714 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/check_sat_result.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3372 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/check_sat_result.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13898 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/combined_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      514 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/combined_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      654 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/combined_solver_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)    11537 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/mus.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1504 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/mus.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1413 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/parallel_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)    27558 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/parallel_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      317 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/parallel_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      504 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/progress_callback.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4019 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/smt_logics.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      995 2022-07-06 19:24:04.877829 z3-solver-4.9.1.0/core/src/solver/smt_logics.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9392 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/solver/solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8704 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/solver/solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6434 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/solver/solver2tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      516 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/solver/solver2tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3094 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/solver/solver_na2as.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1890 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/solver/solver_na2as.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      485 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/solver/solver_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)    13341 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/solver/solver_pool.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1386 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/solver/solver_pool.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12642 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/solver/tactic2solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      983 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/solver/tactic2solver.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.702395 z3-solver-4.9.1.0/core/src/tactic/
+-rw-r--r--   0 vsts      (1001) docker     (121)      489 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/CMakeLists.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.702395 z3-solver-4.9.1.0/core/src/tactic/aig/
+-rw-r--r--   0 vsts      (1001) docker     (121)      141 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/aig/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    57231 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/aig/aig.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2169 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/aig/aig.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3003 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/aig/aig_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      398 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/aig/aig_tactic.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.706395 z3-solver-4.9.1.0/core/src/tactic/arith/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1082 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     5009 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/add_bounds_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      737 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/add_bounds_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4596 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/arith_bounds_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      943 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/arith_bounds_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7637 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/bound_manager.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2709 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/bound_manager.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    30252 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/bound_propagator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10599 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/bound_propagator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    19613 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/bv2int_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4345 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/bv2int_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    22792 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/bv2real_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8499 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/bv2real_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3043 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/card2bv_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3532 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/card2bv_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10738 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/degree_shift_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      729 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/degree_shift_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13172 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/diff_neq_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      753 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/diff_neq_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12766 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/eq2bv_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      533 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/eq2bv_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11133 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/factor_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      447 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/factor_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10817 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/fix_dl_var_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      846 2022-07-06 19:24:04.881829 z3-solver-4.9.1.0/core/src/tactic/arith/fix_dl_var_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    61765 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/fm_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      649 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/fm_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13331 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/lia2card_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      631 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/lia2card_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11585 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/lia2pb_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      511 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/lia2pb_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8164 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/linear_equation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2724 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/linear_equation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17058 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/nla2bv_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      648 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/nla2bv_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5784 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/normalize_bounds_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      611 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/normalize_bounds_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2969 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/pb2bv_model_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      923 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/pb2bv_model_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    38030 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/pb2bv_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      597 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/pb2bv_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    19112 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/probe_arith.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2854 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/probe_arith.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17625 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/propagate_ineqs_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      996 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/propagate_ineqs_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    37167 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/purify_arith_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1855 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/purify_arith_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    14530 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/recover_01_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      764 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/arith/recover_01_tactic.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.710395 z3-solver-4.9.1.0/core/src/tactic/bv/
+-rw-r--r--   0 vsts      (1001) docker     (121)      664 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     9452 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bit_blaster_model_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      564 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bit_blaster_model_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5418 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bit_blaster_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      654 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bit_blaster_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17075 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bv1_blaster_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      990 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bv1_blaster_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6766 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bv_bound_chk_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      466 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bv_bound_chk_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    23632 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bv_bounds_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      745 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bv_bounds_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18044 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bv_size_reduction_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      753 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bv_size_reduction_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    15135 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bvarray2uf_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2152 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bvarray2uf_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3752 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bvarray2uf_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      553 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/bvarray2uf_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4830 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/dt2bv_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      509 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/dt2bv_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10915 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/elim_small_bv_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      511 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/elim_small_bv_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10638 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/max_bv_sharing_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      747 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/bv/max_bv_sharing_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2638 2022-07-06 19:24:04.885829 z3-solver-4.9.1.0/core/src/tactic/converter.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.714395 z3-solver-4.9.1.0/core/src/tactic/core/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1368 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     7023 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/blast_term_ite_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      722 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/blast_term_ite_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    24508 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/cofactor_elim_term_ite.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      700 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/cofactor_elim_term_ite.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2063 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/cofactor_term_ite_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      579 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/cofactor_term_ite_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2094 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/collect_occs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      545 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/collect_occs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6152 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/collect_statistics_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      534 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/collect_statistics_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    20473 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/ctx_simplify_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1807 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/ctx_simplify_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2102 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/der_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      338 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/der_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4433 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/distribute_forall_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      449 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/distribute_forall_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17947 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/dom_simplify_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4339 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/dom_simplify_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5283 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/elim_term_ite_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      542 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/elim_term_ite_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    33793 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/elim_uncnstr_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      512 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/elim_uncnstr_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8848 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/injectivity_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      467 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/injectivity_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3246 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/nnf_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      581 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/nnf_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6781 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/occf_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      743 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/occf_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    21647 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/pb_preprocess_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      579 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/pb_preprocess_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7814 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/propagate_values_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      553 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/propagate_values_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18141 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/reduce_args_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      565 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/reduce_args_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18593 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/reduce_invertible_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      522 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/reduce_invertible_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2902 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/simplify_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1373 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/simplify_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    46582 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/solve_eqs_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      562 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/solve_eqs_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6452 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/special_relations_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1878 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/special_relations_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4893 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/split_clause_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      535 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/split_clause_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    20911 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/symmetry_reduce_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      461 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/symmetry_reduce_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    33057 2022-07-06 19:24:04.889829 z3-solver-4.9.1.0/core/src/tactic/core/tseitin_cnf_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      899 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/core/tseitin_cnf_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3169 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/dependency_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1005 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/dependency_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      749 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/equiv_proof_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1111 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/equiv_proof_converter.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.714395 z3-solver-4.9.1.0/core/src/tactic/fd_solver/
+-rw-r--r--   0 vsts      (1001) docker     (121)      244 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fd_solver/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    13816 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fd_solver/bounded_int2bv_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      358 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fd_solver/bounded_int2bv_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7367 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fd_solver/enum2bv_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      344 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fd_solver/enum2bv_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1281 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fd_solver/fd_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      717 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fd_solver/fd_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5999 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fd_solver/pb2bv_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      355 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fd_solver/pb2bv_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    77411 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fd_solver/smtfd_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      546 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fd_solver/smtfd_solver.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1036 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/filter_model_converter.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.718395 z3-solver-4.9.1.0/core/src/tactic/fpa/
+-rw-r--r--   0 vsts      (1001) docker     (121)      347 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fpa/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     3033 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fpa/fpa2bv_model_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1202 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fpa/fpa2bv_model_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4635 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fpa/fpa2bv_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      468 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fpa/fpa2bv_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4498 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fpa/qffp_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      900 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fpa/qffp_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1994 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fpa/qffplra_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      591 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/fpa/qffplra_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6453 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/generic_model_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1947 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/generic_model_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    20473 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/goal.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8414 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/goal.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      473 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/goal_num_occurs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      616 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/goal_num_occurs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      518 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/goal_shared_occs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1056 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/goal_shared_occs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      590 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/goal_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      249 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/goal_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6208 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/horn_subsume_model_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1905 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/horn_subsume_model_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5352 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/model_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3478 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/model_converter.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.718395 z3-solver-4.9.1.0/core/src/tactic/portfolio/
+-rw-r--r--   0 vsts      (1001) docker     (121)      393 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/portfolio/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     2389 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/portfolio/default_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      497 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/portfolio/default_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5762 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/portfolio/smt_strategic_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      345 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/portfolio/solver2lookahead.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      279 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/portfolio/solver2lookahead.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5238 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/portfolio/solver_subsumption_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      438 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/portfolio/solver_subsumption_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13583 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/probe.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3968 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/probe.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4167 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/proof_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1310 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/proof_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2350 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/replace_proof_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1066 2022-07-06 19:24:04.893829 z3-solver-4.9.1.0/core/src/tactic/replace_proof_converter.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.718395 z3-solver-4.9.1.0/core/src/tactic/sls/
+-rw-r--r--   0 vsts      (1001) docker     (121)      253 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/sls/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    12411 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/sls/bvsls_opt_engine.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1915 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/sls/bvsls_opt_engine.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    21118 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/sls/sls_engine.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3958 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/sls/sls_engine.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    32923 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/sls/sls_evaluator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2441 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/sls/sls_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)      852 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/sls/sls_powers.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4059 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/sls/sls_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      469 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/sls/sls_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    37151 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/sls/sls_tracker.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.722395 z3-solver-4.9.1.0/core/src/tactic/smtlogics/
+-rw-r--r--   0 vsts      (1001) docker     (121)      825 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     1251 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/nra_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      355 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/nra_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2031 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfaufbv_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      443 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfaufbv_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1349 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfauflia_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      449 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfauflia_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5026 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfbv_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      603 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfbv_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4199 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfidl_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      432 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfidl_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8629 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qflia_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      602 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qflia_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2886 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qflra_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      429 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qflra_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4327 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfnia_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      429 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfnia_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1619 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfnra_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      429 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfnra_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1028 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfuf_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      433 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfuf_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      466 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfufbv_ackr_model_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      388 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfufbv_ackr_model_converter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6481 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfufbv_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      626 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfufbv_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      481 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfufbv_tactic_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)     4079 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/quant_tactics.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1591 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/quant_tactics.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      652 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/smt_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      531 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/smtlogics/smt_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7453 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4637 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      827 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/tactic_exception.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1827 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/tactic_params.pyg
+-rw-r--r--   0 vsts      (1001) docker     (121)    42859 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/tactical.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3596 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/tactical.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.722395 z3-solver-4.9.1.0/core/src/tactic/ufbv/
+-rw-r--r--   0 vsts      (1001) docker     (121)      380 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/ufbv/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     4024 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/ufbv/macro_finder_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      439 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/ufbv/macro_finder_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3553 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/ufbv/quasi_macros_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      445 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/ufbv/quasi_macros_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    28684 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/ufbv/ufbv_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    11400 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/ufbv/ufbv_rewriter.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2121 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/ufbv/ufbv_rewriter_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      488 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/ufbv/ufbv_rewriter_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2663 2022-07-06 19:24:04.897829 z3-solver-4.9.1.0/core/src/tactic/ufbv/ufbv_tactic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      578 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/tactic/ufbv/ufbv_tactic.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3686 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/tactic/user_propagator_base.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.730395 z3-solver-4.9.1.0/core/src/test/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3277 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)    20838 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/algebraic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3463 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/api.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1404 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/api_bug.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1641 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/arith_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1502 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/arith_simplifier_plugin.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4462 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/ast.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2473 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/bdd.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7171 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/bit_blaster.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6684 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/bit_vector.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6798 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/bits.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      886 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/buffer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4166 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/chashtable.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1436 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/check_assumptions.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9269 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/cnf_backbones.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2097 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/cube_clause.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1682 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/datalog_parser.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6262 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/ddnf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4346 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/diff_logic.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3092 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/dl_context.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12015 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/dl_product_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9644 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/dl_query.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    11675 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/dl_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2790 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/dl_table.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1293 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/dl_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    15078 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/doc.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4117 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/egraph.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1034 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/escaped.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1050 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/ex.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3066 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/expr_rand.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1643 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/expr_substitution.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    18313 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/ext_numeral.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1587 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/f2n.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      675 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/factor_rewriter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8368 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/finder.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2368 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/fixed_bit_vector.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1609 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/for_each_file.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      478 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/for_each_file.h
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.734395 z3-solver-4.9.1.0/core/src/test/fuzzing/
+-rw-r--r--   0 vsts      (1001) docker     (121)      169 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/fuzzing/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     2080 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/fuzzing/expr_delta.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      899 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/fuzzing/expr_delta.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10966 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/fuzzing/expr_rand.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1092 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/fuzzing/expr_rand.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3661 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/get_consequences.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4290 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/get_implied_equalities.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2926 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/hashtable.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3994 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/heap.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1477 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/heap_trie.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    16590 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/hilbert_basis.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2139 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/horn_subsume_model_converter.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2162 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/hwf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2216 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/im_float_config.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5277 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/inf_rational.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    14651 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/interval.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7957 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/karr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1154 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/list.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.734395 z3-solver-4.9.1.0/core/src/test/lp/
+-rw-r--r--   0 vsts      (1001) docker     (121)      654 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/lp/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     4749 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/lp/argument_parser.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9167 2022-07-06 19:24:04.901829 z3-solver-4.9.1.0/core/src/test/lp/gomory_test.h
+-rw-r--r--   0 vsts      (1001) docker     (121)   139388 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/lp/lp.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      313 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/lp/lp_main.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    28926 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/lp/nla_solver_test.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    13381 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/lp/smt_reader.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1763 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/lp/test_file_reader.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7752 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/main.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1064 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/map.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3463 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/matcher.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1169 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/memory.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1542 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/model2expr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12428 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/model_based_opt.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2241 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/model_evaluator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2047 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/model_retrieval.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1011 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/mpbq.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1807 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/mpf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    19394 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/mpff.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1649 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/mpfx.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3513 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/mpq.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    16789 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/mpz.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1550 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/nlarith_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    25206 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/nlsat.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    25450 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/no_overflow.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3320 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/object_allocator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6996 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/old_interval.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1313 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/optional.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9195 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/parray.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7668 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/pb2bv.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10175 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/pdd.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7720 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/pdd_solver.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2281 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/permutation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    80338 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/polynomial.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6654 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/polynorm.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      838 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/prime_generator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      920 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/proof_checker.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    18036 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/qe_arith.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    19280 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/quant_elim.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9650 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/quant_solve.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      431 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/random.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    16327 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/rational.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5118 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/rcf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      322 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/region.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3574 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/sat_local_search.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1391 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/sat_lookahead.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2746 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/sat_user_scope.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1391 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/scoped_timer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1755 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/simple_parser.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4746 2022-07-06 19:24:04.905830 z3-solver-4.9.1.0/core/src/test/simplex.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7767 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/simplifier.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1532 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/small_object_allocator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4013 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/smt2print_parse.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      783 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/smt_context.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1305 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/solver_pool.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    19191 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/sorting_network.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1648 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/stack.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      874 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/string_buffer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1600 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/substitution.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1246 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/symbol.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      950 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/symbol_table.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3926 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/tbv.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1871 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/test_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      991 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/theory_dl.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4595 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/theory_pb.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      206 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/timeout.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3856 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/total_order.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      625 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/totalizer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5393 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/trigo.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    30163 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/udoc_relation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3915 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/uint_set.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    43146 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/upolynomial.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1763 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/value_generator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1167 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/value_sweep.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2904 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/var_subst.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1335 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/vector.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      708 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/test/zstring.cpp
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.758395 z3-solver-4.9.1.0/core/src/util/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1433 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/CMakeLists.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)     1313 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/approx_nat.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1183 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/approx_nat.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      893 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/approx_set.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6239 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/approx_set.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5533 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/array.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3738 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/array_map.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2398 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/backtrackable_set.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10525 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/basic_interval.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10016 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/bit_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2870 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/bit_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6556 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/bit_vector.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6008 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/bit_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6597 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/buffer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      895 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/cancel_eh.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    21351 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/chashtable.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6535 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/checked_int64.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1306 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/cmd_context_types.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4372 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/cmd_context_types.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      718 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/common_msgs.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      932 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/common_msgs.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2721 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/container_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2928 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/debug.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2595 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/debug.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1355 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/dec_ref_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8572 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/dependency.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      300 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/dictionary.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2193 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/dlist.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3679 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/double_manager.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1268 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/ema.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1419 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/env_params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      411 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/env_params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      759 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/error_codes.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      673 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/event_handler.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      883 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/ext_gcd.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9168 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/ext_numeral.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6983 2022-07-06 19:24:04.909829 z3-solver-4.9.1.0/core/src/util/f2n.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      580 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/file_path.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4493 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/fixed_bit_vector.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4015 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/fixed_bit_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    25448 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/gparams.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4759 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/gparams.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2179 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/hash.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     6338 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/hash.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    28352 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/hashtable.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8081 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/heap.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    17467 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/hwf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5205 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/hwf.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1907 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/id_gen.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4035 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/id_var_list.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10330 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/inf_eps_rational.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1167 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/inf_int_rational.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     9308 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/inf_int_rational.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4953 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/inf_rational.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    12367 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/inf_rational.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      350 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/inf_s_integer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    10263 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/inf_s_integer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      596 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/lbool.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      651 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/lbool.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      751 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/lim_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2158 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/list.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      555 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/luby.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      456 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/luby.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      325 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/machine.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8252 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/map.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6356 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/max_cliques.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11366 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/memory_manager.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3438 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/memory_manager.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6199 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/min_cut.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1453 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/min_cut.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    25098 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/mpbq.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    13896 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/mpbq.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1167 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/mpbqi.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    73951 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/mpf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    11247 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/mpf.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    46099 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/mpff.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    15279 2022-07-06 19:24:04.913830 z3-solver-4.9.1.0/core/src/util/mpff.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    24653 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/mpfx.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    11435 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/mpfx.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    13802 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/mpn.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     3034 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/mpn.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    12270 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/mpq.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    26459 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/mpq.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      761 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/mpq_inf.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7732 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/mpq_inf.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    70068 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/mpz.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    19409 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/mpz.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    11044 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/mpzzp.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      985 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/mutex.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1573 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/nat_set.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1745 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/numeral_buffer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6365 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/obj_hashtable.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1236 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/obj_mark.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5516 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/obj_pair_hashtable.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1612 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/obj_pair_set.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3285 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/obj_ref.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2758 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/obj_ref_hashtable.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     5487 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/obj_triple_hashtable.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     8415 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/object_allocator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2822 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/optional.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1530 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/page.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      994 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/page.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    33686 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/params.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5054 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/params.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    18251 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/parray.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1552 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/permutation.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2201 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/permutation.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1376 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/plugin_manager.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      682 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/pool.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3240 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/prime_generator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1025 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/prime_generator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2132 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/ptr_scoped_buffer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1302 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/queue.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3515 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/rational.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)    16662 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/rational.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2415 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/ref.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3910 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/ref_buffer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6758 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/ref_pair_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1972 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/ref_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10941 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/ref_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3366 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/region.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1958 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/region.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2244 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/rlimit.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2130 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/rlimit.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1308 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/s_integer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     5939 2022-07-06 19:24:04.917830 z3-solver-4.9.1.0/core/src/util/s_integer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6065 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/sat_literal.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1124 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/scoped_ctrl_c.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      810 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/scoped_ctrl_c.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      814 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/scoped_limit_trail.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4527 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/scoped_numeral.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1540 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/scoped_numeral_buffer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1770 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/scoped_numeral_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1976 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/scoped_ptr_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3298 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/scoped_timer.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      582 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/scoped_timer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4683 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/scoped_vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9158 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/sexpr.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2802 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/sexpr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      570 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/sign.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7516 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/small_object_allocator.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1634 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/small_object_allocator.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1802 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/smt2_util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      403 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/smt2_util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    54782 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/sorting_network.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      497 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/sstream.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3735 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/stack.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1286 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/stack.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1326 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/stacked_value.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    21382 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/state_graph.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     7290 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/state_graph.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     7152 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/statistics.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     1225 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/statistics.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      503 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/stats.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1882 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/stopwatch.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      679 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/str_hashtable.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      686 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/stream_buffer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3860 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/string_buffer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4713 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/symbol.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     4536 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/symbol.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     4753 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/symbol_table.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1403 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/timeit.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      572 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/timeit.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1111 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/timeout.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      301 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/timeout.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      689 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/timer.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     3980 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/top_sort.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    10448 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/total_order.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1239 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/tptr.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1621 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/trace.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2374 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/trace.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9693 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/trail.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1013 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/uint_map.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     9681 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/uint_set.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     6276 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/union_find.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2662 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/util.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     8419 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/util.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1591 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/var_queue.h
+-rw-r--r--   0 vsts      (1001) docker     (121)    19790 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/vector.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     2922 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/warning.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      541 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/warning.h
+-rw-r--r--   0 vsts      (1001) docker     (121)     1743 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/z3_exception.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)      879 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/z3_exception.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      298 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/z3_version.h.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (121)      263 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/z3_version.h.in
+-rw-r--r--   0 vsts      (1001) docker     (121)     7749 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/zstring.cpp
+-rw-r--r--   0 vsts      (1001) docker     (121)     2824 2022-07-06 19:24:04.921830 z3-solver-4.9.1.0/core/src/util/zstring.h
+-rw-r--r--   0 vsts      (1001) docker     (121)      352 2022-07-06 19:24:47.978386 z3-solver-4.9.1.0/core/z3.pc.cmake.in
+-rw-r--r--   0 vsts      (1001) docker     (121)      107 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)    13637 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-06 19:24:48.762395 z3-solver-4.9.1.0/z3/
+-rw-r--r--   0 vsts      (1001) docker     (121)      210 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/z3/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   329080 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/z3/z3.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16090 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/z3/z3num.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1113 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/z3/z3poly.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    45224 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/z3/z3printer.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5039 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/z3/z3rcf.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4723 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/z3/z3types.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11388 2022-07-06 19:24:04.709827 z3-solver-4.9.1.0/z3/z3util.py
```

### Comparing `z3-solver-4.9.0.0/PKG-INFO` & `z3-solver-4.9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3-solver
-Version: 4.9.0.0
+Version: 4.9.1.0
 Summary: an efficient SMT solver library
 Home-page: https://github.com/Z3Prover/z3
 Author: The Z3 Theorem Prover Project
 Maintainer: Audrey Dutcher and Nikolaj Bjorner
 Maintainer-email: audrey@rhelmot.io
 License: MIT License
 Keywords: z3,smt,sat,prover,theorem
```

### Comparing `z3-solver-4.9.0.0/core/CMakeLists.txt` & `z3-solver-4.9.1.0/core/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Enforce some CMake policies
 cmake_minimum_required(VERSION 3.4)
 
 set(CMAKE_USER_MAKE_RULES_OVERRIDE_CXX "${CMAKE_CURRENT_SOURCE_DIR}/cmake/cxx_compiler_flags_overrides.cmake")
-project(Z3 VERSION 4.9.0.0 LANGUAGES CXX)
+project(Z3 VERSION 4.9.1.0 LANGUAGES CXX)
 
 ################################################################################
 # Project version
 ################################################################################
 set(Z3_FULL_VERSION_STR "${Z3_VERSION}") # Note this might be modified
 message(STATUS "Z3 version ${Z3_VERSION}")
```

### Comparing `z3-solver-4.9.0.0/core/LICENSE.txt` & `z3-solver-4.9.1.0/core/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/Z3Config.cmake.in` & `z3-solver-4.9.1.0/core/cmake/Z3Config.cmake.in`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/check_link_atomic.cmake` & `z3-solver-4.9.1.0/core/cmake/check_link_atomic.cmake`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/cmake_uninstall.cmake.in` & `z3-solver-4.9.1.0/core/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/compiler_lto.cmake` & `z3-solver-4.9.1.0/core/cmake/compiler_lto.cmake`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/compiler_warnings.cmake` & `z3-solver-4.9.1.0/core/cmake/compiler_warnings.cmake`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/cxx_compiler_flags_overrides.cmake` & `z3-solver-4.9.1.0/core/cmake/cxx_compiler_flags_overrides.cmake`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/git_utils.cmake` & `z3-solver-4.9.1.0/core/cmake/git_utils.cmake`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/modules/FindDotnet.cmake` & `z3-solver-4.9.1.0/core/cmake/modules/FindDotnet.cmake`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/modules/FindGMP.cmake` & `z3-solver-4.9.1.0/core/cmake/modules/FindGMP.cmake`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/msvc_legacy_quirks.cmake` & `z3-solver-4.9.1.0/core/cmake/msvc_legacy_quirks.cmake`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/target_arch_detect.cmake` & `z3-solver-4.9.1.0/core/cmake/target_arch_detect.cmake`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/z3_add_component.cmake` & `z3-solver-4.9.1.0/core/cmake/z3_add_component.cmake`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/z3_add_cxx_flag.cmake` & `z3-solver-4.9.1.0/core/cmake/z3_add_cxx_flag.cmake`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/cmake/z3_append_linker_flag_list_to_target.cmake` & `z3-solver-4.9.1.0/core/cmake/z3_append_linker_flag_list_to_target.cmake`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/build-win-signed.yml` & `z3-solver-4.9.1.0/core/scripts/build-win-signed.yml`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/coverage.yml` & `z3-solver-4.9.1.0/core/scripts/coverage.yml`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_consts_files.py` & `z3-solver-4.9.1.0/core/scripts/mk_consts_files.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_copyright.py` & `z3-solver-4.9.1.0/core/scripts/mk_copyright.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_def_file.py` & `z3-solver-4.9.1.0/core/scripts/mk_def_file.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_genfile_common.py` & `z3-solver-4.9.1.0/core/scripts/mk_genfile_common.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_gparams_register_modules_cpp.py` & `z3-solver-4.9.1.0/core/scripts/mk_gparams_register_modules_cpp.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_install_tactic_cpp.py` & `z3-solver-4.9.1.0/core/scripts/mk_install_tactic_cpp.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_mem_initializer_cpp.py` & `z3-solver-4.9.1.0/core/scripts/mk_mem_initializer_cpp.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_nuget_task.py` & `z3-solver-4.9.1.0/core/scripts/mk_nuget_task.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_pat_db.py` & `z3-solver-4.9.1.0/core/scripts/mk_pat_db.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_project.py` & `z3-solver-4.9.1.0/core/scripts/mk_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Z3 project configuration files
 #
 # Author: Leonardo de Moura (leonardo)
 ############################################
 from mk_util import *
 
 def init_version():
-    set_version(4, 9, 0, 0)
+    set_version(4, 9, 1, 0)
     
 # Z3 Project definition
 def init_project_def():
     init_version()
     add_lib('util', [], includes2install = ['z3_version.h'])
     add_lib('polynomial', ['util'], 'math/polynomial')
     add_lib('interval', ['util'], 'math/interval')
```

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_unix_dist.py` & `z3-solver-4.9.1.0/core/scripts/mk_unix_dist.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_util.py` & `z3-solver-4.9.1.0/core/scripts/mk_util.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/mk_win_dist.py` & `z3-solver-4.9.1.0/core/scripts/mk_win_dist.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/nightly.yaml` & `z3-solver-4.9.1.0/core/scripts/nightly.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 variables:
 
   Major: '4'
   Minor: '9'
-  Patch: '0'
+  Patch: '1'
   NightlyVersion: $(Major).$(Minor).$(Patch).$(Build.BuildId)-$(Build.DefinitionName)
 
 stages:
 - stage: Build
   jobs:
 
   - job: Mac
```

### Comparing `z3-solver-4.9.0.0/core/scripts/pyg2hpp.py` & `z3-solver-4.9.1.0/core/scripts/pyg2hpp.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/release.yml` & `z3-solver-4.9.1.0/core/scripts/release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # * Builds for all platforms (with code signing)
 # * Creates packages for Python and NuGet
 # * Uploads build products to stores (GitHub, NuGet, PyPI)
 
 trigger: none
 
 variables:
-  ReleaseVersion: '4.9.0'
+  ReleaseVersion: '4.9.1'
 
 stages:
 
 # Builds Z3 on various platforms
 - stage: Build
   jobs:
```

### Comparing `z3-solver-4.9.0.0/core/scripts/update_api.py` & `z3-solver-4.9.1.0/core/scripts/update_api.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/update_header_guards.py` & `z3-solver-4.9.1.0/core/scripts/update_header_guards.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/update_include.py` & `z3-solver-4.9.1.0/core/scripts/update_include.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/vsts-vs2013.cmd` & `z3-solver-4.9.1.0/core/scripts/vsts-vs2013.cmd`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/scripts/vsts-vs2017.cmd` & `z3-solver-4.9.1.0/core/scripts/vsts-vs2017.cmd`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ackermannization/ackermannize_bv_tactic.cpp` & `z3-solver-4.9.1.0/core/src/ackermannization/ackermannize_bv_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ackermannization/ackr_bound_probe.cpp` & `z3-solver-4.9.1.0/core/src/ackermannization/ackr_bound_probe.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ackermannization/ackr_helper.cpp` & `z3-solver-4.9.1.0/core/src/ackermannization/ackr_helper.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ackermannization/ackr_helper.h` & `z3-solver-4.9.1.0/core/src/ackermannization/ackr_helper.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ackermannization/ackr_info.h` & `z3-solver-4.9.1.0/core/src/ackermannization/ackr_info.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ackermannization/ackr_model_converter.cpp` & `z3-solver-4.9.1.0/core/src/ackermannization/ackr_model_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ackermannization/lackr.cpp` & `z3-solver-4.9.1.0/core/src/ackermannization/lackr.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ackermannization/lackr.h` & `z3-solver-4.9.1.0/core/src/ackermannization/lackr.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ackermannization/lackr_model_constructor.cpp` & `z3-solver-4.9.1.0/core/src/ackermannization/lackr_model_constructor.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ackermannization/lackr_model_constructor.h` & `z3-solver-4.9.1.0/core/src/ackermannization/lackr_model_constructor.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ackermannization/lackr_model_converter_lazy.cpp` & `z3-solver-4.9.1.0/core/src/ackermannization/lackr_model_converter_lazy.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/api/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_algebraic.cpp` & `z3-solver-4.9.1.0/core/src/api/api_algebraic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_arith.cpp` & `z3-solver-4.9.1.0/core/src/api/api_arith.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_array.cpp` & `z3-solver-4.9.1.0/core/src/api/api_array.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_ast.cpp` & `z3-solver-4.9.1.0/core/src/api/api_ast.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_ast_map.cpp` & `z3-solver-4.9.1.0/core/src/api/api_ast_map.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_ast_map.h` & `z3-solver-4.9.1.0/core/src/api/api_ast_map.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_ast_vector.cpp` & `z3-solver-4.9.1.0/core/src/api/api_ast_vector.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_ast_vector.h` & `z3-solver-4.9.1.0/core/src/api/api_ast_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_bv.cpp` & `z3-solver-4.9.1.0/core/src/api/api_bv.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_config_params.cpp` & `z3-solver-4.9.1.0/core/src/api/api_config_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_context.cpp` & `z3-solver-4.9.1.0/core/src/api/api_context.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_context.h` & `z3-solver-4.9.1.0/core/src/api/api_context.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_datalog.cpp` & `z3-solver-4.9.1.0/core/src/api/api_datalog.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_datalog.h` & `z3-solver-4.9.1.0/core/src/api/api_datalog.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_datatype.cpp` & `z3-solver-4.9.1.0/core/src/api/api_datatype.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_fpa.cpp` & `z3-solver-4.9.1.0/core/src/api/api_fpa.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_goal.cpp` & `z3-solver-4.9.1.0/core/src/api/api_goal.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_goal.h` & `z3-solver-4.9.1.0/core/src/api/api_goal.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_log.cpp` & `z3-solver-4.9.1.0/core/src/api/api_log.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_model.cpp` & `z3-solver-4.9.1.0/core/src/api/api_model.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_model.h` & `z3-solver-4.9.1.0/core/src/api/api_model.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_numeral.cpp` & `z3-solver-4.9.1.0/core/src/api/api_numeral.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_opt.cpp` & `z3-solver-4.9.1.0/core/src/api/api_opt.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_params.cpp` & `z3-solver-4.9.1.0/core/src/api/api_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_parsers.cpp` & `z3-solver-4.9.1.0/core/src/api/api_parsers.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_pb.cpp` & `z3-solver-4.9.1.0/core/src/api/api_pb.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_polynomial.cpp` & `z3-solver-4.9.1.0/core/src/api/api_polynomial.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_polynomial.h` & `z3-solver-4.9.1.0/core/src/api/api_polynomial.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_qe.cpp` & `z3-solver-4.9.1.0/core/src/api/api_qe.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_quant.cpp` & `z3-solver-4.9.1.0/core/src/api/api_quant.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_rcf.cpp` & `z3-solver-4.9.1.0/core/src/api/api_rcf.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_seq.cpp` & `z3-solver-4.9.1.0/core/src/api/api_seq.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_solver.cpp` & `z3-solver-4.9.1.0/core/src/api/api_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_solver.h` & `z3-solver-4.9.1.0/core/src/api/api_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_special_relations.cpp` & `z3-solver-4.9.1.0/core/src/api/api_special_relations.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_stats.cpp` & `z3-solver-4.9.1.0/core/src/api/api_stats.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_stats.h` & `z3-solver-4.9.1.0/core/src/api/api_stats.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_tactic.cpp` & `z3-solver-4.9.1.0/core/src/api/api_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_tactic.h` & `z3-solver-4.9.1.0/core/src/api/api_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/api_util.h` & `z3-solver-4.9.1.0/core/src/api/api_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/c++/z3++.h` & `z3-solver-4.9.1.0/core/src/api/c++/z3++.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dll/dll.cpp` & `z3-solver-4.9.1.0/core/src/api/dll/dll.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/AST.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/AST.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/ASTMap.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/ASTMap.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/ASTVector.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/ASTVector.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/AlgebraicNum.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/AlgebraicNum.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/ApplyResult.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/ApplyResult.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/ArithExpr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/ArithExpr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/ArithSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/ArithSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/ArrayExpr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/ArrayExpr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/ArraySort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/ArraySort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/BitVecExpr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/BitVecExpr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/BitVecNum.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/BitVecNum.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/BitVecSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/BitVecSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/BoolExpr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/BoolExpr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/BoolSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/BoolSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/api/dotnet/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/CharSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/CharSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Constructor.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Constructor.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/ConstructorList.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/ConstructorList.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Context.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Context.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/DatatypeExpr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/DatatypeExpr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/DatatypeSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/DatatypeSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Deprecated.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Deprecated.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/EnumSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/EnumSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Expr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Expr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/FPExpr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/FPExpr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/FPNum.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/FPNum.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/FPRMExpr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/FPRMExpr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/FPRMNum.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/FPRMNum.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/FPRMSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/FPRMSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/FPSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/FPSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/FiniteDomainExpr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/FiniteDomainExpr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/FiniteDomainNum.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/FiniteDomainNum.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/FiniteDomainSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/FiniteDomainSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Fixedpoint.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Fixedpoint.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/FuncDecl.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/FuncDecl.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/FuncInterp.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/FuncInterp.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Global.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Global.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Goal.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Goal.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/IDecRefQueue.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/IDecRefQueue.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/IntExpr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/IntExpr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/IntNum.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/IntNum.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/IntSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/IntSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/IntSymbol.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/IntSymbol.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Lambda.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Lambda.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/ListSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/ListSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Log.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Log.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Microsoft.Z3.csproj.in` & `z3-solver-4.9.1.0/core/src/api/dotnet/Microsoft.Z3.csproj.in`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Microsoft.Z3.props` & `z3-solver-4.9.1.0/core/src/api/dotnet/Microsoft.Z3.props`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Microsoft.Z3.snk` & `z3-solver-4.9.1.0/core/src/api/dotnet/Microsoft.Z3.snk`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Model.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Model.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/NativeContext.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/NativeContext.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/NativeFuncInterp.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/NativeFuncInterp.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/NativeModel.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/NativeModel.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/NativeSolver.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/NativeSolver.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Optimize.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Optimize.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/ParamDescrs.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/ParamDescrs.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Params.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Params.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Pattern.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Pattern.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Probe.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Probe.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Properties/AssemblyInfo.cs.in` & `z3-solver-4.9.1.0/core/src/api/dotnet/Properties/AssemblyInfo.cs.in`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Quantifier.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Quantifier.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/RatNum.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/RatNum.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/ReExpr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/ReExpr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/ReSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/ReSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/RealExpr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/RealExpr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/RealSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/RealSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/RelationSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/RelationSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/SeqExpr.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/SeqExpr.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/SeqSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/SeqSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/SetSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/SetSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Solver.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Solver.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Sort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Sort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Statistics.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Statistics.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Status.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Status.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/StringSymbol.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/StringSymbol.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Symbol.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Symbol.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Tactic.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Tactic.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/TupleSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/TupleSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/UninterpretedSort.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/UninterpretedSort.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/UserPropagator.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/UserPropagator.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Version.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Version.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Z3Exception.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Z3Exception.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/Z3Object.cs` & `z3-solver-4.9.1.0/core/src/api/dotnet/Z3Object.cs`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/cmake_install_gac.cmake.in` & `z3-solver-4.9.1.0/core/src/api/dotnet/cmake_install_gac.cmake.in`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/dotnet/cmake_uninstall_gac.cmake.in` & `z3-solver-4.9.1.0/core/src/api/dotnet/cmake_uninstall_gac.cmake.in`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/AST.java` & `z3-solver-4.9.1.0/core/src/api/java/AST.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/ASTMap.java` & `z3-solver-4.9.1.0/core/src/api/java/ASTMap.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/ASTVector.java` & `z3-solver-4.9.1.0/core/src/api/java/ASTVector.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/AlgebraicNum.java` & `z3-solver-4.9.1.0/core/src/api/java/AlgebraicNum.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/ApplyResult.java` & `z3-solver-4.9.1.0/core/src/api/java/ApplyResult.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/ArraySort.java` & `z3-solver-4.9.1.0/core/src/api/java/ArraySort.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/BitVecExpr.java` & `z3-solver-4.9.1.0/core/src/api/java/BitVecExpr.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/BitVecNum.java` & `z3-solver-4.9.1.0/core/src/api/java/BitVecNum.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/BitVecSort.java` & `z3-solver-4.9.1.0/core/src/api/java/BitVecSort.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/api/java/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Constructor.java` & `z3-solver-4.9.1.0/core/src/api/java/Constructor.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/ConstructorList.java` & `z3-solver-4.9.1.0/core/src/api/java/ConstructorList.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Context.java` & `z3-solver-4.9.1.0/core/src/api/java/Context.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/DatatypeSort.java` & `z3-solver-4.9.1.0/core/src/api/java/DatatypeSort.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/EnumSort.java` & `z3-solver-4.9.1.0/core/src/api/java/EnumSort.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Expr.java` & `z3-solver-4.9.1.0/core/src/api/java/Expr.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/FPExpr.java` & `z3-solver-4.9.1.0/core/src/api/java/FPExpr.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/FPNum.java` & `z3-solver-4.9.1.0/core/src/api/java/FPNum.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/FPRMNum.java` & `z3-solver-4.9.1.0/core/src/api/java/FPRMNum.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/FPSort.java` & `z3-solver-4.9.1.0/core/src/api/java/FPSort.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/FiniteDomainNum.java` & `z3-solver-4.9.1.0/core/src/api/java/FiniteDomainNum.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/FiniteDomainSort.java` & `z3-solver-4.9.1.0/core/src/api/java/FiniteDomainSort.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Fixedpoint.java` & `z3-solver-4.9.1.0/core/src/api/java/Fixedpoint.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/FuncDecl.java` & `z3-solver-4.9.1.0/core/src/api/java/FuncDecl.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/FuncInterp.java` & `z3-solver-4.9.1.0/core/src/api/java/FuncInterp.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Global.java` & `z3-solver-4.9.1.0/core/src/api/java/Global.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Goal.java` & `z3-solver-4.9.1.0/core/src/api/java/Goal.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/IDecRefQueue.java` & `z3-solver-4.9.1.0/core/src/api/java/IDecRefQueue.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/IntNum.java` & `z3-solver-4.9.1.0/core/src/api/java/IntNum.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/IntSymbol.java` & `z3-solver-4.9.1.0/core/src/api/java/IntSymbol.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Lambda.java` & `z3-solver-4.9.1.0/core/src/api/java/Lambda.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/ListSort.java` & `z3-solver-4.9.1.0/core/src/api/java/ListSort.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Log.java` & `z3-solver-4.9.1.0/core/src/api/java/Log.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Model.java` & `z3-solver-4.9.1.0/core/src/api/java/Model.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/NativeStatic.txt` & `z3-solver-4.9.1.0/core/src/api/java/NativeStatic.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Optimize.java` & `z3-solver-4.9.1.0/core/src/api/java/Optimize.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/ParamDescrs.java` & `z3-solver-4.9.1.0/core/src/api/java/ParamDescrs.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Params.java` & `z3-solver-4.9.1.0/core/src/api/java/Params.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Pattern.java` & `z3-solver-4.9.1.0/core/src/api/java/Pattern.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Probe.java` & `z3-solver-4.9.1.0/core/src/api/java/Probe.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Quantifier.java` & `z3-solver-4.9.1.0/core/src/api/java/Quantifier.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/RatNum.java` & `z3-solver-4.9.1.0/core/src/api/java/RatNum.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/RelationSort.java` & `z3-solver-4.9.1.0/core/src/api/java/RelationSort.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Solver.java` & `z3-solver-4.9.1.0/core/src/api/java/Solver.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Sort.java` & `z3-solver-4.9.1.0/core/src/api/java/Sort.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Statistics.java` & `z3-solver-4.9.1.0/core/src/api/java/Statistics.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Status.java` & `z3-solver-4.9.1.0/core/src/api/java/Status.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/StringSymbol.java` & `z3-solver-4.9.1.0/core/src/api/java/StringSymbol.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Symbol.java` & `z3-solver-4.9.1.0/core/src/api/java/Symbol.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Tactic.java` & `z3-solver-4.9.1.0/core/src/api/java/Tactic.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/TupleSort.java` & `z3-solver-4.9.1.0/core/src/api/java/TupleSort.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/UninterpretedSort.java` & `z3-solver-4.9.1.0/core/src/api/java/UninterpretedSort.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Version.java` & `z3-solver-4.9.1.0/core/src/api/java/Version.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Z3Exception.java` & `z3-solver-4.9.1.0/core/src/api/java/Z3Exception.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/java/Z3Object.java` & `z3-solver-4.9.1.0/core/src/api/java/Z3Object.java`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/PUBLISHED_README.md` & `z3-solver-4.9.1.0/core/src/api/js/PUBLISHED_README.md`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/README.md` & `z3-solver-4.9.1.0/core/src/api/js/README.md`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/examples/high-level/miracle-sudoku.ts` & `z3-solver-4.9.1.0/core/src/api/js/examples/high-level/miracle-sudoku.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/examples/low-level/example-raw.ts` & `z3-solver-4.9.1.0/core/src/api/js/examples/low-level/example-raw.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/examples/low-level/test-ts-api.ts` & `z3-solver-4.9.1.0/core/src/api/js/examples/low-level/test-ts-api.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/package-lock.json` & `z3-solver-4.9.1.0/core/src/api/js/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999955116696588%*

 * *Differences: {"'packages'": "{'': {'engines': {'node': '>=16'}}}"}*

```diff
@@ -4795,15 +4795,15 @@
                 "sprintf-js": "^1.1.2",
                 "ts-jest": "^28.0.3",
                 "ts-node": "^10.8.0",
                 "typedoc": "^0.22.17",
                 "typescript": "^4.5.4"
             },
             "engines": {
-                "node": ">=16 <18"
+                "node": ">=16"
             },
             "license": "MIT",
             "name": "z3-solver"
         },
         "node_modules/@ampproject/remapping": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.1.0",
```

### Comparing `z3-solver-4.9.0.0/core/src/api/js/package.json` & `z3-solver-4.9.1.0/core/src/api/js/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9464285714285714%*

 * *Differences: {"'engines'": "{'node': '>=16'}", "'files'": "['build/**/*.{js,d.ts,wasm}']"}*

```diff
@@ -22,18 +22,18 @@
         "sprintf-js": "^1.1.2",
         "ts-jest": "^28.0.3",
         "ts-node": "^10.8.0",
         "typedoc": "^0.22.17",
         "typescript": "^4.5.4"
     },
     "engines": {
-        "node": ">=16 <18"
+        "node": ">=16"
     },
     "files": [
-        "build/*.{js,d.ts,wasm}"
+        "build/**/*.{js,d.ts,wasm}"
     ],
     "homepage": "https://github.com/Z3Prover/z3/tree/master/src/api/js",
     "keywords": [
         "Z3",
         "theorem",
         "prover",
         "solver",
```

### Comparing `z3-solver-4.9.0.0/core/src/api/js/scripts/async-fns.ts` & `z3-solver-4.9.1.0/core/src/api/js/scripts/async-fns.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/scripts/build-wasm.ts` & `z3-solver-4.9.1.0/core/src/api/js/scripts/build-wasm.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/scripts/make-cc-wrapper.ts` & `z3-solver-4.9.1.0/core/src/api/js/scripts/make-cc-wrapper.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/scripts/make-ts-wrapper.ts` & `z3-solver-4.9.1.0/core/src/api/js/scripts/make-ts-wrapper.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/scripts/parse-api.ts` & `z3-solver-4.9.1.0/core/src/api/js/scripts/parse-api.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/src/browser.ts` & `z3-solver-4.9.1.0/core/src/api/js/src/browser.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/src/high-level/high-level.test.ts` & `z3-solver-4.9.1.0/core/src/api/js/src/high-level/high-level.test.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/src/high-level/high-level.ts` & `z3-solver-4.9.1.0/core/src/api/js/src/high-level/high-level.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/src/high-level/types.ts` & `z3-solver-4.9.1.0/core/src/api/js/src/high-level/types.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/src/high-level/utils.test.ts` & `z3-solver-4.9.1.0/core/src/api/js/src/high-level/utils.test.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/src/high-level/utils.ts` & `z3-solver-4.9.1.0/core/src/api/js/src/high-level/utils.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/src/jest.ts` & `z3-solver-4.9.1.0/core/src/api/js/src/jest.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/src/low-level/async-wrapper.js` & `z3-solver-4.9.1.0/core/src/api/js/src/low-level/async-wrapper.js`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/js/src/node.ts` & `z3-solver-4.9.1.0/core/src/api/js/src/node.ts`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/julia/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/api/julia/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/julia/README.md` & `z3-solver-4.9.1.0/core/src/api/julia/README.md`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/julia/z3jl.cpp` & `z3-solver-4.9.1.0/core/src/api/julia/z3jl.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/ml/README.md` & `z3-solver-4.9.1.0/core/src/api/ml/README.md`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/ml/z3.ml` & `z3-solver-4.9.1.0/core/src/api/ml/z3.ml`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/ml/z3.mli` & `z3-solver-4.9.1.0/core/src/api/ml/z3.mli`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/ml/z3native.ml.pre` & `z3-solver-4.9.1.0/core/src/api/ml/z3native.ml.pre`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/ml/z3native_stubs.c.pre` & `z3-solver-4.9.1.0/core/src/api/ml/z3native_stubs.c.pre`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/ml/z3native_stubs.h` & `z3-solver-4.9.1.0/core/src/api/ml/z3native_stubs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/python/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/api/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/python/z3/z3.py` & `z3-solver-4.9.1.0/core/src/api/python/z3/z3.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/python/z3/z3num.py` & `z3-solver-4.9.1.0/core/src/api/python/z3/z3num.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/python/z3/z3poly.py` & `z3-solver-4.9.1.0/core/src/api/python/z3/z3poly.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/python/z3/z3printer.py` & `z3-solver-4.9.1.0/core/src/api/python/z3/z3printer.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/python/z3/z3rcf.py` & `z3-solver-4.9.1.0/core/src/api/python/z3/z3rcf.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/python/z3/z3types.py` & `z3-solver-4.9.1.0/core/src/api/python/z3/z3types.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/python/z3/z3util.py` & `z3-solver-4.9.1.0/core/src/api/python/z3/z3util.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3.h` & `z3-solver-4.9.1.0/core/src/api/z3.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3_algebraic.h` & `z3-solver-4.9.1.0/core/src/api/z3_algebraic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3_api.h` & `z3-solver-4.9.1.0/core/src/api/z3_api.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3_ast_containers.h` & `z3-solver-4.9.1.0/core/src/api/z3_ast_containers.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3_fixedpoint.h` & `z3-solver-4.9.1.0/core/src/api/z3_fixedpoint.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3_fpa.h` & `z3-solver-4.9.1.0/core/src/api/z3_fpa.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3_optimization.h` & `z3-solver-4.9.1.0/core/src/api/z3_optimization.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3_polynomial.h` & `z3-solver-4.9.1.0/core/src/api/z3_polynomial.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3_rcf.h` & `z3-solver-4.9.1.0/core/src/api/z3_rcf.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3_replayer.cpp` & `z3-solver-4.9.1.0/core/src/api/z3_replayer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3_replayer.h` & `z3-solver-4.9.1.0/core/src/api/z3_replayer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3_spacer.h` & `z3-solver-4.9.1.0/core/src/api/z3_spacer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/api/z3_v1.h` & `z3-solver-4.9.1.0/core/src/api/z3_v1.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/ast/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/act_cache.cpp` & `z3-solver-4.9.1.0/core/src/ast/act_cache.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/act_cache.h` & `z3-solver-4.9.1.0/core/src/ast/act_cache.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/arith_decl_plugin.cpp` & `z3-solver-4.9.1.0/core/src/ast/arith_decl_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/arith_decl_plugin.h` & `z3-solver-4.9.1.0/core/src/ast/arith_decl_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/array_decl_plugin.cpp` & `z3-solver-4.9.1.0/core/src/ast/array_decl_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/array_decl_plugin.h` & `z3-solver-4.9.1.0/core/src/ast/array_decl_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast.cpp` & `z3-solver-4.9.1.0/core/src/ast/ast.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast.h` & `z3-solver-4.9.1.0/core/src/ast/ast.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_ll_pp.cpp` & `z3-solver-4.9.1.0/core/src/ast/ast_ll_pp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_ll_pp.h` & `z3-solver-4.9.1.0/core/src/ast/ast_ll_pp.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_lt.cpp` & `z3-solver-4.9.1.0/core/src/ast/ast_lt.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_lt.h` & `z3-solver-4.9.1.0/core/src/ast/ast_lt.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_pp.h` & `z3-solver-4.9.1.0/core/src/ast/ast_pp.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_pp_dot.cpp` & `z3-solver-4.9.1.0/core/src/ast/ast_pp_dot.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_pp_dot.h` & `z3-solver-4.9.1.0/core/src/ast/ast_pp_dot.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_pp_util.cpp` & `z3-solver-4.9.1.0/core/src/ast/ast_pp_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_pp_util.h` & `z3-solver-4.9.1.0/core/src/ast/ast_pp_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_printer.cpp` & `z3-solver-4.9.1.0/core/src/ast/ast_printer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_printer.h` & `z3-solver-4.9.1.0/core/src/ast/ast_printer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_smt2_pp.cpp` & `z3-solver-4.9.1.0/core/src/ast/ast_smt2_pp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_smt2_pp.h` & `z3-solver-4.9.1.0/core/src/ast/ast_smt2_pp.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_smt_pp.cpp` & `z3-solver-4.9.1.0/core/src/ast/ast_smt_pp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_smt_pp.h` & `z3-solver-4.9.1.0/core/src/ast/ast_smt_pp.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_trail.h` & `z3-solver-4.9.1.0/core/src/ast/ast_trail.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_translation.cpp` & `z3-solver-4.9.1.0/core/src/ast/ast_translation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_translation.h` & `z3-solver-4.9.1.0/core/src/ast/ast_translation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_util.cpp` & `z3-solver-4.9.1.0/core/src/ast/ast_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/ast_util.h` & `z3-solver-4.9.1.0/core/src/ast/ast_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/bv_decl_plugin.cpp` & `z3-solver-4.9.1.0/core/src/ast/bv_decl_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/bv_decl_plugin.h` & `z3-solver-4.9.1.0/core/src/ast/bv_decl_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/char_decl_plugin.cpp` & `z3-solver-4.9.1.0/core/src/ast/char_decl_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/char_decl_plugin.h` & `z3-solver-4.9.1.0/core/src/ast/char_decl_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/cost_evaluator.cpp` & `z3-solver-4.9.1.0/core/src/ast/cost_evaluator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/cost_evaluator.h` & `z3-solver-4.9.1.0/core/src/ast/cost_evaluator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/datatype_decl_plugin.cpp` & `z3-solver-4.9.1.0/core/src/ast/datatype_decl_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/datatype_decl_plugin.h` & `z3-solver-4.9.1.0/core/src/ast/datatype_decl_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/decl_collector.cpp` & `z3-solver-4.9.1.0/core/src/ast/decl_collector.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/decl_collector.h` & `z3-solver-4.9.1.0/core/src/ast/decl_collector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/display_dimacs.cpp` & `z3-solver-4.9.1.0/core/src/ast/display_dimacs.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/dl_decl_plugin.cpp` & `z3-solver-4.9.1.0/core/src/ast/dl_decl_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/dl_decl_plugin.h` & `z3-solver-4.9.1.0/core/src/ast/dl_decl_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/euf/euf_egraph.cpp` & `z3-solver-4.9.1.0/core/src/ast/euf/euf_egraph.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/euf/euf_egraph.h` & `z3-solver-4.9.1.0/core/src/ast/euf/euf_egraph.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/euf/euf_enode.cpp` & `z3-solver-4.9.1.0/core/src/ast/euf/euf_enode.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/euf/euf_enode.h` & `z3-solver-4.9.1.0/core/src/ast/euf/euf_enode.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/euf/euf_etable.cpp` & `z3-solver-4.9.1.0/core/src/ast/euf/euf_etable.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/euf/euf_etable.h` & `z3-solver-4.9.1.0/core/src/ast/euf/euf_etable.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/euf/euf_justification.h` & `z3-solver-4.9.1.0/core/src/ast/euf/euf_justification.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr2polynomial.cpp` & `z3-solver-4.9.1.0/core/src/ast/expr2polynomial.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr2polynomial.h` & `z3-solver-4.9.1.0/core/src/ast/expr2polynomial.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr2var.cpp` & `z3-solver-4.9.1.0/core/src/ast/expr2var.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr2var.h` & `z3-solver-4.9.1.0/core/src/ast/expr2var.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr_abstract.cpp` & `z3-solver-4.9.1.0/core/src/ast/expr_abstract.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr_abstract.h` & `z3-solver-4.9.1.0/core/src/ast/expr_abstract.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr_delta_pair.h` & `z3-solver-4.9.1.0/core/src/ast/expr_delta_pair.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr_functors.cpp` & `z3-solver-4.9.1.0/core/src/ast/expr_functors.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr_functors.h` & `z3-solver-4.9.1.0/core/src/ast/expr_functors.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr_map.cpp` & `z3-solver-4.9.1.0/core/src/ast/expr_map.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr_map.h` & `z3-solver-4.9.1.0/core/src/ast/expr_map.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr_stat.cpp` & `z3-solver-4.9.1.0/core/src/ast/expr_stat.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr_stat.h` & `z3-solver-4.9.1.0/core/src/ast/expr_stat.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr_substitution.cpp` & `z3-solver-4.9.1.0/core/src/ast/expr_substitution.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/expr_substitution.h` & `z3-solver-4.9.1.0/core/src/ast/expr_substitution.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/for_each_ast.cpp` & `z3-solver-4.9.1.0/core/src/ast/for_each_ast.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/for_each_ast.h` & `z3-solver-4.9.1.0/core/src/ast/for_each_ast.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/for_each_expr.cpp` & `z3-solver-4.9.1.0/core/src/ast/for_each_expr.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/for_each_expr.h` & `z3-solver-4.9.1.0/core/src/ast/for_each_expr.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/format.cpp` & `z3-solver-4.9.1.0/core/src/ast/format.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/format.h` & `z3-solver-4.9.1.0/core/src/ast/format.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/fpa/bv2fpa_converter.cpp` & `z3-solver-4.9.1.0/core/src/ast/fpa/bv2fpa_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/fpa/bv2fpa_converter.h` & `z3-solver-4.9.1.0/core/src/ast/fpa/bv2fpa_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/fpa/fpa2bv_converter.cpp` & `z3-solver-4.9.1.0/core/src/ast/fpa/fpa2bv_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/fpa/fpa2bv_converter.h` & `z3-solver-4.9.1.0/core/src/ast/fpa/fpa2bv_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/fpa/fpa2bv_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/fpa/fpa2bv_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/fpa/fpa2bv_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/fpa/fpa2bv_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/fpa_decl_plugin.cpp` & `z3-solver-4.9.1.0/core/src/ast/fpa_decl_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/fpa_decl_plugin.h` & `z3-solver-4.9.1.0/core/src/ast/fpa_decl_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/func_decl_dependencies.cpp` & `z3-solver-4.9.1.0/core/src/ast/func_decl_dependencies.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/func_decl_dependencies.h` & `z3-solver-4.9.1.0/core/src/ast/func_decl_dependencies.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/has_free_vars.cpp` & `z3-solver-4.9.1.0/core/src/ast/has_free_vars.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/is_variable_test.h` & `z3-solver-4.9.1.0/core/src/ast/is_variable_test.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/justified_expr.h` & `z3-solver-4.9.1.0/core/src/ast/justified_expr.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macro_substitution.cpp` & `z3-solver-4.9.1.0/core/src/ast/macro_substitution.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macro_substitution.h` & `z3-solver-4.9.1.0/core/src/ast/macro_substitution.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macros/cond_macro.h` & `z3-solver-4.9.1.0/core/src/ast/macros/cond_macro.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macros/macro_finder.cpp` & `z3-solver-4.9.1.0/core/src/ast/macros/macro_finder.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macros/macro_finder.h` & `z3-solver-4.9.1.0/core/src/ast/macros/macro_finder.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macros/macro_manager.cpp` & `z3-solver-4.9.1.0/core/src/ast/macros/macro_manager.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macros/macro_manager.h` & `z3-solver-4.9.1.0/core/src/ast/macros/macro_manager.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macros/macro_util.cpp` & `z3-solver-4.9.1.0/core/src/ast/macros/macro_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macros/macro_util.h` & `z3-solver-4.9.1.0/core/src/ast/macros/macro_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macros/quantifier_macro_info.cpp` & `z3-solver-4.9.1.0/core/src/ast/macros/quantifier_macro_info.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macros/quantifier_macro_info.h` & `z3-solver-4.9.1.0/core/src/ast/macros/quantifier_macro_info.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macros/quasi_macros.cpp` & `z3-solver-4.9.1.0/core/src/ast/macros/quasi_macros.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/macros/quasi_macros.h` & `z3-solver-4.9.1.0/core/src/ast/macros/quasi_macros.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/normal_forms/defined_names.cpp` & `z3-solver-4.9.1.0/core/src/ast/normal_forms/defined_names.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/normal_forms/defined_names.h` & `z3-solver-4.9.1.0/core/src/ast/normal_forms/defined_names.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/normal_forms/elim_term_ite.cpp` & `z3-solver-4.9.1.0/core/src/ast/normal_forms/elim_term_ite.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/normal_forms/elim_term_ite.h` & `z3-solver-4.9.1.0/core/src/ast/normal_forms/elim_term_ite.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/normal_forms/name_exprs.cpp` & `z3-solver-4.9.1.0/core/src/ast/normal_forms/name_exprs.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/normal_forms/name_exprs.h` & `z3-solver-4.9.1.0/core/src/ast/normal_forms/name_exprs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/normal_forms/nnf.cpp` & `z3-solver-4.9.1.0/core/src/ast/normal_forms/nnf.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/normal_forms/nnf.h` & `z3-solver-4.9.1.0/core/src/ast/normal_forms/nnf.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/normal_forms/nnf_params.pyg` & `z3-solver-4.9.1.0/core/src/ast/normal_forms/nnf_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/normal_forms/pull_quant.cpp` & `z3-solver-4.9.1.0/core/src/ast/normal_forms/pull_quant.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/normal_forms/pull_quant.h` & `z3-solver-4.9.1.0/core/src/ast/normal_forms/pull_quant.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/num_occurs.cpp` & `z3-solver-4.9.1.0/core/src/ast/num_occurs.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/num_occurs.h` & `z3-solver-4.9.1.0/core/src/ast/num_occurs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/occurs.cpp` & `z3-solver-4.9.1.0/core/src/ast/occurs.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/pattern/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/ast/pattern/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/pattern/database.smt2` & `z3-solver-4.9.1.0/core/src/ast/pattern/database.smt2`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/pattern/expr_pattern_match.cpp` & `z3-solver-4.9.1.0/core/src/ast/pattern/expr_pattern_match.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/pattern/expr_pattern_match.h` & `z3-solver-4.9.1.0/core/src/ast/pattern/expr_pattern_match.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/pattern/pattern_inference.cpp` & `z3-solver-4.9.1.0/core/src/ast/pattern/pattern_inference.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/pattern/pattern_inference.h` & `z3-solver-4.9.1.0/core/src/ast/pattern/pattern_inference.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/pb_decl_plugin.cpp` & `z3-solver-4.9.1.0/core/src/ast/pb_decl_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/pb_decl_plugin.h` & `z3-solver-4.9.1.0/core/src/ast/pb_decl_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/pp.cpp` & `z3-solver-4.9.1.0/core/src/ast/pp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/pp_params.pyg` & `z3-solver-4.9.1.0/core/src/ast/pp_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/proofs/proof_checker.cpp` & `z3-solver-4.9.1.0/core/src/ast/proofs/proof_checker.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/proofs/proof_checker.h` & `z3-solver-4.9.1.0/core/src/ast/proofs/proof_checker.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/proofs/proof_utils.cpp` & `z3-solver-4.9.1.0/core/src/ast/proofs/proof_utils.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/proofs/proof_utils.h` & `z3-solver-4.9.1.0/core/src/ast/proofs/proof_utils.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/quantifier_stat.cpp` & `z3-solver-4.9.1.0/core/src/ast/quantifier_stat.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/quantifier_stat.h` & `z3-solver-4.9.1.0/core/src/ast/quantifier_stat.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/recfun_decl_plugin.cpp` & `z3-solver-4.9.1.0/core/src/ast/recfun_decl_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/recfun_decl_plugin.h` & `z3-solver-4.9.1.0/core/src/ast/recfun_decl_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/recurse_expr.h` & `z3-solver-4.9.1.0/core/src/ast/recurse_expr.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/recurse_expr_def.h` & `z3-solver-4.9.1.0/core/src/ast/recurse_expr_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/reg_decl_plugins.cpp` & `z3-solver-4.9.1.0/core/src/ast/reg_decl_plugins.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/ast/rewriter/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/arith_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/arith_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/arith_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/arith_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/array_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/array_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/array_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/array_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/ast_counter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/ast_counter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/ast_counter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/ast_counter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bit2int.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bit2int.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bit2int.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bit2int.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/bit_blaster.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/bit_blaster.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/bit_blaster.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/bit_blaster.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/bit_blaster_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/bit_blaster_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/bit_blaster_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/bit_blaster_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/bit_blaster_tpl.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/bit_blaster_tpl.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bit_blaster/bit_blaster_tpl_def.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bit_blaster/bit_blaster_tpl_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bool_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bool_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bool_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bool_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bv_bounds.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bv_bounds.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bv_bounds.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bv_bounds.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bv_elim.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bv_elim.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bv_elim.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bv_elim.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bv_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bv_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/bv_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/bv_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/cached_var_subst.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/cached_var_subst.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/cached_var_subst.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/cached_var_subst.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/char_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/char_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/char_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/char_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/datatype_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/datatype_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/datatype_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/datatype_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/der.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/der.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/der.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/der.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/distribute_forall.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/distribute_forall.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/distribute_forall.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/distribute_forall.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/dl_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/dl_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/dl_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/dl_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/elim_bounds.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/elim_bounds.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/elim_bounds.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/elim_bounds.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/enum2bv_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/enum2bv_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/enum2bv_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/enum2bv_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/expr_replacer.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/expr_replacer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/expr_replacer.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/expr_replacer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/expr_safe_replace.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/expr_safe_replace.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/expr_safe_replace.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/expr_safe_replace.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/factor_equivs.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/factor_equivs.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/factor_equivs.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/factor_equivs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/factor_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/factor_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/factor_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/factor_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/fpa_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/fpa_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/fpa_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/fpa_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/func_decl_replace.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/func_decl_replace.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/func_decl_replace.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/func_decl_replace.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/hoist_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/hoist_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/hoist_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/hoist_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/inj_axiom.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/inj_axiom.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/label_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/label_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/label_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/label_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/maximize_ac_sharing.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/maximize_ac_sharing.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/maximize_ac_sharing.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/maximize_ac_sharing.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/mk_extract_proc.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/mk_extract_proc.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/mk_extract_proc.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/mk_extract_proc.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/mk_simplified_app.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/mk_simplified_app.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/mk_simplified_app.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/mk_simplified_app.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/pb2bv_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/pb2bv_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/pb2bv_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/pb2bv_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/pb_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/pb_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/pb_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/pb_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/pb_rewriter_def.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/pb_rewriter_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/poly_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/poly_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/poly_rewriter_def.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/poly_rewriter_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/push_app_ite.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/push_app_ite.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/push_app_ite.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/push_app_ite.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/quant_hoist.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/quant_hoist.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/quant_hoist.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/quant_hoist.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/recfun_replace.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/recfun_replace.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/recfun_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/recfun_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/recfun_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/recfun_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/rewriter.txt` & `z3-solver-4.9.1.0/core/src/ast/rewriter/rewriter.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/rewriter_def.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/rewriter_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/rewriter_types.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/rewriter_types.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/seq_axioms.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/seq_axioms.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/seq_axioms.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/seq_axioms.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/seq_eq_solver.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/seq_eq_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/seq_eq_solver.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/seq_eq_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/seq_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/seq_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/seq_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/seq_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/seq_skolem.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/seq_skolem.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/seq_skolem.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/seq_skolem.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/th_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/th_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/th_rewriter.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/th_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/value_sweep.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/value_sweep.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/value_sweep.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/value_sweep.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/var_subst.cpp` & `z3-solver-4.9.1.0/core/src/ast/rewriter/var_subst.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/rewriter/var_subst.h` & `z3-solver-4.9.1.0/core/src/ast/rewriter/var_subst.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/scoped_proof.h` & `z3-solver-4.9.1.0/core/src/ast/scoped_proof.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/seq_decl_plugin.cpp` & `z3-solver-4.9.1.0/core/src/ast/seq_decl_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/seq_decl_plugin.h` & `z3-solver-4.9.1.0/core/src/ast/seq_decl_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/shared_occs.cpp` & `z3-solver-4.9.1.0/core/src/ast/shared_occs.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/shared_occs.h` & `z3-solver-4.9.1.0/core/src/ast/shared_occs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/special_relations_decl_plugin.cpp` & `z3-solver-4.9.1.0/core/src/ast/special_relations_decl_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/special_relations_decl_plugin.h` & `z3-solver-4.9.1.0/core/src/ast/special_relations_decl_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/static_features.cpp` & `z3-solver-4.9.1.0/core/src/ast/static_features.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/static_features.h` & `z3-solver-4.9.1.0/core/src/ast/static_features.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/substitution/expr_offset.h` & `z3-solver-4.9.1.0/core/src/ast/substitution/expr_offset.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/substitution/expr_offset_map.h` & `z3-solver-4.9.1.0/core/src/ast/substitution/expr_offset_map.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/substitution/matcher.cpp` & `z3-solver-4.9.1.0/core/src/ast/substitution/matcher.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/substitution/matcher.h` & `z3-solver-4.9.1.0/core/src/ast/substitution/matcher.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/substitution/substitution.cpp` & `z3-solver-4.9.1.0/core/src/ast/substitution/substitution.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/substitution/substitution.h` & `z3-solver-4.9.1.0/core/src/ast/substitution/substitution.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/substitution/substitution_tree.cpp` & `z3-solver-4.9.1.0/core/src/ast/substitution/substitution_tree.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/substitution/substitution_tree.h` & `z3-solver-4.9.1.0/core/src/ast/substitution/substitution_tree.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/substitution/unifier.cpp` & `z3-solver-4.9.1.0/core/src/ast/substitution/unifier.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/substitution/unifier.h` & `z3-solver-4.9.1.0/core/src/ast/substitution/unifier.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/substitution/var_offset_map.h` & `z3-solver-4.9.1.0/core/src/ast/substitution/var_offset_map.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/used_symbols.h` & `z3-solver-4.9.1.0/core/src/ast/used_symbols.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/used_vars.cpp` & `z3-solver-4.9.1.0/core/src/ast/used_vars.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/used_vars.h` & `z3-solver-4.9.1.0/core/src/ast/used_vars.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/value_generator.cpp` & `z3-solver-4.9.1.0/core/src/ast/value_generator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/value_generator.h` & `z3-solver-4.9.1.0/core/src/ast/value_generator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/ast/well_sorted.cpp` & `z3-solver-4.9.1.0/core/src/ast/well_sorted.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/basic_cmds.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/basic_cmds.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/cmd_context.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/cmd_context.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/cmd_context.h` & `z3-solver-4.9.1.0/core/src/cmd_context/cmd_context.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/cmd_context_to_goal.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/cmd_context_to_goal.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/cmd_util.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/cmd_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/cmd_util.h` & `z3-solver-4.9.1.0/core/src/cmd_context/cmd_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/echo_tactic.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/echo_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/eval_cmd.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/eval_cmd.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/extra_cmds/dbg_cmds.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/extra_cmds/dbg_cmds.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/extra_cmds/polynomial_cmds.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/extra_cmds/polynomial_cmds.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/extra_cmds/subpaving_cmds.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/extra_cmds/subpaving_cmds.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/parametric_cmd.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/parametric_cmd.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/parametric_cmd.h` & `z3-solver-4.9.1.0/core/src/cmd_context/parametric_cmd.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/pdecl.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/pdecl.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/pdecl.h` & `z3-solver-4.9.1.0/core/src/cmd_context/pdecl.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/simplify_cmd.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/simplify_cmd.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/tactic_cmds.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/tactic_cmds.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/tactic_cmds.h` & `z3-solver-4.9.1.0/core/src/cmd_context/tactic_cmds.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/tactic_manager.cpp` & `z3-solver-4.9.1.0/core/src/cmd_context/tactic_manager.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/cmd_context/tactic_manager.h` & `z3-solver-4.9.1.0/core/src/cmd_context/tactic_manager.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/automata/automaton.h` & `z3-solver-4.9.1.0/core/src/math/automata/automaton.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/automata/boolean_algebra.h` & `z3-solver-4.9.1.0/core/src/math/automata/boolean_algebra.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/automata/symbolic_automata.h` & `z3-solver-4.9.1.0/core/src/math/automata/symbolic_automata.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/automata/symbolic_automata_def.h` & `z3-solver-4.9.1.0/core/src/math/automata/symbolic_automata_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/dd/dd_bdd.cpp` & `z3-solver-4.9.1.0/core/src/math/dd/dd_bdd.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/dd/dd_bdd.h` & `z3-solver-4.9.1.0/core/src/math/dd/dd_bdd.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/dd/dd_pdd.cpp` & `z3-solver-4.9.1.0/core/src/math/dd/dd_pdd.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/dd/dd_pdd.h` & `z3-solver-4.9.1.0/core/src/math/dd/dd_pdd.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/dd/pdd_eval.h` & `z3-solver-4.9.1.0/core/src/math/dd/pdd_eval.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/dd/pdd_interval.h` & `z3-solver-4.9.1.0/core/src/math/dd/pdd_interval.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/grobner/grobner.cpp` & `z3-solver-4.9.1.0/core/src/math/grobner/grobner.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/grobner/grobner.h` & `z3-solver-4.9.1.0/core/src/math/grobner/grobner.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/grobner/pdd_simplifier.cpp` & `z3-solver-4.9.1.0/core/src/math/grobner/pdd_simplifier.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/grobner/pdd_simplifier.h` & `z3-solver-4.9.1.0/core/src/math/grobner/pdd_simplifier.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/grobner/pdd_solver.cpp` & `z3-solver-4.9.1.0/core/src/math/grobner/pdd_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/grobner/pdd_solver.h` & `z3-solver-4.9.1.0/core/src/math/grobner/pdd_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/hilbert/heap_trie.h` & `z3-solver-4.9.1.0/core/src/math/hilbert/heap_trie.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/hilbert/hilbert_basis.cpp` & `z3-solver-4.9.1.0/core/src/math/hilbert/hilbert_basis.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/hilbert/hilbert_basis.h` & `z3-solver-4.9.1.0/core/src/math/hilbert/hilbert_basis.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/interval/dep_intervals.cpp` & `z3-solver-4.9.1.0/core/src/math/interval/dep_intervals.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/interval/dep_intervals.h` & `z3-solver-4.9.1.0/core/src/math/interval/dep_intervals.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/interval/interval.h` & `z3-solver-4.9.1.0/core/src/math/interval/interval.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/interval/interval_def.h` & `z3-solver-4.9.1.0/core/src/math/interval/interval_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/math/lp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/binary_heap_priority_queue.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/binary_heap_priority_queue.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/binary_heap_priority_queue.h` & `z3-solver-4.9.1.0/core/src/math/lp/binary_heap_priority_queue.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/binary_heap_priority_queue_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/binary_heap_priority_queue_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/binary_heap_upair_queue.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/binary_heap_upair_queue.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/binary_heap_upair_queue.h` & `z3-solver-4.9.1.0/core/src/math/lp/binary_heap_upair_queue.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/binary_heap_upair_queue_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/binary_heap_upair_queue_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/bound_analyzer_on_row.h` & `z3-solver-4.9.1.0/core/src/math/lp/bound_analyzer_on_row.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/column_info.h` & `z3-solver-4.9.1.0/core/src/math/lp/column_info.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/column_namer.h` & `z3-solver-4.9.1.0/core/src/math/lp/column_namer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/conversion_helper.h` & `z3-solver-4.9.1.0/core/src/math/lp/conversion_helper.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/core_solver_pretty_printer.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/core_solver_pretty_printer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/core_solver_pretty_printer.h` & `z3-solver-4.9.1.0/core/src/math/lp/core_solver_pretty_printer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/core_solver_pretty_printer_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/core_solver_pretty_printer_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/cross_nested.h` & `z3-solver-4.9.1.0/core/src/math/lp/cross_nested.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/dense_matrix.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/dense_matrix.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/dense_matrix.h` & `z3-solver-4.9.1.0/core/src/math/lp/dense_matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/dense_matrix_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/dense_matrix_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/emonics.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/emonics.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/emonics.h` & `z3-solver-4.9.1.0/core/src/math/lp/emonics.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/eta_matrix.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/eta_matrix.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/eta_matrix.h` & `z3-solver-4.9.1.0/core/src/math/lp/eta_matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/eta_matrix_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/eta_matrix_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/explanation.h` & `z3-solver-4.9.1.0/core/src/math/lp/explanation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/factorization.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/factorization.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/factorization.h` & `z3-solver-4.9.1.0/core/src/math/lp/factorization.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/factorization_factory_imp.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/factorization_factory_imp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/factorization_factory_imp.h` & `z3-solver-4.9.1.0/core/src/math/lp/factorization_factory_imp.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/general_matrix.h` & `z3-solver-4.9.1.0/core/src/math/lp/general_matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/gomory.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/gomory.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/gomory.h` & `z3-solver-4.9.1.0/core/src/math/lp/gomory.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/hnf.h` & `z3-solver-4.9.1.0/core/src/math/lp/hnf.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/hnf_cutter.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/hnf_cutter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/hnf_cutter.h` & `z3-solver-4.9.1.0/core/src/math/lp/hnf_cutter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/horner.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/horner.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/horner.h` & `z3-solver-4.9.1.0/core/src/math/lp/horner.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/implied_bound.h` & `z3-solver-4.9.1.0/core/src/math/lp/implied_bound.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/incremental_vector.h` & `z3-solver-4.9.1.0/core/src/math/lp/incremental_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/indexed_value.h` & `z3-solver-4.9.1.0/core/src/math/lp/indexed_value.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/indexed_vector.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/indexed_vector.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/indexed_vector.h` & `z3-solver-4.9.1.0/core/src/math/lp/indexed_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/indexed_vector_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/indexed_vector_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/indexer_of_constraints.h` & `z3-solver-4.9.1.0/core/src/math/lp/indexer_of_constraints.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/int_branch.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/int_branch.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/int_branch.h` & `z3-solver-4.9.1.0/core/src/math/lp/int_branch.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/int_cube.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/int_cube.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/int_cube.h` & `z3-solver-4.9.1.0/core/src/math/lp/int_cube.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/int_gcd_test.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/int_gcd_test.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/int_gcd_test.h` & `z3-solver-4.9.1.0/core/src/math/lp/int_gcd_test.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/int_solver.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/int_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/int_solver.h` & `z3-solver-4.9.1.0/core/src/math/lp/int_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lar_constraints.h` & `z3-solver-4.9.1.0/core/src/math/lp/lar_constraints.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lar_core_solver.h` & `z3-solver-4.9.1.0/core/src/math/lp/lar_core_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lar_core_solver_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/lar_core_solver_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lar_solver.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/lar_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lar_solver.h` & `z3-solver-4.9.1.0/core/src/math/lp/lar_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lar_term.h` & `z3-solver-4.9.1.0/core/src/math/lp/lar_term.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lia_move.h` & `z3-solver-4.9.1.0/core/src/math/lp/lia_move.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_api.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_api.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_bound_propagator.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_bound_propagator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_core_solver_base.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/lp_core_solver_base.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_core_solver_base.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_core_solver_base.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_core_solver_base_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_core_solver_base_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_dual_core_solver.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/lp_dual_core_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_dual_core_solver.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_dual_core_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_dual_core_solver_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_dual_core_solver_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_dual_simplex.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/lp_dual_simplex.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_dual_simplex.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_dual_simplex.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_dual_simplex_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_dual_simplex_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_primal_core_solver.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/lp_primal_core_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_primal_core_solver.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_primal_core_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_primal_core_solver_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_primal_core_solver_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_primal_core_solver_tableau_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_primal_core_solver_tableau_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_primal_simplex.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/lp_primal_simplex.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_primal_simplex.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_primal_simplex.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_primal_simplex_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_primal_simplex_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_settings.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/lp_settings.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_settings.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_settings.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_settings_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_settings_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_solver.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/lp_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_solver.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_solver_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_solver_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_types.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_types.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lp_utils.h` & `z3-solver-4.9.1.0/core/src/math/lp/lp_utils.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lu.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/lu.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lu.h` & `z3-solver-4.9.1.0/core/src/math/lp/lu.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/lu_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/lu_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/matrix.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/matrix.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/matrix.h` & `z3-solver-4.9.1.0/core/src/math/lp/matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/matrix_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/matrix_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/mon_eq.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/mon_eq.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/monic.h` & `z3-solver-4.9.1.0/core/src/math/lp/monic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/monomial_bounds.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/monomial_bounds.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/monomial_bounds.h` & `z3-solver-4.9.1.0/core/src/math/lp/monomial_bounds.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/mps_reader.h` & `z3-solver-4.9.1.0/core/src/math/lp/mps_reader.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nex.h` & `z3-solver-4.9.1.0/core/src/math/lp/nex.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nex_creator.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/nex_creator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nex_creator.h` & `z3-solver-4.9.1.0/core/src/math/lp/nex_creator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_basics_lemmas.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/nla_basics_lemmas.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_basics_lemmas.h` & `z3-solver-4.9.1.0/core/src/math/lp/nla_basics_lemmas.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_common.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/nla_common.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_common.h` & `z3-solver-4.9.1.0/core/src/math/lp/nla_common.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_core.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/nla_core.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_core.h` & `z3-solver-4.9.1.0/core/src/math/lp/nla_core.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_defs.h` & `z3-solver-4.9.1.0/core/src/math/lp/nla_defs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_intervals.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/nla_intervals.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_intervals.h` & `z3-solver-4.9.1.0/core/src/math/lp/nla_intervals.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_monotone_lemmas.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/nla_monotone_lemmas.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_monotone_lemmas.h` & `z3-solver-4.9.1.0/core/src/math/lp/nla_monotone_lemmas.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_order_lemmas.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/nla_order_lemmas.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_order_lemmas.h` & `z3-solver-4.9.1.0/core/src/math/lp/nla_order_lemmas.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_settings.h` & `z3-solver-4.9.1.0/core/src/math/lp/nla_settings.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_solver.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/nla_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_solver.h` & `z3-solver-4.9.1.0/core/src/math/lp/nla_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_tangent_lemmas.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/nla_tangent_lemmas.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nla_tangent_lemmas.h` & `z3-solver-4.9.1.0/core/src/math/lp/nla_tangent_lemmas.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nra_solver.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/nra_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/nra_solver.h` & `z3-solver-4.9.1.0/core/src/math/lp/nra_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/numeric_pair.h` & `z3-solver-4.9.1.0/core/src/math/lp/numeric_pair.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/permutation_matrix.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/permutation_matrix.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/permutation_matrix.h` & `z3-solver-4.9.1.0/core/src/math/lp/permutation_matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/permutation_matrix_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/permutation_matrix_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/random_updater.h` & `z3-solver-4.9.1.0/core/src/math/lp/random_updater.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/random_updater_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/random_updater_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/row_eta_matrix.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/row_eta_matrix.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/row_eta_matrix.h` & `z3-solver-4.9.1.0/core/src/math/lp/row_eta_matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/row_eta_matrix_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/row_eta_matrix_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/scaler.h` & `z3-solver-4.9.1.0/core/src/math/lp/scaler.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/scaler_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/scaler_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/sparse_vector.h` & `z3-solver-4.9.1.0/core/src/math/lp/sparse_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/square_dense_submatrix.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/square_dense_submatrix.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/square_dense_submatrix.h` & `z3-solver-4.9.1.0/core/src/math/lp/square_dense_submatrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/square_dense_submatrix_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/square_dense_submatrix_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/square_sparse_matrix.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/square_sparse_matrix.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/square_sparse_matrix.h` & `z3-solver-4.9.1.0/core/src/math/lp/square_sparse_matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/square_sparse_matrix_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/square_sparse_matrix_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/stacked_vector.h` & `z3-solver-4.9.1.0/core/src/math/lp/stacked_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/static_matrix.cpp` & `z3-solver-4.9.1.0/core/src/math/lp/static_matrix.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/static_matrix.h` & `z3-solver-4.9.1.0/core/src/math/lp/static_matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/static_matrix_def.h` & `z3-solver-4.9.1.0/core/src/math/lp/static_matrix_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/tail_matrix.h` & `z3-solver-4.9.1.0/core/src/math/lp/tail_matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/test_bound_analyzer.h` & `z3-solver-4.9.1.0/core/src/math/lp/test_bound_analyzer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/u_set.h` & `z3-solver-4.9.1.0/core/src/math/lp/u_set.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/ul_pair.h` & `z3-solver-4.9.1.0/core/src/math/lp/ul_pair.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/var_eqs.h` & `z3-solver-4.9.1.0/core/src/math/lp/var_eqs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/lp/var_register.h` & `z3-solver-4.9.1.0/core/src/math/lp/var_register.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/algebraic_numbers.cpp` & `z3-solver-4.9.1.0/core/src/math/polynomial/algebraic_numbers.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/algebraic_numbers.h` & `z3-solver-4.9.1.0/core/src/math/polynomial/algebraic_numbers.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/algebraic_params.pyg` & `z3-solver-4.9.1.0/core/src/math/polynomial/algebraic_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/linear_eq_solver.h` & `z3-solver-4.9.1.0/core/src/math/polynomial/linear_eq_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/polynomial.cpp` & `z3-solver-4.9.1.0/core/src/math/polynomial/polynomial.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/polynomial.h` & `z3-solver-4.9.1.0/core/src/math/polynomial/polynomial.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/polynomial_cache.cpp` & `z3-solver-4.9.1.0/core/src/math/polynomial/polynomial_cache.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/polynomial_cache.h` & `z3-solver-4.9.1.0/core/src/math/polynomial/polynomial_cache.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/polynomial_primes.h` & `z3-solver-4.9.1.0/core/src/math/polynomial/polynomial_primes.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/polynomial_var2value.h` & `z3-solver-4.9.1.0/core/src/math/polynomial/polynomial_var2value.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/rpolynomial.cpp` & `z3-solver-4.9.1.0/core/src/math/polynomial/rpolynomial.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/rpolynomial.h` & `z3-solver-4.9.1.0/core/src/math/polynomial/rpolynomial.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/sexpr2upolynomial.cpp` & `z3-solver-4.9.1.0/core/src/math/polynomial/sexpr2upolynomial.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/sexpr2upolynomial.h` & `z3-solver-4.9.1.0/core/src/math/polynomial/sexpr2upolynomial.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/upolynomial.cpp` & `z3-solver-4.9.1.0/core/src/math/polynomial/upolynomial.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/upolynomial.h` & `z3-solver-4.9.1.0/core/src/math/polynomial/upolynomial.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/upolynomial_factorization.cpp` & `z3-solver-4.9.1.0/core/src/math/polynomial/upolynomial_factorization.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/upolynomial_factorization.h` & `z3-solver-4.9.1.0/core/src/math/polynomial/upolynomial_factorization.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/polynomial/upolynomial_factorization_int.h` & `z3-solver-4.9.1.0/core/src/math/polynomial/upolynomial_factorization_int.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/realclosure/mpz_matrix.cpp` & `z3-solver-4.9.1.0/core/src/math/realclosure/mpz_matrix.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/realclosure/mpz_matrix.h` & `z3-solver-4.9.1.0/core/src/math/realclosure/mpz_matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/realclosure/rcf_params.pyg` & `z3-solver-4.9.1.0/core/src/math/realclosure/rcf_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/realclosure/realclosure.cpp` & `z3-solver-4.9.1.0/core/src/math/realclosure/realclosure.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/realclosure/realclosure.h` & `z3-solver-4.9.1.0/core/src/math/realclosure/realclosure.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/simplex/bit_matrix.cpp` & `z3-solver-4.9.1.0/core/src/math/simplex/bit_matrix.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/simplex/bit_matrix.h` & `z3-solver-4.9.1.0/core/src/math/simplex/bit_matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/simplex/model_based_opt.cpp` & `z3-solver-4.9.1.0/core/src/math/simplex/model_based_opt.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/simplex/model_based_opt.h` & `z3-solver-4.9.1.0/core/src/math/simplex/model_based_opt.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/simplex/network_flow.h` & `z3-solver-4.9.1.0/core/src/math/simplex/network_flow.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/simplex/network_flow_def.h` & `z3-solver-4.9.1.0/core/src/math/simplex/network_flow_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/simplex/simplex.cpp` & `z3-solver-4.9.1.0/core/src/math/simplex/simplex.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/simplex/simplex.h` & `z3-solver-4.9.1.0/core/src/math/simplex/simplex.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/simplex/simplex_def.h` & `z3-solver-4.9.1.0/core/src/math/simplex/simplex_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/simplex/sparse_matrix.h` & `z3-solver-4.9.1.0/core/src/math/simplex/sparse_matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/simplex/sparse_matrix_def.h` & `z3-solver-4.9.1.0/core/src/math/simplex/sparse_matrix_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/simplex/sparse_matrix_ops.h` & `z3-solver-4.9.1.0/core/src/math/simplex/sparse_matrix_ops.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/subpaving.cpp` & `z3-solver-4.9.1.0/core/src/math/subpaving/subpaving.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/subpaving.h` & `z3-solver-4.9.1.0/core/src/math/subpaving/subpaving.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_hwf.h` & `z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_hwf.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_mpf.h` & `z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_mpf.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_mpff.h` & `z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_mpff.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_mpfx.h` & `z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_mpfx.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_mpq.h` & `z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_mpq.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_t.h` & `z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_t.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_t_def.h` & `z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_t_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/subpaving_types.h` & `z3-solver-4.9.1.0/core/src/math/subpaving/subpaving_types.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/tactic/expr2subpaving.cpp` & `z3-solver-4.9.1.0/core/src/math/subpaving/tactic/expr2subpaving.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/tactic/expr2subpaving.h` & `z3-solver-4.9.1.0/core/src/math/subpaving/tactic/expr2subpaving.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/math/subpaving/tactic/subpaving_tactic.cpp` & `z3-solver-4.9.1.0/core/src/math/subpaving/tactic/subpaving_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/array_factory.cpp` & `z3-solver-4.9.1.0/core/src/model/array_factory.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/array_factory.h` & `z3-solver-4.9.1.0/core/src/model/array_factory.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/char_factory.h` & `z3-solver-4.9.1.0/core/src/model/char_factory.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/datatype_factory.cpp` & `z3-solver-4.9.1.0/core/src/model/datatype_factory.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/datatype_factory.h` & `z3-solver-4.9.1.0/core/src/model/datatype_factory.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/fpa_factory.h` & `z3-solver-4.9.1.0/core/src/model/fpa_factory.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/func_interp.cpp` & `z3-solver-4.9.1.0/core/src/model/func_interp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/func_interp.h` & `z3-solver-4.9.1.0/core/src/model/func_interp.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model.cpp` & `z3-solver-4.9.1.0/core/src/model/model.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model.h` & `z3-solver-4.9.1.0/core/src/model/model.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model2expr.cpp` & `z3-solver-4.9.1.0/core/src/model/model2expr.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model2expr.h` & `z3-solver-4.9.1.0/core/src/model/model2expr.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_core.cpp` & `z3-solver-4.9.1.0/core/src/model/model_core.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_core.h` & `z3-solver-4.9.1.0/core/src/model/model_core.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_evaluator.cpp` & `z3-solver-4.9.1.0/core/src/model/model_evaluator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_evaluator.h` & `z3-solver-4.9.1.0/core/src/model/model_evaluator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_evaluator_params.pyg` & `z3-solver-4.9.1.0/core/src/model/model_evaluator_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_implicant.cpp` & `z3-solver-4.9.1.0/core/src/model/model_implicant.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_implicant.h` & `z3-solver-4.9.1.0/core/src/model/model_implicant.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_macro_solver.cpp` & `z3-solver-4.9.1.0/core/src/model/model_macro_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_macro_solver.h` & `z3-solver-4.9.1.0/core/src/model/model_macro_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_params.pyg` & `z3-solver-4.9.1.0/core/src/model/model_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_pp.cpp` & `z3-solver-4.9.1.0/core/src/model/model_pp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_smt2_pp.cpp` & `z3-solver-4.9.1.0/core/src/model/model_smt2_pp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/model_v2_pp.cpp` & `z3-solver-4.9.1.0/core/src/model/model_v2_pp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/numeral_factory.cpp` & `z3-solver-4.9.1.0/core/src/model/numeral_factory.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/numeral_factory.h` & `z3-solver-4.9.1.0/core/src/model/numeral_factory.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/seq_factory.h` & `z3-solver-4.9.1.0/core/src/model/seq_factory.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/struct_factory.cpp` & `z3-solver-4.9.1.0/core/src/model/struct_factory.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/struct_factory.h` & `z3-solver-4.9.1.0/core/src/model/struct_factory.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/value_factory.cpp` & `z3-solver-4.9.1.0/core/src/model/value_factory.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/model/value_factory.h` & `z3-solver-4.9.1.0/core/src/model/value_factory.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/bind_variables.cpp` & `z3-solver-4.9.1.0/core/src/muz/base/bind_variables.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/bind_variables.h` & `z3-solver-4.9.1.0/core/src/muz/base/bind_variables.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_boogie_proof.cpp` & `z3-solver-4.9.1.0/core/src/muz/base/dl_boogie_proof.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_boogie_proof.h` & `z3-solver-4.9.1.0/core/src/muz/base/dl_boogie_proof.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_context.cpp` & `z3-solver-4.9.1.0/core/src/muz/base/dl_context.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_context.h` & `z3-solver-4.9.1.0/core/src/muz/base/dl_context.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_costs.cpp` & `z3-solver-4.9.1.0/core/src/muz/base/dl_costs.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_costs.h` & `z3-solver-4.9.1.0/core/src/muz/base/dl_costs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_engine_base.h` & `z3-solver-4.9.1.0/core/src/muz/base/dl_engine_base.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_rule.cpp` & `z3-solver-4.9.1.0/core/src/muz/base/dl_rule.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_rule.h` & `z3-solver-4.9.1.0/core/src/muz/base/dl_rule.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_rule_set.cpp` & `z3-solver-4.9.1.0/core/src/muz/base/dl_rule_set.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_rule_set.h` & `z3-solver-4.9.1.0/core/src/muz/base/dl_rule_set.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_rule_subsumption_index.cpp` & `z3-solver-4.9.1.0/core/src/muz/base/dl_rule_subsumption_index.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_rule_subsumption_index.h` & `z3-solver-4.9.1.0/core/src/muz/base/dl_rule_subsumption_index.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_rule_transformer.cpp` & `z3-solver-4.9.1.0/core/src/muz/base/dl_rule_transformer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_rule_transformer.h` & `z3-solver-4.9.1.0/core/src/muz/base/dl_rule_transformer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_util.cpp` & `z3-solver-4.9.1.0/core/src/muz/base/dl_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/dl_util.h` & `z3-solver-4.9.1.0/core/src/muz/base/dl_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/fp_params.pyg` & `z3-solver-4.9.1.0/core/src/muz/base/fp_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/hnf.cpp` & `z3-solver-4.9.1.0/core/src/muz/base/hnf.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/hnf.h` & `z3-solver-4.9.1.0/core/src/muz/base/hnf.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/rule_properties.cpp` & `z3-solver-4.9.1.0/core/src/muz/base/rule_properties.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/base/rule_properties.h` & `z3-solver-4.9.1.0/core/src/muz/base/rule_properties.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/bmc/dl_bmc_engine.cpp` & `z3-solver-4.9.1.0/core/src/muz/bmc/dl_bmc_engine.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/bmc/dl_bmc_engine.h` & `z3-solver-4.9.1.0/core/src/muz/bmc/dl_bmc_engine.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/clp/clp_context.cpp` & `z3-solver-4.9.1.0/core/src/muz/clp/clp_context.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/clp/clp_context.h` & `z3-solver-4.9.1.0/core/src/muz/clp/clp_context.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/dataflow/dataflow.h` & `z3-solver-4.9.1.0/core/src/muz/dataflow/dataflow.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/dataflow/reachability.h` & `z3-solver-4.9.1.0/core/src/muz/dataflow/reachability.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/ddnf/ddnf.cpp` & `z3-solver-4.9.1.0/core/src/muz/ddnf/ddnf.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/ddnf/ddnf.h` & `z3-solver-4.9.1.0/core/src/muz/ddnf/ddnf.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/fp/datalog_parser.cpp` & `z3-solver-4.9.1.0/core/src/muz/fp/datalog_parser.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/fp/datalog_parser.h` & `z3-solver-4.9.1.0/core/src/muz/fp/datalog_parser.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/fp/dl_cmds.cpp` & `z3-solver-4.9.1.0/core/src/muz/fp/dl_cmds.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/fp/dl_cmds.h` & `z3-solver-4.9.1.0/core/src/muz/fp/dl_cmds.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/fp/dl_register_engine.cpp` & `z3-solver-4.9.1.0/core/src/muz/fp/dl_register_engine.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/fp/dl_register_engine.h` & `z3-solver-4.9.1.0/core/src/muz/fp/dl_register_engine.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/fp/horn_tactic.cpp` & `z3-solver-4.9.1.0/core/src/muz/fp/horn_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/fp/horn_tactic.h` & `z3-solver-4.9.1.0/core/src/muz/fp/horn_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/muz/rel/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/aig_exporter.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/aig_exporter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/aig_exporter.h` & `z3-solver-4.9.1.0/core/src/muz/rel/aig_exporter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/check_relation.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/check_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/check_relation.h` & `z3-solver-4.9.1.0/core/src/muz/rel/check_relation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_base.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_base.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_base.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_base.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_bound_relation.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_bound_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_bound_relation.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_bound_relation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_check_table.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_check_table.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_check_table.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_check_table.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_compiler.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_compiler.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_compiler.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_compiler.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_external_relation.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_external_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_external_relation.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_external_relation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_finite_product_relation.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_finite_product_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_finite_product_relation.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_finite_product_relation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_instruction.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_instruction.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_instruction.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_instruction.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_interval_relation.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_interval_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_interval_relation.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_interval_relation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_lazy_table.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_lazy_table.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_lazy_table.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_lazy_table.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_mk_explanations.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_mk_explanations.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_mk_explanations.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_mk_explanations.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_mk_similarity_compressor.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_mk_similarity_compressor.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_mk_similarity_compressor.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_mk_similarity_compressor.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_mk_simple_joins.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_mk_simple_joins.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_mk_simple_joins.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_mk_simple_joins.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_product_relation.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_product_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_product_relation.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_product_relation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_relation_manager.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_relation_manager.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_relation_manager.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_relation_manager.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_sieve_relation.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_sieve_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_sieve_relation.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_sieve_relation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_sparse_table.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_sparse_table.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_sparse_table.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_sparse_table.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_table.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_table.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_table.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_table.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_table_plugin.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_table_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_table_relation.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_table_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_table_relation.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_table_relation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/dl_vector_relation.h` & `z3-solver-4.9.1.0/core/src/muz/rel/dl_vector_relation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/doc.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/doc.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/doc.h` & `z3-solver-4.9.1.0/core/src/muz/rel/doc.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/karr_relation.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/karr_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/karr_relation.h` & `z3-solver-4.9.1.0/core/src/muz/rel/karr_relation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/rel_context.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/rel_context.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/rel_context.h` & `z3-solver-4.9.1.0/core/src/muz/rel/rel_context.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/tbv.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/tbv.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/tbv.h` & `z3-solver-4.9.1.0/core/src/muz/rel/tbv.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/udoc_relation.cpp` & `z3-solver-4.9.1.0/core/src/muz/rel/udoc_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/rel/udoc_relation.h` & `z3-solver-4.9.1.0/core/src/muz/rel/udoc_relation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/muz/spacer/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_antiunify.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_antiunify.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_antiunify.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_antiunify.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_arith_generalizers.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_arith_generalizers.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_callback.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_callback.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_callback.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_callback.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_context.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_context.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_context.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_context.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_dl_interface.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_dl_interface.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_dl_interface.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_dl_interface.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_farkas_learner.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_farkas_learner.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_farkas_learner.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_farkas_learner.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_generalizers.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_generalizers.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_generalizers.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_generalizers.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_iuc_proof.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_iuc_proof.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_iuc_proof.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_iuc_proof.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_iuc_solver.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_iuc_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_iuc_solver.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_iuc_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_json.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_json.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_json.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_json.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_legacy_frames.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_legacy_frames.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_legacy_frames.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_legacy_frames.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_legacy_mbp.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_legacy_mbp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_legacy_mev.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_legacy_mev.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_legacy_mev.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_legacy_mev.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_manager.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_manager.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_manager.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_manager.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_matrix.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_matrix.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_matrix.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_matrix.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_mbc.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_mbc.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_mbc.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_mbc.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_mev_array.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_mev_array.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_mev_array.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_mev_array.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_notes.txt` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_notes.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_pdr.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_pdr.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_pdr.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_pdr.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_proof_utils.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_proof_utils.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_proof_utils.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_proof_utils.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_prop_solver.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_prop_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_prop_solver.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_prop_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_qe_project.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_qe_project.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_qe_project.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_qe_project.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_quant_generalizer.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_quant_generalizer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_sat_answer.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_sat_answer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_sat_answer.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_sat_answer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_sem_matcher.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_sem_matcher.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_sem_matcher.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_sem_matcher.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_sym_mux.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_sym_mux.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_sym_mux.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_sym_mux.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_unsat_core_learner.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_unsat_core_learner.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_unsat_core_learner.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_unsat_core_learner.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_unsat_core_plugin.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_unsat_core_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_unsat_core_plugin.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_unsat_core_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_util.cpp` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/spacer/spacer_util.h` & `z3-solver-4.9.1.0/core/src/muz/spacer/spacer_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/tab/tab_context.cpp` & `z3-solver-4.9.1.0/core/src/muz/tab/tab_context.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/tab/tab_context.h` & `z3-solver-4.9.1.0/core/src/muz/tab/tab_context.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/muz/transforms/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_array_blast.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_array_blast.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_array_blast.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_array_blast.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_array_eq_rewrite.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_array_eq_rewrite.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_array_eq_rewrite.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_array_eq_rewrite.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_array_instantiation.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_array_instantiation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_array_instantiation.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_array_instantiation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_backwards.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_backwards.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_backwards.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_backwards.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_bit_blast.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_bit_blast.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_bit_blast.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_bit_blast.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_coalesce.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_coalesce.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_coalesce.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_coalesce.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_coi_filter.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_coi_filter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_coi_filter.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_coi_filter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_different.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_different.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_elim_term_ite.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_elim_term_ite.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_elim_term_ite.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_elim_term_ite.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_filter_rules.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_filter_rules.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_filter_rules.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_filter_rules.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_interp_tail_simplifier.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_interp_tail_simplifier.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_interp_tail_simplifier.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_interp_tail_simplifier.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_karr_invariants.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_karr_invariants.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_karr_invariants.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_karr_invariants.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_loop_counter.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_loop_counter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_loop_counter.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_loop_counter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_magic_sets.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_magic_sets.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_magic_sets.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_magic_sets.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_magic_symbolic.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_magic_symbolic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_magic_symbolic.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_magic_symbolic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_quantifier_abstraction.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_quantifier_abstraction.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_quantifier_abstraction.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_quantifier_abstraction.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_quantifier_instantiation.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_quantifier_instantiation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_quantifier_instantiation.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_quantifier_instantiation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_rule_inliner.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_rule_inliner.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_rule_inliner.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_rule_inliner.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_scale.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_scale.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_scale.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_scale.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_separate_negated_tails.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_separate_negated_tails.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_separate_negated_tails.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_separate_negated_tails.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_slice.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_slice.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_slice.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_slice.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_subsumption_checker.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_subsumption_checker.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_subsumption_checker.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_subsumption_checker.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_synchronize.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_synchronize.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_synchronize.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_synchronize.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_unbound_compressor.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_unbound_compressor.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_unbound_compressor.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_unbound_compressor.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_unfold.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_unfold.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_mk_unfold.h` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_mk_unfold.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/muz/transforms/dl_transforms.cpp` & `z3-solver-4.9.1.0/core/src/muz/transforms/dl_transforms.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_assignment.h` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_assignment.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_clause.cpp` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_clause.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_clause.h` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_clause.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_evaluator.cpp` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_evaluator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_evaluator.h` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_evaluator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_explain.cpp` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_explain.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_explain.h` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_explain.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_interval_set.cpp` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_interval_set.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_interval_set.h` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_interval_set.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_justification.h` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_justification.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_params.pyg` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_scoped_literal_vector.h` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_scoped_literal_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_solver.cpp` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_solver.h` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_types.cpp` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_types.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/nlsat_types.h` & `z3-solver-4.9.1.0/core/src/nlsat/nlsat_types.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/tactic/goal2nlsat.cpp` & `z3-solver-4.9.1.0/core/src/nlsat/tactic/goal2nlsat.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/tactic/goal2nlsat.h` & `z3-solver-4.9.1.0/core/src/nlsat/tactic/goal2nlsat.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/tactic/nlsat_tactic.cpp` & `z3-solver-4.9.1.0/core/src/nlsat/tactic/nlsat_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/nlsat/tactic/qfnra_nlsat_tactic.cpp` & `z3-solver-4.9.1.0/core/src/nlsat/tactic/qfnra_nlsat_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/maxcore.cpp` & `z3-solver-4.9.1.0/core/src/opt/maxcore.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/maxcore.h` & `z3-solver-4.9.1.0/core/src/opt/maxcore.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/maxlex.cpp` & `z3-solver-4.9.1.0/core/src/opt/maxlex.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/maxsmt.cpp` & `z3-solver-4.9.1.0/core/src/opt/maxsmt.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/maxsmt.h` & `z3-solver-4.9.1.0/core/src/opt/maxsmt.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_cmds.cpp` & `z3-solver-4.9.1.0/core/src/opt/opt_cmds.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_context.cpp` & `z3-solver-4.9.1.0/core/src/opt/opt_context.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_context.h` & `z3-solver-4.9.1.0/core/src/opt/opt_context.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_cores.cpp` & `z3-solver-4.9.1.0/core/src/opt/opt_cores.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_cores.h` & `z3-solver-4.9.1.0/core/src/opt/opt_cores.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_lns.cpp` & `z3-solver-4.9.1.0/core/src/opt/opt_lns.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_lns.h` & `z3-solver-4.9.1.0/core/src/opt/opt_lns.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_params.pyg` & `z3-solver-4.9.1.0/core/src/opt/opt_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_pareto.cpp` & `z3-solver-4.9.1.0/core/src/opt/opt_pareto.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_pareto.h` & `z3-solver-4.9.1.0/core/src/opt/opt_pareto.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_parse.cpp` & `z3-solver-4.9.1.0/core/src/opt/opt_parse.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_preprocess.cpp` & `z3-solver-4.9.1.0/core/src/opt/opt_preprocess.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_preprocess.h` & `z3-solver-4.9.1.0/core/src/opt/opt_preprocess.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_sls_solver.h` & `z3-solver-4.9.1.0/core/src/opt/opt_sls_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_solver.cpp` & `z3-solver-4.9.1.0/core/src/opt/opt_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/opt_solver.h` & `z3-solver-4.9.1.0/core/src/opt/opt_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/optsmt.cpp` & `z3-solver-4.9.1.0/core/src/opt/optsmt.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/optsmt.h` & `z3-solver-4.9.1.0/core/src/opt/optsmt.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/pb_sls.cpp` & `z3-solver-4.9.1.0/core/src/opt/pb_sls.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/pb_sls.h` & `z3-solver-4.9.1.0/core/src/opt/pb_sls.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/sortmax.cpp` & `z3-solver-4.9.1.0/core/src/opt/sortmax.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/totalizer.cpp` & `z3-solver-4.9.1.0/core/src/opt/totalizer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/totalizer.h` & `z3-solver-4.9.1.0/core/src/opt/totalizer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/opt/wmax.cpp` & `z3-solver-4.9.1.0/core/src/opt/wmax.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/params/arith_rewriter_params.pyg` & `z3-solver-4.9.1.0/core/src/params/arith_rewriter_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/params/array_rewriter_params.pyg` & `z3-solver-4.9.1.0/core/src/params/array_rewriter_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/params/bit_blaster_params.h` & `z3-solver-4.9.1.0/core/src/params/bit_blaster_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/params/bool_rewriter_params.pyg` & `z3-solver-4.9.1.0/core/src/params/bool_rewriter_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/params/bv_rewriter_params.pyg` & `z3-solver-4.9.1.0/core/src/params/bv_rewriter_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/params/context_params.cpp` & `z3-solver-4.9.1.0/core/src/params/context_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/params/context_params.h` & `z3-solver-4.9.1.0/core/src/params/context_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/params/pattern_inference_params.cpp` & `z3-solver-4.9.1.0/core/src/params/pattern_inference_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/params/pattern_inference_params.h` & `z3-solver-4.9.1.0/core/src/params/pattern_inference_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/params/pattern_inference_params_helper.pyg` & `z3-solver-4.9.1.0/core/src/params/pattern_inference_params_helper.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/params/poly_rewriter_params.pyg` & `z3-solver-4.9.1.0/core/src/params/poly_rewriter_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/params/rewriter_params.pyg` & `z3-solver-4.9.1.0/core/src/params/rewriter_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/smt2/marshal.cpp` & `z3-solver-4.9.1.0/core/src/parsers/smt2/marshal.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/smt2/smt2parser.cpp` & `z3-solver-4.9.1.0/core/src/parsers/smt2/smt2parser.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/smt2/smt2parser.h` & `z3-solver-4.9.1.0/core/src/parsers/smt2/smt2parser.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/smt2/smt2scanner.cpp` & `z3-solver-4.9.1.0/core/src/parsers/smt2/smt2scanner.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/smt2/smt2scanner.h` & `z3-solver-4.9.1.0/core/src/parsers/smt2/smt2scanner.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/util/cost_parser.cpp` & `z3-solver-4.9.1.0/core/src/parsers/util/cost_parser.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/util/cost_parser.h` & `z3-solver-4.9.1.0/core/src/parsers/util/cost_parser.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/util/pattern_validation.cpp` & `z3-solver-4.9.1.0/core/src/parsers/util/pattern_validation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/util/pattern_validation.h` & `z3-solver-4.9.1.0/core/src/parsers/util/pattern_validation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/util/scanner.cpp` & `z3-solver-4.9.1.0/core/src/parsers/util/scanner.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/util/scanner.h` & `z3-solver-4.9.1.0/core/src/parsers/util/scanner.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/util/simple_parser.cpp` & `z3-solver-4.9.1.0/core/src/parsers/util/simple_parser.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/parsers/util/simple_parser.h` & `z3-solver-4.9.1.0/core/src/parsers/util/simple_parser.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/lite/qe_lite.cpp` & `z3-solver-4.9.1.0/core/src/qe/lite/qe_lite.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/lite/qe_lite.h` & `z3-solver-4.9.1.0/core/src/qe/lite/qe_lite.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/mbp/mbp_arith.cpp` & `z3-solver-4.9.1.0/core/src/qe/mbp/mbp_arith.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/mbp/mbp_arith.h` & `z3-solver-4.9.1.0/core/src/qe/mbp/mbp_arith.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/mbp/mbp_arrays.cpp` & `z3-solver-4.9.1.0/core/src/qe/mbp/mbp_arrays.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/mbp/mbp_arrays.h` & `z3-solver-4.9.1.0/core/src/qe/mbp/mbp_arrays.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/mbp/mbp_datatypes.cpp` & `z3-solver-4.9.1.0/core/src/qe/mbp/mbp_datatypes.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/mbp/mbp_datatypes.h` & `z3-solver-4.9.1.0/core/src/qe/mbp/mbp_datatypes.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/mbp/mbp_plugin.cpp` & `z3-solver-4.9.1.0/core/src/qe/mbp/mbp_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/mbp/mbp_plugin.h` & `z3-solver-4.9.1.0/core/src/qe/mbp/mbp_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/mbp/mbp_solve_plugin.cpp` & `z3-solver-4.9.1.0/core/src/qe/mbp/mbp_solve_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/mbp/mbp_solve_plugin.h` & `z3-solver-4.9.1.0/core/src/qe/mbp/mbp_solve_plugin.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/mbp/mbp_term_graph.cpp` & `z3-solver-4.9.1.0/core/src/qe/mbp/mbp_term_graph.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/mbp/mbp_term_graph.h` & `z3-solver-4.9.1.0/core/src/qe/mbp/mbp_term_graph.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/nlarith_util.cpp` & `z3-solver-4.9.1.0/core/src/qe/nlarith_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/nlarith_util.h` & `z3-solver-4.9.1.0/core/src/qe/nlarith_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/nlqsat.cpp` & `z3-solver-4.9.1.0/core/src/qe/nlqsat.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/nlqsat.h` & `z3-solver-4.9.1.0/core/src/qe/nlqsat.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe.cpp` & `z3-solver-4.9.1.0/core/src/qe/qe.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe.h` & `z3-solver-4.9.1.0/core/src/qe/qe.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe_arith_plugin.cpp` & `z3-solver-4.9.1.0/core/src/qe/qe_arith_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe_array_plugin.cpp` & `z3-solver-4.9.1.0/core/src/qe/qe_array_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe_bool_plugin.cpp` & `z3-solver-4.9.1.0/core/src/qe/qe_bool_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe_bv_plugin.cpp` & `z3-solver-4.9.1.0/core/src/qe/qe_bv_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe_cmd.cpp` & `z3-solver-4.9.1.0/core/src/qe/qe_cmd.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe_datatype_plugin.cpp` & `z3-solver-4.9.1.0/core/src/qe/qe_datatype_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe_dl_plugin.cpp` & `z3-solver-4.9.1.0/core/src/qe/qe_dl_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe_mbi.cpp` & `z3-solver-4.9.1.0/core/src/qe/qe_mbi.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe_mbi.h` & `z3-solver-4.9.1.0/core/src/qe/qe_mbi.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe_mbp.cpp` & `z3-solver-4.9.1.0/core/src/qe/qe_mbp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe_mbp.h` & `z3-solver-4.9.1.0/core/src/qe/qe_mbp.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qe_tactic.cpp` & `z3-solver-4.9.1.0/core/src/qe/qe_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qsat.cpp` & `z3-solver-4.9.1.0/core/src/qe/qsat.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/qe/qsat.h` & `z3-solver-4.9.1.0/core/src/qe/qsat.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/sat/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/dimacs.cpp` & `z3-solver-4.9.1.0/core/src/sat/dimacs.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/dimacs.h` & `z3-solver-4.9.1.0/core/src/sat/dimacs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_aig_cuts.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_aig_cuts.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_aig_cuts.h` & `z3-solver-4.9.1.0/core/src/sat/sat_aig_cuts.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_aig_finder.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_aig_finder.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_aig_finder.h` & `z3-solver-4.9.1.0/core/src/sat/sat_aig_finder.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_allocator.h` & `z3-solver-4.9.1.0/core/src/sat/sat_allocator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_anf_simplifier.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_anf_simplifier.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_anf_simplifier.h` & `z3-solver-4.9.1.0/core/src/sat/sat_anf_simplifier.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_asymm_branch.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_asymm_branch.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_asymm_branch.h` & `z3-solver-4.9.1.0/core/src/sat/sat_asymm_branch.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_asymm_branch_params.pyg` & `z3-solver-4.9.1.0/core/src/sat/sat_asymm_branch_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_bcd.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_bcd.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_bcd.h` & `z3-solver-4.9.1.0/core/src/sat/sat_bcd.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_big.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_big.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_big.h` & `z3-solver-4.9.1.0/core/src/sat/sat_big.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_binspr.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_binspr.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_binspr.h` & `z3-solver-4.9.1.0/core/src/sat/sat_binspr.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_clause.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_clause.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_clause.h` & `z3-solver-4.9.1.0/core/src/sat/sat_clause.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_clause_set.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_clause_set.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_clause_set.h` & `z3-solver-4.9.1.0/core/src/sat/sat_clause_set.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_clause_use_list.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_clause_use_list.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_clause_use_list.h` & `z3-solver-4.9.1.0/core/src/sat/sat_clause_use_list.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_cleaner.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_cleaner.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_cleaner.h` & `z3-solver-4.9.1.0/core/src/sat/sat_cleaner.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_config.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_config.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_config.h` & `z3-solver-4.9.1.0/core/src/sat/sat_config.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_cut_simplifier.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_cut_simplifier.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_cut_simplifier.h` & `z3-solver-4.9.1.0/core/src/sat/sat_cut_simplifier.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_cutset.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_cutset.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_cutset.h` & `z3-solver-4.9.1.0/core/src/sat/sat_cutset.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_cutset_compute_shift.h` & `z3-solver-4.9.1.0/core/src/sat/sat_cutset_compute_shift.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_ddfw.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_ddfw.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_ddfw.h` & `z3-solver-4.9.1.0/core/src/sat/sat_ddfw.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_drat.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_drat.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_drat.h` & `z3-solver-4.9.1.0/core/src/sat/sat_drat.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_elim_eqs.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_elim_eqs.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_elim_eqs.h` & `z3-solver-4.9.1.0/core/src/sat/sat_elim_eqs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_elim_vars.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_elim_vars.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_elim_vars.h` & `z3-solver-4.9.1.0/core/src/sat/sat_elim_vars.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_extension.h` & `z3-solver-4.9.1.0/core/src/sat/sat_extension.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_gc.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_gc.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_integrity_checker.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_integrity_checker.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_integrity_checker.h` & `z3-solver-4.9.1.0/core/src/sat/sat_integrity_checker.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_justification.h` & `z3-solver-4.9.1.0/core/src/sat/sat_justification.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_local_search.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_local_search.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_local_search.h` & `z3-solver-4.9.1.0/core/src/sat/sat_local_search.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_lookahead.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_lookahead.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_lookahead.h` & `z3-solver-4.9.1.0/core/src/sat/sat_lookahead.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_lut_finder.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_lut_finder.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_lut_finder.h` & `z3-solver-4.9.1.0/core/src/sat/sat_lut_finder.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_model_converter.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_model_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_model_converter.h` & `z3-solver-4.9.1.0/core/src/sat/sat_model_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_mus.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_mus.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_mus.h` & `z3-solver-4.9.1.0/core/src/sat/sat_mus.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_npn3_finder.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_npn3_finder.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_npn3_finder.h` & `z3-solver-4.9.1.0/core/src/sat/sat_npn3_finder.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_parallel.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_parallel.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_parallel.h` & `z3-solver-4.9.1.0/core/src/sat/sat_parallel.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_params.pyg` & `z3-solver-4.9.1.0/core/src/sat/sat_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_prob.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_prob.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_prob.h` & `z3-solver-4.9.1.0/core/src/sat/sat_prob.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_probing.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_probing.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_probing.h` & `z3-solver-4.9.1.0/core/src/sat/sat_probing.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_scc.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_scc.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_scc.h` & `z3-solver-4.9.1.0/core/src/sat/sat_scc.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_simplifier.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_simplifier.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_simplifier.h` & `z3-solver-4.9.1.0/core/src/sat/sat_simplifier.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_simplifier_params.pyg` & `z3-solver-4.9.1.0/core/src/sat/sat_simplifier_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_solver/inc_sat_solver.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_solver/inc_sat_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_solver/inc_sat_solver.h` & `z3-solver-4.9.1.0/core/src/sat/sat_solver/inc_sat_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_solver.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_solver.h` & `z3-solver-4.9.1.0/core/src/sat/sat_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_solver_core.h` & `z3-solver-4.9.1.0/core/src/sat/sat_solver_core.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_types.h` & `z3-solver-4.9.1.0/core/src/sat/sat_types.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_watched.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_watched.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_watched.h` & `z3-solver-4.9.1.0/core/src/sat/sat_watched.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_xor_finder.cpp` & `z3-solver-4.9.1.0/core/src/sat/sat_xor_finder.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/sat_xor_finder.h` & `z3-solver-4.9.1.0/core/src/sat/sat_xor_finder.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/sat/smt/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/arith_axioms.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/arith_axioms.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/arith_diagnostics.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/arith_diagnostics.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/arith_internalize.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/arith_internalize.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/arith_proof_checker.h` & `z3-solver-4.9.1.0/core/src/sat/smt/arith_proof_checker.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/arith_solver.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/arith_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/arith_solver.h` & `z3-solver-4.9.1.0/core/src/sat/smt/arith_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/array_axioms.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/array_axioms.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/array_diagnostics.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/array_diagnostics.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/array_internalize.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/array_internalize.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/array_model.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/array_model.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/array_solver.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/array_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/array_solver.h` & `z3-solver-4.9.1.0/core/src/sat/smt/array_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/atom2bool_var.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/atom2bool_var.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/atom2bool_var.h` & `z3-solver-4.9.1.0/core/src/sat/smt/atom2bool_var.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/ba_xor.h` & `z3-solver-4.9.1.0/core/src/sat/smt/ba_xor.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/bv_ackerman.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/bv_ackerman.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/bv_ackerman.h` & `z3-solver-4.9.1.0/core/src/sat/smt/bv_ackerman.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/bv_delay_internalize.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/bv_delay_internalize.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/bv_internalize.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/bv_internalize.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/bv_invariant.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/bv_invariant.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/bv_solver.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/bv_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/bv_solver.h` & `z3-solver-4.9.1.0/core/src/sat/smt/bv_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/dt_solver.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/dt_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/dt_solver.h` & `z3-solver-4.9.1.0/core/src/sat/smt/dt_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/euf_ackerman.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/euf_ackerman.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/euf_ackerman.h` & `z3-solver-4.9.1.0/core/src/sat/smt/euf_ackerman.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/euf_internalize.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/euf_internalize.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/euf_invariant.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/euf_invariant.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/euf_model.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/euf_model.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/euf_proof.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/euf_proof.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/euf_relevancy.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/euf_relevancy.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/euf_relevancy.h` & `z3-solver-4.9.1.0/core/src/sat/smt/euf_relevancy.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/euf_solver.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/euf_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/euf_solver.h` & `z3-solver-4.9.1.0/core/src/sat/smt/euf_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/fpa_solver.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/fpa_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/fpa_solver.h` & `z3-solver-4.9.1.0/core/src/sat/smt/fpa_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/pb_card.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/pb_card.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/pb_card.h` & `z3-solver-4.9.1.0/core/src/sat/smt/pb_card.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/pb_constraint.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/pb_constraint.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/pb_constraint.h` & `z3-solver-4.9.1.0/core/src/sat/smt/pb_constraint.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/pb_internalize.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/pb_internalize.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/pb_pb.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/pb_pb.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/pb_pb.h` & `z3-solver-4.9.1.0/core/src/sat/smt/pb_pb.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/pb_solver.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/pb_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/pb_solver.h` & `z3-solver-4.9.1.0/core/src/sat/smt/pb_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/pb_solver_interface.h` & `z3-solver-4.9.1.0/core/src/sat/smt/pb_solver_interface.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_clause.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/q_clause.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_clause.h` & `z3-solver-4.9.1.0/core/src/sat/smt/q_clause.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_ematch.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/q_ematch.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_ematch.h` & `z3-solver-4.9.1.0/core/src/sat/smt/q_ematch.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_eval.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/q_eval.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_eval.h` & `z3-solver-4.9.1.0/core/src/sat/smt/q_eval.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_mam.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/q_mam.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_mam.h` & `z3-solver-4.9.1.0/core/src/sat/smt/q_mam.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_mbi.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/q_mbi.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_mbi.h` & `z3-solver-4.9.1.0/core/src/sat/smt/q_mbi.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_model_fixer.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/q_model_fixer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_model_fixer.h` & `z3-solver-4.9.1.0/core/src/sat/smt/q_model_fixer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_queue.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/q_queue.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_queue.h` & `z3-solver-4.9.1.0/core/src/sat/smt/q_queue.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_solver.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/q_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/q_solver.h` & `z3-solver-4.9.1.0/core/src/sat/smt/q_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/recfun_solver.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/recfun_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/recfun_solver.h` & `z3-solver-4.9.1.0/core/src/sat/smt/recfun_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/sat_internalizer.h` & `z3-solver-4.9.1.0/core/src/sat/smt/sat_internalizer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/sat_smt.h` & `z3-solver-4.9.1.0/core/src/sat/smt/sat_smt.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/sat_th.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/sat_th.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/sat_th.h` & `z3-solver-4.9.1.0/core/src/sat/smt/sat_th.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/user_solver.cpp` & `z3-solver-4.9.1.0/core/src/sat/smt/user_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/user_solver.h` & `z3-solver-4.9.1.0/core/src/sat/smt/user_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/smt/xor_solver.d` & `z3-solver-4.9.1.0/core/src/sat/smt/xor_solver.d`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/tactic/goal2sat.cpp` & `z3-solver-4.9.1.0/core/src/sat/tactic/goal2sat.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/tactic/goal2sat.h` & `z3-solver-4.9.1.0/core/src/sat/tactic/goal2sat.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/tactic/sat2goal.cpp` & `z3-solver-4.9.1.0/core/src/sat/tactic/sat2goal.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/tactic/sat2goal.h` & `z3-solver-4.9.1.0/core/src/sat/tactic/sat2goal.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/tactic/sat_tactic.cpp` & `z3-solver-4.9.1.0/core/src/sat/tactic/sat_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/sat/tactic/sat_tactic.h` & `z3-solver-4.9.1.0/core/src/sat/tactic/sat_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/shell/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/shell/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/shell/datalog_frontend.cpp` & `z3-solver-4.9.1.0/core/src/shell/datalog_frontend.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/shell/dimacs_frontend.cpp` & `z3-solver-4.9.1.0/core/src/shell/dimacs_frontend.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/shell/drat_frontend.cpp` & `z3-solver-4.9.1.0/core/src/shell/drat_frontend.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/shell/lp_frontend.cpp` & `z3-solver-4.9.1.0/core/src/shell/lp_frontend.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/shell/main.cpp` & `z3-solver-4.9.1.0/core/src/shell/main.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/shell/opt_frontend.cpp` & `z3-solver-4.9.1.0/core/src/shell/opt_frontend.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/shell/options.h` & `z3-solver-4.9.1.0/core/src/shell/options.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/shell/smtlib_frontend.cpp` & `z3-solver-4.9.1.0/core/src/shell/smtlib_frontend.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/shell/z3_log_frontend.cpp` & `z3-solver-4.9.1.0/core/src/shell/z3_log_frontend.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/smt/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/arith_eq_adapter.cpp` & `z3-solver-4.9.1.0/core/src/smt/arith_eq_adapter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/arith_eq_adapter.h` & `z3-solver-4.9.1.0/core/src/smt/arith_eq_adapter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/arith_eq_solver.cpp` & `z3-solver-4.9.1.0/core/src/smt/arith_eq_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/arith_eq_solver.h` & `z3-solver-4.9.1.0/core/src/smt/arith_eq_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/database.h` & `z3-solver-4.9.1.0/core/src/smt/database.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/database.smt` & `z3-solver-4.9.1.0/core/src/smt/database.smt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/diff_logic.h` & `z3-solver-4.9.1.0/core/src/smt/diff_logic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/dyn_ack.cpp` & `z3-solver-4.9.1.0/core/src/smt/dyn_ack.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/dyn_ack.h` & `z3-solver-4.9.1.0/core/src/smt/dyn_ack.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/expr_context_simplifier.cpp` & `z3-solver-4.9.1.0/core/src/smt/expr_context_simplifier.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/expr_context_simplifier.h` & `z3-solver-4.9.1.0/core/src/smt/expr_context_simplifier.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/fingerprints.cpp` & `z3-solver-4.9.1.0/core/src/smt/fingerprints.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/fingerprints.h` & `z3-solver-4.9.1.0/core/src/smt/fingerprints.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/mam.cpp` & `z3-solver-4.9.1.0/core/src/smt/mam.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/mam.h` & `z3-solver-4.9.1.0/core/src/smt/mam.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/old_interval.cpp` & `z3-solver-4.9.1.0/core/src/smt/old_interval.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/old_interval.h` & `z3-solver-4.9.1.0/core/src/smt/old_interval.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/dyn_ack_params.cpp` & `z3-solver-4.9.1.0/core/src/smt/params/dyn_ack_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/dyn_ack_params.h` & `z3-solver-4.9.1.0/core/src/smt/params/dyn_ack_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/preprocessor_params.cpp` & `z3-solver-4.9.1.0/core/src/smt/params/preprocessor_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/preprocessor_params.h` & `z3-solver-4.9.1.0/core/src/smt/params/preprocessor_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/qi_params.cpp` & `z3-solver-4.9.1.0/core/src/smt/params/qi_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/qi_params.h` & `z3-solver-4.9.1.0/core/src/smt/params/qi_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/smt_params.cpp` & `z3-solver-4.9.1.0/core/src/smt/params/smt_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/smt_params.h` & `z3-solver-4.9.1.0/core/src/smt/params/smt_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/smt_params_helper.pyg` & `z3-solver-4.9.1.0/core/src/smt/params/smt_params_helper.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/theory_arith_params.cpp` & `z3-solver-4.9.1.0/core/src/smt/params/theory_arith_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/theory_arith_params.h` & `z3-solver-4.9.1.0/core/src/smt/params/theory_arith_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/theory_array_params.cpp` & `z3-solver-4.9.1.0/core/src/smt/params/theory_array_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/theory_array_params.h` & `z3-solver-4.9.1.0/core/src/smt/params/theory_array_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/theory_bv_params.cpp` & `z3-solver-4.9.1.0/core/src/smt/params/theory_bv_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/theory_bv_params.h` & `z3-solver-4.9.1.0/core/src/smt/params/theory_bv_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/theory_datatype_params.h` & `z3-solver-4.9.1.0/core/src/smt/params/theory_datatype_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/theory_pb_params.cpp` & `z3-solver-4.9.1.0/core/src/smt/params/theory_pb_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/theory_pb_params.h` & `z3-solver-4.9.1.0/core/src/smt/params/theory_pb_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/theory_str_params.cpp` & `z3-solver-4.9.1.0/core/src/smt/params/theory_str_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/params/theory_str_params.h` & `z3-solver-4.9.1.0/core/src/smt/params/theory_str_params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/proto_model/proto_model.cpp` & `z3-solver-4.9.1.0/core/src/smt/proto_model/proto_model.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/proto_model/proto_model.h` & `z3-solver-4.9.1.0/core/src/smt/proto_model/proto_model.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/qi_queue.cpp` & `z3-solver-4.9.1.0/core/src/smt/qi_queue.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/qi_queue.h` & `z3-solver-4.9.1.0/core/src/smt/qi_queue.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/seq_axioms.cpp` & `z3-solver-4.9.1.0/core/src/smt/seq_axioms.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/seq_axioms.h` & `z3-solver-4.9.1.0/core/src/smt/seq_axioms.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/seq_eq_solver.cpp` & `z3-solver-4.9.1.0/core/src/smt/seq_eq_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/seq_ne_solver.cpp` & `z3-solver-4.9.1.0/core/src/smt/seq_ne_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/seq_offset_eq.cpp` & `z3-solver-4.9.1.0/core/src/smt/seq_offset_eq.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/seq_offset_eq.h` & `z3-solver-4.9.1.0/core/src/smt/seq_offset_eq.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/seq_regex.cpp` & `z3-solver-4.9.1.0/core/src/smt/seq_regex.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/seq_regex.h` & `z3-solver-4.9.1.0/core/src/smt/seq_regex.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt2_extra_cmds.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt2_extra_cmds.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_almost_cg_table.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_almost_cg_table.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_almost_cg_table.h` & `z3-solver-4.9.1.0/core/src/smt/smt_almost_cg_table.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_arith_value.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_arith_value.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_arith_value.h` & `z3-solver-4.9.1.0/core/src/smt/smt_arith_value.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_b_justification.h` & `z3-solver-4.9.1.0/core/src/smt/smt_b_justification.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_bool_var_data.h` & `z3-solver-4.9.1.0/core/src/smt/smt_bool_var_data.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_case_split_queue.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_case_split_queue.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_case_split_queue.h` & `z3-solver-4.9.1.0/core/src/smt/smt_case_split_queue.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_cg_table.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_cg_table.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_cg_table.h` & `z3-solver-4.9.1.0/core/src/smt/smt_cg_table.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_checker.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_checker.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_checker.h` & `z3-solver-4.9.1.0/core/src/smt/smt_checker.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_clause.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_clause.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_clause.h` & `z3-solver-4.9.1.0/core/src/smt/smt_clause.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_clause_proof.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_clause_proof.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_clause_proof.h` & `z3-solver-4.9.1.0/core/src/smt/smt_clause_proof.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_conflict_resolution.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_conflict_resolution.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_conflict_resolution.h` & `z3-solver-4.9.1.0/core/src/smt/smt_conflict_resolution.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_consequences.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_consequences.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_context.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_context.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_context.h` & `z3-solver-4.9.1.0/core/src/smt/smt_context.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_context_inv.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_context_inv.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_context_pp.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_context_pp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_context_stat.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_context_stat.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_enode.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_enode.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_enode.h` & `z3-solver-4.9.1.0/core/src/smt/smt_enode.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_eq_justification.h` & `z3-solver-4.9.1.0/core/src/smt/smt_eq_justification.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_failure.h` & `z3-solver-4.9.1.0/core/src/smt/smt_failure.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_farkas_util.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_farkas_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_farkas_util.h` & `z3-solver-4.9.1.0/core/src/smt/smt_farkas_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_for_each_relevant_expr.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_for_each_relevant_expr.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_for_each_relevant_expr.h` & `z3-solver-4.9.1.0/core/src/smt/smt_for_each_relevant_expr.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_implied_equalities.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_implied_equalities.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_implied_equalities.h` & `z3-solver-4.9.1.0/core/src/smt/smt_implied_equalities.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_induction.cpp.disabled` & `z3-solver-4.9.1.0/core/src/smt/smt_induction.cpp.disabled`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_induction.h.disabled` & `z3-solver-4.9.1.0/core/src/smt/smt_induction.h.disabled`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_internalizer.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_internalizer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_justification.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_justification.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_justification.h` & `z3-solver-4.9.1.0/core/src/smt/smt_justification.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_kernel.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_kernel.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_kernel.h` & `z3-solver-4.9.1.0/core/src/smt/smt_kernel.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_literal.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_literal.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_literal.h` & `z3-solver-4.9.1.0/core/src/smt/smt_literal.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_lookahead.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_lookahead.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_lookahead.h` & `z3-solver-4.9.1.0/core/src/smt/smt_lookahead.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_model_checker.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_model_checker.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_model_checker.h` & `z3-solver-4.9.1.0/core/src/smt/smt_model_checker.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_model_finder.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_model_finder.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_model_finder.h` & `z3-solver-4.9.1.0/core/src/smt/smt_model_finder.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_model_generator.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_model_generator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_model_generator.h` & `z3-solver-4.9.1.0/core/src/smt/smt_model_generator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_parallel.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_parallel.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_quantifier.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_quantifier.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_quantifier.h` & `z3-solver-4.9.1.0/core/src/smt/smt_quantifier.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_quantifier_instances.h` & `z3-solver-4.9.1.0/core/src/smt/smt_quantifier_instances.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_quick_checker.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_quick_checker.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_quick_checker.h` & `z3-solver-4.9.1.0/core/src/smt/smt_quick_checker.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_relevancy.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_relevancy.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_relevancy.h` & `z3-solver-4.9.1.0/core/src/smt/smt_relevancy.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_setup.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_setup.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_setup.h` & `z3-solver-4.9.1.0/core/src/smt/smt_setup.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_solver.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_solver.h` & `z3-solver-4.9.1.0/core/src/smt/smt_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_statistics.h` & `z3-solver-4.9.1.0/core/src/smt/smt_statistics.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_theory.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_theory.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_theory.h` & `z3-solver-4.9.1.0/core/src/smt/smt_theory.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_types.h` & `z3-solver-4.9.1.0/core/src/smt/smt_types.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/smt_value_sort.cpp` & `z3-solver-4.9.1.0/core/src/smt/smt_value_sort.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/spanning_tree.h` & `z3-solver-4.9.1.0/core/src/smt/spanning_tree.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/spanning_tree_base.h` & `z3-solver-4.9.1.0/core/src/smt/spanning_tree_base.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/spanning_tree_def.h` & `z3-solver-4.9.1.0/core/src/smt/spanning_tree_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/tactic/ctx_solver_simplify_tactic.cpp` & `z3-solver-4.9.1.0/core/src/smt/tactic/ctx_solver_simplify_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/tactic/smt_tactic_core.cpp` & `z3-solver-4.9.1.0/core/src/smt/tactic/smt_tactic_core.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/tactic/smt_tactic_core.h` & `z3-solver-4.9.1.0/core/src/smt/tactic/smt_tactic_core.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/tactic/unit_subsumption_tactic.cpp` & `z3-solver-4.9.1.0/core/src/smt/tactic/unit_subsumption_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/tactic/unit_subsumption_tactic.h` & `z3-solver-4.9.1.0/core/src/smt/tactic/unit_subsumption_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_arith.h` & `z3-solver-4.9.1.0/core/src/smt/theory_arith.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_arith_aux.h` & `z3-solver-4.9.1.0/core/src/smt/theory_arith_aux.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_arith_core.h` & `z3-solver-4.9.1.0/core/src/smt/theory_arith_core.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_arith_eq.h` & `z3-solver-4.9.1.0/core/src/smt/theory_arith_eq.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_arith_int.h` & `z3-solver-4.9.1.0/core/src/smt/theory_arith_int.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_arith_inv.h` & `z3-solver-4.9.1.0/core/src/smt/theory_arith_inv.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_arith_nl.h` & `z3-solver-4.9.1.0/core/src/smt/theory_arith_nl.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_arith_pp.h` & `z3-solver-4.9.1.0/core/src/smt/theory_arith_pp.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_array.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_array.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_array.h` & `z3-solver-4.9.1.0/core/src/smt/theory_array.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_array_bapa.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_array_bapa.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_array_bapa.h` & `z3-solver-4.9.1.0/core/src/smt/theory_array_bapa.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_array_base.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_array_base.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_array_base.h` & `z3-solver-4.9.1.0/core/src/smt/theory_array_base.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_array_full.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_array_full.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_array_full.h` & `z3-solver-4.9.1.0/core/src/smt/theory_array_full.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_bv.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_bv.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_bv.h` & `z3-solver-4.9.1.0/core/src/smt/theory_bv.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_char.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_char.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_char.h` & `z3-solver-4.9.1.0/core/src/smt/theory_char.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_datatype.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_datatype.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_datatype.h` & `z3-solver-4.9.1.0/core/src/smt/theory_datatype.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_dense_diff_logic.h` & `z3-solver-4.9.1.0/core/src/smt/theory_dense_diff_logic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_dense_diff_logic_def.h` & `z3-solver-4.9.1.0/core/src/smt/theory_dense_diff_logic_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_diff_logic.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_diff_logic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_diff_logic.h` & `z3-solver-4.9.1.0/core/src/smt/theory_diff_logic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_diff_logic_def.h` & `z3-solver-4.9.1.0/core/src/smt/theory_diff_logic_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_dl.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_dl.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_dummy.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_dummy.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_dummy.h` & `z3-solver-4.9.1.0/core/src/smt/theory_dummy.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_fpa.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_fpa.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_fpa.h` & `z3-solver-4.9.1.0/core/src/smt/theory_fpa.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_lra.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_lra.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_lra.h` & `z3-solver-4.9.1.0/core/src/smt/theory_lra.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_opt.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_opt.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_opt.h` & `z3-solver-4.9.1.0/core/src/smt/theory_opt.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_pb.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_pb.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_pb.h` & `z3-solver-4.9.1.0/core/src/smt/theory_pb.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_recfun.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_recfun.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_recfun.h` & `z3-solver-4.9.1.0/core/src/smt/theory_recfun.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_seq.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_seq.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_seq.h` & `z3-solver-4.9.1.0/core/src/smt/theory_seq.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_seq_empty.h` & `z3-solver-4.9.1.0/core/src/smt/theory_seq_empty.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_special_relations.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_special_relations.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_special_relations.h` & `z3-solver-4.9.1.0/core/src/smt/theory_special_relations.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_str.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_str.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_str.h` & `z3-solver-4.9.1.0/core/src/smt/theory_str.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_str_mc.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_str_mc.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_str_regex.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_str_regex.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_user_propagator.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_user_propagator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_user_propagator.h` & `z3-solver-4.9.1.0/core/src/smt/theory_user_propagator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_utvpi.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_utvpi.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_utvpi.h` & `z3-solver-4.9.1.0/core/src/smt/theory_utvpi.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_utvpi_def.h` & `z3-solver-4.9.1.0/core/src/smt/theory_utvpi_def.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_wmaxsat.cpp` & `z3-solver-4.9.1.0/core/src/smt/theory_wmaxsat.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/theory_wmaxsat.h` & `z3-solver-4.9.1.0/core/src/smt/theory_wmaxsat.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/uses_theory.cpp` & `z3-solver-4.9.1.0/core/src/smt/uses_theory.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/uses_theory.h` & `z3-solver-4.9.1.0/core/src/smt/uses_theory.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/watch_list.cpp` & `z3-solver-4.9.1.0/core/src/smt/watch_list.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/smt/watch_list.h` & `z3-solver-4.9.1.0/core/src/smt/watch_list.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/assertions/asserted_formulas.cpp` & `z3-solver-4.9.1.0/core/src/solver/assertions/asserted_formulas.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/assertions/asserted_formulas.h` & `z3-solver-4.9.1.0/core/src/solver/assertions/asserted_formulas.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/check_logic.cpp` & `z3-solver-4.9.1.0/core/src/solver/check_logic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/check_logic.h` & `z3-solver-4.9.1.0/core/src/solver/check_logic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/check_sat_result.cpp` & `z3-solver-4.9.1.0/core/src/solver/check_sat_result.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/check_sat_result.h` & `z3-solver-4.9.1.0/core/src/solver/check_sat_result.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/combined_solver.cpp` & `z3-solver-4.9.1.0/core/src/solver/combined_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/combined_solver.h` & `z3-solver-4.9.1.0/core/src/solver/combined_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/combined_solver_params.pyg` & `z3-solver-4.9.1.0/core/src/solver/combined_solver_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/mus.cpp` & `z3-solver-4.9.1.0/core/src/solver/mus.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/mus.h` & `z3-solver-4.9.1.0/core/src/solver/mus.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/parallel_params.pyg` & `z3-solver-4.9.1.0/core/src/solver/parallel_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/parallel_tactic.cpp` & `z3-solver-4.9.1.0/core/src/solver/parallel_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/smt_logics.cpp` & `z3-solver-4.9.1.0/core/src/solver/smt_logics.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/smt_logics.h` & `z3-solver-4.9.1.0/core/src/solver/smt_logics.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/solver.cpp` & `z3-solver-4.9.1.0/core/src/solver/solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/solver.h` & `z3-solver-4.9.1.0/core/src/solver/solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/solver2tactic.cpp` & `z3-solver-4.9.1.0/core/src/solver/solver2tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/solver2tactic.h` & `z3-solver-4.9.1.0/core/src/solver/solver2tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/solver_na2as.cpp` & `z3-solver-4.9.1.0/core/src/solver/solver_na2as.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/solver_na2as.h` & `z3-solver-4.9.1.0/core/src/solver/solver_na2as.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/solver_pool.cpp` & `z3-solver-4.9.1.0/core/src/solver/solver_pool.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/solver_pool.h` & `z3-solver-4.9.1.0/core/src/solver/solver_pool.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/tactic2solver.cpp` & `z3-solver-4.9.1.0/core/src/solver/tactic2solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/solver/tactic2solver.h` & `z3-solver-4.9.1.0/core/src/solver/tactic2solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/aig/aig.cpp` & `z3-solver-4.9.1.0/core/src/tactic/aig/aig.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/aig/aig.h` & `z3-solver-4.9.1.0/core/src/tactic/aig/aig.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/aig/aig_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/aig/aig_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/tactic/arith/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/add_bounds_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/add_bounds_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/add_bounds_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/add_bounds_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/arith_bounds_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/arith_bounds_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/arith_bounds_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/arith_bounds_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/bound_manager.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/bound_manager.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/bound_manager.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/bound_manager.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/bound_propagator.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/bound_propagator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/bound_propagator.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/bound_propagator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/bv2int_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/bv2int_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/bv2int_rewriter.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/bv2int_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/bv2real_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/bv2real_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/bv2real_rewriter.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/bv2real_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/card2bv_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/card2bv_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/card2bv_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/card2bv_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/degree_shift_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/degree_shift_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/degree_shift_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/degree_shift_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/diff_neq_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/diff_neq_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/diff_neq_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/diff_neq_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/eq2bv_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/eq2bv_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/eq2bv_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/eq2bv_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/factor_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/factor_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/fix_dl_var_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/fix_dl_var_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/fix_dl_var_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/fix_dl_var_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/fm_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/fm_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/fm_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/fm_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/lia2card_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/lia2card_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/lia2card_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/lia2card_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/lia2pb_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/lia2pb_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/linear_equation.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/linear_equation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/linear_equation.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/linear_equation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/nla2bv_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/nla2bv_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/nla2bv_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/nla2bv_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/normalize_bounds_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/normalize_bounds_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/normalize_bounds_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/normalize_bounds_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/pb2bv_model_converter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/pb2bv_model_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/pb2bv_model_converter.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/pb2bv_model_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/pb2bv_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/pb2bv_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/pb2bv_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/pb2bv_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/probe_arith.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/probe_arith.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/probe_arith.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/probe_arith.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/propagate_ineqs_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/propagate_ineqs_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/propagate_ineqs_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/propagate_ineqs_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/purify_arith_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/purify_arith_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/purify_arith_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/purify_arith_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/recover_01_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/arith/recover_01_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/arith/recover_01_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/arith/recover_01_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/tactic/bv/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bit_blaster_model_converter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/bv/bit_blaster_model_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bit_blaster_model_converter.h` & `z3-solver-4.9.1.0/core/src/tactic/bv/bit_blaster_model_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bit_blaster_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/bv/bit_blaster_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bit_blaster_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/bv/bit_blaster_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bv1_blaster_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/bv/bv1_blaster_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bv1_blaster_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/bv/bv1_blaster_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bv_bound_chk_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/bv/bv_bound_chk_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bv_bounds_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/bv/bv_bounds_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bv_bounds_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/bv/bv_bounds_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bv_size_reduction_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/bv/bv_size_reduction_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bv_size_reduction_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/bv/bv_size_reduction_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bvarray2uf_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/bv/bvarray2uf_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bvarray2uf_rewriter.h` & `z3-solver-4.9.1.0/core/src/tactic/bv/bvarray2uf_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bvarray2uf_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/bv/bvarray2uf_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/bvarray2uf_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/bv/bvarray2uf_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/dt2bv_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/bv/dt2bv_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/elim_small_bv_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/bv/elim_small_bv_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/max_bv_sharing_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/bv/max_bv_sharing_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/bv/max_bv_sharing_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/bv/max_bv_sharing_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/converter.h` & `z3-solver-4.9.1.0/core/src/tactic/converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/tactic/core/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/blast_term_ite_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/blast_term_ite_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/blast_term_ite_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/blast_term_ite_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/cofactor_elim_term_ite.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/cofactor_elim_term_ite.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/cofactor_elim_term_ite.h` & `z3-solver-4.9.1.0/core/src/tactic/core/cofactor_elim_term_ite.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/cofactor_term_ite_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/cofactor_term_ite_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/cofactor_term_ite_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/cofactor_term_ite_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/collect_occs.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/collect_occs.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/collect_occs.h` & `z3-solver-4.9.1.0/core/src/tactic/core/collect_occs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/collect_statistics_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/collect_statistics_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/collect_statistics_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/collect_statistics_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/ctx_simplify_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/ctx_simplify_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/ctx_simplify_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/ctx_simplify_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/der_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/der_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/distribute_forall_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/distribute_forall_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/dom_simplify_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/dom_simplify_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/dom_simplify_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/dom_simplify_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/elim_term_ite_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/elim_term_ite_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/elim_term_ite_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/elim_term_ite_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/elim_uncnstr_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/elim_uncnstr_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/elim_uncnstr_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/elim_uncnstr_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/injectivity_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/injectivity_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/nnf_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/nnf_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/nnf_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/nnf_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/occf_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/occf_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/occf_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/occf_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/pb_preprocess_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/pb_preprocess_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/pb_preprocess_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/pb_preprocess_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/propagate_values_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/propagate_values_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/propagate_values_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/propagate_values_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/reduce_args_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/reduce_args_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/reduce_args_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/reduce_args_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/reduce_invertible_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/reduce_invertible_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/reduce_invertible_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/reduce_invertible_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/simplify_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/simplify_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/simplify_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/simplify_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/solve_eqs_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/solve_eqs_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/solve_eqs_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/solve_eqs_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/special_relations_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/special_relations_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/special_relations_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/special_relations_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/split_clause_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/split_clause_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/split_clause_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/split_clause_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/symmetry_reduce_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/symmetry_reduce_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/tseitin_cnf_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/core/tseitin_cnf_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/core/tseitin_cnf_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/core/tseitin_cnf_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/dependency_converter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/dependency_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/dependency_converter.h` & `z3-solver-4.9.1.0/core/src/tactic/dependency_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/equiv_proof_converter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/equiv_proof_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/equiv_proof_converter.h` & `z3-solver-4.9.1.0/core/src/tactic/equiv_proof_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fd_solver/bounded_int2bv_solver.cpp` & `z3-solver-4.9.1.0/core/src/tactic/fd_solver/bounded_int2bv_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fd_solver/enum2bv_solver.cpp` & `z3-solver-4.9.1.0/core/src/tactic/fd_solver/enum2bv_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fd_solver/fd_solver.cpp` & `z3-solver-4.9.1.0/core/src/tactic/fd_solver/fd_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fd_solver/fd_solver.h` & `z3-solver-4.9.1.0/core/src/tactic/fd_solver/fd_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fd_solver/pb2bv_solver.cpp` & `z3-solver-4.9.1.0/core/src/tactic/fd_solver/pb2bv_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fd_solver/smtfd_solver.cpp` & `z3-solver-4.9.1.0/core/src/tactic/fd_solver/smtfd_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fd_solver/smtfd_solver.h` & `z3-solver-4.9.1.0/core/src/tactic/fd_solver/smtfd_solver.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/filter_model_converter.h` & `z3-solver-4.9.1.0/core/src/tactic/filter_model_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fpa/fpa2bv_model_converter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/fpa/fpa2bv_model_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fpa/fpa2bv_model_converter.h` & `z3-solver-4.9.1.0/core/src/tactic/fpa/fpa2bv_model_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fpa/fpa2bv_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/fpa/fpa2bv_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fpa/qffp_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/fpa/qffp_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fpa/qffp_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/fpa/qffp_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fpa/qffplra_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/fpa/qffplra_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/fpa/qffplra_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/fpa/qffplra_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/generic_model_converter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/generic_model_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/generic_model_converter.h` & `z3-solver-4.9.1.0/core/src/tactic/generic_model_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/goal.cpp` & `z3-solver-4.9.1.0/core/src/tactic/goal.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/goal.h` & `z3-solver-4.9.1.0/core/src/tactic/goal.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/goal_num_occurs.h` & `z3-solver-4.9.1.0/core/src/tactic/goal_num_occurs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/goal_shared_occs.cpp` & `z3-solver-4.9.1.0/core/src/tactic/goal_shared_occs.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/goal_shared_occs.h` & `z3-solver-4.9.1.0/core/src/tactic/goal_shared_occs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/goal_util.cpp` & `z3-solver-4.9.1.0/core/src/tactic/goal_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/horn_subsume_model_converter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/horn_subsume_model_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/horn_subsume_model_converter.h` & `z3-solver-4.9.1.0/core/src/tactic/horn_subsume_model_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/model_converter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/model_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/model_converter.h` & `z3-solver-4.9.1.0/core/src/tactic/model_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/portfolio/default_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/portfolio/default_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/portfolio/smt_strategic_solver.cpp` & `z3-solver-4.9.1.0/core/src/tactic/portfolio/smt_strategic_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/portfolio/solver_subsumption_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/portfolio/solver_subsumption_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/probe.cpp` & `z3-solver-4.9.1.0/core/src/tactic/probe.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/probe.h` & `z3-solver-4.9.1.0/core/src/tactic/probe.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/proof_converter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/proof_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/proof_converter.h` & `z3-solver-4.9.1.0/core/src/tactic/proof_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/replace_proof_converter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/replace_proof_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/replace_proof_converter.h` & `z3-solver-4.9.1.0/core/src/tactic/replace_proof_converter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/sls/bvsls_opt_engine.cpp` & `z3-solver-4.9.1.0/core/src/tactic/sls/bvsls_opt_engine.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/sls/bvsls_opt_engine.h` & `z3-solver-4.9.1.0/core/src/tactic/sls/bvsls_opt_engine.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/sls/sls_engine.cpp` & `z3-solver-4.9.1.0/core/src/tactic/sls/sls_engine.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/sls/sls_engine.h` & `z3-solver-4.9.1.0/core/src/tactic/sls/sls_engine.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/sls/sls_evaluator.h` & `z3-solver-4.9.1.0/core/src/tactic/sls/sls_evaluator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/sls/sls_params.pyg` & `z3-solver-4.9.1.0/core/src/tactic/sls/sls_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/sls/sls_powers.h` & `z3-solver-4.9.1.0/core/src/tactic/sls/sls_powers.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/sls/sls_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/sls/sls_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/sls/sls_tracker.h` & `z3-solver-4.9.1.0/core/src/tactic/sls/sls_tracker.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/nra_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/nra_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfaufbv_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfaufbv_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfauflia_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfauflia_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfbv_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfbv_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfbv_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfbv_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfidl_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfidl_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qflia_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qflia_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qflia_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qflia_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qflra_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qflra_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfnia_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfnia_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfnra_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfnra_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfuf_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfuf_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfufbv_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfufbv_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/qfufbv_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/qfufbv_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/quant_tactics.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/quant_tactics.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/quant_tactics.h` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/quant_tactics.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/smt_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/smt_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/smtlogics/smt_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/smtlogics/smt_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/tactic_exception.h` & `z3-solver-4.9.1.0/core/src/tactic/tactic_exception.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/tactic_params.pyg` & `z3-solver-4.9.1.0/core/src/tactic/tactic_params.pyg`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/tactical.cpp` & `z3-solver-4.9.1.0/core/src/tactic/tactical.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/tactical.h` & `z3-solver-4.9.1.0/core/src/tactic/tactical.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/ufbv/macro_finder_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/ufbv/macro_finder_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/ufbv/quasi_macros_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/ufbv/quasi_macros_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/ufbv/ufbv_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/tactic/ufbv/ufbv_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/ufbv/ufbv_rewriter.h` & `z3-solver-4.9.1.0/core/src/tactic/ufbv/ufbv_rewriter.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/ufbv/ufbv_rewriter_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/ufbv/ufbv_rewriter_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/ufbv/ufbv_tactic.cpp` & `z3-solver-4.9.1.0/core/src/tactic/ufbv/ufbv_tactic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/ufbv/ufbv_tactic.h` & `z3-solver-4.9.1.0/core/src/tactic/ufbv/ufbv_tactic.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/tactic/user_propagator_base.h` & `z3-solver-4.9.1.0/core/src/tactic/user_propagator_base.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/algebraic.cpp` & `z3-solver-4.9.1.0/core/src/test/algebraic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/api.cpp` & `z3-solver-4.9.1.0/core/src/test/api.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/api_bug.cpp` & `z3-solver-4.9.1.0/core/src/test/api_bug.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/arith_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/test/arith_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/arith_simplifier_plugin.cpp` & `z3-solver-4.9.1.0/core/src/test/arith_simplifier_plugin.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/ast.cpp` & `z3-solver-4.9.1.0/core/src/test/ast.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/bdd.cpp` & `z3-solver-4.9.1.0/core/src/test/bdd.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/bit_blaster.cpp` & `z3-solver-4.9.1.0/core/src/test/bit_blaster.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/bit_vector.cpp` & `z3-solver-4.9.1.0/core/src/test/bit_vector.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/bits.cpp` & `z3-solver-4.9.1.0/core/src/test/bits.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/buffer.cpp` & `z3-solver-4.9.1.0/core/src/test/buffer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/chashtable.cpp` & `z3-solver-4.9.1.0/core/src/test/chashtable.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/check_assumptions.cpp` & `z3-solver-4.9.1.0/core/src/test/check_assumptions.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/cnf_backbones.cpp` & `z3-solver-4.9.1.0/core/src/test/cnf_backbones.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/cube_clause.cpp` & `z3-solver-4.9.1.0/core/src/test/cube_clause.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/datalog_parser.cpp` & `z3-solver-4.9.1.0/core/src/test/datalog_parser.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/ddnf.cpp` & `z3-solver-4.9.1.0/core/src/test/ddnf.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/diff_logic.cpp` & `z3-solver-4.9.1.0/core/src/test/diff_logic.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/dl_context.cpp` & `z3-solver-4.9.1.0/core/src/test/dl_context.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/dl_product_relation.cpp` & `z3-solver-4.9.1.0/core/src/test/dl_product_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/dl_query.cpp` & `z3-solver-4.9.1.0/core/src/test/dl_query.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/dl_relation.cpp` & `z3-solver-4.9.1.0/core/src/test/dl_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/dl_table.cpp` & `z3-solver-4.9.1.0/core/src/test/dl_table.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/dl_util.cpp` & `z3-solver-4.9.1.0/core/src/test/dl_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/doc.cpp` & `z3-solver-4.9.1.0/core/src/test/doc.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/egraph.cpp` & `z3-solver-4.9.1.0/core/src/test/egraph.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/escaped.cpp` & `z3-solver-4.9.1.0/core/src/test/escaped.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/ex.cpp` & `z3-solver-4.9.1.0/core/src/test/ex.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/expr_rand.cpp` & `z3-solver-4.9.1.0/core/src/test/expr_rand.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/expr_substitution.cpp` & `z3-solver-4.9.1.0/core/src/test/expr_substitution.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/ext_numeral.cpp` & `z3-solver-4.9.1.0/core/src/test/ext_numeral.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/f2n.cpp` & `z3-solver-4.9.1.0/core/src/test/f2n.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/factor_rewriter.cpp` & `z3-solver-4.9.1.0/core/src/test/factor_rewriter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/finder.cpp` & `z3-solver-4.9.1.0/core/src/test/finder.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/fixed_bit_vector.cpp` & `z3-solver-4.9.1.0/core/src/test/fixed_bit_vector.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/for_each_file.cpp` & `z3-solver-4.9.1.0/core/src/test/for_each_file.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/fuzzing/expr_delta.cpp` & `z3-solver-4.9.1.0/core/src/test/fuzzing/expr_delta.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/fuzzing/expr_delta.h` & `z3-solver-4.9.1.0/core/src/test/fuzzing/expr_delta.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/fuzzing/expr_rand.cpp` & `z3-solver-4.9.1.0/core/src/test/fuzzing/expr_rand.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/fuzzing/expr_rand.h` & `z3-solver-4.9.1.0/core/src/test/fuzzing/expr_rand.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/get_consequences.cpp` & `z3-solver-4.9.1.0/core/src/test/get_consequences.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/get_implied_equalities.cpp` & `z3-solver-4.9.1.0/core/src/test/get_implied_equalities.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/hashtable.cpp` & `z3-solver-4.9.1.0/core/src/test/hashtable.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/heap.cpp` & `z3-solver-4.9.1.0/core/src/test/heap.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/heap_trie.cpp` & `z3-solver-4.9.1.0/core/src/test/heap_trie.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/hilbert_basis.cpp` & `z3-solver-4.9.1.0/core/src/test/hilbert_basis.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/horn_subsume_model_converter.cpp` & `z3-solver-4.9.1.0/core/src/test/horn_subsume_model_converter.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/hwf.cpp` & `z3-solver-4.9.1.0/core/src/test/hwf.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/im_float_config.h` & `z3-solver-4.9.1.0/core/src/test/im_float_config.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/inf_rational.cpp` & `z3-solver-4.9.1.0/core/src/test/inf_rational.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/interval.cpp` & `z3-solver-4.9.1.0/core/src/test/interval.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/karr.cpp` & `z3-solver-4.9.1.0/core/src/test/karr.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/list.cpp` & `z3-solver-4.9.1.0/core/src/test/list.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/lp/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/test/lp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/lp/argument_parser.h` & `z3-solver-4.9.1.0/core/src/test/lp/argument_parser.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/lp/gomory_test.h` & `z3-solver-4.9.1.0/core/src/test/lp/gomory_test.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/lp/lp.cpp` & `z3-solver-4.9.1.0/core/src/test/lp/lp.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/lp/nla_solver_test.cpp` & `z3-solver-4.9.1.0/core/src/test/lp/nla_solver_test.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/lp/smt_reader.h` & `z3-solver-4.9.1.0/core/src/test/lp/smt_reader.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/lp/test_file_reader.h` & `z3-solver-4.9.1.0/core/src/test/lp/test_file_reader.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/main.cpp` & `z3-solver-4.9.1.0/core/src/test/main.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/map.cpp` & `z3-solver-4.9.1.0/core/src/test/map.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/matcher.cpp` & `z3-solver-4.9.1.0/core/src/test/matcher.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/memory.cpp` & `z3-solver-4.9.1.0/core/src/test/memory.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/model2expr.cpp` & `z3-solver-4.9.1.0/core/src/test/model2expr.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/model_based_opt.cpp` & `z3-solver-4.9.1.0/core/src/test/model_based_opt.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/model_evaluator.cpp` & `z3-solver-4.9.1.0/core/src/test/model_evaluator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/model_retrieval.cpp` & `z3-solver-4.9.1.0/core/src/test/model_retrieval.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/mpbq.cpp` & `z3-solver-4.9.1.0/core/src/test/mpbq.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/mpf.cpp` & `z3-solver-4.9.1.0/core/src/test/mpf.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/mpff.cpp` & `z3-solver-4.9.1.0/core/src/test/mpff.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/mpfx.cpp` & `z3-solver-4.9.1.0/core/src/test/mpfx.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/mpq.cpp` & `z3-solver-4.9.1.0/core/src/test/mpq.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/mpz.cpp` & `z3-solver-4.9.1.0/core/src/test/mpz.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/nlarith_util.cpp` & `z3-solver-4.9.1.0/core/src/test/nlarith_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/nlsat.cpp` & `z3-solver-4.9.1.0/core/src/test/nlsat.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/no_overflow.cpp` & `z3-solver-4.9.1.0/core/src/test/no_overflow.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/object_allocator.cpp` & `z3-solver-4.9.1.0/core/src/test/object_allocator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/old_interval.cpp` & `z3-solver-4.9.1.0/core/src/test/old_interval.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/optional.cpp` & `z3-solver-4.9.1.0/core/src/test/optional.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/parray.cpp` & `z3-solver-4.9.1.0/core/src/test/parray.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/pb2bv.cpp` & `z3-solver-4.9.1.0/core/src/test/pb2bv.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/pdd.cpp` & `z3-solver-4.9.1.0/core/src/test/pdd.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/pdd_solver.cpp` & `z3-solver-4.9.1.0/core/src/test/pdd_solver.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/permutation.cpp` & `z3-solver-4.9.1.0/core/src/test/permutation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/polynomial.cpp` & `z3-solver-4.9.1.0/core/src/test/polynomial.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/polynorm.cpp` & `z3-solver-4.9.1.0/core/src/test/polynorm.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/prime_generator.cpp` & `z3-solver-4.9.1.0/core/src/test/prime_generator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/proof_checker.cpp` & `z3-solver-4.9.1.0/core/src/test/proof_checker.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/qe_arith.cpp` & `z3-solver-4.9.1.0/core/src/test/qe_arith.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/quant_elim.cpp` & `z3-solver-4.9.1.0/core/src/test/quant_elim.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/quant_solve.cpp` & `z3-solver-4.9.1.0/core/src/test/quant_solve.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/rational.cpp` & `z3-solver-4.9.1.0/core/src/test/rational.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/rcf.cpp` & `z3-solver-4.9.1.0/core/src/test/rcf.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/sat_local_search.cpp` & `z3-solver-4.9.1.0/core/src/test/sat_local_search.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/sat_lookahead.cpp` & `z3-solver-4.9.1.0/core/src/test/sat_lookahead.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/sat_user_scope.cpp` & `z3-solver-4.9.1.0/core/src/test/sat_user_scope.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/scoped_timer.cpp` & `z3-solver-4.9.1.0/core/src/test/scoped_timer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/simple_parser.cpp` & `z3-solver-4.9.1.0/core/src/test/simple_parser.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/simplex.cpp` & `z3-solver-4.9.1.0/core/src/test/simplex.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/simplifier.cpp` & `z3-solver-4.9.1.0/core/src/test/simplifier.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/small_object_allocator.cpp` & `z3-solver-4.9.1.0/core/src/test/small_object_allocator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/smt2print_parse.cpp` & `z3-solver-4.9.1.0/core/src/test/smt2print_parse.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/smt_context.cpp` & `z3-solver-4.9.1.0/core/src/test/smt_context.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/solver_pool.cpp` & `z3-solver-4.9.1.0/core/src/test/solver_pool.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/sorting_network.cpp` & `z3-solver-4.9.1.0/core/src/test/sorting_network.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/stack.cpp` & `z3-solver-4.9.1.0/core/src/test/stack.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/string_buffer.cpp` & `z3-solver-4.9.1.0/core/src/test/string_buffer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/substitution.cpp` & `z3-solver-4.9.1.0/core/src/test/substitution.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/symbol.cpp` & `z3-solver-4.9.1.0/core/src/test/symbol.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/symbol_table.cpp` & `z3-solver-4.9.1.0/core/src/test/symbol_table.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/tbv.cpp` & `z3-solver-4.9.1.0/core/src/test/tbv.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/test_util.h` & `z3-solver-4.9.1.0/core/src/test/test_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/theory_dl.cpp` & `z3-solver-4.9.1.0/core/src/test/theory_dl.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/theory_pb.cpp` & `z3-solver-4.9.1.0/core/src/test/theory_pb.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/total_order.cpp` & `z3-solver-4.9.1.0/core/src/test/total_order.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/totalizer.cpp` & `z3-solver-4.9.1.0/core/src/test/totalizer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/trigo.cpp` & `z3-solver-4.9.1.0/core/src/test/trigo.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/udoc_relation.cpp` & `z3-solver-4.9.1.0/core/src/test/udoc_relation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/uint_set.cpp` & `z3-solver-4.9.1.0/core/src/test/uint_set.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/upolynomial.cpp` & `z3-solver-4.9.1.0/core/src/test/upolynomial.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/value_generator.cpp` & `z3-solver-4.9.1.0/core/src/test/value_generator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/value_sweep.cpp` & `z3-solver-4.9.1.0/core/src/test/value_sweep.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/var_subst.cpp` & `z3-solver-4.9.1.0/core/src/test/var_subst.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/vector.cpp` & `z3-solver-4.9.1.0/core/src/test/vector.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/test/zstring.cpp` & `z3-solver-4.9.1.0/core/src/test/zstring.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/CMakeLists.txt` & `z3-solver-4.9.1.0/core/src/util/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/approx_nat.cpp` & `z3-solver-4.9.1.0/core/src/util/approx_nat.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/approx_nat.h` & `z3-solver-4.9.1.0/core/src/util/approx_nat.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/approx_set.cpp` & `z3-solver-4.9.1.0/core/src/util/approx_set.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/approx_set.h` & `z3-solver-4.9.1.0/core/src/util/approx_set.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/array.h` & `z3-solver-4.9.1.0/core/src/util/array.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/array_map.h` & `z3-solver-4.9.1.0/core/src/util/array_map.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/backtrackable_set.h` & `z3-solver-4.9.1.0/core/src/util/backtrackable_set.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/basic_interval.h` & `z3-solver-4.9.1.0/core/src/util/basic_interval.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/bit_util.cpp` & `z3-solver-4.9.1.0/core/src/util/bit_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/bit_util.h` & `z3-solver-4.9.1.0/core/src/util/bit_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/bit_vector.cpp` & `z3-solver-4.9.1.0/core/src/util/bit_vector.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/bit_vector.h` & `z3-solver-4.9.1.0/core/src/util/bit_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/buffer.h` & `z3-solver-4.9.1.0/core/src/util/buffer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/cancel_eh.h` & `z3-solver-4.9.1.0/core/src/util/cancel_eh.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/chashtable.h` & `z3-solver-4.9.1.0/core/src/util/chashtable.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/checked_int64.h` & `z3-solver-4.9.1.0/core/src/util/checked_int64.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/cmd_context_types.cpp` & `z3-solver-4.9.1.0/core/src/util/cmd_context_types.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/cmd_context_types.h` & `z3-solver-4.9.1.0/core/src/util/cmd_context_types.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/common_msgs.cpp` & `z3-solver-4.9.1.0/core/src/util/common_msgs.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/common_msgs.h` & `z3-solver-4.9.1.0/core/src/util/common_msgs.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/container_util.h` & `z3-solver-4.9.1.0/core/src/util/container_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/debug.cpp` & `z3-solver-4.9.1.0/core/src/util/debug.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/debug.h` & `z3-solver-4.9.1.0/core/src/util/debug.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/dec_ref_util.h` & `z3-solver-4.9.1.0/core/src/util/dec_ref_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/dependency.h` & `z3-solver-4.9.1.0/core/src/util/dependency.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/dlist.h` & `z3-solver-4.9.1.0/core/src/util/dlist.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/double_manager.h` & `z3-solver-4.9.1.0/core/src/util/double_manager.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/ema.h` & `z3-solver-4.9.1.0/core/src/util/ema.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/env_params.cpp` & `z3-solver-4.9.1.0/core/src/util/env_params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/error_codes.h` & `z3-solver-4.9.1.0/core/src/util/error_codes.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/event_handler.h` & `z3-solver-4.9.1.0/core/src/util/event_handler.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/ext_gcd.h` & `z3-solver-4.9.1.0/core/src/util/ext_gcd.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/ext_numeral.h` & `z3-solver-4.9.1.0/core/src/util/ext_numeral.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/f2n.h` & `z3-solver-4.9.1.0/core/src/util/f2n.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/file_path.h` & `z3-solver-4.9.1.0/core/src/util/file_path.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/fixed_bit_vector.cpp` & `z3-solver-4.9.1.0/core/src/util/fixed_bit_vector.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/fixed_bit_vector.h` & `z3-solver-4.9.1.0/core/src/util/fixed_bit_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/gparams.cpp` & `z3-solver-4.9.1.0/core/src/util/gparams.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/gparams.h` & `z3-solver-4.9.1.0/core/src/util/gparams.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/hash.cpp` & `z3-solver-4.9.1.0/core/src/util/hash.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/hash.h` & `z3-solver-4.9.1.0/core/src/util/hash.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/hashtable.h` & `z3-solver-4.9.1.0/core/src/util/hashtable.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/heap.h` & `z3-solver-4.9.1.0/core/src/util/heap.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/hwf.cpp` & `z3-solver-4.9.1.0/core/src/util/hwf.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/hwf.h` & `z3-solver-4.9.1.0/core/src/util/hwf.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/id_gen.h` & `z3-solver-4.9.1.0/core/src/util/id_gen.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/id_var_list.h` & `z3-solver-4.9.1.0/core/src/util/id_var_list.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/inf_eps_rational.h` & `z3-solver-4.9.1.0/core/src/util/inf_eps_rational.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/inf_int_rational.cpp` & `z3-solver-4.9.1.0/core/src/util/inf_int_rational.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/inf_int_rational.h` & `z3-solver-4.9.1.0/core/src/util/inf_int_rational.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/inf_rational.cpp` & `z3-solver-4.9.1.0/core/src/util/inf_rational.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/inf_rational.h` & `z3-solver-4.9.1.0/core/src/util/inf_rational.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/inf_s_integer.h` & `z3-solver-4.9.1.0/core/src/util/inf_s_integer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/lbool.cpp` & `z3-solver-4.9.1.0/core/src/util/lbool.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/lbool.h` & `z3-solver-4.9.1.0/core/src/util/lbool.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/lim_vector.h` & `z3-solver-4.9.1.0/core/src/util/lim_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/list.h` & `z3-solver-4.9.1.0/core/src/util/list.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/luby.cpp` & `z3-solver-4.9.1.0/core/src/util/luby.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/map.h` & `z3-solver-4.9.1.0/core/src/util/map.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/max_cliques.h` & `z3-solver-4.9.1.0/core/src/util/max_cliques.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/memory_manager.cpp` & `z3-solver-4.9.1.0/core/src/util/memory_manager.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/memory_manager.h` & `z3-solver-4.9.1.0/core/src/util/memory_manager.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/min_cut.cpp` & `z3-solver-4.9.1.0/core/src/util/min_cut.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/min_cut.h` & `z3-solver-4.9.1.0/core/src/util/min_cut.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpbq.cpp` & `z3-solver-4.9.1.0/core/src/util/mpbq.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpbq.h` & `z3-solver-4.9.1.0/core/src/util/mpbq.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpbqi.h` & `z3-solver-4.9.1.0/core/src/util/mpbqi.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpf.cpp` & `z3-solver-4.9.1.0/core/src/util/mpf.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpf.h` & `z3-solver-4.9.1.0/core/src/util/mpf.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpff.cpp` & `z3-solver-4.9.1.0/core/src/util/mpff.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpff.h` & `z3-solver-4.9.1.0/core/src/util/mpff.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpfx.cpp` & `z3-solver-4.9.1.0/core/src/util/mpfx.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpfx.h` & `z3-solver-4.9.1.0/core/src/util/mpfx.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpn.cpp` & `z3-solver-4.9.1.0/core/src/util/mpn.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpn.h` & `z3-solver-4.9.1.0/core/src/util/mpn.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpq.cpp` & `z3-solver-4.9.1.0/core/src/util/mpq.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpq.h` & `z3-solver-4.9.1.0/core/src/util/mpq.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpq_inf.cpp` & `z3-solver-4.9.1.0/core/src/util/mpq_inf.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpq_inf.h` & `z3-solver-4.9.1.0/core/src/util/mpq_inf.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpz.cpp` & `z3-solver-4.9.1.0/core/src/util/mpz.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpz.h` & `z3-solver-4.9.1.0/core/src/util/mpz.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mpzzp.h` & `z3-solver-4.9.1.0/core/src/util/mpzzp.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/mutex.h` & `z3-solver-4.9.1.0/core/src/util/mutex.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/nat_set.h` & `z3-solver-4.9.1.0/core/src/util/nat_set.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/numeral_buffer.h` & `z3-solver-4.9.1.0/core/src/util/numeral_buffer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/obj_hashtable.h` & `z3-solver-4.9.1.0/core/src/util/obj_hashtable.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/obj_mark.h` & `z3-solver-4.9.1.0/core/src/util/obj_mark.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/obj_pair_hashtable.h` & `z3-solver-4.9.1.0/core/src/util/obj_pair_hashtable.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/obj_pair_set.h` & `z3-solver-4.9.1.0/core/src/util/obj_pair_set.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/obj_ref.h` & `z3-solver-4.9.1.0/core/src/util/obj_ref.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/obj_ref_hashtable.h` & `z3-solver-4.9.1.0/core/src/util/obj_ref_hashtable.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/obj_triple_hashtable.h` & `z3-solver-4.9.1.0/core/src/util/obj_triple_hashtable.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/object_allocator.h` & `z3-solver-4.9.1.0/core/src/util/object_allocator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/optional.h` & `z3-solver-4.9.1.0/core/src/util/optional.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/page.cpp` & `z3-solver-4.9.1.0/core/src/util/page.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/page.h` & `z3-solver-4.9.1.0/core/src/util/page.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/params.cpp` & `z3-solver-4.9.1.0/core/src/util/params.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/params.h` & `z3-solver-4.9.1.0/core/src/util/params.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/parray.h` & `z3-solver-4.9.1.0/core/src/util/parray.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/permutation.cpp` & `z3-solver-4.9.1.0/core/src/util/permutation.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/permutation.h` & `z3-solver-4.9.1.0/core/src/util/permutation.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/plugin_manager.h` & `z3-solver-4.9.1.0/core/src/util/plugin_manager.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/pool.h` & `z3-solver-4.9.1.0/core/src/util/pool.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/prime_generator.cpp` & `z3-solver-4.9.1.0/core/src/util/prime_generator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/prime_generator.h` & `z3-solver-4.9.1.0/core/src/util/prime_generator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/ptr_scoped_buffer.h` & `z3-solver-4.9.1.0/core/src/util/ptr_scoped_buffer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/queue.h` & `z3-solver-4.9.1.0/core/src/util/queue.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/rational.cpp` & `z3-solver-4.9.1.0/core/src/util/rational.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/rational.h` & `z3-solver-4.9.1.0/core/src/util/rational.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/ref.h` & `z3-solver-4.9.1.0/core/src/util/ref.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/ref_buffer.h` & `z3-solver-4.9.1.0/core/src/util/ref_buffer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/ref_pair_vector.h` & `z3-solver-4.9.1.0/core/src/util/ref_pair_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/ref_util.h` & `z3-solver-4.9.1.0/core/src/util/ref_util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/ref_vector.h` & `z3-solver-4.9.1.0/core/src/util/ref_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/region.cpp` & `z3-solver-4.9.1.0/core/src/util/region.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/region.h` & `z3-solver-4.9.1.0/core/src/util/region.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/rlimit.cpp` & `z3-solver-4.9.1.0/core/src/util/rlimit.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/rlimit.h` & `z3-solver-4.9.1.0/core/src/util/rlimit.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/s_integer.cpp` & `z3-solver-4.9.1.0/core/src/util/s_integer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/s_integer.h` & `z3-solver-4.9.1.0/core/src/util/s_integer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/sat_literal.h` & `z3-solver-4.9.1.0/core/src/util/sat_literal.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/scoped_ctrl_c.cpp` & `z3-solver-4.9.1.0/core/src/util/scoped_ctrl_c.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/scoped_ctrl_c.h` & `z3-solver-4.9.1.0/core/src/util/scoped_ctrl_c.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/scoped_limit_trail.h` & `z3-solver-4.9.1.0/core/src/util/scoped_limit_trail.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/scoped_numeral.h` & `z3-solver-4.9.1.0/core/src/util/scoped_numeral.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/scoped_numeral_buffer.h` & `z3-solver-4.9.1.0/core/src/util/scoped_numeral_buffer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/scoped_numeral_vector.h` & `z3-solver-4.9.1.0/core/src/util/scoped_numeral_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/scoped_ptr_vector.h` & `z3-solver-4.9.1.0/core/src/util/scoped_ptr_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/scoped_timer.cpp` & `z3-solver-4.9.1.0/core/src/util/scoped_timer.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/scoped_timer.h` & `z3-solver-4.9.1.0/core/src/util/scoped_timer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/scoped_vector.h` & `z3-solver-4.9.1.0/core/src/util/scoped_vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/sexpr.cpp` & `z3-solver-4.9.1.0/core/src/util/sexpr.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/sexpr.h` & `z3-solver-4.9.1.0/core/src/util/sexpr.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/sign.h` & `z3-solver-4.9.1.0/core/src/util/sign.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/small_object_allocator.cpp` & `z3-solver-4.9.1.0/core/src/util/small_object_allocator.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/small_object_allocator.h` & `z3-solver-4.9.1.0/core/src/util/small_object_allocator.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/smt2_util.cpp` & `z3-solver-4.9.1.0/core/src/util/smt2_util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/sorting_network.h` & `z3-solver-4.9.1.0/core/src/util/sorting_network.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/stack.cpp` & `z3-solver-4.9.1.0/core/src/util/stack.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/stack.h` & `z3-solver-4.9.1.0/core/src/util/stack.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/stacked_value.h` & `z3-solver-4.9.1.0/core/src/util/stacked_value.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/state_graph.cpp` & `z3-solver-4.9.1.0/core/src/util/state_graph.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/state_graph.h` & `z3-solver-4.9.1.0/core/src/util/state_graph.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/statistics.cpp` & `z3-solver-4.9.1.0/core/src/util/statistics.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/statistics.h` & `z3-solver-4.9.1.0/core/src/util/statistics.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/stopwatch.h` & `z3-solver-4.9.1.0/core/src/util/stopwatch.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/str_hashtable.h` & `z3-solver-4.9.1.0/core/src/util/str_hashtable.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/stream_buffer.h` & `z3-solver-4.9.1.0/core/src/util/stream_buffer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/string_buffer.h` & `z3-solver-4.9.1.0/core/src/util/string_buffer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/symbol.cpp` & `z3-solver-4.9.1.0/core/src/util/symbol.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/symbol.h` & `z3-solver-4.9.1.0/core/src/util/symbol.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/symbol_table.h` & `z3-solver-4.9.1.0/core/src/util/symbol_table.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/timeit.cpp` & `z3-solver-4.9.1.0/core/src/util/timeit.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/timeit.h` & `z3-solver-4.9.1.0/core/src/util/timeit.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/timeout.cpp` & `z3-solver-4.9.1.0/core/src/util/timeout.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/timer.h` & `z3-solver-4.9.1.0/core/src/util/timer.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/top_sort.h` & `z3-solver-4.9.1.0/core/src/util/top_sort.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/total_order.h` & `z3-solver-4.9.1.0/core/src/util/total_order.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/tptr.h` & `z3-solver-4.9.1.0/core/src/util/tptr.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/trace.cpp` & `z3-solver-4.9.1.0/core/src/util/trace.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/trace.h` & `z3-solver-4.9.1.0/core/src/util/trace.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/trail.h` & `z3-solver-4.9.1.0/core/src/util/trail.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/uint_map.h` & `z3-solver-4.9.1.0/core/src/util/uint_map.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/uint_set.h` & `z3-solver-4.9.1.0/core/src/util/uint_set.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/union_find.h` & `z3-solver-4.9.1.0/core/src/util/union_find.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/util.cpp` & `z3-solver-4.9.1.0/core/src/util/util.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/util.h` & `z3-solver-4.9.1.0/core/src/util/util.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/var_queue.h` & `z3-solver-4.9.1.0/core/src/util/var_queue.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/vector.h` & `z3-solver-4.9.1.0/core/src/util/vector.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/warning.cpp` & `z3-solver-4.9.1.0/core/src/util/warning.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/warning.h` & `z3-solver-4.9.1.0/core/src/util/warning.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/z3_exception.cpp` & `z3-solver-4.9.1.0/core/src/util/z3_exception.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/z3_exception.h` & `z3-solver-4.9.1.0/core/src/util/z3_exception.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/zstring.cpp` & `z3-solver-4.9.1.0/core/src/util/zstring.cpp`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/core/src/util/zstring.h` & `z3-solver-4.9.1.0/core/src/util/zstring.h`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/setup.py` & `z3-solver-4.9.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/z3/z3.py` & `z3-solver-4.9.1.0/z3/z3.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/z3/z3num.py` & `z3-solver-4.9.1.0/z3/z3num.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/z3/z3poly.py` & `z3-solver-4.9.1.0/z3/z3poly.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/z3/z3printer.py` & `z3-solver-4.9.1.0/z3/z3printer.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/z3/z3rcf.py` & `z3-solver-4.9.1.0/z3/z3rcf.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/z3/z3types.py` & `z3-solver-4.9.1.0/z3/z3types.py`

 * *Files identical despite different names*

### Comparing `z3-solver-4.9.0.0/z3/z3util.py` & `z3-solver-4.9.1.0/z3/z3util.py`

 * *Files identical despite different names*

