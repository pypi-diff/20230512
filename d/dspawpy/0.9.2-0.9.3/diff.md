# Comparing `tmp/dspawpy-0.9.2-py3-none-any.whl.zip` & `tmp/dspawpy-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 73004 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/__init__.py
+Zip file size: 72759 bytes, number of entries: 20
+-rw-rw-rw-  2.0 fat       21 b- defN 23-May-11 06:58 dspawpy/__init__.py
 -rw-rw-rw-  2.0 fat    29208 b- defN 23-Apr-25 05:34 dspawpy/plot.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/analysis/__init__.py
--rw-rw-rw-  2.0 fat    24571 b- defN 23-May-06 03:20 dspawpy/analysis/aimdtools.py
+-rw-rw-rw-  2.0 fat    21567 b- defN 23-May-11 06:31 dspawpy/analysis/aimdtools.py
 -rw-rw-rw-  2.0 fat    20152 b- defN 23-Apr-04 06:32 dspawpy/analysis/vacf.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 06:32 dspawpy/diffusion/__init__.py
 -rw-rw-rw-  2.0 fat     3592 b- defN 23-Apr-26 09:25 dspawpy/diffusion/neb.py
 -rw-rw-rw-  2.0 fat    53467 b- defN 23-Apr-26 09:25 dspawpy/diffusion/nebtools.py
 -rw-rw-rw-  2.0 fat    11045 b- defN 23-Apr-25 05:34 dspawpy/diffusion/pathfinder.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-04 08:25 dspawpy/io/__init__.py
--rw-rw-rw-  2.0 fat    52393 b- defN 23-May-06 03:20 dspawpy/io/read.py
+-rw-rw-rw-  2.0 fat    52495 b- defN 23-May-11 06:32 dspawpy/io/read.py
 -rw-rw-rw-  2.0 fat     7721 b- defN 23-Apr-25 05:46 dspawpy/io/read_json.py
--rw-rw-rw-  2.0 fat     8538 b- defN 23-May-06 03:20 dspawpy/io/structure.py
+-rw-rw-rw-  2.0 fat    10343 b- defN 23-May-11 06:32 dspawpy/io/structure.py
 -rw-rw-rw-  2.0 fat    25241 b- defN 23-Apr-26 09:44 dspawpy/io/utils.py
--rw-rw-rw-  2.0 fat    28491 b- defN 23-May-06 03:20 dspawpy/io/write.py
+-rw-rw-rw-  2.0 fat    25401 b- defN 23-May-11 06:32 dspawpy/io/write.py
 -rw-rw-rw-  2.0 fat     1761 b- defN 23-Apr-25 05:51 dspawpy/io/write_json.py
--rw-rw-rw-  2.0 fat     2215 b- defN 23-May-06 03:23 dspawpy-0.9.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 03:23 dspawpy-0.9.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-06 03:23 dspawpy-0.9.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1581 b- defN 23-May-06 03:23 dspawpy-0.9.2.dist-info/RECORD
-20 files, 270076 bytes uncompressed, 70454 bytes compressed:  73.9%
+-rw-rw-rw-  2.0 fat     2496 b- defN 23-May-12 08:40 dspawpy-0.9.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-12 08:40 dspawpy-0.9.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-12 08:40 dspawpy-0.9.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1583 b- defN 23-May-12 08:40 dspawpy-0.9.3.dist-info/RECORD
+20 files, 266193 bytes uncompressed, 70209 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: dspawpy/io/write.py
 Comment: 
 
 Filename: dspawpy/io/write_json.py
 Comment: 
 
-Filename: dspawpy-0.9.2.dist-info/METADATA
+Filename: dspawpy-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: dspawpy-0.9.2.dist-info/WHEEL
+Filename: dspawpy-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: dspawpy-0.9.2.dist-info/top_level.txt
+Filename: dspawpy-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: dspawpy-0.9.2.dist-info/RECORD
+Filename: dspawpy-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dspawpy/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 5f5f 7665 7273 696f 6e5f 5f20 3d20 2730  __version__ = '0
+00000010: 2e39 2e33 27                             .9.3'
```

## dspawpy/analysis/aimdtools.py

```diff
@@ -121,87 +121,36 @@
 
         self.rmin = rmin
         self.rmax = rmax
         self.ngrid = ngrid
 
         self.dr = (self.rmax - self.rmin) / (self.ngrid - 1)  # end points are on grid
         self.r = np.linspace(self.rmin, self.rmax, self.ngrid)  # type: ignore
+        self.shell_volumes = 4.0 * np.pi * self.r**2 * self.dr
+        self.shell_volumes[self.shell_volumes < 1e-8] = 1e8  # avoid divide by zero
 
