---
custom_edit_url: null
toc_max_heading_level: 2
---
# ExecuteProcessCancelEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.ExecuteProcessCancel» 
## Properties
| Property | Description |
| ------ | ----------- |
| [Action](#action) | Gets or sets the action to be performed. This is passed back to the engine. |
| [PackageId](#packageid) | Gets the identity of the package. |
| [ProcessId](#processid) | Gets the process id. |
| [Recommendation](#recommendation) | Gets the recommended action from the engine. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Action Property {#action}
Gets or sets the action to be performed. This is passed back to the engine.
### Declaration
```cs
public BOOTSTRAPPER_EXECUTEPROCESSCANCEL_ACTION Action { get; set; } 
```
## PackageId Property {#packageid}
Gets the identity of the package.
### Declaration
```cs
public string PackageId { get; set; } 
```
## ProcessId Property {#processid}
Gets the process id.
### Declaration
```cs
public int ProcessId { get; set; } 
```
## Recommendation Property {#recommendation}
Gets the recommended action from the engine.
### Declaration
```cs
public BOOTSTRAPPER_EXECUTEPROCESSCANCEL_ACTION Recommendation { get; set; } 
```
