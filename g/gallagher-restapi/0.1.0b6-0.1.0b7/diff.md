# Comparing `tmp/gallagher_restapi-0.1.0b6.tar.gz` & `tmp/gallagher_restapi-0.1.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gallagher_restapi-0.1.0b6.tar", max compression
+gzip compressed data, was "gallagher_restapi-0.1.0b7.tar", max compression
```

## Comparing `gallagher_restapi-0.1.0b6.tar` & `gallagher_restapi-0.1.0b7.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      478 2023-02-28 13:10:35.763716 gallagher_restapi-0.1.0b6/gallagher_restapi/__init__.py
--rw-r--r--   0        0        0     3871 2023-04-27 13:33:38.065231 gallagher_restapi-0.1.0b6/gallagher_restapi/__main__.py
--rw-r--r--   0        0        0     9578 2023-04-27 13:29:58.793058 gallagher_restapi-0.1.0b6/gallagher_restapi/client.py
--rw-r--r--   0        0        0      408 2023-02-17 07:35:07.879731 gallagher_restapi-0.1.0b6/gallagher_restapi/exceptions.py
--rw-r--r--   0        0        0    22956 2023-04-27 13:27:39.116922 gallagher_restapi-0.1.0b6/gallagher_restapi/models.py
--rw-r--r--   0        0        0      382 2023-04-27 13:34:54.533282 gallagher_restapi-0.1.0b6/pyproject.toml
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 gallagher_restapi-0.1.0b6/setup.py
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 gallagher_restapi-0.1.0b6/PKG-INFO
+-rw-r--r--   0        0        0      478 2023-05-12 05:56:23.035117 gallagher_restapi-0.1.0b7/gallagher_restapi/__init__.py
+-rw-r--r--   0        0        0     3712 2023-05-12 09:18:44.285290 gallagher_restapi-0.1.0b7/gallagher_restapi/__main__.py
+-rw-r--r--   0        0        0     9338 2023-05-12 09:14:19.249566 gallagher_restapi-0.1.0b7/gallagher_restapi/client.py
+-rw-r--r--   0        0        0      408 2023-05-12 05:56:23.035117 gallagher_restapi-0.1.0b7/gallagher_restapi/exceptions.py
+-rw-r--r--   0        0        0    22102 2023-05-12 09:22:15.429173 gallagher_restapi-0.1.0b7/gallagher_restapi/models.py
+-rw-r--r--   0        0        0      382 2023-05-12 09:25:17.268835 gallagher_restapi-0.1.0b7/pyproject.toml
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 gallagher_restapi-0.1.0b7/PKG-INFO
```

### Comparing `gallagher_restapi-0.1.0b6/gallagher_restapi/__main__.py` & `gallagher_restapi-0.1.0b7/gallagher_restapi/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,42 +19,38 @@
             cardholder_client = gallagher_restapi.CardholderClient(
                 host=host,
                 port=port,
                 api_key=api_key,
                 httpx_client=httpx_client,
             )
             await cardholder_client.authenticate()
-            pdfs = await cardholder_client.get_personal_data_field(
-                extra_fields=["unique"]
-            )
-            _LOGGER.info(len(pdfs))
-            # await cardholder_client.get_item_types()
-            # if divisions := await cardholder_client.get_item(
-            #     cardholder_client.item_types["Division"], "ICAD"
-            # ):
-            #     _LOGGER.info(divisions[0])
-            #     new_cardholder = FTCardholder(
-            #         firstName="Rami",
-            #         lastName="1",
-            #         division=FTItemReference(href=divisions[0].href),
-            #     )
-            #     if await cardholder_client.create_cardholder(new_cardholder):
-            #         _LOGGER.info("New cardholder created successfully.")
+            await cardholder_client.get_item_types()
+            if divisions := await cardholder_client.get_item(
+                cardholder_client.item_types["Division"], "ICAD"
+            ):
+                _LOGGER.info(divisions[0])
+                # new_cardholder = FTCardholder(
+                #     firstName="Rami",
+                #     lastName="1",
+                #     division=FTItemReference(href=divisions[0].href),
+                # )
+                # if await cardholder_client.create_cardholder(new_cardholder):
+                #     _LOGGER.info("New cardholder created successfully.")
     except gallagher_restapi.GllApiError as err:
         _LOGGER.error(err)
     try:
         async with httpx.AsyncClient(verify=False) as httpx_client:
             cardholder_client = gallagher_restapi.CardholderClient(
                 host=host,
                 port=port,
                 api_key=api_key,
                 httpx_client=httpx_client,
             )
             await cardholder_client.authenticate()
