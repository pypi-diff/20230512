# Comparing `tmp/gwas_sumstats_tools-1.0.0a3.tar.gz` & `tmp/gwas_sumstats_tools-1.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwas_sumstats_tools-1.0.0a3.tar", max compression
+gzip compressed data, was "gwas_sumstats_tools-1.0.1a0.tar", max compression
```

## Comparing `gwas_sumstats_tools-1.0.0a3.tar` & `gwas_sumstats_tools-1.0.1a0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/LICENSE
--rw-r--r--   0        0        0     4610 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/README.md
--rw-r--r--   0        0        0    10971 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/cli.py
--rw-r--r--   0        0        0     1387 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/config.py
--rw-r--r--   0        0        0     5671 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/format.py
--rw-r--r--   0        0        0     8560 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/interfaces/data_table.py
--rw-r--r--   0        0        0     7260 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/interfaces/metadata.py
--rw-r--r--   0        0        0     3913 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/read.py
--rw-r--r--   0        0        0     5754 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/schema/data_table.py
--rw-r--r--   0        0        0     1785 2023-03-20 10:58:07.448067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/schema/metadata.py
--rw-r--r--   0        0        0     4603 2023-03-20 10:58:07.449067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/utils.py
--rw-r--r--   0        0        0     7452 2023-03-20 10:58:07.449067 gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/validate.py
--rw-r--r--   0        0        0      679 2023-03-20 11:15:13.339784 gwas_sumstats_tools-1.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     5254 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-03-14 16:27:27.618973 gwas_sumstats_tools-1.0.1a0/LICENSE
+-rw-r--r--   0        0        0     4846 2023-04-11 15:51:21.526207 gwas_sumstats_tools-1.0.1a0/README.md
+-rw-r--r--   0        0        0    11560 2023-04-11 15:51:21.557208 gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/cli.py
+-rw-r--r--   0        0        0     1387 2023-03-14 16:27:27.619973 gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/config.py
+-rw-r--r--   0        0        0     5701 2023-05-12 13:51:16.162417 gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/format.py
+-rw-r--r--   0        0        0    10291 2023-04-11 15:51:21.558208 gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/interfaces/data_table.py
+-rw-r--r--   0        0        0     7516 2023-05-12 13:51:16.162417 gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/interfaces/metadata.py
+-rw-r--r--   0        0        0     3913 2023-03-14 16:27:27.619973 gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/read.py
+-rw-r--r--   0        0        0     5754 2023-03-14 16:27:27.619973 gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/schema/data_table.py
+-rw-r--r--   0        0        0     1785 2023-03-14 16:27:27.619973 gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/schema/metadata.py
+-rw-r--r--   0        0        0     4773 2023-05-12 13:51:16.163417 gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/utils.py
+-rw-r--r--   0        0        0     8337 2023-04-11 15:51:21.558208 gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/validate.py
+-rw-r--r--   0        0        0      679 2023-05-12 13:51:16.163417 gwas_sumstats_tools-1.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0     5490 1970-01-01 00:00:00.000000 gwas_sumstats_tools-1.0.1a0/PKG-INFO
```

### Comparing `gwas_sumstats_tools-1.0.0a3/LICENSE` & `gwas_sumstats_tools-1.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a3/README.md` & `gwas_sumstats_tools-1.0.1a0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,104 +1,115 @@
 # GWAS SumStats Tools
 
 
