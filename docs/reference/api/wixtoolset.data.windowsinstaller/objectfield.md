---
custom_edit_url: null
toc_max_heading_level: 2
---
# ObjectField Class
Field containing data for an object column in a row.
## Properties
| Property | Description |
| ------ | ----------- |
| [BaseUri](#baseuri) | Gets the base URI of the object field. |
| [EmbeddedFileIndex](#embeddedfileindex) | Gets or sets the index of the embedded file in a library. |
| [PreviousBaseUri](#previousbaseuri) | Gets or sets the path to the embedded cabinet of the previous file. |
| [PreviousEmbeddedFileIndex](#previousembeddedfileindex) | Gets or sets the previous index of the embedded file in the library. |
| [UnresolvedData](#unresolveddata) | Gets or sets the unresolved data for this field. |
| [UnresolvedPreviousData](#unresolvedpreviousdata) | Gets or sets the unresolved previous data. |
`WixToolset.Data.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## BaseUri Property {#baseuri}
Gets the base URI of the object field.
### Declaration
```cs
public System.Uri BaseUri { get; set; } 
```
## EmbeddedFileIndex Property {#embeddedfileindex}
Gets or sets the index of the embedded file in a library.
### Declaration
```cs
public System.Nullable<System.Int32> EmbeddedFileIndex { get; set; } 
```
## PreviousBaseUri Property {#previousbaseuri}
Gets or sets the path to the embedded cabinet of the previous file.
### Declaration
```cs
public System.Uri PreviousBaseUri { get; set; } 
```
## PreviousEmbeddedFileIndex Property {#previousembeddedfileindex}
Gets or sets the previous index of the embedded file in the library.
### Declaration
```cs
public System.Nullable<System.Int32> PreviousEmbeddedFileIndex { get; set; } 
```
## UnresolvedData Property {#unresolveddata}
Gets or sets the unresolved data for this field.
### Declaration
```cs
public string UnresolvedData { get; set; } 
```
## UnresolvedPreviousData Property {#unresolvedpreviousdata}
Gets or sets the unresolved previous data.
### Declaration
```cs
public string UnresolvedPreviousData { get; set; } 
```
