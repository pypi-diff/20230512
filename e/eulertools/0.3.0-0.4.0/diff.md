# Comparing `tmp/eulertools-0.3.0.tar.gz` & `tmp/eulertools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulertools-0.3.0.tar", max compression
+gzip compressed data, was "eulertools-0.4.0.tar", max compression
```

## Comparing `eulertools-0.3.0.tar` & `eulertools-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,13 @@
--rw-r--r--   0        0        0     7652 2023-05-09 19:41:34.782813 eulertools-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0      976 2023-05-09 19:41:34.788663 eulertools-0.3.0/README.rst
--rw-r--r--   0        0        0     2694 2023-05-11 15:59:49.025802 eulertools-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-09 19:41:34.789309 eulertools-0.3.0/src/eulertools/__init__.py
--rw-r--r--   0        0        0       22 2023-05-11 15:59:49.013459 eulertools-0.3.0/src/eulertools/__version__.py
--rw-r--r--   0        0        0      793 2023-05-09 19:41:34.789676 eulertools-0.3.0/src/eulertools/benchmark.py
--rw-r--r--   0        0        0     1724 2023-05-11 15:59:14.099647 eulertools-0.3.0/src/eulertools/compare.py
--rw-r--r--   0        0        0     1209 2023-05-11 15:59:14.375119 eulertools-0.3.0/src/eulertools/generate.py
--rw-r--r--   0        0        0     4255 2023-05-11 15:59:14.375397 eulertools-0.3.0/src/eulertools/main.py
--rw-r--r--   0        0        0     2799 2023-05-11 15:59:14.375661 eulertools-0.3.0/src/eulertools/run.py
--rw-r--r--   0        0        0      915 2023-05-09 19:41:34.790517 eulertools-0.3.0/src/eulertools/statement.py
--rw-r--r--   0        0        0     1042 2023-05-11 15:05:17.461116 eulertools-0.3.0/src/eulertools/test.py
--rw-r--r--   0        0        0     1943 2023-05-11 15:05:17.464023 eulertools-0.3.0/src/eulertools/timeit.py
--rw-r--r--   0        0        0      946 2023-05-11 15:05:17.460986 eulertools-0.3.0/src/eulertools/update.py
--rw-r--r--   0        0        0     5654 2023-05-11 15:59:14.099956 eulertools-0.3.0/src/eulertools/utils.py
--rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 eulertools-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-05-09 19:41:34.782813 eulertools-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0      976 2023-05-09 19:41:34.788663 eulertools-0.4.0/README.rst
+-rw-r--r--   0        0        0     2694 2023-05-12 16:47:11.900398 eulertools-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 19:41:34.789309 eulertools-0.4.0/src/eulertools/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-12 16:47:05.636529 eulertools-0.4.0/src/eulertools/__version__.py
+-rw-r--r--   0        0        0     1894 2023-05-12 14:14:39.715719 eulertools-0.4.0/src/eulertools/compare.py
+-rw-r--r--   0        0        0     1219 2023-05-12 16:45:37.573777 eulertools-0.4.0/src/eulertools/generate.py
+-rw-r--r--   0        0        0     3234 2023-05-12 16:45:37.571776 eulertools-0.4.0/src/eulertools/main.py
+-rw-r--r--   0        0        0     2527 2023-05-12 16:45:58.269757 eulertools-0.4.0/src/eulertools/run.py
+-rw-r--r--   0        0        0     1063 2023-05-12 15:13:14.054136 eulertools-0.4.0/src/eulertools/statement.py
+-rw-r--r--   0        0        0     2654 2023-05-12 16:45:37.571618 eulertools-0.4.0/src/eulertools/time.py
+-rw-r--r--   0        0        0     6013 2023-05-12 15:13:20.367496 eulertools-0.4.0/src/eulertools/utils.py
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 eulertools-0.4.0/PKG-INFO
```

### Comparing `eulertools-0.3.0/LICENSE.txt` & `eulertools-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eulertools-0.3.0/README.rst` & `eulertools-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `eulertools-0.3.0/pyproject.toml` & `eulertools-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "eulertools"
-version = "0.3.0"
+version = "0.4.0"
 description = "Multilanguage competitive coding toolbox"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "README.rst"
```

### Comparing `eulertools-0.3.0/src/eulertools/compare.py` & `eulertools-0.4.0/src/eulertools/compare.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,16 @@
         matrix = [
             ["problem", *self.problems],
             *(self.get_language_timings(language) for language in self.languages),
         ]
         self.print_table(self.transpose(matrix))
 
     def print_table(self, matrix: list[list[str]]) -> None:
+        if len(matrix) == 1:
+            raise ValueError("No data to print")
         n = len(self.languages) + 1
         spacing = ["─" * self.pad_length for _ in range(n)]
         top = "┌" + "┬".join(spacing) + "┐"
         mid = "├" + "┼".join(spacing) + "┤"
         btm = "└" + "┴".join(spacing) + "┘"
         print(top)
         for i, row in enumerate(matrix):
