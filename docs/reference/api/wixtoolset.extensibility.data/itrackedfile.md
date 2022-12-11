---
custom_edit_url: null
toc_max_heading_level: 2
---
# ITrackedFile Interface
Interface used to track all files processed.
## Properties
| Property | Description |
| ------ | ----------- |
| [Path](#path) | Path to tracked file. |
| [SourceLineNumbers](#sourcelinenumbers) | Optional source line numbers where the tracked file was created. |
| [Type](#type) | Type of tracked file. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Path Property {#path}
Path to tracked file.
### Declaration
```cs
public string Path { get; set; } 
```
## SourceLineNumbers Property {#sourcelinenumbers}
Optional source line numbers where the tracked file was created.
### Declaration
```cs
public WixToolset.Data.SourceLineNumber SourceLineNumbers { get; set; } 
```
## Type Property {#type}
Type of tracked file.
### Declaration
```cs
public TrackedFileType Type { get; set; } 
```
