---
custom_edit_url: null
toc_max_heading_level: 2
---
# ValidationErrorInfo Struct
Contains specific information about an error encountered by the «see M:WixToolset.Dtf.WindowsInstaller.View.Validate(WixToolset.Dtf.WindowsInstaller.Record)» , «see M:WixToolset.Dtf.WindowsInstaller.View.ValidateNew(WixToolset.Dtf.WindowsInstaller.Record)» , or «see M:WixToolset.Dtf.WindowsInstaller.View.ValidateFields(WixToolset.Dtf.WindowsInstaller.Record)» methods of the «see T:WixToolset.Dtf.WindowsInstaller.View» class.
## Properties
| Property | Description |
| ------ | ----------- |
| [Column](#column) | Gets the column containing the error, or null if the error applies to the whole row. |
| [Error](#error) | Gets the type of validation error encountered. |
`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Column Property {#column}
Gets the column containing the error, or null if the error applies to the whole row.
### Declaration
```cs
public string Column { get; set; } 
```
## Error Property {#error}
Gets the type of validation error encountered.
### Declaration
```cs
public ValidationError Error { get; set; } 
```