-        max_r = self.rmax + self.dr / 2.0  # add a small shell to improve robustness
-
-        print(f"Calculating neighbor lists for {len(self.structures)} structures,")
-        self.neighbor_lists = []
-        for _c, i in enumerate(self.structures):
-            if _c == 0:
-                print("0%...", end="", flush=True)
-            elif _c / len(self.structures) * 100 == 25:
-                print("25%...", end="", flush=True)
-            elif _c / len(self.structures) * 100 == 50:
-                print("50%...", end="", flush=True)
-            elif _c / len(self.structures) * 100 == 75:
-                print("75%...", end="", flush=True)
-            elif _c == len(self.structures) - 1:
-                print("100%")
-            self.neighbor_lists.append(i.get_neighbor_list(max_r))
-
-        # each neighbor list is a tuple of
-        # center_indices, neighbor_indices, image_vectors, distances
-        (
-            self.center_indices,
-            self.neighbor_indices,
-            self.image_vectors,
-            self.distances,  # 完整的距离列表（遍历体系所有原子）
-        ) = list(zip(*self.neighbor_lists))
-
-        elements = np.array([str(i.specie) for i in structures[0]])  # type: ignore
-        self.center_elements = [elements[i] for i in self.center_indices]
-        self.neighbor_elements = [elements[i] for i in self.neighbor_indices]
-        self.density = [{}] * len(self.structures)
-
-        self.natoms = [
-            i.composition.to_data_dict["unit_cell_composition"]
-            for i in self.structures  # 抽成单胞化学式
-        ]  # {'H': 2, 'O': 1} 字典构成的列表
-
-        for s_index, natoms in enumerate(self.natoms):  # s_index是结构序号，natoms是单胞化学式字典
-            for i, j in natoms.items():  # i是元素符号，j是原子个数
-                self.density[s_index][i] = (
-                    j / self.structures[s_index].volume
-                )  # 原子数除以体积
-
-        self.volumes = 4.0 * np.pi * self.r**2 * self.dr  # 分母的一部分
-        self.volumes[self.volumes < 1e-8] = 1e8  # avoid divide by zero
         self.n_structures = len(self.structures)
         self.sigma = np.ceil(sigma / self.dr)
 
     def _dist_to_counts(self, d):
         """Convert a distance array for counts in the bin
 
         Parameter
         ---------
             d: (1D np.array)
 
         Returns:
             1D array of counts in the bins centered on self.r
         """
-        # print(len(d))
-        # print(f'{d=}\n')
         counts = np.zeros((self.ngrid,))
         indices = np.array(
             np.floor((d - self.rmin + 0.5 * self.dr) / self.dr), dtype=int
         )  # 将找到配对的距离转换为格点序号 (向下取整)
-        # print(len(indices))
-        # print(f'{indices=}\n')
-        # 取整操作，导致格点序号很可能重复，因此需要统计每个格点序号出现的次数并去重
         unique, val_counts = np.unique(indices, return_counts=True)
-        # print(len(unique))
-        # print(f'{unique=}\n')
         counts[unique] = val_counts
