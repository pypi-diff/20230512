# Comparing `tmp/psytricks-2.0.0.tar.gz` & `tmp/psytricks-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psytricks-2.0.0.tar", max compression
+gzip compressed data, was "psytricks-2.1.0.tar", max compression
```

## Comparing `psytricks-2.0.0.tar` & `psytricks-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.0.0/LICENSE
--rw-r--r--   0        0        0     6284 2023-05-10 19:08:40.522092 psytricks-2.0.0/README.md
--rw-r--r--   0        0        0     1045 2023-05-10 19:13:07.196941 psytricks-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       93 2023-05-10 19:13:07.200941 psytricks-2.0.0/src/psytricks/__init__.py
--rw-r--r--   0        0        0     6146 2023-05-10 19:13:07.200941 psytricks-2.0.0/src/psytricks/__ps1__/psytricks-lib.ps1
--rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/__ps1__/psytricks-wrapper.ps1
--rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/__ps1__/restricks-server.example.xml
--rw-r--r--   0        0        0    14826 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/__ps1__/restricks-server.ps1
--rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
--rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
--rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/__ps1__/sampledata/GetSessions.json
--rw-r--r--   0        0        0     6043 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/cli.py
--rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.0.0/src/psytricks/decoder.py
--rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/literals.py
--rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.0.0/src/psytricks/mappings.py
--rw-r--r--   0        0        0    21031 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/wrapper.py
--rw-r--r--   0        0        0     7094 1970-01-01 00:00:00.000000 psytricks-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.0/LICENSE
+-rw-r--r--   0        0        0     6526 2023-05-10 20:14:28.925038 psytricks-2.1.0/README.md
+-rw-r--r--   0        0        0     1045 2023-05-12 19:33:05.240400 psytricks-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-05-12 19:33:05.240400 psytricks-2.1.0/src/psytricks/__init__.py
+-rw-r--r--   0        0        0     6146 2023-05-12 19:33:05.244397 psytricks-2.1.0/src/psytricks/__ps1__/psytricks-lib.ps1
+-rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.0/src/psytricks/__ps1__/psytricks-wrapper.ps1
+-rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.0/src/psytricks/__ps1__/restricks-server.example.xml
+-rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.0/src/psytricks/__ps1__/restricks-server.ps1
+-rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
+-rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
+-rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.0/src/psytricks/__ps1__/sampledata/GetSessions.json
+-rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.0/src/psytricks/cli.py
+-rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.0/src/psytricks/decoder.py
+-rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.0/src/psytricks/literals.py
+-rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.0/src/psytricks/mappings.py
+-rw-r--r--   0        0        0    23720 2023-05-12 19:24:30.404582 psytricks-2.1.0/src/psytricks/wrapper.py
+-rw-r--r--   0        0        0     7336 1970-01-01 00:00:00.000000 psytricks-2.1.0/PKG-INFO
```

### Comparing `psytricks-2.0.0/LICENSE` & `psytricks-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psytricks-2.0.0/README.md` & `psytricks-2.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # PSytricks
 
