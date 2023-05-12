# Comparing `tmp/process_spectra-0.2.6.tar.gz` & `tmp/process_spectra-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "process_spectra-0.2.6.tar", max compression
+gzip compressed data, was "process_spectra-0.2.7.tar", max compression
```

## Comparing `process_spectra-0.2.6.tar` & `process_spectra-0.2.7.tar`

### file list

```diff
@@ -1,11 +1,9 @@
--rw-r--r--   0        0        0     1100 2021-08-28 19:14:58.219981 process_spectra-0.2.6/LICENSE
--rw-r--r--   0        0        0     3767 2021-12-12 19:12:20.646517 process_spectra-0.2.6/process_spectra/__init__.py
--rw-r--r--   0        0        0    18096 2021-12-24 23:49:14.880094 process_spectra-0.2.6/process_spectra/funcs/__init__.py
--rw-r--r--   0        0        0     6001 2022-04-23 15:14:00.762429 process_spectra-0.2.6/process_spectra/funcs/piezo_fbg.py
--rw-r--r--   0        0        0     3688 2021-12-12 02:07:25.632280 process_spectra-0.2.6/process_spectra/unused_and_untested.py
--rw-r--r--   0        0        0     3626 2021-12-15 18:06:45.770815 process_spectra-0.2.6/process_spectra/utils/__init__.py
--rw-r--r--   0        0        0     1504 2021-12-12 18:41:44.358703 process_spectra-0.2.6/process_spectra/utils/fbg.py
--rw-r--r--   0        0        0      835 2022-04-23 15:15:16.962174 process_spectra-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2629 2021-12-12 19:18:07.052405 process_spectra-0.2.6/README.md
--rw-r--r--   0        0        0     3556 2022-04-23 15:15:20.604470 process_spectra-0.2.6/setup.py
--rw-r--r--   0        0        0     3566 2022-04-23 15:15:20.604470 process_spectra-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1100 2023-05-12 15:56:28.645994 process_spectra-0.2.7/LICENSE
+-rw-r--r--   0        0        0     3919 2023-05-12 15:56:28.710121 process_spectra-0.2.7/process_spectra/__init__.py
+-rw-r--r--   0        0        0    18145 2023-05-12 15:56:28.711122 process_spectra-0.2.7/process_spectra/funcs/__init__.py
+-rw-r--r--   0        0        0     6001 2023-05-12 15:56:28.711122 process_spectra-0.2.7/process_spectra/funcs/piezo_fbg.py
+-rw-r--r--   0        0        0     3636 2023-05-12 15:56:28.712124 process_spectra-0.2.7/process_spectra/utils/__init__.py
+-rw-r--r--   0        0        0     1504 2023-05-12 15:56:28.713123 process_spectra-0.2.7/process_spectra/utils/fbg.py
+-rw-r--r--   0        0        0      835 2023-05-12 16:11:51.733473 process_spectra-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2629 2023-05-12 15:56:28.645994 process_spectra-0.2.7/README.md
+-rw-r--r--   0        0        0     3617 1970-01-01 00:00:00.000000 process_spectra-0.2.7/PKG-INFO
```

### Comparing `process_spectra-0.2.6/LICENSE` & `process_spectra-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `process_spectra-0.2.6/process_spectra/__init__.py` & `process_spectra-0.2.7/process_spectra/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,15 +84,18 @@
             spectrum, info = self.load_spectrum(self.filenames[i], **load_kwargs)
 
             if spectrum is not None:
                 for c, step in enumerate(self.steps):
                     spectrum, _info = step(spectrum, info, **self.kwargs[c])
                     info = {**info, **_info}
 
-            self.df = self.df.append(info, ignore_index=True)
+            info_df = pd.DataFrame(info, index=[0, ])
+            self.df = pd.concat([self.df, info_df],
+                                ignore_index=True,
+                                axis=0, join='outer')
 
         if self.out_filename:
             self.export_csv(self.out_filename)
 
     def export_csv(self, export_name):
         """
         Exporta o dataframe atual como um csv
```

