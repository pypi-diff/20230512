# Comparing `tmp/devcontainer_manager-1.3.2.tar.gz` & `tmp/devcontainer_manager-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcontainer_manager-1.3.2.tar", last modified: Sat Apr 29 12:56:29 2023, max compression
+gzip compressed data, was "devcontainer_manager-1.4.0.tar", last modified: Fri May 12 19:47:23 2023, max compression
```

## Comparing `devcontainer_manager-1.3.2.tar` & `devcontainer_manager-1.4.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.194977 devcontainer_manager-1.3.2/
--rw-rw-r--   0 root         (0) root         (0)     1061 2022-01-06 15:44:11.000000 devcontainer_manager-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      108 2023-04-09 12:27:48.000000 devcontainer_manager-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6285 2023-04-29 12:56:29.194977 devcontainer_manager-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5996 2023-04-09 12:55:25.000000 devcontainer_manager-1.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.190977 devcontainer_manager-1.3.2/devcontainer_manager/
--rw-r--r--   0 root         (0) root         (0)       22 2023-04-29 12:55:34.000000 devcontainer_manager-1.3.2/devcontainer_manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/__main__.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-04-09 12:25:48.000000 devcontainer_manager-1.3.2/devcontainer_manager/alias.py
--rw-r--r--   0 root         (0) root         (0)     3872 2023-04-09 12:14:41.000000 devcontainer_manager-1.3.2/devcontainer_manager/base_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.190977 devcontainer_manager-1.3.2/devcontainer_manager/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-04-29 12:53:32.000000 devcontainer_manager-1.3.2/devcontainer_manager/cli/alias.py
--rw-r--r--   0 root         (0) root         (0)     4369 2023-04-29 12:44:30.000000 devcontainer_manager-1.3.2/devcontainer_manager/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     8497 2023-04-09 12:52:29.000000 devcontainer_manager-1.3.2/devcontainer_manager/config.py
--rw-r--r--   0 root         (0) root         (0)      336 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1673 2022-12-11 13:13:18.000000 devcontainer_manager-1.3.2/devcontainer_manager/global_config.py
--rw-r--r--   0 root         (0) root         (0)      412 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.190977 devcontainer_manager-1.3.2/devcontainer_manager/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.190977 devcontainer_manager-1.3.2/devcontainer_manager/templates/{{ cookiecutter.project_path }}/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.190977 devcontainer_manager-1.3.2/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/
--rw-rw-r--   0 root         (0) root         (0)      233 2022-01-07 00:28:25.000000 devcontainer_manager-1.3.2/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/build.sh
--rw-r--r--   0 root         (0) root         (0)      240 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.Dockerfile
--rw-r--r--   0 root         (0) root         (0)     1662 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json
--rw-r--r--   0 root         (0) root         (0)     1834 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/types.py
--rw-r--r--   0 root         (0) root         (0)     1203 2022-11-13 22:15:55.000000 devcontainer_manager-1.3.2/devcontainer_manager/util.py
--rw-r--r--   0 root         (0) root         (0)     2691 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/devcontainer_manager/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-29 12:56:29.190977 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6285 2023-04-29 12:56:29.000000 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1061 2023-04-29 12:56:29.000000 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-29 12:56:29.000000 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-04-29 12:56:29.000000 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      121 2023-04-29 12:56:29.000000 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-29 12:56:29.000000 devcontainer_manager-1.3.2/devcontainer_manager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      408 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-29 12:56:29.194977 devcontainer_manager-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      991 2022-06-11 21:32:03.000000 devcontainer_manager-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/
+-rw-rw-r--   0 root         (0) root         (0)     1061 2022-01-06 15:44:11.000000 devcontainer_manager-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      108 2023-04-09 12:27:48.000000 devcontainer_manager-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6285 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5996 2023-04-09 12:55:25.000000 devcontainer_manager-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/devcontainer_manager/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-12 19:46:40.000000 devcontainer_manager-1.4.0/devcontainer_manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/devcontainer_manager/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1161 2023-05-12 19:36:15.000000 devcontainer_manager-1.4.0/devcontainer_manager/alias.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-05-01 17:41:46.000000 devcontainer_manager-1.4.0/devcontainer_manager/base_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/devcontainer_manager/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/devcontainer_manager/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2376 2023-05-12 19:42:11.000000 devcontainer_manager-1.4.0/devcontainer_manager/cli/alias.py
+-rw-r--r--   0 root         (0) root         (0)     4324 2023-04-29 20:20:31.000000 devcontainer_manager-1.4.0/devcontainer_manager/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     7672 2023-04-29 14:45:53.000000 devcontainer_manager-1.4.0/devcontainer_manager/config.py
+-rw-r--r--   0 root         (0) root         (0)      336 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/devcontainer_manager/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2023-05-12 19:42:45.000000 devcontainer_manager-1.4.0/devcontainer_manager/global_config.py
+-rw-r--r--   0 root         (0) root         (0)      412 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/devcontainer_manager/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.399062 devcontainer_manager-1.4.0/devcontainer_manager/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.399062 devcontainer_manager-1.4.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/
+-rw-rw-r--   0 root         (0) root         (0)      233 2022-01-07 00:28:25.000000 devcontainer_manager-1.4.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/build.sh
+-rw-r--r--   0 root         (0) root         (0)      240 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     1786 2023-05-12 19:44:09.000000 devcontainer_manager-1.4.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-05-12 19:47:20.000000 devcontainer_manager-1.4.0/devcontainer_manager/types.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2022-11-13 22:15:55.000000 devcontainer_manager-1.4.0/devcontainer_manager/util.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/devcontainer_manager/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6285 2023-05-12 19:47:23.000000 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-05-12 19:47:23.000000 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 19:47:23.000000 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-12 19:47:23.000000 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      121 2023-05-12 19:47:23.000000 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-12 19:47:23.000000 devcontainer_manager-1.4.0/devcontainer_manager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      408 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-12 19:47:23.403062 devcontainer_manager-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      991 2022-06-11 21:32:03.000000 devcontainer_manager-1.4.0/setup.py
```

### Comparing `devcontainer_manager-1.3.2/LICENSE` & `devcontainer_manager-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.2/PKG-INFO` & `devcontainer_manager-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devcontainer_manager
-Version: 1.3.2
+Version: 1.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/gnox/devcontainer-manager
 Author: gnox
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `devcontainer_manager-1.3.2/README.md` & `devcontainer_manager-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.2/devcontainer_manager/alias.py` & `devcontainer_manager-1.4.0/devcontainer_manager/alias.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,13 +22,16 @@
         if isinstance(alias, Path):
             alias = alias.as_posix()
         return alias in self.aliases
 
     def resolve(self, alias: str):
         if isinstance(alias, Path):
             alias = alias.as_posix()
-        return self.aliases.get(alias, alias)
+        alias_path = self.aliases.get(alias, alias)
+        if not alias_path.is_absolute():
+            alias_path = self.config_path.parent / alias_path
+        return alias_path
 
     def path_to_alias(self, path: Path):
         path = path.resolve()
         ret = [k for k, p in self.aliases.items() if p.resolve() == path][0]
         return path if not ret else ret
```

