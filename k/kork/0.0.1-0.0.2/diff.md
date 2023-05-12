# Comparing `tmp/kork-0.0.1.tar.gz` & `tmp/kork-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kork-0.0.1.tar", max compression
+gzip compressed data, was "kork-0.0.2.tar", max compression
```

## Comparing `kork-0.0.1.tar` & `kork-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1069 2023-05-04 18:42:42.394496 kork-0.0.1/LICENSE
--rw-r--r--   0        0        0     3490 2023-05-04 18:42:42.394496 kork-0.0.1/README.md
--rw-r--r--   0        0        0      758 2023-05-04 18:42:42.394496 kork-0.0.1/kork/__init__.py
--rw-r--r--   0        0        0     4001 2023-05-04 18:42:42.394496 kork-0.0.1/kork/ast.py
--rw-r--r--   0        0        0     3963 2023-05-04 18:42:42.394496 kork-0.0.1/kork/ast_printer.py
--rw-r--r--   0        0        0    11135 2023-05-05 14:27:01.122055 kork-0.0.1/kork/chain.py
--rw-r--r--   0        0        0     2684 2023-05-04 18:42:42.394496 kork-0.0.1/kork/display.py
--rw-r--r--   0        0        0     2669 2023-05-04 18:42:42.398496 kork-0.0.1/kork/environment.py
--rw-r--r--   0        0        0     4957 2023-05-05 14:27:01.122055 kork-0.0.1/kork/examples.py
--rw-r--r--   0        0        0      516 2023-05-04 18:42:42.398496 kork-0.0.1/kork/exceptions.py
--rw-r--r--   0        0        0     5406 2023-05-04 18:42:42.398496 kork-0.0.1/kork/foreign_funcs.py
--rw-r--r--   0        0        0     5678 2023-05-04 18:42:42.398496 kork-0.0.1/kork/interpreter.py
--rw-r--r--   0        0        0     6848 2023-05-04 18:42:42.398496 kork-0.0.1/kork/parser.py
--rw-r--r--   0        0        0     3019 2023-05-04 18:42:42.398496 kork-0.0.1/kork/prompt_adapter.py
--rw-r--r--   0        0        0        0 2023-05-04 18:42:42.398496 kork-0.0.1/kork/py.typed
--rw-r--r--   0        0        0     2068 2023-05-04 18:42:42.398496 kork-0.0.1/kork/retrieval.py
--rw-r--r--   0        0        0      817 2023-05-05 02:26:47.946876 kork-0.0.1/kork/utils.py
--rw-r--r--   0        0        0      182 2023-05-04 18:42:42.398496 kork-0.0.1/kork/version.py
--rw-r--r--   0        0        0     1810 2023-05-04 18:42:42.398496 kork-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4192 1970-01-01 00:00:00.000000 kork-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-12 14:25:28.959736 kork-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4461 2023-05-12 14:25:28.959736 kork-0.0.2/README.md
+-rw-r--r--   0        0        0      758 2023-05-12 14:25:28.963736 kork-0.0.2/kork/__init__.py
+-rw-r--r--   0        0        0     4051 2023-05-12 14:25:28.963736 kork-0.0.2/kork/ast.py
+-rw-r--r--   0        0        0     4921 2023-05-12 14:25:28.963736 kork-0.0.2/kork/ast_printer.py
+-rw-r--r--   0        0        0    11599 2023-05-12 14:25:28.963736 kork-0.0.2/kork/chain.py
+-rw-r--r--   0        0        0     4115 2023-05-12 14:25:28.963736 kork-0.0.2/kork/display.py
+-rw-r--r--   0        0        0     2858 2023-05-12 14:25:28.963736 kork-0.0.2/kork/environment.py
+-rw-r--r--   0        0        0     4957 2023-05-12 14:25:28.963736 kork-0.0.2/kork/examples.py
+-rw-r--r--   0        0        0      516 2023-05-12 14:25:28.963736 kork-0.0.2/kork/exceptions.py
+-rw-r--r--   0        0        0     5406 2023-05-12 14:25:28.963736 kork-0.0.2/kork/foreign_funcs.py
+-rw-r--r--   0        0        0     5678 2023-05-12 14:25:28.963736 kork-0.0.2/kork/interpreter.py
+-rw-r--r--   0        0        0     6848 2023-05-12 14:25:28.963736 kork-0.0.2/kork/parser.py
+-rw-r--r--   0        0        0     3019 2023-05-12 14:25:28.967736 kork-0.0.2/kork/prompt_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-12 14:25:28.967736 kork-0.0.2/kork/py.typed
+-rw-r--r--   0        0        0     2068 2023-05-12 14:25:28.967736 kork-0.0.2/kork/retrieval.py
+-rw-r--r--   0        0        0      817 2023-05-12 14:25:28.967736 kork-0.0.2/kork/utils.py
+-rw-r--r--   0        0        0      182 2023-05-12 14:25:28.967736 kork-0.0.2/kork/version.py
+-rw-r--r--   0        0        0     1810 2023-05-12 14:25:28.967736 kork-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5257 1970-01-01 00:00:00.000000 kork-0.0.2/setup.py
+-rw-r--r--   0        0        0     5163 1970-01-01 00:00:00.000000 kork-0.0.2/PKG-INFO
```

### Comparing `kork-0.0.1/LICENSE` & `kork-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kork-0.0.1/kork/__init__.py` & `kork-0.0.2/kork/__init__.py`

 * *Files identical despite different names*

### Comparing `kork-0.0.1/kork/ast.py` & `kork-0.0.2/kork/ast.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,18 +27,18 @@
     return snake_case
 
 
 @dataclasses.dataclass(frozen=True)
 class Expr(abc.ABC):
     """Abstract expression."""
 
