---
custom_edit_url: null
toc_max_heading_level: 2
---
# ExecuteFilesInUseEventArgs Class
Event arguments for «see E:WixToolset.Mba.Core.IDefaultBootstrapperApplication.ExecuteFilesInUse» 
## Properties
| Property | Description |
| ------ | ----------- |
| [Files](#files) | Gets the list of files in use. |
| [PackageId](#packageid) | Gets the identity of the package that yielded the files in use message. |
| [Source](#source) | Gets the source of the message. |
`WixToolset.Mba.Core.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Files Property {#files}
Gets the list of files in use.
### Declaration
```cs
public IList<System.String> Files { get; set; } 
```
## PackageId Property {#packageid}
Gets the identity of the package that yielded the files in use message.
### Declaration
```cs
public string PackageId { get; set; } 
```
## Source Property {#source}
Gets the source of the message.
### Declaration
```cs
public FilesInUseType Source { get; set; } 
```
