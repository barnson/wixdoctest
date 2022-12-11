---
custom_edit_url: null
toc_max_heading_level: 2
---
# PlannedPackageEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.PlannedPackage» 
## Properties
| Property | Description |
| ------ | ----------- |
| [Cache](#cache) | Gets whether the package will be cached. |
| [Execute](#execute) | Gets the planned execution action. |
| [PackageId](#packageid) | Gets the identity of the package planned for. |
| [Rollback](#rollback) | Gets the planned rollback action. |
| [Uncache](#uncache) | Gets whether the package will be removed from the package cache. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Cache Property {#cache}
Gets whether the package will be cached.
### Declaration
```cs
public bool Cache { get; set; } 
```
## Execute Property {#execute}
Gets the planned execution action.
### Declaration
```cs
public ActionState Execute { get; set; } 
```
## PackageId Property {#packageid}
Gets the identity of the package planned for.
### Declaration
```cs
public string PackageId { get; set; } 
```
## Rollback Property {#rollback}
Gets the planned rollback action.
### Declaration
```cs
public ActionState Rollback { get; set; } 
```
## Uncache Property {#uncache}
Gets whether the package will be removed from the package cache.
### Declaration
```cs
public bool Uncache { get; set; } 
```
