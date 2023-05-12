# Comparing `tmp/tabdoc-1.0.2-py3-none-any.whl.zip` & `tmp/tabdoc-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5307685 bytes, number of entries: 12
--rw-r--r--  2.0 unx      205 b- defN 23-Apr-27 18:51 tabdoc/__init__.py
+Zip file size: 5306943 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      205 b- defN 23-May-03 15:37 tabdoc/__init__.py
 -rw-r--r--  2.0 unx     7681 b- defN 23-Apr-27 17:15 tabdoc/tabexcel.py
 -rw-r--r--  2.0 unx    10330 b- defN 19-Oct-15 10:31 tabdoc/tabpdf.py
--rw-r--r--  2.0 unx     8081 b- defN 23-Apr-27 17:14 tabdoc/tabword.py
+-rw-r--r--  2.0 unx    16014 b- defN 23-May-10 05:13 tabdoc/tabword.py
 -rw-r--r--  2.0 unx 10063973 b- defN 19-Feb-13 10:22 tabdoc/templates/SimHei.ttf
 -rw-r--r--  2.0 unx      112 b- defN 19-Jul-25 12:59 tabdoc/templates/__init__.py
--rw-r--r--  2.0 unx    20235 b- defN 19-Feb-13 05:45 tabdoc/templates/template.docx
--rw-r--r--  2.0 unx     1066 b- defN 23-Apr-27 18:52 tabdoc-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1272 b- defN 23-Apr-27 18:52 tabdoc-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-27 18:52 tabdoc-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-27 18:52 tabdoc-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      937 b- defN 23-Apr-27 18:52 tabdoc-1.0.2.dist-info/RECORD
-12 files, 10113991 bytes uncompressed, 5306135 bytes compressed:  47.5%
+-rw-r--r--  2.0 unx    17822 b- defN 23-May-04 09:15 tabdoc/templates/template.docx
+-rw-r--r--  2.0 unx     1066 b- defN 23-May-10 05:14 tabdoc-1.0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1272 b- defN 23-May-10 05:14 tabdoc-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 05:14 tabdoc-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-10 05:14 tabdoc-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      938 b- defN 23-May-10 05:14 tabdoc-1.0.3.dist-info/RECORD
+12 files, 10119512 bytes uncompressed, 5305393 bytes compressed:  47.6%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: tabdoc/templates/__init__.py
 Comment: 
 
 Filename: tabdoc/templates/template.docx
 Comment: 
 
-Filename: tabdoc-1.0.2.dist-info/LICENSE
+Filename: tabdoc-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: tabdoc-1.0.2.dist-info/METADATA
+Filename: tabdoc-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: tabdoc-1.0.2.dist-info/WHEEL
+Filename: tabdoc-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: tabdoc-1.0.2.dist-info/top_level.txt
+Filename: tabdoc-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: tabdoc-1.0.2.dist-info/RECORD
+Filename: tabdoc-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tabdoc/__init__.py

```diff
@@ -3,12 +3,12 @@
 
 """
 @author: guoyanfeng
 @software: PyCharm
 @time: 19-3-20 下午6:29
 """
 
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 
 from .tabexcel import *
 from .tabpdf import *
 from .tabword import *
```

## tabdoc/tabword.py

```diff
@@ -4,23 +4,56 @@
 """
 @author: guoyanfeng
 @software: PyCharm
 @time: 19-2-11 下午6:14
 """
 from collections import MutableSequence
 from itertools import zip_longest
-from typing import List
+from typing import Any, List, Optional, Tuple, Union
 
 from docx import Document, document, table
 from docx.enum.table import WD_CELL_VERTICAL_ALIGNMENT, WD_ROW_HEIGHT_RULE, WD_TABLE_ALIGNMENT
 from docx.enum.text import WD_PARAGRAPH_ALIGNMENT
+from docx.oxml import OxmlElement, parse_xml
+from docx.oxml.ns import nsdecls, qn
 from docx.shared import Inches, Pt, RGBColor
+# noinspection PyProtectedMember
+from docx.table import _Cell, _Row
+from docx.text.run import Run
 from path import Path
 
-__all__ = ("WordWriter",)
+__all__ = ("WordWriter", "ValueAttr")
+
+
+class ValueAttr(object):
+    """
+    单元格值属性
+    """
+
+    def __init__(self, value: Any, bgcolor: Optional[str] = None, halignment: str = "center", is_bold: bool = False):
+        """
+            单元格值属性
+        Args:
+            value: 表格值
+            bgcolor: 表格背景颜色
+            halignment: 单元格水平对齐方式
+            is_bold: 是否加粗
+        """
+        self.value: Any = value
+        self.bgcolor: Optional[str] = bgcolor
+        halignment_lower = halignment.lower()
+        if halignment_lower == "center":
+            self.halignment: str = WD_TABLE_ALIGNMENT.CENTER
+        elif halignment_lower == "left":
+            self.halignment = WD_TABLE_ALIGNMENT.LEFT
+        elif halignment_lower == "right":
+            self.halignment = WD_TABLE_ALIGNMENT.RIGHT
+        else:
+            self.halignment: str = WD_TABLE_ALIGNMENT.CENTER
+        self.is_bold: bool = is_bold
 
 
 class WordWriter(object):
     """
     word writer
     """
 
@@ -66,24 +99,27 @@
         for i, val in enumerate(row):
             if hasattr(val, "strftime"):
                 row[i] = val.strftime("%Y-%m-%d %H:%M:%S")
             elif hasattr(val, 'isoformat'):
                 row[i] = val.isoformat()
         return tuple(row)
 
-    def add_table(self, header_name: str, header_data: MutableSequence, table_data: MutableSequence,
-                  merge_cells: list = None, unit=None):
+    def add_table(self, header_name: str, header_data: List[List[Union[ValueAttr, str]]],
+                  table_data: List[List[Union[ValueAttr, str]]],
+                  merge_cells: List[Tuple[Tuple[int, int], Tuple[int, int]]] = None,
+                  unit=None, body_fontsize=10):
         """
         为Word文档中添加表格
         Args:
             header_name: 表格的表头文字
             header_data: 表格的表头数据，可能有多个
             table_data: 表格的body数据，可能有多个
             merge_cells: 要合并的单元格
             unit: 表格数据的单位
+            body_fontsize: body的字号大小
         Returns:
 
         """
         if not isinstance(header_data, MutableSequence):
             raise ValueError("header data值类型错误,请检查")
         if not isinstance(table_data, MutableSequence):
             raise ValueError("table data值类型错误,请检查")
@@ -94,15 +130,15 @@
                 raise ValueError("header data值类型错误,请检查")
         for value in table_data:
             if not isinstance(value, MutableSequence):
                 raise ValueError("table data值类型错误,请检查")
 
         p = self.document.add_paragraph(style="p-first-line-not-indent-center")
         p.alignment = WD_PARAGRAPH_ALIGNMENT.CENTER
-        bold_run = p.add_run(header_name)
+        bold_run: Run = p.add_run(header_name)
         bold_run.font.size = Pt(12)
         bold_run.font.bold = True
 
         if unit:
             unit_p = self.document.add_paragraph()
             unit_p.alignment = WD_PARAGRAPH_ALIGNMENT.RIGHT
             unit_body = unit_p.add_run(f"单位：{unit}")
@@ -126,27 +162,195 @@
         # 设置表居中和自适应
         table_.alignment = WD_TABLE_ALIGNMENT.CENTER
         table_.autofit = True
         # 添加表头，表头有可能有多行
         for index, header in enumerate(header_data):
             row = table_.rows[index]
             row.height_rule = WD_ROW_HEIGHT_RULE.AUTO
-            for i, val in enumerate(header):
-                if not row.cells[i].text:
-                    row.cells[i].text = str(val)
-                row.cells[i].vertical_alignment = WD_CELL_VERTICAL_ALIGNMENT.CENTER  # 垂直居中
+            for col_index, cell_value in enumerate(header):
+                self._add_cell_value(row.cells[col_index], cell_value, body_fontsize)
         # 添加表体
-        for data in table_data:
+        for row_data in table_data:
             row = table_.add_row()
             row.height_rule = WD_ROW_HEIGHT_RULE.AUTO
-            for i, val in enumerate(data):
-                row.cells[i].text = str(val)
-                row.cells[i].vertical_alignment = WD_CELL_VERTICAL_ALIGNMENT.CENTER
+            for col_index, cell_value in enumerate(row_data):
+                self._add_cell_value(row.cells[col_index], cell_value, body_fontsize)
+
+        self.document.add_paragraph()  # 增加一个空行的段落
+
+    def add_table2(self, header_name: str, rows_cols: Tuple[int, int],
+                   table_data: List[List[Union[ValueAttr, str]]],
+                   merge_cells: List[Tuple[Tuple[int, int], Tuple[int, int]]] = None,
+                   unit=None, body_fontsize=10):
+        """
+        为Word文档中添加表格
+        Args:
+            header_name: 表格的表头文字
+            rows_cols: 报表的行列
+            table_data: 表格的body数据，可能有多个
+            merge_cells: 要合并的单元格
+            unit: 表格数据的单位
+            body_fontsize: body的字号大小
+        Returns:
+
+        """
+        if not isinstance(table_data, MutableSequence):
+            raise ValueError("table data值类型错误,请检查")
+        if not isinstance(merge_cells, MutableSequence):
+            raise ValueError("merge cells值类型错误,请检查")
+        for value in table_data:
+            if not isinstance(value, MutableSequence):
+                raise ValueError("table data值类型错误,请检查")
+
+        p = self.document.add_paragraph(style="p-first-line-not-indent-center")
+        p.alignment = WD_PARAGRAPH_ALIGNMENT.CENTER
+        bold_run: Run = p.add_run(header_name)
+        bold_run.font.size = Pt(12)
+        bold_run.font.bold = True
+
+        if unit:
+            unit_p = self.document.add_paragraph()
+            unit_p.alignment = WD_PARAGRAPH_ALIGNMENT.RIGHT
+            unit_body = unit_p.add_run(f"单位：{unit}")
+            unit_body.font.size = Pt(10.5)
+
+        # analysis-data需要模板中指定，指定的方式要简单很多
+        table_: table.Table = self.document.add_table(*rows_cols, "analysis-data")
+        for value in merge_cells:
+            if not isinstance(value, MutableSequence) and len(value) != 2:
+                raise ValueError("merge cells值类型错误,请检查")
+            for row_index, col_index in value:
+                if row_index > rows_cols[0] or col_index > rows_cols[1]:
+                    raise ValueError("merge cells值错误,请检查")
+
+        # 合并单元格
+        if merge_cells:
+            for cell, other_cell in merge_cells:
+                table_.cell(*cell).merge(table_.cell(*other_cell))
+        # 设置表居中和自适应
+        table_.alignment = WD_TABLE_ALIGNMENT.CENTER
+        table_.autofit = True
+        # 添加表头，添加表体
+        for index, row_data in enumerate(table_data):
+            row = table_.rows[index]
+            row.height_rule = WD_ROW_HEIGHT_RULE.AUTO
+            for col_index, cell_value in enumerate(row_data):
+                self._add_cell_value(row.cells[col_index], cell_value, body_fontsize)
+
         self.document.add_paragraph()  # 增加一个空行的段落
 
+    def _add_cell_value(self, cell: _Cell, cell_value: Union[ValueAttr, str], fontsize: int):
+        """
+        添加单元格的值和样式
+        Args:
+            cell: 表格中的单元格
+            cell_value: 单元格值
+            fontsize: 字号大小
+        Returns:
+
+        """
+        if isinstance(cell_value, ValueAttr):
+            # cell.text = str(cell_value.value)
+            # 因为样式中的字号无效，只能手动设置字号
+            cell_body = cell.paragraphs[0].add_run(str(cell_value.value))
+            cell_body.font.size = Pt(fontsize)
+            if cell_value.is_bold:
+                cell_body.font.bold = True
+
+            if cell_value.bgcolor:
+                self.set_cell_bgcolor(cell, cell_value.bgcolor)
+            if cell_value.halignment:
+                self.set_cell_halignment(cell, cell_value.halignment)  # 水平对齐
+        else:
+            # cell.text = str(cell_value)
+            # 因为样式中的字号无效，只能手动设置字号
+            cell_body = cell.paragraphs[0].add_run(str(cell_value))
+            cell_body.font.size = Pt(fontsize)
+            self.set_cell_halignment(cell, WD_TABLE_ALIGNMENT.CENTER)  # 水平居中
+        cell.vertical_alignment = WD_CELL_VERTICAL_ALIGNMENT.CENTER  # 垂直居中
+
+    @staticmethod
+    def set_cell_halignment(cell: _Cell, alignment: str = WD_TABLE_ALIGNMENT.CENTER):
+        """
+        设置单元格的水平对齐方式
+
+        默认为水平居中
+        Args:
+            cell: 单元格
+            alignment: 对齐方式默认居中
+        Returns:
+
+        """
+        cell.paragraphs[0].paragraph_format.alignment = alignment
+
+    @staticmethod
+    def set_cell_bgcolor(cell: _Cell, rgbcolor: str):
+        """
+        设置单元格的背景颜色
+        Args:
+            cell: 单元格
+            rgbcolor: 要设置的RGB颜色
+        Returns:
+
+        """
+        bgcolor_style = parse_xml(r'<w:shd {} w:fill="{}"/>'.format(nsdecls('w'), rgbcolor))
+        # noinspection PyProtectedMember
+        cell._tc.get_or_add_tcPr().append(bgcolor_style)
+
+    def set_row_bgcolor(self, row: _Row, rgbcolor: str):
+        """
+        设整行的背景颜色
+        Args:
+            row: 要设置的整行
+            rgbcolor: 要设置的RGB颜色
+        Returns:
+
+        """
+        for cell in row.cells:
+            self.set_cell_bgcolor(cell, rgbcolor)
+
+    @staticmethod
+    def set_cell_borders(cell: _Cell, **kwargs):
+        """
+        Set cell`s border
+        Usage:
+        set_cell_border(
+            cell,
+            top={"sz": 12, "val": "single", "color": "#FF0000", "space": "0"},
+            bottom={"sz": 12, "color": "#00FF00", "val": "single"},
+            start={"sz": 24, "val": "dashed", "shadow": "true"},
+            end={"sz": 12, "val": "dashed"},
+        )
+        """
+        # noinspection PyProtectedMember
+        tc_pr = cell._tc.get_or_add_tcPr()
+
+        # check for tag existnace, if none found, then create one
+        tc_borders = tc_pr.first_child_found_in("w:tcBorders")
+        if tc_borders is None:
+            tc_borders = OxmlElement('w:tcBorders')
+            tc_pr.append(tc_borders)
+
+        # list over all available tags
+        for edge in ('start', 'top', 'end', 'bottom', 'insideH', 'insideV'):
+            edge_data = kwargs.get(edge)
+            if edge_data:
+                tag = 'w:{}'.format(edge)
+
+                # check for tag existnace, if none found, then create one
+                element = tc_borders.find(qn(tag))
+                if element is None:
+                    element = OxmlElement(tag)
+                    tc_borders.append(element)
+
+                # looks like order of attributes is important
+                for key in ["sz", "val", "color", "space", "shadow"]:
+                    if key in edge_data:
+                        element.set(qn('w:{}'.format(key)), str(edge_data[key]))
+
     def add_paragraph(self, bold_text: List[str] = None, *, other_text: List[str] = None):
         """
         为Word文档中添加段落
         Args:
             bold_text: 段落开头需要加粗的文本
             other_text: 段落正文的内容
         Returns:
```

## tabdoc/templates/template.docx

 * *Format-specific differences are supported for Microsoft Word .docx files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Microsoft Word 2007+*

```diff
@@ -1,1265 +1,1114 @@
-00000000: 504b 0304 1400 0600 0800 0000 2100 6773  PK..........!.gs
-00000010: 282f 9701 0000 2809 0000 1300 0802 5b43  (/....(.......[C
-00000020: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
-00000030: 6c20 a204 0228 a000 0200 0000 0000 0000  l ...(..........
-00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 00c4 96cb 6ac3 3010  ............j.0.
-00000240: 45f7 85fe 83d1 b6d8 4a52 28a5 c4c9 a28f  E.......JR(.....
-00000250: 651b 68fa 018a 348e 4d6d 4948 93d7 df77  e.h...4.MmIH...w
-00000260: 1c3b a194 2436 4d4c 3606 7966 eeb9 3332  .;..$6ML6.yf..32
-00000270: 9686 e375 9107 4b70 3e33 3a66 fda8 c702  ...u..Kp>3:f....
-00000280: d0d2 a84c cf63 f635 7d0b 1f59 e051 6825  ...L.c.5}..Y.Qh%
-00000290: 72a3 2166 1bf0 6c3c babd 194e 3716 7c40  r.!f..l<...N7.|@
-000002a0: d5da c72c 45b4 4f9c 7b99 4221 7c64 2c68  ...,E.O.{.B!|d,h
-000002b0: 8a24 c615 0269 e9e6 dc0a f92d e6c0 07bd  .$...i.....-....
-000002c0: de03 9746 2368 0cb1 d460 a3e1 0b24 6291  ...F#h...`...$b.
-000002d0: 63f0 baa6 d795 1307 b967 c173 9558 b262  c........g.s.X.b
-000002e0: 26ac cd33 2990 e27c a9d5 1f4a 5813 22aa  &..3)..|...JX.".
-000002f0: dce6 f834 b3fe 8e12 183f 4828 23c7 0175  ...4.....?H(#..u
-00000300: dd07 8dc6 650a 8289 70f8 2e0a cae2 2be3  ....e...p.....+.
-00000310: 1457 462e 0aaa 8c4e cb1c f069 9224 93b0  .WF....N...i.$..
-00000320: af2f d5ac 3312 bca7 9917 79b4 8f14 22d3  ./..3.....y...".
-00000330: 3bff 477d 78dc e4e0 2fef a2d2 6dc6 0322  ;.G}x.../...m.."
-00000340: 1574 61a0 566e b4b0 82d9 6767 2e7e 8937  .ta.Vn....gg.~.7
-00000350: 1a49 8c41 6db0 8bdd d84b 379a 00ad 3af2  .I.Am....K7...:.
-00000360: b053 6eb4 9082 50e0 fa97 7750 09b7 e40f  .Sn...P...wP....
-00000370: aec6 2f37 ab93 fe2b e196 fc0e fa6f c9af  ../7...+.....o..
-00000380: c674 7fe5 f977 c06f 3d7f e289 590e 5d38  .t...w.o=...Y.]8
-00000390: a8a5 1b4d 209d c450 3dcf ff12 b732 a790  ...M ..P=....2..
-000003a0: 9439 71c6 7a3a d9dd 3fda de1d dd65 7548  .9q.z:..?....euH
-000003b0: 0d5b 7098 9dfe d3ec 8924 7d76 7f50 de0a  .[p......$}v.P..
-000003c0: 14a8 036c bebd e78c 7e00 0000 ffff 0300  ...l....~.......
-000003d0: 504b 0304 1400 0600 0800 0000 2100 1e91  PK..........!...
-000003e0: 1ab7 ef00 0000 4e02 0000 0b00 0802 5f72  ......N......._r
-000003f0: 656c 732f 2e72 656c 7320 a204 0228 a000  els/.rels ...(..
-00000400: 0200 0000 0000 0000 0000 0000 0000 0000  ................
-00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000004f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000600: 00ac 92c1 6ac3 300c 40ef 83fd 83d1 bd51  ....j.0.@......Q
-00000610: dac1 18a3 4e2f 63d0 db18 d907 085b 494c  ....N/c......[IL
-00000620: 13db d86a d7fe fd3c d8d8 025d e961 47cb  ...j...<...].aG.
-00000630: d2d3 93d0 7a73 9c46 75e0 945d f01a 9655  ....zs.Fu..]...U
-00000640: 0d8a bd09 d6f9 5ec3 5bfb bc78 0095 85bc  ......^.[..x....
-00000650: a531 78d6 70e2 0c9b e6f6 66fd ca23 4929  .1x.p.....f..#I)
-00000660: ca83 8b59 158a cf1a 0691 f888 98cd c013  ...Y............
-00000670: e52a 44f6 e5a7 0b69 2229 cfd4 6324 b3a3  .*D....i")..c$..
-00000680: 9e71 55d7 f798 7e33 a099 31d5 d66a 485b  .qU...~3..1..jH[
-00000690: 7b07 aa3d 45be 861d bace 197e 0a66 3fb1  {..=E......~.f?.
-000006a0: 9733 2d90 8fc2 deb2 5dc4 54ea 93b8 328d  .3-.....].T...2.
-000006b0: 6a29 f52c 1a6c 302f 259c 9162 ac0a 1af0  j).,.l0/%..b....
-000006c0: bcd1 ea7a a3bf a7c5 8985 2c09 a109 892f  ...z......,..../
-000006d0: fb7c 665c 125a fee7 8ae6 193f 36ef 2159  .|f\.Z.....?6.!Y
-000006e0: b45f e16f 1b9c 5d41 f301 0000 ffff 0300  ._.o..]A........
-000006f0: 504b 0304 1400 0600 0800 0000 2100 f7f2  PK..........!...
-00000700: 9656 3f03 0000 e60b 0000 1100 0000 776f  .V?...........wo
-00000710: 7264 2f64 6f63 756d 656e 742e 786d 6ca4  rd/document.xml.
-00000720: 965b 6fda 3014 80df 27ed 3fa0 bcb7 89c3  .[o.0...'.?.....
-00000730: 3d2a adb6 b256 3c4c 42ed f63c 19c7 2116  =*...V<LB..<..!.
-00000740: f145 b681 b25f bfe3 3801 a6b4 28a4 3c90  .E..._..8...(.<.
-00000750: d83e e73b 179f e3f8 eee1 8d17 bd1d d586  .>.;............
-00000760: 4931 0bd0 6d14 f4a8 2032 6562 3d0b 7eff  I1..m... 2eb=.~.
-00000770: 7aba 9904 3d63 b148 7121 059d 0507 6a82  z...=c.Hq!....j.
-00000780: 87fb af5f eef6 492a c996 5361 7b80 1026  ..._..I*..Sa{..&
-00000790: d92b 320b 726b 5512 8686 e494 6373 cb19  .+2.rkU.....cs..
-000007a0: d1d2 c8cc de12 c943 9965 8cd0 702f 751a  .......C.e..p/u.
-000007b0: c611 8aca 37a5 25a1 c680 bd47 2c76 d804  ....7.%....G,v..
-000007c0: 158e bcb5 a3a5 1aef 41d9 0107 21c9 b1b6  ........A...!...
-000007d0: f4ed c440 5743 86e1 349c 3441 7107 1044  ...@WC..4.4Aq..D
-000007e0: 18a3 26aa 7f35 6a14 3aaf 1aa0 4127 1078  ..&..5j.:...A'.x
-000007f0: d520 0dbb 91de 096e d48d 1437 49e3 6ea4  . .....n...7I.n.
-00000800: 7e93 34e9 466a 9413 6f16 b854 54c0 6226  ~.4.Fj..o..TT.b&
-00000810: 35c7 1686 7a1d 72ac 375b 7503 6085 2d5b  5...z.r.7[u.`.-[
-00000820: b182 d903 30a3 518d c14c 6c3a 7804 5a47  ....0.Q..Ll:x.ZG
-00000830: 02ef a757 13c6 2197 292d fa69 4d91 b360  ...W..!.)-.iM..`
-00000840: ab45 52e9 df1c f59d eb89 d7af 1eb5 866e  .ER............n
-00000850: 13bf 5799 5787 4319 79a8 6901 b990 c2e4  ..W.W.C.y.i.....
-00000860: 4c1d 3b9c 77a5 c162 5e43 7697 82d8 f1a2  L.;.w..b^Cv.....
-00000870: 96db 2bd4 b25d 3e3a 9ee6 3e95 2760 1bf7  ..+..]>:..>.'`..
-00000880: abfc f3c2 7b7e 9988 a216 3be2 1047 8d36  ....{~....;..G.6
-00000890: 2efc 6fb3 f684 4315 9e0c 774a cd59 7251  ..o...C...wJ.YrQ
-000008a0: cb03 a406 c40d c088 b096 255d 337c 3621  ..........%]3|6!
-000008b0: 1ed0 3ce3 187a 1d66 5863 cc81 9f5a 7daf  ..<..z.fXc...Z}.
-000008c0: d69f ab96 672d b7ea 4463 9fa3 2d4e bdbf  ....g-..Dc..-N..
-000008d0: 775f e12b 5855 d59d 7782 f99c 33af 3956  w_.+XU..w...3.9V
-000008e0: 7024 7092 2cd6 426a bc2a c023 a8a1 1e94  p$p.,.Bj.*.#....
-000008f0: 41af dc01 f70f bbd2 734d 17dc c355 6125  A.......sM...Ua%
-00000900: d383 7b2a 5819 240a 6bbc 80dd 8ec6 f3e1  ..{*X.$.k.......
-00000910: e0c7 0405 e52c 1cb4 d6cd 8eab 1fcc 2670  .....,........&p
-00000920: 2d49 5f40 309a 4763 143b 413f b5d4 ef4c  -I_@0.Gc.;A?...L
-00000930: ce69 86b7 856d ae2c dd54 ff31 7a1a 4e4b  .i...m.,.T.1z.NK
-00000940: 6fd4 52bb 8751 9840 3820 b4a2 d030 1004  o.R..Q.@8 ...0..
-00000950: 1a8e 9c0e ce2c d57e 143a 41ed e5f5 9314  .....,.~.:A.....
-00000960: d6c0 7ace 0458 a1d8 d86f 8661 2713 5642  ..z..X...o.a'.VB
-00000970: e111 be92 72e3 be04 af16 3e21 a0e3 aa3b  ....r.....>!...;
-00000980: 7270 8139 58fa f32c bf63 b2f1 fc5a f687  rp.9X..,.c...Z..
-00000990: 488f 921e aa4a 3f29 b14b dd36 1b4e 23a7  H....J?).K.6.N#.
-000009a0: 38a5 fa85 6654 c365 0eb6 23b1 0705 56e9  8...fT.e..#...V.
-000009b0: 8e42 d3eb d284 5ea4 5578 1f49 a73e 9f67  .B....^.Ux.I.>.g
-000009c0: 0a63 af90 4969 5be0 2797 a59b f8e9 657f  .c..Ii[.'.....e.
-000009d0: 32a6 cdb9 382a b3f4 b181 863c f2f2 6afd  2...8*.....<..j.
-000009e0: fa17 84e0 f044 68ea 3ecb 6012 de47 937e  .....Dh.>.`..G.~
-000009f0: e5b1 5aff c42e df56 c219 8f06 8372 df34  ..Z....V.....r.4
-00000a00: 5be7 b0eb 6812 95c3 95b4 56f2 d372 41b3  [...h.....V..rA.
-00000a10: b355 1fc2 2c98 0ccb 5df2 1ece 82e9 3476  .U..,...].....4v
-00000a20: c3f5 d696 c3ca 7f22 0b57 55ae 1cc1 eb41  .......".WU....A
-00000a30: 3cf4 d370 bd7e d6ae 89aa 700a 26e0 eeed  <..p.~....p.&...
-00000a40: 4cc1 cb92 5902 4ef7 515c 558a 2f92 f2d5  L...Y.N.Q\U./...
-00000a50: 375b 78ba a0df ff03 0000 ffff 0300 504b  7[x...........PK
-00000a60: 0304 1400 0600 0800 0000 2100 c5aa b29b  ..........!.....
-00000a70: 4001 0000 3d07 0000 1c00 0801 776f 7264  @...=.......word
-00000a80: 2f5f 7265 6c73 2f64 6f63 756d 656e 742e  /_rels/document.
-00000a90: 786d 6c2e 7265 6c73 20a2 0401 28a0 0001  xml.rels ...(...
-00000aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ba0: b495 cb6e 8330 1045 f795 fa0f c8fb 6220  ...n.0.E......b 
-00000bb0: 6dfa 504c 3655 a56c 5bfa 010e 1e1e 2ad8  m.PL6U.l[.....*.
-00000bc0: c89e 3ef8 fb5a 4121 a445 5616 6639 1779  ..>..ZA!.EV.f9.y
-00000bd0: ee61 ee60 36db 9fb6 09be 409b 5a49 46e2  .a.`6.....@.ZIF.
-00000be0: 3022 01c8 5c89 5a96 8cbc 672f 370f 2430  0"..\.Z...g/7.$0
-00000bf0: c8a5 e08d 92c0 480f 866c d3eb abcd 2b34  ......H..l....+4
-00000c00: 1ced 2153 d59d 096c 1769 18a9 10bb 274a  ..!S...l.i....'J
-00000c10: 4d5e 41cb 4da8 3a90 f649 a174 cbd1 96ba  M^A.M.:..I.t....
-00000c20: a41d cf3f 7809 3489 a235 d5d3 1e24 3deb  ...?x.4..5...$=.
-00000c30: 19ec 0423 7a27 ac7f d677 7049 6f55 1475  ...#z'...wpIoU.u
-00000c40: 0ecf 2aff 6c41 e28c 052d 9442 d0b6 23d7  ..*.lA...-.B..#.
-00000c50: 2520 2343 1d87 b611 a1f3 fef1 ca27 00da  % #C.........'..
-00000c60: b370 f23f 9483 e884 f0ca f00d fb37 40b4  .p.?.........7@.
-00000c70: 099b 13c9 4474 81dc fb04 a980 8b69 1a43  ....Dt.......i.C
-00000c80: 9d38 d348 fcae 83c4 8cef 9b49 22a3 e4a2  .8.H.......I"...
-00000c90: f00a 61fe 6571 549c 83f0 8a80 7d03 5380  ..a.eqT.....}.S.
-00000ca0: 43ed b25f 2fbf 07ee afd2 ebfb cf5f 0b2b  C.._/........_.+
-00000cb0: 17c0 9d4f 7f90 425a c749 0247 c539 8368  ...O..BZ.I.G.9.h
-00000cc0: f910 9c33 b8f5 9dc1 9f21 8c92 0be2 71f9  ...3.....!....q.
-00000cd0: 4518 6f24 7af6 d34b 7f01 0000 ffff 0300  E.o$z..K........
-00000ce0: 504b 0304 1400 0600 0800 0000 2100 0d28  PK..........!..(
-00000cf0: 3c0e 7e02 0000 860a 0000 1200 0000 776f  <.~...........wo
-00000d00: 7264 2f66 6f6f 746e 6f74 6573 2e78 6d6c  rd/footnotes.xml
-00000d10: cc96 db92 9a40 1086 ef53 9577 a0b8 d701  .....@...S.w....
-00000d20: 3cac a1c4 2d37 ae29 efb6 7693 0718 8741  <...-7.)..v....A
-00000d30: a865 0e35 338a be7d 7a40 d404 6321 dec4  .e.53..}z@..c!..
-00000d40: 0b70 0eff 4777 4f77 c3f4 79cf 7267 4795  .p..GwOw..y.rgG.
-00000d50: ce04 8f5c bfef b90e e544 c419 df44 eeaf  ...\.....D...D..
-00000d60: 9fcb dec4 75b4 c13c c6b9 e034 720f 54bb  ....u..<...4r.T.
-00000d70: cfb3 af5f a645 9808 61b8 3054 3bc0 e03a  ..._.E..a.0T;..:
-00000d80: 2c24 89dc d418 1922 a449 4a19 d67d 9611  ,$.....".IJ..}..
-00000d90: 25b4 484c 9f08 8644 9264 84a2 42a8 1805  %.HL...D.d..B...
-00000da0: 9eef 95ff a412 846a 0d0f fc8e f90e 6bf7  .......j......k.
-00000db0: 8823 fb76 b458 e102 c416 3844 24c5 cad0  .#.v.X....8D$...
-00000dc0: fd99 e1df 0d19 a16f 68d2 0405 1d40 e061  .......oh....@.a
-00000dd0: e037 5183 bb51 6364 ad6a 8086 9d40 6055  .7Q..Qcd.j...@`U
-00000de0: 8334 ea46 bae2 dcb8 1b29 6892 9eba 9106  .4.F.....)h.....
-00000df0: 4dd2 a41b a991 4eac 99e0 4252 0e8b 8950  M.....N...BR...P
-00000e00: 0c1b 18aa 0d62 587d 6e65 0fc0 129b 6c9d  .....bX}ne....l.
-00000e10: e599 3900 d31b d718 9cf1 cf0e 1681 ea44  ..9............D
-00000e20: 6083 f86e c213 6222 a6f9 20ae 2922 72b7  `..n..b".. .)"r.
-00000e30: 8a87 477d efa4 b7a6 8795 fe78 ab15 aa8d  ..G}.......x....
-00000e40: ff95 6421 c896 516e 4acf 91a2 39c4 4270  ..d!..QnJ...9.Bp
-00000e50: 9d66 f254 e1ac 2b0d 16d3 1ab2 bbe5 c48e  .f.T..+.........
-00000e60: e5f5 be42 fa2d cbe5 5fed 6951 85f2 0c6c  ...B.-.._.iQ...l
-00000e70: 63fe 31fe 2caf 2cbf 4df4 bd16 2762 1127  c.1.,.,.M...'b.'
-00000e80: 451b 13fe 7c66 6d09 832c 3c3f b853 682e  E...|fm..,<?.Sh.
-00000e90: 82eb b76c 2035 2068 00c6 246b 99d2 35a3  ...l 5 h..$k..5.
-00000ea0: 8a26 f803 ca0b 8ea6 f761 4635 461f d8b9  .&.......aF5F...
-00000eb0: d40b b979 2c5b 7e28 b195 675a f618 6d75  ...y,[~(..gZ..mu
-00000ec0: aefd c2be 86ef 601d b3ee b212 f463 c67c  ......`......c.|
-00000ed0: a458 424b 6024 5c6d b850 789d 8345 9043  .XBK`$\m.Px..E.C
-00000ee0: 0ea4 8153 9e80 bdc2 a938 b6e8 dcd9 c5b7  ...S.....8......
-00000ef0: 8253 84e6 2061 bba6 122b 6c84 7261 ca9e  .S.. a...+l.ra..
-00000f00: 7ccf 2f37 4a90 0e43 bbb6 82c9 81e7 0d83  |./7J..C........
-00000f10: d700 3aa7 9d85 4e6c ecec d3f1 67a5 f0e1  ..:...Nl....g...
-00000f20: 12bf 47ae e7bd 2c3c ffd5 3b4d 2d68 82b7  ..G...,<..;M-h..
-00000f30: b969 aebc d9a9 c5d2 9f8f 2acb e49b b237  .i........*....7
-00000f40: 2d31 01d7 60d3 9a42 f180 857e 506a 7062  -1..`..B...~Pjpb
-00000f50: a8aa 4668 3645 2741 a5aa bda8 9654 b5a1  ..Fh6E'A.....T..
-00000f60: bcd6 1e5f f59e 086e 32be 2d5b e2c7 df91  ..._...n2.-[....
-00000f70: f0ae 0462 381f 2d96 2fc1 fc7f 0dc4 5587  ...b8.-./.....U.
-00000f80: 6e05 e562 a067 bf01 0000 ffff 0300 504b  n..b.g........PK
-00000f90: 0304 1400 0600 0800 0000 2100 3a68 3c1d  ..........!.:h<.
-00000fa0: 7c02 0000 800a 0000 1100 0000 776f 7264  |...........word
-00000fb0: 2f65 6e64 6e6f 7465 732e 786d 6ccc 96db  /endnotes.xml...
-00000fc0: 72da 3010 86ef 3bd3 77f0 e81e 6441 38c4  r.0...;.w...dA8.
-00000fd0: 13c8 a4a1 7472 9749 da07 10b2 004f acc3  ....tr.I.....O..
-00000fe0: 4802 c3db 77e5 03a6 3565 8c73 532e 7c58  H...w...5e.sS.|X
-00000ff0: e9ff b4bb da15 7e78 3c88 34d8 7363 1325  ......~x<.4.sc.%
-00001000: 6788 f443 1470 c954 9cc8 cd0c fdfa b9ec  g..C.p.T........
-00001010: 4d51 601d 9531 4d95 e433 74e4 163d cebf  MQ`..1M..3t..=..
-00001020: 7e79 c822 2e63 a91c b701 20a4 8d32 cd66  ~y.".c.... ..2.f
-00001030: 68eb 9c8e 30b6 6ccb 05b5 7d91 30a3 ac5a  h...0.l...}.0..Z
-00001040: bb3e 5302 abf5 3a61 1c67 cac4 7810 9230  .>S...:a.g..x..0
-00001050: 7fd2 4631 6e2d acf7 4ce5 9e5a 54e2 d8a1  ..F1n-..L..ZT...
-00001060: 1d2d 3634 03b1 07de 61b6 a5c6 f143 cd20  .-64....a....C. 
-00001070: 3743 46f8 1e4f 9ba0 4107 1044 3820 4dd4  7CF..O..A..D8 M.
-00001080: f066 d418 7baf 1aa0 bb4e 20f0 aa41 1a75  .f..{....N ..A.u
-00001090: 235d 086e dc8d 3468 9226 dd48 c326 69da  #].n..4h.&.H.&i.
-000010a0: 8dd4 2827 d12c 70a5 b984 c1b5 3282 3a78  ..('.,p.....2.:x
-000010b0: 351b 2ca8 f9d8 e91e 8035 75c9 2a49 1377  5.,......5u.*I.w
-000010c0: 0466 38ae 3034 911f 1d3c 02d5 8920 86f1  .f8.04...<... ..
-000010d0: cd84 0916 2ae6 e930 ae28 6a86 7646 46a5  ....*..0.(j.vFF.
-000010e0: be77 d27b d7a3 425f de2a 8569 137f 2159  .w.{..B_.*.i..!Y
-000010f0: 28b6 135c ba3c 726c 780a b950 d26e 137d  (..\.<rlx..P.n.}
-00001100: ea70 d195 0683 db0a b2bf 16c4 5ea4 d5bc  .p..........^...
-00001110: 4c93 96ed f2af e369 51a4 b206 b671 bfcc  L......iQ....q..
-00001120: bf48 0bcf af13 49d8 6247 3ce2 a468 e3c2  .H....I.bG<..h..
-00001130: 9f6b 569e 08a8 c27a e14e a939 4b2e 6979  .kV....z.N.9K.iy
-00001140: 8054 8041 0330 6649 cb92 ae18 4536 211e  .T.A.0fI....E6!.
-00001150: 509e 712c bf0d 33aa 30f6 28ea 56cf f4e6  P.q,..3.0.(.V...
-00001160: 73d5 f2c3 a89d ae69 c9e7 682f 75ef 67fe  s......i..h/u.g.
-00001170: 5ff8 0656 5975 e79d 603f e7cc fb96 6a38  _..VYu..`?....j8
-00001180: 1204 8b5e 3652 19ba 4ac1 23a8 a100 ca20  ...^6R..J.#.... 
-00001190: c877 c05f 6157 02df 7468 5e7f 2a04 59e4  .w._aW..th^.*.Y.
-000011a0: 8e1a 665b aea9 a14e 1904 26bf f13d 92cf  ..f[...N..&..=..
-000011b0: d3a0 bc8b fcd8 0b18 4764 b27c 5a10 8272  ........Gd.|Z..r
-000011c0: 2b1c c4ce 5b27 e5cf 4be1 b325 7e9b a130  +...['..K..%~..0
-000011d0: fcb6 08c9 f7f0 645a f035 dda5 ae39 f2ea  ......dZ.5...9..
-000011e0: 4d8b 2579 1a15 8ee9 57e3 6f56 5306 91c1  M.%y....W.oVS...
-000011f0: a415 87de 010f c920 d7d0 b5e3 a678 c3f3  ....... .....x..
-00001200: 077c 1214 aa2a 8a62 c814 13f2 6b19 f0a5  .|...*.b....k...
-00001210: d899 922e 91bb fc3c 7cff 3b0f e185 3484  .......<|.;...4.
-00001220: cfcf cb29 59de ffaf 69b8 18d0 9594 d4cf  ...)Y...i.......
-00001230: 76fe 1b00 00ff ff03 0050 4b03 0414 0006  v........PK.....
-00001240: 0008 0000 0021 00c3 4d3e fa43 0200 0019  .....!..M>.C....
-00001250: 0900 0010 0000 0077 6f72 642f 6865 6164  .......word/head
-00001260: 6572 312e 786d 6ca4 96db 8e9b 3010 86ef  er1.xml.....0...
-00001270: 2bf5 1d90 ef13 0339 90a2 25ab b651 aadc  +......9..%..Q..
-00001280: 55dd ed03 38c6 04b4 f820 db09 c9db 7738  U...8.... ....w8
-00001290: 8554 ecae 08c9 0584 31f3 f99f f18c f1d3  .T......1.......
-000012a0: f399 e7ce 8969 9349 1121 6fea 2287 092a  .....i.I.!o."..*
-000012b0: e34c 1c22 f4f7 753b 5921 c758 2262 924b  .L."..u;Y!.X"b.K
-000012c0: c122 7461 063d afbf 7e79 2ac2 34d6 0e78  ."ta.=..~y*.4..x
-000012d0: 0b13 168a 4628 b556 8518 1b9a 324e cc94  ....F(.V....2N..
-000012e0: 6754 4b23 133b a592 6399 2419 65b8 903a  gTK#.;..c.$.e..:
-000012f0: c6be ebb9 d53f a525 65c6 c054 3f89 3811  .....?.%e..T?.8.
-00001300: 831a 1c3d 0fa3 c59a 14e0 5c02 e798 a644  ...=......\....D
-00001310: 5b76 ee18 dedd 9005 fe86 577d 903f 0204  [v........W}.?..
-00001320: 11fa 5e1f 35bb 1bb5 c4a5 aa1e 683e 0a04  ..^.5.......h>..
-00001330: aa7a a4c5 38d2 3bc1 2dc7 91fc 3e29 1847  .z..8.;.-...>).G
-00001340: 9af5 49ab 71a4 5e39 f17e 814b c504 0c26  ..I.q.^9.~.K...&
-00001350: 5273 62e1 511f 3027 faed a826 0056 c466  Rsb.Q.0'...&.V.f
-00001360: fb2c cfec 0598 eeb2 c590 4cbc 8d50 045e  .,........L..P.^
-00001370: 5702 9fc5 7713 02cc 65cc f259 dc52 6484  W...w...e..Y.Rd.
-00001380: 8e5a 848d ffe4 ea5f 4a0f 6bff e6d6 7ae8  .Z....._J.k...z.
-00001390: 21f1 d72e 1b49 8f9c 095b 458e 35cb 2117  !....I...[E.5.!.
-000013a0: 5298 3453 d70e e763 6930 98b6 90d3 6741  R.4S...ci0....gA
-000013b0: 9c78 debe 5728 6f60 bb7c b43d 6dea 5476  .x..W(o`.|.=m.Tv
-000013c0: c021 f29b fcf3 bc56 fe39 d173 07ac 4889  .!.....V.9.s..H.
-000013d0: b87a 0c91 f0ff 9cad 120e 55d8 4d3c 2a35  .z........U.M<*5
-000013e0: 37c9 f506 6e20 2dc0 ef01 9634 1b58 d22d  7...n -....4.X.-
-000013f0: a3ce 26c4 039e 371c c3ee c32c 5a8c b9f0  ..&...7....,Z...
-00001400: aed5 0b75 78ac 5a7e 6979 541d 2d7b 8cb6  ...ux.Z~iyT.-{..
-00001410: eb7a bf28 3fc0 77b0 9aaa bbed 04f3 9898  .z.(?.w.........
-00001420: 9794 28d8 1238 0d77 0721 35d9 e7a0 086a  ..(..8.w.!5....j
-00001430: c881 3270 aa15 28af b02a 4ed9 7468 0da7  ..2p..(..*N.th..
-00001440: 0405 9679 a888 263b 58e5 9917 04db 45f0  ...y..&;X.....E.
-00001450: 0355 56d8 606d 690d 9a1f 5843 3889 c47f  .UV.`mi...XC8...
-00001460: 22e4 ba9b adf7 7d31 bf9a 362c 21c7 dcde  ".....}1..6,!...
-00001470: 8c54 f4df baba bdd8 4b0e 7387 2792 4788  .T......K.s.'.G.
-00001480: cc11 2ead 4611 0aa2 c1bc 67d0 1620 d5f3  ....F.....g.. ..
-00001490: dd12 4812 cb74 fd04 2fe2 0653 deab 2b1c  ..H..t../..S..+.
-000014a0: 6cd6 ff00 0000 ffff 0300 504b 0304 1400  l.........PK....
-000014b0: 0600 0800 0000 2100 1107 81df 4302 0000  ......!.....C...
-000014c0: 1909 0000 1000 0000 776f 7264 2f68 6561  ........word/hea
-000014d0: 6465 7232 2e78 6d6c a496 db8e 9b30 1086  der2.xml.....0..
-000014e0: ef2b f51d 90ef 1303 2187 a225 abd5 a6a9  .+......!..%....
-000014f0: 7257 75b7 0fe0 1813 d0e2 836c 2724 6fdf  rWu........l'$o.
-00001500: e114 52d1 ae08 c905 8431 f3f9 9ff1 8cf1  ..R......1......
-00001510: d3f3 99e7 ce89 6993 4911 216f ea22 8709  ......i.I.!o."..
-00001520: 2ae3 4c1c 22f4 fb7d 3b59 21c7 5822 6292  *.L."..};Y!.X"b.
-00001530: 4bc1 2274 6106 3daf bf7e 792a c234 d60e  K."ta.=..~y*.4..
-00001540: 780b 1316 8a46 28b5 5685 181b 9a32 4ecc  x....F(.V....2N.
-00001550: 9467 544b 2313 3ba5 9263 9924 1965 b890  .gTK#.;..c.$.e..
-00001560: 3ac6 beeb b9d5 3fa5 2565 c6c0 54af 449c  :.....?.%e..T.D.
-00001570: 8841 0d8e 9e87 d162 4d0a 702e 8101 a629  .A.....bM.p....)
-00001580: d196 9d3b 8677 3764 8ebf e155 1fe4 8f00  ...;.w7d...U....
-00001590: 4184 bed7 47cd ee46 2d70 a9aa 070a 4681  A...G..F-p....F.
-000015a0: 4055 8f34 1f47 fa47 708b 7124 bf4f 5a8e  @U.4.G.Gp.q$.OZ.
-000015b0: 23cd faa4 d538 52af 9c78 bfc0 a562 0206  #....8R..x...b..
-000015c0: 13a9 39b1 f0a8 0f98 13fd 7154 1300 2b62  ..9.......qT..+b
-000015d0: b37d 9667 f602 4c77 d162 4826 3e46 2802  .}.g..Lw.bH&>F(.
-000015e0: af2b 81cf e2bb 094b cc65 ccf2 59dc 5264  .+.....K.e..Y.Rd
-000015f0: 848e 5a84 8dff e4ea 5f4a 0f6b ffe6 d67a  ..Z....._J.k...z
-00001600: e821 f1d7 2e1b 498f 9c09 5b45 8e35 cb21  .!....I...[E.5.!
-00001610: 1752 9834 53d7 0ee7 6369 3098 b690 d367  .R.4S...ci0....g
-00001620: 419c 78de be57 286f 60bb fc6f 7bda d4a9  A.x..W(o`..o{...
-00001630: ec80 43e4 37f9 e779 adfc 73a2 e70e 5891  ..C.7..y..s...X.
-00001640: 1271 f518 22e1 ef39 5b25 1caa b09b 7854  .q.."..9[%....xT
-00001650: 6a6e 92eb 0ddc 405a 80df 032c 6836 b0a4  jn....@Z...,h6..
-00001660: 5b46 9d4d 8807 3c6f 3886 dd87 99b7 1873  [F.M..<o8......s
-00001670: e15d ab17 eaf0 58b5 fcd0 f2a8 3a5a f618  .]....X.....:Z..
-00001680: 6dd7 f57e 517e 80ef 6035 5577 db09 e631  m..~Q~..`5Uw...1
-00001690: 316f 2951 b025 701a ee0e 426a b2cf 4111  1o)Q.%p...Bj..A.
-000016a0: d490 0365 e054 2b50 5e61 559c b2e9 d01a  ...e.T+P^aU.....
-000016b0: 4e09 0a2c 41a8 8826 3b58 e5e0 f5e5 fb6a  N..,A..&;X.....j
-000016c0: 116c 5165 850d d696 d665 f303 6b08 2791  .lQe.....e..k.'.
-000016d0: f857 845c 77b3 f55e e6c1 d5b4 6109 39e6  .W.\w..^....a.9.
-000016e0: f666 a4a2 ffd4 d5ed cd5e 7298 3b3c 913c  .f.......^r.;<.<
-000016f0: 4224 40b8 b41a 4528 8806 f39e 415b 8054  B$@...E(....A[.T
-00001700: cf77 4b20 492c d3f5 13bc 881b 4c79 afae  .wK I,......Ly..
-00001710: 70b0 59ff 0100 00ff ff03 0050 4b03 0414  p.Y........PK...
-00001720: 0006 0008 0000 0021 00ce 9637 6d42 0200  .......!...7mB..
-00001730: 0019 0900 0010 0000 0077 6f72 642f 666f  .........word/fo
-00001740: 6f74 6572 312e 786d 6ca4 96db 8e9b 3010  oter1.xml.....0.
-00001750: 86ef 2bf5 1d90 ef13 0349 4816 2d59 558d  ..+......IH.-YU.
-00001760: b6ca 5dd5 dd3e 8063 4c40 8b0f b29d 90bc  ..]..>.cL@......
-00001770: 7d87 732a da15 21b9 8030 663e ff33 9e31  }.s*..!..0f>.3.1
-00001780: 7e7e b9f0 dc39 336d 3229 22e4 cd5d e430  ~~...93m2)"..].0
-00001790: 4165 9c89 6384 7ebf bfce 36c8 3196 8898  Ae..c.~...6.1...
-000017a0: e452 b008 5d99 412f dbaf 5f9e 8b30 b1da  .R..].A/.._..0..
-000017b0: 016f 61c2 42d1 08a5 d6aa 1063 4353 c689  .oa.B......cCS..
-000017c0: 99f3 8c6a 6964 62e7 5472 2c93 24a3 0c17  ...jidb.Tr,.$...
-000017d0: 52c7 d877 3db7 faa7 b4a4 cc18 98ea 3b11  R..w=.........;.
-000017e0: 6762 5083 a397 71b4 5893 029c 4be0 12d3  gbP...q.X...K...
-000017f0: 9468 cb2e 3dc3 bb1b b2c2 4f78 3304 f913  .h..=.....Ox3...
-00001800: 4010 a1ef 0d51 8bbb 5101 2e55 0d40 cb49  @....Q..Q..U.@.I
-00001810: 2050 3520 ada6 91fe 115c 308d e40f 49eb   P5 .....\0...I.
-00001820: 69a4 c590 b499 461a 9413 1f16 b854 4cc0  i.....F......TL.
-00001830: 6022 3527 161e f511 73a2 3f4e 6a06 6045  `"5'....s.?Nj.`E
-00001840: 6c76 c8f2 cc5e 81e9 062d 8664 e263 8222  lv...^...-.d.c."
-00001850: f0ea 087c 11df 4d58 632e 6396 2fe2 9622  ...|..MXc.c./.."
-00001860: 2374 d222 6cfc 679d 7f29 3dac fd9b 5beb  #t."l.g..)=...[.
-00001870: a1c7 c45f bbec 243d 7126 6c15 39d6 2c87  ..._..$=q&l.9.,.
-00001880: 5c48 61d2 4c75 1dce a7d2 6030 6d21 e7cf  \Ha.Lu....`0m!..
-00001890: 8238 f3bc 7daf 50de c876 f9df f6b4 ab53  .8..}.P..v.....S
-000018a0: d903 c7c8 6ff2 cff3 5af9 e744 cf1d b122  ....o...Z..D..."
-000018b0: 25a2 f318 23e1 ef39 5b25 1caa b09f 7852  %...#..9[%....xR
-000018c0: 6a6e 92eb 8ddc 405a 803f 0004 341b 59d2  jn....@Z.?..4.Y.
-000018d0: 2da3 ce26 c403 9e37 1cc3 eec3 ac5a 8cb9  -..&...7.....Z..
-000018e0: f2be d50b 757c ac5a 7e68 7952 3d2d 7b8c  ....u|.Z~hyR=-{.
-000018f0: b6ef 7bbf 283f c077 b09a aabb ed04 f398  ..{.(?.w........
-00001900: 98b7 9428 d812 380d f747 2135 39e4 a008  ...(..8..G!59...
-00001910: 6ac8 8132 70aa 1528 afb0 2a4e d974 680b  j..2p..(..*N.th.
-00001920: a704 0596 65a8 8826 7b58 657f e906 4f0b  ....e..&{Xe...O.
-00001930: df43 9515 3658 5b5a d7cd 0fac 219c 44e2  .C..6X[Z....!.D.
-00001940: 5f11 72dd ddab f76d b5ec 4c3b 9690 536e  _.r....m..L;..Sn
-00001950: 6f46 2afa 4f5d ddde ec35 87b9 c333 c923  oF*.O]...5...3.#
-00001960: 4402 844b ab51 8482 6830 1f18 b405 48f5  D..K.Q..h0....H.
-00001970: 7cb7 0492 c432 5d3f c18b b8c1 94f7 ea0a  |....2]?........
-00001980: 079b ed1f 0000 00ff ff03 0050 4b03 0414  ...........PK...
-00001990: 0006 0008 0000 0021 0051 e447 db42 0200  .......!.Q.G.B..
-000019a0: 0019 0900 0010 0000 0077 6f72 642f 666f  .........word/fo
-000019b0: 6f74 6572 322e 786d 6ca4 96dd aea2 3010  oter2.xml.....0.
-000019c0: c7ef 37d9 7720 bdd7 022a 2a39 78b2 59e3  ..7.w ...**9x.Y.
-000019d0: c6bb cd9e b30f 504b 1172 e847 da2a faf6  ......PK.r.G.*..
-000019e0: 3b7c 891b 764f 10bd 0099 32bf fe67 3a53  ;|..vO....2..g:S
-000019f0: faf2 7ae1 b973 66da 6452 44c8 9bba c861  ..z..sf.dRD....a
-00001a00: 82ca 3813 c708 fd7e df4d 56c8 3196 8898  ..8....~.MV.1...
-00001a10: e452 b008 5d99 41af 9baf 5f5e 8a30 b1da  .R..].A..._^.0..
-00001a20: 016f 61c2 42d1 08a5 d6aa 1063 4353 c689  .oa.B......cCS..
-00001a30: 99f2 8c6a 6964 62a7 5472 2c93 24a3 0c17  ...jidb.Tr,.$...
-00001a40: 52c7 d877 3db7 faa7 b4a4 cc18 98ea 3b11  R..w=.........;.
-00001a50: 6762 5083 a397 61b4 5893 029c 4be0 1cd3  gbP...a.X...K...
-00001a60: 9468 cb2e 1dc3 7b18 b2c0 6bbc ea83 fc11  .h....{...k.....
-00001a70: 2088 d0f7 faa8 d9c3 a800 97aa 7aa0 f928   ...........z..(
-00001a80: 10a8 ea91 16e3 48ff 082e 1847 f2fb a4e5  ......H....G....
-00001a90: 38d2 ac4f 5a8d 23f5 ca89 f70b 5c2a 2660  8..OZ.#.....\*&`
-00001aa0: 3091 9a13 0b8f fa88 39d1 1f27 3501 b022  0.......9..'5.."
-00001ab0: 363b 6479 66af c074 8316 4332 f131 4211  6;dyf..t..C2.1B.
-00001ac0: 78dd 087c 163f 4c58 622e 6396 cfe2 9622  x..|.?LXb.c...."
-00001ad0: 2374 d222 6cfc 2737 ff52 7a58 fb37 b7d6  #t."l.'7.RzX.7..
-00001ae0: 430f 89bf 76d9 4a7a e24c d82a 72ac 590e  C...v.Jz.L.*r.Y.
-00001af0: b990 c2a4 99ba 7538 1f4b 83c1 b485 9c3f  ......u8.K.....?
-00001b00: 0be2 ccf3 f6bd 4279 03db e57f dbd3 b64e  ......By.......N
-00001b10: 6507 1c22 bfc9 3fcf 6be5 9f13 3d77 c08a  e.."..?.k...=w..
-00001b20: 9488 9bc7 1009 7fcf d92a e150 85dd c4a3  .........*.P....
-00001b30: 5273 975c 6fe0 06d2 02fc 1e20 a0d9 c092  Rs.\o...... ....
-00001b40: 6e19 7536 211e f0bc e318 f618 66d1 62cc  n.u6!.......f.b.
-00001b50: 9577 ad5e a8e3 73d5 f243 cb93 ea68 d973  .w.^..s..C...h.s
-00001b60: b47d d7fb 45f9 017e 80d5 54dd 7d27 98e7  .}..E..~..T.}'..
-00001b70: c4bc a544 c196 c069 b83f 0aa9 c921 0745  ...D...i.?...!.E
-00001b80: 5043 0e94 8153 ad40 7985 5571 caa6 431b  PC...S.@y.Uq..C.
-00001b90: 3825 28b0 cc43 4534 d9c3 2a07 ae3b 5bef  8%(..CE4..*..;[.
-00001ba0: 8235 aaac b0c1 dad2 ba6c 7e60 0de1 2412  .5.......l~`..$.
-00001bb0: ff8a 90eb 6e77 deb7 c5fc 66da b284 9c72  ....nw....f....r
-00001bc0: 7b37 52d1 7fea eaf6 66af 39cc 1d9e 491e  {7R.....f.9...I.
-00001bd0: 2112 205c 5a8d 2214 4483 f9c0 a02d 40aa  !. \Z.".D....-@.
-00001be0: e7bb 2590 2496 e9fa 095e c40d a6bc 5757  ..%.$....^....WW
-00001bf0: 38d8 6cfe 0000 00ff ff03 0050 4b03 0414  8.l........PK...
-00001c00: 0006 0008 0000 0021 0024 5682 a244 0200  .......!.$V..D..
-00001c10: 0019 0900 0010 0000 0077 6f72 642f 6865  .........word/he
-00001c20: 6164 6572 332e 786d 6ca4 96df 939a 3010  ader3.xml.....0.
-00001c30: c7df 3bd3 ff81 c9bb 0650 d132 8737 9d7a  ..;......P.2.7.z
-00001c40: d7f1 add3 6bff 8018 8230 477e 4c12 45ff  ....k....0G~L.E.
-00001c50: fb6e 10c4 0eed 0da2 0f20 1bf6 93ef 6e76  .n....... ....nv
-00001c60: 439e 9e4f bcf4 8e4c 9b42 8a04 0553 1f79  C..O...L.B...S.y
-00001c70: 4c50 9916 629f a0df bf5e 272b e419 4b44  LP..b....^'+..KD
-00001c80: 4a4a 2958 82ce cca0 e7f5 e74f 4f55 9ca7  JJ)X.......OOU..
-00001c90: da03 6f61 e24a d104 e5d6 aa18 6343 73c6  ..oa.J......cCs.
-00001ca0: 8999 f282 6a69 6466 a754 722c b3ac a00c  ....jidf.Tr,....
-00001cb0: 5752 a738 f403 bffe a7b4 a4cc 1898 ea1b  WR.8............
-00001cc0: 1147 6250 83a3 a761 b454 930a 9c1d 708e  .GbP...a.T....p.
-00001cd0: 694e b465 a78e 11dc 0d59 e02f 78d5 0785  iN.e.....Y./x...
-00001ce0: 2340 1061 18f4 51b3 bb51 1176 aa7a a0f9  #@.a..Q..Q.v.z..
-00001cf0: 2810 a8ea 9116 e348 ff08 2e1a 470a fba4  (......H....G...
-00001d00: e538 d2ac 4f5a 8d23 f5ca 89f7 0b5c 2a26  .8..OZ.#.....\*&
-00001d10: 6030 939a 130b 8f7a 8f39 d1ef 0735 01b0  `0.....z.9...5..
-00001d20: 22b6 d815 6561 cfc0 f4a3 1643 0af1 3e42  "...ea.....C..>B
-00001d30: 1178 5d09 7c96 de4d 5862 2e53 56ce d296  .x].|..MXb.SV...
-00001d40: 2213 74d0 226e fc27 577f 273d bef8 37b7  ".t."n.'W.'=..7.
-00001d50: d643 0f89 ffe2 b291 f4c0 99b0 75e4 58b3  .C..........u.X.
-00001d60: 1272 2185 c90b 75ed 703e 9606 8379 0b39  .r!...u.p>...y.9
-00001d70: 7e14 c491 97ed 7b95 0a06 b6cb ffb6 a7cd  ~.....{.........
-00001d80: 2595 1d70 88fc 26ff bcbc 28ff 9818 f803  %..p..&...(.....
-00001d90: 56c4 21ae 1e43 24fc 3d67 ab84 4315 7613  V.!..C$.=g..C.v.
-00001da0: 8f4a cd4d 7283 811b 480b 087b 8088 1603  .J.Mr...H..{....
-00001db0: 4bba 655c b209 f180 e70d c7b0 fb30 8b16  K.e\.........0..
-00001dc0: 63ce bc6b f54a ed1f ab96 ef5a 1e54 472b  c..k.J.....Z.TG+
-00001dd0: 1ea3 6dbb deaf dc07 f80e 5653 75b7 9d60  ..m.......VSu..`
-00001de0: 1e13 f396 1305 5b02 a7f1 762f a426 bb12  ......[...v/.&..
-00001df0: 1441 0d79 5006 5ebd 02ee 0aab e2b9 a643  .A.yP.^........C
-00001e00: 6b38 2528 b0cc 6345 34d9 c22a 47b3 e8e5  k8%(..cE4..*G...
-00001e10: 6519 c186 e8ac b0c1 5a67 5d36 3fb0 c670  e.......Zg]6?..p
-00001e20: 1249 7f26 c8f7 37af c1d7 c5fc 6ada b08c  .I.&..7.....j...
-00001e30: 1c4a 7b33 52d3 7fe8 faf6 66cf 25cc 1d1f  .J{3R.....f.%...
-00001e40: 4999 2032 47d8 598d 2214 4483 79c7 a02d  I. 2G.Y.".D.y..-
-00001e50: 406a 10fa 0e48 32cb f4e5 095e c40d c6dd  @j...H2....^....
-00001e60: eb2b 1c6c d67f 0000 00ff ff03 0050 4b03  .+.l.........PK.
-00001e70: 0414 0006 0008 0000 0021 000b f966 2241  .........!...f"A
-00001e80: 0200 0019 0900 0010 0000 0077 6f72 642f  ...........word/
-00001e90: 666f 6f74 6572 332e 786d 6ca4 96df af9a  footer3.xml.....
-00001ea0: 3014 c7df 97ec 7f20 7dd7 022a 3a72 f166  0...... }..*:r.f
-00001eb0: 9971 f16d d9dd fe80 5a8a 904b 7fa4 ada2  .q.m....Z..K....
-00001ec0: fffd 4e11 c485 ed06 d107 2aa7 3d9f 7e4f  ..N.......*.=.~O
-00001ed0: 7b4e e9cb eb99 97de 8969 5348 91a0 60ea  {N.......iSH..`.
-00001ee0: 238f 092a d342 1c12 f4fb d776 b242 9eb1  #..*.B.....v.B..
-00001ef0: 44a4 a494 8225 e8c2 0c7a 5d7f fef4 52c5  D....%...z]...R.
-00001f00: 99d5 1e78 0b13 578a 2628 b756 c518 1b9a  ...x..W.&(.V....
-00001f10: 334e cc94 1754 4b23 333b a592 6399 6505  3N...TK#3;..c.e.
-00001f20: 65b8 923a c5a1 1ff8 f53f a525 65c6 c054  e..:.....?.%e..T
-00001f30: df88 3811 831a 1c3d 0fa3 a59a 54e0 ec80  ..8....=....T...
-00001f40: 734c 73a2 2d3b 778c e061 c802 7fc1 ab3e  sLs.-;w..a.....>
-00001f50: 281c 0182 08c3 a08f 9a3d 8c8a b053 d503  (........=...S..
-00001f60: cd47 8140 558f b418 47fa 4770 d138 52d8  .G.@U...G.Gp.8R.
-00001f70: 272d c791 667d d26a 1ca9 974e bc9f e052  '-..f}.j...N...R
-00001f80: 3101 9d99 d49c 5878 d507 cc89 7e3f aa09  1.....Xx....~?..
-00001f90: 8015 b1c5 be28 0b7b 01a6 1fb5 1852 88f7  .....(.{.....R..
-00001fa0: 118a c0eb 46e0 b3f4 61c2 1273 99b2 7296  ....F...a..s..r.
-00001fb0: b614 99a0 a316 71e3 3fb9 f93b e9f1 d5bf  ......q.?..;....
-00001fc0: 695a 0f3d 24fe abcb 46d2 2367 c2d6 9163  iZ.=$...F.#g...c
-00001fd0: cd4a 580b 294c 5ea8 5b85 f3b1 34e8 cc5b  .JX.)L^.[...4..[
-00001fe0: c8e9 a320 4ebc 6cc7 552a 1858 2eff 3b9e  ... N.l.U*.X..;.
-00001ff0: 36d7 a5ec 8043 e437 ebcf cbab f28f 8981  6....C.7........
-00002000: 3f60 471c e2e6 3144 c2df 73b6 4a38 6461  ?`G...1D..s.J8da
-00002010: 37f1 a8a5 b95b dc60 e001 d202 c21e 20a2  7....[.`...... .
-00002020: c5c0 946e 19d7 d584 78c0 f38e 63d8 6398  ...n....x...c.c.
-00002030: 458b 3117 de95 7aa5 0ecf 65cb 772d 8faa  E.1...z...e.w-..
-00002040: a315 cfd1 765d ed57 ee03 fc00 abc9 bafb  ....v].W........
-00002050: 4a30 cf89 79cb 8982 2381 d378 7710 5293  J0..y...#..xw.R.
-00002060: 7d09 8a20 873c 4803 afde 01f7 845d f15c  }.. .<H......].\
-00002070: d1a1 35dc 1214 58e6 b122 9aec 6097 a3cd  ..5...X.."..`...
-00002080: 76be 0dbe 2e50 6d85 03d6 3aeb b2f9 8135  v....Pm...:....5
-00002090: 869b 48fa 3341 bebf 71e3 e637 d386 65e4  ..H.3A..q..7..e.
-000020a0: 58da bb9e 9afe 43d7 cd9b bd94 3077 7c22  X.....C.....0w|"
-000020b0: 6582 4884 b0b3 1a45 2888 06f3 9e41 5980  e.H....E(....AY.
-000020c0: d420 f41d 9064 96e9 eb1b 0cc4 0dc6 b5f5  . ...d..........
-000020d0: 132e 36eb 3f00 0000 ffff 0300 504b 0304  ..6.?.......PK..
-000020e0: 1400 0600 0800 0000 2100 3a05 cc19 e106  ........!.:.....
-000020f0: 0000 ce20 0000 1500 0000 776f 7264 2f74  ... ......word/t
-00002100: 6865 6d65 2f74 6865 6d65 312e 786d 6cec  heme/theme1.xml.
-00002110: 595b 6b1b 4714 7e2f f43f 2cfb aee8 b6ab  Y[k.G.~/.?,.....
-00002120: 8b89 1ca4 9514 37b1 1313 2b29 791c af46  ......7...+)y..F
-00002130: bb63 cdee 8899 911d 1102 2179 2a85 4221  .c........!y*.B!
-00002140: 2d79 68a0 f4a5 0fa5 34d0 4043 fbd0 ff52  -yh.....4.@C...R
-00002150: 9784 34fd 119d 9995 b43b d22c 4e62 1b42  ..4......;.,Nb.B
-00002160: b16d acb9 7ce7 cc37 e79c 3973 b47b f9ca  .m..|..7..9s.{..
-00002170: bd08 5b87 9032 44e2 965d be54 b22d 18fb  ..[..2D..].T.-..
-00002180: 6488 e2a0 65df 1ef4 0b0d db62 1cc4 4380  d...e......b..C.
-00002190: 490c 5bf6 0c32 fbca e6a7 9f5c 061b 3c84  I.[..2.....\..<.
-000021a0: 11b4 847c cc36 40cb 0e39 9f6c 148b cc17  ...|.6@..9.l....
-000021b0: c380 5d22 1318 8bb9 11a1 11e0 a24b 83e2  ..]".........K..
-000021c0: 9082 23a1 37c2 c54a a954 2b46 00c5 b615  ..#.7..J.T+F....
-000021d0: 8348 a8bd 391a 211f 5a7f bffc e3cd 0f4f  .H..9.!.Z......O
-000021e0: ff7a f8a5 f8b3 3717 6bf4 b0f8 1773 2607  .z....7.k....s&.
-000021f0: 7c4c f7e4 0a50 1354 d8e1 b82c 3fd8 8c79  |L...P.T...,?..y
-00002200: 985a 8700 b76c b1dc 901c 0de0 3d6e 5b18  .Z...l......=n[.
-00002210: 302e 265a 7649 fdd8 c5cd cbc5 a510 e639  0.&ZvI.........9
-00002220: b219 b9be fa99 cbcd 0586 e38a 92a3 c1fe  ................
-00002230: 52d0 715c a7d6 5eea 5700 ccd7 71bd 7aaf  R.q\..^.W...q.z.
-00002240: d6ab 2df5 2900 f07d b1d3 848b aeb3 5ef1  ..-.)..}......^.
-00002250: 9c39 3603 4a9a 06dd dd7a b75a d6f0 19fd  .96.J....z.Z....
-00002260: d535 7cdb 95bf 1a5e 8192 a6b3 86ef f7bd  .5|....^........
-00002270: d486 1950 d274 d7f0 6ea7 d9e9 eafa 1528  ...P.t..n......(
-00002280: 69d6 d6f0 f552 bbeb d435 bc02 8518 c5e3  i....R...5......
-00002290: 3574 c9ad 55bd c56e 9790 11c1 5b46 78d3  5t..U..n....[Fx.
-000022a0: 75fa f5ca 1c9e a28a 99e8 4ae4 639e 176b  u.........J.c..k
-000022b0: 1138 20b4 2f00 cab9 80a3 d8e2 b309 1c01  .8 ./...........
-000022c0: 5fe0 5eff fcc5 ebdf ffb4 b651 108a b89b  _.^........Q....
-000022d0: 8098 3031 5aaa 94fa a5aa f82f 7f1d d552  ..01Z....../...R
-000022e0: 0e05 1b10 6484 9321 9fad 0d49 3a16 f329  ....d..!...I:..)
-000022f0: 9af0 967d 4d68 b533 9057 2f5f 1e3f 7a71  ...}Mh.3.W/_.?zq
-00002300: fce8 b7e3 c78f 8f1f fd32 5f7b 5d6e 0bc4  .........2_{]n..
-00002310: 4156 eeed 8f5f fffb eca1 f5cf afdf bf7d  AV..._.........}
-00002320: f28d 19cf b278 6d6b 4638 d768 7dfb fcf5  .....xmkF8.h}...
-00002330: 8be7 af9e 7ef5 e6a7 2706 789b 82fd 2c7c  ....~...'.x...,|
-00002340: 8022 c8ac 1bf0 c8ba 4522 b141 c302 709f  ."......E".A..p.
-00002350: be9f c420 0428 2bd1 8e03 0662 2065 0ce8  ... .(+....b e..
-00002360: 1e0f 35f4 8d19 c0c0 80eb 40dd 8e77 a8c8  ..5.......@..w..
-00002370: 1626 e0d5 e981 4678 2fa4 538e 0cc0 eb61  .&....Fx/.S....a
-00002380: a401 7708 c11d 428d 7bba 2ed7 ca5a 611a  ..w...B.{....Za.
-00002390: 07e6 c5e9 348b bb05 c0a1 696d 6fc5 cbbd  ....4.....imo...
-000023a0: e944 843d 32a9 f442 a8d1 dcc5 c2e5 2080  .D.=2..B...... .
-000023b0: 31e4 969c 2363 080d 6277 11d2 ecba 837c  1...#c..bw.....|
-000023c0: 4a18 1971 eb2e b23a 0019 4d32 40fb 5a34  J..q...:..M2@.Z4
-000023d0: a542 5b28 127e 9999 080a 7f6b b6d9 b963  .B[(.~.....k...c
-000023e0: 7508 36a9 efc2 431d 29ce 06c0 2695 106b  u.6...C.)...&..k
-000023f0: 66bc 0aa6 1c44 46c6 20c2 59e4 36e0 a189  f....DF. .Y.6...
-00002400: e4de 8cfa 9ac1 1917 9e0e 2026 566f 0819  .......... &Vo..
-00002410: 33c9 dca4 338d ee75 20d2 96d1 ed3b 7816  3...3..u ....;x.
-00002420: e948 cad1 d884 dc06 8464 915d 32f6 4210  .H.......d.]2.B.
-00002430: 4d8c 9c51 1c66 b19f b1b1 0851 60ed 126e  M..Q.f.....Q`..n
-00002440: 2441 f413 22fb c20f 20ce 75f7 1d04 3577  $A.."... .u...5w
-00002450: 9f7c b66f 8b34 640e 1039 33a5 a623 0189  .|.o.4d..93..#..
-00002460: 7e1e 6778 04a0 4979 9b46 5a8a 6d53 648c  ~.gx..Iy.FZ.mSd.
-00002470: 8ece 34d0 427b 1b42 0c8e c010 42eb f667  ..4.B{.B....B..g
-00002480: 263c 9968 364f 495f 0b45 56d9 8226 db5c  &<.h6OI_.EV..&.\
-00002490: 037a acca 7e0c 19b4 546d 6370 2c62 5ac8  .z..~...Tmcp,bZ.
-000024a0: eec1 80e4 f0d9 99ad 249e 1988 2340 f334  ........$...#@.4
-000024b0: df18 eb21 d3db a7e2 309a e215 fb63 2d95  ...!....0....c-.
-000024c0: 222a 0fad 99c4 4d16 69fb cbd5 ba1b 022d  "*....M.i......-
-000024d0: ac64 9f99 e375 4635 ffbd cb19 1332 071f  .d...uF5.....2..
-000024e0: 2003 df5b 4624 f677 b6cd 0060 6d81 3460   ..[F$.w...`m.4`
-000024f0: 0600 59db a674 2b44 34f7 a722 f238 29b1  ..Y..t+D4..".8).
-00002500: a951 6ea4 1fda d40d c595 9a27 42f1 4905  .Qn........'B.I.
-00002510: d04a e9e3 9e5f e923 0a8c 57df 3d33 60cf  .J..._.#..W.=3`.
-00002520: a6dc 3103 4f53 e8e4 e592 d5f2 260f b75a  ..1.OS......&..Z
-00002530: d478 840e d1c7 5fd3 74c1 34de 85e2 1a31  .x...._.t.4....1
-00002540: 402f 4a9a 8b92 e67f 5fd2 e49d e78b 42e6  @/J....._.....B.
-00002550: a290 b928 64cc 22e7 50c8 a4b5 8b7a 00b4  ...(d.".P....z..
-00002560: 78cc a3b4 44b9 cf7c 4608 e33d 3ec3 709b  x...D..|F..=>.p.
-00002570: a9aa 8789 b33f ec8b 41d5 5142 cb47 4c93  .....?..A.QB.GL.
-00002580: 5034 e7cb 69b8 8002 d5b6 28e1 9f23 1eee  P4..i.....(..#..
-00002590: 8560 2296 29ab 1502 3657 1d30 6b42 9828  .`".)...6W.0kB.(
-000025a0: 9cd4 b051 b79c c0d3 6887 0c93 d172 79f1  ...Q....h....ry.
-000025b0: 5453 0800 9e8e 8bc2 6b31 2eaa 349e 8cd6  TS......k1..4...
-000025c0: eae9 e3bb a57a d50b d463 d605 0129 fb3e  .....z...c...).>
-000025d0: 2432 8be9 24aa 0612 f5c5 e009 24d4 cece  $2..$.......$...
-000025e0: 8445 d3c0 a221 d5e7 b250 1f73 af88 cbc9  .E...!...P.s....
-000025f0: 02f2 b9b8 eb24 8c44 b889 901e 4a3f 25f2  .....$.D....J?%.
-00002600: 0bef 9eb9 a7f3 8ca9 6fbb 62d8 5e53 723d  ........o.b.^Sr=
-00002610: 1b4f 6b24 32e1 a693 c884 6128 2e8f d5e1  .Ok$2.....a(....
-00002620: 33f6 7533 75a9 464f 9a62 9d46 bd71 1ebe  3.u3u.FO.b.F.q..
-00002630: 9649 6425 37e0 58ef 5947 e2cc 555d a1c6  .Id%7.X.YG..U]..
-00002640: 0793 963d 12df 9844 339a 087d 4c66 2a80  ...=...D3..}Lf*.
-00002650: 83b8 65fb 7c6e e80f c92c 13ca 7817 b030  ..e.|n...,..x..0
-00002660: 81a9 a964 ff11 e290 5a18 4522 d6b3 6ec0  ...d....Z.E"..n.
-00002670: 71ca ad5c a9cb 3d7e a4e4 9aa5 8fcf 72ea  q..\..=~......r.
-00002680: 23eb 6438 1a41 9fe7 8ca4 5d31 9728 31ce  #.d8.A....]1.(1.
-00002690: 9e12 2c3b 642a 48ef 85c3 236b 1f4f e92d  ..,;d*H...#k.O.-
-000026a0: 200c e5d6 cbd2 8043 c4f8 d29a 4344 33c1   ......C....CD3.
-000026b0: 9d5a 7125 5dcd 8fa2 f6b6 253d a200 4f42  .Zq%].....%=..OB
-000026c0: 30bf 51b2 c93c 81ab f692 4e66 1f8a e9ea  0.Q..<....Nf....
-000026d0: aef4 fe7c 33fb 8174 d2a9 6fdd 9385 e444  ...|3..t..o....D
-000026e0: 2669 e65c 20f2 d634 e78f f3bb e433 acd2  &i.\ ..4.....3..
-000026f0: bcaf b14a 52f7 6aae 6b2e 725d de2d 71fa  ...JR.j.k.r].-q.
-00002700: 0b21 432d 5d4c a326 191b a8a5 a33a b533  .!C-]L.&.....:.3
-00002710: 2c08 32cb 2d43 33ef 8e38 ebdb 6035 6ae5  ,.2.-C3..8..`5j.
-00002720: 05b1 a82b 556f edb5 36d9 3f10 91df 15d5  ...+Uo..6.?.....
-00002730: ea14 73a6 a88a 6f2d 1478 8b17 9249 2650  ..s...o-.x...I&P
-00002740: a38b ec72 8f5b 538a 5af6 fd92 db76 bc8a  ...r.[S.Z....v..
-00002750: eb15 4a0d b757 70aa 4ea9 d070 dbd5 42db  ..J..Wp.N..p..B.
-00002760: 75ab e59e 5b2e 753b 9507 c228 3c8c ca6e  u...[.u;...(<..n
-00002770: b276 5f7c d9c7 b3f9 cb7b 35be f602 3f5a  .v_|.....{5...?Z
-00002780: 94da 977c 1215 89aa 838b 4a58 bdc0 2f57  ...|......JX../W
-00002790: 4c2f f007 72de b690 b0cc fd5a a5df ac36  L/..r......Z...6
-000027a0: 3bb5 42b3 daee 179c 6ea7 5168 7ab5 4ea1  ;.B.....n.Qhz.N.
-000027b0: 5bf3 eadd 7ed7 731b cdfe 03db 3a54 60a7  [...~.s.....:T`.
-000027c0: 5df5 9c5a af51 a895 3daf e0d4 4a92 7ea3  ]..Z.Q..=...J.~.
-000027d0: 59a8 3b95 4adb a9b7 1b3d a7fd 606e 6bb1  Y.;.J....=..`nk.
-000027e0: f3c5 e7c2 bc8a d7e6 7f00 0000 ffff 0300  ................
-000027f0: 504b 0304 1400 0600 0800 0000 2100 f83f  PK..........!..?
-00002800: 6ea7 8705 0000 dc0f 0000 1100 0000 776f  n.............wo
-00002810: 7264 2f73 6574 7469 6e67 732e 786d 6cb4  rd/settings.xml.
-00002820: 575b 6fdb 3614 7e1f b0ff 60f8 798e 75f7  W[o.6.~...`.y.u.
-00002830: 0575 0adb b296 1449 5b54 e9fa 4c4b 74cc  .u.....I[T..LKt.
-00002840: 8522 0592 b6e3 0cfb ef3b 24c5 284e 9422  .".......;$.(N."
-00002850: edd0 9784 3adf b9f1 f0dc fcee fd7d 457b  ....:........}E{
-00002860: 7b2c 24e1 6cd6 f7cf bc7e 0fb3 8297 84dd  {,$.l....~......
-00002870: cefa 5f6f b2c1 b8df 930a b112 51ce f0ac  .._o........Q...
-00002880: 7fc4 b2ff fefc f7df de1d a612 2b05 6cb2  ............+.l.
-00002890: 072a 989c 56c5 acbf 55aa 9e0e 87b2 d8e2  .*..V...U.......
-000028a0: 0ac9 335e 6306 e086 8b0a 29f8 14b7 c30a  ..3^c.....).....
-000028b0: 89bb 5d3d 2878 5523 45d6 8412 751c 069e  ..]=(xU#E...u...
-000028c0: 97f4 1b35 7cd6 df09 366d 540c 2a52 082e  ...5|...6mT.*R..
-000028d0: f946 6991 29df 6c48 819b 7f4e 42bc c5ae  .Fi.).lH...NB...
-000028e0: 1549 79b1 ab30 53c6 e250 600a 3e70 26b7  .Iy..0S..P`.>p&.
-000028f0: a496 4e5b f5b3 da00 dc3a 25fb ef5d 625f  ..N[.....:%..]b_
-00002900: 51c7 77f0 bd37 5cf7 c045 f928 f116 f7b4  Q.w..7\..E.(....
-00002910: 402d 7881 a584 07aa a873 90b0 d670 f442  @-x......s...p.B
-00002920: d1a3 ed33 b0dd 5cd1 a802 71df 33a7 a79e  ...3..\...q.3...
-00002930: c73f a620 78a1 2029 48f9 633a 9246 c710  .?. x. )H.c:.F..
-00002940: 249f e891 f8c7 d4c4 4e8d 3c56 f8de 2992  $.......N.<V..).
-00002950: f42d a1b5 d015 590b 246c e236 71ad 8ae9  .-....Y.$l.6q...
-00002960: e52d e302 ad29 b803 f1ed 4188 7ac6 3bfd  .-...)....A.z.;.
-00002970: 577b 7c0e 45f3 c079 d53b 4c6b 2c0a c81c  W{|.E..y.;Lk,...
-00002980: a838 cfeb 0f35 b006 97a0 0c53 fe91 ab7c  .8...5.....S...|
-00002990: 2704 dfb1 f202 23a0 bd0a 679c ab06 86d7  '.....#...g.....
-000029a0: e69b 5c21 05c6 a6b2 c694 9a02 2e28 46cc  ..\!.........(F.
-000029b0: ea2f f106 eda8 ba41 eb5c f11a b8f6 082e  ./.....A.\......
-000029c0: 1c05 8df9 16a6 3857 47aa f518 0ec4 103d  ......8WG......=
-000029d0: 4a22 0725 52a8 e115 e800 eaff 14a4 fc0b  J".%R...........
-000029e0: 0b45 0a44 f31a 1540 7242 7e9c 34ac 44d6  .E.D...@rB~.4.D.
-000029f0: 141d 2fb8 200f 9c29 44d3 5676 056d e7e8  ../. ..)D.Vv.m..
-00002a00: 249c 1b96 dfa9 7d8d 3bb0 dcc5 1609 5440  $.....}.;.....T@
-00002a10: 0c1a f34b 3021 3875 5cba c908 a881 cf3b  ...K0!8u\......;
-00002a20: 56a8 9d29 752b b72d 45be 4535 4eed a5e5  V..)u+.-E.E5N...
-00002a30: f93b 3e95 9ad0 4441 f6f6 537c 0faf 834b  .;>...DA..S|...K
-00002a40: a2a0 ffd5 a4ac d03d 98f5 a289 d630 ec52  .......=.....0.R
-00002a50: 7198 6ee0 3d18 3cc9 67f1 f40b bcd1 793e  q.n.=.<.g.....y>
-00002a60: f0ad ed67 6473 efe1 7359 ccca 171f cff4  ...gds..sY......
-00002a70: 9c52 9d9a 1341 db64 f549 427c 70c6 c5d7  .R...A.d.IB|p...
-00002a80: 2b9b 4c88 2256 e01c 4246 f1e2 a8a0 93ed  +.L."V..BF......
-00002a90: d6f6 f48d 946a 6b9f 42a7 da15 467b bc40  .....jk.B...F{.@
-00002aa0: c59d a448 6ee7 7a06 1870 476f 0422 e6d9  ...Hn.z..pGo."..
-00002ab0: 2dc1 70af ee6b 9814 f996 6cd4 17ac a0af  -.p..k....l.....
-00002ac0: 1908 957f efa4 ba22 0c5f 6072 bb55 97cc  ......."._`r.U..
-00002ad0: 6499 d523 71b6 ba42 47be 53f6 458d cbb9  d..#q..BG.S.E...
-00002ae0: 9d2c 7037 862a 6c1f f271 5a5c f312 5a3f  .,p7.*l..qZ\..Z?
-00002af0: 880a f2f6 b2d7 024d 6636 a9d3 6988 4392  .......Mf6..i.C.
-00002b00: 41ae e1b6 0c32 48a9 9c3c e039 2b3f c02d  A....2H..<.9+?.-
-00002b10: 0868 b489 f4f3 1e7c cf01 ccb4 e54f d077  .h.....|.....O.w
-00002b20: 6e8e 35ce 3082 28c2 c4fd 35c6 cc9b 6594  n.5.0.(...5...e.
-00002b30: d4d7 041a 8ab8 6425 b4a4 5f66 8c6c 3658  ......d%.._f.l6X
-00002b40: 8001 024d ea1a 4a86 087e 3071 b65d ee57  ...M..J..~0q.].W
-00002b50: d985 0cfb 06cc d0f6 4348 d9e2 6ec1 95e2  ........CH..n...
-00002b60: d5c5 b1de 42ac ffdf 4bba a26b eb0c d6a8  ....B...K..k....
-00002b70: d2b4 027d f802 25fd c8ea 45a1 17af 1a4f  ...}..%...E....O
-00002b80: 35da 227e 128e d2ac 1349 fdf1 b2e9 8ca7  5."~.....I......
-00002b90: 4890 24d1 d2f4 a2e7 48b8 f4b2 b813 8982  H.$.....H.......
-00002ba0: 3059 7523 affa 1665 7e96 74ca c493 781e  0Yu#...e~.t...x.
-00002bb0: 77ca 248b 28f0 3b65 468b 3048 9a02 7c86  w.$.(.;eF.0H..|.
-00002bc0: acfc 387a 0509 268b 4e64 3cf1 c6c9 a20b  ..8z..&.Nd<.....
-00002bd0: 99a4 d12a 1a77 218b d4f3 579d 115d a449  ...*.w!...W..].I
-00002be0: 3a9f 7721 cb70 b49c 8f3a 91c4 5b2d 3a63  :.w!.p...:..[-:c
-00002bf0: b04c c238 4abb 90d4 1bf9 41a7 4c9a f9f3  .L.8J.....A.L...
-00002c00: 38ea 4256 de68 39ea d406 e6c3 5133 6b4f  8.BV.h9.....Q3kO
-00002c10: 916c 9c4c 569d dab2 34c8 16dd 322b 2f98  .l.LV...4...2+/.
-00002c20: 9b88 0e1f 73b9 9aea c556 0f14 7bd2 0db1  ....s....V..{...
-00002c30: 5759 8925 aad6 82a0 deb5 5e7d 879a 632d  WY.%......^}..c-
-00002c40: ee16 8439 7c8d 6175 c24f 917c b776 e060  ...9|.au.O.|.v.`
-00002c50: 6001 5921 4a33 284d 0798 e7a9 cc2a 00d3  `.Y!J3(M.....*..
-00002c60: d59c e935 12b7 adde 8643 7452 6186 7f78  ...5.....CtRa..x
-00002c70: d4a5 972c 2cfe 8475 a9b6 e841 a0da 363a  ...,,..u...A..6:
-00002c80: c7e2 4751 2349 184c a9ca d1e5 6e9d 3b29  ..GQ#I.L....n.;)
-00002c90: 06cb de13 0876 af4f 7b61 e2d4 86e7 3055  .....v.O{a....0U
-00002ca0: d038 ccc0 b842 ed2a 84d9 e06b ae5b 0646  .8...B.*...k.[.F
-00002cb0: 52cd 2541 b3fe c376 b0fc 68e3 5f50 91eb  R.%A...v..h._P..
-00002cc0: 7e83 af51 5ddb b6b5 bef5 677d aa07 a5af  ~..Q].....g}....
-00002cd0: c514 7c95 f0a3 c97c ac6f 8306 0b0c 1658  ..|....|.o.....X
-00002ce0: cc7c a042 5f16 b89b 434b 0b1c ed09 5fe8  .|.B_...CK...._.
-00002cf0: 6861 4b8b 1c2d 6a69 b1a3 c52d 2d71 b444  haK..-ji...--q.D
-00002d00: d3b6 30a8 04ac 9b77 d041 dd51 d337 9c52  ..0....w.A.Q.7.R
-00002d10: 7ec0 e545 8bbf 20d9 2098 d5eb 6777 b186  ~..E.. . ...gw..
-00002d20: 9b9a 1de2 8457 639a b93e d5a0 f7d8 6666  .....Wc..>....ff
-00002d30: 0c4f 844d d63f f345 2fc6 0581 0ccd 8fd5  .O.M.?.E/.......
-00002d40: badd 2ccf ace3 9448 9837 352c a18a 0b87  ..,....H.75,....
-00002d50: fd61 303f 8295 a8b8 84e2 8293 a187 cb6c  .a0?...........l
-00002d60: 1e84 a12d 633f 36cb ab32 2309 defd 0bde  ...-c?6..2#.....
-00002d70: 2c90 c465 8339 d1d8 8afe 13c7 a30c 2a7d  ,..e.9........*}
-00002d80: 3ec8 c671 3688 d251 3a58 2c47 f160 9584  >..q6..Q:X,G.`..
-00002d90: 9378 1507 f328 f2ff 6dea d6fd 2c3f ff0f  .x...(..m...,?..
-00002da0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00002db0: 0000 2100 6d8e ecaa 8513 0000 3bc6 0000  ..!.m.......;...
-00002dc0: 0f00 0000 776f 7264 2f73 7479 6c65 732e  ....word/styles.
-00002dd0: 786d 6cec 5dcf 8fe4 3815 be23 f13f 4475  xml.]...8..#.?Du
-00002de0: 8243 6f77 fde8 ea9e 11bd a87f 3223 6666  .Cow........2#ff
-00002df0: 87ed 9edd 732a 7175 653b 1517 496a 7a7a  ....s*que;..Ijzz
-00002e00: ce08 8438 2201 421c 8003 e200 5c10 070e  ...8".B.....\...
-00002e10: fc37 ec00 ff05 b6e3 a49c 7a76 2acf 71d7  .7........zv*.q.
-00002e20: 4c8f 16a4 9dae 24fe 6cbf ef7d cf7e 8e93  L.....$.l..}.~..
-00002e30: 7cef fb6f e6b1 f79a a459 4493 a35e ff93  |..o.....YD..^..
-00002e40: bd9e 4792 8086 5172 7dd4 7b75 75b1 73d8  ..G...Qr}.{uu.s.
-00002e50: f3b2 dc4f 423f a609 39ea dd91 acf7 fd4f  ...OB?..9......O
-00002e60: bffd adef dd3e cef2 bb98 641e 0348 b2c7  .....>....d..H..
-00002e70: f3e0 a837 cbf3 c5e3 dddd 2c98 91b9 9f7d  ...7......,....}
-00002e80: 4217 2461 27a7 349d fb39 fb99 5eef cefd  B.$a'.4..9..^...
-00002e90: f466 b9d8 09e8 7ce1 e7d1 248a a3fc 6e77  .f....|...$...nw
-00002ea0: b0b7 37ee 4998 b40d 0a9d 4ea3 809c d160  ..7.I.....N....`
-00002eb0: 3927 492e caef a624 6688 34c9 66d1 222b  9'I....$f.4.f."+
-00002ec0: d16e dba0 ddd2 345c a434 2059 c63a 3d8f  .n....4\.4 Y.:=.
-00002ed0: 0bbc b91f 2515 4c7f 0480 e651 90d2 8c4e  ....%.L....Q...N
-00002ee0: f34f 5867 648b 0414 2bde df13 7fcd e315  .OXgd...+.......
-00002ef0: c03e 0e60 0000 c641 14e2 30c6 1263 9795  .>.`...A..0..c..
-00002f00: 5470 3282 83d9 2f61 b2bb 3979 d3f3 e6c1  Tp2.../a..9y....
-00002f10: e3a7 d709 4dfd 49cc 9098 693c d63b 4f00  ....M.I...i<.;O.
-00002f20: f3ff f2ca 3e65 ce11 d2e0 8c4c fd65 9c67  ....>e.....L.e.g
-00002f30: fc67 fa32 953f e52f f1cf 054d f2cc bb7d  .g.2.?./...M...}
-00002f40: ec67 4114 1df5 befe db2f fefd af5f f6d8  .gA....../..._..
-00002f50: 01e2 67f9 7116 f9ea b1d9 7192 d52e 0ab2  ..g.q.....q.....
-00002f60: 9cb5 9f35 621e b1f6 9c44 61d4 dbe5 b037  ...5b....Da....7
-00002f70: 244d d8e9 d77e 7cd4 1b14 87b2 b7d5 817e  $M...~|........~
-00002f80: 79e4 94d7 5c3b 16fb c975 798c 243b af2e  y...\;...uy.$;..
-00002f90: eb4d 793b db39 7dc1 0f4d 5855 473d 3fdd  .My;.9}..MXUG=?.
-00002fa0: b93c e605 7765 878a 7f95 6e2e d67f 898a  .<..we....n.....
-00002fb0: 177e 1089 7a26 84b9 2179 1625 243b eaed  .~..z&..!y.%$;..
-00002fc0: ef09 6471 a8fc e54f 7392 d6ce 8b23 e247  ..dq...Os....#.G
-00002fd0: 51af c02c fead 6ada 05c6 67ca 603a b92c  Q..,..j...g.`:.,
-00002fe0: e4ca ce92 e933 1adc 90f0 3267 278e 7a02  .....3....2g'.z.
-00002ff0: 991d 7cf5 f465 1ad1 9449 f2a8 f7e8 913c  ..|..e...I.....<
-00003000: 7849 e6d1 9328 0c49 a25c 98cc a290 7c39  xI...(.I.\....|9
-00003010: 23c9 ab8c 84ab e33f ba10 b292 0702 ba4c  #......?.......L
-00003020: d8df c383 7de1 1071 169e bf09 c882 8b94  ....}..q........
-00003030: 9d4d 7cce dc0b 5e20 e657 2fa3 55e5 a2f8  .M|...^ .W/.U...
-00003040: 8f4b b092 1c5d f919 f179 a4f2 faeb 10a2  .K...]...y......
-00003050: f928 8801 2f91 29bd d563 2ed7 fa2e ae42  .(../.)..c.....B
-00003060: 5534 dc56 45a3 6d55 b4bf ad8a c6db aae8  U4.VE.mU........
-00003070: 605b 151d 6eab 2201 739f 1545 4948 de14  `[..n.".s..EIH..
-00003080: 4284 d500 d44d 3806 35a2 710c 6243 e318  B....M8.5.q.bC..
-00003090: b484 c631 4805 8d63 5002 1ac7 e0e8 681c  ...1H..cP.....h.
-000030a0: 831f a371 0c6e 8ac0 c969 60f2 42c5 d987  ...q.n...i`.B...
-000030b0: 066f 6fc6 dd3c 46d8 e16e 1e12 ec70 378f  .oo..<F..n...p7.
-000030c0: 0076 b89b 03be 1dee e6f8 6e87 bb39 9cdb  .v........n..9..
-000030d0: e16e 8ede 76b8 9b83 351e b798 6a79 4f99  .n..v...5...jyO.
-000030e0: cc92 bcb3 caa6 94e6 09cd 8997 9337 ddd1  .............7..
-000030f0: fc84 6189 f4cd 0d1e 1ff4 48ea a493 0e60  ..a.......H....`
-00003100: 8ac8 2607 e2ce 6881 2f7e 6ff6 1021 52fb  ..&...h./~o..!R.
-00003110: f13c e709 9e47 a7de 34ba 5ea6 2ceb efda  .<...G..4.^.,...
-00003120: 7092 bc26 31cb bf3d 3f0c 199e 43c0 94e4  p..&1..=?...C...
-00003130: cbd4 6011 1b9f 4ec9 94a4 2409 884b c776  ..`...N...$..K.v
-00003140: 071a b38c d04b 96f3 8903 df5c f8d7 ceb0  .....K.....\....
-00003150: 4812 3a36 5f89 e824 2854 0eed 2ff3 1917  H.:6_..$(T../...
-00003160: 49e4 c0a9 e77e 90d2 ee4d a3be b3f8 f02c  I....~...M.....,
-00003170: caba db8a 8378 27cb 3826 8eb0 5eb8 7131  .....x'.8&..^.q1
-00003180: 81d5 3d37 1030 dd53 0301 d33d 3310 30dd  ..=7.0.S...=3.0.
-00003190: 1303 8533 5726 9268 8e2c 25d1 1c19 4ca2  ...3W&.h.,%...L.
-000031a0: 39b2 5be1 9fae ec26 d11c d94d a239 b29b  9.[....&...M.9..
-000031b0: 44eb 6eb7 ab28 8f45 8857 671d fdf6 6b77  D.n..(.E.Wg...kw
-000031c0: a731 e50b ee9d db71 195d 273e 9b00 741f  .1.....q.]'>..t.
-000031d0: 6ee4 9aa9 f7d2 4ffd ebd4 5fcc 3cbe 40ad  n.....O..._.<.@.
-000031e0: 8755 fb8c ade7 8486 77de 958b 31ad 4272  .U......w...1.Br
-000031f0: 35af 172e 72ca 7a1d 25cb ee06 ada1 b912  5...r.z.%.......
-00003200: 5785 e748 5e15 9e23 8155 78dd 25f6 9c4d  W..H^..#.Ux.%..M
-00003210: 93f9 04ed 899b 7ce6 7239 c9b5 a215 48ad  ......|.r9....H.
-00003220: 447b e9c7 cb62 42db 5d6d 7ede ddc3 5602  D{...bB.]m~...V.
-00003230: b888 d2cc 990c f4b0 0e3c f805 9fce 723a  .........<....r:
-00003240: 5d44 be55 2bbb 376c 85d5 5d56 eb51 c969  ]D.U+.7l..]V.Q.i
-00003250: f324 a483 56c6 34b8 7113 869f dc2d 48ca  .$..V.4.q....-H.
-00003260: d2b2 9bce 4817 348e e92d 09dd 215e e629  ....H.4..-..!^.)
-00003270: 2d7c 4d95 fc40 50d2 4af2 e7f3 c5cc cf22  -|M..@P.J......"
-00003280: 912b d520 da0f f5e5 ad7a efb9 bfe8 dca1  .+. .....z......
-00003290: 97b1 1f25 6e78 3bdf 99fb 51ec b99b 413c  ...%nx;...Q...A<
-000032a0: b97a fecc bba2 0b9e 6672 c3b8 013c a179  .z......fr...<.y
-000032b0: 4ee7 ce30 e54a e077 be24 93ef ba69 e031  N..0.J.w.$...i.1
-000032c0: 4b82 933b 47bd 3d76 b43c 24c0 4e23 0783  K..;G.=v.<$.N#..
-000032d0: 4c81 4443 4748 6c9a 1925 9193 3154 e0fd  L.DCGHl..%..1T..
-000032e0: 90dc 4da8 9f86 6ed0 5ea6 7c0f 0293 744e  ..M...n.^.|...tN
-000032f0: 1c21 5efa f345 31e9 70a0 2d16 176f 59fc  .!^..E1.p.-..oY.
-00003300: 7130 1b12 785f f869 c4d7 855c 89ea ca09  q0..x_.i...\....
-00003310: 98b2 6c98 2d27 5f91 a07b a87b 413d 272b  ..l.-'_..{.{A='+
-00003320: 439f 2d73 b1fe 28a6 baa2 b43b b8ee d384  C.-s..(....;....
-00003330: 1a5c f729 8260 930d 0fdc 7f1d 74b6 06d7  .\.).`......t...
-00003340: bdb3 3538 579d 3d8d fd2c 8b8c b750 adf1  ..58W.=..,...P..
-00003350: 5c75 b7c4 73dd dfee c99f c4a3 314d a7cb  \u..s.......1M..
-00003360: d89d 014b 4067 162c 019d 9990 c6cb 7992  ...K@g.,......y.
-00003370: b9ec b1c0 73d8 6181 e7ba bf0e 5d46 e039  ....s.a.....]F.9
-00003380: 5892 1378 3f48 a3d0 1919 02cc 1513 02cc  X..x?H..........
-00003390: 150d 02cc 1507 02cc 2901 dd77 e828 60dd  ........)..w.(`.
-000033a0: b7e9 2860 ddf7 ea14 608e a600 0a98 2b3f  ..(`....`.....+?
-000033b0: 733a fc3b bacb a380 b9f2 3301 e6ca cf04  s:.;......3.....
-000033c0: 982b 3f13 60ae fc6c 78e6 91e9 944d 82dd  .+?.`..lx....M..
-000033d0: 0d31 0aa4 2b9f 5320 dd0d 3449 4ee6 0b9a  .1..+.S ..4IN...
-000033e0: fae9 9d23 c8f3 985c fb0e 1648 0bb4 9729  ...#...\...H...)
-000033f0: 9df2 c726 6852 6ce2 7600 c9d7 a863 8793  ...&hRl.v....c..
-00003400: ed02 ce15 c95f 9289 b3a6 712c 97ed 72b0  ....._....q,..r.
-00003410: 22ea c731 a58e d6d6 5603 8e28 59df bbb6  "..1....V..(Y...
-00003420: a9d8 157f b0a3 7313 5ec6 7e40 6634 0e49  ......s.^.~@f4.I
-00003430: 6ae8 93b9 2ccb 972f 8b27 35d6 9b2f 9ad1  j...,../.'5../..
-00003440: 6ad9 f359 743d cbbd cb59 b5da afc2 8cc5  j..Yt=...Y......
-00003450: 331c 8d25 cb84 bd56 6c73 853a 9b8f e583  3..%...Vls.:....
-00003460: 30da 62cf 4918 2de7 6543 e1c3 14e3 61fb  0.b.I.-.eC....a.
-00003470: c2c2 a36b 8547 9b0b af66 12b5 92fb 2d4b  ...k.G...f....-K
-00003480: c23a c79b 4bae 66c9 b592 072d 4bc2 3a0f  .:..K.f....-K.:.
-00003490: 5b96 143a ad95 6cd2 c399 9fde 681d e1a0  [..:..l.....h...
-000034a0: c97f aa1c cfe0 7c07 4d5e 5415 d656 dbe4  ......|.M^T..V..
-000034b0: 4855 499d 0b1e 3479 514d 2ade 7110 f0bb  HUI...4yQM*.q...
-000034c0: 0590 9d76 9a31 976f 271e 7379 8c8a cc28  ...v.1.o'.sy...(
-000034d0: 1839 9951 5aeb ca0c d124 b0cf c9eb 888f  .9.QZ....$......
-000034e0: ec98 a029 eaab 764f 80b8 2f26 d1ad 22e7  ...)..vO../&..".
-000034f0: 8f96 b458 b7af dd70 6aff 50d7 5336 714a  ...X...pj.P.S6qJ
-00003500: 32e2 6971 86ed 6f5c d5a2 8cd9 8ead c38d  2.iq..o\........
-00003510: 19a2 75dc 3143 b40e 4066 8856 91c8 581c  ..u.1C..@f.V..X.
-00003520: 1592 cc28 ad63 9319 a275 9032 43a0 a315  ...(.c...u.2C...
-00003530: 1c11 70d1 0a96 c745 2b58 de26 5a41 149b  ..p....E+X.&ZA..
-00003540: 68d5 6116 6086 683d 1d30 43a0 850a 21d0  h.a.`.h=.0C...!.
-00003550: 42ed 3053 3043 a084 0a8a 5b09 15a2 a085  B.0S0C....[.....
-00003560: 0a21 d042 8510 68a1 c209 184e a8b0 3c4e  .!.B..h....N..<N
-00003570: a8b0 bc8d 5021 8a8d 5021 0a5a a810 022d  ....P!..P!.Z...-
-00003580: 5408 8116 2a84 400b 1542 a085 6a39 b737  T...*.@..B..j9.7
-00003590: 16b7 122a 4441 0b15 42a0 850a 21d0 4215  ...*DA..B...!.B.
-000035a0: f3c5 0e42 85e5 7142 85e5 6d84 0a51 6c84  ...B..qB..m..Ql.
-000035b0: 0a51 d042 8510 68a1 4208 b450 2104 5aa8  .Q.B..h.B..P!.Z.
-000035c0: 1002 2d54 0881 122a 286e 2554 8882 162a  ..-T...*(n%T...*
-000035d0: 8440 0b15 42a0 855a 3c6a 682f 5458 1e27  .@..B..Z<jh/TX.'
-000035e0: 5458 de46 a810 c546 a810 052d 5408 8116  TX.F...F...-T...
-000035f0: 2a84 400b 1542 a085 0a21 d042 8510 28a1  *.@..B...!.B..(.
-00003600: 82e2 5642 8528 68a1 4208 b450 2104 5aa8  ..VB.(h.B..P!.Z.
-00003610: e266 6107 a1c2 f238 a1c2 f236 4285 2836  .fa....8...6B.(6
-00003620: 4285 2868 a142 08b4 5021 045a a810 022d  B.(h.B..P!.Z...-
-00003630: 5408 8116 2a84 4009 1514 b712 2a44 410b  T...*.@.....*DA.
-00003640: 1542 a085 0a21 9afc 53de a234 6db3 efe3  .B...!..S..4m...
-00003650: 573d 8d3b f6db dfba 928d fa5c 7d94 5b85  W=.;.......\}.[.
-00003660: 1ab6 872a 5b65 c66a ff2c c209 a537 9ef6  ...*[e.j.,...7..
-00003670: c1c3 a1c8 37da 8144 9338 a262 89da 705b  ....7..D.8.b..p[
-00003680: 5dc5 155b 2250 373e 3f3b 6d7e c247 45ef  ]..["P7>?;m~.GE.
-00003690: f8d2 25f9 2c84 b867 0ac0 476d 4b82 3595  ..%.,..g..GmK.5.
-000036a0: 5193 cbab 2541 9237 6af2 74b5 2498 758e  Q...%A.7j.t.$.u.
-000036b0: 9aa2 af5a 120c 83a3 a6a0 2b74 596e 4a61  ...Z......+tYnJa
-000036c0: c311 28dc 1466 94c2 7d43 f1a6 68ad 1487  ..(..f..}C..h...
-000036d0: 266e 8ad1 4a41 68e1 a6c8 ac14 8406 6e8a  &n..JAh.......n.
-000036e0: c74a c17d 8f07 e7f5 d2c5 2b07 3797 1e57  .J.}......+.7..W
-000036f0: fb4b 0142 933b 2a08 0766 8426 b784 5c95  .K.B.;*..f.&..\.
-00003700: e118 0aa3 2d69 6684 b6ec 9911 dad2 6846  ....-if.......hF
-00003710: 40f1 6984 c113 6b86 4233 6c86 b2a3 1aca  @.i...k.B3l.....
-00003720: 0c4b b5bd 50cd 0858 aa21 8215 d500 c69e  .K..P..X.!......
-00003730: 6a08 654d 3584 b2a3 1a06 462c d510 014b  j.eM5.....F,...K
-00003740: b57d 7036 2358 510d 60ec a986 50d6 5443  .}p6#XQ.`...P.TC
-00003750: 283b aae1 5086 a51a 2260 a986 0858 aa3b  (;..P..."`...X.;
-00003760: 0ec8 4618 7baa 2194 35d5 10ca 8e6a 38b9  ..F.{.!.5....j8.
-00003770: c352 0d11 b054 4304 2cd5 10c1 8a6a 0063  .R...TC.,....j.c
-00003780: 4f35 84b2 a61a 42d9 510d b264 34d5 1001  O5....B.Q..d4...
-00003790: 4b35 44c0 520d 11ac a806 30f6 5443 286b  K5D.R.....0.TC(k
-000037a0: aa21 5413 d562 15a5 4635 8a61 a538 6e12  .!T..b..F5.a.8n.
-000037b0: a614 c40d c84a 415c 7056 0a5a 644b 4a69  .....JA\pV.ZdKJi
-000037c0: cb6c 4941 b0cc 9620 5725 e7b8 6c49 25cd  .lIA... W%..lI%.
-000037d0: 8cd0 963d 3342 5b1a cd08 283e 8d30 7862  ...=3B[...(>.0xb
-000037e0: cd50 6886 cd50 7654 e3b2 251d d5f6 4235  .Ph..PvT..%...B5
-000037f0: 2360 a9c6 654b 46aa 71d9 5223 d5b8 6ca9  #`..eKF.q.R#..l.
-00003800: 916a 5cb6 64a6 1a97 2de9 a8c6 654b 3aaa  .j\.d...-...eK:.
-00003810: ed83 b319 c18a 6a5c b6d4 4835 2e5b 6aa4  ......j\..H5.[j.
-00003820: 1a97 2d99 a9c6 654b 3aaa 71d9 928e 6a5c  ..-...eK:.q...j\
-00003830: b6a4 a3ba e380 6c84 b1a7 1a97 2d35 528d  ......l.....-5R.
-00003840: cb96 cc54 e3b2 251d d5b8 6c49 4735 2e5b  ...T..%...lIG5.[
-00003850: d251 8dcb 968c 54e3 b2a5 46aa 71d9 5223  .Q....T...F.q.R#
-00003860: d5b8 6cc9 4c35 2e5b d251 8dcb 9674 54e3  ..l.L5.[.Q...tT.
-00003870: b225 1dd5 b86c c948 352e 5b6a a41a 972d  .%...l.H5.[j...-
-00003880: 3552 8dcb 969e b322 9183 5740 5dce fd34  5R....."..W@]..4
-00003890: f7dc bd2f ee89 9fcd 72bf fbcb 095f 2529  .../....r...._%)
-000038a0: c968 fc9a 841e baab bbb7 b56f 56f1 3ac4  .h.........oV.:.
-000038b0: c7e6 d8f5 39eb 287f 6db9 f28c 5158 bcb6  ....9.(.m...QX..
-000038c0: 5502 8a0b 9f32 245f 7c76 8a37 c693 dff4  U....2$_|v.7....
-000038d0: 925f 9b12 6d96 b757 8bca 4499 0db5 54b8  ._..m..W..D...T.
-000038e0: 7d80 bbfa 0a95 809e f8ac 279f 714b 88b3  }.........'.qK..
-000038f0: 7e71 34e1 2f2f ac1f e27c 9587 fad2 8357  ~q4.//...|.....W
-00003900: fe53 9e91 0a59 35f8 f671 9ab1 a45d 9ede  .S...Y5..q...]..
-00003910: db3b 7cb4 7738 3e29 ae92 1f19 bb21 64f1  .;|.w8>).....!d.
-00003920: 8255 288e f11f e22b 62e2 d7fa f7c7 f873  .U(....+b......s
-00003930: 59ea b7c5 86c5 e351 fc35 4acc 830f c443  Y......Q.5J....C
-00003940: fcfc c7e7 4bfe bd37 7f99 d3a2 265a bc6a  ....K..7....&Z.j
-00003950: e9d9 ebb8 6a89 a44e b641 7ee4 6d52 d8e4  ....j..N.A~.mR..
-00003960: b4a8 5dfd 365b 79c7 77f5 71b6 d591 d5c7  ..].6[y.w.q.....
-00003970: d98a 63ca 37d6 5064 0d8c 6449 6d5a 9135  ..c.7.Pd..dImZ.5
-00003980: d844 56dd abef 99bf c158 e54f fe2a f81b  .DV......X.O.*..
-00003990: f545 506a c75f 29bd 3a7f f58f f489 07b3  .EPj._).:.......
-000039a0: f96b efbf a2e9 13fe 413e 0e5f 7e22 4f3d  .k......A>._~"O=
-000039b0: 792e 8ff1 f3e2 cb7d da92 ab4f f8f1 c327  y......}...O...'
-000039c0: d527 fcea 4eb3 7290 a164 4d75 90e2 98ad  .'..N.r..dMu....
-000039d0: 830c 8d0e 2277 3258 39c8 f0a3 7490 d2d0  ...."w2X9...t...
-000039e0: 4d02 bf4f ae46 46ae 64dc b0e2 aadc 01f2  M..O.FF.d.......
-000039f0: 8170 7558 e3ea 91c2 d5f0 00c1 95f0 de0f  .puX............
-00003a00: 5bcc 0339 7bac 7d8a 531c b375 90e2 4b93  [..9{.}.S..u..K.
-00003a10: 3a07 915b 84ac 1ca4 9c5c 7e5c 0e52 0eab  :..[.....\~\.R..
-00003a20: edc4 ec9e abb1 912b 99d8 5871 55ee 67fe  .......+..XqU.g.
-00003a30: 40b8 aacd acc6 22ed 9754 156f 4f6e 4795  @....."..T.oOnG.
-00003a40: 70de 0f5c cb9a 995b 71cc d63f 0e8c fe21  p..\...[q..?...!
-00003a50: d356 2bff 2877 157f 54fe 2104 d35e cace  .V+.(w..T.!..^..
-00003a60: a93a 3452 25a3 8615 5587 1f23 55c2 773f  .:4R%...U..#U.w?
-00003a70: 0c29 bbf1 8860 c65c 2290 ef63 3665 e27b  .)...`.\"..c6e.{
-00003a80: c041 0c9f 5a31 102e 13eb d5e2 819e 7f73  .A..Z1.........s
-00003a90: 2b73 be64 d3d4 4298 d4d7 5ee8 6c72 44e9  +s.d..B...^.lrD.
-00003aa0: 899b 1ac6 9a31 890b aad9 1f4f 13ee 97b7  .....1.....O....
-00003ab0: f23b d745 03c3 3752 01ec fc29 89e3 e77e  .;.E..7R...)...~
-00003ac0: 7135 5d98 2f8d c994 ebe7 962f 1e88 347d  q5]./....../..4}
-00003ad0: edfc a478 6dbc b17c 2ad6 178d 00bb f5c6  ...xm..|*.......
-00003ae0: 143f 9b9d a1f8 909c dcf8 6e32 354c c9cb  .?........n25L..
-00003af0: 7753 77b4 720b fa57 ad80 795f b1ac c7f7  wSw.r..W..y_....
-00003b00: 43e8 8396 7442 d8be f27d 66f5 8073 7ed2  C...tB...}f..s~.
-00003b10: e7f3 3135 e0c0 a8a2 c694 b5e5 13d5 634e  ..15..........cN
-00003b20: 681a 9254 ac83 151e 21ea e05f 4f92 dd7a  h..T....!.._O..z
-00003b30: cbe7 73fc 0f56 4309 1bf0 e549 351a 497f  ..s..VC....I5.I.
-00003b40: b12a 5bf9 9255 e9d2 d3ac 0a47 2c8e 85e4  .*[..U.....G,...
-00003b50: 49b7 e25f d815 2f9c be32 7f1b 0d40 5f3b  I.._../..2...@_;
-00003b60: d881 73dd 0d0b c938 072c d799 110e a8f7  ..s....8.,......
-00003b70: 3939 1c09 2354 e0c3 c37e f12d 5131 8c88  99..#T...~.-Q1..
-00003b80: b6b2 c688 968a 7443 1ce6 cf61 b1ce 9f5c  ......tC...a...\
-00003b90: a8a3 46dd 892f b93d 3ea7 b727 7e12 5e46  ..F../.=>..'~.^F
-00003ba0: 6f2b 53c8 6e95 57b0 0ab4 57ac 6cbf baf6  o+S.n.W...W.l...
-00003bb0: 256f 6561 f629 ff4e 0f43 1796 7e9f c36a  %oea.).N.C..~..j
-00003bc0: 54fc 174e bbca 599a 6a9a a2e7 813c 1228  T..N..Y.j....<.(
-00003bd0: 3ab7 11dc c1de f1d9 483c afa4 a34a da50  :.......H<...J.P
-00003be0: ad24 9b55 fe12 c4c4 1763 b8aa 00f6 731a  .$.U.....c....s.
-00003bf0: c5ec ec85 f85f 857c 210e 4efc e0e6 3aa5  ....._.|!.N...:.
-00003c00: cb24 ac08 123d 2998 9204 19e8 8afd 8f8a  .$...=).........
-00003c10: 2d74 547e 4054 0965 b106 0aae 64a0 f82a  -tT~@T.e....d..*
-00003c20: 281b 2342 bb36 8a3c 643e 2d06 ac07 26be  (.#B.6.<d>-...&.
-00003c30: 92d0 8f80 2cfc bce6 0171 3561 6361 ff0b  ....,....q5aca..
-00003c40: 92e6 822d 6889 d62d 3b1f 9c5f 9c89 c74d  ...-h..-;.._...M
-00003c50: 9596 ad0f e3fc e855 94e4 e279 5aab a63e  .......U...yZ..>
-00003c60: a1e9 db0f bfa9 09e1 798d a19d 46e7 4a22  ........y...F.J"
-00003c70: 71f3 b8ee 1cb8 7a6f dbd6 5b8b 40dd 2bce  q.....zo..[.@.+.
-00003c80: de53 87b3 2d74 7817 3117 1f37 cfc5 75fb  .S..-tx.1..7..u.
-00003c90: 4344 93db cfc5 e519 cbb9 b83a b4f2 fa49  CD.........:...I
-00003ca0: 5a1f 5bc1 14d8 7e42 2dae d0cf 6142 ba2c  Z.[...~B-...aB.,
-00003cb0: 0d67 911d e24a 1764 6a52 ac95 9fbc 3e8e  .g...J.djR....>.
-00003cc0: a3eb caf6 35b3 54ae d42e 2398 14cd 1523  ....5.T...#....#
-00003cd0: 4eeb f165 0b53 71f4 f0ed a25f 68c2 efb3  N..e.Sq...._h...
-00003ce0: 53b5 5966 43af da1a c811 d437 c36f c7a6  S.YfC......7.o..
-00003cf0: b608 cec1 3263 fa12 25c0 6261 e2c7 7759  ....2c..%.ba..wY
-00003d00: 94ed 847e 0ef7 73d5 cfe2 e274 b9a8 588f  ...~..s....t..X.
-00003d10: d3e3 93d1 a02f cf18 16ed c44d 02a9 0bb8  ...../.....M....
-00003d20: 8ca7 9efd 26ae 6f2d ae57 e94b 99a4 1cf5  ....&.o-.W.K....
-00003d30: befe db2f fefd af5f 16fd 58bf d571 7f21  .../..._..X..q.!
-00003d40: 52bf da2a a733 4e97 512b ccb5 f5d1 b5e3  R..*.3N.Q+......
-00003d50: 960b 9fac ebf1 60c2 8d5e 07cd d3c1 a4ba  ......`..^......
-00003d60: 99a5 9da5 e192 a5c1 e9a9 36d0 88f6 398a  ..........6...9.
-00003d70: 8955 f846 3b4b 99ae a186 8bc1 96eb 5bc5  .U.F;K........[.
-00003d80: fc2d f5cf 517d 18f1 55fe d742 55d5 e14e  .-..Q}..U..BU..N
-00003d90: 7259 79fc 03d3 418b 01b7 1a5e 47f0 b667  rYy...A....^G..g
-00003da0: fd1d 4d85 79db 8ea9 e5f6 ddfa 987a 3ae6  ..M.y........z:.
-00003db0: e94f 71a6 e57d 0887 a361 6ddc b14f 12da  .Oq..}...am..O..
-00003dc0: 4e3b 1d41 7dec b3e1 8b01 ffff 9ac7 abcb  N;.A}...........
-00003dd0: 64ea 1979 6fe9 a2dc 3bfa 1ea6 c4ee db6b  d..yo...;......k
-00003de0: 96a9 7e8f 8daf dffc 5a4c 98a0 4665 b454  ..~.....ZL..Fe.T
-00003df0: b6d3 f872 0ba4 792a acd9 b650 57f2 d945  ...r..y*...PW..E
-00003e00: ff78 5f6a 5c2a 7571 1216 1ed5 30b1 1149  .x_j\*uq....0..I
-00003e10: 839c 6b08 4bc1 9962 09c3 4254 11fa fd49  ..k.K..b..BT...I
-00003e20: 454c 312d 643f 1734 e321 6b5f 6ecc 56ae  EL1-d?.4.!k_n.V.
-00003e30: 296e 4294 971c 0ef7 aa6c 54e2 6589 bfb8  )nB......lT.e...
-00003e40: a2e2 5d07 656f 0a90 e659 b994 cb6a 04eb  ..].eo...Y...j..
-00003e50: 6bb6 4116 c714 1919 78ad ed94 69ca 79e0  k.A.....x...i.y.
-00003e60: 2ed6 fffd e11f fff9 ddcf bdaf fffa ebff  ................
-00003e70: fce5 4f7a c2cb 07a0 54c6 2555 6d93 1f95  ..Oz....T.%Um...
-00003e80: 5ea7 3d37 7834 5c89 9b52 2a39 68e5 d172  ^.=7x4\..R*9h..r
-00003e90: 23a0 5b8f deb2 0bbe 6f67 83db 2c99 b3fd  #.[.....og..,...
-00003ea0: f727 bf45 3b9b 5cdd fcb0 9cad a1e7 8b1d  .'.E;.\.........
-00003eb0: 31c8 eef0 0d7a 3b51 1232 8e81 2974 d7b4  1....z;Q.2..)t..
-00003ec0: 744e 4d51 6935 f31e c547 67a3 f3f2 914a  tNMQi5...Gg....J
-00003ed0: e396 a1fe be88 a772 e2c4 7f89 eb23 b1a9  .......r.....#..
-00003ee0: 4cd4 c9d7 204e 19ff 197f 5049 2477 d561  L... N....PI$w.a
-00003ef0: e6bc 839a db39 b663 42f3 56b6 54ae b3b1  .....9.cB.V.T...
-00003f00: e7aa f83d da74 b389 da8a 4ceb 0b2d 7c0d  ...=.t....L..-|.
-00003f10: ab41 a3bb 9a4c 726f ecef c890 d9d2 09ca  .A...Lro........
-00003f20: cb75 1d6d f49b 161e 22b1 6d1c a569 72e0  .u.m....".m..ir.
-00003f30: d82b 548f 6e69 b44e deb1 6e48 bc87 b4ed  .+T.ni.N..nH....
-00003f40: 661f 76e8 ddef 7ff6 bf3f fec6 eb63 7b60  f.v......?...c{`
-00003f50: 5ecc d575 42dd f1ad c97b eef3 59d4 8e2e  ^..uB....{..Y...
-00003f60: 50b9 2c4e 3e4d e66c 0e9f ed65 74df de32  P.,N>M.l...et..2
-00003f70: 307a cb00 eb2d 7253 a4bd b77c 344f beb6  0z...-rS...|4O..
-00003f80: 35fe d068 fc21 d6f8 7282 ec4a aadb b5c3  5..h.!..r..J....
-00003f90: c868 8711 d60e e614 ec21 3a61 97a7 00db  .h.......!:a....
-00003fa0: 1a7f df68 fc7d acf1 cd2b 1e1d 9d70 1b76  ...h.}...+...p.v
-00003fb0: 181b ed30 c6da c19c 9a3d 4827 74f5 b452  ...0.....=H't..R
-00003fc0: 83f1 0f8c c63f c01a dfbc 48d1 d509 b760  .....?....H....`
-00003fd0: 8743 a31d 0eb1 7690 9279 604e 789f 8f4d  .C....v..y`Nx..M
-00003fe0: faf0 b9c9 133f 8e29 4dbc 2bf2 a675 66ec  .....?.)M.+..uf.
-00003ff0: 978b 5d1d 1e4f ab1b 7f30 1e8f 4e9b 7741  ..]..O...0..N.wA
-00004000: 68b6 38bc ef95 ac47 d055 7ffe cf77 7fff  h.8....G.U...w..
-00004010: f3bb 3ffc f4dd af7e f6ee 777f 412f 6999  ..?....~..w.A/i.
-00004020: 5d56 6f58 b315 dfcb 0a97 7c08 d7f8 be22  ]VoX......|...."
-00004030: 994e ad59 421e 550d 515e bf31 873e df3b  .N.YB.U.Q^.1.>.;
-00004040: 383d 38db e038 8605 2cbb 641b 690b e3eb  8=8..8..,.d.i...
-00004050: 80e4 ac72 cd16 f2a8 c616 c52a dafb b085  ...r.......*....
-00004060: 211e 56f7 dc3d cd7d 784f 863e d38d f9a1  !.V..=.}xO.>....
-00004070: acb7 36a9 ae6d c2ef aecf 9513 99dc b149  ..6..m.........I
-00004080: 9fa5 efe9 dc52 4acc 68fd 2d27 ff48 9734  .....RJ.h.-'.H.4
-00004090: be80 48ff fea1 f2fb 4ad0 0ee5 3b87 eec3  ..H.....J...;...
-000040a0: 25dd ad7a adf4 6352 6293 1b94 b2d3 29b2  %..z..cRb.....).
-000040b0: a51b 7c58 597d 07e1 21fd ccf8 f224 fd2e  ..|XY}..!....$..
-000040c0: 0f79 5463 e8f2 7d49 f7e9 67f7 12e4 64bb  .yTc..}I..g...d.
-000040d0: 6bb6 2e67 2e6e 839c 6621 a53c d3e4 dd65  k..g.n..f!.<...e
-000040e0: 0b75 e2b6 0a72 6e96 4d90 8e66 7c09 93fe  .u...rn.M..f|...
-000040f0: 1d4c e5c7 db60 9fcb f72e 3d88 80a6 5933  .L...`....=...Y3
-00004100: 2acf 3451 5e7d 7e4e a3b3 0719 d03a 880c  *.4Q^}~N.....:..
-00004110: e967 c617 48c9 98ba 6669 7954 63e8 f29d  .g..H...fiyTc...
-00004120: 510f 21a0 390f 559a e5b6 f24c 93df 562f  Q.!.9.U....L..V/
-00004130: dcd5 c8b6 63a8 dac6 e2da 8a79 930f 3575  ....c......y..5u
-00004140: befa 68b2 c697 1ea2 6831 4b1b e55f d9a7  ..h.....h1K.._..
-00004150: ff07 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-00004160: 0800 0000 2100 bdd4 8dbf 2701 0000 8f02  ....!.....'.....
-00004170: 0000 1400 0000 776f 7264 2f77 6562 5365  ......word/webSe
-00004180: 7474 696e 6773 2e78 6d6c 94d2 cd6a 0231  ttings.xml...j.1
-00004190: 1000 e07b a1ef 1072 d7ac 52a5 2cae 4229  ...{...r..R.,.B)
-000041a0: 965e 4aa1 ed03 c4ec ac86 6632 2113 bbda  .^J.......f2!...
-000041b0: a76f dc6a 7ff0 e25e 4226 c97c c984 992d  .o.j...^B&.|...-
-000041c0: 76e8 c407 44b6 e42b 391a 1652 8037 545b  v...D..+9..R.7T[
-000041d0: bfae e4db eb72 702b 0527 ed6b edc8 4325  .....rp+.'.k..C%
-000041e0: f7c0 7231 bfbe 9ab5 650b ab17 4829 9f64  ..r1....e...H).d
-000041f0: 9115 cf25 9a4a 6e52 0aa5 526c 3680 9a87  ...%.JnR..Rl6...
-00004200: 14c0 e7cd 8622 ea94 c3b8 56a8 e3fb 360c  ....."....V...6.
-00004210: 0c61 d0c9 aeac b369 afc6 4531 9547 265e  .a.....i..E1.G&^
-00004220: a250 d358 03f7 64b6 083e 75f9 2a82 cb22  .P.X..d..>u.*.."
-00004230: 79de d8c0 27ad bd44 6b29 d621 9201 e65c  y...'..Dk).!...\
-00004240: 0fba 6f0f b5f5 3fcc e8e6 0c42 6b22 3135  ..o...?....Bk"15
-00004250: 6998 8b39 bea8 a372 faa8 e866 e87e 8149  i..9...r...f.~.I
-00004260: 3f60 7c06 4c8d adfb 19d3 a3a1 72e6 1f87  ?`|.L.......r...
-00004270: a11f 3339 31bc 47d8 4981 a67c 5c7b 8a7a  ..391.G.I..|\{.z
-00004280: e5b2 94bf 46e4 ea44 071f c6c3 65f3 dc21  ....F..D....e..!
-00004290: 1492 45fb 094b 8a77 915a 86a8 0ecb da39  ..E..K.w.Z.....9
-000042a0: 6a9f 9f1e 72a0 feb5 d1fc 0b00 00ff ff03  j...r...........
-000042b0: 0050 4b03 0414 0006 0008 0000 0021 0030  .PK..........!.0
-000042c0: 0016 7419 0200 00c7 0600 0012 0000 0077  ..t............w
-000042d0: 6f72 642f 666f 6e74 5461 626c 652e 786d  ord/fontTable.xm
-000042e0: 6ce4 93df 6eda 3014 87ef 27ed 1d2c df97  l...n.0...'..,..
-000042f0: 3809 a419 6aa8 5ada 4893 a65e ac9d b45b  8...j.Z.H..^...[
-00004300: 639c c45a 6c47 b681 f208 d32e f71c db03  c..ZlG..........
-00004310: 4c9a f632 abfa 1a3d f947 51e9 34e8 c56e  L..2...=.GQ.4..n
-00004320: 0612 98df 39fe 6c7f 3127 a7b7 b244 4b6e  ....9.l.1'...DKn
-00004330: acd0 2ac1 fe80 60c4 15d3 73a1 f204 7fb8  ..*...`...s.....
-00004340: 498f 628c aca3 6a4e 4bad 7882 d7dc e2d3  I.b...jNK.x.....
-00004350: c9eb 5727 ab71 a695 b308 e62b 3b96 2cc1  ..W'.q.....+;.,.
-00004360: 8573 d5d8 f32c 2bb8 a476 a02b aea0 9869  .s...,+..v.+...i
-00004370: 23a9 839f 26f7 2435 9f16 d511 d3b2 a24e  #...&.$5.......N
-00004380: cc44 29dc da0b 0889 7087 31fb 5074 9609  .D).....p.1.Pt..
-00004390: c62f 345b 48ae 5c33 df33 bc04 a256 b610  ./4[H.\3.3...V..
-000043a0: 95ed 69ab 7d68 2b6d e695 d18c 5b0b 6796  ..i.}h+m....[.g.
-000043b0: 65cb 9354 a80d c61f ee80 a460 465b 9db9  e..T.......`F[..
-000043c0: 011c a6db 5183 82e9 3e69 46b2 7c04 8c0e  ....Q...>iF.|...
-000043d0: 0304 3b80 8889 f961 8ca8 6378 3073 8b63  ..;....a..cx0s.c
-000043e0: f961 9851 8fb1 6bc9 6f31 926c fc36 57da  .a.Q..k.o1.l.6W.
-000043f0: d059 0924 5083 e074 a801 d79f f562 93ee  .Y.$P..t.....b..
-00004400: 6ea0 d558 5109 5d77 dfbf fcfe f9b5 c969  n..XQ.]w.......i
-00004410: e9ae 2083 d292 9609 be16 f27a a1b0 5797  .. ........z..W.
-00004420: 2aaa b4e5 7e5f 22b5 c888 1012 c277 f76e  *...~_"......w.n
-00004430: 1b59 418d e535 be69 8ca3 36ce a814 e5ba  .YA..5.i..6.....
-00004440: 4fe9 c2e9 8e2b 1c2b fa78 498d a8b7 de96  O....+.+.xI.....
-00004450: acc8 a1b0 b033 02eb b5af 10b7 899f e020  .....3......... 
-00004460: 8ed3 3aea 92a0 eff1 a32e 0937 b39a 1ed6  ..:........7....
-00004470: 7386 7553 97f8 5b3d b0a6 d7aa d951 7423  s.uS..[=.....Qt#
-00004480: 24b7 e88a afd0 7b2d a96a 5ced 0a09 4048  $.....{-.j\...@H
-00004490: 4846 b0c0 08c6 2119 3e2b a45d e9a9 10d3  HF....!.>+.]....
-000044a0: 700f 3172 097b 0e2e d3f4 d1c8 1492 e378  p.1r.{.........x
-000044b0: 74fe d408 79f3 1723 e0a3 e5ec 6fe4 fedb  t...y..#....o...
-000044c0: e7fb 1fbf d03b 9117 ee0f 3afe e9fd 38ab  .....;....:...8.
-000044d0: 371c 9c6f d908 e369 7a3c 4dcf 5e74 3f5e  7..o...iz<M.^t?^
-000044e0: 64e3 b9bf d005 57f9 47b1 79b4 ff95 a46e  d.....W.G.y....n
-000044f0: 6027 0f00 0000 ffff 0300 504b 0304 1400  `'........PK....
-00004500: 0600 0800 0000 2100 e823 7037 6f01 0000  ......!..#p7o...
-00004510: e402 0000 1100 0801 646f 6350 726f 7073  ........docProps
-00004520: 2f63 6f72 652e 786d 6c20 a204 0128 a000  /core.xml ...(..
-00004530: 0100 0000 0000 0000 0000 0000 0000 0000  ................
-00004540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000045a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000045b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000045c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000045d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000045e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000045f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004630: 008c 9251 4fc2 3014 85df 4dfc 0f4b dfb7  ...QO.0...M..K..
-00004640: b64c 8d2c db48 d4f0 a489 8918 8d6f a5bd  .L.,.H.......o..
-00004650: 4061 eb9a b630 f8f7 761b 1ba2 3cf8 766f  @a...0..v...<.vo
-00004660: cfb9 dfee 4e9b 4ef6 6511 ecc0 5859 a90c  ....N.N.e...XY..
-00004670: d188 a000 14af 8454 cb0c bdcf a6e1 3d0a  .......T......=.
-00004680: ac63 4ab0 a252 90a1 0358 34c9 afaf 52ae  .cJ..R...X4...R.
-00004690: 135e 1978 3595 06e3 24d8 c093 944d b8ce  .^.x5...$....M..
-000046a0: d0ca 399d 606c f90a 4a66 23ef 505e 5c54  ..9.`l..Jf#.P^\T
-000046b0: a664 ceb7 6689 35e3 1bb6 043c 22e4 0e97  .d..f.5....<"...
-000046c0: e098 608e e106 18ea 8188 8e48 c107 a4de  ..`........H....
-000046d0: 9aa2 0508 8ea1 8012 94b3 9846 149f bc0e  ...........F....
-000046e0: 4c69 2f0e b4ca 0f67 29dd 41c3 456b 2f0e  Li/....g).A.Ek/.
-000046f0: eebd 9583 b1ae eba8 8e5b abdf 9fe2 cf97  .........[......
-00004700: e7b7 f657 43a9 9aac 38a0 3c15 3c71 d215  ...WC...8.<.<q..
-00004710: 90a7 f854 faca 6ee7 6be0 ae3b 1e1a 5f73  ...T..n.k..;.._s
-00004720: 03cc 5526 9faf f786 d056 ee8f 9ab0 3770  ..U&.....V....7p
-00004730: a82b 23ac 1f3c ebbc 4d80 e546 6ae7 afb0  .+#..<..M..Fj...
-00004740: c39e 1d78 77c1 ac7b f177 ba90 201e 0ec3  ...xw..{.w.. ...
-00004750: 17fe 2a8d d9c0 4e36 af21 8fc7 ad65 e8d3  ..*...N6.!...e..
-00004760: 63b6 dd5a 2002 9f49 d225 d82b 1ff1 e3d3  c..Z ..I.%.+....
-00004770: 6c8a f211 a1e3 908c 421a cf08 4d68 9c10  l.......B...Mh..
-00004780: f2d5 6c76 367f 0296 c70d fe49 bc4d 6e7e  ..lv6......I.Mn~
-00004790: 117b 4017 cef9 bbcc bf01 0000 ffff 0300  .{@.............
-000047a0: 504b 0304 1400 0600 0800 0000 2100 2118  PK..........!.!.
-000047b0: af59 6b01 0000 c502 0000 1000 0801 646f  .Yk...........do
-000047c0: 6350 726f 7073 2f61 7070 2e78 6d6c 20a2  cProps/app.xml .
-000047d0: 0401 28a0 0001 0000 0000 0000 0000 0000  ..(.............
-000047e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000047f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000048a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000048b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000048c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000048d0: 0000 0000 0000 9c52 4d4f c330 0cbd 23f1  .......RMO.0..#.
-000048e0: 1faa deb7 741c 2634 7941 6808 71e0 63d2  ....t.&4yAh.q.c.
-000048f0: 0a9c a3c4 6d23 d224 4ab2 89fd 7b9c 154a  ....m#.$J...{..J
-00004900: 119c c8c9 efd9 7e79 7602 57ef bd29 0e18  ......~yv.W..)..
-00004910: a276 765d 2ee6 5559 a095 4e69 dbae cbe7  .vv]..UY..Ni....
-00004920: fa76 7659 1631 09ab 8471 16d7 e511 6379  .vvY.1...q....cy
-00004930: c5cf cf60 1b9c c790 34c6 8224 6c5c 975d  ...`....4..$l\.]
-00004940: 4a7e c558 941d f622 ce29 6d29 d3b8 d08b  J~.X...".)m)....
-00004950: 4430 b4cc 358d 9678 e3e4 be47 9bd8 4555  D0..5..x...G..EU
-00004960: 2d19 be27 b40a d5cc 8f82 e5a0 b83a a4ff  -..'.........:..
-00004970: 8a2a 27b3 bff8 521f 3de9 71a8 b1f7 4624  .*'...R.=.q...F$
-00004980: e48f b9d3 cc95 4b3d b091 85da 2561 6add  ......K=....%aj.
-00004990: 23af 881e 016c 458b 912f 800d 01bc baa0  #....lE../......
-000049a0: 62ae 1902 d874 2208 9968 7f99 9c20 b8f6  b....t"..h... ..
-000049b0: de68 2912 ed95 3f68 195c 744d 2a9e 4e66  .h)...?h.\tM*.Nf
-000049c0: 8bdc 0d6c 5a02 34c0 0ee5 3ee8 74cc 5253  ...lZ.4...>.t.RS
-000049d0: 08f7 dae2 e982 2120 5741 b441 f8ee 444e  ......! WA.A..DN
-000049e0: 10ec a430 b8a1 d179 234c 4460 df04 6c5c  ...0...y#LD`..l\
-000049f0: ef85 2539 3646 a4f7 169f 7ded 6ef2 163e  ..%96F....}.n..>
-00004a00: 5b7e 9293 115f 75ea 765e c8c1 cb9f 3cec  [~..._u.v^....<.
-00004a10: 8845 45ee 4703 2301 77f4 18c1 6475 eab5  .EE.G.#.w...du..
-00004a20: 2daa af9a df89 bcbe 97e1 57f2 c572 5ed1  -.........W..r^.
-00004a30: 39ed eb8b a3a9 c7ef c23f 0000 00ff ff03  9........?......
-00004a40: 0050 4b01 022d 0014 0006 0008 0000 0021  .PK..-.........!
-00004a50: 0067 7328 2f97 0100 0028 0900 0013 0000  .gs(/....(......
-00004a60: 0000 0000 0000 0000 0000 0000 0000 005b  ...............[
-00004a70: 436f 6e74 656e 745f 5479 7065 735d 2e78  Content_Types].x
-00004a80: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-00004a90: 2100 1e91 1ab7 ef00 0000 4e02 0000 0b00  !.........N.....
-00004aa0: 0000 0000 0000 0000 0000 0000 d003 0000  ................
-00004ab0: 5f72 656c 732f 2e72 656c 7350 4b01 022d  _rels/.relsPK..-
-00004ac0: 0014 0006 0008 0000 0021 00f7 f296 563f  .........!....V?
-00004ad0: 0300 00e6 0b00 0011 0000 0000 0000 0000  ................
-00004ae0: 0000 0000 00f0 0600 0077 6f72 642f 646f  .........word/do
-00004af0: 6375 6d65 6e74 2e78 6d6c 504b 0102 2d00  cument.xmlPK..-.
-00004b00: 1400 0600 0800 0000 2100 c5aa b29b 4001  ........!.....@.
-00004b10: 0000 3d07 0000 1c00 0000 0000 0000 0000  ..=.............
-00004b20: 0000 0000 5e0a 0000 776f 7264 2f5f 7265  ....^...word/_re
-00004b30: 6c73 2f64 6f63 756d 656e 742e 786d 6c2e  ls/document.xml.
-00004b40: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
-00004b50: 0000 2100 0d28 3c0e 7e02 0000 860a 0000  ..!..(<.~.......
-00004b60: 1200 0000 0000 0000 0000 0000 0000 e00c  ................
-00004b70: 0000 776f 7264 2f66 6f6f 746e 6f74 6573  ..word/footnotes
-00004b80: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-00004b90: 0000 2100 3a68 3c1d 7c02 0000 800a 0000  ..!.:h<.|.......
-00004ba0: 1100 0000 0000 0000 0000 0000 0000 8e0f  ................
-00004bb0: 0000 776f 7264 2f65 6e64 6e6f 7465 732e  ..word/endnotes.
-00004bc0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-00004bd0: 0021 00c3 4d3e fa43 0200 0019 0900 0010  .!..M>.C........
-00004be0: 0000 0000 0000 0000 0000 0000 0039 1200  .............9..
-00004bf0: 0077 6f72 642f 6865 6164 6572 312e 786d  .word/header1.xm
-00004c00: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00004c10: 0011 0781 df43 0200 0019 0900 0010 0000  .....C..........
-00004c20: 0000 0000 0000 0000 0000 00aa 1400 0077  ...............w
-00004c30: 6f72 642f 6865 6164 6572 322e 786d 6c50  ord/header2.xmlP
-00004c40: 4b01 022d 0014 0006 0008 0000 0021 00ce  K..-.........!..
-00004c50: 9637 6d42 0200 0019 0900 0010 0000 0000  .7mB............
-00004c60: 0000 0000 0000 0000 001b 1700 0077 6f72  .............wor
-00004c70: 642f 666f 6f74 6572 312e 786d 6c50 4b01  d/footer1.xmlPK.
-00004c80: 022d 0014 0006 0008 0000 0021 0051 e447  .-.........!.Q.G
-00004c90: db42 0200 0019 0900 0010 0000 0000 0000  .B..............
-00004ca0: 0000 0000 0000 008b 1900 0077 6f72 642f  ...........word/
-00004cb0: 666f 6f74 6572 322e 786d 6c50 4b01 022d  footer2.xmlPK..-
-00004cc0: 0014 0006 0008 0000 0021 0024 5682 a244  .........!.$V..D
-00004cd0: 0200 0019 0900 0010 0000 0000 0000 0000  ................
-00004ce0: 0000 0000 00fb 1b00 0077 6f72 642f 6865  .........word/he
-00004cf0: 6164 6572 332e 786d 6c50 4b01 022d 0014  ader3.xmlPK..-..
-00004d00: 0006 0008 0000 0021 000b f966 2241 0200  .......!...f"A..
-00004d10: 0019 0900 0010 0000 0000 0000 0000 0000  ................
-00004d20: 0000 006d 1e00 0077 6f72 642f 666f 6f74  ...m...word/foot
-00004d30: 6572 332e 786d 6c50 4b01 022d 0014 0006  er3.xmlPK..-....
-00004d40: 0008 0000 0021 003a 05cc 19e1 0600 00ce  .....!.:........
-00004d50: 2000 0015 0000 0000 0000 0000 0000 0000   ...............
-00004d60: 00dc 2000 0077 6f72 642f 7468 656d 652f  .. ..word/theme/
-00004d70: 7468 656d 6531 2e78 6d6c 504b 0102 2d00  theme1.xmlPK..-.
-00004d80: 1400 0600 0800 0000 2100 f83f 6ea7 8705  ........!..?n...
-00004d90: 0000 dc0f 0000 1100 0000 0000 0000 0000  ................
-00004da0: 0000 0000 f027 0000 776f 7264 2f73 6574  .....'..word/set
-00004db0: 7469 6e67 732e 786d 6c50 4b01 022d 0014  tings.xmlPK..-..
-00004dc0: 0006 0008 0000 0021 006d 8eec aa85 1300  .......!.m......
-00004dd0: 003b c600 000f 0000 0000 0000 0000 0000  .;..............
-00004de0: 0000 00a6 2d00 0077 6f72 642f 7374 796c  ....-..word/styl
-00004df0: 6573 2e78 6d6c 504b 0102 2d00 1400 0600  es.xmlPK..-.....
-00004e00: 0800 0000 2100 bdd4 8dbf 2701 0000 8f02  ....!.....'.....
-00004e10: 0000 1400 0000 0000 0000 0000 0000 0000  ................
-00004e20: 5841 0000 776f 7264 2f77 6562 5365 7474  XA..word/webSett
-00004e30: 696e 6773 2e78 6d6c 504b 0102 2d00 1400  ings.xmlPK..-...
-00004e40: 0600 0800 0000 2100 3000 1674 1902 0000  ......!.0..t....
-00004e50: c706 0000 1200 0000 0000 0000 0000 0000  ................
-00004e60: 0000 b142 0000 776f 7264 2f66 6f6e 7454  ...B..word/fontT
-00004e70: 6162 6c65 2e78 6d6c 504b 0102 2d00 1400  able.xmlPK..-...
-00004e80: 0600 0800 0000 2100 e823 7037 6f01 0000  ......!..#p7o...
-00004e90: e402 0000 1100 0000 0000 0000 0000 0000  ................
-00004ea0: 0000 fa44 0000 646f 6350 726f 7073 2f63  ...D..docProps/c
-00004eb0: 6f72 652e 786d 6c50 4b01 022d 0014 0006  ore.xmlPK..-....
-00004ec0: 0008 0000 0021 0021 18af 596b 0100 00c5  .....!.!..Yk....
-00004ed0: 0200 0010 0000 0000 0000 0000 0000 0000  ................
-00004ee0: 00a0 4700 0064 6f63 5072 6f70 732f 6170  ..G..docProps/ap
-00004ef0: 702e 786d 6c50 4b05 0600 0000 0013 0013  p.xmlPK.........
-00004f00: 00b4 0400 0041 4a00 0000 00              .....AJ....
+00000000: 504b 0304 0a00 0000 0000 874e e240 0000  PK.........N.@..
+00000010: 0000 0000 0000 0000 0000 0900 0000 646f  ..............do
+00000020: 6350 726f 7073 2f50 4b03 0414 0000 0008  cProps/PK.......
+00000030: 0087 4ee2 404d d85f e75e 0100 0072 0200  ..N.@M._.^...r..
+00000040: 0010 0000 0064 6f63 5072 6f70 732f 6170  .....docProps/ap
+00000050: 702e 786d 6c9d 91cd 6e83 3010 84ef 95fa  p.xml...n.0.....
+00000060: 0e88 3b18 c86f 23c7 514a 9a53 d546 8234  ..;..o#.QJ.S.F.4
+00000070: c7c8 321b b00a b665 3b51 f2f6 35a1 22f4  ..2....e;Q..5.".
+00000080: dadb ceac 3cfe b483 57d7 a6f6 2ea0 0d97  ....<...W.......
+00000090: 62e9 c761 e47b 2098 2cb8 2897 fe3e df06  b..a.{ .,.(..>..
+000000a0: 73df 3396 8a82 d652 c0d2 bf81 f157 e4f9  s.3....R.....W..
+000000b0: 09ef b454 a02d 07e3 b908 6196 7e65 ad5a  ...T.-....a.~e.Z
+000000c0: 2064 5805 0d35 a15b 0bb7 3949 dd50 eba4   dX..5.[..9I.P..
+000000d0: 2e91 3c9d 3883 8d64 e706 8445 4914 4d11  ..<.8..d...EI.M.
+000000e0: 5c2d 8802 8a40 f581 7e97 b8b8 d8ff 8616  \-...@..~.......
+000000f0: 92b5 7ce6 2bbf 2907 4c70 0e8d aaa9 05f2  ..|.+.).Lp......
+00000100: d1e2 d461 216d 8351 efe2 1d2d c190 18a3  ...a!m.Q...-....
+00000110: 6ec0 07a9 0b43 228c ba01 a715 d594 5977  n....C".......Yw
+00000120: a7d6 1c28 fcce 857b e9cc 6e70 499a 969a  ...(...{..npI...
+00000130: aaea 6e0e 14ce a5a5 75ce 1b20 7132 769f  ..n.....u.. q2v.
+00000140: f712 678c d690 3a60 72a2 b501 8c1e 469b  ..g...:`r.....F.
+00000150: ff6d f62a 979b 16ff 77ff d71c d01d b8ad  .m.*....w.......
+00000160: 3245 5987 f4e0 1cf8 78ad 54cd 19b5 ae71  2EY.....x.T....q
+00000170: 72d8 65de e7bd 9563 1c87 aefe 703e 4b92  r.e....c....p>K.
+00000180: e336 7e1b 25b3 d734 48a6 2f69 301e 4d8a  .6~.%..4H./i0.M.
+00000190: 601d 4f92 209a a493 7134 8fa2 245d 6334  `.O. ...q4..$]c4
+000001a0: 0cc2 aed5 0cd8 5973 7b6b af31 94ee aa7d  ......Ys{k.1...}
+000001b0: b7e4 0750 4b03 0414 0000 0008 0087 4ee2  ...PK.........N.
+000001c0: 4013 fa0c 9254 0100 007e 0200 0011 0000  @....T...~......
+000001d0: 0064 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
+000001e0: 6d6c 7d92 514f 8330 1485 df4d fc0f a4ef  ml}.QO.0...M....
+000001f0: d016 8c71 0db0 44cd 9e5c 6222 46e3 5b6d  ...q..D..\b"F.[m
+00000200: ef18 0aa5 69bb 31fe bd85 319c d1f8 787b  ....i.1...1...x{
+00000210: cefd eeb9 6dd3 e5a1 a983 3d18 5bb5 2a43  ....m.....=.[.*C
+00000220: 3422 2800 255a 59a9 3243 cfc5 2abc 4181  4"(.%ZY.2C..*.A.
+00000230: 755c 495e b70a 32d4 8345 cbfc f222 159a  u\I^..2..E..."..
+00000240: 89d6 c0a3 6935 1857 810d 3c49 5926 7486  ....i5.W..<IY&t.
+00000250: b6ce 6986 b115 5b68 b88d bc43 7971 d39a  ..i...[h...Cyq..
+00000260: 863b 5f9a 126b 2e3e 7909 3826 e41a 37e0  .;_..k.>y.8&..7.
+00000270: b8e4 8ee3 0118 ea99 8826 a414 3352 ef4c  .........&..3R.L
+00000280: 3d02 a4c0 5043 03ca 594c 238a bfbd 0e4c  =...PC..YL#....L
+00000290: 63ff 6c18 9533 6753 b95e fb9d a6b8 e76c  c.l..3gS.^.....l
+000002a0: 298e e2ec 3ed8 6a36 765d 1775 c918 c3e7  )...>.j6v].u....
+000002b0: a7f8 75fd f034 ae1a 566a b82b 0128 4fa5  ..u..4..Vj.+.(O.
+000002c0: 18c7 3161 803b 9081 07b0 e3b8 93f2 92dc  ..1a.;..........
+000002d0: dd17 2b94 c784 2e42 1287 3429 c882 d184  ..+....B..4)....
+000002e0: 11f2 96e2 936b ea1f 8047 566b f2f7 8f83  .....k...GVk....
+000002f0: 2174 f0cc 47c3 7bd4 dcba b57f ba4d 05f2  !t..G.{......M..
+00000300: b6cf cb5d db73 b501 55a6 f8b7 3a07 6ca6  ...].s..U...:.l.
+00000310: 8e7f 13c6 7148 9290 c605 218c 5cb1 e43c  ....qH....!.\..<
+00000320: e109 900f 190c ecab e12f e5c9 629c 3ad7  ........./..b.:.
+00000330: 63f5 f3c7 e45f 504b 0304 1400 0000 0800  c...._PK........
+00000340: 874e e240 7c52 f707 fe00 0000 7f01 0000  .N.@|R..........
+00000350: 1300 0000 646f 6350 726f 7073 2f63 7573  ....docProps/cus
+00000360: 746f 6d2e 786d 6c9d 90cd 6a84 3018 45f7  tom.xml...j.0.E.
+00000370: 85be 43c8 3e26 a6d8 1925 3a54 9dd9 74d1  ..C.>&...%:T..t.
+00000380: 42a7 b397 1867 02e6 8724 da4a e9bb 3732  B....g...$.J..72
+00000390: fdd9 77f9 713f 0ee7 5eb6 7b57 2398 85f3  ..w.q?..^.{W#...
+000003a0: d2e8 12a6 0981 4068 6e7a a9cf 257c 3d1e  ......@hnz..%|=.
+000003b0: d016 021f 3add 77a3 d1a2 848b f070 57dd  ....:.w......pW.
+000003c0: deb0 6767 ac70 410a 0f22 42fb 125e 42b0  ..gg.pA.."B..^B.
+000003d0: 05c6 9e5f 84ea 7c12 631d 93c1 38d5 8578  ..._..|.c...8..x
+000003e0: ba33 36c3 20b9 680d 9f94 d001 5342 ee31  .36. .h.....SB.1
+000003f0: 9f7c 300a d95f 1cbc f28a 39fc 17d9 1bbe  .|0.._....9.....
+00000400: daf9 d371 b151 b762 dff0 050c 2ac8 be84  ...q.Q.b....*...
+00000410: 1f6d d6b4 6d46 3244 f779 8352 92d6 28bf  .m..mF2D.y.R..(.
+00000420: cb37 886c 09a1 356d 0ef9 c3fe 1302 bb3e  .7.l..5m.......>
+00000430: 5308 74a7 62f5 c797 a788 ed27 1eea 498e  S.t.b......'..I.
+00000440: fd49 b888 9e43 31da 371f 5c45 4946 519a  .I...C1.7.\EIFQ.
+00000450: 2671 c364 bba1 94e1 bf8c e11f 858a e1d5  &q.d............
+00000460: edba 5cf5 0550 4b03 040a 0000 0000 0087  ..\..PK.........
+00000470: 4ee2 4000 0000 0000 0000 0000 0000 0005  N.@.............
+00000480: 0000 0077 6f72 642f 504b 0304 1400 0000  ...word/PK......
+00000490: 0800 874e e240 ae64 84bf 4a14 0000 39a8  ...N.@.d..J...9.
+000004a0: 0000 0f00 0000 776f 7264 2f73 7479 6c65  ......word/style
+000004b0: 732e 786d 6ced 5d4f 6f1c c975 bf07 c877  s.xml.]Oo..u...w
+000004c0: 18cc 2939 70a9 99a1 4489 58ae 2151 62b4  ..)9p...D.X.!Qb.
+000004d0: 0825 2b26 b53e f7cc 34c9 5ef5 744f ba7b  .%+&.>..4.^.tO.{
+000004e0: 4451 e720 86e1 5360 2009 021f e21c 821c  DQ. ..S` .......
+000004f0: 9c5c 821c 82c0 dfc6 96b3 df22 af5e bdea  .\.........".^..
+00000500: aeee eaaa ae7a 4352 6260 fba0 9de6 bc7a  .....zCRb`.....z
+00000510: 55ef cfef fda9 ea9a af7f f461 958e dec7  U..........a....
+00000520: 4599 e4d9 e178 f2d5 83f1 28ce 16f9 32c9  E....x....(...2.
+00000530: 2e0e c76f cf8e 771e 8f47 6515 65cb 28cd  ...o..w..Ge.e.(.
+00000540: b3f8 707c 1d97 e31f 7df3 a77f f2f5 d541  ..p|....}......A
+00000550: 595d a771 3982 01b2 f260 b538 1c5f 56d5  Y].q9....`.8._V.
+00000560: fa60 77b7 5c5c c6ab a8fc 2a5f c719 fcf1  .`w.\\....*_....
+00000570: 3c2f 5651 051f 8b8b dd55 54bc dbac 7716  </VQ.....UT...w.
+00000580: f96a 1d55 c93c 4993 ea7a 77fa e0c1 a331  .j.U.<I..zw....1
+00000590: 0d93 1f8e 3745 7640 43ec ac92 4591 97f9  ....7Ev@C...E...
+000005a0: 7925 480e f2f3 f364 11d3 3f8a a2f0 e12b  y%H....d..?....+
+000005b0: 299f e78b cd2a ce2a e4b8 5bc4 29cc 21cf  )....*.*..[.).!.
+000005c0: cacb 645d aad1 56dc d160 8997 6a90 f7ae  ..d]..V..`..j...
+000005d0: 45bc 5fa5 ea7b 573e ccae f262 b92e f245  E._..{W>...b...E
+000005e0: 5c96 a093 552a 27bf 8a92 ac1e 66b2 670c  \...U*'.....f.g.
+000005f0: 540b ee2b 10dc ae5c feae 180a c827 0ff0  T..+...\.....'..
+00000600: bfb4 794c 1eb8 664c 6217 d48a 6599 1a1c  ..yL..fLb...e...
+00000610: 7bb4 2db5 7892 cc8b a890 6a06 0310 f35e  {.-.x.....j....^
+00000620: 2d0e bebd c8f2 229a a760 5257 93bd f137  -....."..`RW...7
+00000630: 604f cb7c f13c 3e8f 3669 558a 8fc5 9b82  `O.|.<>.6iU.....
+00000640: 3ed2 27fc e738 cfaa 7274 7510 958b 2439  >.'..8..rtu...$9
+00000650: 1cff fe3f 7ef1 bbdf fe72 0c0f 2e9f 6665  ...?~....r....fe
+00000660: eb41 1c95 d5d3 3289 f42f 2dca 0a6c 1378  .A....2../-..l.x
+00000670: ae12 60ff 2c59 26e3 dd6f bede 4566 eadf  ..`.,Y&..o..Ef..
+00000680: 9a29 3cee 4c09 0c06 cce7 54da fdd5 c122  .)<.L.....T...."
+00000690: df64 d5e1 78fa 089c 06be 1b9f ffd5 31da  .d..x.........1.
+000006a0: fae1 583d 789b 5d26 cbf8 a797 71f6 b68c  ..X=x.]&....q...
+000006b0: 97e0 5ff4 c5d3 7895 bc4c 96cb 58f8 1c3d  .._...x..L..X..=
+000006c0: 7bfb ed9b 22c9 0bf0 88c3 f193 27f4 f024  {...".......'..$
+000006d0: 5fbc 8b97 a715 3016 a30a 11a4 e5f2 c587  _.....0.........
+000006e0: 45bc 16b6 0b6c ff5a f1c4 7136 1d86 3891  E....l.Z..q6..8.
+000006f0: 4dd2 8c8c 0f4a 8d3d 3ec8 2221 94d7 62f6  M....J.=>."!..b.
+00000700: a990 c8b6 5c70 fa16 2e97 7124 d065 34f1  ....\p....q$.e4.
+00000710: 61a4 cddc 67cc e92d 8c39 bb85 31f7 6e61  a...g..-.9..1.na
+00000720: cc87 b730 e6a3 5b18 73ff 16c6 7ccc 1953  ...0..[.s...|..S
+00000730: 1abd 32c7 27bd 43e8 ae23 9d52 5225 d932  ..2.'.C..#.RR%.2
+00000740: fe60 3161 374d bf89 ba69 fa4d d04d d36f  .`1a7M...i.M.M.o
+00000750: 626e 9a7e 1372 d3f4 9b88 4963 4103 29c8  bn.~.r....IcA.).
+00000760: 7e9b 3007 d185 dfaf 7337 cdb0 9267 0833  ~.0.....s7...g.3
+00000770: 924f 952f 3c54 dca5 1856 7097 6258 bd5d  .O./<T...Vp.bX.]
+00000780: 8a61 e576 2986 55db a518 566c 9762 588b  .a.v).U...Vl.bX.
+00000790: 5d8a 611d 7629 8635 a8bb a98c 68a3 6fc1  ].a.v).5....h.o.
+000007a0: 5bb3 2ac8 c1cf f3bc caf2 2a1e 55f1 8730  [.*.......*.U..0
+000007b0: ca28 033a cc2c edb4 9da0 ad47 b9a1 3017  .(.:.,.....G..0.
+000007c0: 17bd eb60 8e28 9669 19d1 ed49 049b 8173  ...`.(.i...I...s
+000007d0: 993d 1479 8df4 ae45 8429 4cef 0836 de95  .=.y...E.)L..6..
+000007e0: c818 47f9 f9e8 3cb9 d814 508a f4e5 2a36  ..G...<...P...*6
+000007f0: e238 7b1f a790 a68e a2e5 1268 99c4 455c  .8{........h..E\
+00000800: 4185 12c4 b8b6 a522 3e8f 0b28 afe2 2072  A......">..(.. r
+00000810: cda0 7803 a449 168f b2cd 6a1e a8e9 7574  ..x..I....j...ut
+00000820: c1a2 8bb3 25ba 0e6f b68a 3ad8 f16a e388  ....%..o..:..j..
+00000830: 36d5 a548 a493 4003 5945 506d 06a9 a6ca  6..H..@.YEPm....
+00000840: a391 cb13 6ca6 7892 9461 a022 0846 cf36  ....l.x..a.".F.6
+00000850: 691a 33e8 5e87 ab1e f90d 4732 1d6b 9164  i.3.^.....G2.k.d
+00000860: 3894 1924 7b41 1247 2ec3 c1cc e022 6537  8..${A.G....."e7
+00000870: 622c 8928 192b 234a c602 8992 b14e a96b  b,.(.+#J.....N.k
+00000880: ce3a 8992 b14e a264 ac93 28fb d7d9 0969  .:...N.d..(....i
+00000890: 4395 edc4 55da 9e25 551a 86ba 4769 2e1a  C...U..%U...Gi..
+000008a0: 2e41 c679 9a5c 6411 8487 7e4e 9df5 6841  .A.y.\d...~N..hA
+000008b0: 1f4b 774b 824c ed88 d19b a888 2e8a 687d  .KwK.L........h}
+000008c0: 3912 2d90 a069 3dcb 97d7 a3b3 d03c a6a6  9.-..i=......<..
+000008d0: e2a4 4fe8 a647 30d1 24db f44b c305 8d23  ..O..G0.$..K...#
+000008e0: 45c9 b1e3 9a96 61c9 352d c396 6bda 7e6b  E.....a.5-..k.~k
+000008f0: b6ad f715 6422 22ce be84 b688 253e 770c  ....d"".....%>w.
+00000900: 67d0 115c e674 ba99 57c1 be70 1aa5 1b99  g..\.t..W..p....
+00000910: d206 d9dd 73e8 5a05 1134 2677 9c14 10f0  ....s.Z..4&w....
+00000920: 1879 7bff 1081 76f4 5a24 fe42 21a1 00d0  .y{...v.Z$.B!...
+00000930: 700f 0b34 0d5d 98d1 3674 5254 81eb 34c8  p..4.]..6tRT..4.
+00000940: 03b9 a7d0 9d0c 0796 97d7 ebb8 809c f45d  ...............]
+00000950: 906d 1ce7 699a 5fc5 4b37 75a0 ab4c a7a2  .m..i._.K7u..L..
+00000960: 1eb1 20ef 6955 e496 0010 cac6 159a 5eac  .. .iU........^.
+00000970: d697 5199 9441 d250 5b19 a357 d13a 88f0  ..Q..A.P[..W.:..
+00000980: 4d0a 1df8 709d bdd8 81ce 7d3a 7207 381b  M...p.....}:r.8.
+00000990: c451 15fe 673f 8de7 7f1e 34d9 9767 af4e  .Q..g?....4..g.N
+000009a0: 464f 2129 cfae 570c 4246 9987 1c8f 9240  FO!)..W.BF.....@
+000009b0: dc92 54f9 320c ed90 0ac2 7b92 41a9 9287  ..T.2.....{.A...
+000009c0: 9594 48fb 97f1 f53c 8f60 5726 a40a 46ca  ..H....<.`W&..F.
+000009d0: 3750 9ae1 5645 1533 a84f a3d5 3a30 9b42  7P..VE.3.O..:0.B
+000009e0: ae67 e0f8 5750 9759 c29c cd7c 90f6 bba8  .g..WP.Y...|....
+000009f0: 4844 f1df bbd6 8e3b 6a99 955e 0790 199e  HD.....;j..^....
+00000a00: 5987 b14d 402b c0cb cdfc fb78 1196 7e21  Y..M@+.....x..~!
+00000a10: 4370 1d21 348f 7ea2 3ee5 1669 5848 6991  Cp.!4.~.>..iXHi.
+00000a20: 86e1 ba24 3d4a 23d8 72f4 e980 9a33 56b4  ...$=J#.r....3V.
+00000a30: 9c29 2bda 6de6 1c96 bed1 7af3 342f ce37  .)+.m.....z.4/.7
+00000a40: 294b 4547 8a98 b562 45cc 5a72 9e6e 5659  )KEG...bE.Zr.nVY
+00000a50: c99d 35d2 3227 8db4 dbcc 99a9 26e4 1b96  ..5.2'......&...
+00000a60: 654b 15ff 4591 2c59 8242 428e 9490 9023  eK..E.,Y.BB....#
+00000a70: 2224 e4c8 0709 d9c2 196e fa9b ce8e 1c87  "$.......n......
+00000a80: 7bff 16c2 e12d 0093 10ab cbfe fd63 1b86  {....-.......c..
+00000a90: 4b03 4042 8e1e 9190 a347 24e4 e811 0939  K.@B.....G$....9
+00000aa0: 7a44 428e 1e91 90a3 4724 e4e8 71f6 7c14  zDB.....G$..q.|.
+00000ab0: 9f9f 433c e5c1 9746 ced1 a946 ced1 aca8  ..C<...F...F....
+00000ac0: f7e3 d51a 4eb1 14d7 bd59 89db 145f a4f1  ....N....Y..._..
+00000ad0: 4514 d8c8 9146 fca6 c8cf c569 a03c b31c  E....F.....i.<..
+00000ae0: d670 3316 1d00 6e22 2249 39c2 86dc 9f85  .p3...n""I9.....
+00000af0: bc82 8ecb af5f ab7e c9e2 b308 ca4d 3860  ....._.~.....M8`
+00000b00: 636d 9b75 8619 6aca c87d 4c4b a5d9 4427  cm.u..j..}LK..D'
+00000b10: 8621 9d89 134d fd74 4393 9207 972c 933a  .!...M.tC....,.:
+00000b20: 492e 2eab d1e9 a5a3 0b32 38be ab13 25c7  I........28...%.
+00000b30: 17d8 c19c bcab 7697 838b c8c4 1c7c e668  ......v......|.h
+00000b40: 0cbc 8a97 c966 a544 6333 eb41 e1ec f9b3  .....f.Dc3.A....
+00000b50: b078 c020 0bdc 6eb5 e897 5681 e06d 89a5  .x. ..n...V..m..
+00000b60: 83e3 c3b9 4d6b fb44 1f9f 3bff fde1 f131  ....Mk.D..;....1
+00000b70: fbe0 ce1f 0eb7 0ecd 1fc7 e7ce dfb5 994f  ...............O
+00000b80: f2c1 f1fb 916a f030 dfbe abaf f41c ceda  .....j.0........
+00000b90: 8ef8 eeb5 eff2 ddba dcd9 0a1e f65d 1e5c  .............].\
+00000ba0: b3d8 6209 2e27 aec7 df02 245c e26f c127  ..b..'....$\.o.'
+00000bb0: 34b1 1670 0285 0d15 2e5d 3438 ba2d 1797  4..p.....]48.-..
+00000bc0: 3a1a 40dd 968b 4b29 5d64 dd96 5708 c46e  :.@...K)]d..W..n
+00000bd0: cbcb 1b6b b765 e40d badb 32f2 46df 6d19  ...k.e....2.F.m.
+00000be0: 79c3 f0b6 8cbc f178 4b46 7ec0 bc2d 1317  y......xKF~..-..
+00000bf0: 2ad4 f046 08bd 2d2f 1736 d4bc 3097 d80e  *..F..-/.6..0...
+00000c00: eaf6 5df0 5033 c2a0 b91d 23ff dc57 898e  ..].P3....#..W..
+00000c10: 9b04 b8d4 6482 3797 8b4b 4126 7873 b9b8  ....d.7..KA&xs..
+00000c20: b463 036f 2e2f 0e78 7379 0583 3797 5130  .c.o./.xsy..7.Q0
+00000c30: 7873 1905 8337 9751 3078 7319 0583 3793  xs...7.Q0xs...7.
+00000c40: 5118 7873 99b8 50a1 c6b9 0e78 7379 b9b0  Q.xs..P....xsy..
+00000c50: a1e6 a583 3797 910b 1e6a 463a 7833 1985  ....7....jF:x3..
+00000c60: 8337 b3c2 7ae4 5293 09de 5c2e 2e05 99e0  .7..z.R...\.....
+00000c70: cde5 e2d2 8e0d bcb9 bc38 e0cd e515 0cde  .........8......
+00000c80: 5c46 c1e0 cd65 140c de5c 46c1 e0cd 6514  \F...e...\F...e.
+00000c90: 0cde 4c46 61e0 cd65 e242 851a e73a e0cd  ..LFa..e.B...:..
+00000ca0: e5e5 c286 9a97 0ede 5c46 2e78 a819 e9e0  ........\F.x....
+00000cb0: cd64 140e de96 fdb3 c1f6 a44b 4d26 7873  .d.........KM&xs
+00000cc0: b9b8 1464 8237 978b 4b3b 36f0 e6f2 e280  ...d.7..K;6.....
+00000cd0: 3797 5730 7873 1905 8337 9751 3078 7319  7.W0xs...7.Q0xs.
+00000ce0: 0583 3797 5130 7833 1985 8137 9789 0b15  ..7.Q0x3...7....
+00000cf0: 6a9c eb80 3797 970b 1b6a 5e3a 7873 19b9  j...7....j^:xs..
+00000d00: e0a1 66a4 8337 9351 3878 5bce 30dc 3078  ..f..7.Q8x[.0.0x
+00000d10: 73b9 b814 6482 3797 8b4b 3b36 f0e6 f2e2  s...d.7..K;6....
+00000d20: 8037 9757 3078 7319 0583 3797 5130 7873  .7.W0xs...7.Q0xs
+00000d30: 1905 8337 9751 3078 3319 8581 3797 0907  ...7.Q0x3...7...
+00000d40: bcb9 bc5c d850 63aa 0ede 5c46 2e78 a819  ...\.Pc...\F.x..
+00000d50: e9e0 cd64 140e de96 7364 370c de5c 2e2e  ...d....sd7..\..
+00000d60: 0599 e0cd e5e2 d28e 0dbc b9bc 38e0 cde5  ............8...
+00000d70: 150c de5c 46c1 e0cd 6514 0cde 5c46 c1e0  ...\F...e...\F..
+00000d80: cd65 140c de4c 4661 e0cd 65c2 016f 2e2f  .e...LFa..e..o./
+00000d90: 1736 d498 aa83 3797 910b 1e6a 463a 7823  .6....7....jF:x#
+00000da0: 23b8 5c4c bf4d 4c5c b985 f7e9 c179 a40a  #.\L.ML\.....y..
+00000db0: 5e93 391c afd5 fbbe e288 12dc 2d26 ee45  ^.9.........-&.E
+00000dc0: a3cb c2f0 8bdf e275 6282 4e5c a701 df79  .......ub.N\...y
+00000dd0: 1fc1 a56c fa15 5e74 4211 5f0e 6a8e 84aa  ...l..^tB._.j...
+00000de0: 6f3e 9007 e3d6 6f0a e4bd 8e16 e252 aeab  o>....o......R..
+00000df0: 83b9 7833 08f8 3fc4 c32d f2d3 095c 2051  ..x3..?..-...\ Q
+00000e00: aa47 d139 bcc0 d3fa d0fc 1978 c1c2 684c  .G.9.......x..hL
+00000e10: b8c0 4d0c 5ddc c695 6d57 07ef e242 5c7f  ..M.]...mW...B\.
+00000e20: 86ab a65d 84f2 a37a 30ab 9f1c 89cb e2e4  ...]...z0.......
+00000e30: 97d4 21b1 08d7 89cf e26c e7ed a910 7073  ..!......l....ps
+00000e40: 59dc c7cb 9da3 d7e2 d11c 6e87 3b1c 47c5  Y.........n.;.G.
+00000e50: cee9 5321 2aed 9238 94ff 80c6 6a1d 4df1  ..S!*..8....j.M.
+00000e60: d236 5d47 7461 843a 0c34 8fe0 6ab8 1fd7  .6]Gta.:.4..j...
+00000e70: 6ba1 5966 f0ba b69a b99a 38bc 32a9 1e4d  k.Yf......8.2..M
+00000e80: e9b8 b55b c774 590e e9e3 5d1c af5f c3b0  ...[.tY...].._..
+00000e90: 6810 e203 ea0d 3f95 86fa 677b a87f 52f6  h.....?...g{..R.
+00000ea0: 6c86 9fe0 a54d 6119 fb08 7fe2 c34f 36e2  l....Ma......O6.
+00000eb0: 023f b86f 83ae cdc8 3795 787c f23e 5513  .?.o....7.x|.>U.
+00000ec0: 4533 336c 628e 5ce7 4725 cda5 51e5 1ed5  E33lb.\.G%..Q...
+00000ed0: a58d 2e9b 278d 2ee5 33ae 4a66 5695 90d9  ....'...3.JfV...
+00000ee0: b054 0222 c2d5 b44f ede1 a35b d312 5d3d  .T."...O...[..]=
+00000ef0: 485a a24f 524b 7b13 0cbb 7e5a 420b 33b4  HZ.ORK{...~ZB.3.
+00000f00: d4f6 5c3c 670c 3727 46df e7c5 4b71 d9a2  ..\<g.7'F...Kq..
+00000f10: 7012 bc75 b1f7 2fca a3f4 3fbe a02b 1905  p..u../...?..+..
+00000f20: 6573 15a3 1850 5dc5 086e d732 8dc6 0cfa  es...P]..n.2....
+00000f30: 5c5a 3ee3 9a81 bc75 b2cf 33a9 b1cd 3303  \Z>....u..3...3.
+00000f40: f2d6 fb68 0668 fe86 19dc 9d46 1e5a 1d93  ...h.h.....F.Z..
+00000f50: 5081 a711 f2ea 3bd5 c863 1d3e a74f 34f8  P.....;..c.>.O4.
+00000f60: 9ced 0738 265a a2a1 912f ca31 5528 2a3f  ...8&Z.../.1U(*?
+00000f70: 36f8 2c9f 711d f391 d50c a8ee e599 0179  6.,.q..........y
+00000f80: f57d 3403 347f c30c 6c8e 79f3 1ad9 b76a  .}4.4...l.y....j
+00000f90: 84b2 669e 46c8 abef 5423 adbc e611 d6db  ..f.F...T#......
+00000fa0: 3260 cea6 b593 0ea7 3568 8886 42be 2cbf  2`......5h..B.,.
+00000fb0: ac33 29cd 2f95 2161 6e0e f30f 4a65 1f5b  .3)./.!an...Je.[
+00000fc0: ad80 de1a e459 0139 f53d b402 55c9 b50b  .....Y.9.=..U...
+00000fd0: 1eab 5bde b842 9e58 1542 e501 4f21 e4d3  ..[..B.X.B..O!..
+00000fe0: f750 2168 875f 865b 3699 eb74 0bbd 2f2e  .P!h._.[6..t../.
+00000ff0: a10d b010 3766 40ca 6ceb 0298 f1d2 7569  ....7f@.l.....ui
+00001000: 58b0 5a29 a1bd 8172 1e53 fb46 30be e97b  X.Z)...r.S.F0..{
+00001010: 8537 7638 0460 66f2 e65d 1fcd 5b70 cc2a  .7v8.`f..]..[p.*
+00001020: 8d8a e96a 9eca be06 fcc7 4974 0d15 2f4c  ...j......It../L
+00001030: 4cb6 6cce 930f ea3a 15f8 e351 9ca6 afa2  L.l....:...Q....
+00001040: 42f4 09aa 7c0d 5f82 ebfe 31c2 c82f 2f3f  B...|._...1..//?
+00001050: 4463 9c49 1a9f 8b21 e0af 9307 5858 77fe  Dc.I...!....XXw.
+00001060: 3ecf ab2a 5fd9 e90b 7c4f d33a 0078 833e  >..*_...|O.:.x.>
+00001070: 19f9 51ac 2014 fde1 7e3d b116 bd5e 325f  ..Q. ...~=...^2_
+00001080: 92ed 071c 08b0 75e7 6246 b1e2 a6f4 616d  ......u.bF....am
+00001090: 60e9 0978 7f17 a2b1 c409 e1a5 9ec3 ca67  `..x...........g
+000010a0: 2025 56ac 9c4c 0c69 e977 ed0e cb09 aea6   %V..L.i.w......
+000010b0: dace 5049 30e0 3cf8 730a f02f d810 76bd  ..PI0.<.s../..v.
+000010c0: c4ab 6812 51d6 39b4 f5f6 260f 2935 d6be  ..h.Q.9...&.)5..
+000010d0: 8356 2540 07bf f278 063f d101 d311 d643  .V%@...x.?.....C
+000010e0: e395 59b4 3ecb b1af 49c3 7e06 21f7 37d7  ..Y.>...I.~.!.7.
+000010f0: d4fd 421e 4266 17eb edd6 dafa d912 1dbd  ..B.Bf..........
+00001100: f655 94b3 b83f 126e 2c02 212e c40d 2fd4  .U...?.n,.!.../.
+00001110: 2883 8fe5 c7c3 b1dc 1481 be1b 34d0 7016  (...........4.p.
+00001120: 205b 358c 92b1 a68f dbd4 d9d5 c1f7 8b8e   [5.............
+00001130: 6d48 5db7 f39a 5b75 17b3 27d7 ba19 be5f  mH]...[u..'...._
+00001140: 953d 4dd2 9ee8 66f6 bee1 4611 f42d 5a1f  .=M...f...F..-Z.
+00001150: 7082 e50b 1c06 55c0 afd1 088d 894f 4710  p.....U......OG.
+00001160: 7cc1 3ff0 9126 103b 7082 bea4 beeb eeef  |.?..&.;p.......
+00001170: c46c 699c 892f 8d84 e3c8 4974 9746 d982  .li../....It.F..
+00001180: bb67 08d7 09e8 2b30 fbb7 0ef4 d323 d833  .g....+0.....#.3
+00001190: f851 17f8 f19f 2648 0d1b aedc a294 864b  .Q....&H.......K
+000011a0: 2d4f 0a61 2cda 0097 e9e1 ac82 1f8b 7502  -O.a,.........u.
+000011b0: 4dcc 65fc 5299 bed3 5d7b 784b f2ef 78e4  M.e.R...]{xK..x.
+000011c0: 0249 e7a9 2e7e 7b3a 21bf eb8e d9b5 e92d  .I...~{:!......-
+000011d0: 3625 a40b a7e2 376a 04b0 c0ec 1a63 34cb  6%....7j.....c4.
+000011e0: 78dc 0093 16b9 0fb7 aed2 0d58 f466 9da5  x..........X.f..
+000011f0: b6f7 32d0 8714 be8c f04c bdea fe60 8138  ..2......L...`.8
+00001200: a904 fa70 eff1 545e 185f 892b 2e70 7680  ...p..T^._.+.pv.
+00001210: a1f8 2635 a227 3e16 07f5 60a5 cf8e 293e  ..&5.'>...`...)>
+00001220: 519a 0ac2 4519 bc29 6038 959e c19d a23f  Q...E..)`8.....?
+00001230: c9af 3030 f766 b37a affa 165b dc09 ba6e  ..00.f.z...[...n
+00001240: 42bb 1f0d ac4e 558c 556b 5850 a6b9 d0ec  B....NU.UkXP....
+00001250: 64c0 5ff6 1f3c 7dbe 87fb e016 a189 d863  d._..<}........c
+00001260: 18b3 b030 9d49 7929 1011 9d6a 91c6 1156  ...0.Iy)...j...V
+00001270: 1f9d 1876 9ea4 b0df 788c ff13 5686 ec8e  ...v....x...V...
+00001280: f1e1 3c5a bcbb 28e0 c791 962a b055 b812  ..<Z..(....*.U..
+00001290: 69c7 a416 841c 5349 70e9 dcfd d791 ccf7  i.....SIp.......
+000012a0: fb31 e9be 2be8 5cdc cc0b be88 5e44 dedd  .1..+.\.....^D..
+000012b0: a40f 326d d482 25a5 cfdd 6de0 fbe0 69ee  ..2m..%...m...i.
+000012c0: d872 dff5 281c 4da9 f1de 82a1 33f1 b8ef  .r..(.M.....3...
+000012d0: 1a9a c3af 2e4e be8b 8b0a 5d4d 4228 4473  .....N....]MB(Ds
+000012e0: 5f68 7e31 7d71 fc1c cf0f 69d0 dc8d 9e02  _h~1}q....i.....
+000012f0: b0cf 12f1 2b76 33b5 d5e4 8fd5 38c1 9779  ....+v3.....8..y
+00001300: f1f1 4b9d 6016 8b26 4c6b 76ad 30a7 9b4f  ..K.`..&Lkv.0..O
+00001310: 96e0 2fdf b523 217e a2c4 abc9 282c a12b  ../..#!~....(,.+
+00001320: bb72 736b e1c9 f6ec ca3b 5d5c 796b 8b03  .rsk.....;]\yk..
+00001330: 1963 862a a48a ff51 276c 5e39 adb9 29a1  .c.*...Q'l^9..).
+00001340: e5b4 8f6e 36a7 a56e 8133 a71d 2aa6 87ab  ...n6..n.3..*...
+00001350: af65 bea1 32b2 9372 f5a6 6e70 6242 3508  .e..2..r..npbB5.
+00001360: 31e1 08a3 9629 9996 5ec2 f46c 5d4d f95d  1....)..^..l]M.]
+00001370: 9592 ca7f df3f 4de1 372f ea5c 5136 9664  .....?M.7/.\Q6.d
+00001380: f857 80d5 f84d ad58 cc21 3a99 f81c 9362  .W...M.X.!:....b
+00001390: 7924 0838 7de6 1458 ac75 9b9c 3560 355a  y$.8}..X.u..5`5Z
+000013a0: b268 e8ee 2642 58d0 525a d91d e9a0 6f2d  .h..&BX.RZ....o-
+000013b0: d216 8653 f94e 86c1 1dea 8fa1 100a 60df  ...S.N........`.
+000013c0: 580d bad9 0650 cd4d c508 2e1a bd86 5f28  X....P.M......_(
+000013d0: d859 4655 3496 7eda 39b4 e8d5 13e8 b4dd  .YFU4.~.9.......
+000013e0: 2c4d abd6 91d3 761b 0b00 04db 0727 f23c  ,M....v......'.<
+000013f0: 2a75 9f9a ea83 9aa4 adf2 e38f 787b 38ee  *u..........x{8.
+00001400: c3db faac 823a a857 ff4e 322a 58eb 4aa0  .....:.W.N2*X.J.
+00001410: 6ec1 a85c 90ec 0231 3c1e 0aaa b384 af9e  n..\...1<.......
+00001420: 24ac 1bd3 423b 737d 99d6 d541 a7dd 4719  $...B;s}...A..G.
+00001430: 987a ded3 c7b3 4cb8 4aa7 73d1 55c2 705b  .z....L.J.s.U.p[
+00001440: 8f52 15d3 797d eab5 37bb 0309 f8e6 eec7  .R..y}..7.......
+00001450: 2f8e a747 479d b68a ccdd b177 5367 f4db  /..GG......wSg..
+00001460: e5ee 7571 d12d 0007 6d42 3576 90d0 2718  ..uq.-..mB5v..'.
+00001470: 0804 9fde 31bf 495d 9bdc d1fa 6e88 9fca  ....1.I]....n...
+00001480: 3d3a 4d39 cdc7 6aab f370 9efa bb5b 7945  =:M9..j..p...[yE
+00001490: 3dca 7db3 feed a221 9c09 1375 89be e94d  =.}....!...u...M
+000014a0: bfa0 83bb 3814 f658 5b38 ea5c bbb3 9a80  ....8..X[8.\....
+000014b0: d9d3 dfb7 48a3 7dfc b3a7 efca 4dd6 fe7f  ....H.}.....M...
+000014c0: e690 c713 f1ff 0e24 eb9d 6e51 dd88 7d0a  .......$..nQ..}.
+000014d0: 91a6 d1a6 c4b1 3a50 ed5f 4b6c d953 b9f9  ......:P._Kl.S..
+000014e0: 59da fda7 7536 c9b1 ed34 358f 42fc f0eb  Y...u6...45.B...
+000014f0: fffa c3af 7e3e fafd bfff c31f 7ef3 affd  ....~>......~...
+00001500: 1925 6d3e e947 4726 b4a7 e4de 1a55 5926  .%m>.GG&.....UY&
+00001510: 617e 93c8 6c73 c8c3 7bad e689 0458 ebff  a~..ls..{....X..
+00001520: fecd 3f05 af95 7a0d 9f61 adad 37cf 5c7a  ..?...z..a..7.\z
+00001530: 35f7 ecd7 3be8 fc3b e244 ed8e d8c0 573f  5...;..;.D....W?
+00001540: 70d0 4548 a973 5db9 533a 06ea 5e30 a5fc  p.EH.s].S:..^0..
+00001550: 0666 0a86 70a6 82f6 eee1 833c c21b 7f80  .f..p......<....
+00001560: c373 9297 dce4 c7e9 9de0 97f7 e479 dffa  .s...........y..
+00001570: c991 dced 17fb ff5a 0161 377f 6f31 99a7  .......Z.a7.o1..
+00001580: d35a 6282 9f4a 0e15 151d a1e2 894a bde0  .Zb..J.......J..
+00001590: 3779 889b a8b4 1f4b 9f86 e4a8 e291 5d2c  7y.....K......],
+000015a0: de9e 629e 8c68 8945 5a4f a8db 4ce9 2493  ..b..h.EZO..L.$.
+000015b0: 9768 42b3 42df f38a de96 611e dc6c 89a0  .hB.B.....a..l..
+000015c0: b18c 9da6 b285 daa8 5d7b abe3 a52d 67a2  ........]{...-g.
+000015d0: e321 5e62 309c 4959 887c 0594 0c04 3e60  .!^b0.IY.|....>`
+000015e0: 61e8 aab6 6fc0 2acc 230a 1691 045b 8657  a...o.*.#....[.W
+000015f0: 8b82 1679 5b96 e1ed 1c66 57fb d33f ffec  ...y[....fW..?..
+00001600: 877f f9c7 d124 78dd 526d 6e4b 2073 a165  .....$x.RmnK s.e
+00001610: cf51 d1b7 ff76 a6b7 34cc 9694 c528 c84f  .Q...v..4....(.O
+00001620: 5c32 9a12 78b6 dc85 920d b790 026c 031c  \2..x........l..
+00001630: 0165 b9bd 43c0 5ba5 dd02 842c 61ea 5a25  .e..C.[....,a.Z%
+00001640: bcfc 894a d457 e905 8d6d 4ba8 9b44 51b9  ...J.W...mK..DQ.
+00001650: 4892 3bda b46f 9b5f 93bf 6df3 06a8 afa9  H.;..o._..m.....
+00001660: cdcc 5c95 c43d 0b15 b717 deb4 c5fd 5957  ..\..=........YW
+00001670: 6e66 aeb4 f2bd d095 7b65 72ed 957f 5186  nf......{er...Q.
+00001680: b6cd fb73 de86 6626 cf24 ee87 a1e2 f602  ...s..f&.$......
+00001690: afb6 b86d 8676 272b 37f3 615a f9a3 d095  ...m.v'+7.aZ....
+000016a0: 7be5 c1ed 957f 5986 4618 a1bf 7620 d3b9  {.....Y.F...v ..
+000016b0: 1b0c 2066 9e4d e2de 0f15 77c8 9d13 bda9  .. f.M....w.....
+000016c0: 4483 e52a 69bd d595 9be9 35ad fc71 e8ca  D..*i.....5..q..
+000016d0: c986 dcf9 c117 6068 772c 6033 59ff f4f3  ......`hw,`3Y...
+000016e0: fffe f49f fff6 e9d7 7ffb e9ef 7ff6 e957  ...............W
+000016f0: bf09 9533 bc63 8469 4be7 e5a0 01b9 b705  ...3.c.iK.......
+00001700: dfc8 609b 868f 6f0d 3733 3375 badf 851a  ..`...o.733u....
+00001710: 38dd 6a4d 2e50 cfcb e08d 645c b47b 95f4  8.jM.P....d\.{..
+00001720: 25a3 5883 9142 3b1f fbce ce87 7e80 456c  %.X..B;.....~.El
+00001730: 2fc8 c9f9 deec 52e3 6bb3 85f4 c3ff fcdd  /.....R.k.......
+00001740: ef7e fb4b 39cc 5ced 9b29 4577 aeec 19c6  .~.K9.\..)Ew....
+00001750: 3d6f c598 4503 2986 ba88 1dc5 8022 8d8c  =o..E.)......"..
+00001760: 79cf abe1 68d3 8cad 8c06 11dc 89d2 4096  y...h.........@.
+00001770: 642d 04c6 3ad8 ce30 6b18 16b7 6f3e 0346  d-..:..0k...o>.F
+00001780: dcad 5394 1fb8 4040 251c ba3f 284d 78f9  ..S...@@%..?(Mx.
+00001790: 032d 2dd0 ecf4 cba3 d43e 4c83 1b7d 8506  .--......>L..}..
+000017a0: ebc6 2147 f374 cf2c 3448 5e54 a675 cd93  ..!G.t.,4H^T.u..
+000017b0: 404e 1794 9ab9 97a0 0ce0 b84b f354 a608  @N.........K.T..
+000017c0: ff5a 8ea6 78db 9959 a628 b776 d999 ba9c  .Z..x..Y.(.v....
+000017d0: 4917 9f7a 87ca 4b7c 8376 065e cd29 92ad  I..z..K|.v.^.)..
+000017e0: d720 0d00 a538 4ed1 dceb e0eb cdbe e0b9  . ...8N.........
+000017f0: 6756 2724 65ca 583b d609 d66c 82a7 575d  gV'$e.X;...l..W]
+00001800: f225 80a7 b2ce fa88 4b4b b438 c31b 044a  .%......KK.8...J
+00001810: b3fc 518e ef34 e03e 097b ed11 9184 070d  ..Q..4.>.{......
+00001820: 1815 3814 9f3b 66a7 f637 7170 bb73 7b9b  ..8..;f..7qp.s{.
+00001830: 9d59 ab90 6ca8 a5d0 353b c24a ddab f7bc  .Y..l...5;.J....
+00001840: aa94 50b3 03e1 282b b12f d31b c3cc c244  ..P...(+./.....D
+00001850: 7997 d304 281b 69ad d6ab a9e7 6b02 9f17  y...(.i.....k...
+00001860: c33c 1dcd db98 ccea 84a4 4cc0 d435 26b2  .<........L..5&.
+00001870: b196 78bd 0abf cf6b 4cd6 02c4 d948 92af  ..x....kL....H..
+00001880: 7b60 265a 5fcd b0e7 d5b8 f335 2606 9ec8  {`&Z_......5&...
+00001890: 6cf0 06b1 d65a 0338 5b4d 330a 722d 4bf0  l....Z.8[M3.r-K.
+000018a0: ea35 f9ca e6b3 3a9a 6f87 c9d7 d160 67b0  .5....:.o....`g.
+000018b0: 9bfa af22 78a7 28a9 e065 7869 059d 1d4b  ..."x.(..exi...K
+000018c0: f9d4 7c2f 3fd4 9140 8ca0 2328 7fa7 f256  ..|/?..@..#(...V
+000018d0: 2ff1 a17b 7797 6bbf b20e f881 e583 562a  /..{w.k.......V*
+000018e0: 7896 51de b234 cb82 7233 b78b 52ed ca0e  x.Q..4..r3..R...
+000018f0: c9d2 4b0a dab2 2c81 5dc5 bef2 9bff 0350  ..K...,.]......P
+00001900: 4b03 0414 0000 0008 0087 4ee2 40a6 3496  K.........N.@.4.
+00001910: ede5 0400 0074 0d00 0011 0000 0077 6f72  .....t.......wor
+00001920: 642f 7365 7474 696e 6773 2e78 6d6c b557  d/settings.xml.W
+00001930: 596f db38 107e 5f60 ff83 a177 d7ba 650b  Yo.8.~_`...w..e.
+00001940: 750b eb60 d322 6983 3ad9 7da6 25da e686  u..`."i.:.}.%...
+00001950: 2205 8ab2 ebfc fa0e 75c4 49cd 1445 17cd  ".......u.I..E..
+00001960: 4ba8 f9e6 9ee1 70fc f6fd b78a 4d0e 4436  K.....p.....M.D6
+00001970: 54f0 a5e5 bcb1 ad09 e185 2829 df2d adfb  T.........().-..
+00001980: 3b34 9d5b 9346 615e 6226 3859 5a27 d258  ;4.[.Fa^b&8YZ'.X
+00001990: efdf fdfd d7db 63dc 10a5 80ad 9980 0ade  ......c.........
+000019a0: c455 b1b4 f64a d5f1 6cd6 147b 52e1 e68d  .U...J..l..{R...
+000019b0: a809 0770 2b64 8515 7cca ddac c2f2 a1ad  ...p+d..|.......
+000019c0: a785 a86a ace8 8632 aa4e 33d7 b643 6b50  ...j...2.N3..CkP
+000019d0: 2396 562b 793c a898 56b4 90a2 115b a545  #.V+y<..V....[.E
+000019e0: 62b1 ddd2 820c ff46 09f9 2b76 7bc9 4c14  b......F..+v{.L.
+000019f0: 6d45 b8ea 2cce 2461 e083 e0cd 9ed6 cda8  mE..,.$a........
+00001a00: adfa 5d6d 10e2 7e54 72f8 5910 878a 8d7c  ..]m..~Tr.Y....|
+00001a10: 47c7 fe19 e710 ee51 c8f2 49e2 57dc d302  G......Q..I.W...
+00001a20: b514 0569 1a28 50c5 fa70 2b4c f993 1ac7  ...i.(P..p+L....
+00001a30: bf50 f494 ea37 90ea 596f 7ba6 5581 b863  .P...7..Yo{.U..c
+00001a40: 77a7 b3e7 0dbb 9037 54bb afe2 35dd 482c  w......7T...5.H,
+00001a50: fb32 4303 682f aa22 feb8 e342 e20d 83a6  .2C.h/."...B....
+00001a60: 3a3a bef5 0e3a ea51 886a 728c 6b22 0b28  ::...:.Q.jr.k".(
+00001a70: d2d2 82be b066 1ad8 8017 d0a3 99f8 2cd4  .....f........,.
+00001a80: ba95 52b4 bcbc 2218 68c0 7ec0 e08b f33a  ..R...".h.~....:
+00001a90: 2312 425d 3096 4327 dc4a 000b dd05 a089  #.B]0.C'.J......
+00001aa0: 7068 d582 e80e 595a 83e9 926c 71cb d41d  ph....YZ...lq...
+00001ab0: deac 95a8 4773 be3b c212 1f21 c71f 242d  ....Gs.;...!..$-
+00001ac0: ff21 52d1 02b3 758d 0b20 8dac 4e10 f6be  .!R...u.. ..N...
+00001ad0: 95b4 a919 3e5d 0949 1f05 5798 6567 d91c  ....>].I..W.eg..
+00001ae0: aee0 6994 1855 f7fc a3da d7b8 dd5e 7bb1  ..i..U.......^{.
+00001af0: c712 1710 e860 3e05 1352 b051 a7be 7012  .....`>..R.Q..p.
+00001b00: fae1 b6e5 856a bbb6 1fe4 ba9b a893 dc80  .....j..........
+00001b10: df04 0979 7fdd e71c 33cc 0bb2 8650 1849  ...y....3....P.I
+00001b20: 4e8a 64a2 856a e9d3 bfb4 54fb 8ea9 d415  N.d..j....T.....
+00001b30: b926 f840 125c 3c34 0c37 fb95 1e14 1dd8  .&.@.\<4.7......
+00001b40: b23b 8969 978f 9ed0 71e7 df6a 1827 eb3d  .;.i....q..j.'.=
+00001b50: ddaa af44 c15d ef78 71f9 5fdb a86b cac9  ...D.].xq._..k..
+00001b60: 15a1 bbbd fac8 21e3 6cd0 d310 945f e393  ......!.l...._..
+00001b70: 6855 c7db 0f8f 753f 7e20 408e 2b68 a29e  hU....u?~ @.+h..
+00001b80: 3a8c 941b 5112 0ba0 56d2 8b3e 7db5 cfb5  :...Q...V..>}...
+00001b90: 40df 4cc1 f3dc fc68 4840 ada0 dca4 7370  @.L....hH@....sp
+00001ba0: ad4e 0c92 c6d5 9a3e 9215 2f3f 4114 1486  .N.....>../?A...
+00001bb0: 549f e1df f7e0 670e 10ae 53f3 0586 ebdd  T.....g...S.....
+00001bc0: a926 8860 c822 8ce5 3f63 acab 1962 b4be  .&.`."..?c...b..
+00001bd0: a170 efe4 475e c2ed f863 c6e8 764b 2418  .p..G^...c..vK$.
+00001be0: a058 911b b876 548a 6397 e7fe b6ff 5fbb  .X...vT.c....._.
+00001bf0: b363 dcb7 89ee 7778 f3ca 663c 7c85 2131  .c....wx..f<|.!1
+00001c00: 96df b67d cf0e f261 a468 b633 e284 5e94  ...}...a.h.3..^.
+00001c10: a1be 3a3f 2099 334f 87ab fb12 71c3 d04f  ..:? .3O....q..O
+00001c20: 1726 192f b551 6044 7cd7 0b73 33f2 aa6f  .&./.Q`D|..s3..o
+00001c30: 3e72 5068 9409 16c1 2a30 c613 26be eb18  >rPh....*0..&...
+00001c40: 65a2 c473 c3e1 22bc 8c27 ca9d c07f 0571  e..s.."..'.....q
+00001c50: 1789 1199 2fec 7998 9872 b0c8 fcdc 9f9b  ..../.y..r......
+00001c60: 9024 b39d dc98 d124 0bb3 d5ca 2493 7a51  .$.....$....$.zQ
+00001c70: ba8a 8c48 68e7 8931 0769 e805 7e66 92c9  ...Hh..1.i..~f..
+00001c80: ecc8 718d 3219 7256 816f 92c9 ed28 8d8c  ..q.2.rV.o...(..
+00001c90: dac0 bc17 0d8f c1cb 8ca2 79b8 c88d da50  ..........y....P
+00001ca0: e6a2 c42c 93db eeca 9051 3789 f2c8 770d  ...,.....Q7...w.
+00001cb0: 39f0 508e 506a aa42 e025 f9c2 7387 a7e4  9.P.Pj.B.%..s...
+00001cc0: b96f 2142 793e b7f3 cb48 2327 4b9c 8563  .o!By>...H#'K..c
+00001cd0: 9089 2290 89e6 86ca 4509 f216 a19d 5e6a  ..".....E.....^j
+00001ce0: 4b32 80e0 ef12 c9f2 14e5 abc4 a02d 43ae  K2...........-C.
+00001cf0: b74a 4d1d 8fc2 08ad d0dc d055 08cd 3304  .JM........U..3.
+00001d00: 3daf edc0 34d0 a1c2 0ca8 62bd bddd caf1  =...4.....b.....
+00001d10: a407 faa4 ea1f 8314 571b 49f1 e446 ef77  ........W.I..F.w
+00001d20: 2055 c51b f990 503e e21b 024b 0379 8eac   U....P>...K.y..
+00001d30: dbcd 084e a73d d054 9831 040f f408 74e1  ...N.=.T.1....t.
+00001d40: 54b1 de09 32b2 edd4 b21b 2c77 67bd 0387  T...2.....,wg...
+00001d50: 3452 612b f9f4 a44b 2f4b 447e 80ad a8ee  4Ra+...K/KD~....
+00001d60: ad1d 25ae fb41 3d9a 737c 7fd0 4739 bcb2  ..%..A=.s|..G9..
+00001d70: d548 6fda cd7a 94e2 b0a3 3d83 60c5 fa72  .Ho..z....=.`..r
+00001d80: 905a e1ec 9c9e 63ac 60b5 ef1e bc6b 7cde  .Z....c.`....k|.
+00001d90: 7108 9fde aff5 0344 70a3 560d c54b eb71  q......Dp.V..K.q
+00001da0: 3f4d 3f6b 6918 b94c aef5 2f02 7283 ebba  ?M?ki..L../.r...
+00001db0: df8c 363b 6769 31fd d03b 5a4c c157 09bf  ..6;gi1..;ZL.W..
+00001dc0: 0cba 8fcd ce1d 30b7 c3e0 4b63 dd07 2e74  ......0...Kc...t
+00001dd0: b0c0 3d1c 3443 7f04 aee1 70a6 7923 cd3b  ..=.4C....p.y#.;
+00001de0: d360 efed f9fc 332d 1869 c199 168e 34f8  .`....3-.i....4.
+00001df0: 6572 8cf7 f0d0 4a46 f903 6c13 e351 d3b7  er....JF..l..Q..
+00001e00: 8231 7124 e5d5 485c 5a17 a42e 85e7 9f4b  .1q$..H\Z......K
+00001e10: efbe 0350 4b03 0414 0000 0008 0087 4ee2  ...PK.........N.
+00001e20: 407f d10b b4e8 0100 009e 0500 0010 0000  @...............
+00001e30: 0077 6f72 642f 6865 6164 6572 312e 786d  .word/header1.xm
+00001e40: 6ca5 94db 6e9c 3010 86ef 2bf5 1d90 ef17  l...n.0...+.....
+00001e50: c336 892a 1436 52b3 6a95 bb4a 691f c06b  .6.*.6R.j..Ji..k
+00001e60: cc62 057b 2cdb e06e 9fbe 6316 d84d 8956  .b.{,..n..c..M.V
+00001e70: 39dc 003e cc37 ffcc 3073 7bf7 47b5 492f  9..>.7..0s{.G.I/
+00001e80: ac93 a04b 92a7 1949 84e6 5049 bd2f c9ef  ...K...I..PI./..
+00001e90: 5fdf 575f 49e2 3cd3 156b 418b 921c 8423  _.W_I.<..kA....#
+00001ea0: 779b cf9f 6e43 d154 3641 6bed 8a60 7849  w...nC.T6Ak..`xI
+00001eb0: 1aef 4d41 a9e3 8d50 cca5 4a72 0b0e 6a9f  ..MA...P..Jr..j.
+00001ec0: 7250 14ea 5a72 4103 d88a aeb3 3c1b be8c  rP..ZrA.....<...
+00001ed0: 052e 9c43 57f7 4cf7 cc91 11a7 9634 3042  ...CW.L......40B
+00001ee0: a3af 1aac 62de a560 f754 31fb d499 15d2  ....b..`.T1.....
+00001ef0: 0df3 7227 5be9 0fc8 ce6e 260c 94a4 b3ba  ..r'[....n&.....
+00001f00: 1805 ad66 41d1 a438 0a1a 5f93 855d 44f1  ...fA..8.._..]D.
+00001f10: 82df a3e5 1678 a784 f683 476a 458b 1a40  .....x....GjE..@
+00001f20: bb46 9a53 18ef a561 88cd 24a9 bf14 44af  .F.S...a..$...D.
+00001f30: dae9 5e30 f9d5 c2df 1cf2 6b6a b0b5 2c60  ..^0......kj..,`
+00001f40: 294e c005 ee85 6454 4723 d51e f310 eb7b  )N....dTG#.....{
+00001f50: aaea ffc4 3cbb 14cc 5891 8898 35bc 46c2  ....<...X...5.F.
+00001f60: 739f 9312 c5a4 9e31 ef4b cd59 72f3 eb85  s......1.K.Yr...
+00001f70: 928b b95d 0fff f719 c060 377d a441 7e58  ...].....`7}.A~X
+00001f80: e8cc 1c8f 911f a33d e8a7 9915 9bfa 0dca  .......=........
+00001f90: b29b 4568 ee4d 8045 ef3f 36cc 8859 8e71  ..Eh.M.E.?6..Y.q
+00001fa0: f79d f3a0 b6cc b399 1b42 4883 7129 d7e3  .........BH.q)..
+00001fb0: 2039 ebbe fc0b c5a3 9311 4914 2f1e f61a   9........I./...
+00001fc0: 2cdb b518 5bc8 af92 905f 27b1 41c8 06c7  ,...[...._'.A...
+00001fd0: 9619 1e3f edf0 7af4 8756 24a1 e859 8bd3  ...?..z..V$..Y..
+00001fe0: 6f4d e8b0 fbad 1a4e 77e0 51c9 74aa 71fe  oM.....Nw.Q.t.q.
+00001ff0: 115c 7068 0107 05eb 3cc4 a5fb 5b12 1c9a  .\ph....<...[...
+00002000: f861 1847 7f79 6450 7433 42e2 36b6 155e  .a.G.ydPt3B.6..^
+00002010: d809 1c5f f1c6 7ab8 cf6a 2f90 1357 a345  ..._..z..j/..W.E
+00002020: d414 2d87 274e d7cd 3f50 4b03 0414 0000  ..-.'N..?PK.....
+00002030: 0008 0087 4ee2 4096 3d9c 92c5 0100 0051  ....N.@.=......Q
+00002040: 0500 0010 0000 0077 6f72 642f 6865 6164  .......word/head
+00002050: 6572 322e 786d 6ca5 94cb 6edb 3010 45f7  er2.xml...n.0.E.
+00002060: 05f2 0f02 f716 4537 090a 2172 1631 1a64  ......E7..!r.1.d
+00002070: 5720 ed07 d014 6511 e10b 2425 d67f dfa1  W ....e...$%....
+00002080: 2cc9 6e14 1879 6c44 eb31 67ee 9df1 ccdd  ,.n..ylD.1g.....
+00002090: fd5f 25b3 9e3b 2f8c ae10 c90b 9471 cd4c  ._%..;/......q.L
+000020a0: 2df4 be42 7f7e ff5c fd40 990f 54d7 541a  -..B.~.\.@..T.T.
+000020b0: cd2b 74e0 1edd 6fae bedd c5b2 ad5d 06d1  .+t...o......]..
+000020c0: da97 d1b2 0ab5 21d8 1263 cf5a aea8 cf95  ......!..c.Z....
+000020d0: 60ce 78d3 849c 1985 4dd3 08c6 7134 aec6  `.x.....M...q4..
+000020e0: eb82 14c3 2feb 0ce3 de43 aa07 aa7b ead1  ..../....C...{..
+000020f0: 8853 4b9a b15c 43ae c638 4583 cf8d db63  .SK..\C..8E....c
+00002100: 45dd 4b67 5740 b734 889d 9022 1c80 5ddc  E.KgW@.4..."..].
+00002110: 4e18 53a1 cee9 7214 b49a 05a5 90f2 2868  N.S...r.......(h
+00002120: 3ca6 08b7 70f1 46de 63e4 d6b0 4e71 1d86  <...p.F.c...Nq..
+00002130: 8cd8 7109 1a8c f6ad b027 1b9f a581 c576  ..q......'.....v
+00002140: 92d4 5f32 d12b 397d 172d b95e e49b 2dbf  .._2.+9}.-.^..-.
+00002150: a707 5b47 23b4 e204 5ce0 de28 467d 0c52  ..[G#...\..(F}.R
+00002160: f258 87d4 df53 575f 1349 71c9 ccd8 9184  .X...SW_.Iq.....
+00002170: 9835 bc47 c2ff 3927 258a 0a3d 633e 579a  .5.G..9'%..=c>W.
+00002180: b3e2 929b 8592 8bb5 5d0f ffef 3380 8569  ........]...3..i
+00002190: faca 803c 3ad3 d9d9 8f15 5fa3 3de9 9799  ...<:....._.=...
+000021a0: 9586 fa03 ca8a db85 35ff 21c0 62f6 9f5b  ........5.!.b..[
+000021b0: 6af9 2cc7 fa87 ce07 a3b6 34d0 991b 63cc  j.,.......4...c.
+000021c0: a3f5 39d3 e322 399b 3ef2 1dc3 ab53 10ca  ..9.."9.>....S..
+000021d0: 142b 9ff6 da38 ba93 e02d 92eb 2c92 9b2c  .+...8...-..,..,
+000021e0: 0d08 dac0 dab2 c3e5 971b 8ee7 7090 3c8b  ............p.<.
+000021f0: 654f 256c bf35 c2e9 a9b7 94c1 24c0 e31d  eO%l.5......$...
+00002200: 878d 0310 b286 bd18 4bda 040e 3b22 ddc1  ........K...;"..
+00002210: 8718 5809 93ce e10a 0b71 f30f 504b 0304  ..X......q..PK..
+00002220: 1400 0000 0800 874e e240 963d 9c92 c501  .......N.@.=....
+00002230: 0000 5105 0000 1000 0000 776f 7264 2f68  ..Q.......word/h
+00002240: 6561 6465 7233 2e78 6d6c a594 cb6e db30  eader3.xml...n.0
+00002250: 1045 f705 f20f 02f7 1645 3709 0a21 7216  .E.......E7..!r.
+00002260: 311a 6457 20ed 07d0 1465 11e1 0b24 25d6  1.dW ....e...$%.
+00002270: 7fdf a12c c96e 1418 796c 44eb 3167 ee9d  ...,.n..ylD.1g..
+00002280: f1cc ddfd 5f25 b39e 3b2f 8cae 10c9 0b94  ...._%..;/......
+00002290: 71cd 4c2d f4be 427f 7eff 5cfd 4099 0f54  q.L-..B.~.\.@..T
+000022a0: d754 1acd 2b74 e01e dd6f aebe ddc5 b2ad  .T..+t...o......
+000022b0: 5d06 d1da 97d1 b20a b521 d812 63cf 5aae  ]........!..c.Z.
+000022c0: a8cf 9560 ce78 d384 9c19 854d d308 c671  ...`.x.....M...q
+000022d0: 34ae c6eb 8214 c32f eb0c e3de 43aa 07aa  4....../....C...
+000022e0: 7bea d188 534b 9ab1 5c43 aec6 3845 83cf  {...SK..\C..8E..
+000022f0: 8ddb 6345 dd4b 6757 40b7 3488 9d90 221c  ..cE.KgW@.4...".
+00002300: 805d dc4e 1853 a1ce e972 14b4 9a05 a590  .].N.S...r......
+00002310: f228 683c a608 b770 f146 de63 e4d6 b04e  .(h<...p.F.c...N
+00002320: 711d 868c d871 091a 8cf6 adb0 271b 9fa5  q....q......'...
+00002330: 81c5 7692 d45f 32d1 2b39 7d17 2db9 5ee4  ..v.._2.+9}.-.^.
+00002340: 9b2d bfa7 075b 4723 b4e2 045c e0de 2846  .-...[G#...\..(F
+00002350: 7d0c 52f2 5887 d4df 5357 5f13 4971 c9cc  }.R.X...SW_.Iq..
+00002360: d891 8498 35bc 47c2 ff39 2725 8a0a 3d63  ....5.G..9'%..=c
+00002370: 3e57 9ab3 e292 9b85 928b b55d 0fff ef33  >W.........]...3
+00002380: 8085 69fa ca80 3c3a d3d9 d98f 155f a33d  ..i...<:....._.=
+00002390: e997 9995 86fa 03ca 8adb 8535 ff21 c062  ...........5.!.b
+000023a0: f69f 5b6a f92c c7fa 87ce 07a3 b634 d099  ..[j.,.......4..
+000023b0: 1b63 cca3 f539 d3e3 2239 9b3e f21d c3ab  .c...9.."9.>....
+000023c0: 5310 ca14 2b9f f6da 38ba 93e0 2d92 eb2c  S...+...8...-..,
+000023d0: 929b 2c0d 08da c0da b2c3 e597 1b8e e770  ..,............p
+000023e0: 903c 8b65 4f25 6cbf 35c2 e9a9 b794 c124  .<.eO%l.5......$
+000023f0: c0e3 1d87 8d03 10b2 86bd 184b da04 0e3b  ...........K...;
+00002400: 22dd c187 1858 0993 cee1 0a0b 71f3 0f50  "....X......q..P
+00002410: 4b03 0414 0000 0008 0087 4ee2 400b 297d  K.........N.@.)}
+00002420: dfc4 0100 0051 0500 0010 0000 0077 6f72  .....Q.......wor
+00002430: 642f 666f 6f74 6572 312e 786d 6ca5 94c9  d/footer1.xml...
+00002440: 6ee3 300c 86ef 03f4 1d0c dd63 59e9 8281  n.0........cY...
+00002450: 51a7 8706 2d7a 2bd0 ce03 288a 1c0b d506  Q...-z+...(.....
+00002460: 49b6 266f 3f94 633b 99ba 08ba 5cac 78e1  I.&o?.c;....\.x.
+00002470: c7ff 2743 dede fd55 32eb b8f3 c2e8 0a91  ..'C...U2.......
+00002480: bc40 19d7 cc6c 85de 55e8 cfeb c3e2 37ca  .@...l..U.....7.
+00002490: 7ca0 7a4b a5d1 bc42 7bee d1dd eae2 d76d  |.zK...B{......m
+000024a0: 2ceb e032 88d6 be8c 9655 a809 c196 187b  ,..2.....U.....{
+000024b0: d670 457d ae04 73c6 9b3a e4cc 286c ea5a  .pE}..s..:..(l.Z
+000024c0: 308e a371 5bbc 2c48 d1ff b2ce 30ee 3da4  0..q[.,H....0.=.
+000024d0: baa7 baa3 1e0d 3835 a719 cb35 e4aa 8d53  ......85...5...S
+000024e0: 34f8 dcb8 1d56 d4bd b576 0174 4b83 d808  4....V...v.tK...
+000024f0: 29c2 1ed8 c5cd 8831 156a 9d2e 0741 8b49  )......1.j...A.I
+00002500: 500a 290f 8286 638c 7033 171f e43d 44ae  P.)...c.p3...=D.
+00002510: 0d6b 15d7 a1cf 881d 97a0 c168 df08 7bb4  .k.........h..{.
+00002520: f15d 1a58 6c46 49dd 3913 9d92 e377 d192  .].XlFI.9....w..
+00002530: ab59 bec9 f267 7ab0 7634 422b 8ec0 19ee  .Y...gz.v4B+....
+00002540: 8362 6c0f 414a 1eea 90fa 7bec ea7b 2229  .bl.AJ....{..{")
+00002550: ce99 193a 9210 9386 cf48 f83f e7a8 4451  ...:.....H.?..DQ
+00002560: a127 ccf7 4a73 525c 723d 5372 b6b6 cbfe  .'..JsR\r=Sr....
+00002570: ff7d 02b0 304d 3f19 9047 675a 3bf9 b1e2  .}..0M?..GgZ;...
+00002580: 67b4 27fd 36b1 d250 7f41 5971 33b3 e6bf  g.'.6..P.AYq3...
+00002590: 0498 cdfe 4b43 2d9f e458 7fdf fa60 d49a  ....KC-..X...`..
+000025a0: 063a 7163 8c79 b43e 677a 5824 27d3 472e  .:qc.y.>gzX$'.G.
+000025b0: 31bc 3a06 a14c b1f2 69a7 8da3 1b09 de22  1.:..L..i......"
+000025c0: b9ca 22b9 ced2 80a0 15ac 2ddb 5f9e 5d7f  ..".......-._.].
+000025d0: bc84 bde4 592c 3b2a 61fb 1184 d353 6f29  ....Y,;*a....So)
+000025e0: 8349 80c7 1b0e 1b07 2064 097b 3196 b40e  .I...... d.{1...
+000025f0: 1c76 44ba 830f 31b0 1226 9dfd 1516 e2ea  .vD...1..&......
+00002600: 1f50 4b03 0414 0000 0008 0087 4ee2 400b  .PK.........N.@.
+00002610: 297d dfc4 0100 0051 0500 0010 0000 0077  )}.....Q.......w
+00002620: 6f72 642f 666f 6f74 6572 322e 786d 6ca5  ord/footer2.xml.
+00002630: 94c9 6ee3 300c 86ef 03f4 1d0c dd63 59e9  ..n.0........cY.
+00002640: 8281 51a7 8706 2d7a 2bd0 ce03 288a 1c0b  ..Q...-z+...(...
+00002650: d506 49b6 266f 3f94 633b 99ba 08ba 5cac  ..I.&o?.c;....\.
+00002660: 78e1 c7ff 2743 dede fd55 32eb b8f3 c2e8  x...'C...U2.....
+00002670: 0a91 bc40 19d7 cc6c 85de 55e8 cfeb c3e2  ...@...l..U.....
+00002680: 37ca 7ca0 7a4b a5d1 bc42 7bee d1dd eae2  7.|.zK...B{.....
+00002690: d76d 2ceb e032 88d6 be8c 9655 a809 c196  .m,..2.....U....
+000026a0: 187b d670 457d ae04 73c6 9b3a e4cc 286c  .{.pE}..s..:..(l
+000026b0: ea5a 308e a371 5bbc 2c48 d1ff b2ce 30ee  .Z0..q[.,H....0.
+000026c0: 3da4 baa7 baa3 1e0d 3835 a719 cb35 e4aa  =.......85...5..
+000026d0: 8d53 34f8 dcb8 1d56 d4bd b576 0174 4b83  .S4....V...v.tK.
+000026e0: d808 29c2 1ed8 c5cd 8831 156a 9d2e 0741  ..)......1.j...A
+000026f0: 8b49 500a 290f 8286 638c 7033 171f e43d  .IP.)...c.p3...=
+00002700: 44ae 0d6b 15d7 a1cf 881d 97a0 c168 df08  D..k.........h..
+00002710: 7bb4 f15d 1a58 6c46 49dd 3913 9d92 e377  {..].XlFI.9....w
+00002720: d192 ab59 bec9 f267 7ab0 7634 422b 8ec0  ...Y...gz.v4B+..
+00002730: 19ee 8362 6c0f 414a 1eea 90fa 7bec ea7b  ...bl.AJ....{..{
+00002740: 2229 ce99 193a 9210 9386 cf48 f83f e7a8  ")...:.....H.?..
+00002750: 4451 a127 ccf7 4a73 525c 723d 5372 b6b6  DQ.'..JsR\r=Sr..
+00002760: cbfe ff7d 02b0 304d 3f19 9047 675a 3bf9  ...}..0M?..GgZ;.
+00002770: b1e2 67b4 27fd 36b1 d250 7f41 5971 33b3  ..g.'.6..P.AYq3.
+00002780: e6bf 0498 cdfe 4b43 2d9f e458 7fdf fa60  ......KC-..X...`
+00002790: d49a 063a 7163 8c79 b43e 677a 5824 27d3  ...:qc.y.>gzX$'.
+000027a0: 472e 31bc 3a06 a14c b1f2 69a7 8da3 1b09  G.1.:..L..i.....
+000027b0: de22 b9ca 22b9 ced2 80a0 15ac 2ddb 5f9e  ."..".......-._.
+000027c0: 5d7f bc84 bde4 592c 3b2a 61fb 1184 d353  ].....Y,;*a....S
+000027d0: 6f29 8349 80c7 1b0e 1b07 2064 097b 3196  o).I...... d.{1.
+000027e0: b40e 1c76 44ba 830f 31b0 1226 9dfd 1516  ...vD...1..&....
+000027f0: e2ea 1f50 4b03 0414 0000 0008 0087 4ee2  ...PK.........N.
+00002800: 400b 297d dfc4 0100 0051 0500 0010 0000  @.)}.....Q......
+00002810: 0077 6f72 642f 666f 6f74 6572 332e 786d  .word/footer3.xm
+00002820: 6ca5 94c9 6ee3 300c 86ef 03f4 1d0c dd63  l...n.0........c
+00002830: 59e9 8281 51a7 8706 2d7a 2bd0 ce03 288a  Y...Q...-z+...(.
+00002840: 1c0b d506 49b6 266f 3f94 633b 99ba 08ba  ....I.&o?.c;....
+00002850: 5cac 78e1 c7ff 2743 dede fd55 32eb b8f3  \.x...'C...U2...
+00002860: c2e8 0a91 bc40 19d7 cc6c 85de 55e8 cfeb  .....@...l..U...
+00002870: c3e2 37ca 7ca0 7a4b a5d1 bc42 7bee d1dd  ..7.|.zK...B{...
+00002880: eae2 d76d 2ceb e032 88d6 be8c 9655 a809  ...m,..2.....U..
+00002890: c196 187b d670 457d ae04 73c6 9b3a e4cc  ...{.pE}..s..:..
+000028a0: 286c ea5a 308e a371 5bbc 2c48 d1ff b2ce  (l.Z0..q[.,H....
+000028b0: 30ee 3da4 baa7 baa3 1e0d 3835 a719 cb35  0.=.......85...5
+000028c0: e4aa 8d53 34f8 dcb8 1d56 d4bd b576 0174  ...S4....V...v.t
+000028d0: 4b83 d808 29c2 1ed8 c5cd 8831 156a 9d2e  K...)......1.j..
+000028e0: 0741 8b49 500a 290f 8286 638c 7033 171f  .A.IP.)...c.p3..
+000028f0: e43d 44ae 0d6b 15d7 a1cf 881d 97a0 c168  .=D..k.........h
+00002900: df08 7bb4 f15d 1a58 6c46 49dd 3913 9d92  ..{..].XlFI.9...
+00002910: e377 d192 ab59 bec9 f267 7ab0 7634 422b  .w...Y...gz.v4B+
+00002920: 8ec0 19ee 8362 6c0f 414a 1eea 90fa 7bec  .....bl.AJ....{.
+00002930: ea7b 2229 ce99 193a 9210 9386 cf48 f83f  .{")...:.....H.?
+00002940: e7a8 4451 a127 ccf7 4a73 525c 723d 5372  ..DQ.'..JsR\r=Sr
+00002950: b6b6 cbfe ff7d 02b0 304d 3f19 9047 675a  .....}..0M?..GgZ
+00002960: 3bf9 b1e2 67b4 27fd 36b1 d250 7f41 5971  ;...g.'.6..P.AYq
+00002970: 33b3 e6bf 0498 cdfe 4b43 2d9f e458 7fdf  3.......KC-..X..
+00002980: fa60 d49a 063a 7163 8c79 b43e 677a 5824  .`...:qc.y.>gzX$
+00002990: 27d3 472e 31bc 3a06 a14c b1f2 69a7 8da3  '.G.1.:..L..i...
+000029a0: 1b09 de22 b9ca 22b9 ced2 80a0 15ac 2ddb  ..."..".......-.
+000029b0: 5f9e 5d7f bc84 bde4 592c 3b2a 61fb 1184  _.].....Y,;*a...
+000029c0: d353 6f29 8349 80c7 1b0e 1b07 2064 097b  .So).I...... d.{
+000029d0: 3196 b40e 1c76 44ba 830f 31b0 1226 9dfd  1....vD...1..&..
+000029e0: 1516 e2ea 1f50 4b03 040a 0000 0000 0087  .....PK.........
+000029f0: 4ee2 4000 0000 0000 0000 0000 0000 000b  N.@.............
+00002a00: 0000 0077 6f72 642f 7468 656d 652f 504b  ...word/theme/PK
+00002a10: 0304 1400 0000 0800 874e e240 c8d4 165a  .........N.@...Z
+00002a20: fe05 0000 2c19 0000 1500 0000 776f 7264  ....,.......word
+00002a30: 2f74 6865 6d65 2f74 6865 6d65 312e 786d  /theme/theme1.xm
+00002a40: 6ced 594b 6f1b 3710 be17 e87f 58ec bd95  l.YKo.7.....X...
+00002a50: 64eb 1119 9103 5b8f b88d 9d04 9192 2247  d.....[......."G
+00002a60: 6a97 da65 c45d 2e48 ca8e 6e41 722a 0a14  j..e.].H..nAr*..
+00002a70: 2890 1639 3440 d14b 0f45 d100 0dd0 a03d  (..94@.K.E.....=
+00002a80: f4bf d485 8334 fd11 1d72 a515 2951 f503  .....4...r..)Q..
+00002a90: 3e04 4564 1fb4 dc6f 663e ce70 bf21 5757  >.Ed...of>.p.!WW
+00002aa0: af3d 4ca8 7788 b920 2c6d f995 8fcb be87  .=L.w.. ,m......
+00002ab0: d380 8524 8d5a fedd 41ef a32b be27 244a  ...$.Z..A..+.'$J
+00002ac0: 4344 598a 5bfe 140b ffda f687 1f5c 455b  CDY.[........\E[
+00002ad0: 32c6 09f6 c03e 155b a8e5 c752 665b a592  2....>.[...Rf[..
+00002ae0: 0860 1889 8f59 8653 b837 623c 4112 2e79  .`...Y.S.7b<A..y
+00002af0: 540a 393a 02bf 092d 6d94 cbf5 5282 48ea  T.9:...-m...R.H.
+00002b00: 7b29 4ac0 edad d188 04d8 fbeb d5ef 6fbe  {)J...........o.
+00002b10: 7ff6 e7a3 2fe0 dfdf 9ec7 e852 0894 4aa1  ..../......R..J.
+00002b20: 0602 cafb 2a02 b60c 3536 1c57 1442 4c45  ....*...56.W.BLE
+00002b30: 9b72 ef10 d196 0fe1 4276 34c0 0fa5 ef51  .r......Bv4....Q
+00002b40: 2424 dc68 f965 fdf1 4bdb 574b 686b 6644  $$.h.e..K.WKhkfD
+00002b50: e51a 5bc3 aea7 3f33 bb99 4138 ded0 3179  ..[...?3..A8..1y
+00002b60: 342c 8256 abb5 6a7d a7f0 af01 54ae e2ba  4,.V..j}....T...
+00002b70: 8d6e bd5b 2ffc 6900 0a02 9869 cec5 f6d9  .n.[/.i....i....
+00002b80: d868 5767 5803 947f 75f8 ee34 3a9b 150b  .hWgX...u..4:...
+00002b90: 6ff8 df5c e1bc 5353 7f16 5e83 72ff d515  o..\..SS..^.r...
+00002ba0: 7caf d786 2c5a 780d caf1 b515 7c6d b7b9  |...,Zx.....|m..
+00002bb0: dbb1 fd6b 508e afaf e01b e59d 4eb5 61f9  ...kP.......N.a.
+00002bc0: d7a0 9892 74bc 822e d7ea 9bed f96c 0bc8  ....t........l..
+00002bd0: 88d1 3d27 bc59 abf6 1a1b 33e7 0b14 ac86  ..='.Y....3.....
+00002be0: 6275 a910 2396 ca75 6b2d 410f 18ef 0140  bu..#..uk-A....@
+00002bf0: 0129 9224 f5e4 34c3 2314 c062 7efd d3e7  .).$..4.#..b~...
+00002c00: af7f fbc3 db27 512c 5514 b485 9171 3b1f  .....'Q,U....q;.
+00002c10: 0ac4 ca90 0ae8 8980 934c b6fc 4f33 044f  .........L..O3.O
+00002c20: c7c2 e9c9 ab57 c78f 5f1e 3ffe f5f8 c993  .....W.._.?.....
+00002c30: e3c7 3f9b de2d bb3d 9446 a6dd db1f befa  ..?..-.=.F......
+00002c40: e7f9 23ef ef5f be7b fbf4 eb3c f432 5e98  ..#.._.{...<.2^.
+00002c50: f855 f2cb 7078 960c 5adf bc78 fdf2 c5c9  .U..px..Z..x....
+00002c60: b32f dffc f8d4 e17d 87a3 a109 1f90 040b  ./.....}........
+00002c70: ef26 3ef2 eeb0 0426 a8b3 6307 c043 7e3e  .&>....&..c..C~>
+00002c80: 8b41 8c88 69b1 9346 02a5 4845 71f8 efca  .A..i..F..HEq...
+00002c90: d842 df9c 228a 1cb8 5d6c e7f1 1e07 2d71  .B.."...]l....-q
+00002ca0: 01af 4f1e 5884 fb31 9f48 e2f0 7823 4e2c  ..O.X..1.H..x#N,
+00002cb0: e001 6374 9771 6716 6ea8 5846 9a07 9334  ..ct.qg.n.XF...4
+00002cc0: 7207 e713 1377 07a1 4357 ec36 4aad 2a77  r....w..CW.6J.*w
+00002cd0: 2719 8828 71b9 6cc7 d8a2 799b a254 a208  '..(q.l...y..T..
+00002ce0: a758 7aea 1e1b 63ec 98dd 7d42 acbc 1e90  .Xz...c...}B....
+00002cf0: 8033 c146 d2bb 4fbc 5d44 9c29 1990 a1b5  .3.F..O.]D.)....
+00002d00: 9a16 467b 2481 ba4c 5d04 a1de 566e 0eee  ..F{$..L]...Vn..
+00002d10: 79bb 8cba 66dd c187 3612 9e0d 441d e407  y...f...6...D...
+00002d20: 985a 69bc 8e26 1225 2e97 0394 5033 e1fb  .Zi..&.%....P3..
+00002d30: 48c6 2e92 fd29 0f4c 5c57 48a8 7484 29f3  H....).L\WH.t.).
+00002d40: ba21 16c2 6573 8bc3 7c8d a2df 4020 5fce  .!..es..|...@ _.
+00002d50: b21f d069 6223 b924 6397 cf7d c498 89ec  ...ib#.$c..}....
+00002d60: b071 3b46 49e6 c2f6 491a 9bd8 4fc4 1896  .q;FI...I...O...
+00002d70: 28f2 6e33 e982 1f30 fb09 51d7 5007 94ae  (.n3...0..Q.P...
+00002d80: 2df7 3d82 ad72 9fae 0677 4143 4d4a 8b05  -.=..r...wACMJ..
+00002d90: a2ee 4cb8 a396 d731 b3d6 6f7f 4a47 086b  ..L....1..o.JG.k
+00002da0: a901 85b7 843b 21e9 692a 9e07 b81c fd06  .....;!.i*......
+00002db0: 953c f9f6 b983 f2e5 68b6 dbb1 95f0 93f3  .<......h.......
+00002dc0: a9f5 0e27 cec7 656f 49a3 d7e1 9695 b9cd  ...'..eoI.......
+00002dd0: 7848 de7d 61ee a049 7a1b c3b3 b0da 9dde  xH.}a..Iz.......
+00002de0: ebf2 7b5d f6ff f7ba bcee 79be 7c35 5e08  ..{]......y.|5^.
+00002df0: 3068 b3da 07e6 1b6e bdfd 4ed6 eebe 4784  0h.....n..N...G.
+00002e00: d2be 9c52 bc2f f406 5c40 db09 7b30 a8ec  ...R./..\@..{0..
+00002e10: f401 1417 a7b1 2c86 afea 4986 0016 2ee2  ......,...I.....
+00002e20: 48db 789c c9cf 888c fb31 ca60 f35e f195  H.x......1.`.^..
+00002e30: 9348 cc5c 47c2 cb98 8043 a31e 76fa 5678  .H.\G....C..v.Vx
+00002e40: 3a49 0e58 981f 3a2b 1575 c0cc c543 20b9  :I.X..:+.u...C .
+00002e50: 182f d78a 7138 30c8 1c5d 6f2c 0e52 857b  ./..q80..]o,.R.{
+00002e60: cd36 d207 de39 0165 7b1e 1246 309b c4a6  .6...9.e{..F0...
+00002e70: 8344 633e a892 a48f d790 3407 093d b34b  .Dc>......4..=.K
+00002e80: 61d1 74b0 b8a2 dccf 4bb5 c202 a815 5581  a.t.....K.....U.
+00002e90: 7d91 07bb a996 5fab 8209 18c1 b109 511c  }....._.......Q.
+00002ea0: aa3a e5a5 9e57 5717 f332 2bbd 2e99 d60a  .:...WW..2+.....
+00002eb0: 28c3 0b8e d90a 5854 baa9 b8ae 9d9e 9a5d  (.....XT.......]
+00002ec0: bed4 ce50 698b 84b1 dc6c 123a 33ba 8789  ...Pi....l.:3...
+00002ed0: 1885 78b6 3ad5 e859 689c b7d6 cd45 492d  ..x.:..Yh....EI-
+00002ee0: 7a2a 15b3 5c18 341a 57fe 8bc5 456b 0d76  z*..\.4.W...Ek.v
+00002ef0: cbda 4053 5329 68ea 1db5 fcfa 660d 964c  ..@SS)h.....f..L
+00002f00: 80b2 963f 82c3 3b7c 4d32 583b 42ed 6711  ...?..;|M2X;B.g.
+00002f10: 8de0 4558 2079 fec0 5f44 5932 2e64 0789  ..EX y.._DY2.d..
+00002f20: 384f b816 9d5c 0d12 2231 f728 495a be9a  8O...\.."1.(IZ..
+00002f30: 7e51 069a 6a0d d1dc 2a1b 2008 ef2c b926  ~Q..j...*. ..,.&
+00002f40: c8ca bb46 0e8a 6e17 198f 4638 9066 d98d  ...F..n...F8.f..
+00002f50: 1195 e9fc 1214 3ed7 0ae7 5d6d 7e71 b0b2  ......>...]m~q..
+00002f60: 6413 2877 3f0e 8fbc 219d f03b 0896 58ad  d.(w?...!..;..X.
+00002f70: 5151 090c 8980 573c 953c 9b21 8197 9285  QQ....W<.<.!....
+00002f80: 902d d6df 5263 9ac9 aef9 5650 afa1 7c1c  .-..Rc....VP..|.
+00002f90: d12c 46b3 8e62 8a79 0ed7 525e d0d1 5745  .,F..b.y..R^..WE
+00002fa0: 0e8c abd9 9c21 a146 4a66 8d70 18a9 066b  .....!.FJf.p...k
+00002fb0: 26d5 eaa6 45d7 c839 aced baa7 1ba9 cc19  &...E..9........
+00002fc0: a2b9 e899 96aa a8ae e956 312b c2bc 0d2c  .........V1+...,
+00002fd0: e5f2 624d de60 354f 31b4 4bb3 c3e7 d2bd  ..bM.`5O1.K.....
+00002fe0: 2cb9 cdb9 d62d ed13 8a2e 0109 2ff2 e7e8  ,....-....../...
+00002ff0: ba67 6808 06b5 4530 8b9a 62bc 2ac3 4ab3  .gh...E0..b.*.J.
+00003000: 67a3 76ef 984f f014 6a67 6912 86ea d7e7  g.v..O..jgi.....
+00003010: 6e97 f256 f408 6738 18bc 50e7 07bb e555  n..V..g8..P....U
+00003020: 0b43 a3f9 be52 675a ff88 61fe c0c0 860f  .C...RgZ..a.....
+00003030: 403c 3af0 2a77 42a5 c805 4283 b6ff 0550  @<:.*wB...B....P
+00003040: 4b03 0414 0000 0008 0087 4ee2 4081 b4d3  K.........N.@...
+00003050: 50c4 0200 00e7 0700 0011 0000 0077 6f72  P............wor
+00003060: 642f 646f 6375 6d65 6e74 2e78 6d6c a595  d/document.xml..
+00003070: 4b73 db20 10c7 ef9d e977 d070 b725 f991  Ks. .....w.p.%..
+00003080: 3a9a 2899 3669 3239 b493 a99b 7307 2324  :.(.6i29....s.#$
+00003090: 3196 8001 64d5 f9f4 5d84 1e4e e5bc 2f06  1...d...]..N../.
+000030a0: 99dd dffe 975d e0ec e26f 5978 3baa 3413  .....]...oYx;.4.
+000030b0: 3c46 e134 401e e544 248c 6731 baff 7d3d  <F.4@..D$.g1..}=
+000030c0: 5921 4f1b cc13 5c08 4e63 b4a7 1a5d 9c7f  Y!O...\.Nc...]..
+000030d0: fe74 5647 8920 5549 b9f1 00c1 7554 4b12  .tVG. UI....uTK.
+000030e0: a3dc 1819 f9be 2639 2db1 9e96 8c28 a145  ......&9-....(.E
+000030f0: 6aa6 4494 be48 5346 a85f 0b95 f8b3 200c  j.D..HSF._.... .
+00003100: 9a99 5482 50ad 21de 25e6 3bac 518b 2bc7  ..T.P.!.%.;.Q.+.
+00003110: 3421 2987 58a9 5025 367a 2a54 e697 586d  4!).X.P%6z*T..Xm
+00003120: 2b39 01ba c486 6d58 c1cc 1ed8 c149 8711  +9....mX.....I..
+00003130: 31aa 148f 5a41 935e 9075 899c a076 e83c  1...ZA.^.u...v.<
+00003140: d428 8b23 719d e755 bb03 4d44 5fd1 0234  .(.#q..U..MD_..4
+00003150: 08ae 7326 8734 de4b 8314 f34e d2ee b924  ..s&.4.K...N...$
+00003160: 7665 d1d9 d532 5c8c e2f5 29bf a606 570a  ve...2\...)...W.
+00003170: d750 8a01 38c2 1dd9 8cc4 3995 85db 075b  .P..8.....9....[
+00003180: dfa1 aaff 135f 037c 4ce8 b825 66bc 17f6  ....._.|L..%f...
+00003190: be44 0fb6 2a0c 9edb d4b6 33ac 9021 e472  .D..*.....3..!.r
+000031a0: a4fd d9bd 9d35 fd7d 1052 c291 fac8 01b9  .....5.}.R......
+000031b0: 51a2 92bd 1cc9 3e46 bbe5 db9e 654f f61b  Q.....>F....eO..
+000031c0: 9405 27a3 d4f4 9b00 a3b3 bfce b1a4 bd1c  ..'.............
+000031d0: a92f 2b6d 4479 850d eeb9 755d 4f6b a9a7  ./+mDy....u]Ok..
+000031e0: 84b7 17c9 c1e9 0be7 3e2c 0d4e c82b 4974  ........>,.N.+It
+000031f0: 9b71 a1f0 a680 dcea 70e1 d5e1 d2b3 0704  .q......p.......
+00003200: 9dc3 ddb5 11c9 de8e b2f9 b953 7650 ed70  ...........SvP.p
+00003210: 2db8 d15e 1de5 8c9b 1851 accd 57cd 30f2  -..^.....Q..W.0.
+00003220: ad4d 8179 064b 3b5c c00a 9fdc af11 7c75  .M.y.K;\......|u
+00003230: 2631 7ac8 2797 3fad a5df e260 940e bb11  &1z.'.?....`....
+00003240: 626b 6fab b5c1 ca80 134b 6204 976d 1d71  bko......Kb..m.q
+00003250: 5c82 c23f 37e2 1b26 5b17 a5b3 fdce 93de  \..?7..&[.......
+00003260: d241 1bbd 9a12 e3a0 39c5 0955 bf68 4a15  .A......9..U.hJ.
+00003270: dcda d453 0d56 dd26 4b4b 367b 09e4 9429  ...S.V.&KK6{...)
+00003280: 6d1c 3715 c21c 3587 4bfe 88f9 93f4 f960  m.7...5.K......`
+00003290: 9ed0 1457 c54b 7cb8 8e3b fe23 8727 232c  ...W.K|..;.#.'#,
+000032a0: 0607 baa3 fc05 f95f 8e59 cb6c fd00 516b  ......._.Y.l..Qk
+000032b0: 78d5 c253 fb20 4045 617e b29a af1c 4e66  x..S. @Ea~....Nf
+000032c0: 3fb0 b2ba 8484 ff17 8ba6 1a8a 6539 543d  ?...........e9T=
+000032d0: 5c05 cde7 4618 e8c3 61b9 a0e9 c1aa 931f  \...F...a.......
+000032e0: a3d5 32b4 78b7 bd31 3a3d 9dd9 cfac 32b0  ..2.x..1:=....2.
+000032f0: dbb6 ca4d eb10 51d8 aed2 1213 a8ca 62d6  ...M..Q.......b.
+00003300: 9488 5716 ee0c e03d bd51 cc56 dc15 ae60  ..W....=.Q.V...`
+00003310: 1c1e 5bf8 b493 3b66 08c8 9f87 0d9a e458  ..[...;f.......X
+00003320: ad1d a8a1 439b 754d 0153 d7dc 30e9 5ee8  ....C.uM.S..0.^.
+00003330: f37f 504b 0304 0a00 0000 0000 874e e240  ..PK.........N.@
+00003340: 0000 0000 0000 0000 0000 0000 0a00 0000  ................
+00003350: 6375 7374 6f6d 586d 6c2f 504b 0304 1400  customXml/PK....
+00003360: 0000 0800 874e e240 dc7f 3ecf 9500 0000  .....N.@..>.....
+00003370: 0201 0000 1300 0000 6375 7374 6f6d 586d  ........customXm
+00003380: 6c2f 6974 656d 312e 786d 6c9d 8ec1 0ac2  l/item1.xml.....
+00003390: 3010 44ef 82ff 10f6 6eb7 d58b 9424 3db4  0.D.....n....$=.
+000033a0: 7816 d40f 0869 aa85 7653 baa9 d1bf b750  x....i..vS.....P
+000033b0: 10c5 9bd7 9979 c393 c5a3 efc4 dd8d dc7a  .....y.........z
+000033c0: 5290 2529 0847 d6d7 2d5d 155c ce87 cd1e  R.%).G..-].\....
+000033d0: 0407 43b5 e93c 3905 4fc7 50e8 f54a 726e  ..C..<9.O.P..Jrn
+000033e0: 270e beaf 4c30 623e 2156 700b 61c8 1163  '...L0b>!Vp.a..c
+000033f0: 8c49 1c38 b184 be69 5aeb 2a6f a7de 51c0  .I.8...iZ.*o..Q.
+00003400: 6d9a ed70 aeca 370a 0b9b ff49 6bb9 589c  m..p..7....Ik.X.
+00003410: 9c0d c7d1 0ffc 1da0 96f8 33c0 4f75 fd02  ..........3.Ou..
+00003420: 504b 0304 1400 0000 0800 874e e240 6343  PK.........N.@cC
+00003430: 7b45 e500 0000 4701 0000 1800 0000 6375  {E....G.......cu
+00003440: 7374 6f6d 586d 6c2f 6974 656d 5072 6f70  stomXml/itemProp
+00003450: 7331 2e78 6d6c 658f 516b 8330 1485 df07  s1.xmle.Qk.0....
+00003460: fb0f 72df 3546 ebd4 622c b44e e8eb d860  ..r.5F..b,.N...`
+00003470: af21 5edb 8049 c4c4 da31 f6df 1737 1874  .!^..I...1...7.t
+00003480: 7dba 9c7b b8df 39b7 da5d d510 5c70 b2d2  }..{..9..]..\p..
+00003490: 6806 348a 2140 2d4c 27f5 89c1 db6b 1b16  h.4.!@-L'....k..
+000034a0: 1058 c775 c707 a391 c107 5ad8 d58f 0f55  .X.u......Z....U
+000034b0: 67b7 1d77 dc3a 33e1 d1a1 0afc 42fa 796c  g..w.:3.....B.yl
+000034c0: 187c ee69 99e7 6dde 8449 9ced c34d 5cd0  .|.i..m..I...M\.
+000034d0: b0a4 e921 4c8b 6643 9ff3 2c6b cbe4 0b02  ...!L.fC..,k....
+000034e0: 9fad 3dc6 3238 3b37 6e09 b1e2 8c8a dbc8  ..=.28;7n.......
+000034f0: 8ca8 bdd9 9b49 71e7 e574 22a6 efa5 c0c6  .....Iq..t".....
+00003500: 8859 a176 2489 e327 2266 1faf ded5 00f5  .Y.v$..'"f......
+00003510: dae7 f7fa 057b 7b2b d76a f324 ff52 9665  .....{{+.j.$.R.e
+00003520: 8996 d146 42df 5369 4abc 75f8 0137 fe3f  ...FB.SiJ.u..7.?
+00003530: 2075 45fe b157 7df3 7bfd 0d50 4b03 0414   uE..W}.{..PK...
+00003540: 0000 0008 0087 4ee2 408c af87 adbf 0300  ......N.@.......
+00003550: 0084 1200 0012 0000 0077 6f72 642f 666f  .........word/fo
+00003560: 6e74 5461 626c 652e 786d 6ce5 58dd 4edb  ntTable.xml.X.N.
+00003570: 3014 be9f b477 8872 0f71 d242 4345 41f4  0....w.r.q.BCEA.
+00003580: 2768 d2c4 c560 dab5 9bba ad47 1c57 764a  'h...`.....G.WvJ
+00003590: d727 98a6 5d4d 93f6 06bb d8c5 9026 2e26  .'..]M.......&.&
+000035a0: 6d62 bccc 00f1 163b 7692 d2d2 a46b 5981  mb.....;v....kY.
+000035b0: 4d4b 4569 4fec 83fd f9fb be73 c2e6 f62b  MKEiO......s...+
+000035c0: 1618 4744 48ca c38a 69af 22d3 20a1 cf5b  ..GDH...i.". ..[
+000035d0: 34ec 54cc e707 de8a 6b1a 32c2 610b 073c  4.T.....k.2.a..<
+000035e0: 2415 7348 a4b9 bdf5 f8d1 e6a0 dce6 6124  $.sH..........a$
+000035f0: 0d98 1fca 32f3 2b66 378a 7a65 cb92 7e97  ....2.+f7.ze..~.
+00003600: 302c 5779 8f84 70b3 cd05 c311 7c15 1d8b  0,Wy..p.....|...
+00003610: 6171 d8ef adf8 9cf5 7044 9b34 a0d1 d072  aq......pD.4...r
+00003620: 105a 3793 3462 9e2c bcdd a63e a973 bfcf  .Z7.4b.,...>.s..
+00003630: 4818 e9f9 9620 0164 e4a1 ecd2 9e4c b30d  H.... .d.....L..
+00003640: e6c9 36e0 a2d5 13dc 2752 c29e 5910 e763  ..6.....'R..Y..c
+00003650: 9886 a334 7671 2a11 a3be e092 b7a3 55d8  ...4vq*.......U.
+00003660: 8c15 afc8 52a9 60ba 8df4 2716 9806 f3cb  ....R.`...'.....
+00003670: 4f3a 2117 b819 0076 03bb 686e 25c0 1983  O:!....v..hn%...
+00003680: 7288 1904 0f28 23d2 d823 03e3 1967 38d4  r....(#..#...g8.
+00003690: 037a 38e4 92d8 30e6 0807 1513 39f0 5a47  .z8...0.....9.ZG
+000036a0: 05b4 868a f0e3 c0a7 a269 a94c 7e17 0b49  .........i.L~..I
+000036b0: a2d1 4014 87db 98d1 6098 4685 ceab c7f7  ..@.....`.F.....
+000036c0: 68e4 77d3 f811 1654 2d2c 9e23 6907 6ef4  h.w....T-,.#i.n.
+000036d0: 6513 554c 3812 54da 714b 661c b12b a60b  e.UL8.T.qKf..+..
+000036e0: 1175 2511 0716 155f 400f 3dab 308a e831  .u%...._@.=.0..1
+000036f0: bece a387 d89e a7c6 4004 f224 b3f4 3aad  ........@..$..:.
+00003700: 9842 5388 9c1f bffd 79fa 3e07 081b 8040  .BS.....y.>....@
+00003710: 0080 9dbe 3281 70d7 b380 c0fd 88c7 f109  ....2.p.........
+00003720: 1c5a a48d fb41 340d 43b2 d8c2 350c 8eeb  .Z...A4.C...5...
+00003730: 7a2a 3a05 0330 7826 0c45 9864 2f06 c30b  z*:..0x&.E.d/...
+00003740: a0a3 92a1 cc44 622d 59dc d8af 4c24 90b3  .....Db-Y...L$..
+00003750: 4424 d27d 8f1f 64bc ef6b 42a4 6332 0931  D$.}..d..kB.c2.1
+00003760: 4ea3 f909 b103 3c0d 3251 7050 15f8 50d4  N.....<.2QpP..P.
+00003770: 0251 2271 f284 6167 a120 0754 caf8 c6fc  .Q"q..ag. .T....
+00003780: 8458 862e 141b d084 2e3c b854 50ad 264f  .X.......<.TP.&O
+00003790: 1757 dfdf fd55 bad0 7c06 c350 6c70 5143  .W...U..|..PlpQC
+000037a0: 2f7f 2136 c00c 8dc4 62ba a8f1 bea0 4428  /.!6....b.....D(
+000037b0: cbcc e144 09fc 6143 b341 9965 7121 4e30  ...D..aC.A.eq!N0
+000037c0: de22 22fc 7748 b13f 644d 9e2d 8e35 a815  ."".wH.?dM.-.5..
+000037d0: 3600 60a3 1288 c481 6fa5 785f 37ab 46a6  6.`.....o.x_7.F.
+000037e0: 45e4 558d dfb9 65aa ff7b f688 1a0e 6853  E.U...e..{....hS
+000037f0: 50cd 081c 447b 505b 818b ba7c c6f6 11d7  P...D{P[...|....
+00003800: bfa9 c2ea e982 aa9d 0358 93eb 1f99 85f5  .........X......
+00003810: 56fe 3126 9359 10a5 e2ca b451 9503 d91b  V.1&.Y.....Q....
+00003820: 0bd6 d5cb cf6f 2ebf 9d19 4f69 a71b 65e1  .....o....Oi..e.
+00003830: 94d4 dd1c a01e a0f0 ce41 257b 9ec2 bb64  .........A%{...d
+00003840: 9c76 fbcd 264d 1ce2 069f f4c1 4cbe 654b  .v..&M......L.eK
+00003850: 2e93 4fb7 ec4f e680 69d4 b1e4 d309 56bd  ..O..O..i.....V.
+00003860: 980f c730 a8ee ed66 bbaa 00d0 c67e 8dc4  ...0...f.....~..
+00003870: 9da2 10ff ada4 039b 25aa 14a9 25a2 70f1  ........%...%.p.
+00003880: e1f5 c5c9 9bab 4f67 e73f 8e2f bf9c 408d  ......Og.?./..@.
+00003890: ce29 4aaa 5151 3dbc 9bb4 2bd9 1dfc 721a  .)J.QQ=...+...r.
+000038a0: d786 0dc8 3b0d cdfb b840 af57 eb9e 57f3  ....;....@.W..W.
+000038b0: aa09 48ba 5d53 cd58 61a6 7e60 bd8d 499f  ..H.]S.Xa.~`..I.
+000038c0: a97b f592 3a55 759e 797d ca12 dab5 a5c9  .{..:Uu.y}......
+000038d0: e3e1 bab5 8b8f 5f67 776b 1b40 87fb 788a  ......_gwk.@..x.
+000038e0: d13d b753 1d23 43c1 ad79 a59a b733 4e06  .=.S.#C..y...3N.
+000038f0: 75a8 7399 e982 4f31 fb98 0df1 a1b1 db7f  u.s...O1........
+00003900: 8905 3ca1 e788 03fe 0500 d218 bbee d42f  ..<............/
+00003910: b439 a505 f64f fd62 413c 467e 01d5 f8fc  .9...O.bA<F~....
+00003920: f8f4 3f76 8dc4 3ee4 d62f 504b 0304 0a00  ..?v..>../PK....
+00003930: 0000 0000 874e e240 0000 0000 0000 0000  .....N.@........
+00003940: 0000 0000 0600 0000 5f72 656c 732f 504b  ........_rels/PK
+00003950: 0304 1400 0000 0800 874e e240 0122 221f  .........N.@."".
+00003960: fd00 0000 e102 0000 0b00 0000 5f72 656c  ............_rel
+00003970: 732f 2e72 656c 73ad 92dd 4a03 3110 85ef  s/.rels...J.1...
+00003980: 05df 21cc 7d37 db2a 22d2 6c6f 44e8 9d48  ..!.}7.*".loD..H
+00003990: 7d80 2199 dd0d ddfc 904c b57d 7b83 7fb8  }.!......L.}{...
+000039a0: b0ae bdf0 7232 67ce 7c73 c87a 7374 8378  ....r2g.|s.zst.x
+000039b0: a194 6df0 0a96 550d 82bc 0ec6 fa4e c1f3  ..m...U......N..
+000039c0: ee61 710b 2233 7a83 43f0 a4e0 4419 36cd  .aq."3z.C...D.6.
+000039d0: e5c5 fa89 06e4 3294 7b1b b328 2e3e 2be8  ......2.{..(.>+.
+000039e0: 99e3 9d94 59f7 e430 5721 922f 9d36 2487  ....Y..0W!./.6$.
+000039f0: 5cca d4c9 887a 8f1d c955 5ddf c8f4 d303  \....z...U].....
+00003a00: 9a91 a7d8 1a05 696b ae41 ec4e b16c fedb  ......ik.A.N.l..
+00003a10: 3bb4 add5 741f f4c1 91e7 8915 72ac 28ce  ;...t.......r.(.
+00003a20: 983a 6205 af21 1969 3e07 ab82 0c72 9a66  .:b..!.i>....r.f
+00003a30: 753e cdef 974a 478c 0619 a50e 8916 3195  u>...JG.......1.
+00003a40: 9c12 db92 ec37 5061 792c cff9 5d31 07b4  .....7Pay,..]1..
+00003a50: 3c1f 687c fc54 3c74 64f2 86cc 3c12 c638  <.h|.T<td...<..8
+00003a60: 4774 f59f 44fa 9039 b879 9e0f cd17 921c  Gt..D..9.y......
+00003a70: 7dcc e60d 504b 0304 0a00 0000 0000 874e  }...PK.........N
+00003a80: e240 0000 0000 0000 0000 0000 0000 1000  .@..............
+00003a90: 0000 6375 7374 6f6d 586d 6c2f 5f72 656c  ..customXml/_rel
+00003aa0: 732f 504b 0304 1400 0000 0800 874e e240  s/PK.........N.@
+00003ab0: 743f 397a bc00 0000 2801 0000 1e00 0000  t?9z....(.......
+00003ac0: 6375 7374 6f6d 586d 6c2f 5f72 656c 732f  customXml/_rels/
+00003ad0: 6974 656d 312e 786d 6c2e 7265 6c73 85cf  item1.xml.rels..
+00003ae0: c18a 0231 0c06 e0bb e03b 94dc 9dce 7810  ...1.....;....x.
+00003af0: 91e9 7859 16bc 89b8 e0b5 7432 33c5 6953  ..xY......t23.iS
+00003b00: 9a28 faf6 164f 2b2c ec31 09f9 fea4 dd3f  .(...O+,.1.....?
+00003b10: c2ac ee98 d953 34d0 5435 288c 8e7a 1f47  .....S4.T5(..z.G
+00003b20: 033f e7ef d516 148b 8dbd 9d29 a281 2732  .?.........)..'2
+00003b30: ecbb e5a2 3de1 6ca5 2cf1 e413 aba2 4436  ....=.l.,.....D6
+00003b40: 3089 a49d d6ec 260c 962b 4a18 cb64 a01c  0.....&..+J..d..
+00003b50: ac94 328f 3a59 77b5 23ea 755d 6f74 fe6d  ..2.:Yw.#.u]ot.m
+00003b60: 40f7 61aa 436f 201f fa06 d4f9 994a f2ff  @.a.Co ......J..
+00003b70: 360d 8377 f845 ee16 30ca 1f11 dadd 5828  6..w.E..0.....X(
+00003b80: 5cc2 7ccc 94b8 c836 8f28 06bc 6078 b79a  \.|....6.(..`x..
+00003b90: aadc 0bba 6bf5 c77f dd0b 504b 0304 0a00  ....k.....PK....
+00003ba0: 0000 0000 874e e240 0000 0000 0000 0000  .....N.@........
+00003bb0: 0000 0000 0b00 0000 776f 7264 2f5f 7265  ........word/_re
+00003bc0: 6c73 2f50 4b03 0414 0000 0008 0087 4ee2  ls/PK.........N.
+00003bd0: 40e0 8ea4 be33 0100 0038 0600 001c 0000  @....3...8......
+00003be0: 0077 6f72 642f 5f72 656c 732f 646f 6375  .word/_rels/docu
+00003bf0: 6d65 6e74 2e78 6d6c 2e72 656c 73b5 944b  ment.xml.rels..K
+00003c00: 4fc3 3010 84ef 48fc 07cb 77e2 2485 f250  O.0...H...w.$..P
+00003c10: 935e 1052 af28 485c 8db3 7988 c48e ec2d  .^.R.(H\..y....-
+00003c20: 22ff 9e15 a1a1 952a f7e2 1c77 adcc 371a  "......*...w..7.
+00003c30: c7b3 d97e f71d fb02 eb5a a333 9e44 3167  ...~.....Z.3.D1g
+00003c40: a095 295b 5d67 fcad 78b9 79e0 cca1 d4a5  ..)[]g..x.y.....
+00003c50: ec8c 868c 8fe0 f836 bfbe dabc 4227 913e  .......6....B'.>
+00003c60: 724d 3b38 462a da65 bc41 1c9e 8470 aa81  rM;8F*.e.A...p..
+00003c70: 5eba c80c a0e9 a432 b697 48a3 adc5 20d5  ^......2..H... .
+00003c80: a7ac 41a4 71bc 16f6 5883 e727 9a6c 5766  ..A.q...X..'.lWf
+00003c90: dcee ca47 ce8a 7120 f265 6d53 55ad 8267  ...G..q .emSU..g
+00003ca0: a3f6 3d68 3c83 1048 be80 04a5 ad01 33fe  ..=h<..H......3.
+00003cb0: 3b4e cb24 22a3 5c9c f740 1984 f350 1983  ;N.$".\..@...P..
+00003cc0: 60ff 4d4c f3ca c7bf 5f9e 9ffa f8eb e5f9  `.ML...._.......
+00003cd0: defc ef42 f21b 90e5 71fe d3ec cdff 7679  ...B....q.....vy
+00003ce0: be37 ffd5 f27c 6ffe 6948 be03 446a 1747  .7...|o.iH..Dj.G
+00003cf0: 9a7f cff0 b0f1 fd82 4912 d243 6534 16f2  ........I..Ce4..
+00003d00: a33b ea82 79e5 7541 f518 ae09 d4de a1e9  .;..y.uA........
+00003d10: dfa9 77e6 28a2 48cc 5bd1 22f4 de7b 099a  ..w.(.H.[."..{..
+00003d20: 89c3 b1a3 729f ad4c f321 0d71 d2f7 f90f  ....r..L.!.q....
+00003d30: 504b 0304 1400 0000 0800 874e e240 b2e5  PK.........N.@..
+00003d40: 51b6 9a01 0000 9808 0000 1300 0000 5b43  Q.............[C
+00003d50: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
+00003d60: 6cc5 964f 4fe3 3010 c5ef 487c 87c8 57d4  l..OO.0...H|..W.
+00003d70: b82d 1242 a829 87dd e5c8 7228 1257 634f  .-.B.)....r(.WcO
+00003d80: 5a6b fd4f 9e29 4bbf 3d93 94f6 0055 db10  Zk.O.)K.=....U..
+00003d90: 2a2e 9112 7bde efe9 cd38 c9e4 f6d5 bbe2  *...{....8......
+00003da0: 0532 da18 2a31 2a87 a280 a0a3 b161 5e89  .2..*1*......a^.
+00003db0: c7d9 dde0 5a14 482a 18e5 6280 4aac 00c5  ....Z.H*..b.J...
+00003dc0: edf4 fc6c 325b 25c0 82ab 0356 6241 946e  ...l2[%....VbA.n
+00003dd0: a444 bd00 afb0 8c09 02af d431 7b45 7c9b  .D.........1{E|.
+00003de0: e732 29fd 4fcd 418e 87c3 2ba9 6320 0834  .2).O.A...+.c .4
+00003df0: a046 434c 27bf a156 4b47 c59f 577e bc76  .FCL'..VKG..W~.v
+00003e00: c2e5 a2f8 b5de d7a0 2aa1 5272 562b 62a3  ........*.RrV+b.
+00003e10: b259 953b eb32 38dc 53f8 12cc 0777 8377  .Y.;.28.S....w.w
+00003e20: 6725 57b6 e2b8 b009 2fde 097f 399a 6c0d  g%W...../...9.l.
+00003e30: 140f 2ad3 bdf2 ec43 ea25 52f4 4fde 494b  ..*....C.%R.O.IK
+00003e40: e01f 724c 382a f7fb dd81 8d75 6d35 98a8  ..rL8*.....um5..
+00003e50: 979e a328 b7a2 8d1e 64b2 b0d7 03d7 b560  ...(....d......`
+00003e60: c9a9 f466 4313 bb01 3348 ddd8 3a66 e80e  ...fC...3H..:f..
+00003e70: dfe4 dd54 7726 b6d1 7767 ee0c fb48 f8ff  ...Tw&..wg...H..
+00003e80: 988d dcf6 a96f 9f1b 358e 5903 221f 31ef  .....o..5.Y.".1.
+00003e90: caad b257 36ec 1bbb d647 cd27 62a6 9edd  ...W6....G.'b...
+00003ea0: 1772 ff90 c127 235b e923 4c44 82dc 7fe6  .r...'#[.#LD....
+00003eb0: 7758 6884 8fe4 8f7b 8f41 3ffe e58f f117  wXh....{.A?.....
+00003ec0: a0cc 49f2 5f0b 1fcc 7fbd ed04 f977 e29f  ..I._........w..
+00003ed0: 20ff 23f9 0844 7c78 f1fb 0760 a37c b005   .#..D|x...`.|..
+00003ee0: 482b 07a7 30d0 ea1e c413 7fe7 41b6 d7fe  H+..0.......A...
+00003ef0: af81 5666 8394 ed7f c5f4 0d50 4b01 0214  ..Vf.......PK...
+00003f00: 0014 0000 0008 0087 4ee2 40b2 e551 b69a  ........N.@..Q..
+00003f10: 0100 0098 0800 0013 0000 0000 0000 0001  ................
+00003f20: 0020 0000 0030 3d00 005b 436f 6e74 656e  . ...0=..[Conten
+00003f30: 745f 5479 7065 735d 2e78 6d6c 504b 0102  t_Types].xmlPK..
+00003f40: 1400 0a00 0000 0000 874e e240 0000 0000  .........N.@....
+00003f50: 0000 0000 0000 0000 0600 0000 0000 0000  ................
+00003f60: 0000 1000 0000 2a39 0000 5f72 656c 732f  ......*9.._rels/
+00003f70: 504b 0102 1400 1400 0000 0800 874e e240  PK...........N.@
+00003f80: 0122 221f fd00 0000 e102 0000 0b00 0000  ."".............
+00003f90: 0000 0000 0100 2000 0000 4e39 0000 5f72  ...... ...N9.._r
+00003fa0: 656c 732f 2e72 656c 7350 4b01 0214 000a  els/.relsPK.....
+00003fb0: 0000 0000 0087 4ee2 4000 0000 0000 0000  ......N.@.......
+00003fc0: 0000 0000 000a 0000 0000 0000 0000 0010  ................
+00003fd0: 0000 0032 3300 0063 7573 746f 6d58 6d6c  ...23..customXml
+00003fe0: 2f50 4b01 0214 000a 0000 0000 0087 4ee2  /PK...........N.
+00003ff0: 4000 0000 0000 0000 0000 0000 0010 0000  @...............
+00004000: 0000 0000 0000 0010 0000 0074 3a00 0063  ...........t:..c
+00004010: 7573 746f 6d58 6d6c 2f5f 7265 6c73 2f50  ustomXml/_rels/P
+00004020: 4b01 0214 0014 0000 0008 0087 4ee2 4074  K...........N.@t
+00004030: 3f39 7abc 0000 0028 0100 001e 0000 0000  ?9z....(........
+00004040: 0000 0001 0020 0000 00a2 3a00 0063 7573  ..... ....:..cus
+00004050: 746f 6d58 6d6c 2f5f 7265 6c73 2f69 7465  tomXml/_rels/ite
+00004060: 6d31 2e78 6d6c 2e72 656c 7350 4b01 0214  m1.xml.relsPK...
+00004070: 0014 0000 0008 0087 4ee2 40dc 7f3e cf95  ........N.@..>..
+00004080: 0000 0002 0100 0013 0000 0000 0000 0001  ................
+00004090: 0020 0000 005a 3300 0063 7573 746f 6d58  . ...Z3..customX
+000040a0: 6d6c 2f69 7465 6d31 2e78 6d6c 504b 0102  ml/item1.xmlPK..
+000040b0: 1400 1400 0000 0800 874e e240 6343 7b45  .........N.@cC{E
+000040c0: e500 0000 4701 0000 1800 0000 0000 0000  ....G...........
+000040d0: 0100 2000 0000 2034 0000 6375 7374 6f6d  .. ... 4..custom
+000040e0: 586d 6c2f 6974 656d 5072 6f70 7331 2e78  Xml/itemProps1.x
+000040f0: 6d6c 504b 0102 1400 0a00 0000 0000 874e  mlPK...........N
+00004100: e240 0000 0000 0000 0000 0000 0000 0900  .@..............
+00004110: 0000 0000 0000 0000 1000 0000 0000 0000  ................
+00004120: 646f 6350 726f 7073 2f50 4b01 0214 0014  docProps/PK.....
+00004130: 0000 0008 0087 4ee2 404d d85f e75e 0100  ......N.@M._.^..
+00004140: 0072 0200 0010 0000 0000 0000 0001 0020  .r............. 
+00004150: 0000 0027 0000 0064 6f63 5072 6f70 732f  ...'...docProps/
+00004160: 6170 702e 786d 6c50 4b01 0214 0014 0000  app.xmlPK.......
+00004170: 0008 0087 4ee2 4013 fa0c 9254 0100 007e  ....N.@....T...~
+00004180: 0200 0011 0000 0000 0000 0001 0020 0000  ............. ..
+00004190: 00b3 0100 0064 6f63 5072 6f70 732f 636f  .....docProps/co
+000041a0: 7265 2e78 6d6c 504b 0102 1400 1400 0000  re.xmlPK........
+000041b0: 0800 874e e240 7c52 f707 fe00 0000 7f01  ...N.@|R........
+000041c0: 0000 1300 0000 0000 0000 0100 2000 0000  ............ ...
+000041d0: 3603 0000 646f 6350 726f 7073 2f63 7573  6...docProps/cus
+000041e0: 746f 6d2e 786d 6c50 4b01 0214 000a 0000  tom.xmlPK.......
+000041f0: 0000 0087 4ee2 4000 0000 0000 0000 0000  ....N.@.........
+00004200: 0000 0005 0000 0000 0000 0000 0010 0000  ................
+00004210: 0065 0400 0077 6f72 642f 504b 0102 1400  .e...word/PK....
+00004220: 0a00 0000 0000 874e e240 0000 0000 0000  .......N.@......
+00004230: 0000 0000 0000 0b00 0000 0000 0000 0000  ................
+00004240: 1000 0000 9a3b 0000 776f 7264 2f5f 7265  .....;..word/_re
+00004250: 6c73 2f50 4b01 0214 0014 0000 0008 0087  ls/PK...........
+00004260: 4ee2 40e0 8ea4 be33 0100 0038 0600 001c  N.@....3...8....
+00004270: 0000 0000 0000 0001 0020 0000 00c3 3b00  ......... ....;.
+00004280: 0077 6f72 642f 5f72 656c 732f 646f 6375  .word/_rels/docu
+00004290: 6d65 6e74 2e78 6d6c 2e72 656c 7350 4b01  ment.xml.relsPK.
+000042a0: 0214 0014 0000 0008 0087 4ee2 4081 b4d3  ..........N.@...
+000042b0: 50c4 0200 00e7 0700 0011 0000 0000 0000  P...............
+000042c0: 0001 0020 0000 003f 3000 0077 6f72 642f  ... ...?0..word/
+000042d0: 646f 6375 6d65 6e74 2e78 6d6c 504b 0102  document.xmlPK..
+000042e0: 1400 1400 0000 0800 874e e240 8caf 87ad  .........N.@....
+000042f0: bf03 0000 8412 0000 1200 0000 0000 0000  ................
+00004300: 0100 2000 0000 3b35 0000 776f 7264 2f66  .. ...;5..word/f
+00004310: 6f6e 7454 6162 6c65 2e78 6d6c 504b 0102  ontTable.xmlPK..
+00004320: 1400 1400 0000 0800 874e e240 0b29 7ddf  .........N.@.)}.
+00004330: c401 0000 5105 0000 1000 0000 0000 0000  ....Q...........
+00004340: 0100 2000 0000 0f24 0000 776f 7264 2f66  .. ....$..word/f
+00004350: 6f6f 7465 7231 2e78 6d6c 504b 0102 1400  ooter1.xmlPK....
+00004360: 1400 0000 0800 874e e240 0b29 7ddf c401  .......N.@.)}...
+00004370: 0000 5105 0000 1000 0000 0000 0000 0100  ..Q.............
+00004380: 2000 0000 0126 0000 776f 7264 2f66 6f6f   ....&..word/foo
+00004390: 7465 7232 2e78 6d6c 504b 0102 1400 1400  ter2.xmlPK......
+000043a0: 0000 0800 874e e240 0b29 7ddf c401 0000  .....N.@.)}.....
+000043b0: 5105 0000 1000 0000 0000 0000 0100 2000  Q............. .
+000043c0: 0000 f327 0000 776f 7264 2f66 6f6f 7465  ...'..word/foote
+000043d0: 7233 2e78 6d6c 504b 0102 1400 1400 0000  r3.xmlPK........
+000043e0: 0800 874e e240 7fd1 0bb4 e801 0000 9e05  ...N.@..........
+000043f0: 0000 1000 0000 0000 0000 0100 2000 0000  ............ ...
+00004400: 131e 0000 776f 7264 2f68 6561 6465 7231  ....word/header1
+00004410: 2e78 6d6c 504b 0102 1400 1400 0000 0800  .xmlPK..........
+00004420: 874e e240 963d 9c92 c501 0000 5105 0000  .N.@.=......Q...
+00004430: 1000 0000 0000 0000 0100 2000 0000 2920  .......... ...) 
+00004440: 0000 776f 7264 2f68 6561 6465 7232 2e78  ..word/header2.x
+00004450: 6d6c 504b 0102 1400 1400 0000 0800 874e  mlPK...........N
+00004460: e240 963d 9c92 c501 0000 5105 0000 1000  .@.=......Q.....
+00004470: 0000 0000 0000 0100 2000 0000 1c22 0000  ........ ...."..
+00004480: 776f 7264 2f68 6561 6465 7233 2e78 6d6c  word/header3.xml
+00004490: 504b 0102 1400 1400 0000 0800 874e e240  PK...........N.@
+000044a0: a634 96ed e504 0000 740d 0000 1100 0000  .4......t.......
+000044b0: 0000 0000 0100 2000 0000 ff18 0000 776f  ...... .......wo
+000044c0: 7264 2f73 6574 7469 6e67 732e 786d 6c50  rd/settings.xmlP
+000044d0: 4b01 0214 0014 0000 0008 0087 4ee2 40ae  K...........N.@.
+000044e0: 6484 bf4a 1400 0039 a800 000f 0000 0000  d..J...9........
+000044f0: 0000 0001 0020 0000 0088 0400 0077 6f72  ..... .......wor
+00004500: 642f 7374 796c 6573 2e78 6d6c 504b 0102  d/styles.xmlPK..
+00004510: 1400 0a00 0000 0000 874e e240 0000 0000  .........N.@....
+00004520: 0000 0000 0000 0000 0b00 0000 0000 0000  ................
+00004530: 0000 1000 0000 e529 0000 776f 7264 2f74  .......)..word/t
+00004540: 6865 6d65 2f50 4b01 0214 0014 0000 0008  heme/PK.........
+00004550: 0087 4ee2 40c8 d416 5afe 0500 002c 1900  ..N.@...Z....,..
+00004560: 0015 0000 0000 0000 0001 0020 0000 000e  ........... ....
+00004570: 2a00 0077 6f72 642f 7468 656d 652f 7468  *..word/theme/th
+00004580: 656d 6531 2e78 6d6c 504b 0506 0000 0000  eme1.xmlPK......
+00004590: 1b00 1b00 8d06 0000 fb3e 0000 0000       .........>....
```

## Comparing `tabdoc-1.0.2.dist-info/LICENSE` & `tabdoc-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tabdoc-1.0.2.dist-info/METADATA` & `tabdoc-1.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabdoc
-Version: 1.0.2
+Version: 1.0.3
 Summary: tabular datasets to excel,word,pdf
 Home-page: https://github.com/tinybees/tabdoc
 Author: TinyBees
 Author-email: a598824322@qq.com
 License: MIT
 Keywords: tabular,datasets,excel,word,pdf
 Platform: UNKNOWN
```

## Comparing `tabdoc-1.0.2.dist-info/RECORD` & `tabdoc-1.0.3.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-tabdoc/__init__.py,sha256=qVSCKAJlnhbzHejNw2KlTnqs1duvTogMUpcIb_9j0cM,205
+tabdoc/__init__.py,sha256=LXoOGF8wbXsqHi2lgLX1qoNLzOt88va6ieAvPSQ6CKw,205
 tabdoc/tabexcel.py,sha256=QJwNiRgX_QE8MVs4zgnJVKGPM9ZYYQt7a2cBGPZ9V7I,7681
 tabdoc/tabpdf.py,sha256=bu4aNprhWiWA12Mhz_CtLJBX_KfC6AwmNOaHvNXQ0g8,10330
-tabdoc/tabword.py,sha256=AwCa2x7_kkcDsksSILtEjGW1xPiz8eQiYsdyFPHRmuc,8081
+tabdoc/tabword.py,sha256=Qo9apQgNFEbpvBP3vBw8HaA7G1B6qC-tlcSRuZtnjnk,16014
 tabdoc/templates/SimHei.ttf,sha256=rccIEeST9Ktnzjhw7HH7fosL7jgIsCp9cg7W6A654xA,10063973
 tabdoc/templates/__init__.py,sha256=KWhgTfEXeHp242vVpo5sLjZQv5EKTok52kk2n87PnQ4,112
-tabdoc/templates/template.docx,sha256=z0mn-BicH4AJZD1Sz29clNhADylSjLNmx0pk9UIP6dA,20235
-tabdoc-1.0.2.dist-info/LICENSE,sha256=Zhqbr5LXiWdCR27qxTV0fnscCrUfsMNZmwX7b2YuxrE,1066
-tabdoc-1.0.2.dist-info/METADATA,sha256=4RV5KUJKM3nK_k5waVS7_blXEOMr4dp0zU8Io9apW2o,1272
-tabdoc-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tabdoc-1.0.2.dist-info/top_level.txt,sha256=LC-DKh-j0Rlc6U2wIkElDY4Z_ZOV6GopgaqcDtYgH3s,7
-tabdoc-1.0.2.dist-info/RECORD,,
+tabdoc/templates/template.docx,sha256=2Jk0zRUzNg9HN9srGXmsxDw_N9hStFPhnTcF8C6gnoo,17822
+tabdoc-1.0.3.dist-info/LICENSE,sha256=Zhqbr5LXiWdCR27qxTV0fnscCrUfsMNZmwX7b2YuxrE,1066
+tabdoc-1.0.3.dist-info/METADATA,sha256=jJ_LRY9tfItHOCnynsn_m_TeKaiJQ3lnhbZv48Z2Vtg,1272
+tabdoc-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tabdoc-1.0.3.dist-info/top_level.txt,sha256=LC-DKh-j0Rlc6U2wIkElDY4Z_ZOV6GopgaqcDtYgH3s,7
+tabdoc-1.0.3.dist-info/RECORD,,
```