-    def accept(self, visitor: Visitor) -> Any:
+    def accept(self, visitor: Visitor, **kwargs: Any) -> Any:
         """Accept implementation for a visitor."""
         return getattr(visitor, f"visit_{_to_snake_case(self.__class__.__name__)}")(
-            self
+            self, **kwargs
         )
 
 
 @dataclasses.dataclass(frozen=True)
 class Literal(Expr):
     """A literal expression."""
 
@@ -91,18 +91,18 @@
     elements: Sequence[Expr]
 
 
 @dataclasses.dataclass(frozen=True)
 class Stmt(abc.ABC):
     """Abstract statement."""
 
-    def accept(self, visitor: Visitor) -> Any:
+    def accept(self, visitor: Visitor, **kwargs: Any) -> Any:
         """Accept implementation for a visitor."""
         return getattr(visitor, f"visit_{_to_snake_case(self.__class__.__name__)}")(
-            self
+            self, **kwargs
         )
 
 
 @dataclasses.dataclass(frozen=True)
 class Param(Stmt):
     """Represent a function parameter."""
```

### Comparing `kork-0.0.1/kork/ast_printer.py` & `kork-0.0.2/kork/ast_printer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,140 @@
 import abc
-from typing import Union
+from typing import Any, Union
 
 from kork import ast
 
 
 class AbstractAstPrinter(ast.Visitor, abc.ABC):
     @abc.abstractmethod
-    def visit(self, element: Union[ast.Stmt, ast.Expr]) -> str:
+    def visit(
+        self, element: Union[ast.Stmt, ast.Expr], pretty_print: bool = False
+    ) -> str:
         """Entry-point for printing the AST."""
 
 
 class AstPrinter(AbstractAstPrinter):
     """Default AST Printer implementation."""
 
-    def visit(self, element: Union[ast.Stmt, ast.Expr]) -> str:
+    def visit(
+        self, element: Union[ast.Stmt, ast.Expr], pretty_print: bool = False
+    ) -> str:
         """Entry-point for printing the AST."""
-        return element.accept(self)
+        data = {
+            "call_depth": 0,
+            "pretty_print": pretty_print,
+        }
+        return element.accept(self, **data)
 
-    def visit_program(self, program: ast.Program) -> str:
+    def visit_program(self, program: ast.Program, **data: Any) -> str:
         """Print a program."""
-        return "\n".join(stmt.accept(self) for stmt in program.stmts)
+        return "\n".join(stmt.accept(self, **data) for stmt in program.stmts)
 
     def visit_extern_function_def(
-        self, extern_function_def: ast.ExternFunctionDef
+        self, extern_function_def: ast.ExternFunctionDef, **data: Any
     ) -> str:
         """Print an extern function definition."""
         code = [
             f"extern fn {extern_function_def.name}",
             "(",
-            extern_function_def.params.accept(self),
+            extern_function_def.params.accept(self, **data),
             ")",
             " -> ",
             extern_function_def.return_type,
         ]
 
         if extern_function_def.doc_string:
             # TODO: This is hacky for prototyping, will need to have a better
             # way to represent the doc string.
             doc_string = extern_function_def.doc_string.strip().split("\n")[0]
             code.append(f" // {doc_string}")
 
         return "".join(code)
 
