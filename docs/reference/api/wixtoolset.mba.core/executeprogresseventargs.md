---
custom_edit_url: null
toc_max_heading_level: 2
---
# ExecuteProgressEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.ExecuteProgress» 
## Properties
| Property | Description |
| ------ | ----------- |
| [OverallPercentage](#overallpercentage) | Gets the percentage from 0 to 100 of the execution progress for all payloads. |
| [PackageId](#packageid) | Gets the identity of the package that was executed. |
| [ProgressPercentage](#progresspercentage) | Gets the percentage from 0 to 100 of the execution progress for a single payload. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## OverallPercentage Property {#overallpercentage}
Gets the percentage from 0 to 100 of the execution progress for all payloads.
### Declaration
```cs
public int OverallPercentage { get; set; } 
```
## PackageId Property {#packageid}
Gets the identity of the package that was executed.
### Declaration
```cs
public string PackageId { get; set; } 
```
## ProgressPercentage Property {#progresspercentage}
Gets the percentage from 0 to 100 of the execution progress for a single payload.
### Declaration
```cs
public int ProgressPercentage { get; set; } 
```