### Comparing `devcontainer_manager-1.3.2/devcontainer_manager/base_config.py` & `devcontainer_manager-1.4.0/devcontainer_manager/base_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, Iterable, List, Optional, Type, TypeVar, Union
 
 from pydantic import BaseModel, Field, validator
 from pydantic.fields import ModelField
 from pydantic_yaml import YamlModel
 
-from .util import dict_merge
+from .util import dict_merge, render_recursive_template
 from .yaml import yaml
 
 if TYPE_CHECKING:
     Model = TypeVar("Model", bound="BaseModel")
 
 
 def default_if_none(cls, v, field: ModelField):
@@ -20,32 +20,37 @@
         if field.default_factory is not None:
             return field.default_factory()
     else:
         return v
 
 
 class BaseYamlConfigModel(YamlModel):
-    config_path: Path = Field(Path("."), exclude=True)
+    config_path: Path = Field(Path(".").absolute(), exclude=True)
 
     def __or__(self, other: "Model") -> "Model":
         return type(self).parse_obj(
             dict_merge(
                 self.dict(exclude={"config_path": {}}, exclude_defaults=True),
                 other.dict(exclude={"config_path": {}}, exclude_defaults=True),
             )
         )
 
     @classmethod
     def parse_file(
         cls: Type["Model"],
         path: Union[str, Path],
+        resolve: bool = False,
         **kwargs,
     ) -> "Model":
         obj = super(BaseYamlConfigModel, cls).parse_file(path, **kwargs)