-    def visit_function_call(self, call: ast.FunctionCall) -> str:
+    def visit_function_call(self, call: ast.FunctionCall, **data: Any) -> str:
         """Print a function call."""
-        return f"{call.name}({', '.join(arg.accept(self) for arg in call.args)})"
+        data["call_depth"] += 1
+        if data["pretty_print"]:
+            call_str = f"{call.name}(\n"
+            call_str += ",\n".join(
+                "    " * data["call_depth"] + arg.accept(self, **data)
+                for arg in call.args
+            )
+            call_str += "\n" + "    " * (data["call_depth"] - 1) + ")"
+        else:
+            call_str = (
+                f"{call.name}("
+                f"{', '.join(arg.accept(self, **data) for arg in call.args)}"
+                f")"
+            )
+        return call_str
 
-    def visit_function_def(self, function_def: ast.FunctionDef) -> str:
+    def visit_function_def(self, function_def: ast.FunctionDef, **data: Any) -> str:
         """Print a function definition."""
         signature = [
             f"fn {function_def.name}",
             "(",
-            function_def.params.accept(self),
+            function_def.params.accept(self, **data),
             ")",
             " -> ",
             function_def.return_type,
         ]
 
         code = [" {"]
         for stmt in function_def.body:
-            code.append(stmt.accept(self))
+            code.append(stmt.accept(self, **data))
         code.append("}")
         return "".join(signature) + "\n".join(code)
 
-    def visit_variable(self, variable: ast.Variable) -> str:
+    def visit_variable(self, variable: ast.Variable, **data: Any) -> str:
         """Print a variable."""
         return variable.name
 
-    def visit_var_decl(self, var_decl: ast.VarDecl) -> str:
+    def visit_var_decl(self, var_decl: ast.VarDecl, **data: Any) -> str:
         """Print a variable declaration."""
-        return f"var {var_decl.name} = {var_decl.value.accept(self)}"
+        return f"var {var_decl.name} = {var_decl.value.accept(self, **data)}"
 
-    def visit_assign(self, assign: ast.Assign) -> str:
+    def visit_assign(self, assign: ast.Assign, **data: Any) -> str:
         """Print an assignment."""
-        return f"{assign.name} = {assign.value.accept(self)}"
+        return f"{assign.name} = {assign.value.accept(self, **data)}"
 
-    def visit_literal(self, literal: ast.Literal) -> str:
+    def visit_literal(self, literal: ast.Literal, **data: Any) -> str:
         """Print a literal."""
         value = literal.value
         if isinstance(value, type(None)):
             return "null"
         elif isinstance(value, bool):
             return str(value).lower()
         elif isinstance(value, str):
             return f'"{value}"'
         elif isinstance(value, (float, int)):
             return str(value)
         else:
             raise AssertionError(f"Unknown literal type: {type(value)}")
 
-    def visit_param_list(self, param_list: ast.ParamList) -> str:
+    def visit_param_list(self, param_list: ast.ParamList, **data: Any) -> str:
         """Print a parameter list."""
-        return ", ".join(param.accept(self) for param in param_list.params)
+        return ", ".join(param.accept(self, **data) for param in param_list.params)
 
-    def visit_param(self, param: ast.Param) -> str:
+    def visit_param(self, param: ast.Param, **data: Any) -> str:
         """Print a parameter."""
         return f"{param.name}: {param.type_}"
 
-    def visit_list_(self, list_: ast.List_) -> str:
+    def visit_list_(self, list_: ast.List_, **data: Any) -> str:
         """Print a list."""
-        return f"[{', '.join(element.accept(self) for element in list_.elements)}]"
+        return (
+            f"[{', '.join(element.accept(self, **data) for element in list_.elements)}]"
+        )
 
-    def visit_unary(self, unary: ast.Unary) -> str:
+    def visit_unary(self, unary: ast.Unary, **data: Any) -> str:
         """Visit a unary expression."""
-        return f"{unary.operator}{unary.right.accept(self)}"
+        return f"{unary.operator}{unary.right.accept(self, **data)}"
 
-    def visit_grouping(self, grouping: ast.Grouping) -> str:
-        return f"({grouping.expr.accept(self)})"
+    def visit_grouping(self, grouping: ast.Grouping, **data: Any) -> str:
+        return f"({grouping.expr.accept(self, **data)})"
 
