---
custom_edit_url: null
toc_max_heading_level: 2
---
# PlanCompatibleMsiPackageCompleteEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlanCompatibleMsiPackageComplete» 
## Properties
| Property | Description |
| ------ | ----------- |
| [CompatiblePackageId](#compatiblepackageid) | Gets the identity of the compatible package detected. |
| [PackageId](#packageid) | Gets the identity of the package planned for. |
| [RequestedRemove](#requestedremove) | Gets the requested state of the package. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## CompatiblePackageId Property {#compatiblepackageid}
Gets the identity of the compatible package detected.
### Declaration
```cs
public string CompatiblePackageId { get; set; } 
```
## PackageId Property {#packageid}
Gets the identity of the package planned for.
### Declaration
```cs
public string PackageId { get; set; } 
```
## RequestedRemove Property {#requestedremove}
Gets the requested state of the package.
### Declaration
```cs
public bool RequestedRemove { get; set; } 
```
