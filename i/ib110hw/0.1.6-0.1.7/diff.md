# Comparing `tmp/ib110hw-0.1.6.tar.gz` & `tmp/ib110hw-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Skola\SBAPR\ib110hw\dist\tmpi3f1tgnd\ib110hw-0.1.6.tar", last modified: Mon May  8 22:47:34 2023, max compression
+gzip compressed data, was "C:\Skola\SBAPR\ib110hw\dist\tmpx_ey2wc_\ib110hw-0.1.7.tar", last modified: Fri May 12 20:18:43 2023, max compression
```

## Comparing `ib110hw-0.1.6.tar` & `ib110hw-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/
--rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.6/LICENSE
--rw-rw-rw-   0        0        0    30454 2023-05-08 22:47:34.000000 ib110hw-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0    30013 2023-05-01 15:32:55.000000 ib110hw-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-08 22:47:34.000000 ib110hw-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      700 2023-05-08 22:38:08.000000 ib110hw-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw/
-drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw/automaton/
--rw-rw-rw-   0        0        0     2412 2023-04-17 13:09:33.000000 ib110hw-0.1.6/src/ib110hw/automaton/base.py
--rw-rw-rw-   0        0        0     8339 2023-04-17 13:10:40.000000 ib110hw-0.1.6/src/ib110hw/automaton/dfa.py
--rw-rw-rw-   0        0        0     8592 2023-04-17 13:11:16.000000 ib110hw-0.1.6/src/ib110hw/automaton/nfa.py
--rw-rw-rw-   0        0        0     1461 2023-04-17 08:06:18.000000 ib110hw-0.1.6/src/ib110hw/automaton/utils.py
--rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.6/src/ib110hw/automaton/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw/turing/
--rw-rw-rw-   0        0        0     1227 2023-05-01 15:28:06.000000 ib110hw-0.1.6/src/ib110hw/turing/base.py
--rw-rw-rw-   0        0        0     6270 2023-05-08 22:36:18.000000 ib110hw-0.1.6/src/ib110hw/turing/dtm.py
--rw-rw-rw-   0        0        0     6962 2023-05-08 22:36:08.000000 ib110hw-0.1.6/src/ib110hw/turing/mtm.py
--rw-rw-rw-   0        0        0     3535 2023-05-01 15:33:06.000000 ib110hw-0.1.6/src/ib110hw/turing/tape.py
--rw-rw-rw-   0        0        0     2419 2023-05-08 22:35:52.000000 ib110hw-0.1.6/src/ib110hw/turing/utils.py
--rw-rw-rw-   0        0        0     8749 2023-05-08 22:36:41.000000 ib110hw-0.1.6/src/ib110hw/turing/_helpers.py
--rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.6/src/ib110hw/turing/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.6/src/ib110hw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0    30454 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw.egg-info/requires.txt
--rw-rw-rw-   0        0        0      645 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-05-08 22:47:34.000000 ib110hw-0.1.6/src/ib110hw.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-08 22:47:34.000000 ib110hw-0.1.6/tests/
--rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.6/tests/test_dfa.py
--rw-rw-rw-   0        0        0     2363 2023-05-01 15:18:14.000000 ib110hw-0.1.6/tests/test_dtm.py
--rw-rw-rw-   0        0        0     2022 2023-05-01 15:18:12.000000 ib110hw-0.1.6/tests/test_mtm.py
--rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.6/tests/test_nfa.py
+drwxrwxrwx   0        0        0        0 2023-05-12 20:18:43.000000 ib110hw-0.1.7/
+-rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0    30406 2023-05-12 20:18:43.000000 ib110hw-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0    29965 2023-05-12 20:11:18.000000 ib110hw-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-12 20:18:43.000000 ib110hw-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      700 2023-05-12 20:18:00.000000 ib110hw-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 20:18:43.000000 ib110hw-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-12 20:18:43.000000 ib110hw-0.1.7/src/ib110hw/
+drwxrwxrwx   0        0        0        0 2023-05-12 20:18:43.000000 ib110hw-0.1.7/src/ib110hw/automaton/
+-rw-rw-rw-   0        0        0     2412 2023-04-17 13:09:33.000000 ib110hw-0.1.7/src/ib110hw/automaton/base.py
+-rw-rw-rw-   0        0        0     8339 2023-04-17 13:10:40.000000 ib110hw-0.1.7/src/ib110hw/automaton/dfa.py
+-rw-rw-rw-   0        0        0     8592 2023-04-17 13:11:16.000000 ib110hw-0.1.7/src/ib110hw/automaton/nfa.py
+-rw-rw-rw-   0        0        0     1461 2023-04-17 08:06:18.000000 ib110hw-0.1.7/src/ib110hw/automaton/utils.py
+-rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.7/src/ib110hw/automaton/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 20:18:43.000000 ib110hw-0.1.7/src/ib110hw/turing/
+-rw-rw-rw-   0        0        0     1227 2023-05-01 15:28:06.000000 ib110hw-0.1.7/src/ib110hw/turing/base.py
+-rw-rw-rw-   0        0        0     6268 2023-05-12 16:18:10.000000 ib110hw-0.1.7/src/ib110hw/turing/dtm.py
+-rw-rw-rw-   0        0        0     6962 2023-05-08 22:36:08.000000 ib110hw-0.1.7/src/ib110hw/turing/mtm.py
+-rw-rw-rw-   0        0        0     3535 2023-05-12 10:47:19.000000 ib110hw-0.1.7/src/ib110hw/turing/tape.py
+-rw-rw-rw-   0        0        0     2419 2023-05-08 22:35:52.000000 ib110hw-0.1.7/src/ib110hw/turing/utils.py
+-rw-rw-rw-   0        0        0     9465 2023-05-12 19:56:03.000000 ib110hw-0.1.7/src/ib110hw/turing/_helpers.py
+-rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.7/src/ib110hw/turing/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.7/src/ib110hw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-12 20:18:43.000000 ib110hw-0.1.7/src/ib110hw.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-12 20:18:43.000000 ib110hw-0.1.7/src/ib110hw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0    30406 2023-05-12 20:18:43.000000 ib110hw-0.1.7/src/ib110hw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-05-12 20:18:43.000000 ib110hw-0.1.7/src/ib110hw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      645 2023-05-12 20:18:43.000000 ib110hw-0.1.7/src/ib110hw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 20:18:43.000000 ib110hw-0.1.7/src/ib110hw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-12 20:18:43.000000 ib110hw-0.1.7/tests/
+-rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.7/tests/test_dfa.py
+-rw-rw-rw-   0        0        0     3880 2023-05-12 16:49:59.000000 ib110hw-0.1.7/tests/test_dtm.py
+-rw-rw-rw-   0        0        0     3462 2023-05-12 19:43:51.000000 ib110hw-0.1.7/tests/test_mtm.py
+-rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.7/tests/test_nfa.py
```

### Comparing `ib110hw-0.1.6/LICENSE` & `ib110hw-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.6/PKG-INFO` & `ib110hw-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib110hw
-Version: 0.1.6
+Version: 0.1.7
 Summary: UNKNOWN
 Home-page: https://github.com/pilatmartin/ib110hw
 Author: Martin Pilát
 Author-email: 8pilatmartin8@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -138,17 +138,17 @@
 automaton.get_symbols_between_states("s3", "s5") # returns {"1", "0"}
 automaton.get_symbols_between_states("s1", "s3") # returns set()
 ```
 
 ```python
 # returns True if the given string is accepted by the automaton, False otherwise
 # IMPORTANT: the automaton needs to be valid (see below) to be able to test 
