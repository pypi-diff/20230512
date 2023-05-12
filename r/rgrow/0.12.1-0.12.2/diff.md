# Comparing `tmp/rgrow-0.12.1.tar.gz` & `tmp/rgrow-0.12.2.tar.gz`

## Comparing `rgrow-0.12.1.tar` & `rgrow-0.12.2.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0     1857 1970-01-01 00:00:00.000000 rgrow-0.12.1/local_dependencies/rgrow/Cargo.toml
--rw-r--r--   0     1001      123     3565 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/benches/ratestore.rs
--rw-r--r--   0     1001      123     1875 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/benches/sierpinski.rs
--rw-r--r--   0     1001      123      664 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/benches/ui.rs
--rw-r--r--   0     1001      123     3224 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/barish-perfect-sc.yaml
--rwxr-xr-x   0     1001      123     5881 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/barish-perfect.yaml
--rw-r--r--   0     1001      123      150 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/fission-small-ribbon.yaml
--rw-r--r--   0     1001      123     1718 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/sierpinski.yaml
--rw-r--r--   0     1001      123      401 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/tube.yaml
--rwxr-xr-x   0     1001      123      212 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/1dXOR.tiles
--rwxr-xr-x   0     1001      123      478 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/9-square.tiles
--rwxr-xr-x   0     1001      123      165 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/AB.tiles
--rwxr-xr-x   0     1001      123      137 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/ABdiff.tiles
--rwxr-xr-x   0     1001      123      554 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/BarishSeed.tiles
--rwxr-xr-x   0     1001      123      240 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/BinaryCounter.tiles
--rwxr-xr-x   0     1001      123     1357 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/BinaryCounterSquare.tiles
--rwxr-xr-x   0     1001      123     2661 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/BinaryTree.tiles
--rwxr-xr-x   0     1001      123     3149 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/BusyBeaver3Square.tiles
--rwxr-xr-x   0     1001      123      171 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/COPY.tiles
--rwxr-xr-x   0     1001      123      215 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/COPYseed.tiles
--rwxr-xr-x   0     1001      123      245 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/CombSquare.tiles
--rwxr-xr-x   0     1001      123      927 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/DiamondSet.tiles
--rwxr-xr-x   0     1001      123      534 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/DiamondSet_patrick_mullins.tiles
--rwxr-xr-x   0     1001      123      544 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/Rule110.tiles
--rwxr-xr-x   0     1001      123      643 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/Rule110D.tiles
--rwxr-xr-x   0     1001      123      674 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/Rule110Drandom.tiles
--rwxr-xr-x   0     1001      123      712 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/Rule110V.tiles
--rwxr-xr-x   0     1001      123     2686 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/TwoCounterSquareCapped.tiles
--rwxr-xr-x   0     1001      123     3177 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/UL.seed
--rwxr-xr-x   0     1001      123     3041 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/ULcounter.seed
--rwxr-xr-x   0     1001      123      327 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/UnarySquare.tiles
--rwxr-xr-x   0     1001      123      535 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/UnarySquareBig.tiles
--rwxr-xr-x   0     1001      123      561 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/XOR.tiles
--rwxr-xr-x   0     1001      123      801 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/asyncdemo.tiles
--rwxr-xr-x   0     1001      123      185 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/barcode.tiles
--rwxr-xr-x   0     1001      123      229 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/barseed.tiles
--rwxr-xr-x   0     1001      123      528 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/chunk-test.tiles
--rwxr-xr-x   0     1001      123     7278 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/counter2x2indestructible_seed.tiles
--rwxr-xr-x   0     1001      123     2491 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/counter3x3heal_perfect.tiles
--rwxr-xr-x   0     1001      123      852 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/crosshatch.tiles
--rwxr-xr-x   0     1001      123      131 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/diagonal.tiles
--rwxr-xr-x   0     1001      123      145 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/linear1.tiles
--rwxr-xr-x   0     1001      123      187 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/linear2.tiles
--rwxr-xr-x   0     1001      123      204 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/linear3.tiles
--rwxr-xr-x   0     1001      123      172 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/lines1.tiles
--rwxr-xr-x   0     1001      123      184 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/lines2.tiles
--rwxr-xr-x   0     1001      123      600 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/reversibleXOR.tiles
--rwxr-xr-x   0     1001      123      840 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski.tiles
--rwxr-xr-x   0     1001      123     1561 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski1x1_wb.tiles
--rwxr-xr-x   0     1001      123      737 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski2x2.tiles
--rwxr-xr-x   0     1001      123     6791 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski2x2indestructible_seed.tiles
--rwxr-xr-x   0     1001      123     2503 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski3x3_wb.tiles
--rwxr-xr-x   0     1001      123     2491 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski3x3heal_perfect.tiles
--rwxr-xr-x   0     1001      123      874 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski_diag.tiles
--rwxr-xr-x   0     1001      123      700 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/spiral.tiles
--rw-r--r--   0     1001      123      364 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/zig-zag-3w.tiles
--rwxr-xr-x   0     1001      123      614 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/zig-zag-5w-2.5-4.9.tiles
--rw-r--r--   0     1001      123     2134 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/arcsim.rs
--rw-r--r--   0     1001      123     1616 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/base.rs
--rw-r--r--   0     1001      123    19255 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/canvas.rs
--rw-r--r--   0     1001      123     4516 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/cffi.rs
--rw-r--r--   0     1001      123    30787 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/colors.rs
--rw-r--r--   0     1001      123    19915 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/ffs.rs
--rw-r--r--   0     1001      123      497 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/lib.rs
--rw-r--r--   0     1001      123     2591 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/main.rs
--rw-r--r--   0     1001      123    30026 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/models/atam.rs
--rw-r--r--   0     1001      123    14351 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/models/covers.rs
--rw-r--r--   0     1001      123    56483 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/models/ktam.rs
--rw-r--r--   0     1001      123    13221 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/models/ktam_fission.rs
--rw-r--r--   0     1001      123      111 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/models/mod.rs
--rw-r--r--   0     1001      123    32018 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/models/oldktam.rs
--rw-r--r--   0     1001      123    12402 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/models/oldktam_fission.rs
--rw-r--r--   0     1001      123    11057 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/parser_xgrow.rs
--rw-r--r--   0     1001      123     7539 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/ratestore.rs
--rw-r--r--   0     1001      123     7226 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/simulation.rs
--rw-r--r--   0     1001      123    10948 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/state.rs
--rw-r--r--   0     1001      123    15647 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/system.rs
--rw-r--r--   0     1001      123    33582 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/tileset.rs
--rw-r--r--   0     1001      123     3760 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/src/ui.rs
--rw-r--r--   0     1001      123     6376 2023-05-07 23:13:03.000000 rgrow-0.12.1/local_dependencies/rgrow/tests/main.rs
--rw-r--r--   0        0        0      831 1970-01-01 00:00:00.000000 rgrow-0.12.1/Cargo.toml
--rw-r--r--   0     1001      123     1074 2023-05-07 23:13:03.000000 rgrow-0.12.1/LICENSE
--rw-r--r--   0     1001      123      634 2023-05-07 23:13:03.000000 rgrow-0.12.1/Makefile
--rw-r--r--   0     1001      123      162 2023-05-07 23:13:03.000000 rgrow-0.12.1/README.md
--rw-r--r--   0     1001      123     2007 2023-05-07 23:13:03.000000 rgrow-0.12.1/conf.py
--rw-r--r--   0     1001      123       20 2023-05-07 23:13:03.000000 rgrow-0.12.1/docs/.gitignore
--rw-r--r--   0     1001      123      638 2023-05-07 23:13:03.000000 rgrow-0.12.1/docs/Makefile
--rw-r--r--   0     1001      123      491 2023-05-07 23:13:03.000000 rgrow-0.12.1/docs/requirements-docs.txt
--rw-r--r--   0     1001      123     1867 2023-05-07 23:13:03.000000 rgrow-0.12.1/docs/source/conf.py
--rw-r--r--   0     1001      123      498 2023-05-07 23:13:03.000000 rgrow-0.12.1/docs/source/index.rst
--rw-r--r--   0     1001      123      135 2023-05-07 23:13:03.000000 rgrow-0.12.1/docs/source/reference/ffs.rst
--rw-r--r--   0     1001      123      729 2023-05-07 23:13:03.000000 rgrow-0.12.1/docs/source/reference/simulation.rst
--rw-r--r--   0     1001      123      385 2023-05-07 23:13:03.000000 rgrow-0.12.1/docs/source/reference/tileset.rst
--rw-r--r--   0     1001      123      736 2023-05-07 23:13:03.000000 rgrow-0.12.1/index.rst
--rw-r--r--   0     1001      123    17490 2023-05-07 23:13:03.000000 rgrow-0.12.1/old/lib_old.rs
--rw-r--r--   0     1001      123    70410 2023-05-07 23:13:03.000000 rgrow-0.12.1/old/lib_old_2.rs
--rw-r--r--   0     1001      123    10492 2023-05-07 23:13:03.000000 rgrow-0.12.1/old/utils.py
--rw-r--r--   0     1001      123      155 2023-05-07 23:13:03.000000 rgrow-0.12.1/pyproject.toml
--rw-r--r--   0     1001      123      267 2023-05-07 23:13:03.000000 rgrow-0.12.1/rgrow/__init__.py
--rw-r--r--   0     1001      123        0 2023-05-07 23:13:03.000000 rgrow-0.12.1/rgrow/py.typed
--rw-r--r--   0     1001      123     4252 2023-05-07 23:13:03.000000 rgrow-0.12.1/rgrow/rgrow.pyi
--rw-r--r--   0     1001      123      498 2023-05-07 23:13:03.000000 rgrow-0.12.1/src/lib.rs
--rw-r--r--   0     1001      123    28221 2023-05-07 23:13:03.000000 rgrow-0.12.1/src/tileset.rs
--rw-r--r--   0     1001      123    52920 2023-05-07 23:14:07.000000 rgrow-0.12.1/Cargo.lock
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 rgrow-0.12.1/PKG-INFO
+-rw-r--r--   0        0        0     1947 1970-01-01 00:00:00.000000 rgrow-0.12.2/local_dependencies/rgrow/Cargo.toml
+-rw-r--r--   0     1001      123     3580 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/benches/ratestore.rs
+-rw-r--r--   0     1001      123     1875 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/benches/sierpinski.rs
+-rw-r--r--   0     1001      123      664 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/benches/ui.rs
+-rw-r--r--   0     1001      123     3224 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/barish-perfect-sc.yaml
+-rwxr-xr-x   0     1001      123     5881 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/barish-perfect.yaml
+-rw-r--r--   0     1001      123      150 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/fission-small-ribbon.yaml
+-rw-r--r--   0     1001      123     1718 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/sierpinski.yaml
+-rw-r--r--   0     1001      123      401 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/tube.yaml
+-rwxr-xr-x   0     1001      123      212 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/1dXOR.tiles
+-rwxr-xr-x   0     1001      123      478 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/9-square.tiles
+-rwxr-xr-x   0     1001      123      165 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/AB.tiles
+-rwxr-xr-x   0     1001      123      137 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/ABdiff.tiles
+-rwxr-xr-x   0     1001      123      554 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/BarishSeed.tiles
+-rwxr-xr-x   0     1001      123      240 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/BinaryCounter.tiles
+-rwxr-xr-x   0     1001      123     1357 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/BinaryCounterSquare.tiles
+-rwxr-xr-x   0     1001      123     2661 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/BinaryTree.tiles
+-rwxr-xr-x   0     1001      123     3149 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/BusyBeaver3Square.tiles
+-rwxr-xr-x   0     1001      123      171 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/COPY.tiles
+-rwxr-xr-x   0     1001      123      215 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/COPYseed.tiles
+-rwxr-xr-x   0     1001      123      245 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/CombSquare.tiles
+-rwxr-xr-x   0     1001      123      927 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/DiamondSet.tiles
+-rwxr-xr-x   0     1001      123      534 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/DiamondSet_patrick_mullins.tiles
+-rwxr-xr-x   0     1001      123      544 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/Rule110.tiles
+-rwxr-xr-x   0     1001      123      643 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/Rule110D.tiles
+-rwxr-xr-x   0     1001      123      674 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/Rule110Drandom.tiles
+-rwxr-xr-x   0     1001      123      712 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/Rule110V.tiles
+-rwxr-xr-x   0     1001      123     2686 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/TwoCounterSquareCapped.tiles
+-rwxr-xr-x   0     1001      123     3177 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/UL.seed
+-rwxr-xr-x   0     1001      123     3041 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/ULcounter.seed
+-rwxr-xr-x   0     1001      123      327 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/UnarySquare.tiles
+-rwxr-xr-x   0     1001      123      535 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/UnarySquareBig.tiles
+-rwxr-xr-x   0     1001      123      561 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/XOR.tiles
+-rwxr-xr-x   0     1001      123      801 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/asyncdemo.tiles
+-rwxr-xr-x   0     1001      123      185 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/barcode.tiles
+-rwxr-xr-x   0     1001      123      229 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/barseed.tiles
+-rwxr-xr-x   0     1001      123      528 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/chunk-test.tiles
+-rwxr-xr-x   0     1001      123     7278 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/counter2x2indestructible_seed.tiles
+-rwxr-xr-x   0     1001      123     2491 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/counter3x3heal_perfect.tiles
+-rwxr-xr-x   0     1001      123      852 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/crosshatch.tiles
+-rwxr-xr-x   0     1001      123      131 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/diagonal.tiles
+-rwxr-xr-x   0     1001      123      145 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/linear1.tiles
+-rwxr-xr-x   0     1001      123      187 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/linear2.tiles
+-rwxr-xr-x   0     1001      123      204 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/linear3.tiles
+-rwxr-xr-x   0     1001      123      172 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/lines1.tiles
+-rwxr-xr-x   0     1001      123      184 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/lines2.tiles
+-rwxr-xr-x   0     1001      123      600 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/reversibleXOR.tiles
+-rwxr-xr-x   0     1001      123      840 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski.tiles
+-rwxr-xr-x   0     1001      123     1561 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski1x1_wb.tiles
+-rwxr-xr-x   0     1001      123      737 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski2x2.tiles
+-rwxr-xr-x   0     1001      123     6791 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski2x2indestructible_seed.tiles
+-rwxr-xr-x   0     1001      123     2503 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski3x3_wb.tiles
+-rwxr-xr-x   0     1001      123     2491 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski3x3heal_perfect.tiles
+-rwxr-xr-x   0     1001      123      874 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski_diag.tiles
+-rwxr-xr-x   0     1001      123      700 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/spiral.tiles
+-rw-r--r--   0     1001      123      364 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/zig-zag-3w.tiles
+-rwxr-xr-x   0     1001      123      614 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/zig-zag-5w-2.5-4.9.tiles
+-rw-r--r--   0     1001      123     2134 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/arcsim.rs
+-rw-r--r--   0     1001      123     1616 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/base.rs
+-rw-r--r--   0     1001      123    19255 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/canvas.rs
+-rw-r--r--   0     1001      123     4516 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/cffi.rs
+-rw-r--r--   0     1001      123    30787 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/colors.rs
+-rw-r--r--   0     1001      123    19915 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/ffs.rs
+-rw-r--r--   0     1001      123      497 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/lib.rs
+-rw-r--r--   0     1001      123     2594 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/main.rs
+-rw-r--r--   0     1001      123    32664 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/models/atam.rs
+-rw-r--r--   0     1001      123    14351 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/models/covers.rs
+-rw-r--r--   0     1001      123    56482 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/models/ktam.rs
+-rw-r--r--   0     1001      123    13221 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/models/ktam_fission.rs
+-rw-r--r--   0     1001      123      111 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/models/mod.rs
+-rw-r--r--   0     1001      123    32018 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/models/oldktam.rs
+-rw-r--r--   0     1001      123    12402 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/models/oldktam_fission.rs
+-rw-r--r--   0     1001      123    11057 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/parser_xgrow.rs
+-rw-r--r--   0     1001      123     7539 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/ratestore.rs
+-rw-r--r--   0     1001      123     7478 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/simulation.rs
+-rw-r--r--   0     1001      123    10948 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/state.rs
+-rw-r--r--   0     1001      123    15647 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/system.rs
+-rw-r--r--   0     1001      123    33621 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/tileset.rs
+-rw-r--r--   0     1001      123     3760 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/src/ui.rs
+-rw-r--r--   0     1001      123     6376 2023-05-12 20:11:12.000000 rgrow-0.12.2/local_dependencies/rgrow/tests/main.rs
+-rw-r--r--   0        0        0      844 1970-01-01 00:00:00.000000 rgrow-0.12.2/Cargo.toml
+-rw-r--r--   0     1001      123     1074 2023-05-12 20:11:12.000000 rgrow-0.12.2/LICENSE
+-rw-r--r--   0     1001      123      634 2023-05-12 20:11:12.000000 rgrow-0.12.2/Makefile
+-rw-r--r--   0     1001      123      162 2023-05-12 20:11:12.000000 rgrow-0.12.2/README.md
+-rw-r--r--   0     1001      123       20 2023-05-12 20:11:12.000000 rgrow-0.12.2/docs/.gitignore
+-rw-r--r--   0     1001      123      638 2023-05-12 20:11:12.000000 rgrow-0.12.2/docs/Makefile
+-rw-r--r--   0     1001      123      491 2023-05-12 20:11:12.000000 rgrow-0.12.2/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1863 2023-05-12 20:11:12.000000 rgrow-0.12.2/docs/source/conf.py
+-rw-r--r--   0     1001      123      498 2023-05-12 20:11:12.000000 rgrow-0.12.2/docs/source/index.rst
+-rw-r--r--   0     1001      123      135 2023-05-12 20:11:12.000000 rgrow-0.12.2/docs/source/reference/ffs.rst
+-rw-r--r--   0     1001      123     1005 2023-05-12 20:11:12.000000 rgrow-0.12.2/docs/source/reference/simulation.rst
+-rw-r--r--   0     1001      123      385 2023-05-12 20:11:12.000000 rgrow-0.12.2/docs/source/reference/tileset.rst
+-rw-r--r--   0     1001      123      736 2023-05-12 20:11:12.000000 rgrow-0.12.2/index.rst
+-rw-r--r--   0     1001      123    17490 2023-05-12 20:11:12.000000 rgrow-0.12.2/old/lib_old.rs
+-rw-r--r--   0     1001      123    70410 2023-05-12 20:11:12.000000 rgrow-0.12.2/old/lib_old_2.rs
+-rw-r--r--   0     1001      123    10172 2023-05-12 20:11:12.000000 rgrow-0.12.2/old/utils.py
+-rw-r--r--   0     1001      123      256 2023-05-12 20:11:12.000000 rgrow-0.12.2/pyproject.toml
+-rw-r--r--   0     1001      123     1323 2023-05-12 20:11:12.000000 rgrow-0.12.2/rgrow/__init__.py
+-rw-r--r--   0     1001      123        0 2023-05-12 20:11:12.000000 rgrow-0.12.2/rgrow/py.typed
+-rw-r--r--   0     1001      123     6566 2023-05-12 20:11:12.000000 rgrow-0.12.2/rgrow/rgrow.pyi
+-rw-r--r--   0     1001      123      498 2023-05-12 20:11:12.000000 rgrow-0.12.2/src/lib.rs
+-rw-r--r--   0     1001      123    32208 2023-05-12 20:11:12.000000 rgrow-0.12.2/src/tileset.rs
+-rw-r--r--   0     1001      123     1660 2023-05-12 20:11:12.000000 rgrow-0.12.2/tests/test_runs.py
+-rw-r--r--   0     1001      123    52723 2023-05-12 20:12:24.000000 rgrow-0.12.2/Cargo.lock
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 rgrow-0.12.2/PKG-INFO
```

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/Cargo.toml` & `rgrow-0.12.2/local_dependencies/rgrow/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [package]
 name = "rgrow"
 description = "A modular Tile Assembly Model simulator, inspired by Xgrow."
 readme = "../README.md"
-version = "0.12.1"
+version = "0.12.2"
 authors = ["Constantine Evans <const@costi.eu>"]
 edition = "2021"
 repository = "https://github.com/evansfmm/rgrow"
 license = "BSD-3-Clause"
 categories = ["science", "simulation"]
 resolver = "2"
 
@@ -74,7 +74,11 @@
 
 [dependencies.cached]
 version = "0.18"
 default-features = false
 
 [dependencies.num-traits]
 version = "0.2"
+
+[package.metadata.docs.rs]
+no-default-features = true
+features = ["use_rayon", "python"]
```

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/benches/ratestore.rs` & `rgrow-0.12.2/local_dependencies/rgrow/benches/ratestore.rs`

 * *Files 1% similar despite different names*

```diff
@@ -30,16 +30,18 @@
 
     println!("small update");
 
     let plot_config = PlotConfiguration::default().summary_scale(AxisScale::Logarithmic);
 
     let mut group = c.benchmark_group("ratestore-update-all");
     group.plot_config(plot_config.clone());
