---
custom_edit_url: null
toc_max_heading_level: 2
---
# IBootstrapperApplication Interface
Allows customization of the bootstrapper application.
## Methods
| Method | Description |
| ------ | ----------- |
| [BAProc()](#baproc_nop) | Low level method that is called directly from the engine. |
| [OnBeginMsiTransactionComplete(wzTransactionId, hrStatus)](#onbeginmsitransactioncomplete_wztransactionid_hrstatus) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.BeginMsiTransactionComplete» . |
| [OnCacheComplete(hrStatus)](#oncachecomplete_hrstatus) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.CacheComplete» . |
| [OnCacheContainerOrPayloadVerifyComplete()](#oncachecontainerorpayloadverifycomplete_nop) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.CacheContainerOrPayloadVerifyComplete» . |
| [OnCachePayloadExtractComplete()](#oncachepayloadextractcomplete_nop) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.CachePayloadExtractComplete» . |
| [OnCommitMsiTransactionComplete(wzTransactionId, hrStatus)](#oncommitmsitransactioncomplete_wztransactionid_hrstatus) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.CommitMsiTransactionComplete» . |
| [OnDetectComplete(hrStatus, fEligibleForCleanup)](#ondetectcomplete_hrstatus_feligibleforcleanup) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.DetectComplete» . |
| [OnDetectPackageComplete()](#ondetectpackagecomplete_nop) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.DetectPackageComplete» . |
| [OnElevateComplete(hrStatus)](#onelevatecomplete_hrstatus) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.ElevateComplete» . |
| [OnExecuteComplete(hrStatus)](#onexecutecomplete_hrstatus) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.ExecuteComplete» . |
| [OnLaunchApprovedExeComplete(hrStatus, processId)](#onlaunchapprovedexecomplete_hrstatus_processid) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.LaunchApprovedExeComplete» . |
| [OnPauseAutomaticUpdatesBegin()](#onpauseautomaticupdatesbegin_nop) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PauseAutomaticUpdatesBegin» . |
| [OnPauseAutomaticUpdatesComplete(hrStatus)](#onpauseautomaticupdatescomplete_hrstatus) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PauseAutomaticUpdatesComplete» . |
| [OnPlanCompatibleMsiPackageComplete()](#onplancompatiblemsipackagecomplete_nop) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlanCompatibleMsiPackageComplete» . |
| [OnPlanComplete(hrStatus)](#onplancomplete_hrstatus) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlanComplete» . |
| [OnPlannedCompatiblePackage()](#onplannedcompatiblepackage_nop) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlannedCompatiblePackage» . |
| [OnPlannedPackage()](#onplannedpackage_nop) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlannedPackage» . |
| [OnPlanPackageComplete(wzPackageId, hrStatus, requested)](#onplanpackagecomplete_wzpackageid_hrstatus_requested) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlanPackageComplete» . |
| [OnRegisterComplete(hrStatus)](#onregistercomplete_hrstatus) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.RegisterComplete» . |
| [OnRollbackMsiTransactionBegin(wzTransactionId)](#onrollbackmsitransactionbegin_wztransactionid) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.RollbackMsiTransactionBegin» . |
| [OnRollbackMsiTransactionComplete(wzTransactionId, hrStatus)](#onrollbackmsitransactioncomplete_wztransactionid_hrstatus) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.RollbackMsiTransactionComplete» . |
| [OnSetUpdateBegin()](#onsetupdatebegin_nop) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.SetUpdateBegin» . |
| [OnSetUpdateComplete()](#onsetupdatecomplete_nop) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.SetUpdateComplete» . |
| [OnStartup()](#onstartup_nop) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.Startup» . |
| [OnSystemRestorePointBegin()](#onsystemrestorepointbegin_nop) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.SystemRestorePointBegin» . |
| [OnSystemRestorePointComplete(hrStatus)](#onsystemrestorepointcomplete_hrstatus) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.SystemRestorePointComplete» . |
| [OnUnregisterComplete(hrStatus)](#onunregistercomplete_hrstatus) | See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.UnregisterComplete» . |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## BAProc() Method {#baproc_nop}
Low level method that is called directly from the engine.
### Declaration
```cs
public int BAProc
```
## OnBeginMsiTransactionComplete(wzTransactionId, hrStatus) Method {#onbeginmsitransactioncomplete_wztransactionid_hrstatus}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.BeginMsiTransactionComplete» .
### Declaration
```cs
public int OnBeginMsiTransactionComplete(
  string wzTransactionId,
  int hrStatus
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| wzTransactionId | string |  |
| hrStatus | int |  |
## OnCacheComplete(hrStatus) Method {#oncachecomplete_hrstatus}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.CacheComplete» .
### Declaration
```cs
public int OnCacheComplete(
  int hrStatus
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hrStatus | int |  |
## OnCacheContainerOrPayloadVerifyComplete() Method {#oncachecontainerorpayloadverifycomplete_nop}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.CacheContainerOrPayloadVerifyComplete» .
### Declaration
```cs
public int OnCacheContainerOrPayloadVerifyComplete
```
## OnCachePayloadExtractComplete() Method {#oncachepayloadextractcomplete_nop}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.CachePayloadExtractComplete» .
### Declaration
```cs
public int OnCachePayloadExtractComplete
```
## OnCommitMsiTransactionComplete(wzTransactionId, hrStatus) Method {#oncommitmsitransactioncomplete_wztransactionid_hrstatus}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.CommitMsiTransactionComplete» .
### Declaration
```cs
public int OnCommitMsiTransactionComplete(
  string wzTransactionId,
  int hrStatus
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| wzTransactionId | string |  |
| hrStatus | int |  |
## OnDetectComplete(hrStatus, fEligibleForCleanup) Method {#ondetectcomplete_hrstatus_feligibleforcleanup}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.DetectComplete» .
### Declaration
```cs
public int OnDetectComplete(
  int hrStatus,
  bool fEligibleForCleanup
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hrStatus | int |  |
| fEligibleForCleanup | bool |  |
## OnDetectPackageComplete() Method {#ondetectpackagecomplete_nop}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.DetectPackageComplete» .
### Declaration
```cs
public int OnDetectPackageComplete
```
## OnElevateComplete(hrStatus) Method {#onelevatecomplete_hrstatus}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.ElevateComplete» .
### Declaration
```cs
public int OnElevateComplete(
  int hrStatus
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hrStatus | int |  |
## OnExecuteComplete(hrStatus) Method {#onexecutecomplete_hrstatus}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.ExecuteComplete» .
### Declaration
```cs
public int OnExecuteComplete(
  int hrStatus
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hrStatus | int |  |
## OnLaunchApprovedExeComplete(hrStatus, processId) Method {#onlaunchapprovedexecomplete_hrstatus_processid}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.LaunchApprovedExeComplete» .
### Declaration
```cs
public int OnLaunchApprovedExeComplete(
  int hrStatus,
  int processId
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hrStatus | int |  |
| processId | int |  |
## OnPauseAutomaticUpdatesBegin() Method {#onpauseautomaticupdatesbegin_nop}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PauseAutomaticUpdatesBegin» .
### Declaration
```cs
public int OnPauseAutomaticUpdatesBegin
```
## OnPauseAutomaticUpdatesComplete(hrStatus) Method {#onpauseautomaticupdatescomplete_hrstatus}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PauseAutomaticUpdatesComplete» .
### Declaration
```cs
public int OnPauseAutomaticUpdatesComplete(
  int hrStatus
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hrStatus | int |  |
## OnPlanCompatibleMsiPackageComplete() Method {#onplancompatiblemsipackagecomplete_nop}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlanCompatibleMsiPackageComplete» .
### Declaration
```cs
public int OnPlanCompatibleMsiPackageComplete
```
## OnPlanComplete(hrStatus) Method {#onplancomplete_hrstatus}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlanComplete» .
### Declaration
```cs
public int OnPlanComplete(
  int hrStatus
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hrStatus | int |  |
## OnPlannedCompatiblePackage() Method {#onplannedcompatiblepackage_nop}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlannedCompatiblePackage» .
### Declaration
```cs
public int OnPlannedCompatiblePackage
```
## OnPlannedPackage() Method {#onplannedpackage_nop}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlannedPackage» .
### Declaration
```cs
public int OnPlannedPackage
```
## OnPlanPackageComplete(wzPackageId, hrStatus, requested) Method {#onplanpackagecomplete_wzpackageid_hrstatus_requested}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlanPackageComplete» .
### Declaration
```cs
public int OnPlanPackageComplete(
  string wzPackageId,
  int hrStatus,
  RequestState requested
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| wzPackageId | string |  |
| hrStatus | int |  |
| requested | RequestState |  |
## OnRegisterComplete(hrStatus) Method {#onregistercomplete_hrstatus}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.RegisterComplete» .
### Declaration
```cs
public int OnRegisterComplete(
  int hrStatus
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hrStatus | int |  |
## OnRollbackMsiTransactionBegin(wzTransactionId) Method {#onrollbackmsitransactionbegin_wztransactionid}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.RollbackMsiTransactionBegin» .
### Declaration
```cs
public int OnRollbackMsiTransactionBegin(
  string wzTransactionId
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| wzTransactionId | string |  |
## OnRollbackMsiTransactionComplete(wzTransactionId, hrStatus) Method {#onrollbackmsitransactioncomplete_wztransactionid_hrstatus}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.RollbackMsiTransactionComplete» .
### Declaration
```cs
public int OnRollbackMsiTransactionComplete(
  string wzTransactionId,
  int hrStatus
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| wzTransactionId | string |  |
| hrStatus | int |  |
## OnSetUpdateBegin() Method {#onsetupdatebegin_nop}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.SetUpdateBegin» .
### Declaration
```cs
public int OnSetUpdateBegin
```
## OnSetUpdateComplete() Method {#onsetupdatecomplete_nop}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.SetUpdateComplete» .
### Declaration
```cs
public int OnSetUpdateComplete
```
## OnStartup() Method {#onstartup_nop}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.Startup» .
### Declaration
```cs
public int OnStartup
```
## OnSystemRestorePointBegin() Method {#onsystemrestorepointbegin_nop}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.SystemRestorePointBegin» .
### Declaration
```cs
public int OnSystemRestorePointBegin
```
## OnSystemRestorePointComplete(hrStatus) Method {#onsystemrestorepointcomplete_hrstatus}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.SystemRestorePointComplete» .
### Declaration
```cs
public int OnSystemRestorePointComplete(
  int hrStatus
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hrStatus | int |  |
## OnUnregisterComplete(hrStatus) Method {#onunregistercomplete_hrstatus}
See «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.UnregisterComplete» .
### Declaration
```cs
public int OnUnregisterComplete(
  int hrStatus
)
```
### Parameters
| Parameter | Type | Description |
| --------- | ---- | ----------- |
| hrStatus | int |  |