-            if cardholders := await cardholder_client.get_cardholder():
+            if cardholders := await cardholder_client.get_cardholder(detailed=True):
                 _LOGGER.info(
                     "Successfully connected to Gallagher server"
                     "and retrieved %s cardholders",
                     len(cardholders),
                 )
     except gallagher_restapi.GllApiError as err:
         _LOGGER.error(err)
```

### Comparing `gallagher_restapi-0.1.0b6/gallagher_restapi/client.py` & `gallagher_restapi-0.1.0b7/gallagher_restapi/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     FTApiFeatures,
     FTCardholder,
     FTEvent,
     FTEventGroup,
     FTItem,
     FTItemReference,
     FTITemTypes,
-    FTPersonalDataFieldDefinition,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class BaseClient:
     """Gallagher REST api base client."""
@@ -103,15 +102,15 @@
         response = await self._async_request("GET", f"{self.server_url}/api/")
         self.api_features = FTApiFeatures(**response["features"])
 
     async def get_item_types(self) -> None:
         """Get FTItem types."""
         item_types: list[str] = []
         response = await self._async_request(
-            "GET", self.api_features.href("items/item_types")
+            "GET", self.api_features.href("items/itemTypes")
         )
         if response.get("itemTypes"):
             item_types = [
                 item_type["name"]
                 for item_type in response["itemTypes"]
                 if item_type["name"]
             ]
@@ -132,31 +131,25 @@
             items = [FTItem(**item) for item in response["results"]]
         return items
 
 
 class CardholderClient(BaseClient):
     """REST api cardholder client for Gallagher Command Center."""
 
-    async def get_personal_data_field(
-        self, name: str | None = None, extra_fields: list[str] = []
-    ) -> list[FTItem]:
+    async def get_personal_data_field(self, name: str | None = None) -> list[FTItem]:
         """Return List of available personal data fields."""
         pdfs: list[FTItem] = []
-        extra_fields.append("defaults")
-        params = {"fields": ",".join(extra_fields)}
+        params = {}
         if name:
             params = {"name": name}
 
         if response := await self._async_request(
             "GET", self.api_features.href("personalDataFields"), params=params
         ):
