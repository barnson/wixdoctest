---
custom_edit_url: null
toc_max_heading_level: 2
---
# ProgressEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.Progress» 
## Properties
| Property | Description |
| ------ | ----------- |
| [OverallPercentage](#overallpercentage) | Gets the percentage from 0 to 100 completed for the bundle. |
| [ProgressPercentage](#progresspercentage) | Gets the percentage from 0 to 100 completed for a package. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## OverallPercentage Property {#overallpercentage}
Gets the percentage from 0 to 100 completed for the bundle.
### Declaration
```cs
public int OverallPercentage { get; set; } 
```
## ProgressPercentage Property {#progresspercentage}
Gets the percentage from 0 to 100 completed for a package.
### Declaration
```cs
public int ProgressPercentage { get; set; } 
```
