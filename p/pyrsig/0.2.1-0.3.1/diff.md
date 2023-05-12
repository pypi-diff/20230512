# Comparing `tmp/pyrsig-0.2.1.tar.gz` & `tmp/pyrsig-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyrsig-0.2.1.tar", last modified: Thu Apr 27 13:41:21 2023, max compression
+gzip compressed data, was "dist/pyrsig-0.3.1.tar", last modified: Fri May 12 20:31:01 2023, max compression
```

## Comparing `pyrsig-0.2.1.tar` & `pyrsig-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-04-27 13:41:21.000000 pyrsig-0.2.1/
--rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.2.1/setup.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-04-27 13:41:21.000000 pyrsig-0.2.1/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.2.1/LICENSE
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig.egg-info/
--rw-r--r--   0 bhenders (83225) romo       (131)      357 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig.egg-info/SOURCES.txt
--rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig.egg-info/PKG-INFO
--rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig.egg-info/dependency_links.txt
--rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig.egg-info/top_level.txt
--rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig.egg-info/requires.txt
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig/
-drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-04-27 13:41:21.000000 pyrsig-0.2.1/pyrsig/tests/
--rw-r--r--   0 bhenders (83225) romo       (131)      800 2023-03-29 20:44:48.000000 pyrsig-0.2.1/pyrsig/tests/test_api.py
--rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.2.1/pyrsig/tests/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2058 2023-03-29 20:31:50.000000 pyrsig-0.2.1/pyrsig/tests/test_ioapi.py
--rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-03-29 20:35:02.000000 pyrsig-0.2.1/pyrsig/tests/test_misc.py
--rw-r--r--   0 bhenders (83225) romo       (131)     2460 2023-03-29 20:44:35.000000 pyrsig-0.2.1/pyrsig/tests/test_dataframes.py
--rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.2.1/pyrsig/tests/test_coards.py
--rw-r--r--   0 bhenders (83225) romo       (131)    33171 2023-04-26 13:25:55.000000 pyrsig-0.2.1/pyrsig/__init__.py
--rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-04-27 13:41:21.000000 pyrsig-0.2.1/setup.cfg
--rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.2.1/README.md
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-12 20:31:01.000000 pyrsig-0.3.1/
+-rw-r--r--   0 bhenders (83225) romo       (131)      966 2023-03-20 17:04:08.000000 pyrsig-0.3.1/setup.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-05-12 20:31:01.000000 pyrsig-0.3.1/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)    35149 2023-03-20 17:04:08.000000 pyrsig-0.3.1/LICENSE
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-12 20:31:01.000000 pyrsig-0.3.1/pyrsig.egg-info/
+-rw-r--r--   0 bhenders (83225) romo       (131)      357 2023-05-12 20:31:00.000000 pyrsig-0.3.1/pyrsig.egg-info/SOURCES.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)     2825 2023-05-12 20:31:00.000000 pyrsig-0.3.1/pyrsig.egg-info/PKG-INFO
+-rw-r--r--   0 bhenders (83225) romo       (131)        1 2023-05-12 20:31:00.000000 pyrsig-0.3.1/pyrsig.egg-info/dependency_links.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)        7 2023-05-12 20:31:00.000000 pyrsig-0.3.1/pyrsig.egg-info/top_level.txt
+-rw-r--r--   0 bhenders (83225) romo       (131)       23 2023-05-12 20:31:00.000000 pyrsig-0.3.1/pyrsig.egg-info/requires.txt
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-12 20:31:01.000000 pyrsig-0.3.1/pyrsig/
+drwxr-xr-x   0 bhenders (83225) romo       (131)        0 2023-05-12 20:31:01.000000 pyrsig-0.3.1/pyrsig/tests/
+-rw-r--r--   0 bhenders (83225) romo       (131)      800 2023-03-29 20:44:48.000000 pyrsig-0.3.1/pyrsig/tests/test_api.py
+-rw-r--r--   0 bhenders (83225) romo       (131)        0 2023-03-20 17:04:08.000000 pyrsig-0.3.1/pyrsig/tests/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2058 2023-03-29 20:31:50.000000 pyrsig-0.3.1/pyrsig/tests/test_ioapi.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      142 2023-03-29 20:35:02.000000 pyrsig-0.3.1/pyrsig/tests/test_misc.py
+-rw-r--r--   0 bhenders (83225) romo       (131)     2460 2023-03-29 20:44:35.000000 pyrsig-0.3.1/pyrsig/tests/test_dataframes.py
+-rw-r--r--   0 bhenders (83225) romo       (131)      805 2023-03-29 20:12:31.000000 pyrsig-0.3.1/pyrsig/tests/test_coards.py
+-rw-r--r--   0 bhenders (83225) romo       (131)    37717 2023-05-12 20:28:38.000000 pyrsig-0.3.1/pyrsig/__init__.py
+-rw-r--r--   0 bhenders (83225) romo       (131)       38 2023-05-12 20:31:01.000000 pyrsig-0.3.1/setup.cfg
+-rw-r--r--   0 bhenders (83225) romo       (131)     2290 2023-04-26 13:24:41.000000 pyrsig-0.3.1/README.md
```

### Comparing `pyrsig-0.2.1/setup.py` & `pyrsig-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.2.1/PKG-INFO` & `pyrsig-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.2.1
+Version: 0.3.1
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.2.1/LICENSE` & `pyrsig-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsig-0.2.1/pyrsig.egg-info/PKG-INFO` & `pyrsig-0.3.1/pyrsig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsig
-Version: 0.2.1
+Version: 0.3.1
 Summary: Python interface to RSIG Web API
 Home-page: https://github.com/barronh/pyrsig
 Author: Barron H. Henderson
 Author-email: barronh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyrsig-0.2.1/pyrsig/tests/test_api.py` & `pyrsig-0.3.1/pyrsig/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.2.1/pyrsig/tests/test_ioapi.py` & `pyrsig-0.3.1/pyrsig/tests/test_ioapi.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.2.1/pyrsig/tests/test_dataframes.py` & `pyrsig-0.3.1/pyrsig/tests/test_dataframes.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.2.1/pyrsig/tests/test_coards.py` & `pyrsig-0.3.1/pyrsig/tests/test_coards.py`

 * *Files identical despite different names*

### Comparing `pyrsig-0.2.1/pyrsig/__init__.py` & `pyrsig-0.3.1/pyrsig/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __all__ = ['RsigApi', 'open_ioapi']
-__version__ = '0.2.1'
+__version__ = '0.3.1'
 
 import pandas as pd
 
 _def_grid_kw = {
     '12US1': dict(
         GDNAM='12US1', GDTYP=2, NCOLS=459, NROWS=299,
         XORIG=-2556000.0, YORIG=-1728000.0, XCELL=12000., YCELL=12000.,
@@ -104,70 +104,79 @@
     'tempo.proxy_l2.o3p.ozone_information_content',
     'tempo.proxy_l2.o3p.ground_pixel_quality_flag',
     'tropomi.offl.no2.nitrogendioxide_tropospheric_column',
     'tropomi.offl.no2.air_mass_factor_troposphere',
     'tropomi.offl.hcho.formaldehyde_tropospheric_vertical_column',
     'tropomi.offl.co.carbonmonoxide_total_column',
     'tropomi.offl.ch4.methane_mixing_ratio',
-    'tropomi.offl.ch4.methane_mixing_ratio',
     'tropomi.offl.ch4.methane_mixing_ratio_bias_corrected',
     'viirsnoaa.jrraod.AOD550', 'viirsnoaa.vaooo.AerosolOpticalDepth_at_550nm',
 )
 
 _point_prefixes = ('airnow', 'aqs', 'purpleair', 'pandora')
 
 
 def parsexml(root):
     """Recursive xml parsing:
     Given a root, return dictionaries for each element and its children.
     Each element has children, attributes (attr), tag, and text.
     If any of these has no elements, it will be removed.
     """
-    out = dict(
-        children=[], attr=root.attrib, text=root.text,
-        tag=root.tag.split('}')[1]
-    )
+    out = {}
+    out['tag'] = root.tag.split('}')[-1]
+    out['attr'] = root.attrib
+    out['text'] = root.text
+    out['children'] = []
+
     for child in root:
         childd = parsexml(child)
         out['children'].append(childd)
+
     if len(out['children']) == 0:
         del out['children']
     if out['text'] is None:
         out['text'] = ''
+
     out['text'] = out['text'].strip()
     if len(out['text']) == 0:
         del out['text']
     if len(out['attr']) == 0:
         del out['attr']
+
     return out
 
 
 def coverages_from_xml(txt):
     """Based on xml text, create coverage data"""
     import xml.etree.ElementTree as ET
+
     root = ET.fromstring(txt)
+
     xmlout = parsexml(root)
     out = []
     for c in xmlout['children']:
         record = {k: v for k, v in c.items() if k != 'children'}
         kids = c['children']
         for e in kids:
             if 'attr' not in e and len(e.get('children', [])) == 0:
                 record[e['tag']] = e.get('text', '')
+
             if e['tag'] == 'lonLatEnvelope':
                 envtxt = ''
                 for p in e['children']:
                     envtxt += ' ' + p['text']
                 record['bbox_str'] = envtxt
+
             if e['tag'] == 'domainSet':
                 for s in e['children']:
                     if s['tag'] == 'temporalDomain':
                         for tp in s['children']:
                             for te in tp['children']:
                                 record[te['tag']] = te['text']
+
         out.append(record)
 
     return out
 
 
 def _progress(blocknum, readsize, totalsize):
     """
@@ -385,15 +394,16 @@
           teh api_key property to their own key. Contact PurpleAir for more
           details.
 
         """
         self._description = {}
         self._keys = None
         self._capabilities = None
-        self._describecoverage = None
+        self._describecoverages = None
+        self._coveragesdf = None
         self.server = server
         self.key = key
         self.compress = compress
         self.workdir = workdir
         self.encoding = encoding
         self.overwrite = overwrite
 
@@ -438,71 +448,187 @@
                 'out_in_flag': 0, 'freq': 'hourly',
                 'maximum_difference': 5, 'maximum_ratio': 0.70,
                 'agg_pct': 75, 'api_key': '<your key here>'
             }
 
         self.purpleair_kw = purpleair_kw
 