-    for (pn, pv) in &[("all", &allchanges[..]),
-        ("all_shuffle", &allchanges_shuffled[..])] {
+    for (pn, pv) in &[
+        ("all", &allchanges[..]),
+        ("all_shuffle", &allchanges_shuffled[..]),
+    ] {
         group.bench_with_input(BenchmarkId::new("small update", pn), &pv, |b, a| {
             b.iter(|| rs._update_multiple_small(a))
         });
 
         group.bench_with_input(BenchmarkId::new("large update", pn), &pv, |b, a| {
             b.iter(|| rs_large._update_multiple_large(a))
         });
```

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/benches/sierpinski.rs` & `rgrow-0.12.2/local_dependencies/rgrow/benches/sierpinski.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/benches/ui.rs` & `rgrow-0.12.2/local_dependencies/rgrow/benches/ui.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/barish-perfect-sc.yaml` & `rgrow-0.12.2/local_dependencies/rgrow/examples/barish-perfect-sc.yaml`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/barish-perfect.yaml` & `rgrow-0.12.2/local_dependencies/rgrow/examples/barish-perfect.yaml`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/sierpinski.yaml` & `rgrow-0.12.2/local_dependencies/rgrow/examples/sierpinski.yaml`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/BarishSeed.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/BarishSeed.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/BinaryCounterSquare.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/BinaryCounterSquare.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/BinaryTree.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/BinaryTree.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/BusyBeaver3Square.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/BusyBeaver3Square.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/DiamondSet.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/DiamondSet.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/DiamondSet_patrick_mullins.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/DiamondSet_patrick_mullins.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/Rule110.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/Rule110.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/Rule110D.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/Rule110D.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/Rule110Drandom.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/Rule110Drandom.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/Rule110V.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/Rule110V.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/TwoCounterSquareCapped.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/TwoCounterSquareCapped.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/UL.seed` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/UL.seed`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/ULcounter.seed` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/ULcounter.seed`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/UnarySquareBig.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/UnarySquareBig.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/XOR.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/XOR.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/asyncdemo.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/asyncdemo.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/chunk-test.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/chunk-test.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/counter2x2indestructible_seed.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/counter2x2indestructible_seed.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/counter3x3heal_perfect.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/counter3x3heal_perfect.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/crosshatch.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/crosshatch.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/reversibleXOR.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/reversibleXOR.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski1x1_wb.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski1x1_wb.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski2x2.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski2x2.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski2x2indestructible_seed.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski2x2indestructible_seed.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski3x3_wb.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski3x3_wb.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski3x3heal_perfect.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski3x3heal_perfect.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/sierpinski_diag.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/sierpinski_diag.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/spiral.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/spiral.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/examples/xgrow-format/zig-zag-5w-2.5-4.9.tiles` & `rgrow-0.12.2/local_dependencies/rgrow/examples/xgrow-format/zig-zag-5w-2.5-4.9.tiles`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/arcsim.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/arcsim.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/base.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/base.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/canvas.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/canvas.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/cffi.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/cffi.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/colors.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/colors.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/ffs.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/ffs.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/main.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/main.rs`

 * *Files 2% similar despite different names*

```diff
@@ -64,25 +64,25 @@
     input: String,
 }
 
 fn main() -> anyhow::Result<()> {
     let opts = Opts::parse();
 
     match opts.subcmd {
-        SubCommand::Run(po) =>
-        {
-            #[cfg(feature = "ui")] {
+        SubCommand::Run(po) => {
+            #[cfg(feature = "ui")]
+            {
                 let parsed = TileSet::from_file(po.input)?;
                 run_window(&parsed)?;
-                Ok(())            
+                Ok(())
             }
-            #[cfg(not(feature = "ui"))] {
+            #[cfg(not(feature = "ui"))]
+            {
                 Err(anyhow::anyhow!("UI not enabled."))
             }
-
         }
         SubCommand::NucRate(po) => {
             nucrate(po)?;
             Ok(())
         }
     }
 }
```

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/models/atam.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/models/atam.rs`

 * *Files 6% similar despite different names*

```diff
@@ -298,16 +298,82 @@
                     v.push((*p, *t));
                 }
             }
         };
         v
     }
 
