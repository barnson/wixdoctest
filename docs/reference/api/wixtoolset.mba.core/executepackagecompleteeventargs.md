---
custom_edit_url: null
toc_max_heading_level: 2
---
# ExecutePackageCompleteEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.ExecutePackageComplete» Additional arguments used when the engine has completed installing a specific package.
## Properties
| Property | Description |
| ------ | ----------- |
| [PackageId](#packageid) | Gets the identity of the package that was acted on. |
| [Restart](#restart) | Gets the package restart state after being applied. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## PackageId Property {#packageid}
Gets the identity of the package that was acted on.
### Declaration
```cs
public string PackageId { get; set; } 
```
## Restart Property {#restart}
Gets the package restart state after being applied.
### Declaration
```cs
public ApplyRestart Restart { get; set; } 
```