-    def describe(self, key):
+    def describe(self, key, as_dataframe=True, raw=False):
         """
-        Describe is currently unreliable becuase of malformed xml.
-        Use descriptions and query by name.
+        describe returns details about the coverage specified by key. Details
+        include spatial bounding box, time coverage, time resolution, variable
+        label, and a short description.
+
+        DescribeCoverage with a COVERAGE should be faster than descriptions
+        because it only returns a smalll xml chunk. Currently, DescribeCoverage
+        with a COVERAGE specified is unreliable because of malformed xml. If
+        this fails, describe will instead request all coverages and query it
+        for the specific coverage. This is much slower and is being addressed.
+
+        Arguments
+        ---------
+        as_dataframe : bool
+            Defaults to True and descriptions are returned as a dataframe.
+            If False, returns a list of elements.
+        raw : bool
+            Return raw xml instead of parsing. Useful for debugging.
+
+        Returns
+        -------
+        coverages : pandas.DataFrame or list
+            dataframe or list of parsed descriptions
+
+        Example
+        -------
+            df = rsigapi.describe('airnow.no2')
+            print(df.to_csv())
+            # ,name,label,description,bbox_str,beginPosition,timeResolution
+            # 0,no2,no2(ppb),UTC hourly mean surface measured nitrogen ...,
+            # ... -157 21 -51 64,2003-01-02T00:00:00Z,PT1H
         """
         import requests
