---
custom_edit_url: null
toc_max_heading_level: 2
---
# CacheAcquireBeginEventArgs Class
EventArgs for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.CacheAcquireBegin» .
## Properties
| Property | Description |
| ------ | ----------- |
| [DownloadUrl](#downloadurl) | Gets the optional URL to download container or payload. |
| [PackageOrContainerId](#packageorcontainerid) | Gets the identifier of the container or package. |
| [PayloadContainerId](#payloadcontainerid) | Gets the optional identity of the container that contains the payload being acquired. |
| [PayloadId](#payloadid) | Gets the identifier of the payload (if acquiring a payload). |
| [Source](#source) | Gets the source of the container or payload. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## DownloadUrl Property {#downloadurl}
Gets the optional URL to download container or payload.
### Declaration
```cs
public string DownloadUrl { get; set; } 
```
## PackageOrContainerId Property {#packageorcontainerid}
Gets the identifier of the container or package.
### Declaration
```cs
public string PackageOrContainerId { get; set; } 
```
## PayloadContainerId Property {#payloadcontainerid}
Gets the optional identity of the container that contains the payload being acquired.
### Declaration
```cs
public string PayloadContainerId { get; set; } 
```
## PayloadId Property {#payloadid}
Gets the identifier of the payload (if acquiring a payload).
### Declaration
```cs
public string PayloadId { get; set; } 
```
## Source Property {#source}
Gets the source of the container or payload.
### Declaration
```cs
public string Source { get; set; } 
```