### Comparing `process_spectra-0.2.6/process_spectra/funcs/__init__.py` & `process_spectra-0.2.7/process_spectra/funcs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,15 +328,15 @@
     info['resonant_wl'] = x
     info['resonant_wl_power'] = y
 
     return spectrum, info
 
 
 def get_approximate_valley(spectrum, info, approx_func=lorentz, prominence=5,
-                           resolution_proximity=2, p0=None, valley_samples=100,
+                           resolution_proximity=2, p0=None, dwl=2,
                            plot=False):
     """
     Aproxima a região do vale como uma curva determinada na 'approx_func',
         depois extrai o comprimento de onda ressonante a partir da curva
         aproximada (funciona também para espectros com mais de um vale).
         Também retorna o índice do vale com maior proeminência (best_index),
         para integrar melhor na interrogação do sensor
@@ -358,17 +358,16 @@
     :type resolution_proximity: float
 
     :param p0: Os parâmetros iniciais da aproximação. Deve ser uma lista com
         os parâmetros da função de aproximação (em ordem, ignorando x). Devem
         ser ajustados se a aproximação consistentemente falhar.
     :type p0: list
 
-    :param valley_samples: A quantidade máxima de samples em um vale. Deve ser
-        ajustado de acordo com a resolução do medidor
-    :type valley_samples: int
+    :param dwl: Espaçamento ao redor do vale que será usado para ajuste da função
+    :type valley_samples: float
 
     :param plot: Se deve ou não plotar os gráficos com aproximações. Se for
         True, o script deve estar rodando em um caminho que possui uma pasta
         chamada 'plots/'. Esse parâmetro serve para ajudar a ajustar os p0 e
         valley_samples
     :type plot: bool
 
@@ -378,46 +377,46 @@
     """
 
     wl = spectrum[::, 0]
     power = spectrum[::, 1]
     resolution = np.mean(np.diff(wl))
 
     peaks, peak_info = sg.find_peaks(-power, prominence=prominence,
-                                  plateau_size=0, wlen=valley_samples)
+                                  plateau_size=0, wlen=None)
 
     _info = dict()
 
     if plot:
         fig, ax = plt.subplots()
         ax.plot(wl, power)
 
-    for i in range(len(peaks)):
-        valley = spectrum[peak_info['left_bases'][i]: peak_info['right_bases'][i], ::]
+    _info['valley_count'] = len(peaks)
 
-        p0 = p0 or [-peak_info['prominences'][i],
-              wl[peaks[i]] * 1e6,
-              1,
-              power[peaks[i]]]
+    for i in range(len(peaks)):
+        wl0 = wl[peaks[i]]
+        mask = (spectrum[:, 0] > wl0 - dwl/2) & (spectrum[:, 0] < wl0 + dwl/2)
+        valley = spectrum[mask, ::]
 
         try:
-            popt, _ = curve_fit(approx_func, valley[::, 0] * 1e6, valley[::, 1],
-                                p0=p0, max_nfev=10000,
-                                bounds=(-np.inf, (0, np.inf, np.inf, np.inf)))
+            print(p0)
+            print(((-np.inf, wl0-resolution_proximity*resolution, 1e-10, -np.inf),
+                                        (+np.inf, wl0+resolution_proximity*resolution, 100, np.inf)))
+
+            popt, _ = curve_fit(approx_func, valley[::, 0], valley[::, 1],
+                                p0=None, max_nfev=10000,
+                                bounds=((-np.inf, wl0-resolution_proximity*resolution, 1e-10, -np.inf),
+                                        (+np.inf, wl0+resolution_proximity*resolution, 100, np.inf)))
 
-            resonant_wl = popt[1] * 1e-6
+            resonant_wl = popt[1]
             resonant_power = approx_func(popt[1], *popt)
 
         except RuntimeError:
             resonant_wl = wl[peaks[i]]
             resonant_power = power[peaks[i]]
 
-        if abs(resonant_wl - wl[peaks[i]]) > resolution_proximity * resolution:
-            resonant_wl = wl[peaks[i]]
-            resonant_power = power[peaks[i]]
-
         if len(peaks) == 1:
             _info['resonant_wl'] = resonant_wl
             _info['resonant_wl_power'] = resonant_power
         else:
             _info[f'resonant_wl_{i}'] = resonant_wl
             _info[f'resonant_wl_power_{i}'] = resonant_power
```

### Comparing `process_spectra-0.2.6/process_spectra/funcs/piezo_fbg.py` & `process_spectra-0.2.7/process_spectra/funcs/piezo_fbg.py`

 * *Files identical despite different names*

### Comparing `process_spectra-0.2.6/process_spectra/utils/__init__.py` & `process_spectra-0.2.7/process_spectra/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     :param unit: A unidade do espectro. dBm por padrão
     :type unit: string
 
     :param noise: O ruído elétrico na leitura da potência. O valor é usado
         como variância na geração de um aleatório
     :type noise: float
 
