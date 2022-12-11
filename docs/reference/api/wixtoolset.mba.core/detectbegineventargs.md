---
custom_edit_url: null
toc_max_heading_level: 2
---
# DetectBeginEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.DetectBegin» 
## Properties
| Property | Description |
| ------ | ----------- |
| [Cached](#cached) | Gets whether the bundle is cached. |
| [PackageCount](#packagecount) | Gets the number of packages to detect. |
| [RegistrationType](#registrationtype) | Gets the bundle's registration state. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Cached Property {#cached}
Gets whether the bundle is cached.
### Declaration
```cs
public bool Cached { get; set; } 
```
## PackageCount Property {#packagecount}
Gets the number of packages to detect.
### Declaration
```cs
public int PackageCount { get; set; } 
```
## RegistrationType Property {#registrationtype}
Gets the bundle's registration state.
### Declaration
```cs
public RegistrationType RegistrationType { get; set; } 
```