-        # print(f'{counts=}\n')
-        # raise IndexError
         return counts
 
     def get_rdf(
         self,
         ref_species: Union[str, List[str]],
         species: Union[str, List[str]],
         is_average=True,
@@ -219,70 +168,62 @@
 
         Returns
         -------
         (x, rdf)
             x is the radial points, and rdf is the rdf value.
         """
         print("Calculating RDF...")
+        if isinstance(ref_species, str):
+            ref_species = [ref_species]
+
+        if isinstance(species, str):
+            species = [species]
+        ref_species_index = []
+        species_index = []
+        for i in range(len(self.structures[0].species)):
+            ele = str(self.structures[0].species[i])
+            if ele in ref_species:
+                ref_species_index.append(i)
+            elif ele in species:
+                species_index.append(i)
         all_rdfs = [
-            self.get_one_rdf(ref_species, species, i)[1]
+            self.get_one_rdf(ref_species_index, species_index, i)[1]
             for i in range(self.n_structures)
         ]
         if is_average:
             all_rdfs = np.mean(all_rdfs, axis=0)
         return self.r, all_rdfs
 
     def get_one_rdf(
         self,
-        ref_species: Union[str, List[str]],
-        species: Union[str, List[str]],
+        ref_species_index: Union[str, List[str]],
+        species_index: Union[str, List[str]],
         index=0,
     ):
         """Get the RDF for one structure, indicated by the index of the structure
-        in all structures
-
-        Parameter
-        ---------
-        ref_species (list of species or just single specie str):
-            the reference species. The rdfs are calculated with these species at the center
-        species (list of species or just single specie str):
-            the species that we are interested in. The rdfs are calculated on these species.
-        index (int):
-            structure index in the list
+        in all structures"""
+        lattice = self.structures[index].lattice
+        distances = []
+        refsp_frac_coord = self.structures[index].frac_coords[ref_species_index]
+        sp_frac_coord = self.structures[index].frac_coords[species_index]
+        d = lattice.get_all_distances(refsp_frac_coord, sp_frac_coord)
+        indices = (
+            (d >= self.rmin - self.dr / 2.0)
+            & (d <= self.rmax + self.dr / 2.0)
+            & (d > 1e-8)
+        )
+        distances = d[indices]
+        counts = self._dist_to_counts(np.array(distances))  # 统计该距离内目标元素的原子数，列表
 
-        Returns
-        -------
-            (x, rdf) x is the radial points, and rdf is the rdf value.
-        """
-        if isinstance(ref_species, str):
-            ref_species = [ref_species]
+        npairs = len(distances)
+        rdf_temp = counts / npairs / self.shell_volumes / self.structures[index].volume
 
-        if isinstance(species, str):
-            species = [species]
-        # print(f'{len(self.center_elements[index])=}')
-        indices = (  # 须同时满足下列条件
-            (np.isin(self.center_elements[index], ref_species))
-            & (np.isin(self.neighbor_elements[index], species))
-            & (self.distances[index] >= self.rmin - self.dr / 2.0)
-            & (self.distances[index] <= self.rmax + self.dr / 2.0)
-            & (self.distances[index] > 1e-8)
-        )
-        # print(f'{len(indices)=}')
-        # raise ValueError
-        # print(f'{indices=}\n')
-        density = sum(self.density[index][i] for i in species)  # 目标元素的原子数密度，单浮点数
-        natoms = sum(self.natoms[index][i] for i in ref_species)  # 中心元素的原子总数，单整数
-        distances = self.distances[index][indices]  # 针对每个中心原子，目标元素的距离列表
-        counts = self._dist_to_counts(distances)  # 统计该距离内目标元素的原子数，列表
-        rdf_temp = (
-            counts / density / self.volumes / natoms
-        )  # counts包含了所有中心元素(ref_species)对应的原子的信息，因此需要除以中心原子总数
         if self.sigma > 1e-8:
             rdf_temp = gaussian_filter1d(rdf_temp, self.sigma)
-        return self.r, rdf_temp
+        return self.r, rdf_temp, npairs
 
     def get_coordination_number(self, ref_species, species, is_average=True):
         """returns running coordination number
 
         Parameter
         ---------
         ref_species (list of species or just single specie str):
```

## dspawpy/io/read.py

```diff
@@ -311,26 +311,26 @@
         densities = dos["DosInfo"]["Spin1"]["Dos"]
     else:
         raise TypeError(f"{os.path.abspath(phonon_dos_dir)} must be h5 or json file")
 
     return PhononDos(frequencies, densities)
 
 
-def get_sinfo(datafile: str, scaled=False, index=None, ele=None, ai=None):
+def get_sinfo(datafile: str, scaled=False, si=None, ele=None, ai=None):
     """Wrapper to get structure information from h5/json/as file.
 
     从datafile中读取结构信息
 
     Parameters
     ----------
     datafile : str
         h5 / json 文件路径
     scaled : bool, optional
         是否返回分数坐标，默认False
-    index : int or list or str, optional
+    si : int or list or str, optional
         运动轨迹中的第几步，从1开始计数！
         如果要切片，用字符串写法： '1, 10'
         默认为None，返回所有步
     ele : list, optional
         元素列表, Natom x 1
         默认为None，从h5文件中读取
     ai : int or list or str, optional
@@ -372,23 +372,23 @@
         # decide task type by check the internal key
         if "/Structures" in hf.keys():  # multi-steps
             Total_step = np.array(hf.get("/Structures/FinalStep"))[0]  # 总步数
 
             if ele is not None and ai is not None:
                 raise ValueError("暂不支持同时指定元素和原子序号")
             # 步数
-            if index is not None:
-                if isinstance(index, int):  # 1
-                    indices = [index]
+            if si is not None:
+                if isinstance(si, int):  # 1
+                    indices = [si]
 
-                elif isinstance(index, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-                    indices = index
+                elif isinstance(si, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                    indices = si
 
-                elif isinstance(index, str):  # ':', '-3:'
-                    indices = __parse_indices(index, Total_step)
+                elif isinstance(si, str):  # ':', '-3:'
+                    indices = __parse_indices(si, Total_step)
 
                 else:
                     raise ValueError("请输入正确格式的index")
 
                 Nstep = len(indices)
             else:
                 Nstep = Total_step
@@ -520,15 +520,15 @@
                     "Fix_y": atomFixs[:, :, 1],
                     "Fix_z": atomFixs[:, :, 2],
                     "LatticeFixs": latticeFixs,
                 }
 
             if scaled:  # Fractional coordinates
                 for k, ind in enumerate(indices):  # 步数
-                    for j, sli in enumerate(location):  # atom index
+                    for j, sli in enumerate(location):  # atom si
                         poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], np.eye(3, 3))
             else:  # Cartesian coordinates
                 for k, ind in enumerate(indices):  # 步数
                     for j, sli in enumerate(location):
                         poses[k, j, :] = np.dot(wrapped_poses[k, :, sli], lats)
 
         elif "/UnrelaxStructure" in hf.keys():  # single-step
@@ -578,23 +578,23 @@
                 Total_step = len(data["Structures"])  # aimd.json
             else:
                 Total_step = len(data)  # relax.json, neb01.json
 
             if ele is not None and ai is not None:
                 raise ValueError("暂不支持同时指定元素和原子序号")
             # 步数
-            if index is not None:
-                if isinstance(index, int):  # 1
-                    indices = [index]
+            if si is not None:
+                if isinstance(si, int):  # 1
+                    indices = [si]
 
-                elif isinstance(index, list) or isinstance(ai, np.ndarray):  # [1,2,3]
-                    indices = index
+                elif isinstance(si, list) or isinstance(ai, np.ndarray):  # [1,2,3]
+                    indices = si
 
-                elif isinstance(index, str):  # ':', '-3:'
-                    indices = __parse_indices(index, Total_step)
+                elif isinstance(si, str):  # ':', '-3:'
+                    indices = __parse_indices(si, Total_step)
 
                 else:
                     raise ValueError("请输入正确格式的index")
 
                 Nstep = len(indices)
             else:
                 Nstep = Total_step
@@ -665,15 +665,18 @@
 
             if "Structures" in data:  # aimd
                 for i, ind in enumerate(indices):  # for every ionic step
                     lat = data["Structures"][ind - 1]["Lattice"]
                     lattices[i] = np.array(lat).reshape(3, 3)
                     mag_for_each_step = []
                     fix_for_each_step = []
-                    fixlat_raw = data["Structures"][ind - 1]["FixLattice"]
+                    if "FixLattice" in data["Structures"][ind - 1]:
+                        fixlat_raw = data["Structures"][ind - 1]["FixLattice"]
+                    else:
+                        fixlat_raw = []
                     if fixlat_raw == []:
                         fixlat_raw = np.full((9, 1), fill_value=False).tolist()
                     fixlat_str = [
                         "True" if _v == True else "False" for _v in fixlat_raw
                     ]
                     fixlat_arr = np.array(fixlat_str).reshape(9, 1)
                     # repeat fixlat for each atom
