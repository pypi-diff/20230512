# Comparing `tmp/pydrawise-2023.1.4.tar.gz` & `tmp/pydrawise-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydrawise-2023.1.4.tar", last modified: Mon Jan  9 03:22:12 2023, max compression
+gzip compressed data, was "pydrawise-2023.5.0.tar", last modified: Fri May 12 02:26:47 2023, max compression
```

## Comparing `pydrawise-2023.1.4.tar` & `pydrawise-2023.5.0.tar`

### file list

```diff
@@ -1,24 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 03:22:12.491109 pydrawise-2023.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-09 03:21:59.000000 pydrawise-2023.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-01-09 03:22:12.491109 pydrawise-2023.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-01-09 03:21:59.000000 pydrawise-2023.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 03:22:12.487109 pydrawise-2023.1.4/pydrawise/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-01-09 03:21:59.000000 pydrawise-2023.1.4/pydrawise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-01-09 03:21:59.000000 pydrawise-2023.1.4/pydrawise/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5390 2023-01-09 03:21:59.000000 pydrawise-2023.1.4/pydrawise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-01-09 03:21:59.000000 pydrawise-2023.1.4/pydrawise/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-01-09 03:21:59.000000 pydrawise-2023.1.4/pydrawise/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 03:22:12.491109 pydrawise-2023.1.4/pydrawise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-01-09 03:22:12.000000 pydrawise-2023.1.4/pydrawise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-01-09 03:22:12.000000 pydrawise-2023.1.4/pydrawise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 03:22:12.000000 pydrawise-2023.1.4/pydrawise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-09 03:22:12.000000 pydrawise-2023.1.4/pydrawise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-09 03:22:12.000000 pydrawise-2023.1.4/pydrawise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 03:22:12.000000 pydrawise-2023.1.4/pydrawise.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 03:22:12.491109 pydrawise-2023.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-01-09 03:21:59.000000 pydrawise-2023.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 03:22:12.491109 pydrawise-2023.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 03:21:59.000000 pydrawise-2023.1.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-01-09 03:21:59.000000 pydrawise-2023.1.4/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-09 03:21:59.000000 pydrawise-2023.1.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-09 03:21:59.000000 pydrawise-2023.1.4/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.937234 pydrawise-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.933234 pydrawise-2023.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.933234 pydrawise-2023.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.github/workflows/publish-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.933234 pydrawise-2023.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-12 02:26:47.937234 pydrawise-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/hydrawise.graphql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.933234 pydrawise-2023.5.0/pydrawise/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pydrawise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pydrawise/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pydrawise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pydrawise/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10729 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pydrawise/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.937234 pydrawise-2023.5.0/pydrawise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 02:26:47.000000 pydrawise-2023.5.0/pydrawise.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 02:26:47.937234 pydrawise-2023.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:47.937234 pydrawise-2023.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-12 02:26:31.000000 pydrawise-2023.5.0/tests/test_schema.py
```

### Comparing `pydrawise-2023.1.4/LICENSE` & `pydrawise-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.1.4/PKG-INFO` & `pydrawise-2023.5.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2023.1.4
+Version: 2023.5.0
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
-Home-page: https://github.com/dknowles2/pydrawise
-Download-URL: https://github.com/dknowles2/pydrawise/tarball/2023.1.4
-Author: David Knowles
-Author-email: dknowles2@gmail.com
+Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/dknowles2/pydrawise
+Project-URL: Source Code, https://github.com/dknowles2/pydrawise
+Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
-Classifier: Programming Language :: Python :: 3.9
+Platform: any
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pydrawise
 Python 3 library for interacting with Hydrawise sprinkler controllers.
```

### Comparing `pydrawise-2023.1.4/README.md` & `pydrawise-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.1.4/pydrawise/schema.py` & `pydrawise-2023.5.0/pydrawise/schema.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from collections import namedtuple
 from dataclasses import dataclass, field, fields, is_dataclass
 from datetime import datetime, timedelta, timezone
