# Comparing `tmp/schematodes-0.1.0.tar.gz` & `tmp/schematodes-0.2.0.tar.gz`

## Comparing `schematodes-0.1.0.tar` & `schematodes-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 schematodes-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     2809 2023-05-10 20:27:50.000000 schematodes-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      686 2023-05-10 20:27:50.000000 schematodes-0.1.0/.gitignore
--rw-r--r--   0     1001      123      806 2023-05-10 20:27:50.000000 schematodes-0.1.0/Readme.md
--rw-r--r--   0     1001      123     3757 2023-05-10 20:27:50.000000 schematodes-0.1.0/examples/playtest.py
--rw-r--r--   0     1001      123      438 2023-05-10 20:27:50.000000 schematodes-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123     1671 2023-05-10 20:27:50.000000 schematodes-0.1.0/scratch.txt
--rw-r--r--   0     1001      123       89 2023-05-10 20:27:50.000000 schematodes-0.1.0/setup.cfg
--rw-r--r--   0     1001      123     9568 2023-05-10 20:27:50.000000 schematodes-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     1295 2023-05-10 20:27:50.000000 schematodes-0.1.0/stubs/schematodes/__init__.pyi
--rw-r--r--   0     1001      123     8083 2023-05-10 20:27:50.000000 schematodes-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 schematodes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 schematodes-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     2809 2023-05-12 13:38:43.000000 schematodes-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      692 2023-05-12 13:38:43.000000 schematodes-0.2.0/.gitignore
+-rw-r--r--   0     1001      123      806 2023-05-12 13:38:43.000000 schematodes-0.2.0/Readme.md
+-rw-r--r--   0     1001      123     4373 2023-05-12 13:38:43.000000 schematodes-0.2.0/examples/playtest.py
+-rw-r--r--   0     1001      123      405 2023-05-12 13:38:43.000000 schematodes-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123     1295 2023-05-12 13:38:43.000000 schematodes-0.2.0/schematodes.pyi
+-rw-r--r--   0     1001      123     1671 2023-05-12 13:38:43.000000 schematodes-0.2.0/scratch.txt
+-rw-r--r--   0     1001      123       89 2023-05-12 13:38:43.000000 schematodes-0.2.0/setup.cfg
+-rw-r--r--   0     1001      123    10947 2023-05-12 13:38:43.000000 schematodes-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123     8083 2023-05-12 13:38:43.000000 schematodes-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 schematodes-0.2.0/PKG-INFO
```

### Comparing `schematodes-0.1.0/.github/workflows/CI.yml` & `schematodes-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `schematodes-0.1.0/.gitignore` & `schematodes-0.2.0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 /target
-
+.mypy*
 # Byte-compiled / optimized / DLL files
 __pycache__/
 .pytest_cache/
 *.py[cod]
 
 # C extensions
 *.so
```

### Comparing `schematodes-0.1.0/Readme.md` & `schematodes-0.2.0/Readme.md`

 * *Files identical despite different names*

### Comparing `schematodes-0.1.0/examples/playtest.py` & `schematodes-0.2.0/examples/playtest.py`

 * *Files 22% similar despite different names*

```diff
@@ -150,7 +150,37 @@
         [0, 1, 1, 1],  # f1'
         [1, 0, 2, 1],  # f2'
     ]
 )
 for c in tss:
     print("===========================")
     print(f"{c.redescribed_schema} ----- \n {c.bubble_indices}")
+
+print()
+print("-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-")
+print()
+tss = sc.schemer(
+    [
+        [2, 1, 0],
+        [0, 1, 2],
+        [1, 2, 0],
+        [0, 2, 1],
+    ]
+)
+for c in tss:
+    print("===========================")
+    print(f"{c.redescribed_schema} ----- \n {c.bubble_indices}")
+
+print()
+print("-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-=-")
+print()
+tss = sc.schemer(
+    [
+        [2, 1, 0],
+        [0, 2, 1],
+        [1, 2, 0],
+        [0, 1, 2],
+    ]
+)
+for c in tss:
+    print("===========================")
+    print(f"{c.redescribed_schema} ----- \n {c.bubble_indices}")
```

### Comparing `schematodes-0.1.0/scratch.txt` & `schematodes-0.2.0/scratch.txt`

 * *Files identical despite different names*

### Comparing `schematodes-0.1.0/src/lib.rs` & `schematodes-0.2.0/src/lib.rs`

 * *Files 13% similar despite different names*