-    fn calc_mismatch_locations<S: State>(&self, _state: &S) -> Array2<usize> {
-        todo!()
+    fn calc_mismatch_locations<S: State>(&self, state: &S) -> Array2<usize> {
+        let threshold = self.threshold / 4.0; // FIXME: this is a hack
+        let mut mismatch_locations = Array2::<usize>::zeros((state.nrows(), state.ncols()));
+
+        // TODO: this should use an iterator from the canvas, which we should implement.
+        for i in 0..state.nrows() {
+            for j in 0..state.ncols() {
+                if !state.inbounds((i, j)) {
+                    continue;
+                }
+                let p = PointSafe2((i, j));
+
+                let t = state.tile_at_point(p);
+
+                if t == 0 {
+                    continue;
+                }
+
+                let tn;
+                let te;
+                let ts;
+                let tw;
+
+                // We set duple directions to 0, because these will be
+                // excluded from the mismatch calculation.
+                match self.tile_shape(t) {
+                    TileShape::Single => {
+                        tn = state.tile_to_n(p);
+                        te = state.tile_to_e(p);
+                        ts = state.tile_to_s(p);
+                        tw = state.tile_to_w(p);
+                    }
+                    TileShape::DupleToRight(_) => {
+                        tn = state.tile_to_n(p);
+                        te = 0;
+                        ts = state.tile_to_s(p);
+                        tw = state.tile_to_w(p);
+                    }
+                    TileShape::DupleToBottom(_) => {
+                        tn = state.tile_to_n(p);
+                        te = state.tile_to_e(p);
+                        ts = 0;
+                        tw = state.tile_to_w(p);
+                    }
+                    TileShape::DupleToLeft(_) => {
+                        tn = state.tile_to_n(p);
+                        te = state.tile_to_e(p);
+                        ts = state.tile_to_s(p);
+                        tw = 0;
+                    }
+                    TileShape::DupleToTop(_) => {
+                        tn = 0;
+                        te = state.tile_to_e(p);
+                        ts = state.tile_to_s(p);
+                        tw = state.tile_to_w(p);
+                    }
+                }
+
+                let mm_n = ((tn != 0) & (self.get_energy_ns(tn, t) < threshold)) as usize;
+                let mm_e = ((te != 0) & (self.get_energy_we(t, te) < threshold)) as usize;
+                let mm_s = ((ts != 0) & (self.get_energy_ns(t, ts) < threshold)) as usize;
+                let mm_w = ((tw != 0) & (self.get_energy_we(tw, t) < threshold)) as usize;
+
+                mismatch_locations[(i, j)] = 8 * mm_n + 4 * mm_e + 2 * mm_s + mm_w;
+            }
+        }
+
+        mismatch_locations
     }
 }
 
 impl ATAM {
     fn get_energy_ns(&self, tn: Tile, ts: Tile) -> Energy {
         self.energy_ns[(tn as usize, ts as usize)]
     }
```

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/models/covers.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/models/covers.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/models/ktam.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/models/ktam.rs`

 * *Files 0% similar despite different names*

```diff
@@ -835,15 +835,15 @@
                     self.energy_ns[(t1, t2)] = self.g_se * self.glue_strengths[t1r[2]]
                 }
                 self.energy_we[(t1, t2)] = self.g_se * self.glue_links[(t1r[1], t2r[3])];
                 if t1r[1] == t2r[3] {
                     self.energy_we[(t1, t2)] = self.g_se * self.glue_strengths[t1r[1]]
                 }
             }
-            self.should_be_counted[t1] =  (t1 > 0) && (self.tile_concs[t1] > 0.);
+            self.should_be_counted[t1] = (t1 > 0) && (self.tile_concs[t1] > 0.);
         }
 
         if (self.double_to_right.sum() > 0) || (self.double_to_bottom.sum() > 0) {
             self.has_duples = true;
             for (t1, t2) in self.double_to_right.indexed_iter() {
                 if (t1 > 0) & (t2 > &0) {
                     let t2 = *t2 as usize;
```

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/models/ktam_fission.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/models/ktam_fission.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/models/oldktam.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/models/oldktam.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/models/oldktam_fission.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/models/oldktam_fission.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/parser_xgrow.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/parser_xgrow.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/ratestore.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/ratestore.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/simulation.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/simulation.rs`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         state_index: usize,
         bounds: EvolveBounds,
     ) -> Result<EvolveOutcome, GrowError>;
     fn state_ref(&self, state_index: usize) -> &dyn State; //std::sync::Arc<RwLock<dyn State>>;
     fn state_mut_ref(&mut self, state_index: usize) -> &mut dyn State; //std::sync::Arc<RwLock<dyn State>>;
     fn n_states(&self) -> usize;
 
+    fn iter_states(&self) -> std::vec::IntoIter<&dyn State>;
+
     fn mismatch_array(&self, state_index: usize) -> Array2<usize>;
     fn n_mismatches(&self, state_index: usize) -> usize;
 
     fn state_keys(&self) -> Vec<usize>;
 
     fn add_state(&mut self) -> Result<usize, GrowError>;
     fn add_n_states(&mut self, n: usize) -> Result<Vec<usize>, GrowError> {
@@ -80,19 +82,25 @@
     fn n_states(&self) -> usize {
         self.states.len()
     }
     fn state_ref(&self, state_index: usize) -> &dyn State {
         //std::sync::Arc<RwLock<dyn State>> {
         &self.states[state_index] //.clone()
     }
+
     fn state_mut_ref(&mut self, state_index: usize) -> &mut dyn State {
         //std::sync::Arc<RwLock<dyn State>> {
         &mut self.states[state_index] //.clone()
     }
 
+    fn iter_states(&self) -> std::vec::IntoIter<&dyn State> {
+        let states: Vec<&dyn State> = self.states.iter().map(|s| s as &dyn State).collect();
+        states.into_iter()
+    }
+
     fn mismatch_array(&self, state_index: usize) -> Array2<usize> {
         let state = &self.states[state_index]; //.lock().unwrap();
         self.system.calc_mismatch_locations(state)
     }
 
     fn n_mismatches(&self, state_index: usize) -> usize {
         let state = &self.states[state_index]; //.lock().unwrap();
```

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/state.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/state.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/system.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/system.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/tileset.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/tileset.rs`

 * *Files 2% similar despite different names*

```diff
@@ -590,39 +590,40 @@
                 .map_or_else(|| None, |x| *(x.downcast_ref().unwrap())),
             update_rate: value
                 .get("update_rate")
                 .map_or_else(update_rate_default, |x| *(x.downcast_ref().unwrap())),
             kf: value
                 .get("kf")
                 .map_or_else(|| None, |x| Some(*(x.downcast_ref().unwrap()))),
-            fission: value.get("chunk_size").map_or_else(
-                fission_default,
-                |x| (x.downcast_ref::<String>().unwrap().as_str()).into(),
-            ),
+            fission: value.get("chunk_size").map_or_else(fission_default, |x| {
+                (x.downcast_ref::<String>().unwrap().as_str()).into()
+            }),
             block: value
                 .get("block")
                 .map_or_else(block_default, |x| *(x.downcast_ref().unwrap())),
             chunk_handling: value.get("chunk_handling").map_or_else(
                 || None,
                 |x| Some((x.downcast_ref::<String>().unwrap().as_str()).into()),
             ),
             chunk_size: value.get("chunk_size").map_or_else(
                 || None,
                 |x| Some(x.downcast_ref::<String>().unwrap().as_str().into()),
             ),
-            canvas_type: value.get("canvas_type").map_or_else(
-                canvas_type_default,
-                |x: &Box<dyn Any>| x.downcast_ref::<String>().unwrap().as_str().into(),
-            ),
+            canvas_type: value
+                .get("canvas_type")
+                .map_or_else(canvas_type_default, |x: &Box<dyn Any>| {
+                    x.downcast_ref::<String>().unwrap().as_str().into()
+                }),
             hdoubletiles: Vec::new(),
             vdoubletiles: Vec::new(),
-            model: value.get("model").map_or_else(
-                model_default,
-                |x: &Box<dyn Any>| x.downcast_ref::<String>().unwrap().as_str().into(),
-            ),
+            model: value
+                .get("model")
+                .map_or_else(model_default, |x: &Box<dyn Any>| {
+                    x.downcast_ref::<String>().unwrap().as_str().into()
+                }),
             threshold: value
                 .get("threshold")
                 .map_or_else(threshold_default, |x| *(x.downcast_ref().unwrap())),
         }
     }
 }