-        obj.config_path = Path(path)
+        if resolve:
+            resolved = render_recursive_template(obj.json(), obj.dict())
+            obj = cls.parse_raw(resolved)
+
+        obj.config_path = Path(path).absolute()
         return obj
 
     def yaml(self, with_descriptions=False, **dict_kwargs):
         if with_descriptions:
             yaml_dict = yaml.load(self.yaml(**dict_kwargs))
             _construct_yaml_dict_with_comments(type(self), yaml_dict)
         else:
```

### Comparing `devcontainer_manager-1.3.2/devcontainer_manager/cli/alias.py` & `devcontainer_manager-1.4.0/devcontainer_manager/cli/alias.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,18 +17,26 @@
                 yield (alias, path.as_posix())
 
     return _complete
 
 
 @app.command()
 def add(alias: str = typer.Argument(...), config_path: str = typer.Argument(...)):
-    path = Path(config_path)
-    alias_config = GlobalConfig.load().load_alias_config()
-    alias_config.aliases[alias] = path.resolve().as_posix()
+    path = Path(config_path).resolve()
+    global_config = GlobalConfig.load()
+    global_config_dir = global_config.config_path.resolve().parent
+
+    alias_config = global_config.load_alias_config()
+
+    if path.as_posix().startswith(global_config_dir.as_posix()):
+        path = path.relative_to(global_config_dir)
+
+    alias_config.aliases[alias] = path
     alias_config.write_yaml()
+    typer.echo(f"Alias created: '{typer.style(alias, fg=typer.colors.BLUE)}'")
 
 
 @app.command()
 def remove(
     alias: List[str] = typer.Argument(..., autocompletion=complete_aliases("alias")),
 ):
     alias_config = GlobalConfig.load().load_alias_config()
@@ -49,15 +57,18 @@
 
 @app.command()
 def list():
     global_config = GlobalConfig.load()
     typer.echo("Available aliases:")
     aliases_msg = ""
     for alias, path in global_config.load_alias_config().aliases.items():
-        file_exists = Path(path).exists()
-        file_color = typer.colors.GREEN if file_exists else typer.colors.RED
+        path = Path(path)
+        if not path.is_absolute():
+            path = global_config.config_path.parent / path
+
+        file_color = typer.colors.GREEN if path.exists() else typer.colors.RED
         aliases_msg += (
             f"  {typer.style(alias, fg=typer.colors.BLUE)}: "
             f"{typer.style(path, fg=file_color)}"
             "\n"
         )
     typer.echo(aliases_msg)
```

### Comparing `devcontainer_manager-1.3.2/devcontainer_manager/cli/cli.py` & `devcontainer_manager-1.4.0/devcontainer_manager/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 def generate(
     templates: Optional[List[str]] = typer.Argument(
         None, autocompletion=alias.complete_aliases("templates")
     ),
     build: bool = typer.Option(False, "--build", "-b"),
     print_config: bool = typer.Option(False, "--print-config", "--print", "-p"),
 ):
-    global_config = GlobalConfig.load(create_if_not_exist=True)
+    global_config: GlobalConfig = GlobalConfig.load(create_if_not_exist=True)
     alias_config = global_config.load_alias_config()
     from_override = not templates
 
     if from_override:
         template_path = global_config.defaults.project_path / global_config.override_config_path
         overrides_exist = template_path.exists()
         path_color = typer.colors.GREEN if overrides_exist else typer.colors.RED
@@ -89,28 +89,29 @@
         global_template = True
         path = path.with_suffix(".yaml")
 
     if global_template:
         if global_config.template_dir.is_absolute():
             typer.echo("Error: --local not specified but path is absolute", err=True)
             raise typer.Exit(1)