@@ -692,15 +695,15 @@
                         if fix_for_each_atom == []:
                             fix_for_each_atom = ["False"]
                         fix_for_each_step.append(fix_for_each_atom)
 
                     mags.append(mag_for_each_step)
                     Atomfixs.append(fix_for_each_step)
                     if not scaled:
-                        poses = np.dot(poses, lattices[i])
+                        poses[i] = np.dot(poses[i], lattices[i])
 
             else:  # relax, neb01
                 print(
                     "Warning: mag and fix info are not available for relax.json and nebXX.json yet, trying read info..."
                 )
 
                 for i, ind in enumerate(indices):  # for every ionic step
@@ -732,15 +735,15 @@
                         if fix_for_each_atom == []:
                             fix_for_each_atom = ["False"]
                         fix_for_each_step.append(fix_for_each_atom)
 
                     mags.append(mag_for_each_step)
                     Atomfixs.append(fix_for_each_step)
                     if not scaled:
-                        poses = np.dot(poses, lattices[i])
+                        poses[i] = np.dot(poses[i], lattices[i])
 
             elements = elements.tolist()
             Mags = np.array(mags).tolist()  # (Nstep, Natom, ?) or (Nstep, 0,)
 
             D_mag_fix = {"Mag": Mags, "Fix": Atomfixs, "LatticeFixs": LatFixs}
 
     else:
```

## dspawpy/io/structure.py

```diff
@@ -7,61 +7,101 @@
 import numpy as np
 from pymatgen.core import Structure
 
 from dspawpy.io.read import get_lines_without_comment, get_sinfo
 
 
 def build_Structures_from_datafile(
-    datafile: Union[str, List[str]], scaled=False, index=None, ele=None, ai=None
+    datafile: Union[str, List[str]], si=None, ele=None, ai=None
 ) -> List[Structure]:
-    """读取一/多个h5/json文件，返回pymatgen的Structures列表
+    r"""读取一/多个h5/json文件，返回pymatgen的Structures列表
 
     Parameters
     ----------
-    datafile : 字符串或字符串列表
-        h5/json/as/hzw文件路径；若给定字符串列表，将依次读取数据并合并成一个Structures列表
+    datafile : str or list
+        - h5/json/as/hzw/cif/poscar/cssr/xsf/mcsqs/prismatic/yaml/fleur-inpgen文件路径;
+        - 若给定字符串列表，将依次读取数据并合并成一个Structures列表
+        - 文件类型依据后缀名判断，请勿使用不规范的后缀名
+    si: int, list or str
+        构型编号，从 1 开始
+        - si=1, 读取第一个构型
+        - si=[1,2], 读取第一个和第二个构型
+        - si=':', 读取所有构型
+        - si='-3:', 读取最后三个构型
+    ele: str or list
+        元素符号，如['H','O']
+    ai: int or list
+        原子编号，从 1 开始，用法同si
 
     Returns
     -------
-    List[Structure] : pymatgen structures 列表
+    List[Structure] : pymatgen Structures 列表
 
     Examples
     --------
+
     >>> from dspawpy.io.structure import build_Structures_from_datafile
-    # 读取单个文件
-    >>> pymatgen_Structures = build_Structures_from_datafile(datafile='aimd1.h5')
-    # 当datafile为列表时，将依次读取多个文件，合并成一个Structures列表
+
+    读取单个文件生成 Structures 列表，目前支持 h5/json/as/hzw/cif/poscar/cssr/xsf/mcsqs/prismatic/yaml/fleur-inpgen 格式，文件格式根据后缀名判断，请勿使用不规范的后缀名
+
+    >>> pymatgen_Structures = build_Structures_from_datafile(datafile='relax.h5')
+    Reading E:\Dev\dspawpy\test\relax.h5 ...
+    >>> pymatgen_Structures
+    [Structure Summary
+    Lattice
+        abc : 3.2024004097211822 3.20240519054306 18.40999985
+    angles : 90.0 90.0 119.99975020767022
+    volume : 163.50740406185463
+        A : 3.2024004097211822 0.0 0.0
+        B : -1.6011905042240808 2.773371228955793 0.0
+        C : 0.0 0.0 18.40999985
+        pbc : True True True
+    PeriodicSite: Mo (1.5977, 0.9224, 9.2050) [0.6652, 0.3326, 0.5000]
+    ...
+    PeriodicSite: S (1.5977, 2.7673, 10.7755) [1.0000, 1.0000, 0.5853]]
+
+    注意pymatgen_Structures是由多个 Structure 对象组成的列表，每个 Structure 对象分别对应一个构型。如果只有一个构型，也会返回列表，请使用 pymatgen_Structures[0] 获取 Structure 对象
+
+    当datafile为列表时，将依次读取多个文件，合并成一个Structures列表
+
     >>> pymatgen_Structures = build_Structures_from_datafile(datafile=['aimd1.h5','aimd2.h5'])
     """
     dfs = []
     if isinstance(datafile, list):  # 续算模式，给的是多个文件
         dfs = datafile
     else:  # 单次计算模式，处理单个文件
-        if (
-            datafile.endswith(".h5")
-            or datafile.endswith(".json")
-            or datafile.endswith(".as")
-        ):
+        if datafile.split(".")[-1] in [
+            "h5",
+            "json",
+            "as",
+            "hzw",
+            "cif",
+            "poscar",
+            "cssr",
+            "xsf",
+            "mcsqs",
+            "prismatic",
+            "yaml",
+            "fleur-inpgen",
+        ]:
             df = datafile
         else:
-            raise FileNotFoundError("未找到h5或json文件！")
+            raise NotImplementedError(f"{datafile}文件类型暂时无法读取")
         dfs.append(df)
 
     # 读取结构数据
     pymatgen_Structures = []
     for df in dfs:
-        structure_list = _get_structure_list(df, scaled, index, ele, ai)
+        structure_list = _get_structure_list(df, si, ele, ai)
         pymatgen_Structures.extend(structure_list)
 
     return pymatgen_Structures
 
 
-def _get_structure_list(
-    df: str, scaled=False, index=None, ele=None, ai=None
-) -> List[Structure]:
+def _get_structure_list(df: str, si=None, ele=None, ai=None) -> List[Structure]:
     """get pymatgen structures from single datafile
 
     Parameters
     ----------
     df : str
         datafile
 
