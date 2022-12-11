---
custom_edit_url: null
toc_max_heading_level: 2
---
# DatabaseTableAttribute Class
Apply to a subclass of QRecord to indicate the name of the table the record type is to be used with.
## Properties
| Property | Description |
| ------ | ----------- |
| [Table](#table) | Gets or sets the table associated with the record type. |
### Remarks
If this attribute is not used on a record type, the default table name will be derived from the record type name. (An optional underscore suffix is stripped.)
`WixToolset.Dtf.WindowsInstaller.Linq.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Table Property {#table}
Gets or sets the table associated with the record type.
### Declaration
```cs
public string Table { get; set; } 
```
