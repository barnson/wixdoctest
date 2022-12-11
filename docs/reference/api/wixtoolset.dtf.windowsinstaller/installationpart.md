---
custom_edit_url: null
toc_max_heading_level: 2
---
# InstallationPart Class
Subclasses of this abstract class represent an instance of a registered feature or component.
## Properties
| Property | Description |
| ------ | ----------- |
| [Product](#product) | Gets the product that this item is a part of. |
| [State](#state) | Gets the current installation state of the item. |
`WixToolset.Dtf.WindowsInstaller.dll` version `4.0.0-preview.1+7a4632adc0c7b1a363259abb4ed08b11ee3b2d87`
## Product Property {#product}
Gets the product that this item is a part of.
### Declaration
```cs
public ProductInstallation Product { get; set; } 
```
## State Property {#state}
Gets the current installation state of the item.
### Declaration
```cs
public InstallState State { get; set; } 
```
