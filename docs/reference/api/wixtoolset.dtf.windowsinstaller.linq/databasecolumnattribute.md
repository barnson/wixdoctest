---
custom_edit_url: null
toc_max_heading_level: 2
---
# DatabaseColumnAttribute Class
Apply to a property on a subclass of QRecord to indicate the name of the column the property is to be associated with.
## Properties
| Property | Description |
| ------ | ----------- |
| [Column](#column) | Gets or sets the column associated with the record property. |
### Remarks
If this attribute is not used on a property, the default column name will be the same as the property name.
`WixToolset.Dtf.WindowsInstaller.Linq.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Column Property {#column}
Gets or sets the column associated with the record property.
### Declaration
```cs
public string Column { get; set; } 
```