@@ -37,13 +39,14 @@
         return [
             language.name,
             *(str(timings.get(problem, "N/A")) for problem in self.problems),
         ]
 
     @staticmethod
     def transpose(matrix: list[list[str]]) -> list[list[str]]:
-        return [list(row) for row in zip(*matrix, strict=True)]
+        new_lines = (list(row) for row in zip(*matrix, strict=True))
+        return [line for line in new_lines if any(item != "N/A" for item in line[1:])]
 
     def padded_print(self, string: str, *, heading: bool) -> str:
         if heading:
             return string.center(self.pad_length)
         return string.rjust(self.pad_length)
```

### Comparing `eulertools-0.3.0/src/eulertools/run.py` & `eulertools-0.4.0/src/eulertools/run.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,70 @@
 import subprocess
-import sys
+from itertools import product
 
-from eulertools.utils import Language, Modes, get_answers_dict, get_solution
+from eulertools.utils import Language, Modes, get_answers, get_solution
 
 
 class Run:
     def __init__(
         self,
-        language: Language,
-        problem: str,
+        languages: list[Language],
+        problems: list[str],
+        verbosity: int,
         *,
-        debug: bool = False,
         times: int = 1,
         mode: str = Modes.RUN,
     ):
-        self.language = language
-        self.problem = problem
+        self.languages = languages
+        self.problems = problems
         self.mode = mode
         self.times = times
-        self.debug = debug
+        self.verbosity = verbosity
 
-    def run(self) -> list[int]:
-        if self.mode == Modes.TIMING and self.times < 3:
-            raise ValueError("Timing mode requires at least 3 runs. Aborting...")
+    def run(self) -> None:
+        for language, problem in product(self.languages, self.problems):
+            self.run_single_problem(language, problem)
 
-        if self.mode != Modes.TIMING and self.times != 1:
-            raise ValueError("Only timing mode supports multiple runs. Aborting...")
-
-        solution = get_solution(self.language, self.problem)
+    def run_single_problem(self, language: Language, problem: str) -> list[int] | None:
+        solution = get_solution(language, problem)
         if not solution.exists():
-            raise FileNotFoundError(
-                f"Problem {self.problem} not solved for {self.language}. Aborting..."
-            )
+            return None
         raw_output = subprocess.run(
-            [  # noqa: S603
-                self.language.runner,
-                self.problem,
-                self.mode,
-                str(self.times),
-            ],
+            [language.runner, problem, self.mode, str(self.times)],  # noqa: S603
             capture_output=True,
         )
         output = raw_output.stdout.decode()
-        if self.debug:
-            sys.tracebacklimit = 9999
+        if self.verbosity > 3:
             print(output)
         timings = [
             int(line[6:]) or 1
             for line in output.splitlines()
             if line.startswith("Time: ")
         ]
-        expected_answers = get_answers_dict(self.problem)
+        expected_answers = get_answers(problem)
         actual_answers: dict[int, str] = {}
-        prefix = "Testing" if self.mode == "test" else "Running"
         for line in output.strip().splitlines():
             if line.startswith("Time: "):
                 continue
             raw_key, value = line.split(maxsplit=1)
             key = int(raw_key[:-1])
             actual_answers[key] = value
         success = True
-        if self.mode == "test" and len(actual_answers) != len(expected_answers):
+        if self.mode != Modes.TIMING and len(actual_answers) != len(expected_answers):
             success = False
-            print(f"🔴 {prefix} {self.problem}...")
+            print(f"🔴 Running {problem}...")
         for key, value in actual_answers.items():
             if key not in expected_answers:
-                if self.mode != "timing":
-                    print(f"🟠 {prefix} {self.problem}/{key}... new response: {value}")
+                if self.mode != Modes.TIMING:
+                    print(
+                        f"🟠 Running {language.name}/{problem}/{key}... new response: {value}"
+                    )
             elif value != expected_answers[key]:
                 success = False
                 print(
-                    f"🔴 {prefix} {self.problem}/{key}... expected: {expected_answers[key]}, got: {value}"
+                    f"🔴 Running {language.name}/{problem}/{key}... expected: {expected_answers[key]}, got: {value}"
                 )
-            elif self.mode != "timing":
-                print(f"🟢 {prefix} {self.problem}/{key}... {value}")
+            elif self.mode != Modes.TIMING:
+                print(f"🟢 Running {language.name}/{problem}/{key}... {value}")
         if not success:
-            raise ValueError(f"{prefix} failed. Aborting...")
+            raise ValueError("Running failed. Aborting...")
         return timings
```

### Comparing `eulertools-0.3.0/src/eulertools/utils.py` & `eulertools-0.4.0/src/eulertools/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import re
-from collections.abc import Iterator
 from dataclasses import dataclass, field
 from decimal import Decimal
 from enum import StrEnum, unique
 from pathlib import Path
 from typing import Any, Self
 
 from dj_settings import SettingsParser