-automaton.is_accepted("11") # True
-automaton.is_accepted("00") # True
-automaton.is_accepted("10") # False
+automaton.is_accepted("11") # False
+automaton.is_accepted("00") # False
+automaton.is_accepted("10") # True
 ```
 
 ```python
 # Checks whether the DFA is valid:
 #     1. The states set is not empty.
 #     2. The initial state is in states.
 #     3. Final states are subset of states.
@@ -267,16 +267,16 @@
 ```
 
 </br>
 
 [![DFA object with removed transition](https://mermaid.ink/img/pako:eNpdkT1rwzAQhv-KOAjYYIM_FxUyZUyWZKw7COvSCH_IyPJgQv57L3KlJtWk59Hx6ri7Q6slAodvI6YbO56bkdGZsyiaszj-pZwoD1QQFYFKojJQRVQFqiPCOn6yz_1kXyxN95TpswlzZwqfH0z5YjJnav_rsyZ5c7vdFrbJyjcUTPli8rew-n-Y87Nde6SO2VX1faon0Sq78iyhB6M7_DMfkMCAZhBK0iDvLgDsDQdsgNNVCtM10IwPqhOL1Zd1bIFbs2ACyySFxYMSNP8B-FX0M1mUympz2jbjFvT4AUZlcck?type=png)](https://mermaid.live/edit#pako:eNpdkT1rwzAQhv-KOAjYYIM_FxUyZUyWZKw7COvSCH_IyPJgQv57L3KlJtWk59Hx6ri7Q6slAodvI6YbO56bkdGZsyiaszj-pZwoD1QQFYFKojJQRVQFqiPCOn6yz_1kXyxN95TpswlzZwqfH0z5YjJnav_rsyZ5c7vdFrbJyjcUTPli8rew-n-Y87Nde6SO2VX1faon0Sq78iyhB6M7_DMfkMCAZhBK0iDvLgDsDQdsgNNVCtM10IwPqhOL1Zd1bIFbs2ACyySFxYMSNP8B-FX0M1mUympz2jbjFvT4AUZlcck)
 
 ```python