-        path = global_config.config_path.parent / global_config.template_dir / path
+        template_dir = global_config.template_dir
+        if not template_dir.is_absolute():
+            template_dir = global_config.config_path.parent.absolute() / template_dir
+
+        path = template_dir / path
 
     if path.exists() and not force:
         if not typer.confirm(f"Config '{path}' already exists, overwrite?"):
             raise typer.Exit(1)
 
     Config().write_yaml(path, with_descriptions=with_descriptions)
     typer.echo(f"Config written to '{typer.style(path, typer.colors.GREEN)}'")
 
     if global_template:
-        alias_config = global_config.load_alias_config()
-        alias_config.aliases[path.stem] = path.as_posix()
-        alias_config.write_yaml()
-        typer.echo(f"Alias created: '{typer.style(path.stem, fg=typer.colors.BLUE)}'")
+        alias.add(path.stem, path.as_posix())
 
 
 @app.command()
 def version():
     typer.echo(__version__)
```

### Comparing `devcontainer_manager-1.3.2/devcontainer_manager/config.py` & `devcontainer_manager-1.4.0/devcontainer_manager/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -122,61 +122,39 @@
             '- ENTRYPOINT ["fish"]'
         ),
     )
 
     _not_none = validator("*", pre=True, allow_reuse=True)(default_if_none)
 
 
-class VSCodeConfig(BaseYamlConfigModel):
-    docker_host: Optional[str] = Field(
-        None, description="corresponds to vscode option 'docker.host'"
-    )
-    options: Optional[List[str]] = Field(
-        default_factory=list,
-        description=(
-            "list of options to that will be appended to vscode settings config\n"
-            "in json) for example:\n"
-            "options:\n"
-            "  - '\"python.testing.unittestEnabled: false\"'\n"
-            "  - '\"python.testing.pytestEnabled\": true'"
-        ),
-    )
-
-    _not_none = validator("*", pre=True, allow_reuse=True)(default_if_none)
-
-    def should_create_config(self):
-        return self.docker_host is not None or bool(self.options)
-
-
 class GlobalVariables(BaseModel):
     project_root_basename: str = Field(
         default_factory=get_project_root_basename, description="root directory of current project"
     )
     uid: str = Field(default_factory=os.getuid, description="id of current user")
     login: str = Field(default_factory=os.getlogin, description="username of current user")
     hostname: str = Field(default_factory=platform.node, description="hostname of current machine")
 
     def to_readme_string(self):
         global_variables_info = []
-        for k, v in self.dict().items():
+        for k in self.dict():
             field = self.__fields__[k]
             global_variables_info.append(f"{{{{ {k} }}}}: {field.field_info.description}")
         return "\n".join(global_variables_info) + "\n"
 
 
 class Config(BaseYamlConfigModelWithBase):
     project_path: Path = Field(
         Path(),
         description=(
             "root path for current project relative to current working directory or\n"
             "absolute path"
         ),
     )
     devcontainer: Optional[DevcontainerConfig] = DevcontainerConfig()
-    # vscode: Optional[VSCodeConfig] = VSCodeConfig()
     docker: Optional[DockerConfig] = DockerConfig()
 
     _not_none = validator("*", pre=True, allow_reuse=True)(default_if_none)
 
     def resolve(self, config_path: Path = None) -> "ResolvedConfig":
         values = self.dict()
         values.update(GlobalVariables().dict())
@@ -196,15 +174,14 @@
 
     @classmethod
     def none(cls):
         return Config.construct(
             base_config=None,
             devcontainer=DevcontainerConfig.none(),
             docker=DockerConfig.none(),
-            vscode=VSCodeConfig.none(),
         )
 
 
 class ResolvedConfig(Config):
     @root_validator
     def validate_nested(cls, values):
         cls._validate_docker_path(values)