```

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/src/ui.rs` & `rgrow-0.12.2/local_dependencies/rgrow/src/ui.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/local_dependencies/rgrow/tests/main.rs` & `rgrow-0.12.2/local_dependencies/rgrow/tests/main.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/Cargo.toml` & `rgrow-0.12.2/Cargo.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [package]
 name = "pyrgrow"
 description = "Python interface to rgrow."
-version = "0.12.1"
+version = "0.12.2"
 authors = ["Constantine Evans <const@costi.eu>"]
 edition = "2021"
 repository = "https://github.com/evansfmm/rgrow"
 license = "BSD-3-Clause"
 categories = ["science", "simulation"]
 resolver = "2"
 
 
 [features]
-default = ["use_rayon"]  # "ui"
+default = ["use_rayon", "ui"]         # "ui"
 use_rayon = ["rgrow/use_rayon"]
 ui = ["rgrow/ui"]
 
 [lib]
 name = "rgrow"
 path = "src/lib.rs"
 crate-type = ["cdylib"]
```

### Comparing `rgrow-0.12.1/LICENSE` & `rgrow-0.12.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/Makefile` & `rgrow-0.12.2/Makefile`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/docs/Makefile` & `rgrow-0.12.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/docs/source/conf.py` & `rgrow-0.12.2/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 #
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
-#import sphinx_autosummary_accessors
+# import sphinx_autosummary_accessors
 
 # sys.path.insert(0, os.path.abspath("../.."))
 
-project = 'Rgrow'
-copyright = '2023, Constantine Evans'
-author = 'Constantine Evans'
-release = '0.12.0-alpha'
+project = "Rgrow"
+copyright = "2023, Constantine Evans"
+author = "Constantine Evans"
+release = "0.12.2"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     # ----------------------
     # sphinx extensions
@@ -33,34 +33,32 @@
     "sphinx.ext.mathjax",
     "sphinx.ext.todo",
     # ----------------------
     # third-party extensions
     # ----------------------
     "autodocsumm",
     "numpydoc",
-    #"sphinx_autosummary_accessors",
+    # "sphinx_autosummary_accessors",
     "sphinx_copybutton",
     "sphinx_design",
     "sphinx_favicon",
 ]
 
