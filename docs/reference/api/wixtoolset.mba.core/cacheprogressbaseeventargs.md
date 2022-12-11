---
custom_edit_url: null
toc_max_heading_level: 2
---
# CacheProgressBaseEventArgs Class
Base class for cache progress events.
## Properties
| Property | Description |
| ------ | ----------- |
| [OverallPercentage](#overallpercentage) | Gets the overall percentage of progress of caching. |
| [PackageOrContainerId](#packageorcontainerid) | Gets the identifier of the container or package. |
| [PayloadId](#payloadid) | Gets the identifier of the payload. |
| [Progress](#progress) | Gets the number of bytes cached thus far. |
| [Total](#total) | Gets the total bytes to cache. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## OverallPercentage Property {#overallpercentage}
Gets the overall percentage of progress of caching.
### Declaration
```cs
public int OverallPercentage { get; set; } 
```
## PackageOrContainerId Property {#packageorcontainerid}
Gets the identifier of the container or package.
### Declaration
```cs
public string PackageOrContainerId { get; set; } 
```
## PayloadId Property {#payloadid}
Gets the identifier of the payload.
### Declaration
```cs
public string PayloadId { get; set; } 
```
## Progress Property {#progress}
Gets the number of bytes cached thus far.
### Declaration
```cs
public System.Int64 Progress { get; set; } 
```
## Total Property {#total}
Gets the total bytes to cache.
### Declaration
```cs
public System.Int64 Total { get; set; } 
```