-# removes the state s4 and every transition associated with it
-dfa_showcase.remove_state("s4")
+# removes the state s3 and every transition associated with it
+dfa_showcase.remove_state("s")
 ```
 
 </br>
 
 [![DFA object after removing a state](https://mermaid.ink/img/pako:eNplkT1rwzAQhv-KOAjYYIM_5EWFTh3bJRnrDsK6NCK2ZSR5MCH_vRe1kkurSc-j471Dd4PBKAQBn1YuF_Z67GdGx1VZ5qo8_6GaqE7UEDWRDgfmWhJteuZEPFGXEXb5g2P0O_tgZflMsTGesA6m2UObJNvYl0wVTPer96Os-KfrVMt3yZOMkTw16eK8f_OCd34bkUZnZz2OpVnkoP0mqoIerLnibp6ggAntJLWiT72FAPAXnLAHQVcl7bWHfr5TnVy9OW3zAMLbFQtYFyU9vmhJu5hAnOXoyKLS3ti37y2FZd2_AMruc3E?type=png)](https://mermaid.live/edit#pako:eNplkT1rwzAQhv-KOAjYYIM_5EWFTh3bJRnrDsK6NCK2ZSR5MCH_vRe1kkurSc-j471Dd4PBKAQBn1YuF_Z67GdGx1VZ5qo8_6GaqE7UEDWRDgfmWhJteuZEPFGXEXb5g2P0O_tgZflMsTGesA6m2UObJNvYl0wVTPer96Os-KfrVMt3yZOMkTw16eK8f_OCd34bkUZnZz2OpVnkoP0mqoIerLnibp6ggAntJLWiT72FAPAXnLAHQVcl7bWHfr5TnVy9OW3zAMLbFQtYFyU9vmhJu5hAnOXoyKLS3ti37y2FZd2_AMruc3E)
 
 ##### Visualization
@@ -569,20 +569,20 @@
 checkB  X -> reject X S
 back    a -> back   a L
 back    b -> back   b L
 back    X -> mark   X R
 
 ```
 
-The file above can then be simply loaded using the `load_dtm_from_file(...)`:
+The file above can then be simply loaded using the `import_dtm(...)`:
 
 ```python
-from ib110hw.turing.utils import load_dtm_from_file
+from ib110hw.turing.utils import import_dtm
 
-machine = load_dtm_from_file("./dtm_file")
+machine = import_dtm("./dtm_file")
 ```
 
 ## Multi-tape Turing Machine (MTM)
 
 On top of the properties required to create DTM, you will need to specify the number of tapes as well. The default tape count is set to 2.
 
 The following MTM has the same function as the DTM above:
@@ -673,20 +673,20 @@
 check       (b b) -> check        (b b) (R L)
 check       (_ _) -> acc          (_ _) (S S)
 check       (a b) -> rej          (a b) (S S)
 check       (b a) -> rej          (b a) (S S)
 
 ```
 
-The file above can then be simply loaded using the `load_dtm_from_file(...)`:
+The file above can then be simply loaded using the `import_mtm(...)`:
 
 ```python