-templates_path = ['_templates'] #, sphinx_autosummary_accessors.templates_path]
+templates_path = ["_templates"]  # , sphinx_autosummary_accessors.templates_path]
 exclude_patterns = []
 
 
-
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "pydata_sphinx_theme"
 
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 
 autosummary_generate = True
 numpydoc_show_class_members = False
 
 intersphinx_mapping = {
     "numpy": ("https://numpy.org/doc/stable/", None),
     "python": ("https://docs.python.org/3", None),
 }
-
```

### Comparing `rgrow-0.12.1/docs/source/reference/simulation.rst` & `rgrow-0.12.2/docs/source/reference/simulation.rst`

 * *Files 8% similar despite different names*

```diff
@@ -10,27 +10,37 @@
 
 .. autosummary::
     :toctree: api/
 
     Simulation
     Simulation.evolve
     Simulation.evolve_all
+    Simulation.evolve_some
 
 ---------------------------------------------
 Modifying simulations and getting information
 ---------------------------------------------
 
 .. autosummary::
     :toctree: api/
 
     Simulation.add_state
     Simulation.add_n_states
     Simulation.set_system_param
     Simulation.get_system_param
     Simulation.canvas_copy
     Simulation.canvas_view
+    Simulation.names_canvas
+    Simulation.state_events
+    Simulation.state_time
+    Simulation.state_ntiles
+    Simulation.states_events
+    Simulation.states_time
+    Simulation.states_ntiles
     Simulation.tile_concs
     Simulation.tile_stoics
     Simulation.tile_names
-    Simulation.state_events
-    Simulation.state_time
-    Simulation.state_ntiles
+    Simulation.tile_colors
+    Simulation.n_mismatches
+    Simulation.mismatch_array
+    Simulation.plot_state
+    Simulation.tile_cmap
```

### Comparing `rgrow-0.12.1/index.rst` & `rgrow-0.12.2/index.rst`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/old/lib_old.rs` & `rgrow-0.12.2/old/lib_old.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/old/lib_old_2.rs` & `rgrow-0.12.2/old/lib_old_2.rs`

 * *Files identical despite different names*

### Comparing `rgrow-0.12.1/old/utils.py` & `rgrow-0.12.2/old/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List, Optional, Tuple, Union, cast, Callable
+
 # import statsmodels
 # import statsmodels.stats.proportion
 from numpy import ndarray
 import numpy as np
 import pandas as pd
 import rgrow.rgrow as rg
 import multiprocessing
@@ -16,16 +17,16 @@
 
     backarray = list(np.array(x) for x in backlist)
 
     trajs = np.full((ntraj, nsurf), -1, dtype=np.int16)
 
     trajs[:, -1] = np.arange(0, ntraj, dtype=np.int16)
 
-    for j in range(nsurf-2, -1, -1):
-        trajs[:, j] = backarray[j+1][trajs[:, j+1]]
+    for j in range(nsurf - 2, -1, -1):
+        trajs[:, j] = backarray[j + 1][trajs[:, j + 1]]
 
     return trajs
 
 
 class FFSResult(rgrow.FFSResult):
     # nucleation_rate: float
     # dimerization_rate: float
@@ -35,21 +36,18 @@
     # num_trials_per_surface: ndarray
     # assembly_size_per_surface: ndarray
     # previous_configs: List[List[int]]
     # aligned_configs: bool = False
     # _saved_trajectory_configs: Optional[ndarray] = None
     # _saved_trajectory_indices: Optional[ndarray] = None
 
-    def align_configs(self,
-                      alignment_function: Callable[
-                          [ndarray], ndarray]) -> None:
+    def align_configs(self, alignment_function: Callable[[ndarray], ndarray]) -> None:
         for assemblies_at_surface in self.assemblies:
             for i in range(0, len(assemblies_at_surface)):
-                assemblies_at_surface[i] = alignment_function(
-                    assemblies_at_surface[i])
+                assemblies_at_surface[i] = alignment_function(assemblies_at_surface[i])
         self.aligned_configs = True
 
     @property
     def trajectory_indices(self) -> ndarray:
         if self._saved_trajectory_indices is not None:
             return self._saved_trajectory_indices
         else:
@@ -69,17 +67,17 @@
         traj_indices = self.trajectory_indices
 
         # FIXME: might be too small...
         tc = np.array(traj_indices.shape + self.canvas_shape, np.int16)
 
         for traj_idx in range(0, len(traj_indices)):
             for surf_idx in range(0, len(traj_indices[0])):
-                tc[traj_idx, surf_idx, :, :] = (self.assemblies[surf_idx][
-                                                traj_indices[traj_idx,
-                                                             surf_idx]])
+                tc[traj_idx, surf_idx, :, :] = self.assemblies[surf_idx][
+                    traj_indices[traj_idx, surf_idx]
+                ]
 
         return tc
 
     @property
     def canvas_shape(self) -> Tuple[int, int]:
         return cast(Tuple[int, int], self.assemblies[0][0].shape)
 
@@ -87,96 +85,142 @@
     def iter_configs(self) -> None:
         pass
 
     @property
     def has_all_configs(self) -> bool:
         return len(self.assemblies) > 1
 
-    def seeds_of_trajectories(self, ts: rgrow.TileSet,
-                              pool: Optional[multiprocessing.pool.Pool]
-                              = None, proppool=False, ci_width=0.1,
-                              min=0.4, max=0.6, ci_pct=0.95, max_events=10_000_000) -> pd.DataFrame:
+    def seeds_of_trajectories(
+        self,
+        ts: rgrow.TileSet,
+        pool: Optional[multiprocessing.pool.Pool] = None,
+        proppool=False,
+        ci_width=0.1,
+        min=0.4,
+        max=0.6,
+        ci_pct=0.95,
+        max_events=10_000_000,
+    ) -> pd.DataFrame:
         trajs = self.trajectory_configs
 
         ts.to_simulation()
 
         if proppool or (pool is None):
             seeds = []
             seedinfos = []
             for i, trajectory in enumerate(trajs):
-                seed, seedinfo = trajectory_seed(system, trajectory, ci_width,
-                                                 min, max, ci_pct, max_events, pool)
+                seed, seedinfo = trajectory_seed(
+                    system, trajectory, ci_width, min, max, ci_pct, max_events, pool
+                )
                 print(".", end=None, flush=True)
                 seeds.append(seed)
                 seedinfos.append(seedinfo)
         else:
-            ss = pool.starmap(trajectory_seed, [
-                              (system, trajectory, ci_width,
-                               min, max, ci_pct, max_events) for trajectory in trajs])
+            ss = pool.starmap(
+                trajectory_seed,
+                [
+                    (system, trajectory, ci_width, min, max, ci_pct, max_events)
+                    for trajectory in trajs
+                ],
+            )
             seeds, seedinfos = zip(*ss)
 
         p = pd.DataFrame(seedinfos)
-        p['config'] = list(seeds)
+        p["config"] = list(seeds)
 
         return p
 
     @property
-    def tuple(self) -> Tuple[float, float, ndarray, List[ndarray], ndarray,
-                             ndarray, ndarray, List[List[int]]]:
-        return (self.nucleation_rate,
-                self.dimerization_rate,
-                self.forward_probability,
-                self.assemblies,
-                self.num_configs_per_surface,
-                self.num_trials_per_surface,
-                self.assembly_size_per_surface,
-                self.previous_configs)
+    def tuple(
+        self,
+    ) -> Tuple[
+        float, float, ndarray, List[ndarray], ndarray, ndarray, ndarray, List[List[int]]
+    ]:
+        return (
+            self.nucleation_rate,
+            self.dimerization_rate,
+            self.forward_probability,
+            self.assemblies,
+            self.num_configs_per_surface,
+            self.num_trials_per_surface,
+            self.assembly_size_per_surface,
+            self.previous_configs,
+        )
 
-    def __getitem__(self, idx: int) -> Union[float, ndarray, List[ndarray],
-                                             List[List[int]]]:
+    def __getitem__(
+        self, idx: int
+    ) -> Union[float, ndarray, List[ndarray], List[List[int]]]:
         """Fakes the old return tuple"""
         return self.tuple[idx]
 
     def __repr__(self) -> str:
-        return (f"FFSResult(nucrate={self.nucleation_rate:.4g} M/s, " +
-                f"has_all_configs={self.has_all_configs}, " +
-                f"num_surfaces={len(self.assembly_size_per_surface)}, " +
-                f"num_trajectories={len(self.previous_indices[-1])}"
-                ")")
+        return (
+            f"FFSResult(nucrate={self.nucleation_rate:.4g} M/s, "
+            + f"has_all_configs={self.has_all_configs}, "
+            + f"num_surfaces={len(self.assembly_size_per_surface)}, "
+            + f"num_trajectories={len(self.previous_indices[-1])}"
+            ")"
+        )
 
     def __str__(self) -> str:
         return repr(self)
 
 