-    :return: A potência calculada
+    :return: A potência calculada, em Watts
     """
 
     if unit.upper() in ['DBM', 'DBMW']:
         y = dBmW_to_W(y)
     elif unit != 'W':
         raise ValueError(f'{unit} é uma unidade inválida, '
                          f'as implementadas são "dBm" e "W"')
```

### Comparing `process_spectra-0.2.6/process_spectra/utils/fbg.py` & `process_spectra-0.2.7/process_spectra/utils/fbg.py`

 * *Files identical despite different names*

### Comparing `process_spectra-0.2.6/pyproject.toml` & `process_spectra-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "process_spectra"
-version = "0.2.6"
+version = "0.2.7"
 description = "A package designed to process optical spectra of fiber optic sensors based on long period gratings (LPGs)."
 authors = ["Felipe Barino <felipebarino@gmail.com>", "Guilherme Sampaio <guilherme_albuquerque2@hotmail.com>"]
 maintainers = ["Guilherme Sampaio <guilherme_albuquerque2@hotmail.com>", "Felipe Barino <felipebarino@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/felipebarino/process_spectra"
 homepage = "https://github.com/felipebarino/process_spectra"
 readme = "README.md"
@@ -16,9 +16,9 @@
 scipy = "^1.6.2"
 matplotlib = "^3.3.2"
 pandas = "^1.3.4"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `process_spectra-0.2.6/README.md` & `process_spectra-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `process_spectra-0.2.6/setup.py` & `process_spectra-0.2.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,80 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: process-spectra
+Version: 0.2.7
+Summary: A package designed to process optical spectra of fiber optic sensors based on long period gratings (LPGs).
+Home-page: https://github.com/felipebarino/process_spectra
+License: MIT
+Author: Felipe Barino
+Author-email: felipebarino@gmail.com
+Maintainer: Guilherme Sampaio
+Maintainer-email: guilherme_albuquerque2@hotmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: matplotlib (>=3.3.2,<4.0.0)
+Requires-Dist: numpy (>=1.20.0,<2.0.0)
+Requires-Dist: pandas (>=1.3.4,<2.0.0)
+Requires-Dist: scipy (>=1.6.2,<2.0.0)
+Project-URL: Repository, https://github.com/felipebarino/process_spectra
+Description-Content-Type: text/markdown
 
-packages = \
-['process_spectra', 'process_spectra.funcs', 'process_spectra.utils']
+# process_spectra
 
-package_data = \
-{'': ['*']}
+This is the repo for the process_spectra package. It is a package designed to process optical spectra of fiber optic sensors based on long period gratings (LPGs). The documentation is written in portuguese, since the project was conceived to improve research at a brazilian university lab (LITel - UFJF). If the contents of the library may be useful to you, and you do not speak portuguese, please send us an e-mail or open an issue.
 
-install_requires = \
-['matplotlib>=3.3.2,<4.0.0',
- 'numpy>=1.20.0,<2.0.0',
- 'pandas>=1.3.4,<2.0.0',
- 'scipy>=1.6.2,<2.0.0']
-
-setup_kwargs = {
-    'name': 'process-spectra',
-    'version': '0.2.6',
-    'description': 'A package designed to process optical spectra of fiber optic sensors based on long period gratings (LPGs).',
-    'long_description': "# process_spectra\n\nThis is the repo for the process_spectra package. It is a package designed to process optical spectra of fiber optic sensors based on long period gratings (LPGs). The documentation is written in portuguese, since the project was conceived to improve research at a brazilian university lab (LITel - UFJF). If the contents of the library may be useful to you, and you do not speak portuguese, please send us an e-mail or open an issue.\n\nPacote python feito com o intuito de processar o espectro óptico de sensores ópticos a fibra baseados em grades de periodo longo (LPGs). Com esse pacote é possível fazer a extração de dados de conjuntos grandes de espectros, seguindo uma rotina específica. \n\n## Instalação:\n\nO pacote foi colocado no PyPi, logo é possível instalar pelo pip:\n\n```\npip install process_spectra\n```\n\n## Como usar:\n\nPara usar o pacote, basta criar um objeto da classe *MassSpectraData*, adicionar passos com os devidos argumentos e rodar. Como um exemplo simples que extrai os vales ressonantes de espectros na pasta *spectra*:\n\n``` python\nimport os\nimport process_spectra as ps\n\n\n# Criando a lista de caminhos\nfiles = os.listdir('spectra')\nfiles_complete = [os.path.join('spectra', x) for x in files]\n\n# Criando o objeto, passando a lista e o nome do arquivo para \n# salvar as informações extraídas\nspectra = ps.MassSpectraData(files_complete, 'resonant_wavelengths.csv')\n\n\n# Adicionando o passo de extração, com um dicionário de argumentos \n# para a função do passo\nspectra.add_step(ps.funcs.find_valley, {'prominence': 5, 'ignore_errors': True})\n\nspectra.run(ignore_errors=True)\n\n```\n\nVale notar que os ignore_errors são passados para evitar que o programa encerre no caso de encontrar algum. Isso é útil quando não se tem certeza da integridade de todos os espectros, visto que se um estiver corrompido, o programa pode travar nele.\n\nNa pasta de exemplos estão alguns scripts que foram escritos para e usados em pesquisas, e mostram mais funcionalidades do pacote.\n\n## Documentação\n\nA documentação não foi publicada em sites, mas foi colocada no código, então é possível encontrar ela através do comando help() do python, passando como argumento uma classe, função ou módulo, ou também lendo do código direto.\n\nTambém é possível gerar a documentação através do sphinx. Basta clonar / baixar o repositórrio, abrir um cmd na pasta sphinx e rodar o comando \n\n```\nmake html\n```\n\nA documentação será gerada em html, como um site, e pode ser encontrada no caminho *sphinx/_build/html/index.html*.",
-    'author': 'Felipe Barino',
-    'author_email': 'felipebarino@gmail.com',
-    'maintainer': 'Guilherme Sampaio',
-    'maintainer_email': 'guilherme_albuquerque2@hotmail.com',
-    'url': 'https://github.com/felipebarino/process_spectra',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+Pacote python feito com o intuito de processar o espectro óptico de sensores ópticos a fibra baseados em grades de periodo longo (LPGs). Com esse pacote é possível fazer a extração de dados de conjuntos grandes de espectros, seguindo uma rotina específica. 
 
+## Instalação:
 
-setup(**setup_kwargs)
+O pacote foi colocado no PyPi, logo é possível instalar pelo pip:
+
+```
+pip install process_spectra
+```
+
+## Como usar:
+
+Para usar o pacote, basta criar um objeto da classe *MassSpectraData*, adicionar passos com os devidos argumentos e rodar. Como um exemplo simples que extrai os vales ressonantes de espectros na pasta *spectra*:
+
+``` python
+import os
+import process_spectra as ps
+
+
+# Criando a lista de caminhos
+files = os.listdir('spectra')
+files_complete = [os.path.join('spectra', x) for x in files]
+
+# Criando o objeto, passando a lista e o nome do arquivo para 
+# salvar as informações extraídas
+spectra = ps.MassSpectraData(files_complete, 'resonant_wavelengths.csv')
+
+
+# Adicionando o passo de extração, com um dicionário de argumentos 
+# para a função do passo
+spectra.add_step(ps.funcs.find_valley, {'prominence': 5, 'ignore_errors': True})
+
+spectra.run(ignore_errors=True)
+
+```
+
+Vale notar que os ignore_errors são passados para evitar que o programa encerre no caso de encontrar algum. Isso é útil quando não se tem certeza da integridade de todos os espectros, visto que se um estiver corrompido, o programa pode travar nele.
+
+Na pasta de exemplos estão alguns scripts que foram escritos para e usados em pesquisas, e mostram mais funcionalidades do pacote.
+
+## Documentação
+
+A documentação não foi publicada em sites, mas foi colocada no código, então é possível encontrar ela através do comando help() do python, passando como argumento uma classe, função ou módulo, ou também lendo do código direto.
+
+Também é possível gerar a documentação através do sphinx. Basta clonar / baixar o repositórrio, abrir um cmd na pasta sphinx e rodar o comando 
+
+```
+make html
+```
+
+A documentação será gerada em html, como um site, e pode ser encontrada no caminho *sphinx/_build/html/index.html*.
```

