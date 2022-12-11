---
custom_edit_url: null
toc_max_heading_level: 2
---
# ILibraryResult Interface
Result of a library combine operation.
## Properties
| Property | Description |
| ------ | ----------- |
| [Library](#library) | Output of librarian. |
| [TrackedFiles](#trackedfiles) | Collection of files tracked when binding files into the library. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Library Property {#library}
Output of librarian.
### Declaration
```cs
public WixToolset.Data.Intermediate Library { get; set; } 
```
## TrackedFiles Property {#trackedfiles}
Collection of files tracked when binding files into the library.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.Data.ITrackedFile> TrackedFiles { get; set; } 
```