-def trajectory_seed(sim, trajectory,
-                    ci_width=0.1,
-                    min=0.4, max=0.6, ci_pct=0.95, max_events=10_000_000,
-                    pool: multiprocessing.pool.Pool = None,) -> Tuple[ndarray, pd.Series]:
+def trajectory_seed(
+    sim,
+    trajectory,
+    ci_width=0.1,
+    min=0.4,
+    max=0.6,
+    ci_pct=0.95,
+    max_events=10_000_000,
+    pool: multiprocessing.pool.Pool = None,
+) -> Tuple[ndarray, pd.Series]:
     """Given a sim and trajectory (of configurations), find the seed
     (committor closest to 0.5)"""
 
     if pool is None:
-        trajs = pd.DataFrame([committor_mid(sim, config, ci_width=0.10)
-                              for config in trajectory],
-                             columns=[
-            "in", "side", "c", "clow", "chigh", "succ", "trials"])
+        trajs = pd.DataFrame(
+            [committor_mid(sim, config, ci_width=0.10) for config in trajectory],
+            columns=["in", "side", "c", "clow", "chigh", "succ", "trials"],
+        )
     else:
         trres = pool.starmap(
-            committor_mid, [(sim, config, ci_width, min, max, ci_pct, rg.StaticKTAMPeriodic, max_events) for config in trajectory])
-        trajs = pd.DataFrame(trres, columns=[
-            "in", "side", "c", "clow", "chigh", "succ", "trials"])
+            committor_mid,
+            [
+                (
+                    sim,
+                    config,
+                    ci_width,
+                    min,
+                    max,
+                    ci_pct,
+                    rg.StaticKTAMPeriodic,
+                    max_events,
+                )
+                for config in trajectory
+            ],
+        )
+        trajs = pd.DataFrame(
+            trres, columns=["in", "side", "c", "clow", "chigh", "succ", "trials"]
+        )
 
     seed_idx = np.abs(trajs.loc[:, "c"] - 0.5).argmin()
 
     return (trajectory[seed_idx], trajs.loc[seed_idx, :])
 
 
-def committor(sim: rgrow.Simulation, config, ci_width: float = 0.05, state_type=rg.StateKTAMPeriodic,
-              ci_pct: float = 0.95, min_trials: float = 10) -> Tuple[float, float,
-                                                                     float, int, int]:
+def committor(
+    sim: rgrow.Simulation,
+    config,
+    ci_width: float = 0.05,
+    state_type=rg.StateKTAMPeriodic,
+    ci_pct: float = 0.95,
+    min_trials: float = 10,
+) -> Tuple[float, float, float, int, int]:
     trials = 0
     successes = 0
 
     while True:
         state = state_type(config.shape[0], system)
         for y in range(0, config.shape[0]):
             for x in range(0, config.shape[1]):
@@ -184,28 +228,31 @@
         state.evolve_in_size_range(system, 0, 300, 1_000_000)
         trials += 1
         if state.ntiles >= 300:
             successes += 1
         elif state.ntiles != 0:
             raise ValueError
         ci: Tuple[float, float] = statsmodels.stats.proportion.proportion_confint(
-            successes, trials, 1-ci_pct, method='jeffreys')  # type:ignore
-        if ci[1]-ci[0] <= ci_width and trials > min_trials:
+            successes, trials, 1 - ci_pct, method="jeffreys"
+        )  # type:ignore
+        if ci[1] - ci[0] <= ci_width and trials > min_trials:
             # print(f"Finished after {trials}: p = {successes/trials} {ci}")
-            return (successes/trials, ci[0], ci[1], successes, trials)
+            return (successes / trials, ci[0], ci[1], successes, trials)
 
 
-def committor_mid(sim: rgrow.Simulation, config, ci_width=0.05,
-                  min=0.4, max=0.6, ci_pct=0.95,
-                  state_type=rg.StateKTAMPeriodic,
-                  max_events=10_000_000) -> Tuple[bool,
-                                                            Optional[bool],
-                                                            float,
-                                                            float, float,
-                                                            int, int]:
+def committor_mid(
+    sim: rgrow.Simulation,
+    config,
+    ci_width=0.05,
+    min=0.4,
+    max=0.6,
+    ci_pct=0.95,
+    state_type=rg.StateKTAMPeriodic,
+    max_events=10_000_000,
+) -> Tuple[bool, Optional[bool], float, float, float, int, int]:
     trials = 0
     successes = 0
 
     while True:
         state = state_type(config.shape[0], system)
         for y in range(0, config.shape[0]):
             for x in range(0, config.shape[1]):
@@ -213,52 +260,61 @@
         state.evolve_in_size_range(system, 0, 300, max_events)
         trials += 1
         if state.ntiles >= 300:
             successes += 1
         elif state.ntiles != 0:
             raise ValueError
         ci: Tuple[float, float] = statsmodels.stats.proportion.proportion_confint(
-            successes, trials, 1-ci_pct, method='jeffreys')  # type:ignore
-        if ci[1]-ci[0] <= ci_width and trials > 4:
+            successes, trials, 1 - ci_pct, method="jeffreys"
+        )  # type:ignore
+        if ci[1] - ci[0] <= ci_width and trials > 4:
             # print(f"Finished after {trials}: p = {successes/trials} {ci}")
-            return (True, None, successes/trials, ci[0], ci[1],
-                    successes, trials)
+            return (True, None, successes / trials, ci[0], ci[1], successes, trials)
         elif (ci[1] < min) or (ci[0] > max):
-            return (False, ci[0] > max, successes/trials, ci[0],
-                    ci[1], successes, trials)
-
-
-def ffs_nucleation(system,
-                   max_size=200,
-                   canvas_size=32,
-                   keep_surface_configs=False,
-                   cutoff_probability=0.99,
-                   cutoff_surfaces=4,
-                   min_configs=1_000,
-                   varpermean2=1e-4,
-                   min_cutoff_size=30,
-                   _surface_size_step=1,
-                   _surface_init_size=3,
-                   _max_init_events=10_000,
-                   _max_subseq_events=1_000_000):
+            return (
+                False,
+                ci[0] > max,
+                successes / trials,
+                ci[0],
+                ci[1],
+                successes,
+                trials,
+            )
+
+
+def ffs_nucleation(
+    system,
+    max_size=200,
+    canvas_size=32,
+    keep_surface_configs=False,
+    cutoff_probability=0.99,
+    cutoff_surfaces=4,
+    min_configs=1_000,
+    varpermean2=1e-4,
+    min_cutoff_size=30,
+    _surface_size_step=1,
+    _surface_init_size=3,
+    _max_init_events=10_000,
+    _max_subseq_events=1_000_000,
+):
     if isinstance(system, rg.StaticKTAMPeriodic):
         restuple = rg.ffs_run_final_p_cvar_cut(
             system,
             varpermean2,
             min_configs,
             max_size,
             cutoff_probability,
             cutoff_surfaces,
             min_cutoff_size,
             canvas_size,
             _max_init_events,
             _max_subseq_events,
             _surface_init_size,
             _surface_size_step,
-            keep_surface_configs
+            keep_surface_configs,
         )
         return FFSResult(*restuple, system=system)
     elif isinstance(system, rg.NewKTAMPeriodic):
         restuple = rg.ffs_run_final_p_cvar_cut_new(
             system,
             varpermean2,
             min_configs,
@@ -267,12 +323,12 @@
             cutoff_surfaces,
             min_cutoff_size,
             canvas_size,
             _max_init_events,
             _max_subseq_events,
             _surface_init_size,
             _surface_size_step,
-            keep_surface_configs
+            keep_surface_configs,
         )
         return FFSResult(*restuple, system=system)
     else:
         raise TypeError(f"Can't handle system type {type(system)}.")
```

### Comparing `rgrow-0.12.1/rgrow/rgrow.pyi` & `rgrow-0.12.2/rgrow/rgrow.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+from typing import Any, Sequence, TYPE_CHECKING
 import numpy as np
 
-class EvolveOutcome(object):
-    ...
+if TYPE_CHECKING:  # pragma: no cover
+    import matplotlib.pyplot as plt
+    import matplotlib.colors
+
+class EvolveOutcome(object): ...
 
 class FFSLevel(object):
     @property
     def configs(self) -> list[np.ndarray]:
         """List of configurations at this level, as arrays (not full states)."""
         ...
     @property
@@ -21,92 +25,70 @@
         for_events: int | None = None,
         total_events: int | None = None,
         for_time: float | None = None,
         total_time: float | None = None,
         size_min: float | None = None,
         size_max: float | None = None,
         for_wall_time: float | None = None,
-        require_strong_bound: bool = True
-    ) -> EvolveOutcome: 
+        require_strong_bound: bool = True,
+    ) -> EvolveOutcome:
         """Evolve a particular state, with index `state_index`,
         subject to some bounds.  Runs state 0 by default.
 
         By default, this requires a strong bound (the simulation
         will eventually end, eg, not a size or other potentially
         unreachable bound).
-        
+
         Releases the GIL during the simulation."""
         ...
