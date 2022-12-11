---
custom_edit_url: null
toc_max_heading_level: 2
---
# PlanPackageCompleteEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlanPackageComplete» 
## Properties
| Property | Description |
| ------ | ----------- |
| [PackageId](#packageid) | Gets the identity of the package planned for. |
| [Requested](#requested) | Gets the requested state for the package. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## PackageId Property {#packageid}
Gets the identity of the package planned for.
### Declaration
```cs
public string PackageId { get; set; } 
```
## Requested Property {#requested}
Gets the requested state for the package.
### Declaration
```cs
public RequestState Requested { get; set; } 
```
