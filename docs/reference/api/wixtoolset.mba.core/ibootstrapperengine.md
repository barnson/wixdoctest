---
custom_edit_url: null
toc_max_heading_level: 2
---
# IBootstrapperEngine Interface
Allows calls into the bootstrapper engine.
## Methods
| Method | Description |
| ------ | ----------- |
| [Apply(hwndParent)](#apply_hwndparent) | See «see M:WixToolset.Mba.Core.IEngine.Apply(System.IntPtr)» . |
| [CloseSplashScreen()](#closesplashscreen_nop) | See «see M:WixToolset.Mba.Core.IEngine.CloseSplashScreen» . |
| [Detect(hwndParent)](#detect_hwndparent) | See «see M:WixToolset.Mba.Core.IEngine.Detect(System.IntPtr)» . |
| [Elevate(hwndParent)](#elevate_hwndparent) | See «see M:WixToolset.Mba.Core.IEngine.Elevate(System.IntPtr)» . |
| [LaunchApprovedExe(hwndParent, wzApprovedExeForElevationId, wzArguments, dwWaitForInputIdleTimeout)](#launchapprovedexe_hwndparent_wzapprovedexeforelevationid_wzarguments_dwwaitforinputidletimeout) | See «see M:WixToolset.Mba.Core.IEngine.LaunchApprovedExe(System.IntPtr,System.String,System.String,System.Int32)» . |
| [Log(level, wzMessage)](#log_level_wzmessage) | See «see M:WixToolset.Mba.Core.IEngine.Log(WixToolset.Mba.Core.LogLevel,System.String)» . |
| [Plan(action)](#plan_action) | See «see M:WixToolset.Mba.Core.IEngine.Plan(WixToolset.Mba.Core.LaunchAction)» . |
| [Quit(dwExitCode)](#quit_dwexitcode) | See «see M:WixToolset.Mba.Core.IEngine.Quit(System.Int32)» . |
| [SetDownloadSource(wzPackageOrContainerId, wzPayloadId, wzUrl, wzUser, wzPassword)](#setdownloadsource_wzpackageorcontainerid_wzpayloadid_wzurl_wzuser_wzpassword) | See «see M:WixToolset.Mba.Core.IEngine.SetDownloadSource(System.String,System.String,System.String,System.String,System.String)» . |
| [SetLocalSource(wzPackageOrContainerId, wzPayloadId, wzPath)](#setlocalsource_wzpackageorcontainerid_wzpayloadid_wzpath) | See «see M:WixToolset.Mba.Core.IEngine.SetLocalSource(System.String,System.String,System.String)» . |
| [SetUpdate(wzLocalSource, wzDownloadSource, qwValue, hashType, wzHash)](#setupdate_wzlocalsource_wzdownloadsource_qwvalue_hashtype_wzhash) | See «see M:WixToolset.Mba.Core.IEngine.SetUpdate(System.String,System.String,System.Int64,WixToolset.Mba.Core.UpdateHashType,System.String)» . |
| [SetUpdateSource(url)](#setupdatesource_url) | Sets the URL to the update feed. |
| [SetVariableNumeric(wzVariable, llValue)](#setvariablenumeric_wzvariable_llvalue) | See «see M:WixToolset.Mba.Core.IEngine.SetVariableNumeric(System.String,System.Int64)» . |
| [SetVariableString(wzVariable, wzValue, fFormatted)](#setvariablestring_wzvariable_wzvalue_fformatted) | See «see M:WixToolset.Mba.Core.IEngine.SetVariableString(System.String,System.String,System.Boolean)» . |
| [SetVariableVersion(wzVariable, wzValue)](#setvariableversion_wzvariable_wzvalue) | See «see M:WixToolset.Mba.Core.IEngine.SetVariableVersion(System.String,System.String)» . |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Apply(hwndParent) Method {#apply_hwndparent}
See «see M:WixToolset.Mba.Core.IEngine.Apply(System.IntPtr)» .
### Declaration
```cs
public void Apply(
  System.IntPtr hwndParent
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hwndParent | System.IntPtr |  |
## CloseSplashScreen() Method {#closesplashscreen_nop}
See «see M:WixToolset.Mba.Core.IEngine.CloseSplashScreen» .
### Declaration
```cs
public void CloseSplashScreen
```
## Detect(hwndParent) Method {#detect_hwndparent}
See «see M:WixToolset.Mba.Core.IEngine.Detect(System.IntPtr)» .
### Declaration
```cs
public void Detect(
  System.IntPtr hwndParent
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hwndParent | System.IntPtr |  |
## Elevate(hwndParent) Method {#elevate_hwndparent}
See «see M:WixToolset.Mba.Core.IEngine.Elevate(System.IntPtr)» .
### Declaration
```cs
public int Elevate(
  System.IntPtr hwndParent
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hwndParent | System.IntPtr |  |
## LaunchApprovedExe(hwndParent, wzApprovedExeForElevationId, wzArguments, dwWaitForInputIdleTimeout) Method {#launchapprovedexe_hwndparent_wzapprovedexeforelevationid_wzarguments_dwwaitforinputidletimeout}
See «see M:WixToolset.Mba.Core.IEngine.LaunchApprovedExe(System.IntPtr,System.String,System.String,System.Int32)» .
### Declaration
```cs
public void LaunchApprovedExe(
  System.IntPtr hwndParent,
  string wzApprovedExeForElevationId,
  string wzArguments,
  int dwWaitForInputIdleTimeout
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hwndParent | System.IntPtr |  |
| wzApprovedExeForElevationId | string |  |
| wzArguments | string |  |
| dwWaitForInputIdleTimeout | int |  |
## Log(level, wzMessage) Method {#log_level_wzmessage}
See «see M:WixToolset.Mba.Core.IEngine.Log(WixToolset.Mba.Core.LogLevel,System.String)» .
### Declaration
```cs
public void Log(
  LogLevel level,
  string wzMessage
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| level | LogLevel |  |
| wzMessage | string |  |
## Plan(action) Method {#plan_action}
See «see M:WixToolset.Mba.Core.IEngine.Plan(WixToolset.Mba.Core.LaunchAction)» .
### Declaration
```cs
public void Plan(
  LaunchAction action
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| action | LaunchAction |  |
## Quit(dwExitCode) Method {#quit_dwexitcode}
See «see M:WixToolset.Mba.Core.IEngine.Quit(System.Int32)» .
### Declaration
```cs
public void Quit(
  int dwExitCode
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| dwExitCode | int |  |
## SetDownloadSource(wzPackageOrContainerId, wzPayloadId, wzUrl, wzUser, wzPassword) Method {#setdownloadsource_wzpackageorcontainerid_wzpayloadid_wzurl_wzuser_wzpassword}
See «see M:WixToolset.Mba.Core.IEngine.SetDownloadSource(System.String,System.String,System.String,System.String,System.String)» .
### Declaration
```cs
public void SetDownloadSource(
  string wzPackageOrContainerId,
  string wzPayloadId,
  string wzUrl,
  string wzUser,
  string wzPassword
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| wzPackageOrContainerId | string |  |
| wzPayloadId | string |  |
| wzUrl | string |  |
| wzUser | string |  |
| wzPassword | string |  |
## SetLocalSource(wzPackageOrContainerId, wzPayloadId, wzPath) Method {#setlocalsource_wzpackageorcontainerid_wzpayloadid_wzpath}
See «see M:WixToolset.Mba.Core.IEngine.SetLocalSource(System.String,System.String,System.String)» .
### Declaration
```cs
public void SetLocalSource(
  string wzPackageOrContainerId,
  string wzPayloadId,
  string wzPath
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| wzPackageOrContainerId | string |  |
| wzPayloadId | string |  |
| wzPath | string |  |
## SetUpdate(wzLocalSource, wzDownloadSource, qwValue, hashType, wzHash) Method {#setupdate_wzlocalsource_wzdownloadsource_qwvalue_hashtype_wzhash}
See «see M:WixToolset.Mba.Core.IEngine.SetUpdate(System.String,System.String,System.Int64,WixToolset.Mba.Core.UpdateHashType,System.String)» .
### Declaration
```cs
public void SetUpdate(
  string wzLocalSource,
  string wzDownloadSource,
  System.Int64 qwValue,
  UpdateHashType hashType,
  string wzHash
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| wzLocalSource | string |  |
| wzDownloadSource | string |  |
| qwValue | System.Int64 |  |
| hashType | UpdateHashType |  |
| wzHash | string |  |
## SetUpdateSource(url) Method {#setupdatesource_url}
Sets the URL to the update feed.
### Declaration
```cs
public void SetUpdateSource(
  string url
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| url | string | URL of the update feed. |
## SetVariableNumeric(wzVariable, llValue) Method {#setvariablenumeric_wzvariable_llvalue}
See «see M:WixToolset.Mba.Core.IEngine.SetVariableNumeric(System.String,System.Int64)» .
### Declaration
```cs
public void SetVariableNumeric(
  string wzVariable,
  System.Int64 llValue
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| wzVariable | string |  |
| llValue | System.Int64 |  |
## SetVariableString(wzVariable, wzValue, fFormatted) Method {#setvariablestring_wzvariable_wzvalue_fformatted}
See «see M:WixToolset.Mba.Core.IEngine.SetVariableString(System.String,System.String,System.Boolean)» .
### Declaration
```cs
public void SetVariableString(
  string wzVariable,
  System.IntPtr wzValue,
  bool fFormatted
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| wzVariable | string |  |
| wzValue | System.IntPtr |  |
| fFormatted | bool |  |
## SetVariableVersion(wzVariable, wzValue) Method {#setvariableversion_wzvariable_wzvalue}
See «see M:WixToolset.Mba.Core.IEngine.SetVariableVersion(System.String,System.String)» .
### Declaration
```cs
public void SetVariableVersion(
  string wzVariable,
  System.IntPtr wzValue
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| wzVariable | string |  |
| wzValue | System.IntPtr |  |