@@ -72,47 +112,56 @@
     Examples
     --------
     >>> from dspawpy.analysis.aimdtools import get_structure_list
     >>> structure_list = get_structure_list(df='aimd.h5')
     """
 
     # create Structure structure_list from aimd.h5
-    if df.endswith(".as"):
+    fmt = df.split(".")[-1]
+    if fmt == "as":
         strs = [_from_dspaw_as(df)]
-    elif df.endswith(".hzw"):
+    elif fmt == "hzw":
         print("build from hzw file may lack mag & fix info!")
         strs = [_from_hzw(df)]
+    elif fmt in [
+        "cif",
+        "poscar",
+        "cssr",
+        "xsf",
+        "mcsqs",
+        "prismatic",
+        "yaml",
+        "fleur-inpgen",
+    ]:
+        strs = [Structure.from_file(df)]
     else:
-        assert df.endswith(".h5") or df.endswith(
-            ".json"
-        ), "datafile must be h5/json/as/hzw file!"
+        assert df.endswith(".h5") or df.endswith(".json"), "expecting h5/json file"
 
         Nstep, elements, positions, lattices, D_mag_fix = get_sinfo(
-            df, scaled, index, ele, ai
-        )
-        icart = 0 if scaled else 1  # 0: scaled, 1: cartesian
+            datafile=df, si=si, ele=ele, ai=ai
+        )  # returned positions, not scaled-positions
         strs = []
         for i in range(Nstep):
             if D_mag_fix:
                 strs.append(
                     Structure(
                         lattices[i],
                         elements,
                         positions[i],
-                        coords_are_cartesian=icart,
+                        coords_are_cartesian=True,
                         site_properties={k: v[i] for k, v in D_mag_fix.items()},
                     )
                 )
             else:
                 strs.append(
                     Structure(
                         lattices[i],
                         elements,
                         positions[i],
-                        coords_are_cartesian=icart,
+                        coords_are_cartesian=True,
                     )
                 )
     return strs
 
 
 def _from_dspaw_as(as_file: str = "structure.as") -> Structure:
     """从DSPAW的as结构文件中读取结构信息
```

## dspawpy/io/write.py

```diff
@@ -3,233 +3,128 @@
 """
 
 import json
 import os
 
 import numpy as np
 
-from dspawpy.io.read import _get_lammps_non_orthogonal_box, get_sinfo, load_h5
+from dspawpy.io.read import _get_lammps_non_orthogonal_box, load_h5
 
 
-def write_xyz_traj(
-    datafile="aimd.h5",
-    ai=None,
-    ele=None,
-    index=None,
+def _write_xyz_traj(
+    structures,
     xyzfile="aimdTraj.xyz",
-    icombine=False,
 ):
     r"""保存xyz格式的轨迹文件
 
     Parameters
     ----------
-    datafile : str or list
-        DSPAW计算完成后保存的h5/json文件或包含它们的文件夹路径
-    ai : int
-        原子编号列表（体系中的第几号原子，不是质子数）
-    ele : str
-        元素，例如 'C'，'H'，'O'，'N'
-    index : int
-        优化过程中的第几步
+    structures: list
+        pymatgen的Structures列表
     xyzfile : str
         写入xyz格式的轨迹文件，默认为aimdTraj.xyz