-from enum import auto, Enum
+from enum import Enum, auto
 from functools import cache
 from typing import (
     Iterator,
     List,
     Optional,
     Type,
     Union,
@@ -24,41 +24,28 @@
 from apischema.graphql import graphql_schema
 from apischema.metadata import conversion, skip
 from apischema.metadata.keys import CONVERSION_METADATA, SKIP_METADATA
 from apischema.utils import to_camel_case
 from gql.dsl import DSLField, DSLInlineFragment, DSLSchema
 from graphql import GraphQLSchema
 
-from .auth import Auth
-from .exceptions import NotAuthenticatedError
-
-
 # For compatibility with < python 3.10.
 NoneType = type(None)
 
 
 def deserialize(*args, **kwargs):
     kwargs.setdefault("aliaser", to_camel_case)
     return _deserialize(*args, **kwargs)
 
 
 @cache
 def get_schema() -> GraphQLSchema:
     return graphql_schema(
-        query=[Query.me, Query.controller, Query.zone],
-        mutation=[
-            Mutation.start_zone,
-            Mutation.stop_zone,
-            Mutation.suspend_zone,
-            Mutation.resume_zone,
-            Mutation.start_all_zones,
-            Mutation.stop_all_zones,
-            Mutation.suspend_all_zones,
-            Mutation.resume_all_zones,
-        ],
+        query=[getattr(Query, m) for m in Query.__abstractmethods__],
+        mutation=[getattr(Mutation, m) for m in Mutation.__abstractmethods__],
     )
 
 
 _Field = namedtuple("_Field", ["name", "types"])
 
 
 def _fields(cls) -> Iterator[_Field]:
@@ -114,44 +101,39 @@
                     .select(*get_selectors(ds, f_type))
                 )
             ret.append(getattr(dsl_field, "select")(*sel_args))
     return ret
 
 
 class StatusCodeEnum(Enum):
-
     OK = auto()
     WARNING = auto()
     ERROR = auto()
 
 
 @dataclass
 class StatusCodeAndSummary:
-
     status: StatusCodeEnum
     summary: str
 
 
 @dataclass
 class LocalizedValueType:
-
     value: float
     unit: str
 
 
 @dataclass
 class Option:
-
     value: int
     label: str
 
 
 @dataclass
 class DateTime:
-
     value: str
     timestamp: int
 
     @staticmethod
     def from_json(dt: DateTime) -> datetime:
         return datetime.fromtimestamp(dt.timestamp)
 
@@ -178,29 +160,26 @@
     Conversion(lambda d: timedelta(minutes=d), source=int, target=timedelta),
     Conversion(lambda d: d.minutes, source=timedelta, target=int),
 )
 
 
 @dataclass
 class CycleAndSoakSettings:
-
     cycle_duration: timedelta = field(metadata=duration_conversion)
     soak_duration: timedelta = field(metadata=duration_conversion)
 
 
 @dataclass
 class RunTimeGroup:
-
     id: int
     duration: timedelta = field(metadata=duration_conversion)
 
 
 @dataclass
 class AdvancedProgram:
-
     advanced_program_id: int
     run_time_group: RunTimeGroup
 
 
 class AdvancedProgramDayPatternEnum(Enum):
     def _generate_next_value_(name, start, count, last_values):
         return name
@@ -214,358 +193,204 @@
     FRIDAY = auto()
     SATURDAY = auto()
     SUNDAY = auto()
     DAYS = auto()
 
 
 @dataclass
-class ProgramStartTimeApplication:
+class BaseZone:
+    id: int
+    number: Option
+    name: str
 
+
+@dataclass
+class ProgramStartTimeApplication:
     all: bool
-    zones: [BaseZone]
+    zones: List[BaseZone]
 
 
 @dataclass
 class ProgramStartTime:
-
     id: int
     time: str  # e.g. "02:00"
     watering_days: list[AdvancedProgramDayPatternEnum]
 
 
 @dataclass
 class WateringSettings:
-
     fixed_watering_adjustment: int
     cycle_and_soak_settings: Optional[CycleAndSoakSettings]
 
 
 @dataclass
 class AdvancedWateringSettings(WateringSettings):
-
     advanced_program: Optional[AdvancedProgram]
 
 
 @dataclass
 class StandardProgram:
-
     name: str
     start_times: list[str]
 
 
 @dataclass
 class StandardProgramApplication:
-
     zone: BaseZone
     standard_program: StandardProgram
     run_time_group: RunTimeGroup
 
 
 @dataclass
 class StandardWateringSettings(WateringSettings):
-
     standard_program_applications: list[StandardProgramApplication]
 
 
 @dataclass
 class RunStatus:
-
     value: int
     label: str
 
 
 @dataclass
 class ScheduledZoneRun:
-
     id: str
     start_time: datetime = field(metadata=DateTime.conversion())
     end_time: datetime = field(metadata=DateTime.conversion())
     normal_duration: timedelta = field(metadata=duration_conversion)
     duration: timedelta = field(metadata=duration_conversion)
     status: RunStatus
 
 
 @dataclass
 class ScheduledZoneRuns:
-
     summary: str
     current_run: Optional[ScheduledZoneRun]
     next_run: Optional[ScheduledZoneRun]
     status: Optional[str]
 
 
 @dataclass
 class PastZoneRuns:
-
     last_run: Optional[ScheduledZoneRun]
     runs: list[ScheduledZoneRun]
 
 
 @dataclass
 class ZoneStatus:
-
     relative_water_balance: int
     suspended_until: datetime = field(metadata=DateTime.conversion())
 
 
 @dataclass
 class ZoneSuspension:
-
     id: int
     start_time: datetime = field(metadata=DateTime.conversion())
     end_time: datetime = field(metadata=DateTime.conversion())
 
 
 @dataclass
-class BaseZone:
-
-    id: int
-    number: Option
-    name: str
-
-
-@dataclass
 class Zone(BaseZone):
-
     watering_settings: Union[AdvancedWateringSettings, StandardWateringSettings]
     scheduled_runs: ScheduledZoneRuns
     past_runs: PastZoneRuns
     status: ZoneStatus
     suspensions: list[ZoneSuspension] = field(default_factory=list)
 
-    _auth: Optional[Auth] = field(
-        default=None,
-        init=False,
-        repr=False,
-        metadata=skip(serialization=True, deserialization=True),
-    )
-
-    async def start(
-        self,
-        mark_run_as_scheduled: bool = False,
-        custom_run_duration: Optional[int] = None,
-    ):
-        if not self._auth:
-            raise NotAuthenticatedError
-        ds = DSLSchema(get_schema())
-        kwargs = {
-            "zoneId": self.id,
-            "markRunAsScheduled": mark_run_as_scheduled,
-        }
-        if custom_run_duration is not None:
-            kwargs["customRunDuration"] = custom_run_duration
-
-        selector = ds.Mutation.startZone.args(**kwargs).select(
-            *get_selectors(ds, StatusCodeAndSummary),
-        )
-        await self._auth.mutation(selector)
-
-    async def stop(self) -> None:
-        if not self._auth:
-            raise NotAuthenticatedError
-        ds = DSLSchema(get_schema())
-        selector = ds.Mutation.stopZone.args(zoneId=self.id).select(
-            *get_selectors(ds, StatusCodeAndSummary),
-        )
-        await self._auth.mutation(selector)
-
-    async def suspend(self, until: datetime) -> None:
-        if not self._auth:
-            raise NotAuthenticatedError
-        ds = DSLSchema(get_schema())
-        selector = ds.Mutation.suspendZone.args(
-            zoneId=self.id,
-            until=DateTime.to_json(until).value,
-        ).select(*get_selectors(ds, StatusCodeAndSummary))
-        await self._auth.mutation(selector)
-
-    async def resume(self) -> None:
-        if not self._auth:
-            raise NotAuthenticatedError
-        ds = DSLSchema(get_schema())
-        selector = ds.Mutation.resumeZone.args(zoneId=self.id).select(
-            *get_selectors(ds, StatusCodeAndSummary),
-        )
-        await self._auth.mutation(selector)
-
 
 @dataclass
 class ControllerFirmware:
-
     type: str
     version: str
 
 
 @dataclass
 class ControllerModel:
-
     name: str
     description: str
 
 
 @dataclass
 class ControllerHardware:
-
     serial_number: str
     version: str
     status: str
     model: ControllerModel
     firmware: list[ControllerFirmware]
 
 
 @dataclass
 class SensorModel:
-
     id: int
     name: str
     active: bool
     off_level: int
     off_timer: int
     delay: int
     divisor: float
     flow_rate: float
 
 
 @dataclass
 class SensorStatus:
-
     water_flow: Optional[LocalizedValueType]
     active: bool
 
 
 @dataclass
 class SensorFlowSummary:
-
     total_water_volume: LocalizedValueType
 
 
 @dataclass
 class Sensor:
-
     id: int
     name: str
     model: SensorModel
     status: SensorStatus
 
 
 @dataclass
 class WaterTime:
-
     value: timedelta = field(metadata=duration_conversion)
 
 
 @dataclass
 class ControllerStatus:
-
     summary: str
     online: bool
     actual_water_time: WaterTime
     normal_water_time: WaterTime
     last_contact: Optional[DateTime] = None
 
 
 @dataclass
 class Controller:
-
     id: int
     name: str
     software_version: str
     hardware: ControllerHardware
     last_contact_time: datetime = field(metadata=DateTime.conversion())
     last_action: datetime = field(metadata=DateTime.conversion())
     online: bool
     sensors: list[Sensor]
     zones: list[Zone] = field(default_factory=list, metadata=skip(deserialization=True))
     permitted_program_start_times: list[ProgramStartTime] = field(default_factory=list)
     status: Optional[ControllerStatus] = field(default=None)
 