-`P`ower`S`hell P`y`thon Ci`tri`x Tri`cks`.
+![PyPI](https://img.shields.io/pypi/v/psytricks)
+![PyPI - License](https://img.shields.io/pypi/l/psytricks)
+![pdoc](https://img.shields.io/badge/docs-pdoc-brightgreen.svg)
+![black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
-Pun intended.
+`P`ower`S`hell P`y`thon Ci`tri`x Tri`cks` - pun intended.
 
 ![logo](https://raw.githubusercontent.com/imcf/psytricks/main/resources/images/logo.png)
 
 This package provides an abstraction layer allowing Python code to interact with
 a [Citrix Virtual Apps and Desktops (CVAD)][www_cvad] stack, i.e. to fetch
 status information and trigger actions on machines and sessions. Since CVAD only
 provides a *PowerShell Snap-In* to do so, a core component written in `Windows
```

### Comparing `psytricks-2.0.0/pyproject.toml` & `psytricks-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 authors = ["Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>"]
 description = "PowerShell Python Citrix Tricks."
 license = "GPL-3.0-or-later"
 name = "psytricks"
 readme = "README.md"
-version = "2.0.0"
+version = "2.1.0"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/imcf/psytricks/blob/main/CHANGELOG.md"
 "Organisation Homepage" = "https://imcf.one/"
 "Twitter" = "https://twitter.com/imcf_basel"
 
 [tool.poetry.dependencies]
```

### Comparing `psytricks-2.0.0/src/psytricks/__ps1__/psytricks-lib.ps1` & `psytricks-2.1.0/src/psytricks/__ps1__/psytricks-lib.ps1`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <#
 
 Collection of functions and other definitions to be sourced by other scripts.
 
 #>
 
 # the version variable will be filled by poetry at build time:
-$Version = "2.0.0"
+$Version = "2.1.0"
 
 
 #region properties-selectors
 
 $MachineProperties = @(
     "AgentVersion",
     "AssociatedUserUPNs",
```

### Comparing `psytricks-2.0.0/src/psytricks/__ps1__/psytricks-wrapper.ps1` & `psytricks-2.1.0/src/psytricks/__ps1__/psytricks-wrapper.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.0.0/src/psytricks/__ps1__/restricks-server.example.xml` & `psytricks-2.1.0/src/psytricks/__ps1__/restricks-server.example.xml`

 * *Files identical despite different names*

### Comparing `psytricks-2.0.0/src/psytricks/__ps1__/restricks-server.ps1` & `psytricks-2.1.0/src/psytricks/__ps1__/restricks-server.ps1`

 * *Files 3% similar despite different names*

```diff
@@ -3,36 +3,40 @@
 # on *PowerShell Core* et al, so we strictly need the "Desktop" edition:
 #Requires -PSEdition Desktop
 
 [CmdletBinding()]
 param (
     [Parameter(
         Mandatory = $true,
-        ParameterSetName = "Start",
+        ParameterSetName = "Startup",
         HelpMessage = "The address of the Citrix Delivery Controller."
     )]
     [string]
     $AdminAddress,
 
     [Parameter(
-        ParameterSetName = "Start",
+        ParameterSetName = "Startup",
         HelpMessage = "The port to listen on (default: 8080)."
     )]
+    [Parameter(
+        ParameterSetName = "Shutdown",
+        HelpMessage = "The port to send the shutdown request to (default: 8080)."
+    )]
     [int]
     $ListenPort = 8080,
 
     [Parameter(
-        ParameterSetName = "Start",
+        ParameterSetName = "Startup",
         HelpMessage = "A logfile to use for the output (default: stdtout)."
     )]
     [string]
     $LogFile,
 
     [Parameter(
-        ParameterSetName = "Stop",
+        ParameterSetName = "Shutdown",
         HelpMessage = "Shut down the listener and terminate the script."
     )]
     [switch]
     $Shutdown
 )
 
 $ErrorActionPreference = "Stop"
@@ -75,19 +79,21 @@
     try {
         # first create the shutdown marker file:
         $StopMarker = Join-Path $env:TEMP "_shutdown_restricks_server_"
         "Terminate" | Out-File $StopMarker
 
         # now send a shutdown request to the listener with a very short timeout:
         try {
-            $null = Invoke-WebRequest "http://localhost:8080/end" -TimeoutSec 1
+            $null = Invoke-WebRequest "http://localhost:$ListenPort/end" -TimeoutSec 1
         } catch {
             # in case the request timed out this means the listener has been
             # shut down or crashed before, usually resulting in an orphaned
-            # "restricks-server.exe" process that needs to be killed explicitly:
+            # "restricks-server.exe" process that needs to be killed explicitly
+            # (use 'SilentlyContinue' in case the server was started differently
+            # or the WinSW executable has a different name):
             Stop-Process -Name "restricks-server" -ErrorAction SilentlyContinue
         }
     } catch {
         Write-Host "Issue shutting down: $_"
     } finally {
         exit
     }
@@ -140,32 +146,60 @@
     param (
         [Parameter(
             Mandatory = $true,
             HelpMessage = "The HttpListener context response object."
         )]
         $Response,
 
-        # the HTTP status code
-        [Parameter()]
+        [Parameter(HelpMessage = "The HTTP status code to send (default=200).")]
         [int]
         $StatusCode = 200,
 
-        [Parameter(HelpMessage = "The content body to return in the response.")]
-        [string]
+        [Parameter(
+            HelpMessage = 'The content body ("payload") to return in the ' + `
+                'response. For non-HTML responses (which are the default), ' + `
+                'this will be placed in the "Data" object. A "Status" ' + `
+                'object will be automatically generated from the other ' + `
+                'parameters. Needs to be serializable!'
+        )]
         $Body = "",
 
+        [Parameter(HelpMessage = "The internal execution status (0 = success).")]
+        [string]
+        $ExecutionStatus = 0,
+
+        [Parameter(HelpMessage = "An error message for the 'Status' JSON section.")]
+        [string]
+        $ErrorMesage = "",
+
         [Parameter(HelpMessage = "Use 'text/html' instead of 'application/json'.")]
         [Switch]
         $Html
     )
     $Type = "application/json"
     if ($Html) {
         $Type = "text/html"
+        $Payload = $Body
+    } else {
+        $Status = @{
+            ExecutionStatus  = $ExecutionStatus
+            ErrorMessage     = $ErrorMesage
+            ScriptName       = $ScriptName
+            ScriptPath       = $ScriptPath
+            PSyTricksVersion = $Version
+            Timestamp        = [int64](Get-Date -UFormat %s)
+        }
+
+        $Payload = @{
+            "Status" = $Status
+            "Data"   = $Body
+        } | ConvertTo-Json -Depth 4
     }
-    $Buffer = [System.Text.Encoding]::UTF8.GetBytes($Body)  # convert to bytes
+
+    $Buffer = [System.Text.Encoding]::UTF8.GetBytes($Payload)  # convert to bytes
     $Response.ContentLength64 = $Buffer.Length
     $Response.ContentType = $Type
     $Response.StatusCode = $StatusCode
     $Response.OutputStream.Write($Buffer, 0, $Buffer.Length)
     $Response.OutputStream.Close()
     Write-Host "Response sent successfully." @Green
 
@@ -217,16 +251,15 @@
         # "DisconnectAll" { throw "Not yet implemented!" }
 
         Default { throw "Invalid: $Command" }
     }
     Write-Host "Got $($BrokerData.Length) $Desc from Citrix." @Cyan
     Write-Host "Took $(($(Get-Date) - $TStart).TotalMilliseconds) ms" @Magenta
 
-    $Json = $BrokerData | ConvertTo-Json -Depth 4
-    return $Json
+    return $BrokerData
 }
 
 
 function Send-BrokerRequest {
     param (
         # the parsed URL as returned by Split-RawUrl
         [Parameter(Mandatory = $True)]
@@ -301,53 +334,52 @@
         }
 
         Default { throw "Invalid: $Command" }
     }
     Write-Host "Sent $Desc request to Citrix." @Cyan
     Write-Host "Took $(($(Get-Date) - $TStart).TotalMilliseconds) ms" @Magenta
 
-    $Json = $BrokerData | ConvertTo-Json -Depth 4
-    return $Json
+    return $BrokerData
 }
 
 
 function Switch-GetRequest {
     param (
         [Parameter()]
         $Request
     )
     Write-Host "GET> $($Request.Url)" @Blue
     $ParsedUrl = Split-RawUrl -RawUrl $Request.RawUrl
     $Command = $ParsedUrl[1]
 
     if ($Command -eq 'end') {
-        Send-Response -Response $Response -Body "Terminating." -Html
+        Send-Response -Response $Response -Body "Terminating."
         Write-Host "Received a termination request, stopping." @Red
         break
 
     } elseif ($Command -eq '') {
         $html = "<h1>$ScriptName ($Version)</h1><p>Running from: $ScriptPath</p>"
         Send-Response -Response $Response -Body $html -Html
 
     } elseif ($Command -eq 'version') {
-        $Body = @{ PSyTricksVersion = $Version } | ConvertTo-Json
-        Send-Response -Response $Response -Body $Body
+        Send-Response -Response $Response -Body ""
 
     } elseif ($GetRoutes -contains $Command) {
         try {
             $Body = Get-BrokerData -ParsedUrl $ParsedUrl
         } catch {
-            Send-Response -Response $Response -StatusCode 400 -Body $_
+            Send-Response -Response $Response -StatusCode 400 -Body $_ -Html
         }
         Send-Response -Response $Response -Body $Body
 
     } else {
         Send-Response `
             -Response $Response `
             -StatusCode 400 `
+            -Html `
             -Body "Invalid or unknown command: [$Command]"
     }
 }
 
 
 function Switch-PostRequest {
     param (
@@ -355,33 +387,34 @@
         $Request
     )
     Write-Host "POST> $($Request.Url)" @Blue
     $ParsedUrl = Split-RawUrl -RawUrl $Request.RawUrl
     $Command = $ParsedUrl[1]
 
     if (-not ($Request.HasEntityBody)) {
-        Send-Response -Response $Response -Body "No POST data." -StatusCode 400
+        Send-Response -Response $Response -Body "No POST data." -StatusCode 400 -Html
 
     } elseif ($PostRoutes -contains $Command) {
         try {
             $StreamReader = [System.IO.StreamReader]::new($Request.InputStream)
             $Content = $StreamReader.ReadToEnd()
             $Decoded = ConvertFrom-Json $Content
         } catch {
-            Send-Response $Response -Body "Error decoding JSON: $_" -StatusCode 422
+            Send-Response $Response -Body "Decoding error: $_" -StatusCode 422 -Html
             return
         }
 
         $BrokerData = Send-BrokerRequest -ParsedUrl $ParsedUrl -Payload $Decoded
         Send-Response -Response $Response -Body $BrokerData
 
     } else {
         Send-Response `
             -Response $Response `
             -StatusCode 400 `
+            -Html `
             -Body "Invalid or unknown command: [$Command]"
     }
 }
 
 
 function Start-ListenerBlocking {
     try {
@@ -391,17 +424,14 @@
         $Listener.Start()
 
         if ($Listener.IsListening) {
             Write-Host "[$(Format-Date)] $ScriptName listening: $Prefix" @Yellow
         }
 
         while ($Listener.IsListening) {
-            if ([Console]::KeyAvailable) {
-                Write-Host "Hey!"
-            }
             try {
                 # when a request is made GetContext() will return it as an object:
                 $Context = $Listener.GetContext()
 
                 $Request = $Context.Request
                 $Response = $Context.Response
 
@@ -412,16 +442,20 @@
                 if ($Request.HttpMethod -eq 'POST') {
                     Switch-PostRequest -Request $Request
                 }
             } catch {
                 $Message = "ERROR processing request"
                 Write-Host "$($Message): $_" @Red
                 try {
-                    # do NOT include details in the response, only log it to stdout!
-                    Send-Response -Response $Response -Body "$($Message)!" -Html
+                    Send-Response `
+                        -Response $Response `
+                        -StatusCode 400 `
+                        -ExecutionStatus 1 `
+                        -ErrorMesage $_ `
+                        -Body $Message
                 } catch {
                     Write-Host "Unable to send the response: $_" @Red
                 }
             }
         }
 
     } catch {
```

### Comparing `psytricks-2.0.0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json` & `psytricks-2.1.0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.0.0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json` & `psytricks-2.1.0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.0.0/src/psytricks/__ps1__/sampledata/GetSessions.json` & `psytricks-2.1.0/src/psytricks/__ps1__/sampledata/GetSessions.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.0.0/src/psytricks/cli.py` & `psytricks-2.1.0/src/psytricks/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,15 +154,14 @@
     cdc : str
         The address of the Citrix Delivery Controller (CDC) to connect to.
     verbose : int
         The logging verbosity.
     command : str
         The command indicating which wrapper method to call.
     """
-    # FIXME: adapt for "kwargs" being dropped in PSyTricksWrapper
     configure_logging(verbose)
     wrapper = PSyTricksWrapper(deliverycontroller=cdc)
     details = ""
 
     if command == "machines":
         details = wrapper.get_machine_status()
```

### Comparing `psytricks-2.0.0/src/psytricks/decoder.py` & `psytricks-2.1.0/src/psytricks/decoder.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.0.0/src/psytricks/literals.py` & `psytricks-2.1.0/src/psytricks/literals.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.0.0/src/psytricks/mappings.py` & `psytricks-2.1.0/src/psytricks/mappings.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.0.0/src/psytricks/wrapper.py` & `psytricks-2.1.0/src/psytricks/wrapper.py`

 * *Files 19% similar despite different names*

```diff
@@ -318,79 +318,130 @@
     Attributes
     ----------
     base_url : str
         See the constructor for details.
     timeout : int
         The timeout in seconds to use for `requests.get` and `requests.post`
         calls, defaulting to 5.
+    server_version : list
+        The server version as a list of version components, where the first
+        three components are of type `int` (representing `major.minor.patch`),
+        whereas the last component may be a `str` as well.
     """
 
     def __init__(self, base_url: str = "http://localhost:8080/", verify: bool = True):
         """Constructor for the `ResTricksWrapper` class.
 
         Parameters
         ----------
         base_url : str, optional
             The base URL where to find the ResTricks service, by default
             `http://localhost:8080/`.
         verify : bool, optional
             By default the constructor will try to establish a connection to the
             ResTricks service and validate the version. Set to `False` to
-            disable the initial connection and version check.
+            disable the version check and ignore potential problems during the
+            initial connection check.
+
+        Raises
+        ------
+        ValueError
+            Raised in case the server version doesn't match the local version.
+        ConnectionError
+            Raised in case the initial connection check failed.
         """
         self.base_url = base_url
         self.timeout = 5
         self.server_version = [0, 0, 0, 0]
-        if verify:
-            server_version = self.send_get_request("version")
+        try:
+            status = self.send_get_request("version")["Status"]
+            log.trace(f"Server status: [{status}]")
+            server_version = status["PSyTricksVersion"]
+            log.info(f"Server version: [{server_version}]")
+
             log.success("Successfully tested connection 🔌 to ResTricks server 🆗")
-            self.validate_version(server_version)
+            if verify:
+                version_matching = self.validate_version(server_version)
+                if not version_matching:
+                    raise ValueError(f"Unexpected server version: {server_version}")
+        except Exception as ex:  # pylint: disable-msg=broad-except
+            if verify:
+                raise ConnectionError(f"Connecting to [{base_url}] failed!") from ex
 
         log.debug(f"Initialized {self.__class__.__name__}({base_url}) ✨")
 
     def validate_version(self, server_ver):
         """Validate the server version against the local module.
 
         Parse the version strings of the local module and the server response
         and compare them for equality (ignoring the 4th component, which may
         denote a pre- or development-release).
 
-        Currently only log messages are generated, with an error-level message
-        in case the versions don't match. No other action is taken.
-
         Parameters
         ----------
         server_ver : dict
             The dict parsed from the JSON response when sending a `version` GET
             request to the server.
+
+        Returns
+        -------
+        bool
+            True in case the versions are matching, False otherwise.
         """
 
-        def parse_version(ver):
+        def parse_ver(ver):
+            log.trace(f"Parsing version string: [{ver}]")
             _split = ver.split(".")
             version = [int(x) for x in _split[:3]]
             version.append(0)
             if len(_split) > 3:
                 # the 4th component is usually a string, so do not cast it if present:
                 version[3] = _split[3]
             return version
 
         try:
-            self.server_version = parse_version(server_ver["PSyTricksVersion"])
+            self.server_version = parse_ver(server_ver)
             log.info(f"Server version: {self.server_version} 🪪")
         except Exception as ex:  # pylint: disable-msg=broad-except
             log.warning(f"Unable to parse server version [{server_ver}]: {ex}")
+            return False
 
-        client_version = parse_version(__version__)
+        client_version = parse_ver(__version__)
         log.info(f"Client version: {client_version} 🪪")
 
         # compare versions, ignoring the 4th component (dev/pre/alpha/...)
         if client_version[:3] == self.server_version[:3]:
             log.success("Versions are matching! 🏅")
-        else:
-            log.error("Version mismatch! 🧨")
+            return True
+
+        log.error("Version mismatch! 🧨")
+        return False
+
+    @staticmethod
+    def _check_response(response):
+        """Helper checking the HTTP response code and JSON status attributes."""
+        if response.status_code == 200:
+            return
+
+        log.warning(f"Response code {response.status_code} indicates a problem!")
+
+        payload = response.json()
+        try:
+            status = payload["Status"]
+            log.warning(
+                "Status details:\n"
+                f"['Timestamp']: {status['Timestamp']}\n"
+                f"['PSyTricksVersion']: {status['PSyTricksVersion']}\n"
+                f"['ExecutionStatus']: {status['ExecutionStatus']}\n"
+                f"['ErrorMessage']: {status['ErrorMessage']}\n"
+            )
+        except Exception as ex:  # pylint: disable-msg=broad-except
+            log.error(f"Error fetching response payload status: {ex}")
+            log.warning(response.text)
+            raise ValueError(f"Malformed response: {response.text}") from ex
 
     def send_get_request(self, raw_url: str) -> list:
         """Common method to perform a `GET` request and process the response.
 
         Parameters
         ----------
         raw_url : str
@@ -403,21 +454,23 @@
             something went wrong performing the GET request or processing the
             response.
         """
         try:
             response = requests.get(self.base_url + raw_url, timeout=self.timeout)
         except Exception as ex:  # pylint: disable-msg=broad-except
             log.error(f"GET request [{raw_url}] failed: {ex}")
-            return []
+            raise ex
 
         try:
-            data = response.json()
+            data = response.json(object_hook=parse_powershell_json)
         except Exception as ex:  # pylint: disable-msg=broad-except
             log.error(f"GET request [{raw_url}] didn't return any JSON: {ex}")
-            return []
+            raise ex
+
+        ResTricksWrapper._check_response(response)
 
         return data
 
     def send_post_request(
         self, raw_url: str, payload: dict, no_json: bool = False
     ) -> list:
         """Common method to perform a `POST` request and process the response.
@@ -441,83 +494,86 @@
         """
         try:
             response = requests.post(
                 self.base_url + raw_url, json=payload, timeout=self.timeout
             )
         except Exception as ex:  # pylint: disable-msg=broad-except
             log.error(f"POST request [{raw_url}] failed: {ex}")
-            return []
+            raise ex
+
+        ResTricksWrapper._check_response(response)
 
         if no_json:
             log.debug(f"No-payload response status code: {response.status_code}")
             return []
 
-        return response.json()
+        return response.json(object_hook=parse_powershell_json)
 
     def get_machine_status(self) -> list:
         """Send a `GET` request with `GetMachineStatus`.
 
         Returns
         -------
-        list(str)
-            The `JSON` returned by the REST service.
+        dict
+            The `Data` dict parsed from the JSON returned by the REST service.
         """
         log.debug("Requesting current status of machines...")
-        return self.send_get_request("GetMachineStatus")
+        return self.send_get_request("GetMachineStatus")["Data"]
 
     def get_sessions(self) -> list:
         """Send a `GET` request with `GetSessions`.
 
         Returns
         -------
-        list(str)
-            The `JSON` returned by the REST service.
+        dict
+            The `Data` dict parsed from the JSON returned by the REST service.
         """
         log.debug("Requesting current sessions...")
-        return self.send_get_request("GetSessions")
+        return self.send_get_request("GetSessions")["Data"]
 
     def get_access_users(self, group: str) -> list:
         """Send a `GET` request with `GetAccessUsers`.
 
         Parameters
         ----------
         group : str
             The name of the Delivery Group to request users having access.
 
         Returns
         -------
-        list(str)
-            The `JSON` returned by the REST service.
+        dict
+            The `Data` dict parsed from the JSON returned by the REST service.
         """
         log.debug(f"Requesting users having access to group [{group}]...")
-        return self.send_get_request(f"GetAccessUsers/{group}")
+        return self.send_get_request(f"GetAccessUsers/{group}")["Data"]
 
     def disconnect_session(self, machine: str) -> list:
         """Send a `POST` request with `DisconnectSession`.
 
         Parameters
         ----------
         machine : str
             The FQDN of the machine to disconnect the session on.
 
         Returns
         -------
-        list(str)
-            The `JSON` containing details on the affected session, as returned
-            by the REST service. In case the server doesn't return (valid) JSON
-            (for example no session exists on the given machine) an empty list
-            will be returned.
+        dict
+            The `Data` dict parsed from the JSON returned by the REST service,
+            containing details on the affected session. In case the JSON
+            contains an empty `Data` object, an empty dict will be returned.
+            Please note that sending a disconnect request for a session that is
+            already disconnected will not change the session state but still
+            return the session details.
         """
         log.debug(f"Requesting session on [{machine}] to be disconnected...")
         payload = {"DNSName": machine}
-        try:
-            session = self.send_post_request("DisconnectSession", payload)
-        except json.JSONDecodeError:
-            log.debug(f"No JSON received, probably [{machine}] has no session.")
-            return []
+        session = self.send_post_request("DisconnectSession", payload)["Data"]
+        if session is None:
+            log.debug(f"No data received, probably [{machine}] has no session.")
+            return {}
 
         return session
 
     def set_access_users(self, group: str, users: str, disable: bool) -> list:
         """Send a `POST` request with `SetAccessUsers`.
 
         Parameters
@@ -529,49 +585,49 @@
             permissions to the given group should be adapted.
         disable : bool
             A flag requesting the permissions for the given username(s) to be
             removed (if True) instead of being added (if False).
 
         Returns
         -------
-        list(str)
-            The `JSON` returned by the REST service.
+        dict
+            The `Data` dict parsed from the JSON returned by the REST service.
         """
         verb = "Removing" if disable else "Adding"
         log.debug(f"{verb} access to group [{group}] for user(s) [{users}]...")
         payload = {
             "Group": group,
             "UserNames": users,
             "RemoveAccess": disable,
         }
-        return self.send_post_request("SetAccessUsers", payload)
+        return self.send_post_request("SetAccessUsers", payload)["Data"]
 
     def set_maintenance(self, machine: str, disable: bool) -> list:
         """Send a `POST` request with `SetMaintenanceMode`.
 
         Parameters
         ----------
         machine : str
             The FQDN of the machine to modify maintenance mode on.
         disable : bool
             A flag requesting maintenance mode for the given machine(s) to be
             turned off (if True) instead of being turned on (if False).
 
         Returns
         -------
-        list(str)
-            The `JSON` returned by the REST service.
+        dict
+            The `Data` dict parsed from the JSON returned by the REST service.
         """
         verb = "Disabling" if disable else "Enabling"
         log.debug(f"{verb} maintenance mode on [{machine}]...")
         payload = {
             "DNSName": machine,
             "Disable": disable,
         }
-        return self.send_post_request("SetMaintenanceMode", payload)
+        return self.send_post_request("SetMaintenanceMode", payload)["Data"]
 
     def send_message(self, machine: str, message: str, title: str, style: MsgStyle):
         """Send a `POST` request with `SendSessionMessage`.
 
         Parameters
         ----------
         machine : str
@@ -598,14 +654,20 @@
 
         Parameters
         ----------
         machine : str
             The FQDN of the machine to disconnect the session on.
         action : str
             The power action to perform, one of `psytricks.literals.Action`.
+
+        Returns
+        -------
+        dict
+            The `Data` dict parsed from the JSON returned by the REST service
+            containing details on the power action status of the machine.
         """
         log.debug(f"Requesting action [{action}] for machine [{machine}]...")
         payload = {
             "DNSName": machine,
             "Action": action,
         }
-        self.send_post_request("MachinePowerAction", payload)
+        return self.send_post_request("MachinePowerAction", payload)["Data"]
```

### Comparing `psytricks-2.0.0/PKG-INFO` & `psytricks-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psytricks
-Version: 2.0.0
+Version: 2.1.0
 Summary: PowerShell Python Citrix Tricks.
 License: GPL-3.0-or-later
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -16,17 +16,20 @@
 Project-URL: Changelog, https://github.com/imcf/psytricks/blob/main/CHANGELOG.md
 Project-URL: Organisation Homepage, https://imcf.one/
 Project-URL: Twitter, https://twitter.com/imcf_basel
 Description-Content-Type: text/markdown
 
 # PSytricks
 
-`P`ower`S`hell P`y`thon Ci`tri`x Tri`cks`.
+![PyPI](https://img.shields.io/pypi/v/psytricks)
+![PyPI - License](https://img.shields.io/pypi/l/psytricks)
+![pdoc](https://img.shields.io/badge/docs-pdoc-brightgreen.svg)
+![black](https://img.shields.io/badge/code%20style-black-000000.svg)
 
-Pun intended.
+`P`ower`S`hell P`y`thon Ci`tri`x Tri`cks` - pun intended.
 
 ![logo](https://raw.githubusercontent.com/imcf/psytricks/main/resources/images/logo.png)
 
 This package provides an abstraction layer allowing Python code to interact with
 a [Citrix Virtual Apps and Desktops (CVAD)][www_cvad] stack, i.e. to fetch
 status information and trigger actions on machines and sessions. Since CVAD only
 provides a *PowerShell Snap-In* to do so, a core component written in `Windows
```