```

### Comparing `devcontainer_manager-1.3.2/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json` & `devcontainer_manager-1.4.0/devcontainer_manager/templates/{{ cookiecutter.project_path }}/.devcontainer/devcontainer.json`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,26 @@
         {%- if loop.first -%}
         ,
         {%- endif %}
         "{{ arg }}",
         {%- endfor %}
     ],
     {%- if cookiecutter.devcontainer.extensions|length > 0 %}
-    "extensions": [
-        {%- for extension in cookiecutter.devcontainer.extensions %}
-        "{{ extension }}"
-        {%- if not loop.last -%}
-        ,
-        {%- endif %}
-        {%- endfor %}
-    ],
+    "customizations": {
+        "vscode": {
+            "extensions": [
+                {%- for extension in cookiecutter.devcontainer.extensions %}
+                "{{ extension }}"
+                {%- if not loop.last -%}
+                ,
+                {%- endif %}
+                {%- endfor %}
+            ]
+        }
+    },
     {%- endif %}
     {%- if cookiecutter.devcontainer.shutdown_action is not none %}
     "shutdownAction": "{{ cookiecutter.devcontainer.shutdown_action }}"
     {%- endif %}
     {%- for option in cookiecutter.devcontainer.additional_options %}
     {%- if loop.first -%}
     ,
```

### Comparing `devcontainer_manager-1.3.2/devcontainer_manager/types.py` & `devcontainer_manager-1.4.0/devcontainer_manager/types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 from typing import Optional
 
+from . import __version__
+
 DEVCONTAINER_MOUNT_STR_REGEX = re.compile(r"^src=(?P<src>.+),dst=(?P<dst>.+)(?P<args>,.+)?")
 SIMPLE_MOUNT_REGEX = re.compile(r"(?P<src>.+):(?P<dst>.+)")
 
 
 class MountString(str):
     __slots__ = ("src", "dst")
 
@@ -61,7 +63,63 @@
     def to_devcontainer_format(self):
         return MountString(
             f"src={self.src}," f"dst={self.dst}," "type=bind,consistency=cached",
         )
 
     def __repr__(self) -> str:
         return f"MountString({self})"
+
+class Version(str):
+    __slots__ = ("major", "minor", "patch")
+
+    def __new__(cls, v: Optional[str], **kwargs):
+        return str.__new__(cls, v if v is not None else cls.build(**kwargs))
+
+    def __init__(
+        self,
+        version: str = __version__,
+        *,
+        major: int = None,
+        minor: int = None,
+        patch: int = None,
+    ):
+        str.__init__(version)
+        if major is None or minor is None or patch is None:
+            arg_dict = type(self).validate_string(version)
+            major = arg_dict["major"]
+            minor = arg_dict["minor"]
+            patch = arg_dict["patch"]
+
+        self.major = major
+        self.minor = minor
+        self.patch = patch
+
+    @classmethod
+    def validate_string(cls, version_string: str):
+        version_parts = version_string.split(".")
+        if len(version_parts) != 3:
+            raise ValueError(f"Invalid version string: {version_string}")
+
+        major, minor, patch = version_parts
+        return dict(major=major, minor=minor, patch=patch)
+
+    @classmethod
+    def __get_validators__(cls):
+        yield cls.validate
+
+    @classmethod
+    def validate(cls, value: str):
+        if value.__class__ == cls:
+            return value
+
+        if not isinstance(value, str):
+            raise TypeError("version must be string")
+
+        return cls(value, **cls.validate_string(value))
+
+    @classmethod
+    def build(cls, *, major: int, minor: int, patch: int):
+        return f"{major}.{minor}.{patch}"
+
+
+    def __repr__(self) -> str:
+        return f"{self.__class__.__qualname__}({self})"
```

### Comparing `devcontainer_manager-1.3.2/devcontainer_manager/util.py` & `devcontainer_manager-1.4.0/devcontainer_manager/util.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.2/devcontainer_manager/yaml.py` & `devcontainer_manager-1.4.0/devcontainer_manager/yaml.py`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.2/devcontainer_manager.egg-info/PKG-INFO` & `devcontainer_manager-1.4.0/devcontainer_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devcontainer-manager
-Version: 1.3.2
+Version: 1.4.0
 Summary: UNKNOWN
 Home-page: https://github.com/gnox/devcontainer-manager
 Author: gnox
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `devcontainer_manager-1.3.2/devcontainer_manager.egg-info/SOURCES.txt` & `devcontainer_manager-1.4.0/devcontainer_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devcontainer_manager-1.3.2/setup.py` & `devcontainer_manager-1.4.0/setup.py`

 * *Files identical despite different names*

