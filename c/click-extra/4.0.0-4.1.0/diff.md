# Comparing `tmp/click_extra-4.0.0.tar.gz` & `tmp/click_extra-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "click_extra-4.0.0.tar", max compression
+gzip compressed data, was "click_extra-4.1.0.tar", max compression
```

## Comparing `click_extra-4.0.0.tar` & `click_extra-4.1.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0     5296 2023-05-08 19:27:41.758221 click_extra-4.0.0/click_extra/__init__.py
--rw-r--r--   0        0        0    22598 2023-05-08 19:27:41.758221 click_extra-4.0.0/click_extra/colorize.py
--rw-r--r--   0        0        0    13795 2023-05-08 19:27:41.758221 click_extra-4.0.0/click_extra/commands.py
--rw-r--r--   0        0        0    29092 2023-05-08 19:27:41.758221 click_extra-4.0.0/click_extra/config.py
--rw-r--r--   0        0        0     3955 2023-05-08 19:27:41.758221 click_extra-4.0.0/click_extra/decorators.py
--rw-r--r--   0        0        0     6380 2023-05-08 19:27:41.758221 click_extra-4.0.0/click_extra/docs_update.py
--rw-r--r--   0        0        0    10968 2023-05-08 19:27:41.758221 click_extra-4.0.0/click_extra/logging.py
--rw-r--r--   0        0        0     4393 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/parameters.py
--rw-r--r--   0        0        0    14729 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/platforms.py
--rw-r--r--   0        0        0        0 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/py.typed
--rw-r--r--   0        0        0     7754 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/pygments.py
--rw-r--r--   0        0        0     4139 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/run.py
--rw-r--r--   0        0        0     5658 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/sphinx.py
--rw-r--r--   0        0        0     5718 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tabulate.py
--rw-r--r--   0        0        0     2534 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/telemetry.py
--rw-r--r--   0        0        0      770 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/__init__.py
--rw-r--r--   0        0        0    14063 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/conftest.py
--rw-r--r--   0        0        0    16720 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/test_colorize.py
--rw-r--r--   0        0        0    13810 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/test_commands.py
--rw-r--r--   0        0        0    20954 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/test_config.py
--rw-r--r--   0        0        0     6955 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/test_logging.py
--rw-r--r--   0        0        0     6412 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/test_parameters.py
--rw-r--r--   0        0        0     9733 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/test_platforms.py
--rw-r--r--   0        0        0     8599 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/test_pygments.py
--rw-r--r--   0        0        0     7062 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/test_run.py
--rw-r--r--   0        0        0    14284 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/test_tabulate.py
--rw-r--r--   0        0        0     3153 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/test_telemetry.py
--rw-r--r--   0        0        0     4585 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/tests/test_version.py
--rw-r--r--   0        0        0     7150 2023-05-08 19:27:41.762221 click_extra-4.0.0/click_extra/version.py
--rw-r--r--   0        0        0     6853 2023-05-08 19:27:41.766221 click_extra-4.0.0/pyproject.toml
--rw-r--r--   0        0        0     5635 2023-05-08 19:27:41.766221 click_extra-4.0.0/readme.md
--rw-r--r--   0        0        0     8734 1970-01-01 00:00:00.000000 click_extra-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     5362 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/__init__.py
+-rw-r--r--   0        0        0    22995 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/colorize.py
+-rw-r--r--   0        0        0    14955 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/commands.py
+-rw-r--r--   0        0        0    29599 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/config.py
+-rw-r--r--   0        0        0     3973 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/decorators.py
+-rw-r--r--   0        0        0     6380 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/docs_update.py
+-rw-r--r--   0        0        0    11543 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/logging.py
+-rw-r--r--   0        0        0     5259 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/parameters.py
+-rw-r--r--   0        0        0    14729 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/platforms.py
+-rw-r--r--   0        0        0        0 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/py.typed
+-rw-r--r--   0        0        0     7754 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/pygments.py
+-rw-r--r--   0        0        0     4139 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/run.py
+-rw-r--r--   0        0        0     5658 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/sphinx.py
+-rw-r--r--   0        0        0     5718 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tabulate.py
+-rw-r--r--   0        0        0     2534 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/telemetry.py
+-rw-r--r--   0        0        0      770 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/__init__.py
+-rw-r--r--   0        0        0    14614 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/conftest.py
+-rw-r--r--   0        0        0    17445 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_colorize.py
+-rw-r--r--   0        0        0    14025 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_commands.py
+-rw-r--r--   0        0        0    21404 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_config.py
+-rw-r--r--   0        0        0     7256 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_logging.py
+-rw-r--r--   0        0        0     7814 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_parameters.py
+-rw-r--r--   0        0        0     9733 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_platforms.py
+-rw-r--r--   0        0        0     8047 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_pygments.py
+-rw-r--r--   0        0        0     7062 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_run.py
+-rw-r--r--   0        0        0    14284 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_tabulate.py
+-rw-r--r--   0        0        0     3153 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_telemetry.py
+-rw-r--r--   0        0        0     3531 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_timer.py
+-rw-r--r--   0        0        0     4585 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/tests/test_version.py
+-rw-r--r--   0        0        0     2385 2023-05-12 06:28:38.571972 click_extra-4.1.0/click_extra/timer.py
+-rw-r--r--   0        0        0     7098 2023-05-12 06:28:38.575971 click_extra-4.1.0/click_extra/version.py
+-rw-r--r--   0        0        0     6924 2023-05-12 06:28:38.579972 click_extra-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6637 2023-05-12 06:28:38.579972 click_extra-4.1.0/readme.md
+-rw-r--r--   0        0        0     9732 1970-01-01 00:00:00.000000 click_extra-4.1.0/PKG-INFO
```

### Comparing `click_extra-4.0.0/click_extra/__init__.py` & `click_extra-4.1.0/click_extra/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Expose package-wide elements."""
 
-__version__ = "4.0.0"
+__version__ = "4.1.0"
 """Examples of valid version strings according :pep:`440#version-scheme`:
 
 .. code-block:: python
 
     __version__ = "1.2.3.dev1"  # Development release 1
     __version__ = "1.2.3a1"  # Alpha Release 1
     __version__ = "1.2.3b1"  # Beta Release 1
@@ -39,28 +39,27 @@
 from .colorize import (  # noqa: I001, E402, F401
     ColorOption,
     HelpExtraFormatter,
     HelpOption,
     HelpExtraTheme,
 )
 from .commands import (  # noqa: I001, E402, F401
-    TimerOption,
     ExtraCommand,
     ExtraContext,
     ExtraGroup,
 )
 from .config import ConfigOption, ShowParamsOption  # noqa: I001, E402, F401
 from .decorators import (  # type: ignore[no-redef] # noqa: I001, E402, F401
     color_option,
     command,  # noqa: E402
     config_option,
     extra_command,
     extra_group,
     group,  # noqa: E402
-    help_option,
+    help_option,  # type: ignore[has-type]
     show_params_option,
     table_format_option,
     telemetry_option,
     timer_option,
     verbosity_option,
     version_option,
 )
@@ -69,14 +68,15 @@
     ExtraLogFormatter,
     ExtraLogHandler,
     extra_basic_config,
 )
 from .parameters import ExtraOption  # noqa: I001, E402, F401
 from .tabulate import TableFormatOption  # noqa: I001, E402, F401
 from .telemetry import TelemetryOption  # noqa: I001, E402, F401