-    icombine : bool
-        是否将多个文件合并为一个文件，默认为False
 
     Example
     -------
     >>> from dspawpy.io.write import write_xyz_traj
     >>> write_xyz_traj(datafile='aimd.h5', ai=[1,2,3], index=1, xyzfile='aimdTraj.xyz')
     Reading E:\Dev\dspawpy\test\new\aimd.h5 ...
     """
-    if isinstance(datafile, list):
-        dfs = datafile
-    elif isinstance(datafile, str):
-        dfs = [datafile]
-    else:
-        raise TypeError("datafile must be a str or a list of str!")
-
-    xyzs = []
-    for i, df in enumerate(dfs):
-        if len(dfs) == 1:
-            xyzfilename = xyzfile
-        else:
-            xyzfilename = str(i + 1) + xyzfile
-        xyzs.append(xyzfilename)
-
-        # search df in the given directory
-        if os.path.isdir(df):
-            directory = df  # specified df is actually a directory
-            print("您指定了一个文件夹，正在查找相关h5或json文件...")
-            if os.path.exists(os.path.join(directory, "aimd.h5")):
-                df = os.path.join(directory, "aimd.h5")
-                print("Reading aimd.h5...")
-            elif os.path.exists(os.path.join(directory, "aimd.json")):
-                df = os.path.join(directory, "aimd.json")
-                print("Reading aimd.json...")
-            else:
-                raise FileNotFoundError("未找到aimd.h5/aimd.json文件！")
-
-        if df.endswith(".h5") or df.endswith(".json"):
-            Nstep, eles, poses, lats, D_mag_fix = get_sinfo(
-                datafile=df, scaled=True, index=index, ele=ele, ai=ai
+    if not isinstance(structures, list):  # single Structure
+        structures = [structures]
+    with open(xyzfile, "w") as f:
+        # Nstep
+        for _, structure in enumerate(structures):
+            # 原子数不会变，就是不合并的元素总数
+            eles = [s.species_string for s in structure.sites]
+            f.write("%d\n" % len(eles))
+            # lattice
+            lm = structure.lattice.matrix
+            f.write(
+                'Lattice="%f %f %f %f %f %f %f %f %f" Properties=species:S:1:pos:R:3 pbc="T T T"\n'
+                % (
+                    lm[0, 0],
+                    lm[0, 1],
+                    lm[0, 2],
+                    lm[1, 0],
+                    lm[1, 1],
+                    lm[1, 2],
+                    lm[2, 0],
+                    lm[2, 1],
+                    lm[2, 2],
+                )
             )
-        else:
-            raise TypeError("write_xyz_traj 仅支持读取h5或json文件！")
-
-        # 写入文件
-        with open(xyzfilename, "w") as f:
-            # Nstep
-            for n in range(Nstep):
-                # 原子数不会变，就是不合并的元素总数
-                f.write("%d\n" % len(eles))
-                # lattice
+            # position and element
+            poses = structure.cart_coords
+            for j in range(len(eles)):
                 f.write(
-                    'Lattice="%f %f %f %f %f %f %f %f %f" Properties=species:S:1:pos:R:3 pbc="T T T"\n'
-                    % (
-                        lats[n, 0, 0],
-                        lats[n, 0, 1],
-                        lats[n, 0, 2],
-                        lats[n, 1, 0],
-                        lats[n, 1, 1],
-                        lats[n, 1, 2],
-                        lats[n, 2, 0],
-                        lats[n, 2, 1],
-                        lats[n, 2, 2],
-                    )
+                    "%s %f %f %f\n" % (eles[j], poses[j, 0], poses[j, 1], poses[j, 2])
                 )
-                # position and element
-                for j in range(len(eles)):
-                    f.write(
-                        "%s %f %f %f\n"
-                        % (eles[j], poses[n, j, 0], poses[n, j, 1], poses[n, j, 2])
-                    )
-        print(f"{xyzfilename} 文件已保存！")
 
-    if icombine and isinstance(datafile, list):
-        # combine xyz by calling python internal utility
-        lines = []
-        for xyzFile in xyzs:
-            with open(xyzFile, "r") as f:
-                lines.extend(f.readlines())
-        with open(f"total_{xyzFile}", "w") as f:
-            f.writelines(lines)
-
-        print(f"total_{xyzfile} 文件已保存！")
-
-
-def write_dump_traj(
-    datafile="aimd.h5",
-    ai=None,
-    ele=None,
-    index=None,
+    print(f"{xyzfile} 文件已保存！")
+
+
+def _write_dump_traj(
+    structures,
     dumpfile="aimdTraj.dump",
-    icombine=False,
 ):
     r"""保存为lammps的dump格式的轨迹文件，暂时只支持正交晶胞
 
     Parameters
     ----------
-    datafile : str or list
-        DSPAW计算完成后保存的h5/json文件或包含它们的文件夹路径
-    ai : int
-        原子编号列表（体系中的第几号原子，不是质子数）
-    ele : str
-        元素，例如 'C'，'H'，'O'，'N'
-    index : int
-        优化过程中的第几步
+    structures: list
+        pymatgen的Structures列表
     dumpfile : str
         dump格式的轨迹文件名，默认为aimdTraj.dump