-    _auth: Optional[Auth] = field(
-        default=None,
-        init=False,
-        repr=False,
-        metadata=skip(serialization=True, deserialization=True),
-    )
-
-    async def get_zones(self) -> list[Zone]:
-        if not self._auth:
-            raise NotAuthenticatedError
-        ds = DSLSchema(get_schema())
-        selector = ds.Query.controller(controllerId=self.id).select(
-            ds.Controller.zones.select(*get_selectors(ds, Zone)),
-        )
-        result = await self._auth.query(selector)
-        zones = deserialize(list[Zone], result["controller"]["zones"])
-        for zone in zones:
-            zone._auth = self._auth
-        return zones
-
-    async def start_all_zones(
-        self, mark_run_as_scheduled: bool = False, custom_run_duration: int = 0
-    ) -> None:
-        if not self._auth:
-            raise NotAuthenticatedError
-        ds = DSLSchema(get_schema())
-        kwargs = {
-            "controllerId": self.id,
-            "markRunAsScheduled": mark_run_as_scheduled,
-        }
-        if custom_run_duration > 0:
-            kwargs["customRunDuration"] = custom_run_duration
-
-        selector = ds.Mutation.startAllZones.args(**kwargs).select(
-            *get_selectors(ds, StatusCodeAndSummary),
-        )
-        await self._auth.mutation(selector)
-
-    async def stop_all_zones(self) -> None:
-        if not self._auth:
-            raise NotAuthenticatedError
-        ds = DSLSchema(get_schema())
-        selector = ds.Mutation.stopAllZones.args(controllerId=self.id).select(
-            *get_selectors(ds, StatusCodeAndSummary),
-        )
-        await self._auth.mutation(selector)
-
-    async def suspend_all_zones(self, until: datetime) -> None:
-        if not self._auth:
-            raise NotAuthenticatedError
-        ds = DSLSchema(get_schema())
-        selector = ds.Mutation.suspendZone.args(
-            controllerId=self.id,
-            until=DateTime.to_json(until).value,
-        ).select(*get_selectors(ds, StatusCodeAndSummary))
-        await self._auth.mutation(selector)
-
-    async def resume_all_zones(self) -> None:
-        if not self._auth:
-            raise NotAuthenticatedError
-        ds = DSLSchema(get_schema())
-        selector = ds.Mutation.resumeAllZones.args(controllerId=self.id).select(
-            *get_selectors(ds, StatusCodeAndSummary),
-        )
-        await self._auth.mutation(selector)
-
 
 @dataclass
 class User:
-
     id: int
     name: str
     email: str
     controllers: list[Controller] = field(
         default_factory=list, metadata=skip(deserialization=True)
     )
 
-    _auth: Optional[Auth] = field(
-        default=None,
-        init=False,
-        repr=False,
-        metadata=skip(serialization=True, deserialization=True),
-    )
-
 
 class Query(ABC):
     @staticmethod
     @abstractmethod
     def me() -> User:
         ...
 
@@ -622,7 +447,12 @@
     def suspend_all_zones(controller_id: int, until: str) -> StatusCodeAndSummary:
         ...
 
     @staticmethod
     @abstractmethod
     def resume_all_zones(controller_id: int) -> StatusCodeAndSummary:
         ...
+
+    @staticmethod
+    @abstractmethod
+    def delete_zone_suspension(id: int) -> bool:
+        ...
```

### Comparing `pydrawise-2023.1.4/pydrawise.egg-info/PKG-INFO` & `pydrawise-2023.5.0/pydrawise.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2023.1.4
+Version: 2023.5.0
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
-Home-page: https://github.com/dknowles2/pydrawise
-Download-URL: https://github.com/dknowles2/pydrawise/tarball/2023.1.4
-Author: David Knowles
-Author-email: dknowles2@gmail.com
+Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/dknowles2/pydrawise
+Project-URL: Source Code, https://github.com/dknowles2/pydrawise
+Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
-Classifier: Programming Language :: Python :: 3.9
+Platform: any
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pydrawise
 Python 3 library for interacting with Hydrawise sprinkler controllers.
```

### Comparing `pydrawise-2023.1.4/tests/test_auth.py` & `pydrawise-2023.5.0/tests/test_auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import timedelta
 
 from aioresponses import aioresponses
 from freezegun import freeze_time
-from pydrawise import auth
 from pytest import fixture
 
+from pydrawise import auth
+
 
 @fixture
 def token_payload():
     return {
         "access_token": "__access-token__",
         "refresh_token": "__refresh-token__",
         "token_type": "bearer",
```