+from .timer import TimerOption  # noqa: I001, E402, F401
 from .version import VersionOption  # noqa: I001, E402, F401
 
 __all__ = [  # noqa: F405
     "Abort",
     "Argument",
     "argument",
     "BadArgumentUsage",
```

### Comparing `click_extra-4.0.0/click_extra/colorize.py` & `click_extra-4.1.0/click_extra/colorize.py`

 * *Files 2% similar despite different names*

```diff
@@ -317,14 +317,16 @@
 
     def collect_keywords(self, ctx):
         """Parse click context to collect option names, choices and metavar keywords."""
         cli_names: set[str] = set()
         subcommands: set[str] = set()
         command_aliases: set[str] = set()
         options: set[str] = set()
+        long_options: set[str] = set()
+        short_options: set[str] = set()
         choices: set[str] = set()
         metavars: set[str] = set()
 
         # Includes CLI base name and its commands.
         cli_names.add(ctx.command_path)
         command = ctx.command
 
@@ -350,20 +352,23 @@
 
             if isinstance(param.type, Choice):
                 choices.update(param.type.choices)
 
             metavars.add(param.make_metavar())
 
         # Split between shorts and long options
-        long_options: set[str] = set()
-        short_options: set[str] = set()
         for option_name in options:
-            # TODO: reuse ctx._opt_prefixes for finer match?
-            # Short options no longer than 2 characters like "-D", "/d", "/?", "+w",
-            # "-w", "f_", "_f", ...)
+            # Short options are no longer than 2 characters like "-D", "/d", "/?",
+            # "+w", "-w", "f_", "_f", ...
+            # XXX We cannot reuse the _short_opts and _long_opts attributes from
+            # https://github.com/pallets/click/blob/b0538df/src/click/parser.py#L173-L182
+            # because their values are not passed when the context is updated like
+            # ctx._opt_prefixes is at:
+            # https://github.com/pallets/click/blob/b0538df/src/click/core.py#L1408 .
+            # So we rely on simple heuristics to guess the option category.
             if len(option_name) <= 2:
                 short_options.add(option_name)
             # Any other is considered a long options. Like: "--debug", "--c", "-otest",
             # "---debug", "-vvvv, "++foo", "/debug", "from_", "_from", ...
             else:
                 long_options.add(option_name)
```

### Comparing `click_extra-4.0.0/click_extra/commands.py` & `click_extra-4.1.0/click_extra/commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,77 +18,30 @@
 Our flavor of commands, groups and context are all subclasses of their vanilla
 counterparts, but are pre-configured with good and common defaults. You can still
 leverage the mixins in here to build up your own custom variants.
 """
 
 from __future__ import annotations
 
-from gettext import gettext as _
-from logging import getLevelName, getLogger
-from time import perf_counter
-from typing import Any, Dict, Sequence, Iterable
+import logging
+from typing import Any, Dict
 
 import click
 import cloup
 
-from . import Command, Group, echo
+from . import Command, Group
 from .colorize import ExtraHelpColorsMixin
-from .parameters import ExtraOption, all_envvars, normalize_envvar
+from .parameters import ExtraOption, all_envvars, normalize_envvar, search_params
 from .colorize import ColorOption, HelpOption
 from .config import ConfigOption, ShowParamsOption
 from .logging import VerbosityOption
+from .timer import TimerOption
 from .version import VersionOption
 
 
-class TimerOption(ExtraOption):
-    """A pre-configured option that is adding a ``--time``/``--no-time`` flag to print
-    elapsed time at the end of CLI execution."""
-
-    def print_timer(self):
-        """Compute and print elapsed execution time."""
-        echo(f"Execution time: {perf_counter() - self.start_time:0.3f} seconds.")
-
-    def register_timer_on_close(self, ctx, param, value):
-        """Callback setting up all timer's machinery.
-
-        Computes and print the execution time at the end of the CLI, if option has been
-        activated.
-        """
-        # Skip timekeeping if option is not active.
-        if not value:
-            return
-
-        # Take timestamp snapshot.
-        self.start_time = perf_counter()
-
-        # Register printing at the end of execution.
-        ctx.call_on_close(self.print_timer)
-
-    def __init__(
-        self,
-        param_decls: Sequence[str] | None = None,
-        default=False,
-        expose_value=False,
-        help=_("Measure and print elapsed execution time."),
-        **kwargs,
-    ):
-        if not param_decls:
-            param_decls = ("--time/--no-time",)
-
-        kwargs.setdefault("callback", self.register_timer_on_close)
-
-        super().__init__(
-            param_decls=param_decls,
-            default=default,
-            expose_value=expose_value,
-            help=help,
-            **kwargs,
-        )
-
-
 class ExtraContext(cloup.Context):
     """Like ``cloup._context.Context``, but with the ability to populate the context's
     ``meta`` property at instanciation."""
 
     _extra_meta: dict[str, Any] = {}
 
     def __init__(self, *args, meta: dict[str, Any] = {}, **kwargs) -> None:
@@ -101,67 +54,66 @@
         """Returns context meta augmented with our own."""
         meta = dict(self._meta)
         meta.update(self._extra_meta)
         return meta
 
 
 def default_extra_params():
-    """Default additional options added to ``extra_command`` and ``extra_group``:
+    """Default additional options added to ``extra_command`` and ``extra_group``.
+
+    .. caution::
+        The order of options has been carefully crafted to handle subtle edge-cases and
+        avoid leaky states in unittests.
+
+        You can still override this hard-coded order for easthetic reasons and it
+        should be fine. Your end-users are unlikely to be affected by these sneaky
+        bugs, as the CLI context is going to be naturraly resetted after each
+        invokation (which is not the case in unitests).
 
     #. ``--time`` / ``--no-time``
-    #. ``--color``, ``--ansi`` / ``--no-color``, ``--no-ansi``
+        .. hint::
+            ``--time`` is placed at the top so all other options can be timed.
     #. ``-C``, ``--config CONFIG_PATH``
+        .. attention::
+            ``--config`` is at the top so it can have a direct influence on the default
+            behavior and value of the other options.
+    #. ``--color``, ``--ansi`` / ``--no-color``, ``--no-ansi``
     #. ``--show-params``
     #. ``-v``, ``--verbosity LEVEL``
     #. ``--version``
     #. ``-h``, ``--help``
 
-    Order is important to let options at the top have influence on those below.
+    .. todo::
+        For bullet-proof handling of edge-cases, we should probably add an indirection
+        layer to have the processing order of options (the one below) different from
+        the presentation order of options in the help screen.
+
+        This is probably something that has been requested in {issue}`544`.
+
+    .. important::
+        Sensitivity to order still remains to be proven. With the code of Click Extra
+        and its dependencies moving fast, there is a non-zero chance that all the
+        options are now sound enough to be re-ordered in a more natural way.
     """
     return [
         TimerOption(),
         ColorOption(),
-        # XXX Should we move config to the top as it might influence other options?
         ConfigOption(),
         ShowParamsOption(),
         VerbosityOption(),
         VersionOption(print_env_info=True),
         HelpOption(),
     ]
 
 
 class ExtraCommand(ExtraHelpColorsMixin, Command):
     """Like ``cloup.command``, with sane defaults and extra help screen colorization."""
 
     context_class: type[cloup.Context] = ExtraContext
 
-    @staticmethod
-    def _search_params(
-        params: Iterable[click.Parameter],
-        klass: type[click.Parameter],
-        unique: bool = True,
-    ) -> list[click.Parameter] | click.Parameter | None:
-        """Search on the command all instances of a parameter and return them.
-
-        :param klass: the class of the parameters to look for.
-        :param unique: if ``True``, raise an error if more than one parameter of the
-            provided ``klass`` is found.
-        """
-        param_list = [p for p in params if isinstance(p, klass)]
-        if not param_list:
-            return None
-        if unique:
-            if len(param_list) != 1:
-                raise RuntimeError(
-                    f"More than one {klass.__name__} parameters found "
-                    f"on command: {param_list}"
-                )
-            return param_list.pop()
-        return param_list
-
     def __init__(
         self,
         *args,
         version: str | None = None,
         extra_option_at_end: bool = True,
         populate_auto_envvars: bool = True,
         **kwargs: Any,
@@ -177,36 +129,78 @@
             The original order of the options is preserved among themselves.
         :param populate_auto_envvars: forces all parameters to have their auto-generated
             environment variables registered. This address the shortcoming of ``click``
             which only evaluates them dynamiccaly. By forcing their registration, the
             auto-generated environment variables gets displayed in the help screen,
             fixing `click#2483 issue <https://github.com/pallets/click/issues/2483>`_.
 
-        By default, these context settings are applied:
+        By default, these `Click context settings
+        <https://click.palletsprojects.com/en/8.1.x/api/#click.Context>`_ are applied:
+
+        - ``auto_envvar_prefix = self.name``
+
+          Auto-generate environment variables for all options, using the command ID as
+          prefix. The prefix is normalized to be uppercased and all non-alphanumerics
+          replaced by underscores.
 
-        - ``show_default = True``: `show all default values
+        - ``help_option_names = ("--help", "-h")``
+
+          `Allow help screen to be invoked with either --help or -h options
+          <https://click.palletsprojects.com/en/8.1.x/documentation/#help-parameter-customization>`_.
+
+        - ``show_default = True``
+
+          `Show all default values
           <https://click.palletsprojects.com/en/8.1.x/api/#click.Context.show_default>`_
           in help screen.
 
-        - ``auto_envvar_prefix = self.name``: auto-generate environment variables for
-          all options, using the command ID as prefix.
+        Additionnaly, these `Cloup context settings
+        <https://cloup.readthedocs.io/en/stable/pages/formatting.html#formatting-settings>`_
+        are set:
+
+        - ``align_option_groups = False`` (*Cloup feature*)
 
-        - ``align_option_groups = False``: `align option groups in help screen
+          `Aligns option groups in help screen
           <https://cloup.readthedocs.io/en/stable/pages/option-groups.html#aligned-vs-non-aligned-groups>`_.
 
-        - ``show_constraints = True``: `show all constraints in help screen
+        - ``show_constraints = True`` (*Cloup feature*)
+
+          `Show all constraints in help screen
           <https://cloup.readthedocs.io/en/stable/pages/constraints.html#the-constraint-decorator>`_.
 
-        - ``show_subcommand_aliases = True``: `show all subcommand aliases in help
-          screen
+        - ``show_subcommand_aliases = True`` (*Cloup feature*)
+
+          `Show all subcommand aliases in help screen
           <https://cloup.readthedocs.io/en/stable/pages/aliases.html?highlight=show_subcommand_aliases#help-output-of-the-group>`_.
 
-        - ``help_option_names = ("--help", "-h")``: `allow help screen to be invoked
-          with either --help or -h options
-          <https://click.palletsprojects.com/en/8.1.x/documentation/#help-parameter-customization>`_.
+        Click Extra also adds its own ``context_settings``:
+
+        - ``show_choices = None`` (*Click Extra feature*)
+
+          If set to ``True`` or ``False``, will force that value on all options, so we
+          can globally show or hide choices when prompting a user for input. Only makes
+          sense for options whose ``prompt`` property is set.
+
+          Defaults to ``None``, which will leave all options untouched, and let them
+          decide of their own ``show_choices`` setting.
+
+        - ``show_envvar = None`` (*Click Extra feature*)
+
+          If set to ``True`` or ``False``, will force that value on all options, so we
+          can globally enable or disable the display of environment variables in help
+          screen.
+
+          Defaults to ``None``, which will leave all options untouched, and let them
+          decide of their own ``show_envvar`` setting. The rationale being that
+          discoverability of environment variables is enabled by the ``--show-params``
+          option, which is active by default on extra commands. So there is no need to
+          surcharge the help screen.
+
+          This addresses the
+          `click#2313 issue <https://github.com/pallets/click/issues/2313>`_.
 
         To override these defaults, you can pass your own settings with the
         ``context_settings`` parameter:
 
         .. code-block:: python
 
             @extra_command(
@@ -214,42 +208,57 @@
                     "show_default": False,
                     ...
                 }
             )
         """
         super().__init__(*args, **kwargs)
 
-        # TODO: implements:
-        # self.show_all_default = show_default
-        # self.show_all_choices = show_choices
-        # self.show_all_envvar = show_envvar =>
-        # https://github.com/pallets/click/issues/2313
+        # List of additional global settings for options.
+        extra_option_settings = ["show_choices", "show_envvar"]
 
         default_ctx_settings: Dict[str, Any] = {
-            "show_default": True,
+            # Click settings:
             # "default_map": {"verbosity": "DEBUG"},
+            "help_option_names": ("--help", "-h"),
+            "show_default": True,
+            # Cloup settings:
             "align_option_groups": False,
             "show_constraints": True,
             "show_subcommand_aliases": True,
-            "help_option_names": ("--help", "-h"),
+            # Click Extra settings:
+            "show_choices": None,
+            "show_envvar": None,
         }
 
+        # Generate environment variables for all options based on the command name.
         if self.name:
             default_ctx_settings["auto_envvar_prefix"] = normalize_envvar(self.name)
 
-        # Fill-in the unset settings with our defaults.
+        # Merge defaults and user settings.
         default_ctx_settings.update(self.context_settings)
+
+        # If set, force extra settings on all options.
+        for setting in extra_option_settings:
+            if default_ctx_settings[setting] is not None:
+                for param in self.params:
+                    # These attributes are specific to options.
+                    if isinstance(param, click.Option):
+                        param.show_envvar = default_ctx_settings[setting]
+
+        # Remove Click Extra-specific settings, before passing it to Cloup and Click.
+        for setting in extra_option_settings:
+            del default_ctx_settings[setting]
         self.context_settings: Dict[str, Any] = default_ctx_settings
 
         if populate_auto_envvars:
             for param in self.params:
                 param.envvar = all_envvars(param, self.context_settings)
 
         if version:
-            version_param = self._search_params(self.params, VersionOption)
+            version_param = search_params(self.params, VersionOption)
             if version_param:
                 version_param.version = version  # type: ignore[union-attr]
 
         if extra_option_at_end:
             self.params.sort(key=lambda p: isinstance(p, ExtraOption))
 
         # Forces re-identification of grouped and non-grouped options as we re-ordered
@@ -295,24 +304,24 @@
         """Main execution of the command, just after the context has been instantiated
         in ``main()``.
 
         If an instance of ``VersionOption`` has been setup on the command, adds to the
         normal execution flow the output of ``--version`` in ``DEBUG`` logs. This
         facilitates troubleshooting of user's issues.
         """
-        logger = getLogger("click_extra")
-        if getLevelName(logger.level) == "DEBUG":
+        logger = logging.getLogger("click_extra")
+        if logger.getEffectiveLevel() == logging.DEBUG:
             # Look for our custom version parameter.
-            version_param = self._search_params(ctx.command.params, VersionOption)
+            version_param = search_params(ctx.command.params, VersionOption)
             if version_param:
                 version_message = version_param.callback(
                     ctx, version_param, True, capture_output=True
                 )
                 for line in version_message.splitlines():
-                    # TODO: pretty print JSON output (easier to read in bug reports).
+                    # TODO: pretty print JSON output (easier to read in bug reports)?
                     logger.debug(line)
 
         return super().invoke(ctx)
 
 
 class ExtraGroup(ExtraCommand, Group):
     """Same as ``cloup.group``, but with sane defaults and extra help screen
```

### Comparing `click_extra-4.0.0/click_extra/config.py` & `click_extra-4.1.0/click_extra/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 import os
 import sys
 from collections.abc import MutableMapping
 from configparser import ConfigParser, ExtendedInterpolation
 from enum import Enum
 from functools import reduce
-from logging import getLogger
+import logging
 from gettext import gettext as _
 from operator import getitem, methodcaller
 from pathlib import Path
 from typing import Any, Iterable, Sequence
 from unittest.mock import patch
 from functools import cached_property
 
@@ -73,15 +73,15 @@
     Style,
     Tuple,
     echo,
     get_app_dir,
     get_current_context,
 )
 from .colorize import KO, OK, default_theme
-from .parameters import ExtraOption, all_envvars
+from .parameters import ExtraOption, all_envvars, search_params
 from .platforms import is_windows
 
 
 class Formats(Enum):
     """Supported configuration formats and the list of their default extensions.
 
     The default order set the priority by which each format is searched for the default
@@ -445,15 +445,15 @@
 
         ``pattern`` is considered as an URL only if it is parseable as such and starts
         with ``http://`` or ``https://``.
 
         Returns an iterator of raw content for each file/URL matching the
         pattern.
         """
-        logger = getLogger("click_extra")
+        logger = logging.getLogger("click_extra")
 
         # Check if the pattern is an URL.
         location = URL(pattern)
         if location and location.scheme.lower() in ("http", "https"):
             logger.debug("Fetch configuration from remote URL.")
             with requests.get(location) as response:
                 if response.ok:
@@ -484,15 +484,15 @@
 
         A successful parsing in any format is supposed to return a ``dict``. Any other
         result, including any raised exception, is considered a failure and the next
         format is tried.
         """
         user_conf = None
         for conf_format in self.formats:
-            logger = getLogger("click_extra")
+            logger = logging.getLogger("click_extra")
             logger.debug(f"Parse configuration as {conf_format.name}...")
 
             try:
                 if conf_format == Formats.TOML:
                     user_conf = tomllib.loads(conf_content)
 
                 elif conf_format == Formats.YAML:
@@ -623,15 +623,15 @@
         User configuration is
         `merged to the context default_map as Click does <https://click.palletsprojects.com/en/8.1.x/commands/#context-defaults>`_.
         
         This allow user's config to only overrides defaults. Values sets from direct
         command line parameters, environment variables or interactive prompts, takes
         precedence over any values from the config file.
         """
-        logger = getLogger("click_extra")
+        logger = logging.getLogger("click_extra")
 
         explicit_conf = ctx.get_parameter_source("config") in (
             ParameterSource.COMMANDLINE,
             ParameterSource.ENVIRONMENT,
             ParameterSource.PROMPT,
         )
         # Always print a message if the user explicitly set the configuration location.
@@ -725,26 +725,27 @@
 
     def print_params(self, ctx, param, value):
         """Introspects current CLI and list its parameters and metadata.
 
         .. important::
             Click doesn't keep a list of all parsed arguments and their origin.
             So we need to emulate here what's happening during CLI invokation.
-            But can't even to that because the raw, pre-parsed arguments are
-            not available anywhere.
+
+            Unfortunately we cannot even do that because the raw, pre-parsed arguments
+            are not available anywhere within Click's internals.
 
             Our workaround consist in leveraging our custom
             ``ExtraCommand``/``ExtraGroup`` classes, in which we are attaching
             a ``click_extra.raw_args`` metadata entry to the context.
         """
         # Exit early if the callback was processed but the option wasn't set.
         if not value:
             return
 