-    icombine : bool
-        是否将多个文件合并为一个文件，默认为False
 
     Example
     -------
     >>> from dspawpy.io.write import write_dump_traj
     >>> write_dump_traj(datafile='aimd.h5', ai=[1,2,3], index=1, dumpfile='aimdTraj.dump')
     Reading E:\Dev\dspawpy\test\new\aimd.h5 ...
     """
-    if isinstance(datafile, list):
-        dfs = datafile
-    elif isinstance(datafile, str):
-        dfs = [datafile]
-    else:
-        raise TypeError("datafile must be a str or a list of str!")
-
-    dumps = []
-    for i, df in enumerate(dfs):
-        if len(dfs) == 1:
-            dumpfilename = dumpfile
-        else:
-            dumpfilename = str(i + 1) + dumpfile
-        dumps.append(dumpfilename)
-
-        # search df in the given directory
-        if os.path.isdir(df):
-            directory = df  # specified df is actually a directory
-            print("您指定了一个文件夹，正在查找相关h5或json文件...")
-            if os.path.exists(os.path.join(directory, "aimd.h5")):
-                df = os.path.join(directory, "aimd.h5")
-                print("Reading aimd.h5...")
-            elif os.path.exists(os.path.join(directory, "aimd.json")):
-                df = os.path.join(directory, "aimd.json")
-                print("Reading aimd.json...")
-            else:
-                raise FileNotFoundError("未找到aimd.h5/aimd.json文件！")
-
-        if df.endswith(".h5") or df.endswith(".json"):
-            Nstep, eles, poses, lats, D_mag_fix = get_sinfo(df, index, ele, ai)
-        else:
-            raise TypeError("write_dump_traj 仅支持读取h5或json文件！")
-
-        # 写入文件
-        with open(dumpfilename, "w") as f:
-            for n in range(Nstep):
-                box_bounds = _get_lammps_non_orthogonal_box(lats[n])
-                f.write("ITEM: TIMESTEP\n%d\n" % n)
-                f.write("ITEM: NUMBER OF ATOMS\n%d\n" % (len(eles)))
-                f.write("ITEM: BOX BOUNDS xy xz yz xx yy zz\n")
+    if not isinstance(structures, list):  # single Structure
+        structures = [structures]
+    with open(dumpfile, "w") as f:
+        for n, structure in enumerate(structures):
+            lat = structure.lattice.matrix
+            eles = [s.species_string for s in structure.sites]
+            poses = structure.cart_coords
+
+            box_bounds = _get_lammps_non_orthogonal_box(lat)
+            f.write("ITEM: TIMESTEP\n%d\n" % n)
+            f.write("ITEM: NUMBER OF ATOMS\n%d\n" % (len(eles)))
+            f.write("ITEM: BOX BOUNDS xy xz yz xx yy zz\n")
+            f.write(
+                "%f %f %f\n%f %f %f\n %f %f %f\n"
+                % (
+                    box_bounds[0][0],
+                    box_bounds[0][1],
+                    box_bounds[0][2],
+                    box_bounds[1][0],
+                    box_bounds[1][1],
+                    box_bounds[1][2],
+                    box_bounds[2][0],
+                    box_bounds[2][1],
+                    box_bounds[2][2],
+                )
+            )
+            f.write("ITEM: ATOMS type x y z id\n")
+            for i in range(len(eles)):
                 f.write(
-                    "%f %f %f\n%f %f %f\n %f %f %f\n"
+                    "%s %f %f %f %d\n"
                     % (
-                        box_bounds[0][0],
-                        box_bounds[0][1],
-                        box_bounds[0][2],
-                        box_bounds[1][0],
-                        box_bounds[1][1],
-                        box_bounds[1][2],
-                        box_bounds[2][0],
-                        box_bounds[2][1],
-                        box_bounds[2][2],
+                        eles[i],
+                        poses[i, 0],
+                        poses[i, 1],
+                        poses[i, 2],
+                        i + 1,
                     )
                 )
-                f.write("ITEM: ATOMS type x y z id\n")
-                for i in range(len(eles)):
-                    f.write(
-                        "%s %f %f %f %d\n"
-                        % (
-                            eles[i],
-                            poses[n, i, 0],
-                            poses[n, i, 1],
-                            poses[n, i, 2],
-                            i + 1,
-                        )
-                    )
-        print(f"{dumpfilename} 文件已保存！")
-
-    if icombine and isinstance(datafile, list):
-        # combine xyz by calling python internal utility
-        lines = []
-        for dumpFile in dumps:
-            with open(dumpFile, "r") as f:
-                lines.extend(f.readlines())
-        with open(f"total_{dumpfile}", "w") as f:
-            f.writelines(lines)
-
-        print(f"total_{dumpfile} 文件已保存！")
+    print(f"{dumpfile} 文件已保存！")
 
 
 def write_VESTA(in_filename: str, data_type, out_filename="DS-PAW.vesta"):
     """从包含电子体系信息的json或h5文件中读取数据并写入VESTA格式的文件中
 
     Parameters
     ----------
@@ -432,17 +327,20 @@
     Parameters
     ----------
     structure : Structure
         pymatgen的Structure对象
     filename : str
         结构文件名
     fmt : str
-        结构文件类型，目前支持 "json","as","hzw","pdb"四种类型
+        - 结构文件类型，目前支持 'json', 'as', 'hzw', 'pdb', 'xyz', 'dump', 'cif', 'poscar', 'cssr', 'xsf', 'mcsqs', 'prismatic', 'yaml', 'fleur-inpgen'
+        - 若不指定，则根据文件名后缀判断
+        - 'pdb', 'xyz' 和 'dump' 支持传入多个结构，structure参数可以是一个Structure对象列表；其他类型的文件只支持传入单个结构
     coords_are_cartesian : bool
-        坐标是否为笛卡尔坐标，默认为True
+        - 是否写作笛卡尔坐标，默认为True；否则写成分数坐标形式
+        - 此选项暂时仅对 as 和 json 格式有效
 
     Examples
     --------
 
     如果不指定 fmt 参数，将尝试根据文件名后缀判断。
 
     如果要生成 as 结构文件（可用于开始新任务），可参考如下命令:
@@ -485,24 +383,43 @@
     >>> to_file(s, filename='PtH.pdb')
     --> 成功写入文件 E:\Dev\dspawpy\test\new\PtH.pdb
     """
 
     if fmt is None:
         fmt = filename.split(".")[-1]
 
-    if fmt == "json":
+    if fmt == "json":  # 单个构型
+        assert not isinstance(structure, list), "只接受单个构型"
         _to_dspaw_json(structure, filename, coords_are_cartesian)
     elif fmt == "as":
+        assert not isinstance(structure, list), "只接受单个构型"
         _to_dspaw_as(structure, filename, coords_are_cartesian)
     elif fmt == "hzw":
+        assert not isinstance(structure, list), "只接受单个构型"
         _to_hzw(structure, filename)
-    elif fmt == "pdb":
+    elif fmt == "pdb":  # 可以是多个构型
         _to_pdb(structure, filename)
+    elif fmt == "xyz":  # 可以是多个构型
+        _write_xyz_traj(structure, filename)
+    elif fmt == "dump":  # 可以是多个构型
+        _write_dump_traj(structure, filename)
+    elif fmt in [
+        "cif",
+        "poscar",
+        "cssr",
+        "xsf",
+        "mcsqs",
+        "prismatic",
+        "yaml",
+        "fleur-inpgen",
+    ]:
+        assert not isinstance(structure, list), "只接受单个构型"
+        structure.to(filename, fmt=fmt)
     else:
-        raise NotImplementedError(f"不支持的文件格式 {fmt}")
+        raise NotImplementedError(f"暂不支持写成 {fmt} 格式")
 
     print(f"--> 成功写入文件 {os.path.abspath(filename)} ")
 
 
 def _write_atoms(fileobj, hdf5):
     fileobj.write("DS-PAW Structure\n")
     fileobj.write("  1.00\n")
```

## Comparing `dspawpy-0.9.2.dist-info/METADATA` & `dspawpy-0.9.3.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspawpy
-Version: 0.9.2
+Version: 0.9.3
 Summary: Tools for dspaw
 Home-page: http://www.hzwtech.com/
 Author: Hzwtech
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Requires-Dist: pymatgen (>=2021.2.8.1)
@@ -27,14 +27,21 @@
 
 再重新用pip安装。
 
 详见 https://stackoverflow.com/questions/75542688/conda-installed-pip-failed-to-find-packages/75542962#75542962
 
 ## 版本更新简述
 
+### 0.9.3
+
+- 新增功能： 接入pymatgen支持的几类结构文件的读写操作
+- 新增功能： 支持通过 `dspawpy.__version__` 查看版本号
+- 重要变更： write_xyz_traj, write_dump_traj 并入 to_file 函数
+- 细节优化： 大幅提高RDF计算效率
+
 ### 0.9.2
 
 - 新增功能： 支持从as文件中解析磁矩和FIX信息
 - 新增功能： 从h5/json文件中读取数据时支持指定读取的离子步（从1开始）
 
 ### 0.9.1
```

## Comparing `dspawpy-0.9.2.dist-info/RECORD` & `dspawpy-0.9.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-dspawpy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+dspawpy/__init__.py,sha256=c60whb_Zk-Ow7zx5khIRULcdxxjoCXM2XCO4tAZztbk,21
 dspawpy/plot.py,sha256=ocLkU08WfMb2fyETrBSSZvxZFSg2sPX8rLusXZLT5BM,29208
 dspawpy/analysis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dspawpy/analysis/aimdtools.py,sha256=9AMUG7Eeesgyj86MDtWDZ9EpsOkJ86cMNFwqpeMUr-M,24571
+dspawpy/analysis/aimdtools.py,sha256=72N58P2EBA5z8EZwaY1W6ab8ZGZVwefQCjME8490HqU,21567
 dspawpy/analysis/vacf.py,sha256=g5IS6Q7QGYa17XBVnYEH-MubGSpkUsDPpMaI_ELacw4,20152
 dspawpy/diffusion/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dspawpy/diffusion/neb.py,sha256=U6J7lSlE_xp1rCON5mgfWWi5DFHVZYVb5xjqLlGxXXI,3592
 dspawpy/diffusion/nebtools.py,sha256=tfQCQPUmZKELz7ImwyiJiiFfXahC9U3doarExspL-DU,53467
 dspawpy/diffusion/pathfinder.py,sha256=HhCVoh42Q2qIksBAruZ1atULfR5D55uzZvbaCtUxSig,11045
 dspawpy/io/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dspawpy/io/read.py,sha256=uVkODhh8IPU8k4Np31a-FFYF8SNK7wOe-gDOV49D-DU,52393
+dspawpy/io/read.py,sha256=jZYWmjTtQde_Za5kbTt206_6w6yieXVx5ZN8Z1YfkWY,52495
 dspawpy/io/read_json.py,sha256=2bcNQP51SR2yMyFE7c2TIutYp93K8IH-dpLmH5yy4bo,7721
-dspawpy/io/structure.py,sha256=vm_GKQqFvvGRjUQx3_pSn9eI2eEc8ZiX-z-71lbHF5s,8538
+dspawpy/io/structure.py,sha256=7iLLzyoaxRE3bCC1URKpx8QzoAx4CzwFXtA5wxX-jNA,10343
 dspawpy/io/utils.py,sha256=FdbFbZqKfnDOGBJ4OaKD-4IBAAlqjtQ0l1NppvkMKOM,25241
-dspawpy/io/write.py,sha256=W70yWfHDhQ2n8YItr80ubPhV591ClbvcmfKBAnapND8,28491
+dspawpy/io/write.py,sha256=-bHzDvE1Vr0x0kxZ8yJGQOmHQTjhkITG9dvUggOnxmU,25401
 dspawpy/io/write_json.py,sha256=n3GhdDnFFtW7eY4U5u7czdlpbSWnsGP7WUD5eS1ZmqI,1761
-dspawpy-0.9.2.dist-info/METADATA,sha256=Ad4kzjShQczca8QTJtZCHROpU6VkZwUZVFjIkI4Z1Wk,2215
-dspawpy-0.9.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-dspawpy-0.9.2.dist-info/top_level.txt,sha256=esEMNTnd880qHE4wkZVKM3gzqZMuOobS886owAyaUmA,8
-dspawpy-0.9.2.dist-info/RECORD,,
+dspawpy-0.9.3.dist-info/METADATA,sha256=exrAYV7qeKIsMUMvlswVbxc9DIHBdmx4wRcpa1ibx8M,2496
+dspawpy-0.9.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+dspawpy-0.9.3.dist-info/top_level.txt,sha256=esEMNTnd880qHE4wkZVKM3gzqZMuOobS886owAyaUmA,8
+dspawpy-0.9.3.dist-info/RECORD,,
```