-from ib110hw.turing.utils import load_mtm_from_file
+from ib110hw.turing.utils import import_mtm
 
-machine = load_mtm_from_file("./mtm_file")
+machine = import_mtm("./mtm_file")
 ```
 
 # DTM and MTM Simulation
 
 You can simulate the Turing machine using the provided function `simulate(...)`. By default, every step of the Turing machine will be printed to console with 0.5s delay in-between. This behavior can be changed by setting the `to_console` and `delay` parameters. If the parameter `to_console` is set to `False`, the delay will be ignored.
 
 ```python
```

### Comparing `ib110hw-0.1.6/README.md` & `ib110hw-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -123,17 +123,17 @@
 automaton.get_symbols_between_states("s3", "s5") # returns {"1", "0"}
 automaton.get_symbols_between_states("s1", "s3") # returns set()
 ```
 
 ```python
 # returns True if the given string is accepted by the automaton, False otherwise
 # IMPORTANT: the automaton needs to be valid (see below) to be able to test 
-automaton.is_accepted("11") # True
-automaton.is_accepted("00") # True
-automaton.is_accepted("10") # False
+automaton.is_accepted("11") # False
+automaton.is_accepted("00") # False
+automaton.is_accepted("10") # True
 ```
 
 ```python
 # Checks whether the DFA is valid:
 #     1. The states set is not empty.
 #     2. The initial state is in states.
 #     3. Final states are subset of states.
@@ -252,16 +252,16 @@
 ```
 
 </br>
 
 [![DFA object with removed transition](https://mermaid.ink/img/pako:eNpdkT1rwzAQhv-KOAjYYIM_FxUyZUyWZKw7COvSCH_IyPJgQv57L3KlJtWk59Hx6ri7Q6slAodvI6YbO56bkdGZsyiaszj-pZwoD1QQFYFKojJQRVQFqiPCOn6yz_1kXyxN95TpswlzZwqfH0z5YjJnav_rsyZ5c7vdFrbJyjcUTPli8rew-n-Y87Nde6SO2VX1faon0Sq78iyhB6M7_DMfkMCAZhBK0iDvLgDsDQdsgNNVCtM10IwPqhOL1Zd1bIFbs2ACyySFxYMSNP8B-FX0M1mUympz2jbjFvT4AUZlcck?type=png)](https://mermaid.live/edit#pako:eNpdkT1rwzAQhv-KOAjYYIM_FxUyZUyWZKw7COvSCH_IyPJgQv57L3KlJtWk59Hx6ri7Q6slAodvI6YbO56bkdGZsyiaszj-pZwoD1QQFYFKojJQRVQFqiPCOn6yz_1kXyxN95TpswlzZwqfH0z5YjJnav_rsyZ5c7vdFrbJyjcUTPli8rew-n-Y87Nde6SO2VX1faon0Sq78iyhB6M7_DMfkMCAZhBK0iDvLgDsDQdsgNNVCtM10IwPqhOL1Zd1bIFbs2ACyySFxYMSNP8B-FX0M1mUympz2jbjFvT4AUZlcck)
 
 ```python
-# removes the state s4 and every transition associated with it
-dfa_showcase.remove_state("s4")
+# removes the state s3 and every transition associated with it
+dfa_showcase.remove_state("s")
 ```
 
 </br>
 
 [![DFA object after removing a state](https://mermaid.ink/img/pako:eNplkT1rwzAQhv-KOAjYYIM_5EWFTh3bJRnrDsK6NCK2ZSR5MCH_vRe1kkurSc-j471Dd4PBKAQBn1YuF_Z67GdGx1VZ5qo8_6GaqE7UEDWRDgfmWhJteuZEPFGXEXb5g2P0O_tgZflMsTGesA6m2UObJNvYl0wVTPer96Os-KfrVMt3yZOMkTw16eK8f_OCd34bkUZnZz2OpVnkoP0mqoIerLnibp6ggAntJLWiT72FAPAXnLAHQVcl7bWHfr5TnVy9OW3zAMLbFQtYFyU9vmhJu5hAnOXoyKLS3ti37y2FZd2_AMruc3E?type=png)](https://mermaid.live/edit#pako:eNplkT1rwzAQhv-KOAjYYIM_5EWFTh3bJRnrDsK6NCK2ZSR5MCH_vRe1kkurSc-j471Dd4PBKAQBn1YuF_Z67GdGx1VZ5qo8_6GaqE7UEDWRDgfmWhJteuZEPFGXEXb5g2P0O_tgZflMsTGesA6m2UObJNvYl0wVTPer96Os-KfrVMt3yZOMkTw16eK8f_OCd34bkUZnZz2OpVnkoP0mqoIerLnibp6ggAntJLWiT72FAPAXnLAHQVcl7bWHfr5TnVy9OW3zAMLbFQtYFyU9vmhJu5hAnOXoyKLS3ti37y2FZd2_AMruc3E)
 
 ##### Visualization
@@ -554,20 +554,20 @@
 checkB  X -> reject X S
 back    a -> back   a L
 back    b -> back   b L
 back    X -> mark   X R
 
 ```
 