-            pdfs = [
-                FTPersonalDataFieldDefinition.from_dict(pdf)
-                for pdf in response["results"]
-            ]
+            pdfs = [FTItem(**pdf) for pdf in response]
 
         return pdfs
 
     async def get_cardholder(
         self,
         *,
         ftitem_id: int | None = None,
```

### Comparing `gallagher_restapi-0.1.0b6/gallagher_restapi/models.py` & `gallagher_restapi-0.1.0b7/gallagher_restapi/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,22 +58,22 @@
         except ValueError:
             raise ValueError("Incorrect syntax of feature.")
 
         if not (attr := getattr(self, main_feature)):
             raise ValueError(f"{main_feature} is not a valid feature")
         if sub_feature and sub_feature not in attr:
             raise ValueError(f"{sub_feature} is not found in {main_feature}")
-        return attr[main_feature or sub_feature]["href"]
+        return attr[sub_feature or main_feature]["href"]
 
 
 @dataclass
 class FTItemReference:
     """FTItem reference class."""
 
-    href: str = field(default_factory=str)
+    href: str = ""
 
 
 @dataclass
 class FTStatus:
     """FTStatus class."""
 
     value: str
@@ -89,36 +89,36 @@
 
 
 @dataclass
 class FTItem:
     """FTItem class."""
 
     id: str
-    name: str
-    href: str = field(default_factory=str)
-    type: dict = field(default_factory=dict)
+    name: str = ""
+    href: str = ""
+    type: dict = ""
 
 
 @dataclass
 class FTLinkItem:
     """FTLinkItem class."""
 
     name: str
-    href: str = field(default_factory=str)
+    href: str = ""
 
 
 @dataclass
 class FTAccessGroupMembership:
     """FTAccessGroupMembership base class."""
 
     status: FTStatus = field(init=False)
     access_group: FTLinkItem = field(init=False)
     active_from: datetime = field(init=False)
     active_until: datetime = field(init=False)
-    href: str = field(default_factory=str)
+    href: str = ""
 
     @property
     def as_dict(self) -> dict[str, Any]:
         """Return json string for post and update."""
         _dict: dict[str, Any] = {"accessgroup": {"href": self.href}}
         if self.active_from:
             _dict["from"] = f"{self.active_from.isoformat()}Z"
@@ -225,50 +225,32 @@
         if active_until := kwargs.get("until"):
             _cls.active_until = datetime.fromisoformat(active_until[:-1]).replace(
                 tzinfo=pytz.utc
             )
         return _cls
 
 
-@dataclass(init=False)
-class FTPersonalDataFieldDefinition:
-    """FTPersonalDataFieldDefinition class."""
+@dataclass
+class FTPersonalDataDefinition:
+    """FTPersonalDataDefinition class."""
 
     id: str
     name: str
-    description: str
     type: str
-    division: FTItemReference | None = None
-    default: str = field(default_factory=str)
-    href: str = field(default_factory=str)
-    required: bool = False
-    unique: bool = False
-    accessGroups: list[FTLinkItem] = field(default_factory=list)
-    regex: str = ""
-    regexDescription: str = ""
-    contentType: str = ""
-    isProfileImage: bool = False
-
-    @classmethod
-    def from_dict(cls, kwargs: dict[str, Any]) -> FTPersonalDataFieldDefinition:
-        """Return FTPersonalDataFieldDefinition object from dict."""
-        _cls = FTPersonalDataFieldDefinition()
-        for key, value in kwargs.items():
-            setattr(_cls, key, value)
-        return _cls
+    href: str = ""
 
 
 @dataclass
 class FTCardholderPdfValue:
     """FTCardholderPdfValue class."""
 
     name: str
     value: str | FTItemReference = field(init=False)
     notifications: bool = field(init=False)
-    definition: FTItem = field(init=False)
+    definition: FTPersonalDataDefinition = field(init=False)
     href: str = field(init=False)
 
     @property
     def as_dict(self) -> dict[str, Any]:
         """Return json string for post and update."""
         return {f"@{self.name}": {"notifications": self.notifications}}
 
@@ -321,15 +303,15 @@
         from_dict=lambda val: datetime.fromisoformat(val[:-1]).replace(tzinfo=pytz.utc),
     ),
     FTCardholderField(
         name="lastSuccessfulAccessZone",
         from_dict=lambda val: FTLinkItem(**val),
     ),
     FTCardholderField(name="serverDisplayName"),
-    FTCardholderField(name="division", from_dict=lambda val: FTItemReference(**val)),
+    FTCardholderField(name="division", from_dict=lambda val: FTItem(**val)),
     FTCardholderField(name="disableCipherPad"),
     FTCardholderField(name="usercode"),
     FTCardholderField(name="operatorLoginEnabled"),
     FTCardholderField(name="operatorUsername"),
     FTCardholderField(name="operatorPassword"),
     FTCardholderField(name="operatorPasswordExpired"),
     FTCardholderField(name="windowsLoginEnabled"),
@@ -461,15 +443,15 @@
 
 # Gallagher alarm and event models
 @dataclass
 class FTAlarm:
     """FTAlarm summary class"""
 
     state: str
-    href: str = field(default_factory=str)
+    href: str = ""
 
 
 @dataclass
 class FTEventCard:
     """Event card details."""
 
     number: str
@@ -488,15 +470,15 @@
 
 @dataclass
 class FTEventGroup:
     """FTEvent group class."""
 
     id: str
     name: str
-    href: str = field(default_factory=str)
+    href: str = ""
     event_types: list[FTItem] = field(init=False)
 
     @classmethod
     def from_dict(cls, kwargs: dict[str, Any]) -> FTEventGroup:
         """Return Event card object from dict."""
         event_types = kwargs.pop("eventTypes")
         _cls = FTEventGroup(**kwargs)
```

