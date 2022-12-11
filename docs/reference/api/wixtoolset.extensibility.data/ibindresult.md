---
custom_edit_url: null
toc_max_heading_level: 2
---
# IBindResult Interface
Result of bind operation.
## Properties
| Property | Description |
| ------ | ----------- |
| [FileTransfers](#filetransfers) | Collection of file transfers to complete. |
| [TrackedFiles](#trackedfiles) | Collection of files tracked during binding. |
| [Wixout](#wixout) | Output of binding. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## FileTransfers Property {#filetransfers}
Collection of file transfers to complete.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.Data.IFileTransfer> FileTransfers { get; set; } 
```
## TrackedFiles Property {#trackedfiles}
Collection of files tracked during binding.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.Data.ITrackedFile> TrackedFiles { get; set; } 
```
## Wixout Property {#wixout}
Output of binding.
### Declaration
```cs
public WixToolset.Data.WixOutput Wixout { get; set; } 
```