-The file above can then be simply loaded using the `load_dtm_from_file(...)`:
+The file above can then be simply loaded using the `import_dtm(...)`:
 
 ```python
-from ib110hw.turing.utils import load_dtm_from_file
+from ib110hw.turing.utils import import_dtm
 
-machine = load_dtm_from_file("./dtm_file")
+machine = import_dtm("./dtm_file")
 ```
 
 ## Multi-tape Turing Machine (MTM)
 
 On top of the properties required to create DTM, you will need to specify the number of tapes as well. The default tape count is set to 2.
 
 The following MTM has the same function as the DTM above:
@@ -658,20 +658,20 @@
 check       (b b) -> check        (b b) (R L)
 check       (_ _) -> acc          (_ _) (S S)
 check       (a b) -> rej          (a b) (S S)
 check       (b a) -> rej          (b a) (S S)
 
 ```
 
-The file above can then be simply loaded using the `load_dtm_from_file(...)`:
+The file above can then be simply loaded using the `import_mtm(...)`:
 
 ```python
-from ib110hw.turing.utils import load_mtm_from_file
+from ib110hw.turing.utils import import_mtm
 
-machine = load_mtm_from_file("./mtm_file")
+machine = import_mtm("./mtm_file")
 ```
 
 # DTM and MTM Simulation
 
 You can simulate the Turing machine using the provided function `simulate(...)`. By default, every step of the Turing machine will be printed to console with 0.5s delay in-between. This behavior can be changed by setting the `to_console` and `delay` parameters. If the parameter `to_console` is set to `False`, the delay will be ignored.
 
 ```python