-    def visit_binary(self, binary: ast.Binary) -> str:
+    def visit_binary(self, binary: ast.Binary, **data: Any) -> str:
         """Print a binary expression."""
         return (
-            f"{binary.left.accept(self)} "
-            f"{binary.operator} {binary.right.accept(self)}"
+            f"{binary.left.accept(self, **data)} "
+            f"{binary.operator} {binary.right.accept(self, **data)}"
         )
```

### Comparing `kork-0.0.1/kork/chain.py` & `kork-0.0.2/kork/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Implementation of a programming chain."""
 from __future__ import annotations
 
 from typing import (
+    Any,
     Callable,
     Dict,
     List,
+    Mapping,
     Optional,
     Sequence,
     Tuple,
     TypedDict,
     Union,
     cast,
 )
@@ -141,29 +143,32 @@
     def output_keys(self) -> List[str]:
         """Output keys to return.
 
         :meta private:
         """
         return ["raw", "errors", "code", "environment"]
 
-    def prepare_context(self, query: str) -> Tuple[Environment, FewShotTemplate]:
+    def prepare_context(
+        self, query: str, variables: Optional[Mapping[str, Any]] = None
+    ) -> Tuple[Environment, FewShotTemplate]:
         """Get the pre-populated environment and the few shot template.
 
         Args:
             query: The query to prepare the context for.