-A basic toolkit for reading and formatting GWAS sumstats files from the GWAS Catalog.
+A simple toolkit for reading and formatting GWAS sumstats files from the GWAS Catalog.
 Built with:
 * [Petl](https://petl.readthedocs.io/en/stable/index.html)
 * [Pydantic](https://docs.pydantic.dev/)
 * [Typer](https://typer.tiangolo.com/)
 
-There are three commands, `read`, `validate` and `format`.
+There are three commands, `validate`, `read` and `format`.
+
+
+`validate` is for:
+* Validating a summary statistic file using a dynamically generated schema
 
 `read` is for:
 * Previewing a data file: _no options_
 * Extracting the field headers: `-h`
 * Extracting all the metadata: `-M`
 * Extacting specific field, value pairs from the metada: `-m <field name>`
-
-`validate` is for:
-* Validating a summary statistic file using a dynamically generated schema
+* More functionality is to come...
 
 `format` is for:
 * Converting a minamally formatted sumstats data file to the standard format. This is not guaranteed to return a valid standard file, because manadatory data fields could be missing in the input. It simply does the following. `-s`
   * Renames `variant_id` -> `rsid`
   * Reorders the fields
   * Converts `NA` missing values to `#NA`
   * It is memory efficient and will take approx. 30s per 1 million records
 * Generate metadata for a data file: `-m`
   * Read metadata in from existing file: `--meta-in <file>`
   * Create metadata from the GWAS Catalog (internal use, requires authenticated API): `-g`
   * Edit/add the values to the metadata: `-e` with `--<FIELD>=<VALUE>`
 
+## Requirements
+- python >= 3.9
+
 ## Installation
 ```console
 $ pip install gwas-sumstats-tools
 ```
 
 ## Usage
 
+<p align="center"><img src="gwas-demo.gif"/></p>
+
 ```console
 $ gwas-ssf [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 **Commands**:
 
-* `format`: Format a sumstats file and...
+* `validate`: Validate a sumstats file
+* `format`: Format a sumstats file
 * `read`: Read a sumstats file
 
-### `gwas-ssf read`
 
-Read (preview) a sumstats file
+### `gwas-ssf validate`
+
+Validate a sumstats file
+
 
 **Usage**:
 
 ```console
-$ gwas-ssf read [OPTIONS] FILENAME
+$ gwas-ssf validate [OPTIONS] FILENAME
 ```
 
 **Arguments**:
 
-* `FILENAME`: Input sumstats file  [required]
+* `FILENAME`: Input sumstats file. Must be TSV (may be gzipped) [required]
 
 **Options**:
 
-* `-h, --get-header`: Just return the headers of the file  [default: False]
-* `--meta-in PATH`: Specify a metadata file to read in, defaulting to <filename>-meta.yaml
-* `-M, --get-all-metadata`: Return all metadata  [default: False]
-* `-m, --get-metadata TEXT`: Get metadata for the specified fields e.g. `-m genomeAssembly -m isHarmonised
+* `-e, --errors-out`: Output erros to a csv file, <filename>.err.csv.gz
+* `-z, --p-zero`: Force p-values of zero to be allowable. Takes precedence over inferred value (-i)
+* `-m, --min-rows`:  Minimum rows acceptable for the file [default: 100000]
+* `-i, --infer-from-metadata`: Infer validation options from the metadata file <filename>-meta.yaml. E.g. a populated field for analysis software makes p-values of zero allowable.
 * `--help`: Show this message and exit.
 
 
-### `gwas-ssf validate`
+### `gwas-ssf read`
 
-Validate a sumstats file
+Read (preview) a sumstats file
 
 **Usage**:
 
 ```console
-$ gwas-ssf validate [OPTIONS] FILENAME
+$ gwas-ssf read [OPTIONS] FILENAME
 ```
 
 **Arguments**:
 
-* `FILENAME`: Input sumstats file. Must be TSV or CSV and may be gzipped [required]
+* `FILENAME`: Input sumstats file  [required]
 
 **Options**:
 
-* `-e, --errors-out`: Output erros to a csv file, <filename>.err.csv.gz
-* `-z, --p-zero`: Force p-values of zero to be allowable. Takes precedence over inferred value (-i)
-* `-n, --p-neg-log`: Force p-values to be validated as -log10. Takes precedence over inferred value (-i)
-* `-m, --min-rows`:  Minimum rows acceptable for the file [default: 100000]
-* `-i, --infer-from-metadata`: Infer validation options from the metadata file <filename>-meta.yaml. E.g. fields for analysis software and negative log10 p-values affect the data validation behaviour.
+* `-h, --get-header`: Just return the headers of the file  [default: False]
+* `--meta-in PATH`: Specify a metadata file to read in, defaulting to <filename>-meta.yaml
+* `-M, --get-all-metadata`: Return all metadata  [default: False]
+* `-m, --get-metadata TEXT`: Get metadata for the specified fields e.g. `-m genomeAssembly -m isHarmonised
 * `--help`: Show this message and exit.
 
+
+
 ### `gwas-ssf format`
 
 Format a sumstats file and creating a new one. Add/edit metadata.
 
 **Usage**:
 
 ```console
@@ -128,7 +139,11 @@
 
 1. [install poetry](https://python-poetry.org/docs/#installation)
 
 2. `git clone https://github.com/EBISPOT/gwas-sumstats-tools.git`
 3. `cd gwas-sumstats-tools`
 4. `poetry install`
 5. `poetry run pytest`
+
+To make a change:
+branch from master -> PR to master -> poetry version -> git add pyproject.toml -> git commit -> git tag <version> -> git push origin master --tags
+If all the tests pass, this will publish to pypi.
```

### Comparing `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/cli.py` & `gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,21 +36,27 @@
                                                  help="Output erros to a csv file, <filename>.err.csv.gz"),
                 pval_zero: bool = typer.Option(False,
                                                "--p-zero", "-z",
                                                help="Force p-values of zero to be allowable. Takes precedence over inferred value (-i)"),
                 minimum_rows: int = typer.Option(100_000,
                                                  "--min-rows", "-m",
                                                  help="Minimum rows acceptable for the file"),
+                chunkzize: int = typer.Option(1_000_000,
+                                              "--chunksize", "-s",
+                                              help=("Number of rows to store in memory at once. "
+                                                    "Increase this number for more speed at the cost "
+                                                    "of more memory. Decrease to save memory, at the "
+                                                    "cost of speed.")),
                 infer_from_metadata: bool = typer.Option(False,
-                                                   "--infer-from-metadata", "-i",
-                                                   help=("Infer validation options from the "
-                                                         "metadata file <filename>-meta.yaml. "
-                                                         "E.g. fields for analysis software and "
-                                                         "negative log10 p-values affect the data "
-                                                         "validation behaviour."))
+                                                         "--infer-from-metadata", "-i",
+                                                         help=("Infer validation options from the "
+                                                               "metadata file <filename>-meta.yaml. "
+                                                               "E.g. fields for analysis software and "
+                                                               "negative log10 p-values affect the data "
+                                                               "validation behaviour."))
                 ):
     """
     [green]VALIDATE[/green] a GWAS summary statistics data file
     """
     print(f"Validating file: {filename}")
     with Progress(SpinnerColumn(),
                   TextColumn("[progress.description]{task.description}"),
@@ -60,14 +66,15 @@
         (valid,
          message,
          error_preview,
          error_type) = validate(filename=filename,
                                 errors_file=errors_file,
                                 pval_zero=pval_zero,
                                 minimum_rows=minimum_rows,
+                                chunksize=chunkzize,
                                 infer_from_metadata=infer_from_metadata)
     print(f"Validation status: {valid}")
     print(message)
     if error_type:
         print(("Primary reason for validation failure: "
                f"[red]{error_type}[/red]"))
     if error_preview:
```

### Comparing `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/config.py` & `gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/config.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/format.py` & `gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
         Keyword Arguments:
             from_gwas_cat -- update with data from GWAS catalog (default: {False})
             custom_metadata -- Update with this map (default: {None})
 
         Returns:
             metadata object
         """
+        self.meta.from_file()
         meta_dict = get_file_metadata(in_file=self.data_infile,
                                       out_file=self.data_outfile)
         if from_gwas_cat:
             accession_id = parse_accession_id(filename=self.data_infile)
             meta_dict.update(metadata_dict_from_gwas_cat(accession_id=accession_id))
         if custom_metadata:
             meta_dict.update(custom_metadata)
```

### Comparing `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/interfaces/data_table.py` & `gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/interfaces/data_table.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
 from typing import Union
 import pandas as pd
+from pandas.io.parsers import TextFileReader
 import numpy as np
 import petl as etl
 
 
 """formatters
 
 rename_headers(chromosome=...,)
@@ -30,15 +31,14 @@
     FIELDS_EFFECT = ("beta", "odds_ratio", "hazard_ratio")
     FIELDS_OPTIONAL = ("variant_id", "rsid", "info", "ci_upper", "ci_lower", "ref_allele")
 
     def __init__(self, sumstats_file: Path, delimiter: str = None) -> None:
         self.filename = str(sumstats_file)
         self.delimiter = delimiter if delimiter else self._get_delimiter(sumstats_file)
         self.sumstats = self.from_file(infile=self.filename)
-        self.sumstats_df = None
 
     def reformat_header(self, header_map: dict = FIELD_MAP) -> etl.Table:
         """Reformats the headers according to the standard
 
         Returns:
             etl.Table
         """
@@ -62,21 +62,29 @@
             infile -- Input file
 
         Returns:
             petl Table or None
         """
         try:
             self.sumstats = etl.fromcsv(self.filename, delimiter=self.delimiter)
-            if etl.nrows(self.head_table(nrows=1)) < 1:
+            if not self.is_table_content():
                 return None
             return self.sumstats
         except (IOError, UnicodeDecodeError) as exception:
             print(exception)
             return None
 
+    def is_table_content(self) -> bool:
+        """Bool for whether table content exists
+
+        Returns:
+            Boolean
+        """
+        return etl.nrows(self.head_table(nrows=1)) > 0
+    
     def to_file(self, outfile: Path) -> None:
         """Write table to TSV file
 
         Arguments:
             outfile -- Output file name
         """
         self.sumstats.totsv(str(outfile))
@@ -172,27 +180,27 @@
 
     def header(self) -> tuple:
         """Get the header of the file
 
         Returns:
             tuple of the headers
         """
-        if self.sumstats:
+        if self.is_table_content():
             return etl.header(self.sumstats)
         return ()
 
     def effect_field(self) -> Union[str, None]:
         """Get the effect allele (field index 4).
 
         Returns:
             effect field label
         """
         field_4 = self._get_field_label_from_index(4)
         return field_4
-    
+
     def p_value_field(self) -> Union[str, None]:
         """Get the p_value field (field index 7).
 
         Returns:
             p_value field label
         """
         field_4 = self._get_field_label_from_index(7)
@@ -215,39 +223,71 @@
                                     'e|E',
                                     newfields=['_p_value_mantissa',
                                                '_p_value_exponent'],
                                     include_original=True,
                                     maxsplit=1)
         return table_w_split_p
 
+    def pval_to_mantissa_and_exponent(self, df: pd.DataFrame) -> pd.DataFrame:
+        """Create the mantissa and exponent columns from the pvalue field.
+        First a row needs to be appended (we use index -99) with the delimiter,
+        else the split cannot be done if no delimiters were found. The row is
+        removed by index before returning the dataframe.
+
+        Arguments:
+            df -- dataframe
+
+        Returns:
+            dataframe
+        """
+        mant_and_exp = ['_p_value_mantissa', '_p_value_exponent']
+        psplit_row = pd.Series({self.p_value_field(): '1000e1000'}, name=-99)
+        df = pd.concat([df, psplit_row.to_frame().T], ignore_index=False)
+        df[mant_and_exp] = (df[self.p_value_field()]
+                            .str.split(r"e|E",
+                                       regex=True,
+                                       n=1,
+                                       expand=True))
+        df = df.drop(index=-99)
+        return df
+
     def _prep_table_for_validation(self) -> etl.Table:
         table = etl.Table()
-        if self.sumstats:
+        if self.is_table_content():
             table = self._pval_to_mantissa_and_exponent(table=self.sumstats)
         return table
 
-    def as_pd_df(self, nrows: int = None) -> pd.DataFrame:
-        """Sumstats table as a Pandas dataframe
+    def as_pd_df(self,
+                 nrows: int = None,
+                 chunksize: int = None,
+                 skiprows: int = None) -> Union[pd.DataFrame, TextFileReader]:
+        """Sumstats table as a Pandas dataframe or dataframe
+        iterator (TextFileReader)
 
         Keyword Arguments:
             nrows -- Number of rows (default: {None, which means all rows})
+            chunksize -- Number of rows to store in mem at once
+            skiprows -- Number of rows to skip from start of file
 
         Returns:
-            Pandas dataframe
+            Pandas dataframe or iter
         """
-
         df = pd.DataFrame()
-        if self.sumstats:
-            table_to_validate = self._square_up_table(self._prep_table_for_validation())
-            df = etl.todataframe(table_to_validate, nrows=nrows)
-            df = df.replace([None, "", "#NA", "NA", "N/A", "NaN"], np.nan)
+        skip = range(1, skiprows) if skiprows else None
+        if self.is_table_content():
+            df = pd.read_table(self.filename,
+                               sep=self.delimiter,
+                               chunksize=chunksize,
+                               nrows=nrows,
+                               na_values=["", "#NA", "NA", "N/A", "NaN", "NR"],
+                               dtype=str,
+                               skiprows=skip
+                               )
         return df
-    
-    def _square_up_table(self, table: etl.Table, missing: str="#NA") -> etl.Table:
+
+    def _square_up_table(self, table: etl.Table, missing: str = "#NA") -> etl.Table:
         """Square up a table with missing/extra values on rows.
 
         Returns:
             etl.Table
         """
         return etl.cat(table, missing=missing)
-
-
```

### Comparing `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/interfaces/metadata.py` & `gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/interfaces/metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,16 @@
                                         GWAS_CAT_SAMPLE_MAPPINGS,
                                         GENOME_ASSEMBLY_MAPPINGS)
 from gwas_sumstats_tools.utils import (download_with_requests,
                                        parse_accession_id,
                                        parse_genome_assembly,
                                        get_md5sum,
                                        replace_dictionary_keys,
-                                       split_fields_on_delimiter)
+                                       split_fields_on_delimiter,
+                                       update_dict_if_not_set)
 from gwas_sumstats_tools.schema.metadata import SumStatsMetadata
 
 
 class MetadataClient:
     def __init__(self, meta_dict: dict = {},
                  in_file: Path = None,
                  out_file: Path = None) -> None:
@@ -159,33 +160,34 @@
                 if fields_to_split:
                     element = split_fields_on_delimiter(data_dict=element,
                                                         fields=fields_to_split)
                 formatted_list.append(element)
     return formatted_list
 
 
-def get_file_metadata(in_file: Path, out_file: str) -> dict:
+def get_file_metadata(in_file: Path, out_file: str, meta_dict: dict = {}) -> dict:
     """Get file related metadata
 
     Arguments:
         in_file -- sumstats in file
         outfile -- sumstats out file
 
     Returns:
         Metadata dict
     """
-    meta_dict = {}
-    accession_id = parse_accession_id(filename=in_file) 
-    meta_dict['gwas_id'] = accession_id
-    meta_dict['data_file_name'] = Path(out_file).name
-    meta_dict['file_type'] = 'GWAS-SFF v1.0'
-    meta_dict['genome_assembly'] = GENOME_ASSEMBLY_MAPPINGS.get(parse_genome_assembly(filename=in_file), 'unknown')
-    meta_dict['data_file_md5sum'] = get_md5sum(out_file) if Path(out_file).exists() else None
-    meta_dict['date_last_modified'] = date.today()
-    meta_dict['gwas_catalog_api'] = GWAS_CAT_API_STUDIES_URL + accession_id
+    inferred_meta_dict = {}
+    inferred_meta_dict['gwas_id'] = parse_accession_id(filename=in_file)
+    inferred_meta_dict['data_file_name'] = Path(out_file).name
+    inferred_meta_dict['file_type'] = 'GWAS-SFF v1.0'
+    inferred_meta_dict['genome_assembly'] = GENOME_ASSEMBLY_MAPPINGS.get(parse_genome_assembly(filename=in_file), 'unknown')
+    inferred_meta_dict['data_file_md5sum'] = get_md5sum(out_file) if Path(out_file).exists() else None
+    inferred_meta_dict['date_last_modified'] = date.today()
+    inferred_meta_dict['gwas_catalog_api'] = GWAS_CAT_API_STUDIES_URL + parse_accession_id(filename=in_file)
+    for field, value in inferred_meta_dict.items():
+        update_dict_if_not_set(meta_dict, field, value)
     return meta_dict
 
 
 def init_metadata_from_file(filename: Path, metadata_infile: Path = None) -> Union[SumStatsMetadata, None]:
     m_in = metadata_infile if metadata_infile else filename.with_suffix(filename.suffix + "-meta.yaml")
     if m_in.exists():
         ssm = MetadataClient(in_file=m_in)