@@ -23,15 +22,14 @@
     WARNING = "\033[33m"
 
 
 @unique
 class Modes(StrEnum):
     TIMING = "timing"
     RUN = "run"
-    TEST = "test"
 
 
 @dataclass(frozen=True, slots=True)
 class Timing:
     time: Decimal
     unit: str
 
@@ -89,50 +87,29 @@
         return cls(
             name=language["name"],
             extension=language["extension"],
             runner=project_root.joinpath(language["runner"]),
         )
 
 
-@dataclass(frozen=True, slots=True)
-class Languages:
-    _all: tuple[Language, ...] = field(repr=False)
-    _data: dict[str, Language] = field(init=False, repr=False)
-
-    def __init__(self, languages: tuple[Language, ...]) -> None:
-        object.__setattr__(self, "_all", languages)
-        object.__setattr__(
-            self, "_data", {language.name: language for language in languages}
-        )
-
-    def __len__(self) -> int:
-        return len(self._all)
-
-    def __iter__(self) -> Iterator[Language]:
-        return iter(self._all)
-
-    def __getitem__(self, item: str) -> Language:
-        return self._data[item]
-
-
 def get_project_root() -> Path:
     cwd = Path.cwd().resolve()
     while not cwd.joinpath("leet.toml").exists():
         if cwd.as_posix() == "/":
             raise RuntimeError("Could not find project root")
         cwd = cwd.parent
     return cwd
 
 
 def get_settings() -> dict[str, Any]:
     return SettingsParser(get_project_root().joinpath("leet.toml")).data
 
 
-def get_answers_dict(problem: str) -> dict[int, str]:
-    answers = get_project_root().joinpath("answers.txt")
+def get_answers(problem: str) -> dict[int, str]:
+    answers = get_project_root().joinpath("common", "answers.txt")
     output: dict[int, str] = {}
     for line in answers.read_text().splitlines():
         if line.startswith(problem):
             problem_part, mode_id, answer = line.split(maxsplit=2)
             output[int(mode_id[:-1])] = answer
     return output
 
@@ -156,35 +133,63 @@
 
 def get_average(values: list[int]) -> float:
     if len(values) >= 3:
         values = sorted(values)[1:-1]
     return sum(values) // len(values)
 
 
-def get_problem(problem: str) -> str:
-    settings = get_settings()
-    problem_format: str = settings["problems"]["format"]
-    return problem_format.format(problem=problem)
+def get_statement(problem: str) -> Path:
+    return get_project_root().joinpath("common", "statements", f"{problem}.txt")
 
 
-def get_statement(problem: str) -> Path:
-    return get_project_root().joinpath("statements", f"{problem}.txt")
+def get_signature(language: Language, problem: str) -> str:
+    statement = get_project_root().joinpath("common", "statements", f"{problem}.txt")
+    with statement.open() as file:
+        for line in file.readlines():
+            if line.startswith(f"::{language.name}::"):
+                return line.split("::")[2].strip()
+
+    return ""
 
 
 def get_template(language: Language) -> Path:
-    return get_project_root().joinpath(
-        "templates", f"template.solution.{language.extension}"
-    )
+    return get_project_root().joinpath(language.name, ".leet", "template")
 
 
 def get_solution(language: Language, problem: str) -> Path:
     return get_project_root().joinpath(
         language.name, "src", "solutions", f"{problem}.{language.extension}"
     )
 
 
-def get_languages() -> Languages:
-    language_settings = get_settings()["languages"]
-    languages = tuple(
-        Language.from_settings(name) for name in sorted(language_settings)
-    )
-    return Languages(languages)
+def get_context(language: Language, problem: str) -> dict[str, str]:
+    signature = get_signature(language, problem)
+    regex_list = get_settings()["languages"][language.name].get("regex", [])
+    context = {"problem": problem}
+    for regex in regex_list:
+        if regex_match := re.search(regex, signature):
+            context |= regex_match.groupdict()
+    return context
+
+
+def get_all_languages() -> list[str]:
+    languages = get_settings()["languages"]
+    return sorted(languages)
+
+
+def get_all_problems() -> list[str]:
+    statement_dir = get_project_root().joinpath("common", "statements")
+    return sorted(file.stem for file in statement_dir.glob("*.txt"))
+
+
+def filter_languages(parsed_languages: list[str]) -> list[Language]:
+    language_strings = get_all_languages()
+    return [
+        Language.from_settings(language)
+        for language in language_strings
+        if language in parsed_languages
+    ]
+
+
+def filter_problems(parsed_problems: list[str]) -> list[str]:
+    problem_strings = get_all_problems()
+    return [problem for problem in problem_strings if problem in parsed_problems]
```

### Comparing `eulertools-0.3.0/PKG-INFO` & `eulertools-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulertools
-Version: 0.3.0
+Version: 0.4.0
 Summary: Multilanguage competitive coding toolbox
 Home-page: https://eulertools.readthedocs.io/en/latest/
 License: LGPL-3.0+
 Keywords: leetcode,topcoder,project_euler
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.11,<4.0
```