+            variables: Any variables that should be added to the context.
 
         Returns:
             The prepopulated environment and a pre-formatted few shot template.
         """
         if self.context_retriever:
             external_function_definitions = self.context_retriever.retrieve(query)
         else:
             external_function_definitions = []
 
-        environment = create_environment(external_function_definitions)
+        environment = create_environment(external_function_definitions, variables)
 
         if self.example_retriever:
             formatted_examples = self.example_retriever.retrieve(query)
         else:
             formatted_examples = []
 
         external_functions = "\n".join(
@@ -206,15 +211,24 @@
     def _call(self, inputs: Dict[str, str]) -> CodeResult:  # type: ignore
         """Call the chain."""
         # Note not using original query!!
         # We remove the leading and trailing whitespace from the query
         # to make things a bit more robust.
         query = inputs[self.input_key].strip()
 
-        environment, few_shot_template = self.prepare_context(query)
+        variables: Mapping[str, Any] = cast(
+            Mapping[str, Any], inputs.get("variables", {})
+        )
+
+        if not isinstance(variables, dict):
+            raise TypeError(
+                f"Variables must be a dictionary, got {type(variables)} instead."
+            )
+
+        environment, few_shot_template = self.prepare_context(query, variables)
 
         chain = LLMChain(
             prompt=few_shot_template,
             llm=self.llm,
         )
 
         formatted_query = format_text(query, self.input_formatter)
```

### Comparing `kork-0.0.1/kork/display.py` & `kork-0.0.2/kork/display.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,61 +1,113 @@
 """Utils for displaying chain results in a notebook."""
+import base64
 import math
 from html import escape
+from io import BytesIO
 from typing import Any, Optional, Sequence, TypedDict, Union
 
+from kork.ast_printer import AstPrinter
 from kork.chain import CodeResult
+from kork.parser import parse  # type: ignore
+
+try:
+    from PIL.Image import Image
+except ImportError:
+    Image = None
+
+
+def image_base64(image: Image) -> str:
+    """Get a base64 representation of an image."""
+    with BytesIO() as buffer:
+        image.save(buffer, "jpeg")
+        return base64.b64encode(buffer.getvalue()).decode()
+
+
+def as_img_tag(image: Image) -> str:
+    """Get an HTML representation of an image."""
+    return f'<img src="data:image/jpeg;base64,{image_base64(image)}">'
 
 
 class HtmlResult(TypedDict):
     """A result that can be displayed in a notebook."""
 
     query: str
     errors: str
     raw: str
     code: str
     result: str
     expected: str
     correct: str
 
 
+class _NoExpectedAnswer:
+    """A sentinel class to indicate that there is no expected answer."""
+
+    pass
+
+
+NO_EXPECTED_ANSWER = _NoExpectedAnswer()
+
+
 def as_html_dict(
     code_result: CodeResult,
     query: Optional[str] = None,
     expected_answer: Optional[Any] = None,
+    result_key: str = "result",
+    pretty_print: bool = True,
 ) -> HtmlResult:
     """Use to generate a dict that can be easily displayed in an IPython notebook."""
-    from IPython.display import Code
+    from IPython import display as ipy_display
 
     code = code_result["code"].strip()
 
+    if pretty_print:
+        code = AstPrinter().visit(parse(code), pretty_print=True)
+    else:
+        code = code
+
     if code:
-        _code = Code(data=code)._repr_html_().strip().replace("\n", "<br/>")
+        _code = ipy_display.Code(data=code)._repr_html_().strip().replace("\n", "<br/>")
     else:
         _code = code
 
     env = code_result["environment"]
 
-    result = env.variables.get("result", "") if env else ""
+    result = env.variables.get(result_key, "") if env else ""
 
-    if isinstance(expected_answer, (float, int)) and isinstance(result, (float, int)):
-        correct = math.isclose(expected_answer, result)
+    if expected_answer is NO_EXPECTED_ANSWER:
+        _correct = "N/A"
     else:
-        correct = bool(expected_answer == result)
+        if isinstance(expected_answer, (float, int)) and isinstance(
+            result, (float, int)
+        ):
+            correct = math.isclose(expected_answer, result)
+        else:
+            correct = bool(expected_answer == result)
+        _correct = "✅" if correct else "⛔"
 
     query = query or code_result.get("query", "")  # type: ignore
 
+    if Image and isinstance(result, Image):
+        _result = as_img_tag(result)
+    else:
+        _result = escape(str(result).strip())
+
+    _expected = (
+        "" if expected_answer is NO_EXPECTED_ANSWER else escape(str(expected_answer))
+    )
+
     return {
         "query": escape(str(query)),
         "errors": escape(str(code_result["errors"])),
         "raw": escape(str(code_result["raw"])).replace("\n", "<br/>"),
         "code": _code,
-        "result": escape(str(result).strip()),
-        "expected": escape(str(expected_answer)),
-        "correct": "✅" if correct else "⛔",
+        "result": _result,
+        "expected": _expected,
+        "correct": _correct,
     }
 
 
 def display_html_results(
     html_results: Union[Sequence[HtmlResult], HtmlResult],
     columns: Optional[Sequence[str]] = None,
 ) -> Any:
@@ -69,24 +121,30 @@
         columns
         if columns
         else ["query", "code", "result", "expected", "correct", "errors", "raw"]
     )
 
     df = pd.DataFrame(_results, columns=_columns)
     if "query" in df.columns:
-        df["query"] = df["query"].str.wrap(30)
+        df["query"] = df["query"].str.wrap(40)
         df["query"] = df["query"].str.replace("\n", "<br/>")
     df = df.style.set_properties(**{"text-align": "left"})
-    return display.HTML(df.to_html(escape=False))
+    return display.HTML(df.to_html(escape=False, index=False))
 
 
 def display_code_result(
     code_result: CodeResult,
     query: Optional[str] = None,
-    expected_answer: Optional[Any] = None,
+    expected_answer: Optional[Any] = NO_EXPECTED_ANSWER,
     columns: Optional[Sequence[str]] = None,
+    result_key: str = "result",
 ) -> Any:
     """Display a code result as a table."""
     return display_html_results(
-        as_html_dict(code_result, query=query, expected_answer=expected_answer),
+        as_html_dict(
+            code_result,
+            query=query,
+            expected_answer=expected_answer,
+            result_key=result_key,
+        ),
         columns=columns,
     )
```

### Comparing `kork-0.0.1/kork/examples.py` & `kork-0.0.2/kork/examples.py`

 * *Files identical despite different names*

### Comparing `kork-0.0.1/kork/exceptions.py` & `kork-0.0.2/kork/exceptions.py`

 * *Files identical despite different names*

### Comparing `kork-0.0.1/kork/foreign_funcs.py` & `kork-0.0.2/kork/foreign_funcs.py`

 * *Files identical despite different names*

### Comparing `kork-0.0.1/kork/interpreter.py` & `kork-0.0.2/kork/interpreter.py`

 * *Files identical despite different names*

### Comparing `kork-0.0.1/kork/parser.py` & `kork-0.0.2/kork/parser.py`

 * *Files identical despite different names*

### Comparing `kork-0.0.1/kork/prompt_adapter.py` & `kork-0.0.2/kork/prompt_adapter.py`

 * *Files identical despite different names*

### Comparing `kork-0.0.1/kork/retrieval.py` & `kork-0.0.2/kork/retrieval.py`

 * *Files identical despite different names*

### Comparing `kork-0.0.1/kork/utils.py` & `kork-0.0.2/kork/utils.py`

 * *Files identical despite different names*

### Comparing `kork-0.0.1/pyproject.toml` & `kork-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kork"
-version = "0.0.1"
+version = "0.0.2"
 description = "Programming with LLMs"
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/langchain-ai/kork"
 
 [tool.poetry.dependencies]
```