```

### Comparing `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/read.py` & `gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/read.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/schema/data_table.py` & `gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/schema/data_table.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/schema/metadata.py` & `gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/schema/metadata.py`

 * *Files identical despite different names*

### Comparing `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/utils.py` & `gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,20 @@
 
     Returns:
         dict with keys replaced
     """
     return {replace_dict.get(k, k): v for k, v in data_dict.items()}
 
 
+def update_dict_if_not_set(data_dict: dict, field: str, value: any) -> dict:
+    if data_dict.get(field) is None:
+        data_dict[field] = value
+    return data_dict
+
+
 def split_fields_on_delimiter(data_dict: dict,
                               fields: tuple,
                               delimiter: str = "|") -> dict:
     """Split specified fields in dict on delimiter
 
     Arguments:
         data_dict -- dict to split fields in
```

### Comparing `gwas_sumstats_tools-1.0.0a3/gwas_sumstats_tools/validate.py` & `gwas_sumstats_tools-1.0.1a0/gwas_sumstats_tools/validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from typing import Union
 from pathlib import Path
 import pandas as pd
 import petl as etl
 from pandera import errors
+from rich import print
 
 from gwas_sumstats_tools.schema.data_table import SumStatsSchema
 from gwas_sumstats_tools.interfaces.data_table import SumStatsTable
 from gwas_sumstats_tools.interfaces.metadata import init_metadata_from_file
 
 
 class Validator(SumStatsTable):
     def __init__(self,
                  sumstats_file: Path,
                  pval_zero: bool = False,
                  minimum_rows: int = 100_000,
                  sample_size: int = 100_000,
+                 chunksize: int = 1_000_000,
                  **kwargs) -> None:
         super().__init__(sumstats_file=sumstats_file)
         self.pval_zero = pval_zero
         self.errors_table = None
         self.minimum_rows = minimum_rows
         self.sample_size = sample_size