+        import warnings
         if key not in self._description:
             r = requests.get(
                 f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION='
                 f'1.0.0&REQUEST=DescribeCoverage&COVERAGE={key}&compress=1'
             )
             self._description[key] = r.text
 
-        return self._description[key]
+        if raw:
+            return self._description[key]
+
+        try:
+            coverages = coverages_from_xml(self._description[key])
+        except Exception as e:
+            warnings.warn(str(e) + '; using descriptions')
+            return self.descriptions().query(f'name == "{key}"')
+
+        if as_dataframe:
+            coverages = pd.DataFrame.from_records(coverages)
+            coverages['prefix'] = coverages['name'].apply(
+                lambda x: x.split('.')[0]
+            )
+            coverages = coverages.drop('tag', axis=1)
 
-    def descriptions(self, as_dataframe=True):
+        return coverages
+
+    def descriptions(self, as_dataframe=True, verbose=0):
         """
         Experimental and may change.
 
+        descriptions returns details about all coverages. Details include
+        spatial bounding box, time coverage, time resolution, variable label,
+        and a short description.
+
         Currently, parses capabilities using xml.etree.ElementTree and returns
         coverages from details available in CoverageOffering elements from
         DescribeCoverage.
 
         Currently cleaning up data xml elements that are bad and doing a
         per-coverage parsing to increase fault tolerance in the xml.
 
-        Examples:
+        Arguments
+        ---------
+        as_dataframe : bool
+            Defaults to True and descriptions are returned as a dataframe.
+            If False, returns a list of elements.
+        verbose : int
+            If verbose is greater than 0, show warnings from parsing.
+
+        Returns
+        -------
+        coverages : pandas.DataFrame or list
+            dataframe or list of parsed descriptions
+
+        Example
+        -------
 
             rsigapi = pyrsig.RsigApi()
             desc = rsigapi.descriptions()
-            desc[desc['name'].str.startswith('tropomi')]
-
+            print(desc.query('prefix == "tropomi"').name.unique())
+            # ['tropomi.nrti.no2.nitrogendioxide_tropospheric_column'
+            #  ... 43 other name here
+            #  'tropomi.rpro.ch4.methane_mixing_ratio_bias_corrected']
         """
         import re
         import pandas as pd
         import warnings
