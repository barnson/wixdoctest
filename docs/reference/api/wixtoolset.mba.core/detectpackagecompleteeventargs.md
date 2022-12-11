---
custom_edit_url: null
toc_max_heading_level: 2
---
# DetectPackageCompleteEventArgs Class
Additional arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.DetectPackageComplete» .
## Properties
| Property | Description |
| ------ | ----------- |
| [Cached](#cached) | Gets whether any part of the package is cached. |
| [PackageId](#packageid) | Gets the identity of the package detected. |
| [State](#state) | Gets the state of the specified package. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Cached Property {#cached}
Gets whether any part of the package is cached.
### Declaration
```cs
public bool Cached { get; set; } 
```
## PackageId Property {#packageid}
Gets the identity of the package detected.
### Declaration
```cs
public string PackageId { get; set; } 
```
## State Property {#state}
Gets the state of the specified package.
### Declaration
```cs
public PackageState State { get; set; } 
```