-    
     def evolve_all(
         self,
         state_index: int | None = None,
         for_events: int | None = None,
         total_events: int | None = None,
         for_time: float | None = None,
         total_time: float | None = None,
         size_min: float | None = None,
         size_max: float | None = None,
         for_wall_time: float | None = None,
-        require_strong_bound: bool = True
+        require_strong_bound: bool = True,
     ) -> list[EvolveOutcome]:
         """Evolve *all* states, stopping each as they reach the
         boundary conditions.  Runs multithreaded using available
         cores.  Runs state 0 by default.
         """
         ...
-
-    def canvas_copy(
-        self,
-        state_index: int | None
-    ) -> np.ndarray:
+    def canvas_copy(self, state_index: int | None) -> np.ndarray:
         "Returns a copy of the state canvas."
-
-    def canvas_view(
-        self,
-        state_index: int | None
-    ) -> np.ndarray:
+    def canvas_view(self, state_index: int | None) -> np.ndarray:
         """Returns a direct view of the state canvas.  Note that this
         can potentially be unsafe, if the state is later erased."""
-
-    def state_ntiles(
-        self,
-        state_index: int | None
-    ) -> int:
+    def state_ntiles(self, state_index: int | None) -> int:
         """Returns the number of tiles in the state."""
-
-    def state_time(
-        self,
-        state_index: int | None
-    ) -> float:
+    def state_time(self, state_index: int | None) -> float:
         """Returns the amount of time simulated (in seconds) for the state."""
-
-    def state_events(
-        self,
-        state_index: int | None
-    ) -> int:
+    def state_events(self, state_index: int | None) -> int:
         """Returns the number of events simulated for the state."""
-
-    def add_state(
-        self
-    ) -> int:
+    def add_state(self) -> int:
         """Add a new state, returning its index."""
-
-    def add_n_states(
-        self,
-        n: int
-    ) -> list[int]:
+    def add_n_states(self, n: int) -> list[int]:
         """Add `n` new states, returning their indices."""
-    
     tile_concs: list[float]
     tile_stoics: list[float]
 
+    @property
+    def tile_colors(self) -> list[tuple[int, int, int, int]]: ...
+    def plot_state(
+        self: Simulation, state: int = 0, ax: "int | plt.Axes" = None
+    ) -> "plt.QuadMesh | Any": ...
+    def tile_cmap(self) -> "matplotlib.colors.ListedColorMap": ...
+
 class FFSResult(object):
     @property
-    def nucleation_rate(self) -> float: 
+    def nucleation_rate(self) -> float:
         """
         The calculated nucleation rate, in M/s.
         """
         ...
     @property
     def forward_vec(self) -> np.ndarray: ...
     @property
@@ -134,13 +116,76 @@
         surface_init_size: int = 3,
         max_init_events: int = 10_000,
         max_subseq_events: int = 1_000_000,
         max_init_time: float | None = None,
         max_subseq_time: float | None = None,
         keep_surface_configs: bool = False,
     ) -> FFSResult: ...
+    def __init__(
+        self,
+        tiles: Sequence[Tile],
+        bonds: Sequence[tuple[str | int, float]],
+        glues: Sequence[tuple[str | int, str | int, float]],
+        options: dict[str, Any],
+    ) -> None: ...
 
 class Tile(object):
-    ...
+    def __init__(
+        self,
+        bonds: list[str | int],
+        name: str | None = None,
+        stoic: float | None = None,
+        color: str | None = None,
+    ) -> None: ...
+
+class EvolveBounds(object):
+    def __init__(
+        self,
+        for_events: int | None = None,
+        total_events: int | None = None,
+        for_time: float | None = None,
+        total_time: float | None = None,
+        size_min: float | None = None,
+        size_max: float | None = None,
+        for_wall_time: float | None = None,
+        require_strong_bound: bool = True,
+    ) -> None: ...
 
 class FFSRunConfig(object):
-    ...
+    # Use constant-variance, variable-configurations-per-surface method.
+    # If false, use max_configs for each surface.
+    @property
+    def constant_variance(self) -> bool: ...
+    # Variance per mean^2 for constant-variance method.
+    @property
+    def var_per_mean2(self) -> float: ...
+    # Minimum number of configuratons to generate at each level.
+    @property
+    def min_configs(self) -> int: ...
+    # Maximum number of configurations to generate at each level.
+    @property
+    def max_configs(self) -> int: ...
+    # Use early cutoff for constant-variance method.
+    @property
+    def early_cutoff(self) -> bool: ...
+    @property
+    def cutoff_probability(self) -> float: ...
+    @property
+    def cutoff_number(self) -> int: ...
+    @property
+    def min_cutoff_size(self) -> int: ...
+    @property
+    def init_bound(self) -> EvolveBounds: ...
+    @property
+    def subseq_bound(self) -> EvolveBounds: ...
+    @property
+    def start_size(self) -> int: ...
+    @property
+    def size_step(self) -> int: ...
+    @property
+    def keep_configs(self) -> bool: ...
+    @property
+    def min_nuc_rate(self) -> float | None: ...
+    @property
+    def canvas_size(self) -> tuple[int, int]: ...
+    @property
+    def target_size(self) -> int: ...
```

### Comparing `rgrow-0.12.1/src/tileset.rs` & `rgrow-0.12.2/src/tileset.rs`

 * *Files 10% similar despite different names*

```diff
@@ -20,16 +20,14 @@
 use rgrow::simulation;
 use rgrow::system::EvolveBounds;
 use rgrow::system::EvolveOutcome;
 use rgrow::tileset;
 use rgrow::tileset::Ident;
 use rgrow::tileset::TileShape;
 
-
-
 #[derive(FromPyObject, Clone)]
 struct Bond(Ident, f64);
 
 impl From<tileset::Tile> for Tile {
     fn from(tile: tileset::Tile) -> Self {
         Tile(tile)
     }
@@ -486,17 +484,14 @@
     /// By default, this requires a strong bound (the simulation
     /// will eventually end, eg, not a size or other potentially
     /// unreachable bound). Releases the GIL during the simulation.
     /// Bounds are applied for each state individually.    
     ///
     /// Parameters
     /// ----------
-    /// state_index : int, optional
-    ///    The index of the state to evolve.  Defaults to 0, and creates sufficient states
-    ///    if they do not already exist.
     /// for_events : int, optional
     ///    Evolve until this many events have occurred.  Defaults to no limit. (Strong bound)
     /// total_events : int, optional
     ///    Evolve until this many events have occurred in total.  Defaults to no limit. (Strong bound)
     /// for_time : float, optional
     ///    Evolve until this much (physical) time has passed.  Defaults to no limit. (Strong bound)
     /// total_time : float, optional
@@ -557,14 +552,52 @@
         let res = py.allow_threads(|| self.write().unwrap().evolve_all(bounds));
 
         res.into_iter()
             .map(|x| x.map_err(|y| PyValueError::new_err(y.to_string())))
             .collect()
     }
 
+    /// Evolve *some* states, stopping each as they reach the
+    /// boundary conditions.  Runs multithreaded using available
+    /// cores.
+    ///
+    /// By default, this requires a strong bound (the simulation
+    /// will eventually end, eg, not a size or other potentially
+    /// unreachable bound). Releases the GIL during the simulation.
+    /// Bounds are applied for each state individually.    
+    ///
+    /// Parameters
+    /// ----------
+    /// state_indices : list[int]
+    ///   The indices of the states to evolve.
+    /// for_events : int, optional
+    ///    Evolve until this many events have occurred.  Defaults to no limit. (Strong bound)
+    /// total_events : int, optional
+    ///    Evolve until this many events have occurred in total.  Defaults to no limit. (Strong bound)
+    /// for_time : float, optional
+    ///    Evolve until this much (physical) time has passed.  Defaults to no limit. (Strong bound)
+    /// total_time : float, optional
+    ///    Evolve until this much (physical) time has passed since the state creation.  
+    ///    Defaults to no limit. (Strong bound)
+    /// size_min : int, optional
+    ///    Evolve until the system has this many, or fewer, tiles. Defaults to no limit. (Weak bound)
+    /// size_max : int, optional
+    ///    Evolve until the system has this many, or more, tiles. Defaults to no limit. (Weak bound)
+    /// for_wall_time : float, optional
+    ///    Evolve until this much (wall) time has passed.  Defaults to no limit. (Strong bound)
+    /// require_strong_bound : bool, optional
+    ///    If True (default), a ValueError will be raised unless at least one strong bound has been
+    ///    set, ensuring that the simulation will eventually end.  If False, ensure only that some
+    ///    weak bound has been set, which may result in an infinite simulation.
+    ///
+    /// Returns
+    /// -------
+    ///
+    /// list[EvolveOutcome]
+    ///   The stopping condition that caused each simulation to end.
     #[pyo3(
         signature = (state_indices,
                     for_events=None,
                     total_events=None,
                     for_time=None,
                     total_time=None,
                     size_min=None,
@@ -642,14 +675,39 @@
         Ok(self
             .read()?
             .state_ref(state_index)
             .raw_array()
             .to_pyarray(py))
     }
 