```diff
@@ -80,118 +80,150 @@
             redescribed_schema: one_symbol_schema.to_vec(),
             bubble_indices: vec![],
             signature,
         };
         return vec![lone_schema];
     }
     // the members of the one_symbol_schema are hashed so that we can easily check whether a permutation of a schema maintains closure
-    let one_symbol_schema_hash: HashSet<&Vec<u8>> = HashSet::<_>::from_iter(one_symbol_schema);
+    let one_symbol_schema_hash: HashSet<Vec<u8>> =
+        HashSet::<_>::from_iter(one_symbol_schema.clone());
 
     // Find the nontrivial columns of the one_symbol_schema; trivial columns are those for which all symbols are the same
     let n_cols = one_symbol_schema[0].len();
     let nontrivial_columns: Vec<usize> = (0..n_cols)
         .filter(|i| {
             one_symbol_schema
                 .iter()
                 .any(|x| x[*i] != one_symbol_schema[0][*i])
         })
         .collect();
 
     // initialize the two-symbol schema vector that we will eventually return
-    let mut sym: Vec<TwoSymbolSchemata> = vec![];
+    let mut sym: HashSet<TwoSymbolSchemata> = HashSet::new();
 
     // every one-symbol schemata must eventually be covered by a two symbol schemata
     let mut uncovered_schema: BTreeSet<&Vec<u8>> = BTreeSet::from_iter(one_symbol_schema);
     while !uncovered_schema.is_empty() {
         // the schemata `root` corresponds to the representative of the two-symbol schemata that will generate on this iteration of the loop
         let root = uncovered_schema.pop_last().unwrap();
-
         // a transposition is a candidate if
         // 1. it maps root to a different element of the one_symbol_schema OR
         // 2. it transposes nontrivial columns that leave root invariant.
         // condition 1:
-        let mut swap_candidates: Vec<Vec<usize>> = one_symbol_schema
+        let mut swap_candidates: HashSet<Vec<usize>> = one_symbol_schema
             .iter()
             .map(|x| differing_indices(root, x, Some(2)))
             .filter(|y| y.len() == 2)
             .collect();
         // condition 2:
         for pair in nontrivial_columns.iter().combinations(2) {
             let i = *pair[0];
             let j = *pair[1];
             if root[i] == root[j] {
-                swap_candidates.push(vec![i, j]);
+                swap_candidates.insert(vec![i, j]);
             }
         }
 
-        // Now we start looking for an inclusion-maximal product of symmetric groups that can act on root while maintaining closure.
-        // The trivial group acting on root is the trivial case; we will expand from there.
-        let mut redescribed_schema: HashSet<Vec<u8>> = HashSet::new();
-        redescribed_schema.insert(root.clone());
-        let mut merged_swaps: Vec<HashSet<usize>> = (0..root.len())
-            .map(|ind| HashSet::from_iter(ind..ind + 1))
-            .collect();
-        // Iterate through the candidate swaps and merge them in order if they keeps the merged set in the one_symbol_schema set.
-        for y in swap_candidates {
-            // this iter,map,collect chain applies the swap to everything we have added so far
-            let swapped_schema: HashSet<Vec<u8>> = redescribed_schema
-                .iter()
-                .map(|g| {
-                    let mut gs = g.clone();
-                    gs.swap(y[0], y[1]);
-                    gs
-                })
+        // We iterate over all combinations of swaps, from most to least to find the inclusion-maximal ones that work
+        let mut good_swaps: Vec<HashSet<Vec<usize>>> = Vec::new();
+        for skipped_swaps in swap_candidates.iter().powerset() {
+            let mut swaps = swap_candidates.clone();
+            swaps.retain(|x| !skipped_swaps.contains(&x));
+
+            if good_swaps.iter().any(|x| swaps.is_subset(x)) {
+                continue;
+            }
+
+            // Now we start looking for an inclusion-maximal product of symmetric groups that can act on root while maintaining closure.
+            let mut redescribed_schema: HashSet<Vec<u8>> = HashSet::new();
+            redescribed_schema.insert(root.clone());
+            let mut merged_swaps: Vec<HashSet<usize>> = (0..root.len())
+                .map(|ind| HashSet::from_iter(ind..ind + 1))
                 .collect();
 
-            // check if the swap maps redescribed_schema into the one_symbol_schema set;
-            // if so, add this image to the redscribed_schema and record the swapped indices.
-            if swapped_schema
-                .iter()
-                .all(|g| one_symbol_schema_hash.contains(&g))
-            {
-                redescribed_schema.extend(swapped_schema);
-                uncovered_schema.retain(|&g| !redescribed_schema.contains(g));
-                merged_swaps[y[0]].insert(y[1]);
-                merged_swaps[y[1]].insert(y[0]);
+            // This section applies the transfomrations to the root iteratively until no new schema are reached
+            let mut old_size = 0;
+            let mut closed = true;
+            while old_size != redescribed_schema.len() {
+                old_size = redescribed_schema.len();
+                for swap in swaps.iter() {
+                    merged_swaps[swap[0]].insert(swap[1]);
+                    merged_swaps[swap[1]].insert(swap[0]);
+                    let new_schema: HashSet<Vec<u8>> = redescribed_schema
+                        .iter()
+                        .map(|g| {
+                            let mut gs = g.clone();
+                            gs.swap(swap[0], swap[1]);
+                            gs
+                        })
+                        .collect();
+                    redescribed_schema.extend(new_schema.iter().cloned());
+                }
+                if !redescribed_schema.is_subset(&one_symbol_schema_hash) {
+                    closed = false;
+                    break;
+                }
             }
-        }
-        // record the columns of the redescribed schema that are not the same in this subset
-        let nontrivial_redescription_columns: Vec<usize> = (0..n_cols)
-            .filter(|i| redescribed_schema.iter().any(|x| x[*i] != root[*i]))
-            .collect();
 
-        // finally, convert the transpoitions to bubble indices
-        let mut bubble_indices: Vec<Vec<usize>> = vec![];
-        let mut seen_inds: HashSet<usize> = HashSet::new();
-        for (i, x) in merged_swaps.iter().enumerate() {
-            if seen_inds.contains(&i) {
-                // avoid duplicates
+            // if we leave the input set, the set of swaps does not form a group action on our input set of one-symbol schema
+            if !closed || !redescribed_schema.is_subset(&one_symbol_schema_hash) {
                 continue;
             }
-            if x.iter() // only consider transpositions that map to nontrivial columns, i.e., we are not doing same-symbol symmetry here
-                .any(|&x| !nontrivial_redescription_columns.contains(&x))
-            {
+
+            // record the columns of the redescribed schema that are not the same in this subset
+            let trivial_redescription_columns: Vec<usize> = (0..n_cols)
+                .filter(|i| redescribed_schema.iter().all(|x| x[*i] == root[*i]))
+                .collect();
+
+            // we skip the swaps that include trivial columns because these are not faithful group actions
+            if swaps.iter().any(|swap| {
+                swap.iter()
+                    .any(|x| trivial_redescription_columns.contains(x))
+            }) {
                 continue;
             }
-            seen_inds.extend(x);
 
-            let mut xv: Vec<usize> = x.iter().cloned().collect(); // cana expects a list of bubble indices, so we convert to vec here
-            if xv.len() > 1 {
-                xv.sort_unstable(); // we use unstable sort because we don't have duplicates, and even if we did, we wouldn't care if they got swapped
-                bubble_indices.push(xv);
+            // if we found a good swap, record it so that we don't spend resources on its subsets
+            good_swaps.push(swaps.clone());
+
+            // finally, convert the transpoitions to bubble indices
+            let mut bubble_indices: Vec<Vec<usize>> = vec![];
+            let mut seen_inds: HashSet<usize> = HashSet::new();
+            for (i, x) in merged_swaps.iter().enumerate() {
+                if seen_inds.contains(&i) {
+                    // avoid duplicates
+                    continue;
+                }
+                if x.iter() // only consider transpositions that map to nontrivial columns, i.e., we are not doing same-symbol symmetry here
+                    .all(|&x| trivial_redescription_columns.contains(&x))
+                {
+                    continue;
+                }
+                seen_inds.extend(x);
+
+                let mut xv: Vec<usize> = x.iter().cloned().collect(); // cana expects a list of bubble indices, so we convert to vec here
+                if xv.len() > 1 {
+                    xv.sort_unstable(); // we use unstable sort because we don't have duplicates, and even if we did, we wouldn't care if they got swapped
+                    bubble_indices.push(xv);
+                }
             }
+
+            sym.insert(TwoSymbolSchemata {
+                redescribed_schema: redescribed_schema
+                    .iter()
+                    .map(|x| x.to_vec())
+                    .sorted()
+                    .collect(),
+                bubble_indices: bubble_indices.iter().map(|x| x.to_vec()).sorted().collect(),
+                signature,
+            });
         }
-        sym.push(TwoSymbolSchemata {
-            redescribed_schema: redescribed_schema.iter().map(|x| x.to_vec()).collect(),
-            bubble_indices,
-            signature,
-        });
     }
 
-    sym
+    sym.into_iter().collect()
 }
 
 /// Find the indices where the input arrays `x` and `y` differ, and return a vector of the indices.
 /// Optionally, a `break_above parameter` can be provided, which returns early if the number of indices exceeds `break_above`.
 /// This is useful for when we only want to identify arrays that differ by a specific number of entries.
 fn differing_indices(x: &[u8], y: &[u8], break_above: Option<usize>) -> Vec<usize> {
     let mut diff: Vec<usize> = Vec::new();
```

### Comparing `schematodes-0.1.0/stubs/schematodes/__init__.pyi` & `schematodes-0.2.0/schematodes.pyi`

 * *Files identical despite different names*

### Comparing `schematodes-0.1.0/Cargo.lock` & `schematodes-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "schematodes"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "itertools",
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
```