-        logger = getLogger("click_extra")
+        logger = logging.getLogger("click_extra")
 
         if "click_extra.raw_args" in ctx.meta:
             raw_args = ctx.meta.get("click_extra.raw_args", [])
             logger.debug(f"click_extra.raw_args: {raw_args}")
 
             # Mimics click.core.Command.parse_args() so we can produce the list of
             # parsed options values.
@@ -768,31 +769,42 @@
             def vanilla_getter(param):
                 param_value = None
                 source = ctx.get_parameter_source(param.name)
                 return param_value, source
 
             get_param_value = vanilla_getter
 
+        # Inspect the CLI to search for any --config option.
+        config_option = search_params(ctx.command.params, ConfigOption)
+
         table = []
         for path, param_type in self.flatten_tree_dict(self.params_types).items():
             # Get the parameter instance.
             tree_keys = path.split(self.SEP)
             param = self.get_tree_value(self.params_objects, *tree_keys)
             assert param.name == tree_keys[-1]
 
             param_value, source = get_param_value(param)
             param_class = self.get_tree_value(self.params_objects, *tree_keys).__class__
             param_spec = param.get_help_record(ctx)[0]
 
+            # Check if the parameter is allowed in the configuration file.
+            allowed_in_conf = None
+            if config_option:
+                if path in config_option.exclude_params:
+                    allowed_in_conf = KO
+                else:
+                    allowed_in_conf = OK
+
             line = (
                 default_theme.invoked_command(path),
                 f"{param_class.__module__}.{param_class.__qualname__}",
                 param_spec,
                 param_type.__name__,
-                None,  # XXX TODO
+                allowed_in_conf,
                 OK if param.expose_value is True else KO,
                 ", ".join(all_envvars(param, ctx)),
                 param.get_default(ctx),
                 param_value,
                 source._name_ if source else None,
             )
             table.append(line)
```

### Comparing `click_extra-4.0.0/click_extra/decorators.py` & `click_extra-4.1.0/click_extra/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,19 +16,20 @@
 """Decorators for group, commands and options."""
 
 from functools import wraps
 
 import cloup
 
 from .colorize import ColorOption, HelpOption
-from .commands import ExtraCommand, ExtraGroup, TimerOption, default_extra_params
+from .commands import ExtraCommand, ExtraGroup, default_extra_params
 from .config import ConfigOption, ShowParamsOption
 from .logging import VerbosityOption
 from .tabulate import TableFormatOption
 from .telemetry import TelemetryOption
+from .timer import TimerOption
 from .version import VersionOption
 
 
 def allow_missing_parenthesis(dec_factory):
     """Allow to use decorators with or without parenthesis.
 
     As proposed in
```

### Comparing `click_extra-4.0.0/click_extra/docs_update.py` & `click_extra-4.1.0/click_extra/docs_update.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/logging.py` & `click_extra-4.1.0/click_extra/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,76 +14,110 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 """Logging utilities."""
 
 from __future__ import annotations
 
 import logging
+from logging import (
+    Logger,
+    WARNING,
+    _levelToName,
+    Formatter,
+    Handler,
+    LogRecord,
+)
 import sys
 from collections.abc import Generator, Iterable, Sequence
 from gettext import gettext as _
 from typing import Literal, TypeVar
 
 import click
 
 from . import Choice
 from .colorize import default_theme
 from .parameters import ExtraOption
 
+
+_original_get_logger = logging.getLogger
+
+
+def _patched_get_logger(name: str | None = None) -> Logger:
+    """Patch ``logging.getLogger`` to return the right root logger object.
+
+    .. warning::
+        This is a bugfix for Python 3.8 and earlier for which the ``root`` logger
+        cannot be fetched with its plain ``root`` name.
+
+        See:
+        - `cpython#81923 <https://github.com/python/cpython/issues/81923>`_
+        - `cpython@cb65b3a <https://github.com/python/cpython/commit/cb65b3a>`_
+    """
+    if name == "root":
+        name = None
+    return _original_get_logger(name)
+
+
+if sys.version_info < (3, 9):
+    logging.getLogger = _patched_get_logger
+
+
 LOG_LEVELS: dict[str, int] = {
     name: value
-    for value, name in sorted(logging._levelToName.items(), reverse=True)
+    for value, name in sorted(_levelToName.items(), reverse=True)
     if name != "NOTSET"
 }
 """Mapping of canonical log level names to their IDs.
 
 Sorted from lowest to highest verbosity.
 
 Are ignored:
 
 - ``NOTSET``, which is considered internal
 - ``WARN``, which `is obsolete
   <https://docs.python.org/3/library/logging.html?highlight=warn#logging.Logger.warning>`_
-- ``FATAL``, which `has been deprecated
+- ``FATAL``, which `shouldn't be used <https://github.com/python/cpython/issues/85013>`_
+  and `replaced by CRITICAL
   <https://github.com/python/cpython/blob/0df7c3a/Lib/logging/__init__.py#L1538-L1541>`_
-  in favor of ``CRITICAL``
 """
 
 
-DEFAULT_LEVEL: int = logging.WARNING
+DEFAULT_LEVEL: int = WARNING
+DEFAULT_LEVEL_NAME: str = _levelToName[DEFAULT_LEVEL]
 """``WARNING`` is the default level we expect any loggers to starts their lives at.
 
 ``WARNING`` has been chosen as it is `the level at which the default Python's global
 root logger is set up
 <https://github.com/python/cpython/blob/0df7c3a/Lib/logging/__init__.py#L1945>`_.
 
 This value is also used as the default level of the ``--verbosity`` option below.
 """
 
 
-Formatter = TypeVar("Formatter", bound=logging.Formatter)
-Handler = TypeVar("Handler", bound=logging.Handler)
+TFormatter = TypeVar("TFormatter", bound=Formatter)
+THandler = TypeVar("THandler", bound=Handler)
+"""Custom types to be used in type hints below."""
 
 
-class ExtraLogHandler(logging.Handler):
+class ExtraLogHandler(Handler):
     """A handler to output logs to console's ``<stderr>``."""
 
-    def emit(self, record: logging.LogRecord) -> None:
+    def emit(self, record: LogRecord) -> None:
         """Use ``click.echo`` to print to ``<stderr>`` and supports colors."""
         try:
             msg = self.format(record)
             click.echo(msg, err=True)
 
         # If exception occurs format it to the stream.
         except Exception:
             self.handleError(record)
 
 
-class ExtraLogFormatter(logging.Formatter):
-    def formatMessage(self, record: logging.LogRecord) -> str:
+class ExtraLogFormatter(Formatter):
+    def formatMessage(self, record: LogRecord) -> str:
         """Colorize the record's log level name before calling the strandard
         formatter."""
         level = record.levelname.lower()
         level_style = getattr(default_theme, level, None)
         if level_style:
             record.levelname = level_style(level)
         return super().formatMessage(record)
@@ -91,19 +125,19 @@
 
 def extra_basic_config(
     logger_name: str | None = None,
     format: str | None = "{levelname}: {message}",
     datefmt: str | None = None,
     style: Literal["%", "{", "$"] = "{",
     level: int | None = None,
-    handlers: Iterable[logging.Handler] | None = None,
+    handlers: Iterable[Handler] | None = None,
     force: bool = True,
-    handler_class: type[Handler] = ExtraLogHandler,  # type: ignore[assignment]
-    formatter_class: type[Formatter] = ExtraLogFormatter,  # type: ignore[assignment]
-) -> logging.Logger:
+    handler_class: type[THandler] = ExtraLogHandler,  # type: ignore[assignment]
+    formatter_class: type[TFormatter] = ExtraLogFormatter,  # type: ignore[assignment]
+) -> Logger:
     """Setup and configure a logger.
 
     Reimplements `logging.basicConfig
     <https://docs.python.org/3/library/logging.html?highlight=basicconfig#logging.basicConfig>`_,
     but with sane defaults and more parameters.
 
     :param logger_name: ID of the logger to setup. If ``None``, Python's ``root``
@@ -184,58 +218,56 @@
     This will be provided to
     `logging.getLogger <https://docs.python.org/3/library/logging.html?highlight=getlogger#logging.getLogger>`_
     method to fetch the logger object, and as such, can be a dot-separated string to
     build hierarchical loggers.
     """
 
     @property
-    def all_loggers(self) -> Generator[logging.Logger, None, None]:
+    def all_loggers(self) -> Generator[Logger, None, None]:
         """Returns the list of logger IDs affected by the verbosity option.
 
-        Will returns the option's logger and Click Extra's internal logger, so we'll
-        have the level of these two aligned.
+        Will returns Click Extra's internal logger first, then the option's custom
+        logger.
         """
-        for name in (self.logger_name, "click_extra"):
-            # XXX This is a bug for Python 3.8 and earlier for which the ``root``
-            # logger cannot be fetch with its ``"root"`` name: See:
-            #   https://github.com/python/cpython/issues/81923
-            #   https://github.com/python/cpython/commit/cb65b3a4f484ce71dcb76a918af98c7015513025
-            if sys.version_info < (3, 9) and name == "root":
-                yield logging.getLogger()
+        for name in ("click_extra", self.logger_name):
             yield logging.getLogger(name)
 
     def reset_loggers(self):
         """Forces all loggers managed by the option to be reset to the default level.
 
+        Reset loggers in reverse order to ensure the internal logger is reset last.
+
         .. danger::
             Resseting loggers is extremely important for unittests. Because they're
             global, loggers have tendency to leak and pollute their state between
             multiple test calls.
         """
-        for logger in self.all_loggers:
+        for logger in list(self.all_loggers)[::-1]:
+            logging.getLogger("click_extra").debug(
+                f"Reset {logger} to {DEFAULT_LEVEL_NAME}."
+            )
             logger.setLevel(DEFAULT_LEVEL)
 
     def set_levels(self, ctx, param, value):
         """Set level of all loggers configured on the option.
 
         Also prints the chosen value as a debug message via the internal
         ``click_extra`` logger.
         """
         for logger in self.all_loggers:
             logger.setLevel(LOG_LEVELS[value])
-            if logger.name == "click_extra":
-                logger.debug(f"Verbosity set to {value}.")
+            logging.getLogger("click_extra").debug(f"Set {logger} to {value}.")
 
         ctx.call_on_close(self.reset_loggers)
 
     def __init__(
         self,
         param_decls: Sequence[str] | None = None,
-        default_logger: logging.Logger | str | None = None,
-        default: str = logging._levelToName[DEFAULT_LEVEL],
+        default_logger: Logger | str | None = None,
+        default: str = DEFAULT_LEVEL_NAME,
         metavar="LEVEL",
         type=Choice(LOG_LEVELS, case_sensitive=False),  # type: ignore[arg-type]
         expose_value=False,
         help=_("Either {log_levels}.").format(log_levels=", ".join(LOG_LEVELS)),
         is_eager=True,
         **kwargs,
     ) -> None:
@@ -253,15 +285,15 @@
             Write more documentation to detail in which case the user is responsible
             for setting up the logger, and when ``extra_basic_config`` is used.
         """
         if not param_decls:
             param_decls = ("--verbosity", "-v")
 
         # Use the provided logger instance as-is.
-        if isinstance(default_logger, logging.Logger):
+        if isinstance(default_logger, Logger):
             logger = default_logger
         # If a string is provided, use it as the logger name.
         elif isinstance(default_logger, str):
             logger = logging.getLogger(default_logger)
         # ``None`` will produce a default root logger.
         else:
             logger = extra_basic_config(default_logger)
```

### Comparing `click_extra-4.0.0/click_extra/parameters.py` & `click_extra-4.1.0/click_extra/parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 Also implements environment variable utilities.
 """
 
 from __future__ import annotations
 
 import re
-from typing import Any, Dict, Sequence
+from typing import Any, Dict, Sequence, Iterable
 
 import click
 from boltons.iterutils import unique
 
 from . import Option
 
 
@@ -117,7 +117,32 @@
 class ExtraOption(Option):
     """All new options implemented by ``click-extra`` derives from this class.
 
     Does nothing in particular for now but provides a way to identify click-extra's own
     options with certainty. Might be used in the future to implement common behavior,
     fixes or hacks.
     """
