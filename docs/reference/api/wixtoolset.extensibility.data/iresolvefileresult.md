---
custom_edit_url: null
toc_max_heading_level: 2
---
# IResolveFileResult Interface
Result of resolving a file.
## Properties
| Property | Description |
| ------ | ----------- |
| [CheckedPaths](#checkedpaths) | Collection of paths checked to find file. |
| [Path](#path) | Path to found file, if found. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## CheckedPaths Property {#checkedpaths}
Collection of paths checked to find file.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<System.String> CheckedPaths { get; set; } 
```
## Path Property {#path}
Path to found file, if found.
### Declaration
```cs
public string Path { get; set; } 
```