+        import requests
 
-        c = self.describecoverages()
-        ctext = c.text.replace('<?xml version="1.0" encoding="UTF-8" ?>', '')
-        # Currently correcting information that wasn't working.
-        ctext = ctext.replace('<=', 'less than or equal to')
-        ctext = ctext.replace('<0=', 'less than zero =')
-        ctext = ctext.replace('>0=', 'greater than zero =')
-        ctext = ctext.replace(
-            '<lonLatEnvelope srsName="WGS84(DD)"\n',
-            '<lonLatEnvelope srsName="WGS84(DD)">\n'
+        if as_dataframe and self._coveragesdf is not None:
+            return self._coveragesdf
+
+        if self._describecoverages is None:
+            if verbose > 1:
+                print('Requesting...', flush=True)
+            self._describecoverages = requests.get(
+                f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION='
+                '1.0.0&REQUEST=DescribeCoverage&compress=1'
+            ).text
+
+        ctext = self._describecoverages
+
+        # Start Cleaning Section
+        # BHH 2023-05-10
+        # This section provides "cleaning" to the xml content provided by
+        # DescribeCoverage. This should not have to happen and should be
+        # removable at some point in the future.
+        # Working with TP to fix xml
+
+        descmidre = re.compile(
+            r'\</CoverageDescription\>.+?\<CoverageDescription.+?\>',
+            flags=re.MULTILINE + re.DOTALL
+        )
+        mismatchtempre = re.compile(
+            r'\</lonLatEnvelope\>\s+\</spatialDomain\>',
+            flags=re.MULTILINE + re.DOTALL
         )
+
+        # Regex, replacement
+        resubsdesc = [
+            (descmidre, ''),
+            (re.compile('<='), '&lt;='),  # associated with <= 32 in Modis
+            (
+                mismatchtempre,
+                '</lonLatEnvelope><domainSet><spatialDomain></spatialDomain>',
+            ),  # Missing open block for spatialDomain in goes (eg imager.calb)
+            (
+                re.compile(r'</CoverageOffering>\s+</CoverageOfferingBrief>'),
+                '</CoverageOffering>',
+            ),  # Ceiliometers have wrong opening tags and extra close tag
+            (
+                re.compile('CoverageOfferingBrief'), 'CoverageOffering'
+            ),  # Ceiliometers have wrong opening tags and extra close tag
+            (
+                re.compile(
+                    r'<rangeSet>\s+<RangeSet>\s+<supportedCRSs>',
+                    flags=re.MULTILINE + re.DOTALL
+                ),
+                '<rangeSet><RangeSet></RangeSet></rangeSet><supportedCRSs>'
+            ),  # Ceiliometers have missing rangeset content and closing tags
+        ]
+        for reg, sub in resubsdesc:
+            ctext = reg.sub(sub, ctext)
+
+        # End Cleaning Section
+
+        # Selecting coverages and removing garbage when necessary.
         cleanre = re.compile(
             r'\</name\>.+?\</CoverageOffering\>',
             flags=re.MULTILINE + re.DOTALL
         )
         # <CoverageOffering>.+?</CoverageOffering>
         coverre = re.compile(
             r'\<CoverageOffering\>.+?\</CoverageOffering\>',
             flags=re.MULTILINE + re.DOTALL
         )
+
         coverages = []
+        limited_details = []
         for rex in coverre.finditer(ctext):
             secttxt = ctext[rex.start():rex.end()]
             secttxt = (
                 '<CoverageDescription version="1.0.0"'
                 + ' xmlns="http://www.opengeospatial.org/standards/wcs"'
                 + ' xmlns:gml="http://www.opengis.net/gml"'
                 + ' xmlns:xlink="http://www.w3.org/1999/xlink">'
@@ -514,23 +640,35 @@
             except Exception as e:
                 try:
                     secttxt = cleanre.sub(
                         '</name></CoverageOffering>', secttxt
                     )
                     coverage = coverages_from_xml(secttxt)
                     coverages.extend(coverage)
-                    warnings.warn(f'Limited details for {coverage[0]["name"]}')
+                    limited_details.append(coverage[0]["name"])
                 except Exception as e2:
                     # If a secondary error was raised, print it... but raise
                     # the original error
                     print(e)
                     raise e2
 
+        nlimited = len(limited_details)
+        if nlimited > 0 and verbose > 0:
+            limitedstr = ', '.join(limited_details)
+            warnings.warn(
+                f'Limited details for {nlimited} coverages: {limitedstr}'
+            )
+
         if as_dataframe:
             coverages = pd.DataFrame.from_records(coverages)
+            coverages['prefix'] = coverages['name'].apply(
+                lambda x: x.split('.')[0]
+            )
+            coverages = coverages.drop('tag', axis=1)
+            self._coveragesdf = coverages
 
         return coverages
 
     def capabilities(self):
         """
         At this time, the capabilities does not list cmaq.*
 
@@ -540,29 +678,14 @@
             self._capabilities = requests.get(
                 f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION='
                 '1.0.0&REQUEST=GetCapabilities&compress=1'
             )
 
         return self._capabilities
 
-    def describecoverages(self):
-        """
-        DescribeCoverage is a call to the server to get all key contents.
-        Right now, I do not allow specific key requests because they are
-        unreliable. They are unreliable because of malformed xml.
-        """
-        import requests
-        if self._describecoverage is None:
-            self._describecoverage = requests.get(
-                f'https://{self.server}/rsig/rsigserver?SERVICE=wcs&VERSION='
-                '1.0.0&REQUEST=DescribeCoverage&compress=1'
-            )
-
-        return self._describecoverage
-
     def keys(self, offline=True):
         """
         Arguments
         ---------
         offline : bool
             If True, uses small cached set of coverages.
             If False, finds all coverages from capabilities.
@@ -698,16 +821,16 @@
             f'&TIME={bdate:%Y-%m-%dT%H:%M:%SZ}/{edate:%Y-%m-%dT%H:%M:%SZ}'
             f'&BBOX={wlon},{slat},{elon},{nlat}'
             f'&COVERAGE={key}'
             f'&COMPRESS={compress}'
         ) + purpleairstr + viirsnoaastr + tropomistr + gridstr + cornerstr
 
         outpath = (
-            f'{self.workdir}/{key}_{bdate:%Y-%m-%dT%H:%M:%SZ}'
-            f'_{edate:%Y-%m-%dT%H:%M:%SZ}'
+            f'{self.workdir}/{key}_{bdate:%Y-%m-%dT%H%M%SZ}'
+            f'_{edate:%Y-%m-%dT%H%M%SZ}'
         )
 
         if formatstr.lower() == 'ascii':
             outpath += '.csv'
         elif formatstr.lower() == 'netcdf-ioapi':
             outpath += '.nc'
         elif formatstr.lower() == 'netcdf-coards':
@@ -764,15 +887,16 @@
         unit_keys : bool
           If True, keep unit in column name.
           If False, move last parenthetical part of key to attrs of Series.
         parse_dates : bool
           If True, parse Timestamp(UTC)
         withmeta: bool
           If True, add 'GetMetadata' results as a "metadata" attribute of the
-          dataframe.
+          dataframe. This is useful for understanding the underlying datasets
+          used to create the result.
         verbose : int
           level of verbosity
 
         Returns
         -------
         df : pandas.DataFrame
             Results from download
@@ -836,15 +960,16 @@
           beginning date (inclusive) defaults to yesterday at 0Z
         edate : str or pd.Datetime
           ending date (inclusive) defaults to bdate + 23:59:59
         bbox : tuple
           wlon, slat, elon, nlat in decimal degrees (-180 to 180)
         withmeta : bool
           If True, add 'GetMetadata' results at an attribute "metadata" to the
-          netcdf file.
+          netcdf file. This is useful for understanding the underlying datasets
+          used to create the result.
         removegz : bool
           If True, then remove the downloaded gz file. Bad for caching.
 
         Returns
         -------
         ds : xarray.Dataset
             Results from download
```

### Comparing `pyrsig-0.2.1/README.md` & `pyrsig-0.3.1/README.md`

 * *Files identical despite different names*

