---
custom_edit_url: null
toc_max_heading_level: 2
---
# CachePackageBeginEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.CachePackageBegin» 
## Properties
| Property | Description |
| ------ | ----------- |
| [CachePayloads](#cachepayloads) | Gets number of payloads to be cached. |
| [PackageCacheSize](#packagecachesize) | Gets the size on disk required by the specific package. |
| [PackageId](#packageid) | Gets the identity of the package that is being cached. |
| [Vital](#vital) | If caching a package is not vital, then acquisition will be skipped unless the BA opts in through «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.CachePackageNonVitalValidationFailure» . |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## CachePayloads Property {#cachepayloads}
Gets number of payloads to be cached.
### Declaration
```cs
public System.Int64 CachePayloads { get; set; } 
```
## PackageCacheSize Property {#packagecachesize}
Gets the size on disk required by the specific package.
### Declaration
```cs
public System.Int64 PackageCacheSize { get; set; } 
```
## PackageId Property {#packageid}
Gets the identity of the package that is being cached.
### Declaration
```cs
public string PackageId { get; set; } 
```
## Vital Property {#vital}
If caching a package is not vital, then acquisition will be skipped unless the BA opts in through «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.CachePackageNonVitalValidationFailure» .
### Declaration
```cs
public bool Vital { get; set; } 
```