+
+
+def search_params(
+    params: Iterable[click.Parameter],
+    klass: type[click.Parameter],
+    unique: bool = True,
+) -> list[click.Parameter] | click.Parameter | None:
+    """Search a particular class of parameter in a list and return them.
+
+    :param params: list of parameter instances to search in.
+    :param klass: the class of the parameters to look for.
+    :param unique: if ``True``, raise an error if more than one parameter of the
+        provided ``klass`` is found.
+    """
+    param_list = [p for p in params if isinstance(p, klass)]
+    if not param_list:
+        return None
+    if unique:
+        if len(param_list) != 1:
+            raise RuntimeError(
+                f"More than one {klass.__name__} parameters found "
+                f"on command: {param_list}"
+            )
+        return param_list.pop()
+    return param_list
```

### Comparing `click_extra-4.0.0/click_extra/platforms.py` & `click_extra-4.1.0/click_extra/platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/pygments.py` & `click_extra-4.1.0/click_extra/pygments.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/run.py` & `click_extra-4.1.0/click_extra/run.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/sphinx.py` & `click_extra-4.1.0/click_extra/sphinx.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/tabulate.py` & `click_extra-4.1.0/click_extra/tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/telemetry.py` & `click_extra-4.1.0/click_extra/telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/tests/__init__.py` & `click_extra-4.1.0/click_extra/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/tests/conftest.py` & `click_extra-4.1.0/click_extra/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -373,29 +373,41 @@
     r"\x1b\[0m\x1b\[35mWARNING\x1b\[0m\x1b\[90m\]\x1b\[0m\n"
     r"  \x1b\[36m--version\x1b\[0m                 Show the version and exit.\n"
     r"  \x1b\[36m-h\x1b\[0m, \x1b\[36m--help\x1b\[0m"
     r"                Show this message and exit.\n"
 )
 
 
-default_debug_uncolored_log = (
-    r"debug: Verbosity set to DEBUG.\n"
+default_debug_uncolored_log_start = (
+    r"debug: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
+    r"debug: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
     r"debug: Load configuration matching .+\*\.{toml,yaml,yml,json,ini,xml}\n"
     r"debug: Pattern is not an URL.\n"
     r"debug: Search local file system.\n"
     r"debug: No configuration file found.\n"
     r"debug: \S+, version \S+\n"
     r"debug: {.*}\n"
 )
 
+default_debug_uncolored_log_end = (
+    r"debug: Reset <RootLogger root \(DEBUG\)> to WARNING.\n"
+    r"debug: Reset <Logger click_extra \(DEBUG\)> to WARNING.\n"
+)
+
 
-default_debug_colored_log = (
-    r"\x1b\[34mdebug\x1b\[0m: Verbosity set to DEBUG.\n"
+default_debug_colored_log_start = (
+    r"\x1b\[34mdebug\x1b\[0m: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
+    r"\x1b\[34mdebug\x1b\[0m: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
     r"\x1b\[34mdebug\x1b\[0m: Load configuration"
     r" matching .+\*\.{toml,yaml,yml,json,ini,xml}\n"
     r"\x1b\[34mdebug\x1b\[0m: Pattern is not an URL.\n"
     r"\x1b\[34mdebug\x1b\[0m: Search local file system.\n"
     r"\x1b\[34mdebug\x1b\[0m: No configuration file found.\n"
     r"\x1b\[34mdebug\x1b\[0m: \x1b\[97m\S+\x1b\[0m,"
     r" version \x1b\[32m\S+\x1b\[0m(\x1b\[90m)?\n"
     r"\x1b\[34mdebug\x1b\[0m: {.*}\x1b\[0m\n"
 )
+
+default_debug_colored_log_end = (
+    r"\x1b\[34mdebug\x1b\[0m: Reset <RootLogger root \(DEBUG\)> to WARNING.\n"
+    r"\x1b\[34mdebug\x1b\[0m: Reset <Logger click_extra \(DEBUG\)> to WARNING.\n"
+)
```

### Comparing `click_extra-4.0.0/click_extra/tests/test_colorize.py` & `click_extra-4.1.0/click_extra/tests/test_colorize.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,16 +39,18 @@
     extra_group,
     help_option,
     verbosity_option,
 )
 from ..logging import LOG_LEVELS
 from .conftest import (
     command_decorators,
-    default_debug_colored_log,
-    default_debug_uncolored_log,
+    default_debug_colored_log_start,
+    default_debug_colored_log_end,
+    default_debug_uncolored_log_start,
+    default_debug_uncolored_log_end,
     default_options_colored_help,
     skip_windows_colors,
 )
 
 
 def test_theme_definition():
     """Ensure we do not leave any property we would have inherited from cloup and
@@ -282,28 +284,40 @@
         assert result.stdout == (
             "\x1b[33mIt works!\x1b[0m\n"
             "\x1b[0m\x1b[1;36mArt\x1b[46;34m\x1b[0m\n"
             "\x1b[35mRun command.\x1b[0m\n"
             "\x1b[34mprint() bypass Click.\x1b[0m\n"
             "\x1b[32mDone.\x1b[0m\n"
         )
-        assert result.stderr == (
-            "\x1b[34mdebug\x1b[0m: Verbosity set to DEBUG.\n"
-            "\x1b[33mwarning\x1b[0m: Processing...\n"
+        assert re.fullmatch(
+            (
+                r"\x1b\[34mdebug\x1b\[0m: "
+                r"Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
+                r"\x1b\[34mdebug\x1b\[0m: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
+                r"\x1b\[33mwarning\x1b\[0m: Processing...\n"
+                rf"{default_debug_colored_log_end}"
+            ),
+            result.stderr,
         )
     else:
         assert result.stdout == (
             "It works!\n"
             "Art\n"
             "Run command.\n"
             "\x1b[34mprint() bypass Click.\x1b[0m\n"
             "Done.\n"
         )
-        assert result.stderr == (
-            "debug: Verbosity set to DEBUG.\nwarning: Processing...\n"
+        assert re.fullmatch(
+            (
+                r"debug: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
+                r"debug: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
+                rf"warning: Processing\.\.\.\n"
+                rf"{default_debug_uncolored_log_end}"
+            ),
+            result.stderr,
         )
 
 
 @skip_windows_colors
 @pytest.mark.parametrize(
     "env, env_expect_colors",
     (
@@ -390,30 +404,35 @@
             "\x1b[0m\x1b[1;36mArt\x1b[46;34m\x1b[0m\n"
             "\x1b[35mRun command #1.\x1b[0m\n"
             "\x1b[34mprint() bypass Click.\x1b[0m\n"
             "\x1b[32mDone.\x1b[0m\n"
         )
         assert re.fullmatch(
             (
-                rf"{default_debug_colored_log}"
+                rf"{default_debug_colored_log_start}"
                 r"\x1b\[33mwarning\x1b\[0m: Processing...\n"
+                rf"{default_debug_colored_log_end}"
             ),
             result.stderr,
         )
 
     else:
         assert result.output == (
             "It works!\n"
             "Art\n"
             "Run command #1.\n"
             "\x1b[34mprint() bypass Click.\x1b[0m\n"
             "Done.\n"
         )
         assert re.fullmatch(
-            rf"{default_debug_uncolored_log}warning: Processing\.\.\.\n",
+            (
+                rf"{default_debug_uncolored_log_start}"
+                rf"warning: Processing\.\.\.\n"
+                rf"{default_debug_uncolored_log_end}"
+            ),
             result.stderr,
         )
 
 
 @pytest.mark.parametrize(
     "substrings, expected, ignore_case",
     (
```

### Comparing `click_extra-4.0.0/click_extra/tests/test_commands.py` & `click_extra-4.1.0/click_extra/tests/test_commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,21 +23,21 @@
 import re
 from pathlib import Path
 from textwrap import dedent
 
 import click
 import cloup
 import pytest
-from pytest_cases import fixture, parametrize
+from pytest_cases import fixture
 
 from .. import echo, option, option_group, pass_context
-from ..decorators import extra_command, extra_group, timer_option
+from ..decorators import extra_command, extra_group
 from .conftest import (
-    command_decorators,
-    default_debug_uncolored_log,
+    default_debug_uncolored_log_start,
+    default_debug_uncolored_log_end,
     default_options_colored_help,
     default_options_uncolored_help,
     skip_windows_colors,
 )
 
 
 def test_module_root_declarations():
@@ -83,15 +83,15 @@
         key=lambda m: (m.lower(), m),
     )
     assert expected_members == click_extra_members
 
 
 @fixture
 def all_command_cli():
-    """A CLI that used all variations and flavors of subcommands."""
+    """A CLI that is mixing all variations and flavors of subcommands."""
 
     @extra_group(version="2021.10.08")
     def command_cli1():
         echo("It works!")
 
     @command_cli1.command()
     def default_subcommand():
@@ -152,15 +152,16 @@
 def test_required_command(invoke, all_command_cli):
     result = invoke(all_command_cli, "--verbosity", "DEBUG", color=False)
     assert result.exit_code == 2
     # In debug mode, the version is always printed.
     assert not result.stdout
     assert re.fullmatch(
         (
-            rf"{default_debug_uncolored_log}"
+            rf"{default_debug_uncolored_log_start}"
+            rf"{default_debug_uncolored_log_end}"
             r"Usage: command-cli1 \[OPTIONS\] COMMAND \[ARGS\]...\n"
             r"\n"
             r"Error: Missing command.\n"
         ),
         result.stderr,
     )
 
@@ -247,80 +248,24 @@
         It works!
         Run {cmd_id} subcommand...
         """
     )
     assert not result.stderr
 
 
-def test_integrated_time_option(invoke, all_command_cli):
-    result = invoke(all_command_cli, "--time", "default-subcommand")
-    assert result.exit_code == 0
-    assert re.fullmatch(
-        r"It works!\nRun default subcommand...\nExecution time: [0-9.]+ seconds.\n",
-        result.output,
-    )
-    assert not result.stderr
-
-
-def test_integrated_notime_option(invoke, all_command_cli):
-    result = invoke(all_command_cli, "--no-time", "default-subcommand")
-    assert result.exit_code == 0
-    assert result.output == "It works!\nRun default subcommand...\n"
-    assert not result.stderr
-
-
 def test_integrated_version_value(invoke, all_command_cli):
     result = invoke(all_command_cli, "--version", color=False)
     assert result.exit_code == 0
 
     regex_output = r"command-cli1, version 2021.10.08\n{'.+'}\n"
     assert re.fullmatch(regex_output, result.output)
 
     assert not result.stderr
 
 
-@parametrize(
-    "cmd_decorator",
-    # Skip click extra's commands, as timer option is already part of the default.
-    command_decorators(no_groups=True, no_extra=True),
-)
-@parametrize("option_decorator", (timer_option, timer_option()))
-def test_standalone_timer_option(invoke, cmd_decorator, option_decorator):
-    @cmd_decorator
-    @option_decorator
-    def standalone_timer():
-        echo("It works!")
-
-    result = invoke(standalone_timer, "--help")
-    assert result.exit_code == 0
-    assert not result.stderr
-    assert result.stdout == dedent(
-        """\
-        Usage: standalone-timer [OPTIONS]
-
-        Options:
-          --time / --no-time  Measure and print elapsed execution time.
-          --help              Show this message and exit.
-        """
-    )
-
-    result = invoke(standalone_timer, "--time")
-    assert result.exit_code == 0
-    assert not result.stderr
-    assert re.fullmatch(
-        r"It works!\nExecution time: [0-9.]+ seconds.\n",
-        result.output,
-    )
-
-    result = invoke(standalone_timer, "--no-time")
-    assert result.exit_code == 0
-    assert not result.stderr
-    assert result.output == "It works!\n"
-
-
 def test_no_option_leaks_between_subcommands(invoke):
     """As reported in https://github.com/kdeldycke/click-extra/issues/489."""
 
     @click.group
     def cli():
         echo("Run cli...")
 
@@ -453,7 +398,62 @@
         dummy_flag is True
         Raw parameters: ['--dummy-flag', 'subcommand', '--int-param', '33']
         -- Subcommand output --
         int_parameter is 33
         Raw parameters: ['--int-param', '33']
         """
     )
+
+
+@pytest.mark.parametrize(
+    "cmd_decorator, ctx_settings, expected_help",
+    (
+        # Click does not show all envvar in the help screen by default, unless
+        # specifficaly set on an option.
+        (
+            click.command,
+            {},
+            "  --flag1\n  --flag2  [env var: custom2]\n  --flag3\n",
+        ),
+        # Click Extra defaults to let each option choose its own show_envvar value.
+        (
+            extra_command,
+            {},
+            "  --flag1\n"
+            "  --flag2                   [env var: custom2, CLI_FLAG2]\n"
+            "  --flag3\n",
+        ),
+        # Click Extra allow bypassing its global show_envvar setting.
+        (
+            extra_command,
+            {"show_envvar": None},
+            "  --flag1\n"
+            "  --flag2                   [env var: custom2, CLI_FLAG2]\n"
+            "  --flag3\n",
+        ),
+        # Click Extra force the show_envvar value on all options.
+        (
+            extra_command,
+            {"show_envvar": True},
+            "  --flag1                   [env var: custom1, CLI_FLAG1]\n"
+            "  --flag2                   [env var: custom2, CLI_FLAG2]\n"
+            "  --flag3                   [env var: custom3, CLI_FLAG3]\n",
+        ),
+        (
+            extra_command,
+            {"show_envvar": False},
+            "  --flag1\n  --flag2\n  --flag3\n",
+        ),
+    ),
+)
+def test_show_envvar_parameter(invoke, cmd_decorator, ctx_settings, expected_help):
+    @cmd_decorator(context_settings=ctx_settings)
+    @option("--flag1", is_flag=True, envvar=["custom1"])
+    @option("--flag2", is_flag=True, envvar=["custom2"], show_envvar=True)
+    @option("--flag3", is_flag=True, envvar=["custom3"], show_envvar=False)
+    def cli():
+        pass
+
+    result = invoke(cli, "--help")
+    assert result.exit_code == 0
+    assert not result.stderr
+    assert expected_help in result.stdout
```

### Comparing `click_extra-4.0.0/click_extra/tests/test_config.py` & `click_extra-4.1.0/click_extra/tests/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,20 +41,21 @@
     Tuple,
     argument,
     echo,
     get_app_dir,
     option,
 )
 from ..colorize import escape_for_help_sceen
-from ..commands import ExtraCommand
 from ..config import ConfigOption, ShowParamsOption
 from ..decorators import config_option, extra_command, extra_group, show_params_option
+from ..parameters import search_params
 from .conftest import (
     command_decorators,
-    default_debug_uncolored_log,
+    default_debug_uncolored_log_start,
+    default_debug_uncolored_log_end,
 )
 
 DUMMY_TOML_FILE = """
     # Comment
 
     top_level_param             = "to_ignore"
 
