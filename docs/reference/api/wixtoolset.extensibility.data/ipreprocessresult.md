---
custom_edit_url: null
toc_max_heading_level: 2
---
# IPreprocessResult Interface
Result of preprocessing.
## Properties
| Property | Description |
| ------ | ----------- |
| [Document](#document) | Document result of preprocessor. |
| [IncludedFiles](#includedfiles) | Collection of files included during preprocessing. |
`WixToolset.Extensibility.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Document Property {#document}
Document result of preprocessor.
### Declaration
```cs
public System.Xml.Linq.XDocument Document { get; set; } 
```
## IncludedFiles Property {#includedfiles}
Collection of files included during preprocessing.
### Declaration
```cs
public System.Collections.Generic.IReadOnlyCollection<WixToolset.Extensibility.Data.IIncludedFile> IncludedFiles { get; set; } 
```
