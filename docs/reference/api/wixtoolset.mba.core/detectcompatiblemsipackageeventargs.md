---
custom_edit_url: null
toc_max_heading_level: 2
---
# DetectCompatibleMsiPackageEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.DetectCompatibleMsiPackage» 
## Properties
| Property | Description |
| ------ | ----------- |
| [CompatiblePackageId](#compatiblepackageid) | Gets the identity of the compatible package that was detected. |
| [CompatiblePackageVersion](#compatiblepackageversion) | Gets the version of the compatible package that was detected. |
| [PackageId](#packageid) | Gets the identity of the package that was not detected. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## CompatiblePackageId Property {#compatiblepackageid}
Gets the identity of the compatible package that was detected.
### Declaration
```cs
public string CompatiblePackageId { get; set; } 
```
## CompatiblePackageVersion Property {#compatiblepackageversion}
Gets the version of the compatible package that was detected.
### Declaration
```cs
public string CompatiblePackageVersion { get; set; } 
```
## PackageId Property {#packageid}
Gets the identity of the package that was not detected.
### Declaration
```cs
public string PackageId { get; set; } 
```