+    /// Returns the current canvas for state_index (default 0), as an array of tile names.
+    /// 'empty' indicates empty locations; numbers are translated to strings.
+    ///
+    /// Parameters
+    /// ----------
+    /// state_index : int, optional
+    ///  The index of the state to return.  Defaults to 0.
+    ///
+    /// Returns
+    /// -------
+    ///
+    /// numpy.ndarray[str]
+    ///  The current canvas for the state, as an array of tile names.
+    fn name_canvas<'py>(
+        &self,
+        state_index: Option<usize>,
+        py: Python<'py>,
+    ) -> PyResult<&'py PyArray2<PyObject>> {
+        let state_index = self.check_state(state_index)?;
+        let sim = self.read()?;
+        let ra = sim.state_ref(state_index).raw_array();
+        let names = sim.tile_names();
+        Ok(ra.mapv(|x| names[x as usize].to_object(py)).to_pyarray(py))
+    }
+
     /// Returns the current canvas for state_index (default 0), as a
     /// *direct* view of the state array.  This array will update as
     /// the simulation evolves.  It should not be modified, as modifications
     /// will not result in rate and other necessary updates.
     ///
     /// Using this may cause memory safety problems: it is 'unsafe'-labelled in Rust.
     /// Unless the state is deleted, the array should remain valid so long as the
@@ -675,14 +733,36 @@
         let sim = sim.read()?;
 
         let ra = sim.state_ref(state_index).raw_array();
 
         unsafe { Ok(PyArray2::borrow_from_array(&ra, this)) }
     }
 
+    /// Returns a list of the number of tiles in each state.
+    #[getter]
+    fn states_ntiles(&self) -> PyResult<Vec<u32>> {
+        Ok(self.read()?.iter_states().map(|x| x.ntiles()).collect())
+    }
+
+    /// Returns a list of the amount of time simulated (in seconds) for each state.
+    #[getter]
+    fn states_time(&self) -> PyResult<Vec<f64>> {
+        Ok(self.read()?.iter_states().map(|x| x.time()).collect())
+    }
+
+    /// Returns a list of the total number of events simulated for each state.
+    #[getter]
+    fn states_events(&self) -> PyResult<Vec<u64>> {
+        Ok(self
+            .read()?
+            .iter_states()
+            .map(|x| x.total_events())
+            .collect())
+    }
+
     /// Returns the number of tiles in the state.
     fn state_ntiles(&self, state_index: Option<usize>) -> PyResult<u32> {
         let state_index = self.check_state(state_index)?;
         Ok(self.read()?.state_ref(state_index).ntiles())
     }
 
     /// Returns the amount of time simulated (in seconds) for the state.
@@ -722,21 +802,45 @@
     }
 
     #[getter]
     fn get_tile_names(&self) -> PyResult<Vec<String>> {
         Ok(self.read()?.tile_names())
     }
 
-    fn set_system_param(&self, name: &str, value: RustAny) {
+    #[getter]
+    fn get_tile_colors(&self) -> PyResult<Vec<[u8; 4]>> {
+        Ok(self.read()?.tile_colors().clone())
+    }
+
+    /// Sets a system parameter.
+    ///
+    /// Parameters
+    /// ----------
+    /// name : str
+    ///   The name of the parameter.
+    /// value : Any
+    ///   The value of the parameter.
+    fn set_system_param(&self, name: &str, value: RustAny) -> PyResult<()> {
         self.write()
             .unwrap()
             .set_system_param(name, value.0)
-            .unwrap();
+            .map_err(|x| PyValueError::new_err(x.to_string()))
     }
 
+    /// Gets a system parameter.
+    ///
+    /// Parameters
+    /// ----------
+    /// name : str
+    ///   The name of the parameter.
+    ///
+    /// Returns
+    /// -------
+    /// Any
+    ///   The value of the parameter.
     fn get_system_param(&self, name: &str, py: Python) -> PyResult<Py<PyAny>> {
         self.read()
             .unwrap()
             .get_system_param(name)
             .map(|x| RustAny(x).into_py(py))
             .map_err(|x| PyValueError::new_err(x.to_string()))
     }
```

### Comparing `rgrow-0.12.1/Cargo.lock` & `rgrow-0.12.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -185,17 +185,17 @@
 name = "block"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0d8c1fef690941d3e7788d328517591fecc684c084084702d6ff1641e993699a"
 
 [[package]]
 name = "bumpalo"
-version = "3.12.1"
+version = "3.12.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
+checksum = "3c6ed94e98ecff0c12dd1b04c15ec0d7d9458ca8fe806cea6f12954efe74c63b"
 
 [[package]]
 name = "bytemuck"
 version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
 
@@ -451,20 +451,14 @@
 checksum = "dd4056f63fce3b82d852c3da92b08ea59959890813a7f4ce9c0ff85b10cf301b"
 dependencies = [
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
-name = "cty"
-version = "0.2.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b365fabc795046672053e29c954733ec3b05e4be654ab130fe8f1f94d7051f35"
-
-[[package]]
 name = "d3d12"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8f0de2f5a8e7bd4a9eec0e3c781992a4ce1724f68aec7d7a3715344de8b39da"
 dependencies = [
  "bitflags 1.3.2",
  "libloading",
@@ -496,34 +490,33 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "fltk"
-version = "1.4.2"
+version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4f8b550f22216bd317bc77db5e888200f0caf3789f8e4b2df126eccbaab3bbfd"
+checksum = "9aaf7cacace3db3d685f447f54b69fdc73c757fac0a00b5d965c4592e01de343"
 dependencies = [
  "bitflags 2.2.1",
  "crossbeam-channel",
  "fltk-sys",
  "paste",
  "raw-window-handle",
  "ttf-parser",
 ]
 
 [[package]]
 name = "fltk-sys"
-version = "1.4.2"
+version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ada976a05b18bac0b880786e03fb6678f7d6176ab52c5761f726c732b5500f8"
+checksum = "f4e06030256cc3edd00bfc01f5730a2ec08bf16086be01721d67980f753ac2db"
 dependencies = [
  "cmake",
- "cty",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
@@ -778,17 +771,17 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.62"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "68c16e1bfd491478ab155fd8b4896b86f9ede344949b641e61501e07c2b8b4d5"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "khronos-egl"
 version = "4.1.0"
@@ -804,17 +797,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.143"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "edc207893e85c5d6be840e969b496b53d94cec8be2d501b214f50daa97fa8024"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "libloading"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
 dependencies = [
@@ -1262,31 +1255,31 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyrgrow"
-version = "0.12.1"
+version = "0.12.2"
 dependencies = [
  "bincode",
  "indent",
  "ndarray",
  "numpy",
  "pyo3",
  "rand",
  "rgrow",
  "serde",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1385,15 +1378,15 @@
 name = "renderdoc-sys"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1382d1f0a252c4bf97dc20d979a2fdd05b024acd7c2ed0f7595d7817666a157"
 
 [[package]]
 name = "rgrow"
-version = "0.12.1"
+version = "0.12.2"
 dependencies = [
  "anyhow",
  "bimap",
  "cached",
  "clap 4.2.7",
  "criterion",
  "fltk",
@@ -1468,17 +1461,17 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
 name = "serde"
-version = "1.0.162"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71b2f6e1ab5c2b98c05f0f35b236b22e8df7ead6ffbf51d7808da7f8817e7ab6"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_cbor"
 version = "0.11.2"
@@ -1487,17 +1480,17 @@
 dependencies = [
  "half",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.162"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2a0814352fd64b58489904a44ea8d90cb1a91dcb6b4f5ebabc32c8318e93cb6"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.15",
 ]
 
 [[package]]
@@ -1714,83 +1707,83 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "5b6cb788c4e39112fbe1822277ef6fb3c55cd86b95cb3d3c4c1c9597e4ac74b4"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "35e522ed4105a9d626d885b35d62501b30d9666283a5c8be12c14a8bdafe7822"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.34"
+version = "0.4.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f219e0d211ba40266969f6dbdd90636da12f75bee4fc9d6c23d1260dadb51454"
+checksum = "083abe15c5d88556b77bdf7aef403625be9e327ad37c62c4e4129af740168163"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "358a79a0cb89d21db8120cbfb91392335913e4890665b1a7981d9e956903b434"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "4783ce29f09b9d93134d41297aded3a712b7b979e9c6f28c32cb88c973a94869"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.85"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "a901d592cafaa4d711bc324edfaff879ac700b19c3dfd60058d2b445be2691eb"
 
 [[package]]
 name = "web-sys"
-version = "0.3.61"
+version = "0.3.62"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+checksum = "16b5f940c7edfdc6d12126d98c9ef4d1b3d470011c47c76a6581df47ad9ba721"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "wgpu"
```

### Comparing `rgrow-0.12.1/PKG-INFO` & `rgrow-0.12.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgrow
-Version: 0.12.1
+Version: 0.12.2
 Requires-Dist: numpy
 License-File: LICENSE
 Summary: Python interface to rgrow.
 Author: Constantine Evans <const@costi.eu>
 Author-email: Constantine Evans <const@costi.eu>
 License: BSD-3-Clause
 Requires-Python: >=3.9
```