```

### Comparing `ib110hw-0.1.6/setup.py` & `ib110hw-0.1.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ib110hw",
-    version="0.1.6",
+    version="0.1.7",
     author="Martin Pilát",
     author_email="8pilatmartin8@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ib110hw-0.1.6/src/ib110hw/automaton/base.py` & `ib110hw-0.1.7/src/ib110hw/automaton/base.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.6/src/ib110hw/automaton/dfa.py` & `ib110hw-0.1.7/src/ib110hw/automaton/dfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.6/src/ib110hw/automaton/nfa.py` & `ib110hw-0.1.7/src/ib110hw/automaton/nfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.6/src/ib110hw/automaton/utils.py` & `ib110hw-0.1.7/src/ib110hw/automaton/utils.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.6/src/ib110hw/turing/base.py` & `ib110hw-0.1.7/src/ib110hw/turing/base.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.6/src/ib110hw/turing/dtm.py` & `ib110hw-0.1.7/src/ib110hw/turing/dtm.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,25 +17,25 @@
     """
 
     def __init__(
         self,
         states: Set[str] = None,
         input_alphabet: Set[str] = None,
         acc_state: str = "accept",
-        rej_states: str = "reject",
+        rej_state: str = "reject",
         transitions: DTMTransitions = None,
         tape: Tape = None,
         initial_state: str = "init",
         start_symbol: str = START_SYMBOL,
     ) -> None:
         super().__init__(
             states,
             input_alphabet,
             acc_state,
-            rej_states,
+            rej_state,
             initial_state,
             start_symbol,
         )
         self.transitions = transitions if transitions is not None else {}
         self.tape = tape or Tape()
 
     def get_transition(self, state: str, read: str) -> Optional[DTMRule]:
```

### Comparing `ib110hw-0.1.6/src/ib110hw/turing/mtm.py` & `ib110hw-0.1.7/src/ib110hw/turing/mtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.6/src/ib110hw/turing/tape.py` & `ib110hw-0.1.7/src/ib110hw/turing/tape.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.6/src/ib110hw/turing/utils.py` & `ib110hw-0.1.7/src/ib110hw/turing/utils.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.6/src/ib110hw/turing/_helpers.py` & `ib110hw-0.1.7/src/ib110hw/turing/_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     if file:
         file.close()
 
 
 # inspired by https://stackoverflow.com/a/43106497
 def get_step_direction() -> str:
     step_direction = None
-    print("Use arrow keys [L|R] to go back or forward. Esc to exit.")
+    print("Use arrow keys [L|R] to go back or forward. Press ESC to exit.")
 
     def on_press(key):
         nonlocal step_direction
         try:
             if key.name in ["left", "right", "esc"]:
                 step_direction = key.name
                 return False
@@ -89,17 +89,17 @@
     init, acc, rej = "", "", ""
     alphabet = set()
 
     for line in config:
         if line.startswith("init"):
             init = line.split()[1]
         elif line.startswith("acc"):
-            acc = {*line.split()[1:]}
+            acc = line.split()[1]
         elif line.startswith("rej"):
-            rej = {*line.split()[1:]}
+            rej = line.split()[1]
         elif line.startswith("alphabet"):
             alphabet = {*line.split()[1:]}
 
     return init, acc, rej, alphabet or set()
 
 
 def get_mtm_configuration(
@@ -126,59 +126,79 @@
         curr_state, read = left.split()
         next_state, write, direction = right.split()
 
         if not function.get(curr_state):
             function[curr_state] = {}
 
         read = read if read != "_" else ""
+        write = write if write != "_" else ""
         function[curr_state][read] = (next_state, write, parse_direction(direction))
 
     return function
 
 
 def validate_dtm_configuration(definition: List[str]) -> Optional[str]:
     if all(l.strip() != "---" for l in definition):
         return "The divider is missing."
 
-    config = list(takewhile(lambda l: l != "---", definition))[:-1]
+    config = list(takewhile(lambda l: l != "---", definition))
 
     if not any((l.startswith("init") for l in config)):
         return "Specifying the initial state is mandatory."
 
     init_line = next((l for l in config if l.startswith("init")), None)
-    if init_line:
-        if len(init_line.split()) != 2:
-            return "Invalid initial state"
+    if init_line and len(init_line.split()) != 2:
+        return "Invalid initial state."
+
+    acc_line = next((l for l in config if l.startswith("acc")), None)
+    if acc_line and len(acc_line.split()) != 2:
+        return "Invalid accepting state."
+
+    rej_line = next((l for l in config if l.startswith("rej")), None)
+    if rej_line and len(rej_line.split()) != 2:
+        return "Invalid rejecting state."
+
+    alphabet_line = next((l for l in config if l.startswith("alphabet")), None)
+    if not alphabet_line:
+        return "The alphabet definition is missing."
+
+    if len(alphabet_line.split()) < 2 or any(len(s) > 1 for s in alphabet_line.split()[1:]):
+        return "Invalid alphabet."
 
 
 def validate_mtm_configuration(definition: List[str]) -> Optional[str]:
     err = validate_dtm_configuration(definition)
     if err:
         return err
 
     tapes_line = [
         l for l in definition if re.match(r"tapes ([2-9]|[1-9]\d+)", l.strip())
     ]
     if len(tapes_line) > 1:
         return "Duplicate definition of tape count."
 
-    if len(tapes_line) == 0:
+    if not tapes_line:
         return "Missing or invalid definition of tape count."
 
 
 def validate_dtm_transitions(definition: List[str]) -> Optional[str]:
     get_part = lambda l, i: l.split("->")[i]
+    
     # checks the length of arguments on the left side
     valid_current = lambda l: len(get_part(l, 0).split()) == 2
+    
     # checks the length of the read symbol
     valid_read = lambda l: len(get_part(l, 0).split()[1]) == 1
+    
     # checks the length of arguments on the right side
     valid_next = lambda l: len(get_part(l, 1).split()) == 3
+    
     # checks the length of the write symbol
     valid_write = lambda l: len(get_part(l, 1).split()[1]) == 1
+    
     # checks the direction
     valid_dir = lambda l: get_part(l, 1).split()[-1] in ["L", "R", "S"]
 
     return validate_transitions(
         definition,
         valid_current,
         valid_read,
@@ -188,24 +208,27 @@
     )
 
 
 def validate_mtm_transitions(definition: List[str]) -> Optional[str]:
     get_part = lambda l, i: l.split("->")[i]
     # checks the length of arguments on the left side
     valid_current = lambda l: re.match(r"^\w+ \([^)]+\)", get_part(l, 0)) is not None
+    
     # checks the length of the read symbols
     valid_read = (
         lambda l: re.match(r"(. )+.", get_part(l, 0).split(" (")[1][:-1]) is not None
     )
     # checks the length of arguments on the right side
-    valid_next = lambda l: len(get_part(l, 1).split(" (")) == 3
+    valid_next = lambda l: len(list(filter(None, get_part(l, 1).split(" (")))) == 3
+    
     # checks the length of the write symbols
     valid_write = (
         lambda l: bool(re.match(r"^(. )+.$", get_part(l, 1).split(" (")[1][:-1])) == 1
     )
+    
     # checks the direction
     valid_dir = lambda l: set(get_part(l, 1).split(" (")[-1][:-1].split()).issubset(
         ["L", "R", "S"]
     )
 
     return validate_transitions(
         definition,
```

### Comparing `ib110hw-0.1.6/src/ib110hw.egg-info/PKG-INFO` & `ib110hw-0.1.7/src/ib110hw.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ib110hw
-Version: 0.1.6
+Version: 0.1.7
 Summary: UNKNOWN
 Home-page: https://github.com/pilatmartin/ib110hw
 Author: Martin Pilát
 Author-email: 8pilatmartin8@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -138,17 +138,17 @@
 automaton.get_symbols_between_states("s3", "s5") # returns {"1", "0"}
 automaton.get_symbols_between_states("s1", "s3") # returns set()
 ```
 
 ```python
 # returns True if the given string is accepted by the automaton, False otherwise
 # IMPORTANT: the automaton needs to be valid (see below) to be able to test 
-automaton.is_accepted("11") # True
-automaton.is_accepted("00") # True
-automaton.is_accepted("10") # False
+automaton.is_accepted("11") # False
+automaton.is_accepted("00") # False
+automaton.is_accepted("10") # True
 ```
 
 ```python
 # Checks whether the DFA is valid:
 #     1. The states set is not empty.
 #     2. The initial state is in states.
 #     3. Final states are subset of states.
@@ -267,16 +267,16 @@
 ```
 
 </br>
 
 [![DFA object with removed transition](https://mermaid.ink/img/pako:eNpdkT1rwzAQhv-KOAjYYIM_FxUyZUyWZKw7COvSCH_IyPJgQv57L3KlJtWk59Hx6ri7Q6slAodvI6YbO56bkdGZsyiaszj-pZwoD1QQFYFKojJQRVQFqiPCOn6yz_1kXyxN95TpswlzZwqfH0z5YjJnav_rsyZ5c7vdFrbJyjcUTPli8rew-n-Y87Nde6SO2VX1faon0Sq78iyhB6M7_DMfkMCAZhBK0iDvLgDsDQdsgNNVCtM10IwPqhOL1Zd1bIFbs2ACyySFxYMSNP8B-FX0M1mUympz2jbjFvT4AUZlcck?type=png)](https://mermaid.live/edit#pako:eNpdkT1rwzAQhv-KOAjYYIM_FxUyZUyWZKw7COvSCH_IyPJgQv57L3KlJtWk59Hx6ri7Q6slAodvI6YbO56bkdGZsyiaszj-pZwoD1QQFYFKojJQRVQFqiPCOn6yz_1kXyxN95TpswlzZwqfH0z5YjJnav_rsyZ5c7vdFrbJyjcUTPli8rew-n-Y87Nde6SO2VX1faon0Sq78iyhB6M7_DMfkMCAZhBK0iDvLgDsDQdsgNNVCtM10IwPqhOL1Zd1bIFbs2ACyySFxYMSNP8B-FX0M1mUympz2jbjFvT4AUZlcck)
 
 ```python
-# removes the state s4 and every transition associated with it
-dfa_showcase.remove_state("s4")
+# removes the state s3 and every transition associated with it
+dfa_showcase.remove_state("s")
 ```
 
 </br>
 
 [![DFA object after removing a state](https://mermaid.ink/img/pako:eNplkT1rwzAQhv-KOAjYYIM_5EWFTh3bJRnrDsK6NCK2ZSR5MCH_vRe1kkurSc-j471Dd4PBKAQBn1YuF_Z67GdGx1VZ5qo8_6GaqE7UEDWRDgfmWhJteuZEPFGXEXb5g2P0O_tgZflMsTGesA6m2UObJNvYl0wVTPer96Os-KfrVMt3yZOMkTw16eK8f_OCd34bkUZnZz2OpVnkoP0mqoIerLnibp6ggAntJLWiT72FAPAXnLAHQVcl7bWHfr5TnVy9OW3zAMLbFQtYFyU9vmhJu5hAnOXoyKLS3ti37y2FZd2_AMruc3E?type=png)](https://mermaid.live/edit#pako:eNplkT1rwzAQhv-KOAjYYIM_5EWFTh3bJRnrDsK6NCK2ZSR5MCH_vRe1kkurSc-j471Dd4PBKAQBn1YuF_Z67GdGx1VZ5qo8_6GaqE7UEDWRDgfmWhJteuZEPFGXEXb5g2P0O_tgZflMsTGesA6m2UObJNvYl0wVTPer96Os-KfrVMt3yZOMkTw16eK8f_OCd34bkUZnZz2OpVnkoP0mqoIerLnibp6ggAntJLWiT72FAPAXnLAHQVcl7bWHfr5TnVy9OW3zAMLbFQtYFyU9vmhJu5hAnOXoyKLS3ti37y2FZd2_AMruc3E)
 
 ##### Visualization
@@ -569,20 +569,20 @@
 checkB  X -> reject X S
 back    a -> back   a L
 back    b -> back   b L
 back    X -> mark   X R
 
 ```
 
-The file above can then be simply loaded using the `load_dtm_from_file(...)`:
+The file above can then be simply loaded using the `import_dtm(...)`:
 
 ```python
-from ib110hw.turing.utils import load_dtm_from_file
+from ib110hw.turing.utils import import_dtm
 
-machine = load_dtm_from_file("./dtm_file")
+machine = import_dtm("./dtm_file")
 ```
 
 ## Multi-tape Turing Machine (MTM)
 
 On top of the properties required to create DTM, you will need to specify the number of tapes as well. The default tape count is set to 2.
 
 The following MTM has the same function as the DTM above:
@@ -673,20 +673,20 @@
 check       (b b) -> check        (b b) (R L)
 check       (_ _) -> acc          (_ _) (S S)
 check       (a b) -> rej          (a b) (S S)
 check       (b a) -> rej          (b a) (S S)
 
 ```
 
-The file above can then be simply loaded using the `load_dtm_from_file(...)`:
+The file above can then be simply loaded using the `import_mtm(...)`:
 
 ```python
-from ib110hw.turing.utils import load_mtm_from_file
+from ib110hw.turing.utils import import_mtm
 
-machine = load_mtm_from_file("./mtm_file")
+machine = import_mtm("./mtm_file")
 ```
 
 # DTM and MTM Simulation
 
 You can simulate the Turing machine using the provided function `simulate(...)`. By default, every step of the Turing machine will be printed to console with 0.5s delay in-between. This behavior can be changed by setting the `to_console` and `delay` parameters. If the parameter `to_console` is set to `False`, the delay will be ignored.
 
 ```python
```

### Comparing `ib110hw-0.1.6/src/ib110hw.egg-info/SOURCES.txt` & `ib110hw-0.1.7/src/ib110hw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.6/tests/test_dfa.py` & `ib110hw-0.1.7/tests/test_dfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.1.6/tests/test_nfa.py` & `ib110hw-0.1.7/tests/test_nfa.py`

 * *Files identical despite different names*