@@ -230,15 +231,18 @@
 
 def test_unset_conf_debug_message(invoke, simple_config_cli):
     result = invoke(
         simple_config_cli, "--verbosity", "DEBUG", "default-command", color=False
     )
     assert result.exit_code == 0
     assert result.output == "dummy_flag = False\nmy_list = ()\nint_parameter = 10\n"
-    assert re.fullmatch(default_debug_uncolored_log, result.stderr)
+    assert re.fullmatch(
+        default_debug_uncolored_log_start + default_debug_uncolored_log_end,
+        result.stderr,
+    )
 
 
 def test_conf_default_path(invoke, simple_config_cli):
     result = invoke(simple_config_cli, "--help", color=False)
     assert result.exit_code == 0
 
     # OS-specific path.
@@ -345,15 +349,15 @@
         "random_file2",
         color=False,
     )
 
     assert result.exit_code == 0
     assert result.output == "Works!\n"
 
-    cli_config_option = ExtraCommand._search_params(config_cli2.params, ConfigOption)
+    cli_config_option = search_params(config_cli2.params, ConfigOption)
     assert cli_config_option.params_template == {
         "config-cli2": {
             "flag1": None,
             "flag2": None,
             "str_param1": None,
             "str_param2": None,
             "int_param1": None,
@@ -455,34 +459,40 @@
     invoke, simple_config_cli, create_config, httpserver, conf_name, conf_content
 ):
     # Create a local file and remote config.
     conf_filepath = create_config(conf_name, conf_content)
     httpserver.expect_request(f"/{conf_name}").respond_with_data(conf_content)
     conf_url = httpserver.url_for(f"/{conf_name}")
 
-    for conf_path in conf_filepath, conf_url:
+    for conf_path, is_url in (conf_filepath, False), (conf_url, True):
         result = invoke(
             simple_config_cli,
             "--config",
             str(conf_path),
             "default-command",
             color=False,
         )
         assert result.exit_code == 0
         assert result.stdout == (
             "dummy_flag = True\nmy_list = ('pip', 'npm', 'gem')\nint_parameter = 3\n"
         )
 
         # Debug level has been activated by configuration file.
-        debug_log = (
-            rf"Load configuration matching {re.escape(str(conf_path))}\n"
-            r"(.+\n)*"
-            r"debug: Verbosity set to DEBUG.\n"
+        debug_log = rf"Load configuration matching {re.escape(str(conf_path))}\n"
+        if is_url:
+            debug_log += (
+                r'info: 127\.0\.0\.1 - - \[\S+ \S+\] '
+                rf'"GET /{re.escape(conf_name)} HTTP/1\.1" 200 -\n'
+            )
+        debug_log += (
+            r"debug: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
+            r"debug: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
             r"debug: \S+, version \S+\n"
             r"debug: {.*}\n"
+            rf"{default_debug_uncolored_log_end}"
         )
         assert re.fullmatch(debug_log, result.stderr)
 
 
 @all_config_formats
 def test_auto_env_var_conf(
     invoke, simple_config_cli, create_config, httpserver, conf_name, conf_content
@@ -621,111 +631,111 @@
 
     table = [
         (
             "show-params-cli.color",
             "click_extra.colorize.ColorOption",
             "--color, --ansi / --no-color, --no-ansi",
             "bool",
-            "",
+            "✓",
             "✘",
             "SHOW_PARAMS_CLI_COLOR",
             True,
             True,
             "DEFAULT",
         ),
         (
             "show-params-cli.config",
             "click_extra.config.ConfigOption",
             "-C, --config CONFIG_PATH",
             "str",
-            "",
+            "✘",
             "✘",
             "SHOW_PARAMS_CLI_CONFIG",
             f"{Path(get_app_dir('show-params-cli')).resolve()}{sep}*.{{toml,yaml,yml,json,ini,xml}}",
             str(conf_path),
             "COMMANDLINE",
         ),
         (
             "show-params-cli.help",
             "click_extra.colorize.HelpOption",
             "-h, --help",
             "bool",
-            "",
+            "✘",
             "✘",
             "SHOW_PARAMS_CLI_HELP",
             False,
             True,
             "COMMANDLINE",
         ),
         (
             "show-params-cli.int_param1",
             "cloup._params.Option",
             "--int-param1 INTEGER",
             "int",
-            "",
+            "✓",
             "✓",
             "SHOW_PARAMS_CLI_INT_PARAM1",
             3,
             9999,
             "COMMANDLINE",
         ),
         (
             "show-params-cli.int_param2",
             "cloup._params.Option",
             "--int-param2 INTEGER",
             "int",
-            "",
+            "✓",
             "✓",
             "SHOW_PARAMS_CLI_INT_PARAM2",
             555,
             555,
             "DEFAULT",
         ),
         (
             "show-params-cli.show_params",
             "click_extra.config.ShowParamsOption",
             "--show-params",
             "bool",
-            "",
+            "✘",
             "✘",
             "SHOW_PARAMS_CLI_SHOW_PARAMS",
             False,
             True,
             "COMMANDLINE",
         ),
         (
             "show-params-cli.time",
-            "click_extra.commands.TimerOption",
+            "click_extra.timer.TimerOption",
             "--time / --no-time",
             "bool",
-            "",
+            "✓",
             "✘",
             "SHOW_PARAMS_CLI_TIME",
             False,
             False,
             "DEFAULT",
         ),
         (
             "show-params-cli.verbosity",
             "click_extra.logging.VerbosityOption",
             "-v, --verbosity LEVEL",
             "str",
-            "",
+            "✓",
             "✘",
             "SHOW_PARAMS_CLI_VERBOSITY",
             "WARNING",
             "DeBuG",
             "COMMANDLINE",
         ),
         (
             "show-params-cli.version",
             "click_extra.version.VersionOption",
             "--version",
             "bool",
-            "",
+            "✘",
             "✘",
             "SHOW_PARAMS_CLI_VERSION",
             False,
             False,
             "DEFAULT",
         ),
     ]
```

### Comparing `click_extra-4.0.0/click_extra/tests/test_logging.py` & `click_extra-4.1.0/click_extra/tests/test_logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,41 +15,45 @@
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 from __future__ import annotations
 
 import re
 import logging
 import random
-import sys
 
 import pytest
 from pytest_cases import parametrize
 import click
 
 from .. import echo
 from ..decorators import extra_command, verbosity_option
 from ..logging import LOG_LEVELS
-from .conftest import command_decorators, default_debug_colored_log, skip_windows_colors
+from .conftest import (
+    command_decorators,
+    default_debug_colored_log_start,
+    default_debug_uncolored_log_end,
+    default_debug_colored_log_end,
+    skip_windows_colors,
+)
 from ..logging import DEFAULT_LEVEL
 
 
 def test_level_default_order():
     assert tuple(LOG_LEVELS) == ("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG")
 
 
 def test_root_logger_defaults():
     """Check our internal default is aligned to Python's root logger."""
-    # Check the root logger is the default logger.
-    if sys.version_info < (3, 9):
-        assert logging.getLogger() is not logging.getLogger("root")
-    else:
-        assert logging.getLogger() is logging.getLogger("root")
+    # Check the root logger is the default logger, ans that getLogger is
+    # properly patched on Python 3.8.
+    assert logging.getLogger() is logging.getLogger("root")
     assert logging.getLogger() is logging.root
 
     # Check root logger's level.
+    assert logging.root.getEffectiveLevel() == logging.WARNING
     assert logging._levelToName[logging.root.level] == "WARNING"
     assert logging.root.level == DEFAULT_LEVEL
 
 
 @pytest.mark.parametrize("cmd_decorator, cmd_type", command_decorators(with_types=True))
 def test_unrecognized_verbosity(invoke, cmd_decorator, cmd_type):
     @cmd_decorator
@@ -107,98 +111,99 @@
 
     result = invoke(logging_cli2, "--verbosity", level, color=True)
     assert result.exit_code == 0
     assert result.output == "It works!\n"
 
     messages = (
         (
-            "\x1b[34mdebug\x1b[0m: Verbosity set to DEBUG.\n"
-            "\x1b[34mdebug\x1b[0m: my random message.\n"
-            "\x1b[34mdebug\x1b[0m: my debug message.\n"
+            r"\x1b\[34mdebug\x1b\[0m: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
+            r"\x1b\[34mdebug\x1b\[0m: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
+            r"\x1b\[34mdebug\x1b\[0m: my random message.\n"
+            r"\x1b\[34mdebug\x1b\[0m: my debug message.\n"
         ),
-        "info: my info message.\n",
-        "\x1b[33mwarning\x1b[0m: my warning message.\n",
-        "\x1b[31merror\x1b[0m: my error message.\n",
-        "\x1b[31mcritical\x1b[0m: my critical message.\n",
+        r"info: my info message.\n",
+        r"\x1b\[33mwarning\x1b\[0m: my warning message.\n",
+        r"\x1b\[31merror\x1b\[0m: my error message.\n",
+        r"\x1b\[31mcritical\x1b\[0m: my critical message.\n",
     )
     level_index = {index: level for level, index in enumerate(LOG_LEVELS)}[level]
-    log_records = "".join(messages[-level_index - 1 :])
-    assert result.stderr == log_records
+    log_records = r"".join(messages[-level_index - 1 :])
+
+    if level == "DEBUG":
+        log_records += default_debug_colored_log_end
+    assert re.fullmatch(log_records, result.stderr)
 
 
 @skip_windows_colors
 @pytest.mark.parametrize("level", LOG_LEVELS.keys())
 # TODO: test extra_group
 def test_integrated_verbosity_option(invoke, level):
     @extra_command
     def logging_cli3():
         echo("It works!")
 
     result = invoke(logging_cli3, "--verbosity", level, color=True)
     assert result.exit_code == 0
     assert result.output == "It works!\n"
     if level == "DEBUG":
-        assert re.fullmatch(default_debug_colored_log, result.stderr)
+        assert re.fullmatch(
+            default_debug_colored_log_start + default_debug_colored_log_end,
+            result.stderr,
+        )
     else:
         assert not result.stderr
 
 
-@skip_windows_colors
-@pytest.mark.parametrize("params", (("--verbosity", "DEBUG"), None))
-def test_custom_logger_id(invoke, params):
-    my_app_logger = logging.getLogger("awesome_app")
-
-    @click.command
-    @verbosity_option(default_logger="awesome_app")
-    def awesome_app():
-        echo("Starting Awesome App...")
-        my_app_logger.debug("Awesome App has started.")
-
-    result = invoke(awesome_app, params, color=True)
-    assert result.exit_code == 0
-    assert result.output == "Starting Awesome App...\n"
-    if params:
-        assert result.stderr == (
-            "\x1b[34mdebug\x1b[0m: Verbosity set to DEBUG.\n"
-            "\x1b[34mdebug\x1b[0m: Awesome App has started.\n"
-        )
-
-
-@skip_windows_colors
+@pytest.mark.parametrize(
+    "logger_param", (logging.getLogger("awesome_app"), "awesome_app")
+)
 @pytest.mark.parametrize("params", (("--verbosity", "DEBUG"), None))
-def test_custom_logger_object(invoke, params):
-    my_app_logger = logging.getLogger("awesome_app")
+def test_custom_logger_param(invoke, logger_param, params):
+    """Passing a logger instance or name to the ``default_logger`` parameter works.
+    """
 
     @click.command
-    @verbosity_option(default_logger=my_app_logger)
+    @verbosity_option(default_logger=logger_param)
     def awesome_app():
         echo("Starting Awesome App...")
-        my_app_logger.debug("Awesome App has started.")
+        logging.getLogger("awesome_app").debug("Awesome App has started.")
 
-    result = invoke(awesome_app, params, color=True)
+    result = invoke(awesome_app, params, color=False)
     assert result.exit_code == 0
     assert result.output == "Starting Awesome App...\n"
     if params:
-        assert result.stderr == (
-            "\x1b[34mdebug\x1b[0m: Verbosity set to DEBUG.\n"
-            "\x1b[34mdebug\x1b[0m: Awesome App has started.\n"
+        assert re.fullmatch(
+            (
+                r"debug: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
+                r"debug: Set <Logger awesome_app \(DEBUG\)> to DEBUG.\n"
+                r"debug: Awesome App has started\.\n"
+                r"debug: Reset <Logger awesome_app \(DEBUG\)> to WARNING.\n"
+                r"debug: Reset <Logger click_extra \(DEBUG\)> to WARNING.\n"
+            ),
+            result.stderr,
         )
+    else:
+        assert not result.stderr
 
 
-@skip_windows_colors
 def test_custom_option_name(invoke):
     param_names = ("--blah", "-B")
 
     @click.command
     @verbosity_option(*param_names)
     def awesome_app():
         root_logger = logging.getLogger()
         root_logger.debug("my debug message.")
 
     for name in param_names:
-        result = invoke(awesome_app, name, "DEBUG", color=True)
+        result = invoke(awesome_app, name, "DEBUG", color=False)
         assert result.exit_code == 0
         assert not result.output
-        assert result.stderr == (
-            "\x1b[34mdebug\x1b[0m: Verbosity set to DEBUG.\n"
-            "\x1b[34mdebug\x1b[0m: my debug message.\n"
+        assert re.fullmatch(
+            (
+                r"debug: Set <Logger click_extra \(DEBUG\)> to DEBUG.\n"
+                r"debug: Set <RootLogger root \(DEBUG\)> to DEBUG.\n"
+                r"debug: my debug message\.\n"
+                rf"{default_debug_uncolored_log_end}"
+            ),
+            result.stderr,
         )
```

### Comparing `click_extra-4.0.0/click_extra/tests/test_parameters.py` & `click_extra-4.1.0/click_extra/tests/test_parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.
 
 from __future__ import annotations
 
 import pytest
 from pytest_cases import parametrize
+import click
 
 from .. import echo, option, extra_command, command
 from ..parameters import normalize_envvar, extend_envvars
 from ..platforms import is_windows
 
 
 @pytest.mark.parametrize(
@@ -47,30 +48,63 @@
 
 
 @pytest.mark.parametrize(
     "env_name, normalized_env",
     (
         ("show-params-cli_VERSION", "SHOW_PARAMS_CLI_VERSION"),
         ("show---params-cli___VERSION", "SHOW_PARAMS_CLI_VERSION"),
+        ("__show-__params-_-_-", "SHOW_PARAMS"),
     ),
 )
 def test_normalize_envvar(env_name, normalized_env):
     assert normalize_envvar(env_name) == normalized_env
 
 
+@pytest.mark.parametrize(
+    "cmd_decorator, option_help",
+    (
+        # Click does not show the auto-generated envvar in the help screen.
+        (click.command, "  --flag / --no-flag  [env var: custom]\n"),
+        # Click Extra always adds the auto-generated envvar to the help screen
+        # (and show the defaults).
+        (
+            extra_command,
+            "  --flag / --no-flag        "
+            "[env var: custom, yo_FLAG; default: no-flag]\n",
+        ),
+    ),
+)
+def test_show_auto_envvar_help(invoke, cmd_decorator, option_help):
+    """Check that the auto-generated envvar appears in the help screen with the extra
+    variants.
+
+    Checks that https://github.com/pallets/click/issues/2483 is addressed.
+    """
+
+    @cmd_decorator(context_settings={"auto_envvar_prefix": "yo"})
+    @option("--flag/--no-flag", envvar=["custom"], show_envvar=True)
+    def envvar_help():
+        pass
+
+    result = invoke(envvar_help, "--help")
+    assert result.exit_code == 0
+    assert not result.stderr
+    assert option_help in result.stdout
+
+
 def envvars_test_cases():
     params = []
 
     matrix = {
         (command, "command"): {
             "working_envvar": (
                 # User-defined envvars are recognized as-is.
                 "Magic",
                 "sUper",
-                # XXX Uppercased auto-generated envvar is recognized be should not.
+                # XXX Uppercased auto-generated envvar is recognized but should not be.
                 "YO_FLAG",
             ),
             "unknown_envvar": (
                 # Uppercased user-defined envvar is not recognized.
                 "MAGIC",
                 # XXX Literal auto-generated is not recognized but should be.
                 "yo_FLAG",
@@ -82,15 +116,15 @@
             "working_envvar": (
                 # User-defined envvars are recognized as-is.
                 "Magic",
                 "sUper",
                 # Literal auto-generated is properly recognized but is not in vanilla
                 # Click (see above).
                 "yo_FLAG",
-                # XXX Uppercased auto-generated envvar is recognized be should not.
+                # XXX Uppercased auto-generated envvar is recognized but should not be.
                 "YO_FLAG",
             ),
             "unknown_envvar": (
                 # Uppercased user-defined envvar is not recognized.
                 "MAGIC",
                 # Mixed-cased auto-generated envvat is not recognized.
                 "yo_FlAg",
@@ -122,18 +156,20 @@
             },
         }
 
     # If properly recognized, these envvar values should be passed to the flag.
     working_value_map = {
         "True": True,
         "true": True,
+        "tRuE": True,
         "1": True,
         "": False,  # XXX: Should be True?
         "False": False,
         "false": False,
+        "fAlsE": False,
         "0": False,
     }
     # No envvar value will have an effect on the flag if the envvar is not recognized.
     broken_value_map = {k: False for k in working_value_map}
 
     for (cmd_decorator, decorator_name), envvar_cases in matrix.items():
         for case_name, envvar_names in envvar_cases.items():
@@ -153,15 +189,21 @@
                         )
                     )
 
     return params
 
 
 @parametrize("cmd_decorator, envvars, expected_flag", envvars_test_cases())
-def test_default_auto_envvar(invoke, cmd_decorator, envvars, expected_flag):
+def test_auto_envvar_parsing(invoke, cmd_decorator, envvars, expected_flag):
+    """This test highlights the way Click recognize and parse envvars.
+
+    It shows that the default behavior is not ideal, and covers how ``extra_command``
+    improves the situation by normalizing the envvar name.
+    """
+
     @cmd_decorator(context_settings={"auto_envvar_prefix": "yo"})
     @option("--flag/--no-flag", envvar=["Magic", "sUper"])
     def my_cli(flag):
         echo(f"Flag value: {flag}")
 
     registered_envvars = ["Magic", "sUper"]
     # @extra_command forces registration of auto-generated envvar.
```

### Comparing `click_extra-4.0.0/click_extra/tests/test_platforms.py` & `click_extra-4.1.0/click_extra/tests/test_platforms.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/tests/test_pygments.py` & `click_extra-4.1.0/click_extra/tests/test_pygments.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,21 +20,19 @@
 import tarfile
 from operator import itemgetter
 from pathlib import Path
 from importlib import metadata
 
 from boltons.strutils import camel2under
 from boltons.typeutils import issubclass
-from pip._internal.cli.status_codes import SUCCESS
-from pip._internal.commands.download import DownloadCommand
-from pip._internal.utils.temp_dir import global_tempdir_manager, tempdir_registry
 from pygments.filter import Filter
 from pygments.formatter import Formatter
 from pygments.lexers import find_lexer_class_by_name
 from pygments.style import Style
+import requests
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib  # type: ignore[import]
 
 from .. import pygments as extra_pygments
@@ -59,65 +57,60 @@
     """Look into Pygments test suite to find all ANSI lexers candidates.
 
     Good candidates for ANSI colorization are lexers that are producing
     ``Generic.Output`` tokens, which are often used by REPL-like and scripting
     terminal to render text in a console.
 
     The list is manually maintained in Click Extra code, and this test is here to
-    detect new candidates from Pygments new releases.
+    detect new candidates from new releases of Pygments.
+
+    .. attention::
+        The Pygments source code is downloaded from GitHub in the form of an archive,
+        and extracted in a temporary folder.
+
+        The version of Pygments used for this test is the one installed in the current
+        environment.
+
+    .. danger:: Security check
+        While extracting the archive, we double check we are not fed an archive
+        exploiting relative ``..`` or ``.`` path attacks.
     """
-    # Get the version of the Pygments package installed in the current environment.
     version = metadata.version("pygments")
 
-    # Emulate CLI call to download Pygments' source distribution (which contains the
-    # full test suite and data) from PyPi via pip:
-    #   $ pip download --no-binary=:all: --no-deps pygments==2.14.0
-    # Source: https://stackoverflow.com/a/56773693
-    cmd = DownloadCommand(name="dummy_name", summary="dummy_summary")
-
-    # Inspired by pip._internal.cli.base_command.Command._main(). See:
-    # https://github.com/pypa/pip/blob/ba38c33b6b4fc3ee22dabb747a4b4ccff0a87d22/src/pip/_internal/cli/base_command.py#L105-L114
-    with cmd.main_context():
-        cmd.tempdir_registry = cmd.enter_context(tempdir_registry())
-        cmd.enter_context(global_tempdir_manager())
-        options, args = cmd.parse_args(
-            [
-                "--no-binary=:all:",
-                "--no-deps",
-                "--dest",
-                f"{tmp_path}",
-                f"pygments=={version}",
-            ]
-        )
-        cmd.verbosity = options.verbose
-        outcome = cmd.run(options, args)
-        assert outcome == SUCCESS
-
-    base_folder = f"Pygments-{version}"
-    package_path = tmp_path.joinpath(f"{base_folder}.tar.gz")
-    assert package_path.exists()
-    assert package_path.is_file()
+    source_url = (
+        f"https://github.com/pygments/pygments/archive/refs/tags/{version}.tar.gz"
+    )
+    base_folder = f"pygments-{version}"
+    archive_path = tmp_path / f"{base_folder}.tar.gz"
+
+    # Download the source distribution from GitHub.
+    with requests.get(source_url) as response:
+        assert response.ok
+        archive_path.write_bytes(response.content)
+
+    assert archive_path.exists()
+    assert archive_path.is_file()
+    assert archive_path.stat().st_size > 0
 
     # Locations of lexer artifacts in test suite.
     parser_token_traces = {
         str(tmp_path / base_folder / "tests" / "examplefiles" / "*" / "*.output"),
         str(tmp_path / base_folder / "tests" / "snippets" / "*" / "*.txt"),
     }
 
     # Browse the downloaded package to find the test suite, and inspect the
     # traces of parsed tokens used as gold master for lexers tests.
     lexer_candidates = set()
-    with tarfile.open(package_path, "r:gz") as tar:
+    with tarfile.open(archive_path, "r:gz") as tar:
         for member in tar.getmembers():
             # Skip non-test files.
             if not member.isfile():
                 continue
 
-            # Double check we are not fed an archive exploiting relative ``..`` or
-            # ``.`` path attacks.
+            # XXX Security check of relative ``..`` or ``.`` path attacks.
             filename = tmp_path.joinpath(member.name).resolve()
             if sys.version_info >= (3, 9):
                 assert filename.is_relative_to(tmp_path)
             else:
                 assert is_relative_to(filename, tmp_path)
 
             # Skip files that are not part of the test suite data.
@@ -139,14 +132,15 @@
             # Skip lexers that are rendering generic, terminal-like output tokens.
             if f" {'.'.join(DEFAULT_TOKEN_TYPE)}\n" not in content:
                 continue
 
             # Extarct lexer alias from the test file path.
             lexer_candidates.add(filename.parent.name)
 
+    assert lexer_candidates
     lexer_classes = {find_lexer_class_by_name(alias) for alias in lexer_candidates}
     # We cannot test for strict equality yet, as some ANSI-ready lexers do not
     # have any test artifacts producing ``Generic.Output`` tokens.
     assert lexer_classes.issubset(collect_session_lexers())
 
 
 def get_pyproject_section(*section_path: str) -> dict[str, str]:
```

### Comparing `click_extra-4.0.0/click_extra/tests/test_run.py` & `click_extra-4.1.0/click_extra/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/tests/test_tabulate.py` & `click_extra-4.1.0/click_extra/tests/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/tests/test_telemetry.py` & `click_extra-4.1.0/click_extra/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/tests/test_version.py` & `click_extra-4.1.0/click_extra/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `click_extra-4.0.0/click_extra/version.py` & `click_extra-4.1.0/click_extra/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,16 @@
         param_decls: Sequence[str] | None = None,
         version: str | None = None,
         package_name: str | None = None,
         prog_name: str | None = None,
         message: str | None = None,
         print_env_info: bool = False,
         version_style=Style(fg="green"),
-        package_name_style=default_theme.invoked_command,  # type: ignore[has-type]
-        prog_name_style=default_theme.invoked_command,  # type: ignore[has-type]
+        package_name_style=default_theme.invoked_command,
+        prog_name_style=default_theme.invoked_command,
         message_style=None,
         env_info_style=Style(fg="bright_black"),
         is_flag=True,
         expose_value=False,
         is_eager=True,
         help=_("Show the version and exit."),
         **kwargs,
```

### Comparing `click_extra-4.0.0/pyproject.toml` & `click_extra-4.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 # Docs: https://python-poetry.org/docs/pyproject/
 name = "click-extra"
-version = "4.0.0"
+version = "4.1.0"
 description = "🌈 Extra colorization and configuration loading for Click."
 license = 'GPL-2.0-or-later'
 authors = ["Kevin Deldycke <kevin@deldycke.com>"]
 readme = "readme.md"
 homepage = 'https://github.com/kdeldycke/click-extra'
 repository = 'https://github.com/kdeldycke/click-extra'
 documentation = 'https://kdeldycke.github.io/click-extra'
@@ -68,15 +68,16 @@
 # List of python versions and their support status:
 # https://en.wikipedia.org/wiki/History_of_Python#Support
 python = "^3.8"
 # XXX boltons.ecoutils 23.0.0 breaks PDB interactive sessions in pytest.
 # Investigation of the root cause is being discussed upstream at:
 # https://github.com/mahmoud/boltons/issues/334
 boltons = "^23.0.0"
-click = "^8.1.3"
+# Click 8.1 is the first version to support ``params=`` in ``@command``.
+click = "^8.1"
 cloup = "^2.0.0.post1"
 commentjson = "^0.9.0"
 furo = "^2023.03.27"
 mergedeep = "^1.3.4"
 # Pallets-Sphinx-Themes 2.1.0 is the first version rendering ``.. sourcecode:: shell-session`` code-blocks.
 Pallets-Sphinx-Themes = "^2.1.0"
 # Pygments 2.14.0 is the first version with ``lexers.algebra.GAPConsoleLexer`` that is referenced in our code.
```

### Comparing `click_extra-4.0.0/readme.md` & `click_extra-4.1.0/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -30,37 +30,41 @@
 
 ![click-extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/assets/click-extra-screen.png)
 
 To undestrand how we ended up with the result above, [go read the tutorial](https://kdeldycke.github.io/click-extra/tutorial.html).
 
 ## Features
 
-- Configuration file loader for:
+- [Configuration file](https://kdeldycke.github.io/click-extra/config.html) loader for:
   - `TOML`
   - `YAML`
   - `JSON`, with inline and block comments (Python-style `#` and Javascript-style `//`)
   - `INI`, with extended interpolation, multi-level sections and non-native types (`list`, `set`, …)
   - `XML`
 - Automatic inference of the configuration file structure from your CLI's options
-- Remote loading of configuration files from URLs
-- Optional strict validation of configuration
-- Search of configuration file from default user folder and glob patterns
-- Respect of `CLI` > `Configuration` > `Environment` > `Defaults` precedence
-- `--show-params` option to debug parameters defaults, values, environment variables and provenance
-- Colorization of help screens
+- Remote loading of [configuration files from URLs](https://kdeldycke.github.io/click-extra/config.html#remote-url)
+- Optional [strict validation](https://kdeldycke.github.io/click-extra/config.html#strictness) of configuration
+- Respect the [default application path](https://kdeldycke.github.io/click-extra/config.html#default-folder) on each platform (XDG spec on Linux)
+- [Glob search patterns](https://kdeldycke.github.io/click-extra/config.html#pattern-matching) for configuration files
+- Respect of `CLI` > `Configuration` > `Environment` > `Defaults` [precedence](https://kdeldycke.github.io/click-extra/config.html#precedence)
+- Normalization and discoverability of environment variables
+- [`--show-params` option](https://kdeldycke.github.io/click-extra/config.html#show-params-option) to debug parameters defaults, values, environment variables and provenance
+- [Colorization of help screens](https://kdeldycke.github.io/click-extra/colorize.html) at the semantic-level of options, parameters, subheadings, choices, metavars and defaults
+- Global `show_envvar` option to display all environment variables in help screens
 - `-h`/`--help` option names (see [rant on other inconsistencies](https://blog.craftyguy.net/cmdline-help/))
 - `--color`/`--no-color` option flag
 - `--telemetry`/`--no-telemetry` flag to opt-in/out of tracking code
 - Recognize traditional environment variable conventions:
   - `NO_COLOR` from [`no-color.org`](https://no-color.org)
   - `DO_NOT_TRACK` from [`consoledonottrack.com`](https://consoledonottrack.com)
 - Colored `--version` option
-- Colored `--verbosity` option and logs
+- [Colored `--verbosity` option and logs](https://kdeldycke.github.io/click-extra/logging.html)
 - `--time`/`--no-time` flag to measure duration of command execution
-- Platform recognition utilities (macOS, Linux, Windows, UNIX, \*BSD, …)
+- Global `show_choices` to activate selection of choices on user input prompts
+- [Platform recognition](https://kdeldycke.github.io/click-extra/platforms.html) utilities (macOS, Linux, Windows, UNIX, \*BSD, …)
 - New conditional markers for `pytest`:
   - `@skip_linux`, `@skip_macos` and `@skip_windows`
   - `@unless_linux`, `@unless_macos` and `@unless_windows`
   - `@destructive` and `@non_destructive`
 - [`.. click:example::` and `.. click:run::` Sphinx directives](https://kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and their execution
 - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell session and console output
 - Pygments styles and filters for ANSI rendering
```

#### html2text {}

```diff
@@ -17,48 +17,61 @@
 and patches](https://kdeldycke.github.io/click-extra/issues.html) that have not
 reached upstream yet (or are unlikely to). ## Example It transforms this
 vanilla `click` CLI: ![click CLI help screen](https://github.com/kdeldycke/
 click-extra/raw/main/docs/assets/click-help-screen.png) Into this: ![click-
 extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/
 assets/click-extra-screen.png) To undestrand how we ended up with the result
 above, [go read the tutorial](https://kdeldycke.github.io/click-extra/
-tutorial.html). ## Features - Configuration file loader for: - `TOML` - `YAML`
-- `JSON`, with inline and block comments (Python-style `#` and Javascript-style
-`//`) - `INI`, with extended interpolation, multi-level sections and non-native
-types (`list`, `set`, â¦) - `XML` - Automatic inference of the configuration
-file structure from your CLI's options - Remote loading of configuration files
-from URLs - Optional strict validation of configuration - Search of
-configuration file from default user folder and glob patterns - Respect of
-`CLI` > `Configuration` > `Environment` > `Defaults` precedence - `--show-
-params` option to debug parameters defaults, values, environment variables and
-provenance - Colorization of help screens - `-h`/`--help` option names (see
-[rant on other inconsistencies](https://blog.craftyguy.net/cmdline-help/)) - `-
--color`/`--no-color` option flag - `--telemetry`/`--no-telemetry` flag to opt-
+tutorial.html). ## Features - [Configuration file](https://kdeldycke.github.io/
+click-extra/config.html) loader for: - `TOML` - `YAML` - `JSON`, with inline
+and block comments (Python-style `#` and Javascript-style `//`) - `INI`, with
+extended interpolation, multi-level sections and non-native types (`list`,
+`set`, â¦) - `XML` - Automatic inference of the configuration file structure
+from your CLI's options - Remote loading of [configuration files from URLs]
+(https://kdeldycke.github.io/click-extra/config.html#remote-url) - Optional
+[strict validation](https://kdeldycke.github.io/click-extra/
+config.html#strictness) of configuration - Respect the [default application
+path](https://kdeldycke.github.io/click-extra/config.html#default-folder) on
+each platform (XDG spec on Linux) - [Glob search patterns](https://
+kdeldycke.github.io/click-extra/config.html#pattern-matching) for configuration
+files - Respect of `CLI` > `Configuration` > `Environment` > `Defaults`
+[precedence](https://kdeldycke.github.io/click-extra/config.html#precedence) -
+Normalization and discoverability of environment variables - [`--show-params`
+option](https://kdeldycke.github.io/click-extra/config.html#show-params-option)
+to debug parameters defaults, values, environment variables and provenance -
+[Colorization of help screens](https://kdeldycke.github.io/click-extra/
+colorize.html) at the semantic-level of options, parameters, subheadings,
+choices, metavars and defaults - Global `show_envvar` option to display all
+environment variables in help screens - `-h`/`--help` option names (see [rant
+on other inconsistencies](https://blog.craftyguy.net/cmdline-help/)) - `--
+color`/`--no-color` option flag - `--telemetry`/`--no-telemetry` flag to opt-
 in/out of tracking code - Recognize traditional environment variable
 conventions: - `NO_COLOR` from [`no-color.org`](https://no-color.org) -
 `DO_NOT_TRACK` from [`consoledonottrack.com`](https://consoledonottrack.com) -
-Colored `--version` option - Colored `--verbosity` option and logs - `--time`/
-`--no-time` flag to measure duration of command execution - Platform
-recognition utilities (macOS, Linux, Windows, UNIX, \*BSD, â¦) - New
-conditional markers for `pytest`: - `@skip_linux`, `@skip_macos` and
-`@skip_windows` - `@unless_linux`, `@unless_macos` and `@unless_windows` -
-`@destructive` and `@non_destructive` - [`.. click:example::` and `.. click:
-run::` Sphinx directives](https://kdeldycke.github.io/click-extra/sphinx.html)
-to document CLI source code and their execution - [ANSI-capable Pygments
-lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell
-session and console output - Pygments styles and filters for ANSI rendering -
-[Fixes 30+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from
-other Click-related projects - Rely on [`cloup`](https://github.com/janluke/
-cloup) to add: - option groups - constraints - subcommands sections - aliases -
-command suggestion (`Did you mean ?`) ## Used in Check these projects to get
-real-life examples of `click-extra` usage: - ![GitHub stars](https://
-img.shields.io/github/stars/kdeldycke/meta-package-
-manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager](https://
-github.com/kdeldycke/meta-package-manager#readme) \- A unifying CLI for
-multiple package managers. - ![GitHub stars](https://img.shields.io/github/
+Colored `--version` option - [Colored `--verbosity` option and logs](https://
+kdeldycke.github.io/click-extra/logging.html) - `--time`/`--no-time` flag to
+measure duration of command execution - Global `show_choices` to activate
+selection of choices on user input prompts - [Platform recognition](https://
+kdeldycke.github.io/click-extra/platforms.html) utilities (macOS, Linux,
+Windows, UNIX, \*BSD, â¦) - New conditional markers for `pytest`: -
+`@skip_linux`, `@skip_macos` and `@skip_windows` - `@unless_linux`,
+`@unless_macos` and `@unless_windows` - `@destructive` and `@non_destructive` -
+[`.. click:example::` and `.. click:run::` Sphinx directives](https://
+kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and
+their execution - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/
+click-extra/pygments.html#lexers) for shell session and console output -
+Pygments styles and filters for ANSI rendering - [Fixes 30+ bugs](https://
+kdeldycke.github.io/click-extra/issues.html) from other Click-related projects
+- Rely on [`cloup`](https://github.com/janluke/cloup) to add: - option groups -
+constraints - subcommands sections - aliases - command suggestion (`Did you
+mean ?`) ## Used in Check these projects to get real-life examples of `click-
+extra` usage: - ![GitHub stars](https://img.shields.io/github/stars/kdeldycke/
+meta-package-manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager]
+(https://github.com/kdeldycke/meta-package-manager#readme) \- A unifying CLI
+for multiple package managers. - ![GitHub stars](https://img.shields.io/github/
 stars/kdeldycke/mail-deduplicate?label=%E2%AD%90&style=flat-square) [Mail
 Deduplicate](https://github.com/kdeldycke/mail-deduplicate#readme) - A CLI to
 deduplicate similar emails. - ![GitHub stars](https://img.shields.io/github/
 stars/Sprocket-Security/fireproxng?label=%E2%AD%90&style=flat-square)
 [fireproxng](https://github.com/Sprocket-Security/fireproxng#readme) - A
 rewrite of the fireprox tool. - ![GitHub stars](https://img.shields.io/github/
 stars/hugolundin/badger?label=%E2%AD%90&style=flat-square) [badger-proxy]
```

### Comparing `click_extra-4.0.0/PKG-INFO` & `click_extra-4.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: click-extra
-Version: 4.0.0
+Version: 4.1.0
 Summary: 🌈 Extra colorization and configuration loading for Click.
 Home-page: https://github.com/kdeldycke/click-extra
 License: GPL-2.0-or-later
 Keywords: ansi-colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-tabulate,sphinx,terminal,toml,xml,yaml
 Author: Kevin Deldycke
 Author-email: kevin@deldycke.com
 Requires-Python: >=3.8,<4.0
@@ -37,15 +37,15 @@
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Text Processing :: Markup :: reStructuredText
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: Pallets-Sphinx-Themes (>=2.1.0,<3.0.0)
 Requires-Dist: boltons (>=23.0.0,<24.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: cloup (>=2.0.0.post1,<3.0.0)
 Requires-Dist: commentjson (>=0.9.0,<0.10.0)
 Requires-Dist: furo (>=2023.03.27,<2024.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: pygments (>=2.14,<3.0)
 Requires-Dist: pygments-ansi-color (>=0.2.0,<0.3.0)
 Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
@@ -95,37 +95,41 @@
 
 ![click-extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/assets/click-extra-screen.png)
 
 To undestrand how we ended up with the result above, [go read the tutorial](https://kdeldycke.github.io/click-extra/tutorial.html).
 
 ## Features
 
-- Configuration file loader for:
+- [Configuration file](https://kdeldycke.github.io/click-extra/config.html) loader for:
   - `TOML`
   - `YAML`
   - `JSON`, with inline and block comments (Python-style `#` and Javascript-style `//`)
   - `INI`, with extended interpolation, multi-level sections and non-native types (`list`, `set`, …)
   - `XML`
 - Automatic inference of the configuration file structure from your CLI's options
-- Remote loading of configuration files from URLs
-- Optional strict validation of configuration
-- Search of configuration file from default user folder and glob patterns
-- Respect of `CLI` > `Configuration` > `Environment` > `Defaults` precedence
-- `--show-params` option to debug parameters defaults, values, environment variables and provenance
-- Colorization of help screens
+- Remote loading of [configuration files from URLs](https://kdeldycke.github.io/click-extra/config.html#remote-url)
+- Optional [strict validation](https://kdeldycke.github.io/click-extra/config.html#strictness) of configuration
+- Respect the [default application path](https://kdeldycke.github.io/click-extra/config.html#default-folder) on each platform (XDG spec on Linux)
+- [Glob search patterns](https://kdeldycke.github.io/click-extra/config.html#pattern-matching) for configuration files
+- Respect of `CLI` > `Configuration` > `Environment` > `Defaults` [precedence](https://kdeldycke.github.io/click-extra/config.html#precedence)
+- Normalization and discoverability of environment variables
+- [`--show-params` option](https://kdeldycke.github.io/click-extra/config.html#show-params-option) to debug parameters defaults, values, environment variables and provenance
+- [Colorization of help screens](https://kdeldycke.github.io/click-extra/colorize.html) at the semantic-level of options, parameters, subheadings, choices, metavars and defaults
+- Global `show_envvar` option to display all environment variables in help screens
 - `-h`/`--help` option names (see [rant on other inconsistencies](https://blog.craftyguy.net/cmdline-help/))
 - `--color`/`--no-color` option flag
 - `--telemetry`/`--no-telemetry` flag to opt-in/out of tracking code
 - Recognize traditional environment variable conventions:
   - `NO_COLOR` from [`no-color.org`](https://no-color.org)
   - `DO_NOT_TRACK` from [`consoledonottrack.com`](https://consoledonottrack.com)
 - Colored `--version` option
-- Colored `--verbosity` option and logs
+- [Colored `--verbosity` option and logs](https://kdeldycke.github.io/click-extra/logging.html)
 - `--time`/`--no-time` flag to measure duration of command execution
-- Platform recognition utilities (macOS, Linux, Windows, UNIX, \*BSD, …)
+- Global `show_choices` to activate selection of choices on user input prompts
+- [Platform recognition](https://kdeldycke.github.io/click-extra/platforms.html) utilities (macOS, Linux, Windows, UNIX, \*BSD, …)
 - New conditional markers for `pytest`:
   - `@skip_linux`, `@skip_macos` and `@skip_windows`
   - `@unless_linux`, `@unless_macos` and `@unless_windows`
   - `@destructive` and `@non_destructive`
 - [`.. click:example::` and `.. click:run::` Sphinx directives](https://kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and their execution
 - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell session and console output
 - Pygments styles and filters for ANSI rendering
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: click-extra Version: 4.0.0 Summary: ð Extra
+Metadata-Version: 2.1 Name: click-extra Version: 4.1.0 Summary: ð Extra
 colorization and configuration loading for Click. Home-page: https://
 github.com/kdeldycke/click-extra License: GPL-2.0-or-later Keywords: ansi-
 colors,cli,cloup,colorization,configuration,console,ini,json,logging,multiplatform,pygments,pytest,python,python-
 tabulate,sphinx,terminal,toml,xml,yaml Author: Kevin Deldycke Author-email:
 kevin@deldycke.com Requires-Python: >=3.8,<4.0 Classifier: Development Status
 :: 5 - Production/Stable Classifier: Environment :: Console Classifier:
 Environment :: Plugins Classifier: Framework :: Pytest Classifier: Framework ::
@@ -21,15 +21,15 @@
 Classifier: Topic :: System :: Shells Classifier: Topic :: Terminals
 Classifier: Topic :: Text Processing :: Filters Classifier: Topic :: Text
 Processing :: Markup :: HTML Classifier: Topic :: Text Processing :: Markup ::
 Markdown Classifier: Topic :: Text Processing :: Markup :: XML Classifier:
 Topic :: Text Processing :: Markup :: reStructuredText Classifier: Topic ::
 Utilities Classifier: Typing :: Typed Requires-Dist: Pallets-Sphinx-Themes
 (>=2.1.0,<3.0.0) Requires-Dist: boltons (>=23.0.0,<24.0.0) Requires-Dist: click
-(>=8.1.3,<9.0.0) Requires-Dist: cloup (>=2.0.0.post1,<3.0.0) Requires-Dist:
+(>=8.1,<9.0) Requires-Dist: cloup (>=2.0.0.post1,<3.0.0) Requires-Dist:
 commentjson (>=0.9.0,<0.10.0) Requires-Dist: furo (>=2023.03.27,<2024.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0) Requires-Dist: pygments (>=2.14,<3.0)
 Requires-Dist: pygments-ansi-color (>=0.2.0,<0.3.0) Requires-Dist: pyyaml
 (>=6.0.0,<7.0.0) Requires-Dist: regex (>=2023.3.22,<2024.0.0) Requires-Dist:
 requests (>=2.28.2,<3.0.0) Requires-Dist: sphinx (>=6,<7) Requires-Dist:
 tabulate[widechars] (>=0.9,<0.10) Requires-Dist: tomli (>=2.0.1,<3.0.0) ;
 python_version < "3.11" Requires-Dist: wcmatch (>=8.4.1,<9.0.0) Requires-Dist:
@@ -58,48 +58,61 @@
 and patches](https://kdeldycke.github.io/click-extra/issues.html) that have not
 reached upstream yet (or are unlikely to). ## Example It transforms this
 vanilla `click` CLI: ![click CLI help screen](https://github.com/kdeldycke/
 click-extra/raw/main/docs/assets/click-help-screen.png) Into this: ![click-
 extra CLI help screen](https://github.com/kdeldycke/click-extra/raw/main/docs/
 assets/click-extra-screen.png) To undestrand how we ended up with the result
 above, [go read the tutorial](https://kdeldycke.github.io/click-extra/
-tutorial.html). ## Features - Configuration file loader for: - `TOML` - `YAML`
-- `JSON`, with inline and block comments (Python-style `#` and Javascript-style
-`//`) - `INI`, with extended interpolation, multi-level sections and non-native
-types (`list`, `set`, â¦) - `XML` - Automatic inference of the configuration
-file structure from your CLI's options - Remote loading of configuration files
-from URLs - Optional strict validation of configuration - Search of
-configuration file from default user folder and glob patterns - Respect of
-`CLI` > `Configuration` > `Environment` > `Defaults` precedence - `--show-
-params` option to debug parameters defaults, values, environment variables and
-provenance - Colorization of help screens - `-h`/`--help` option names (see
-[rant on other inconsistencies](https://blog.craftyguy.net/cmdline-help/)) - `-
--color`/`--no-color` option flag - `--telemetry`/`--no-telemetry` flag to opt-
+tutorial.html). ## Features - [Configuration file](https://kdeldycke.github.io/
+click-extra/config.html) loader for: - `TOML` - `YAML` - `JSON`, with inline
+and block comments (Python-style `#` and Javascript-style `//`) - `INI`, with
+extended interpolation, multi-level sections and non-native types (`list`,
+`set`, â¦) - `XML` - Automatic inference of the configuration file structure
+from your CLI's options - Remote loading of [configuration files from URLs]
+(https://kdeldycke.github.io/click-extra/config.html#remote-url) - Optional
+[strict validation](https://kdeldycke.github.io/click-extra/
+config.html#strictness) of configuration - Respect the [default application
+path](https://kdeldycke.github.io/click-extra/config.html#default-folder) on
+each platform (XDG spec on Linux) - [Glob search patterns](https://
+kdeldycke.github.io/click-extra/config.html#pattern-matching) for configuration
+files - Respect of `CLI` > `Configuration` > `Environment` > `Defaults`
+[precedence](https://kdeldycke.github.io/click-extra/config.html#precedence) -
+Normalization and discoverability of environment variables - [`--show-params`
+option](https://kdeldycke.github.io/click-extra/config.html#show-params-option)
+to debug parameters defaults, values, environment variables and provenance -
+[Colorization of help screens](https://kdeldycke.github.io/click-extra/
+colorize.html) at the semantic-level of options, parameters, subheadings,
+choices, metavars and defaults - Global `show_envvar` option to display all
+environment variables in help screens - `-h`/`--help` option names (see [rant
+on other inconsistencies](https://blog.craftyguy.net/cmdline-help/)) - `--
+color`/`--no-color` option flag - `--telemetry`/`--no-telemetry` flag to opt-
 in/out of tracking code - Recognize traditional environment variable
 conventions: - `NO_COLOR` from [`no-color.org`](https://no-color.org) -
 `DO_NOT_TRACK` from [`consoledonottrack.com`](https://consoledonottrack.com) -
-Colored `--version` option - Colored `--verbosity` option and logs - `--time`/
-`--no-time` flag to measure duration of command execution - Platform
-recognition utilities (macOS, Linux, Windows, UNIX, \*BSD, â¦) - New
-conditional markers for `pytest`: - `@skip_linux`, `@skip_macos` and
-`@skip_windows` - `@unless_linux`, `@unless_macos` and `@unless_windows` -
-`@destructive` and `@non_destructive` - [`.. click:example::` and `.. click:
-run::` Sphinx directives](https://kdeldycke.github.io/click-extra/sphinx.html)
-to document CLI source code and their execution - [ANSI-capable Pygments
-lexers](https://kdeldycke.github.io/click-extra/pygments.html#lexers) for shell
-session and console output - Pygments styles and filters for ANSI rendering -
-[Fixes 30+ bugs](https://kdeldycke.github.io/click-extra/issues.html) from
-other Click-related projects - Rely on [`cloup`](https://github.com/janluke/
-cloup) to add: - option groups - constraints - subcommands sections - aliases -
-command suggestion (`Did you mean ?`) ## Used in Check these projects to get
-real-life examples of `click-extra` usage: - ![GitHub stars](https://
-img.shields.io/github/stars/kdeldycke/meta-package-
-manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager](https://
-github.com/kdeldycke/meta-package-manager#readme) \- A unifying CLI for
-multiple package managers. - ![GitHub stars](https://img.shields.io/github/
+Colored `--version` option - [Colored `--verbosity` option and logs](https://
+kdeldycke.github.io/click-extra/logging.html) - `--time`/`--no-time` flag to
+measure duration of command execution - Global `show_choices` to activate
+selection of choices on user input prompts - [Platform recognition](https://
+kdeldycke.github.io/click-extra/platforms.html) utilities (macOS, Linux,
+Windows, UNIX, \*BSD, â¦) - New conditional markers for `pytest`: -
+`@skip_linux`, `@skip_macos` and `@skip_windows` - `@unless_linux`,
+`@unless_macos` and `@unless_windows` - `@destructive` and `@non_destructive` -
+[`.. click:example::` and `.. click:run::` Sphinx directives](https://
+kdeldycke.github.io/click-extra/sphinx.html) to document CLI source code and
+their execution - [ANSI-capable Pygments lexers](https://kdeldycke.github.io/
+click-extra/pygments.html#lexers) for shell session and console output -
+Pygments styles and filters for ANSI rendering - [Fixes 30+ bugs](https://
+kdeldycke.github.io/click-extra/issues.html) from other Click-related projects
+- Rely on [`cloup`](https://github.com/janluke/cloup) to add: - option groups -
+constraints - subcommands sections - aliases - command suggestion (`Did you
+mean ?`) ## Used in Check these projects to get real-life examples of `click-
+extra` usage: - ![GitHub stars](https://img.shields.io/github/stars/kdeldycke/
+meta-package-manager?label=%E2%AD%90&style=flat-square) [Meta Package Manager]
+(https://github.com/kdeldycke/meta-package-manager#readme) \- A unifying CLI
+for multiple package managers. - ![GitHub stars](https://img.shields.io/github/
 stars/kdeldycke/mail-deduplicate?label=%E2%AD%90&style=flat-square) [Mail
 Deduplicate](https://github.com/kdeldycke/mail-deduplicate#readme) - A CLI to
 deduplicate similar emails. - ![GitHub stars](https://img.shields.io/github/
 stars/Sprocket-Security/fireproxng?label=%E2%AD%90&style=flat-square)
 [fireproxng](https://github.com/Sprocket-Security/fireproxng#readme) - A
 rewrite of the fireprox tool. - ![GitHub stars](https://img.shields.io/github/
 stars/hugolundin/badger?label=%E2%AD%90&style=flat-square) [badger-proxy]
```

