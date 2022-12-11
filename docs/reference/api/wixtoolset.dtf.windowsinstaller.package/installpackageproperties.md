---
custom_edit_url: null
toc_max_heading_level: 2
---
# InstallPackageProperties Class
Accessor for getting and setting properties of the «see T:WixToolset.Dtf.WindowsInstaller.Package.InstallPackage» database.
## Properties
| Property | Description |
| ------ | ----------- |
| [Item](#item) | Gets or sets a property in the database. When getting a property that does not exist in the database, an empty string is returned. To remove a property from the database, set it to an empty string. |
`WixToolset.Dtf.WindowsInstaller.Package.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Item Property {#item}
Gets or sets a property in the database. When getting a property that does not exist in the database, an empty string is returned. To remove a property from the database, set it to an empty string.
### Declaration
```cs
public string Item { get; set; } 
```
### Remarks
This has the same results as direct SQL queries on the Property table; it's only meant to be a more convenient way of access.
