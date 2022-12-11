---
custom_edit_url: null
toc_max_heading_level: 2
---
# SetUpdateCompleteEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.SetUpdateComplete» 
## Properties
| Property | Description |
| ------ | ----------- |
| [NewPackageId](#newpackageid) | Gets the identifier of the update package that was added. |
| [PreviousPackageId](#previouspackageid) | Gets the identifier of the update package that was removed. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## NewPackageId Property {#newpackageid}
Gets the identifier of the update package that was added.
### Declaration
```cs
public string NewPackageId { get; set; } 
```
## PreviousPackageId Property {#previouspackageid}
Gets the identifier of the update package that was removed.
### Declaration
```cs
public string PreviousPackageId { get; set; } 
```