+        self.chunksize = chunksize
         self.primary_error_type = None
         self.valid = None
 
     def schema(self) -> SumStatsSchema:
         effect_field = self.effect_field() if self.effect_field() in \
             SumStatsSchema().EFFECT_FIELD_DEFINITIONS else 'beta'
         p_value_field = self.p_value_field() if self.p_value_field() in \
@@ -39,27 +42,42 @@
         First validate a sample of 100,000 records,
         if this sample is valid, validate the rest of
         the data.
 
         Returns:
             Validation status, message
         """
+        print("Validating extension")
         self.valid, message = self._validate_file_ext()
         if self.valid:
+            print("--> [green]Ok[/green]")
+            print("Validating column order")
             self.valid, message = self._validate_field_order()
         if self.valid:
+            print("--> [green]Ok[/green]")
             nrows = max(self.sample_size, self.minimum_rows)
+            print("Validating minimum row count")
             sample_df = self.as_pd_df(nrows=nrows)
             self.valid, message = self._minrow_check(df=sample_df)
         if self.valid:
-            self.valid, message = self._validate_df(sample_df,
-                                                    message=f"Validated the first {nrows} rows.")
+            print("--> [green]Ok[/green]")
+            print(f"Validating the first {nrows} rows")
+            self.valid, message = self._validate_df(sample_df)
         if self.valid:
-            full_df = self.as_pd_df()
-            self.valid, message = self._validate_df(full_df)
+            print("--> [green]Ok[/green]")
+            print("Validating the rest of the file")
+            try:
+                df_iter = self.as_pd_df(chunksize=self.chunksize,
+                                        skiprows=nrows)
+                for df in df_iter:
+                    self.valid, message = self._validate_df(df)
+                    if self.valid is False:
+                        break
+            except pd.errors.EmptyDataError:
+                print("Nothing left to validate")
         self._evaluate_errors()
         return self.valid, message
 
     def write_errors_to_file(self) -> None:
         """Write the error df to a CSV file
         """
         errors_out = self.filename + ".err.csv.gz"
@@ -97,14 +115,15 @@
             sample_size -- Number of rows (default: {None})
             message -- Custom error message (default: {"Errors were found in data"})
 
         Returns:
             Validation status, message
         """
         try:
+            dataframe = self.pval_to_mantissa_and_exponent(dataframe)
             self.schema().schema().validate(dataframe, lazy=True)
             valid = True
             message = "Data table is valid."
             self.errors_table = None
             self.primary_error_type = None
         except errors.SchemaErrors as err:
             self.errors_table = etl.fromdataframe(err.failure_cases) if len(err.failure_cases) > 0 else None
@@ -142,14 +161,15 @@
                 self.primary_error_type = 'data'
 
 
 def validate(filename: Path,
              errors_file: bool = False,
              pval_zero: bool = False,
              minimum_rows: int = 100_000,
+             chunksize: int = 1_000_000,
              infer_from_metadata: bool = False) -> tuple[bool,
                                                          str,
                                                          Union[etl.Table, None],
                                                          Union[str, None]
                                                          ]:
     """Validate driver function
 
@@ -172,15 +192,16 @@
         if ssm:
             if pval_zero is False:
                 pval_zero = True if ssm.as_dict().get('analysisSoftware') is not None else False
         else:
             print("Cannot infer options from metadata file, because metadata file cannot be found.")
     validator = Validator(pval_zero=pval_zero,
                           minimum_rows=minimum_rows,
-                          sumstats_file=filename)
+                          sumstats_file=filename,
+                          chunksize=chunksize)
     valid, message = validator.validate()
     if not valid:
         if validator.errors_table:
             error_preview = validator.errors_table.head(10)
         if errors_file and validator.errors_table:
             message += f"\n[green]Writing errors --> {filename}.err.csv.gz[/green]"
             validator.write_errors_to_file()
```

### Comparing `gwas_sumstats_tools-1.0.0a3/pyproject.toml` & `gwas_sumstats_tools-1.0.1a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwas-sumstats-tools"
-version = "1.0.0a3"
+version = "1.0.1a0"
 description = ""
 authors = ["jdhayhurst <jhayhurst@ebi.ac.uk>"]
 readme = "README.md"
 packages = [{include = "gwas_sumstats_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gwas_sumstats_tools-1.0.0a3/PKG-INFO` & `gwas_sumstats_tools-1.0.1a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwas-sumstats-tools
-Version: 1.0.0a3
+Version: 1.0.1a0
 Summary: 
 Author: jdhayhurst
 Author-email: jhayhurst@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -16,108 +16,119 @@
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # GWAS SumStats Tools
 
 
-A basic toolkit for reading and formatting GWAS sumstats files from the GWAS Catalog.
+A simple toolkit for reading and formatting GWAS sumstats files from the GWAS Catalog.
 Built with:
 * [Petl](https://petl.readthedocs.io/en/stable/index.html)
 * [Pydantic](https://docs.pydantic.dev/)
 * [Typer](https://typer.tiangolo.com/)
 
-There are three commands, `read`, `validate` and `format`.
+There are three commands, `validate`, `read` and `format`.
+
+
+`validate` is for:
+* Validating a summary statistic file using a dynamically generated schema
 
 `read` is for:
 * Previewing a data file: _no options_
 * Extracting the field headers: `-h`
 * Extracting all the metadata: `-M`
 * Extacting specific field, value pairs from the metada: `-m <field name>`
-
-`validate` is for:
-* Validating a summary statistic file using a dynamically generated schema
+* More functionality is to come...
 
 `format` is for:
 * Converting a minamally formatted sumstats data file to the standard format. This is not guaranteed to return a valid standard file, because manadatory data fields could be missing in the input. It simply does the following. `-s`
   * Renames `variant_id` -> `rsid`
   * Reorders the fields
   * Converts `NA` missing values to `#NA`
   * It is memory efficient and will take approx. 30s per 1 million records
 * Generate metadata for a data file: `-m`
   * Read metadata in from existing file: `--meta-in <file>`
   * Create metadata from the GWAS Catalog (internal use, requires authenticated API): `-g`
   * Edit/add the values to the metadata: `-e` with `--<FIELD>=<VALUE>`
 
+## Requirements
+- python >= 3.9
+
 ## Installation
 ```console
 $ pip install gwas-sumstats-tools
 ```
 
 ## Usage
 
+<p align="center"><img src="gwas-demo.gif"/></p>
+
 ```console
 $ gwas-ssf [OPTIONS] COMMAND [ARGS]...
 ```
 
 **Options**:
 
 * `--help`: Show this message and exit.
 
 **Commands**:
 
-* `format`: Format a sumstats file and...
+* `validate`: Validate a sumstats file
+* `format`: Format a sumstats file
 * `read`: Read a sumstats file
 
-### `gwas-ssf read`
 
-Read (preview) a sumstats file
+### `gwas-ssf validate`
+
+Validate a sumstats file
+
 
 **Usage**:
 
 ```console
-$ gwas-ssf read [OPTIONS] FILENAME
+$ gwas-ssf validate [OPTIONS] FILENAME
 ```
 
 **Arguments**:
 
-* `FILENAME`: Input sumstats file  [required]
+* `FILENAME`: Input sumstats file. Must be TSV (may be gzipped) [required]
 
 **Options**:
 
-* `-h, --get-header`: Just return the headers of the file  [default: False]
-* `--meta-in PATH`: Specify a metadata file to read in, defaulting to <filename>-meta.yaml
-* `-M, --get-all-metadata`: Return all metadata  [default: False]
-* `-m, --get-metadata TEXT`: Get metadata for the specified fields e.g. `-m genomeAssembly -m isHarmonised
+* `-e, --errors-out`: Output erros to a csv file, <filename>.err.csv.gz
+* `-z, --p-zero`: Force p-values of zero to be allowable. Takes precedence over inferred value (-i)
+* `-m, --min-rows`:  Minimum rows acceptable for the file [default: 100000]
+* `-i, --infer-from-metadata`: Infer validation options from the metadata file <filename>-meta.yaml. E.g. a populated field for analysis software makes p-values of zero allowable.
 * `--help`: Show this message and exit.
 
 
-### `gwas-ssf validate`
+### `gwas-ssf read`
 
-Validate a sumstats file
+Read (preview) a sumstats file
 
 **Usage**:
 
 ```console
-$ gwas-ssf validate [OPTIONS] FILENAME
+$ gwas-ssf read [OPTIONS] FILENAME
 ```
 
 **Arguments**:
 
-* `FILENAME`: Input sumstats file. Must be TSV or CSV and may be gzipped [required]
+* `FILENAME`: Input sumstats file  [required]
 
 **Options**:
 
-* `-e, --errors-out`: Output erros to a csv file, <filename>.err.csv.gz
-* `-z, --p-zero`: Force p-values of zero to be allowable. Takes precedence over inferred value (-i)
-* `-n, --p-neg-log`: Force p-values to be validated as -log10. Takes precedence over inferred value (-i)
-* `-m, --min-rows`:  Minimum rows acceptable for the file [default: 100000]
-* `-i, --infer-from-metadata`: Infer validation options from the metadata file <filename>-meta.yaml. E.g. fields for analysis software and negative log10 p-values affect the data validation behaviour.
+* `-h, --get-header`: Just return the headers of the file  [default: False]
+* `--meta-in PATH`: Specify a metadata file to read in, defaulting to <filename>-meta.yaml
+* `-M, --get-all-metadata`: Return all metadata  [default: False]
+* `-m, --get-metadata TEXT`: Get metadata for the specified fields e.g. `-m genomeAssembly -m isHarmonised
 * `--help`: Show this message and exit.
 
+
+
 ### `gwas-ssf format`
 
 Format a sumstats file and creating a new one. Add/edit metadata.
 
 **Usage**:
 
 ```console
@@ -148,7 +159,10 @@
 1. [install poetry](https://python-poetry.org/docs/#installation)
 
 2. `git clone https://github.com/EBISPOT/gwas-sumstats-tools.git`
 3. `cd gwas-sumstats-tools`
 4. `poetry install`
 5. `poetry run pytest`
 
+To make a change:
+branch from master -> PR to master -> poetry version -> git add pyproject.toml -> git commit -> git tag <version> -> git push origin master --tags
+If all the tests pass, this will publish to pypi.
```

